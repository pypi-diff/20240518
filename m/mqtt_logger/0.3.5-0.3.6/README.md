# Comparing `tmp/mqtt_logger-0.3.5.tar.gz` & `tmp/mqtt_logger-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_logger-0.3.5.tar", max compression
+gzip compressed data, was "mqtt_logger-0.3.6.tar", max compression
```

## Comparing `mqtt_logger-0.3.5.tar` & `mqtt_logger-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2024-01-04 06:12:37.923694 mqtt_logger-0.3.5/LICENSE
--rw-r--r--   0        0        0     3786 2024-01-04 06:12:37.923694 mqtt_logger-0.3.5/README.md
--rw-r--r--   0        0        0       62 2024-01-04 06:12:37.923694 mqtt_logger-0.3.5/mqtt_logger/__init__.py
--rw-r--r--   0        0        0     3831 2024-01-04 06:12:37.923694 mqtt_logger-0.3.5/mqtt_logger/database.py
--rw-r--r--   0        0        0    10033 2024-01-04 06:12:37.923694 mqtt_logger-0.3.5/mqtt_logger/logger.py
--rw-r--r--   0        0        0      582 2024-01-04 06:12:37.923694 mqtt_logger-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 mqtt_logger-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-18 00:09:47.560278 mqtt_logger-0.3.6/LICENSE
+-rw-r--r--   0        0        0     4118 2024-05-18 00:09:47.560278 mqtt_logger-0.3.6/README.md
+-rw-r--r--   0        0        0      130 2024-05-18 00:09:47.560278 mqtt_logger-0.3.6/mqtt_logger/__init__.py
+-rw-r--r--   0        0        0     4583 2024-05-18 00:09:47.560278 mqtt_logger-0.3.6/mqtt_logger/database.py
+-rw-r--r--   0        0        0    10905 2024-05-18 00:09:47.560278 mqtt_logger-0.3.6/mqtt_logger/logger.py
+-rw-r--r--   0        0        0      582 2024-05-18 00:09:47.560278 mqtt_logger-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 mqtt_logger-0.3.6/PKG-INFO
```

### Comparing `mqtt_logger-0.3.5/LICENSE` & `mqtt_logger-0.3.6/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 Blake Haydon
+Copyright © 2024 Blake Haydon
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mqtt_logger-0.3.5/README.md` & `mqtt_logger-0.3.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # MQTT to SQLite Logger
 
 [![PyPI version](https://badge.fury.io/py/mqtt-logger.svg)](https://badge.fury.io/py/mqtt-logger)
-[![Python package](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-package.yml/badge.svg)](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-package.yml)
+[![Unit Tests](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-test.yml/badge.svg)](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-test.yml)
 [![Upload Python Package](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-publish.yml)
+[![codecov](https://codecov.io/github/Blake-Haydon/mqtt-logger/graph/badge.svg?token=8PA3F5RWXA)](https://codecov.io/github/Blake-Haydon/mqtt-logger)
 
 ## Table of Contents
 
 - [MQTT to SQLite Logger](#mqtt-to-sqlite-logger)
   - [Table of Contents](#table-of-contents)
   - [Description](#description)
   - [Installation](#installation)
@@ -29,16 +30,15 @@
 pip install mqtt-logger
 ```
 
 ## Example Usage
 
 ### Recording MQTT Messages
 
-This example records messages to the `test/#` topic using a public MQTT broker. It will record for 10 seconds. If you
-are using a private broker, you may need to set the `username` and `password` parameters.
+This example records messages to the `test/#` topic using a public MQTT broker. It will record for 10 seconds. If you are using a private broker, you may need to set the `username` and `password` parameters.
 
 <!-- poetry run python examples/10s_recording.py -->
 
 _Example recorder taken from [examples/10s_recording.py](examples/10s_recording.py)_
 
 ```python
 import mqtt_logger
@@ -47,14 +47,23 @@
 
 # Initalise mqtt recorder object
 rec = mqtt_logger.Recorder(
     sqlite_database_path=os.path.join(os.path.dirname(__file__), "MQTT_log.db"),
     topics=["test/#"],
     broker_address="broker.hivemq.com",
     verbose=True,
+
+    ## Uncomment for TLS connection
+    # port=8883,
+	# use_tls=True,
+	# tls_insecure=False,
+
+    ## Uncomment for username and password
+    # username="username",
+    # password="password",
 )
 
 # Start the logger, wait 10 seconds and stop the logger
 rec.start()
 time.sleep(10)
 rec.stop()
 ```
```

### Comparing `mqtt_logger-0.3.5/mqtt_logger/database.py` & `mqtt_logger-0.3.6/mqtt_logger/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import sqlite3
 import time
+import logging
+from typing import Optional, List, Set
 
 
 LOGGER_TABLE_NAME = "LOG"
 RUNS_TABLE_NAME = "RUN"
 
 
 def create_tables(con: sqlite3.Connection):
     """Initialise the database by creating the necessary tables for logging."""
     cur = con.cursor()
 
-    query = f"""
+    log_query = f"""
         CREATE TABLE {LOGGER_TABLE_NAME}
         (ID                         INTEGER             PRIMARY KEY,
         RUN_ID                      INTEGER             NOT NULL,
         UNIX_TIME                   DECIMAL(15,6)       NOT NULL,
         TOPIC                       VARCHAR             NOT NULL,
         MESSAGE                     BLOB                NOT NULL);
     """
-    cur.execute(query)
 
-    query = f"""
+    run_query = f"""
         CREATE TABLE {RUNS_TABLE_NAME}
         (ID                         INTEGER             PRIMARY KEY,
         START_UNIX_TIME             DECIMAL(15,6)       NOT NULL,
         END_UNIX_TIME               DECIMAL(15,6));
         """
-    cur.execute(query)
+
+    cur.execute(log_query)
+    cur.execute(run_query)
 
     # Commit database tables to the database
     con.commit()
 
 
 def tables_exist(con: sqlite3.Connection) -> bool:
-    """Checks if the LOG table exists in the database."""
+    """Checks if the `LOG` and `RUN` tables exists in the database."""
     cur = con.cursor()
 
     log_query = f"""
         SELECT name FROM sqlite_master WHERE type='table' AND name='{LOGGER_TABLE_NAME}'
         """
 
     run_query = f"""
@@ -51,83 +54,105 @@
         raise RuntimeError(
             "Tables must exist together. Check that the database is either empty or contains both tables."
         )
 
     return log_exists  # or run_exists could be used as they are equivalent
 
 
-def start_run_entry(con: sqlite3.Connection) -> int:
+def start_run_entry(con: sqlite3.Connection) -> Optional[int]:
     """Inserts a run entry into the database. Returns the run id."""
     cur = con.cursor()
 
     query = f"""
         INSERT INTO {RUNS_TABLE_NAME}
         (START_UNIX_TIME)
         VALUES ({time.time()})
         """
 
     cur.execute(query)
     con.commit()
     return cur.lastrowid
 
 
-def stop_run_entry(con: sqlite3.Connection, run_id: int):
+def stop_run_entry(con: sqlite3.Connection, run_id: Optional[int]):
     """Inserts a run entry into the database. Returns the run id."""
     cur = con.cursor()
 
     query = f"""
         UPDATE {RUNS_TABLE_NAME}
         SET END_UNIX_TIME = {time.time()}
         WHERE ROWID = {run_id}
         """
 
+    if run_id is None:
+        raise ValueError("run_id must be provided.")
     cur.execute(query)
     con.commit()
 
 
-def insert_log_entry(con: sqlite3.Connection, topic: str, message: bytes, run_id: int):
+def insert_log_entry(con: sqlite3.Connection, topic: str, message: bytes, run_id: Optional[int]):
     """Inserts a log entry into the database."""
     cur = con.cursor()
 
     query = f"""
         INSERT INTO {LOGGER_TABLE_NAME}
         (UNIX_TIME, TOPIC, MESSAGE, RUN_ID)
         VALUES ({time.time()}, ?, ?, ?)
         """
 
     # NOTE: time.time() will not be the correct time if the system clock is reset (i.e on a raspberry pi)
+    if run_id is None:
+        raise ValueError("run_id must be provided.")
+
+    if run_id not in run_ids(con):
+        logging.warning(
+            f"Run ID {run_id} does not exist in the database, please call start_run_entry() first."
+        )
+
     cur.execute(query, (topic, message, run_id))
     con.commit()
 
 
-def retrieve_log_entries(con: sqlite3.Connection, patterns: [str] = None) -> list:
+def retrieve_log_entries(con: sqlite3.Connection, patterns: Optional[List[str]] = None) -> list:
     """Retrieves all log entries from the database."""
     cur = con.cursor()
 
     query = f"""
         SELECT UNIX_TIME, TOPIC, MESSAGE FROM {LOGGER_TABLE_NAME}
         """
 
     if patterns is not None:
-        query += " WHERE " + " OR ".join([f"TOPIC LIKE '{pattern}' " for pattern in patterns])
+        query += " WHERE " + " OR ".join(
+            [f"TOPIC LIKE '{pattern}' " for pattern in patterns]
+        )
 
     # Convert list of tuples into a list of dicts
     return [
         {
             "unix_time": record[0],
             "topic": record[1],
             "message": record[2],
         }
         for record in cur.execute(query).fetchall()
     ]
 
 
 def start_time(con: sqlite3.Connection) -> float:
-    """Retrieves the logging start time"""
+    """Retrieves the logging start time."""
     cur = con.cursor()
 
     # TODO: Implement this with run numbers
     query = f"""
         SELECT MIN(UNIX_TIME) FROM {LOGGER_TABLE_NAME}
         """
 
     return cur.execute(query).fetchone()[0]
+
+
+def run_ids(con: sqlite3.Connection) -> Set[int]:
+    """Retrieves all run ids from the database."""
+    cur = con.cursor()
+
+    query = f"""SELECT ID FROM {RUNS_TABLE_NAME}"""
+
+    all_run_ids = cur.execute(query).fetchall()
+    return {record[0] for record in all_run_ids}
```

### Comparing `mqtt_logger-0.3.5/mqtt_logger/logger.py` & `mqtt_logger-0.3.6/mqtt_logger/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 import sqlite3
 import asyncio
-
+from typing import Optional, List
 import paho.mqtt.client as mqtt
 from rich.logging import RichHandler
 
 from mqtt_logger.database import (
     create_tables,
     insert_log_entry,
     start_run_entry,
     stop_run_entry,
     tables_exist,
     retrieve_log_entries,
     start_time,
 )
 
-# Set logging to output all info by default
+# Set logging to output only warnings default
 logging.basicConfig(
     format="%(message)s",
     level=logging.WARNING,
     handlers=[RichHandler()],
 )
 
 
@@ -30,14 +30,20 @@
     ----------
     sqlite_database_path : str
         Filepath to the *.db file that sqlite uses to save data
     topics : List(str)
         A list containing the topic strings that are to be subscribed to
     broker_address : str
         The IP address that the MQTT broker lives on
+    port : int
+        The port of the MQTT broker
+    use_tls : bool
+        Setup a TLS connection with the MQTT broker
+    tls_insecure : bool
+        Allow invalid certificates
     verbose : bool
         Set logging output to INFO level if True
     username : str
         Username for mqtt broker
     password : str
         Password for mqtt broker
 
@@ -54,19 +60,22 @@
     _client : paho.mqtt.client
         MQTT client that connects to the broker and receives the messages
     """
 
     def __init__(
         self,
         sqlite_database_path: str = "MQTT_log.db",
-        topics: list = ["#"],
+        topics: List[str] = ["#"],
         broker_address: str = "localhost",
+        port: int = 1883,
+        use_tls: bool = False,
+        tls_insecure: bool = False,
         verbose: bool = False,
-        username: str = None,
-        password: str = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
     ):
         # If set to verbose print info messages
         if verbose:
             logging.getLogger().setLevel(logging.INFO)
 
         # Connect to sqlite database
         # check_same_thread needs to be false as the MQTT callbacks run on a different thread
@@ -90,17 +99,20 @@
         # Do not start logging when object is created (wait for start method)
         self._recording = False
 
         # Connect to MQTT broker
         self._client = mqtt.Client()
         self._client.on_connect = self._on_connect
         self._client.on_message = self._on_message
+        if use_tls:
+            self._client.tls_set()
+            self._client.tls_insecure_set(tls_insecure)
         if username is not None and password is not None:
             self._client.username_pw_set(username, password)
-        self._client.connect(broker_address)
+        self._client.connect(broker_address, port=port)
         self._client.loop_start()  # Threaded execution loop
 
     def _on_connect(self, client, userdata, flags, rc):
         """Callback function for MQTT broker on connection."""
 
         if rc == 0:
             logging.info("Connection Successful")
@@ -156,14 +168,20 @@
 
     Parameters
     ----------
     sqlite_database_path : str
         Filepath to the *.db file that sqlite uses to save data
     broker_address : str
         The IP address of the MQTT broker
+    port : int
+        The port of the MQTT broker
+    use_tls : bool
+        Setup a TLS connection with the MQTT broker
+    tls_insecure : bool
+        Allow invalid certificates
     verbose : bool
         Set logging output to INFO level if True
     username : str
         Username for mqtt broker
     password : str
         Password for mqtt broker
 
@@ -178,17 +196,20 @@
     """
 
     def __init__(
         self,
         sqlite_database_path: str = "MQTT_log.db",
         broker_address: str = "localhost",
         topics: list = ["#"],
+        port: int = 1883,
+        use_tls: bool = False,
+        tls_insecure: bool = False,
         verbose: bool = False,
-        username: str = None,
-        password: str = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
     ):
         # If set to verbose print info messages
         if verbose:
             logging.getLogger().setLevel(logging.INFO)
 
         sql_patterns = []
         for topic in topics:
@@ -202,18 +223,21 @@
         self._log_data = retrieve_log_entries(self._con, sql_patterns)
 
         # Save the async task so that it can be cancelled
         self._publish_task = None
 
         # Connect to MQTT broker
         self._client = mqtt.Client()
+        if use_tls:
+            self._client.tls_set()
+            self._client.tls_insecure_set(tls_insecure)
         if username is not None and password is not None:
             self._client.username_pw_set(username, password)
         self._client.on_connect = self._on_connect
-        self._client.connect(broker_address)
+        self._client.connect(broker_address, port=port)
         self._client.loop_start()  # Threaded execution loop
 
     def _on_connect(self, client, userdata, flags, rc):
         """Callback function for MQTT broker on connection."""
 
         if rc == 0:
             logging.info("Connection Successful")
```

### Comparing `mqtt_logger-0.3.5/pyproject.toml` & `mqtt_logger-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 license = "MIT"
 name = "mqtt_logger"
-version = "0.3.5"
+version = "0.3.6"
 description = "Python based MQTT to SQLite3 logger"
 authors = ["Blake Haydon <blake.a.haydon@gmail.com>"]
 readme = "README.md"
 keywords = ["MQTT", "SQLite3"]
 homepage = "https://github.com/Blake-Haydon/mqtt-logger"
 
 [tool.poetry.dependencies]
```

### Comparing `mqtt_logger-0.3.5/PKG-INFO` & `mqtt_logger-0.3.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt_logger
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python based MQTT to SQLite3 logger
 Home-page: https://github.com/Blake-Haydon/mqtt-logger
 License: MIT
 Keywords: MQTT,SQLite3
 Author: Blake Haydon
 Author-email: blake.a.haydon@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -19,16 +19,17 @@
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: rich (>=12.0.0,<13.0.0)
 Description-Content-Type: text/markdown
 
 # MQTT to SQLite Logger
 
 [![PyPI version](https://badge.fury.io/py/mqtt-logger.svg)](https://badge.fury.io/py/mqtt-logger)
-[![Python package](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-package.yml/badge.svg)](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-package.yml)
+[![Unit Tests](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-test.yml/badge.svg)](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-test.yml)
 [![Upload Python Package](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Blake-Haydon/mqtt-logger/actions/workflows/python-publish.yml)
+[![codecov](https://codecov.io/github/Blake-Haydon/mqtt-logger/graph/badge.svg?token=8PA3F5RWXA)](https://codecov.io/github/Blake-Haydon/mqtt-logger)
 
 ## Table of Contents
 
 - [MQTT to SQLite Logger](#mqtt-to-sqlite-logger)
   - [Table of Contents](#table-of-contents)
   - [Description](#description)
   - [Installation](#installation)
@@ -51,16 +52,15 @@
 pip install mqtt-logger
 ```
 
 ## Example Usage
 
 ### Recording MQTT Messages
 
-This example records messages to the `test/#` topic using a public MQTT broker. It will record for 10 seconds. If you
-are using a private broker, you may need to set the `username` and `password` parameters.
+This example records messages to the `test/#` topic using a public MQTT broker. It will record for 10 seconds. If you are using a private broker, you may need to set the `username` and `password` parameters.
 
 <!-- poetry run python examples/10s_recording.py -->
 
 _Example recorder taken from [examples/10s_recording.py](examples/10s_recording.py)_
 
 ```python
 import mqtt_logger
@@ -69,14 +69,23 @@
 
 # Initalise mqtt recorder object
 rec = mqtt_logger.Recorder(
     sqlite_database_path=os.path.join(os.path.dirname(__file__), "MQTT_log.db"),
     topics=["test/#"],
     broker_address="broker.hivemq.com",
     verbose=True,
+
+    ## Uncomment for TLS connection
+    # port=8883,
+	# use_tls=True,
+	# tls_insecure=False,
+
+    ## Uncomment for username and password
+    # username="username",
+    # password="password",
 )
 
 # Start the logger, wait 10 seconds and stop the logger
 rec.start()
 time.sleep(10)
 rec.stop()
 ```
```


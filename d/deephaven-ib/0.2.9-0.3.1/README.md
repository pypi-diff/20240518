# Comparing `tmp/deephaven_ib-0.2.9.tar.gz` & `tmp/deephaven_ib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/deephaven-ib/deephaven-ib/dist/tmp_epp6scl/deephaven_ib-0.2.9.tar", last modified: Mon Aug  8 22:31:18 2022, max compression
+gzip compressed data, was "/home/runner/work/deephaven-ib/deephaven-ib/dist/.tmp-bld3v21f/deephaven_ib-0.3.1.tar", last modified: Fri May 17 21:59:36 2024, max compression
```

## Comparing `deephaven_ib-0.2.9.tar` & `deephaven_ib-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    29778 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    28728 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib/
--rw-r--r--   0 runner    (1001) docker     (121)    48077 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib/_internal/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_internal/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_internal/short_rates.py
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_internal/tablewriter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4038 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_internal/threading.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_internal/trace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_query_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib/_tws/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_tws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7483 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_tws/contract_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    29545 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_tws/ib_type_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4459 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_tws/order_id_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_tws/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)    44033 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/_tws/tws_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-08-08 22:31:04.000000 deephaven_ib-0.2.9/src/deephaven_ib/time.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    29778 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-08 22:31:18.000000 deephaven_ib-0.2.9/src/deephaven_ib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    33326 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32275 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib/
+-rw-r--r--   0 runner    (1001) docker     (127)    50242 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_internal/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_internal/short_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_internal/tablewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_internal/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_internal/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib/_tws/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_tws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_tws/contract_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29502 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_tws/ib_type_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_tws/order_id_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_tws/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44397 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/_tws/tws_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-17 21:59:25.000000 deephaven_ib-0.3.1/src/deephaven_ib/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    33326 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 21:59:36.000000 deephaven_ib-0.3.1/src/deephaven_ib.egg-info/top_level.txt
```

### Comparing `deephaven_ib-0.2.9/LICENSE` & `deephaven_ib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven_ib-0.2.9/PKG-INFO` & `deephaven_ib-0.3.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,10 @@
-Metadata-Version: 2.1
-Name: deephaven_ib
-Version: 0.2.9
-Summary: An Interactive Brokers integration for Deephaven
-Home-page: https://github.com/deephaven-examples/deephaven-ib
-Author: David R. (Chip) Kent IV
-Author-email: chipkent@deephaven.io
-Project-URL: Deephaven, https://deephaven.io
-Project-URL: Deephaven GitHub, https://github.com/deephaven/deephaven-core
-Project-URL: GitHub Issues, https://github.com/deephaven-examples/deephaven-ib/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Topic :: Database :: Database Engines/Servers
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # deephaven-ib
 
-![Deephaven Data Labs Logo](docs/assets/Deephaven-Logo-Wordmark-Community-OnLight.png)
+![Deephaven Data Labs Logo](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/Deephaven-Logo-Wordmark-Community-OnLight.png)
 
 ![Build CI](https://github.com/deephaven-examples/deephaven-ib/actions/workflows/build-and-publish.yml/badge.svg?branch=main)
 
 An [Interactive Brokers](https://www.interactivebrokers.com/) integration for [Deephaven](https://deephaven.io).
 
 [Interactive Brokers](https://www.interactivebrokers.com/) is a very popular brokerage in the quantitative finance world,
 with about $200B of customer equity.  Quants and hedge funds often choose [Interactive Brokers](https://www.interactivebrokers.com/) because of its low trading costs and API that facilitates automated trading.  With low minimum account balances, 
@@ -57,15 +34,15 @@
 * Bonds
 * Foreign Exchange (Forex or FX)
 * Cryptocurrency
 * Contracts for Differences (CFDs)
 * Warrants
 * Commodities
 
-![Overview Image](docs/assets/overview.png)
+![Overview Image](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/overview.png)
 
 **WARNING: Automated trading can go horribly wrong very quickly.  Verify your code on a paper trading account before 
 unleashing trading on an account where money can be lost.  If you think this can not happen to you, read
 [The Rise and Fall of Knight Capital](https://medium.com/dataseries/the-rise-and-fall-of-knight-capital-buy-high-sell-low-rinse-and-repeat-ae17fae780f6).
 The [Setup](#setup) section shows configurations to prevent accidental trade submission.**
 
 For more details, see:
@@ -135,15 +112,15 @@
     * `ticks_string`: real-time tick market data of string values requested via `request_market_data`.
     * `ticks_efp`: real-time tick market data of exchange for physical (EFP) values requested via `request_market_data`.
     * `ticks_generic`: real-time tick market data of generic floating point values requested via `request_market_data`.
     * `ticks_option_computation`: real-time tick market data of option computations requested via `request_market_data`.
     * `ticks_trade`: real-time tick market data of trade prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
     * `ticks_bid_ask`: real-time tick market data of bid and ask prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
     * `ticks_mid_point`: real-time tick market data of mid-point prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
-    * `bars_historical`: historical price bars requested via `request_bars_historical`.
+    * `bars_historical`: historical price bars requested via `request_bars_historical`.  Real-time bars change as new data arrives.
     * `bars_realtime`: real-time price bars requested via `request_bars_realtime`.
 * Order Management System (OMS)
     * `orders_submitted`: submitted orders **FOR THE THE CLIENT'S ID**.  A client ID of 0 contains manually entered orders.  Automatically populated.
     * `orders_status`: order statuses.  Automatically populated.
     * `orders_completed`: completed orders.  Automatically populated.
     * `orders_exec_details`: order execution details.  Automatically populated.
     * `orders_exec_commission_report`: order execution commission report.  Automatically populated.
@@ -154,142 +131,207 @@
 
 You may want to combine data from other sources with your IB data.  [Deephaven](https://deephaven.io) can load data from:
 * [CSV](https://deephaven.io/core/docs/how-to-guides/csv-import/)
 * [Parquet](https://deephaven.io/core/docs/how-to-guides/parquet-flat/) 
 * [Kafka](https://deephaven.io/core/docs/how-to-guides/kafka-topics/).  
 See the [Deephaven Documentation](https://deephaven.io/core/docs) for details.
 
-Files placed in the `./docker/data/` directory are visible in the Docker container at `/data/`.  
-See [Access your file system with Docker data volumes](https://deephaven.io/core/docs/conceptual/docker-data-volumes/) for details.
-
 # Run deephaven-ib
 
-Follow these steps to run a [Deephaven](https://deephaven.io) plus [Interactive Brokers](https://interactivebrokers.com) system. 
+Follow these steps to run a [Deephaven](https://deephaven.io) plus [Interactive Brokers](https://interactivebrokers.com) system.
 
-`<deephaven_version>` is the version of [Deephaven](https://deephaven.io) to run (e.g., `0.11.0`).  A list of available versions 
-can be found on the [Deephaven Releases GitHub page](https://github.com/deephaven/deephaven-core/releases).  
-Version `0.11.0` or higher must be used.
+These instructions produce a virtual environment with [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), [Deephaven](https://deephaven.io), and `ibapi` installed.
+For more details on using pip-installed Deephaven, see [Deephaven's Installation Guide for pip](https://deephaven.io/core/docs/tutorials/pip-install/).
 
-**Windows users need to run the commands in WSL.**
+| :exclamation:  Windows users _must_ run these commands in WSL.   |
+|------------------------------------------------------------------|
 
-## Setup
+## Setup IB
 To setup and configure the system:
 
-1) Follow the [Deephaven Quick Start Guide](https://deephaven.io/core/docs/tutorials/quickstart/) to get [Deephaven](https://deephaven.io) running.  
 1) Follow the [TWS Installation Instructions](https://www.interactivebrokers.com/en/trading/tws.php) to get [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) running.
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-1) In [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), click on the gear in the
-upper right corner.  ![](docs/assets/config-gear.png)  
+2) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
+3) In [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), click on the gear in the
+upper right corner.  ![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/config-gear.png)  
   In `API->Settings`, make sure:
 
     * "Enable ActiveX and Socket Clients" is selected.
     * "Allow connections from localhost only" is not selected.
     * "Read-Only API" is selected if you want to prevent trade submission from [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).  
         
     Also, note the "Socket port" value.  It is needed when connecting [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
-    ![](docs/assets/config-api.png)
-1) [For Paper Trading] Log into the [Interactive Brokers Web Interface](https://interactivebrokers.com/).
-1) [For Paper Trading] In the [Interactive Brokers Web Interface](https://interactivebrokers.com/), navigate to `Account->Settings->Paper Trading Account` and make sure that "Share real-time market data subscriptions with paper trading account?" is set to true.
+    ![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/config-api.png)
+4) [For Paper Trading] Log into the [Interactive Brokers Web Interface](https://interactivebrokers.com/).
+5) [For Paper Trading] In the [Interactive Brokers Web Interface](https://interactivebrokers.com/), navigate to `Account->Settings->Paper Trading Account` and make sure that "Share real-time market data subscriptions with paper trading account?" is set to true.
+6) Once [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) is launched (see [below](#launch)), accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
+![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/allow-connections.png)
 
+## Virtual Environment
 
-## Launch
-To launch the system:
+Interactive Brokers does not make their Python wheels available via PyPI, and the wheels are not redistributable.
+As a result, installing [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) requires a Python script to build the wheels locally before installation.
+The script installs `deephaven-ib`, `ibapi`, and `deephaven` into the environment.
 
-### Launch with Docker
+To keep your development environment clean, the script creates a virtual environment for [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
+Follow the directions below to build and activate the virtual environment using the [./dhib_env.py](./dhib_env.py) script.
 
-This is the most tested way to launch.
+An existing virtual environment can be used with the `--create_venv false` and `--path_venv <path>` options.
 
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-2) Accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
-![](docs/assets/allow-connections.png)
-3) Create a directory for your data and scripts
-    ```bash
-    mkdir data
-    ```
-4) Launch the system (Option 1):
-    * On Mac:
+If you prefer to install directly into your system Python without a virtual environment, 
+you can use the `--use_venv false` option to [./dhib_env.py](./dhib_env.py).
+
+
+### Build the Virtual Environment
+
+1) Install Java 17 and set the appropriate `JAVA_HOME` environment variable.    
+2) Check out [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib)
     ```bash
     git clone git@github.com:deephaven-examples/deephaven-ib.git
-    cd deephaven-ib/docker/dev/build.sh
-    # Set jvm_args to the desired JVM memory for Deephaven
-    docker run -it -v data:/data -p 10000:10000 deephaven-examples/deephaven-ib:dev python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
     ```
-    * On other platforms:
+3) Change to the deephaven-ib directory:
     ```bash
-    # Set jvm_args to the desired JVM memory for Deephaven
-    docker run -it -v data:/data -p 10000:10000 ghcr.io/deephaven-examples/deephaven-ib python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
+    cd deephaven-ib
     ```
-5) Launch the system and execute a custom script (Option 2):
-    * On Mac:
-    ```bash
-    git clone git@github.com:deephaven-examples/deephaven-ib.git
-    cd deephaven-ib/docker/dev/build.sh
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    cp path/to/your_script.py data/your_script.py
-    docker run -it -v data:/data -p 10000:10000 deephaven-examples/deephaven-ib:dev python3 -i /data/your_script.py
-    ```
-    * On other platforms:
+4) Build a [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) virtual environment:
+
+   First, install the dependencies needed to run the script:
     ```bash
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    cp path/to/your_script.py data/your_script.py
-    docker run -it -v data:/data -p 10000:10000 ghcr.io/deephaven-examples/deephaven-ib python3 -i /data/your_script.py
+    python3 -m pip install -r requirements_dhib_env.txt
     ```
-7) Launch the [Deephaven IDE](https://github.com/deephaven/deephaven-core/blob/main/README.md#run-deephaven-ide) by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in a browser.
 
-### Launch with a local installation (No Docker)
-
-> **_NOTE:_**  Deephaven pip install is not yet supported on all architectures.  This launch should work on Linux (AMD64 and ARM64) and Windows WSL.  It is not yet supported on Windows without WSL or Mac.  For these architectures, you should use the Docker installation.  As soon as Deephaven supports these architectures for pip, [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) will work.
-
-It is possible to use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) without docker, but this is a 
-new feature and has not been well tested.  To do this:
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-2) Accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
-![](docs/assets/allow-connections.png)
-3) Install `ibapi`:
+   To see all options:
     ```bash
-    # pip installed version of ibapi is too old.  You must download and install a more recent version.
-    curl -o ./api.zip "https://interactivebrokers.github.io/downloads/twsapi_macunix.1016.01.zip"
-    unzip api.zip
-    cd ./IBJts/source/pythonclient
-    python3 setup.py install
+    python3 ./dhib_env.py --help
     ```
-4) Install [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib):
+
+   To install the latest production release version of [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) from PyPi plus the release-specified `ibapi` and `deephaven` versions: 
     ```bash
-    pip3 install --upgrade pip setuptools wheel
-    pip3 install deephaven-ib
+    python3 ./dhib_env.py release
     ```
-5) Install Java 11 and set the appropriate `JAVA_HOME` environment variable.    
-6) Launch the system (Option 1):
+   
+   To install the latest development version of [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) from source plus the default `ibapi` and `deephaven` versions:
     ```bash
-    # Set jvm_args to the desired JVM memory for Deephaven
-    python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
+    python3 ./dhib_env.py dev
     ```
-7) Launch the system and execute a custom script (Option 2):
+
+   To create a venv for developing [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) in PyCharm: (This will not install `deephaven-ib`, but it will install the default `ibapi` and `deephaven` versions.)
     ```bash
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    python3 -i /data/your_script.py
+    python3 ./dhib_env.py dev --install_dhib false
     ```
-8) Launch the [Deephaven IDE](https://github.com/deephaven/deephaven-core/blob/main/README.md#run-deephaven-ide) by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in a browser.
-9) Use `host=localhost` for the hostname in the examples
+   
+5) In the logs, take note of where the virtual environment is located.  It will be in a directory like `./venv-<versiondetails>`.
+   
+### Activate the Virtual Environment
+
+To activate the virtual environment:
+```bash
+source ./venv-<versiondetails>/bin/activate
+```
+
+Once the virtual environment is activated, `python` and `pip` will use the virtual environment's Python and packages --
+including everything needed to run [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
+
+### Deactivate the Virtual Environment
+
+To deactivate the virtual environment:
+```bash
+deactivate
+```
+
+Once the virtual environment is deactivated, `python` and `pip` will use the system's Python and packages.
+[deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) will not be available.
+
 
 # Use deephaven-ib
 
-To use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), you will need to open the [Deephaven Web IDE](http://localhost:10000/ide/) 
-by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in your web browser.  The following commands
-can be executed in the console.
+To use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), you need to start a [Deephaven](https://deephaven.io) server and connect to 
+[IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
+You can optionally use the Deephaven IDE to visualize data and run queries.
+
+## Start Deephaven
+
+First, start a [Deephaven](https://deephaven.io) server.  This server will be used to process data and run queries.
+
+The documentation and examples here illustrate using Deephaven's [Pre-Shared Key (PSK) authentication](https://deephaven.io/core/docs/how-to-guides/authentication/auth-psk/)
+with the password `DeephavenRocks!`.  Other types of Deephaven authentication can also work.  
+See the [Deephaven Documentation](https://deephaven.io/core/docs/) for details.
+
+
+### Option 1: Use the `deephaven` command
+
+The easiest way to start a deephaven server is using `deephaven` on the command line.
+The `deephaven` command was added to the virtual environment when it was created.
+It is available in [Deephaven](https://deephaven.io) versions `>= 0.34.0`.
+
+This command will start a deephaven server with 4GB of memory and the password `DeephavenRocks!`.
+It will also automatically open the Deephaven IDE in a web browser.
+
+```bash
+source ./venv-<versiondetails>/bin/activate
+deephaven server --jvm-args "-Xmx4g -Dauthentication.psk=DeephavenRocks! -Dstorage.path=~/.deephaven"
+```
+
+
+### Option 2: Use a Python script
+
+An alternative way to launch a deephaven server is to use a Python script.  This works with all versions of 
+[Deephaven](https://deephaven.io) and can be used to populate the server with queries.  
+See [Deephaven's Installation Guide for pip](https://deephaven.io/core/docs/tutorials/pip-install/) for more details on 
+running [Deephaven](https://deephaven.io) this way.
+
+To start Python with the virtual environment, run:
+```bash
+source ./venv-<versiondetails>/bin/activate
+python
+```
+
+Once Python is running, you can start a deephaven server with the following script:
+```python
+import os
+from time import sleep
+from deephaven_server import Server
+
+_server = Server(port=10000, jvm_args=['-Xmx4g','-Dauthentication.psk=DeephavenRocks!','-Dstorage.path=' + os.path.expanduser('~/.deephaven')])
+_server.start()
+
+# You can insert queries here
+
+# Keep the server running
+while True:
+    sleep(1)
+```
+> :warning: These deephaven server commands **must** be run before importing `deephaven` or `deephaven_ib`.
+
+At the indicated place in the script, you can put queries that you want to run when the server starts.  
+This could be code to conenct to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), request data, analyze data, visualize data, or trade.  
+See the examples below for more details.
+
+
+## Launch the Deephaven IDE
+
+Once the Deephaven server is started, you can launch the Deephaven IDE.
+If you used the `deephaven` command to start the server, the Deephaven IDE will automatically open in your web browser.
+
+The Deephaven IDE is a web-based interface for working with Deephaven.
+Once in the IDE, you can run queries, create notebooks, and visualize data.
+You can also run all of the example code below and the more complex examples in [./examples](./examples).
+
+To launch the Deephaven IDE, navigate to [http://localhost:10000/ide/](http://localhost:10000/ide/) in your web browser.
+Chrome, Edge, Chrome-based, and Firefox browsers are supported.  Safari is not supported.
+How you authenticate will depend upon how authentication is configured.  
+In the examples here, you will use the password `DeephavenRocks!`.
+
 
 ## Connect to TWS
 
 All [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) sessions need to first create a client for interacting 
 with [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
 
-`host` is the computer to connect to.  When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) inside
+`host` is the computer to connect to.  When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) locally, `host` is usually set to `localhost`.
+When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) inside
 of Docker, `host` should be set to `host.docker.internal`.  
 
 `port` is the network port [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 communicates on.  This value can be found in the [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 settings.  By default, production trading uses port 7496, and paper trading uses port 7497.  See [Setup](#setup) and [TWS Initial Setup](https://interactivebrokers.github.io/tws-api/initial_setup.html) for more details.
 
 `read_only` is a boolean value that is used to enable trading.  By default `read_only=True`, preventing trading.  Use `read_only=False` to enable trading.
@@ -305,36 +347,36 @@
 * `OrderIdStrategy.BASIC` - Request a new order ID from TWS every time one is needed.  Does not retry, so it may deadlock if TWS does not respond.
 * `OrderIdStrategy.INCREMENT` - Use the initial order ID sent by TWS and increment the value upon every request.  This is fast, but it may fail for multiple, concurrent sessions connected to TWS.
 
 For a read-write session that allows trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=False)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=False)
 client.connect()
 ```
 
 For a read-only session that does not allow trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=True)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=True)
 client.connect()
 ```
 
 For a read-only financial advisor (FA) session that does not allow trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=True, is_fa=True)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=True, is_fa=True)
 client.connect()
 ```
 
 After `client.connect()` is called, TWS requires that the connection be accepted.
-![](docs/assets/accept-connection.png)
+![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/accept-connection.png)
 
 ## Get data
 
 [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) data is stored in
 the [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) client as two dictionaries of tables:
 * `tables` contains the tables most users will want.  
 * `tables_raw` contains raw [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
@@ -465,16 +507,16 @@
 contract.secType = "STK"
 contract.currency = "USD"
 contract.exchange = "SMART"
 
 rc = client.get_registered_contract(contract)
 print(contract)
 
-start = to_datetime("2021-01-01T00:00:00 NY")
-end = to_datetime("2021-01-10T00:00:00 NY")
+start = "2021-01-01T00:00:00 ET"
+end = "2021-01-10T00:00:00 ET"
 client.request_news_historical(rc, start=start, end=end)
 
 client.request_news_article(provider_code="BRFUPDN", article_id="BRFUPDN$107d53ea")
 ```
 
 [./examples/example_all_functionality.py](./examples/example_all_functionality.py) illustrates requesting
 news data.
@@ -573,15 +615,15 @@
 bars_dia = bars_realtime.where("Symbol=`DIA`")
 bars_spy = bars_realtime.where("Symbol=`SPY`")
 bars_joined = bars_dia.view(["Timestamp", "TimestampEnd", "Dia=Close"]) \
     .natural_join(bars_spy, on="TimestampEnd", joins="Spy=Close") \
     .update("Ratio = Dia/Spy")
 ```
 
-![DIA SPY Ratio](docs/assets/dia_spy_ratio.png)
+![DIA SPY Ratio](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/dia_spy_ratio.png)
 
 ## Plotting
 
 [Deephaven](https://deephaven.io) has very powerful plotting functionality for both static and real-time data.
 The example below plots the bid and ask prices of `AAPL` for every tick in the market.
 
 For more details, see the [Deephaven Coummunity Core Documentation](https://deephaven.io/core/docs/).
@@ -608,15 +650,15 @@
 from deephaven.plot import Figure
 
 plot_aapl = Figure().plot_xy("Bid",  t=ticks_bid_ask, x="ReceiveTime", y="BidPrice") \
     .plot_xy("Ask",  t=ticks_bid_ask, x="ReceiveTime", y="AskPrice") \
     .show()
 ```
 
-![AAPL Bid Ask](docs/assets/aapl_bid_ask.png)
+![AAPL Bid Ask](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/aapl_bid_ask.png)
 
 ## Help!
 
 ### Error Table
 
 [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) logs all [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 errors to the `errors` table.  This table should be monitored when using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
@@ -650,12 +692,28 @@
 If you can not solve your problems through either the `errors` table or through logging, you can try:
 
 * [deephaven-ib API Documentation](https://deephaven-examples.github.io/deephaven-ib/)
 * [Interactive Brokers Support](https://www.interactivebrokers.com/en/support/individuals.php)
 * [Gitter: A relaxed chat room about all things Deephaven](https://gitter.im/deephaven/deephaven)
 * [Deephaven Community Slack](https://deephaven.io/slack)
 
+### `Takes N positional arguments but M were given`
+
+You may encounter an error that looks like: `Takes N positional arguments but M were given`.  
+If you see a problem like this, your `ibapi` version does not match the version needed by [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).  
+The [`ibapi` version in PyPI](https://pypi.org/project/ibapi/) is ancient and appears to have been abandoned by [Interactive Brokers](https://www.interactivebrokers.com/).  
+Currently [Interactive Brokers](https://www.interactivebrokers.com/) is delivering `ibapi` either via the [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) 
+download or via git. 
+
+To check your `ibapi` version:
+```python
+import ibapi
+print(ibapi.__version__)
+```
+
+The `ibapi` API is very unstable.  If your version does not exactly match the version needed by [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), 
+you will need to install the correct version.  Regenerate your virtual environment as described above.
 
 # Examples
 
 Examples can be found in [./examples](./examples).
```

### Comparing `deephaven_ib-0.2.9/README.md` & `deephaven_ib-0.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,33 @@
+Metadata-Version: 2.1
+Name: deephaven_ib
+Version: 0.3.1
+Summary: An Interactive Brokers integration for Deephaven
+Home-page: https://github.com/deephaven-examples/deephaven-ib
+Author: David R. (Chip) Kent IV
+Author-email: chipkent@deephaven.io
+Project-URL: Deephaven, https://deephaven.io
+Project-URL: Deephaven GitHub, https://github.com/deephaven/deephaven-core
+Project-URL: GitHub Issues, https://github.com/deephaven-examples/deephaven-ib/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # deephaven-ib
 
-![Deephaven Data Labs Logo](docs/assets/Deephaven-Logo-Wordmark-Community-OnLight.png)
+![Deephaven Data Labs Logo](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/Deephaven-Logo-Wordmark-Community-OnLight.png)
 
 ![Build CI](https://github.com/deephaven-examples/deephaven-ib/actions/workflows/build-and-publish.yml/badge.svg?branch=main)
 
 An [Interactive Brokers](https://www.interactivebrokers.com/) integration for [Deephaven](https://deephaven.io).
 
 [Interactive Brokers](https://www.interactivebrokers.com/) is a very popular brokerage in the quantitative finance world,
 with about $200B of customer equity.  Quants and hedge funds often choose [Interactive Brokers](https://www.interactivebrokers.com/) because of its low trading costs and API that facilitates automated trading.  With low minimum account balances, 
@@ -34,15 +57,15 @@
 * Bonds
 * Foreign Exchange (Forex or FX)
 * Cryptocurrency
 * Contracts for Differences (CFDs)
 * Warrants
 * Commodities
 
-![Overview Image](docs/assets/overview.png)
+![Overview Image](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/overview.png)
 
 **WARNING: Automated trading can go horribly wrong very quickly.  Verify your code on a paper trading account before 
 unleashing trading on an account where money can be lost.  If you think this can not happen to you, read
 [The Rise and Fall of Knight Capital](https://medium.com/dataseries/the-rise-and-fall-of-knight-capital-buy-high-sell-low-rinse-and-repeat-ae17fae780f6).
 The [Setup](#setup) section shows configurations to prevent accidental trade submission.**
 
 For more details, see:
@@ -112,15 +135,15 @@
     * `ticks_string`: real-time tick market data of string values requested via `request_market_data`.
     * `ticks_efp`: real-time tick market data of exchange for physical (EFP) values requested via `request_market_data`.
     * `ticks_generic`: real-time tick market data of generic floating point values requested via `request_market_data`.
     * `ticks_option_computation`: real-time tick market data of option computations requested via `request_market_data`.
     * `ticks_trade`: real-time tick market data of trade prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
     * `ticks_bid_ask`: real-time tick market data of bid and ask prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
     * `ticks_mid_point`: real-time tick market data of mid-point prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
-    * `bars_historical`: historical price bars requested via `request_bars_historical`.
+    * `bars_historical`: historical price bars requested via `request_bars_historical`.  Real-time bars change as new data arrives.
     * `bars_realtime`: real-time price bars requested via `request_bars_realtime`.
 * Order Management System (OMS)
     * `orders_submitted`: submitted orders **FOR THE THE CLIENT'S ID**.  A client ID of 0 contains manually entered orders.  Automatically populated.
     * `orders_status`: order statuses.  Automatically populated.
     * `orders_completed`: completed orders.  Automatically populated.
     * `orders_exec_details`: order execution details.  Automatically populated.
     * `orders_exec_commission_report`: order execution commission report.  Automatically populated.
@@ -131,142 +154,207 @@
 
 You may want to combine data from other sources with your IB data.  [Deephaven](https://deephaven.io) can load data from:
 * [CSV](https://deephaven.io/core/docs/how-to-guides/csv-import/)
 * [Parquet](https://deephaven.io/core/docs/how-to-guides/parquet-flat/) 
 * [Kafka](https://deephaven.io/core/docs/how-to-guides/kafka-topics/).  
 See the [Deephaven Documentation](https://deephaven.io/core/docs) for details.
 
-Files placed in the `./docker/data/` directory are visible in the Docker container at `/data/`.  
-See [Access your file system with Docker data volumes](https://deephaven.io/core/docs/conceptual/docker-data-volumes/) for details.
-
 # Run deephaven-ib
 
-Follow these steps to run a [Deephaven](https://deephaven.io) plus [Interactive Brokers](https://interactivebrokers.com) system. 
+Follow these steps to run a [Deephaven](https://deephaven.io) plus [Interactive Brokers](https://interactivebrokers.com) system.
 
-`<deephaven_version>` is the version of [Deephaven](https://deephaven.io) to run (e.g., `0.11.0`).  A list of available versions 
-can be found on the [Deephaven Releases GitHub page](https://github.com/deephaven/deephaven-core/releases).  
-Version `0.11.0` or higher must be used.
+These instructions produce a virtual environment with [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), [Deephaven](https://deephaven.io), and `ibapi` installed.
+For more details on using pip-installed Deephaven, see [Deephaven's Installation Guide for pip](https://deephaven.io/core/docs/tutorials/pip-install/).
 
-**Windows users need to run the commands in WSL.**
+| :exclamation:  Windows users _must_ run these commands in WSL.   |
+|------------------------------------------------------------------|
 
-## Setup
+## Setup IB
 To setup and configure the system:
 
-1) Follow the [Deephaven Quick Start Guide](https://deephaven.io/core/docs/tutorials/quickstart/) to get [Deephaven](https://deephaven.io) running.  
 1) Follow the [TWS Installation Instructions](https://www.interactivebrokers.com/en/trading/tws.php) to get [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) running.
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-1) In [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), click on the gear in the
-upper right corner.  ![](docs/assets/config-gear.png)  
+2) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
+3) In [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), click on the gear in the
+upper right corner.  ![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/config-gear.png)  
   In `API->Settings`, make sure:
 
     * "Enable ActiveX and Socket Clients" is selected.
     * "Allow connections from localhost only" is not selected.
     * "Read-Only API" is selected if you want to prevent trade submission from [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).  
         
     Also, note the "Socket port" value.  It is needed when connecting [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
-    ![](docs/assets/config-api.png)
-1) [For Paper Trading] Log into the [Interactive Brokers Web Interface](https://interactivebrokers.com/).
-1) [For Paper Trading] In the [Interactive Brokers Web Interface](https://interactivebrokers.com/), navigate to `Account->Settings->Paper Trading Account` and make sure that "Share real-time market data subscriptions with paper trading account?" is set to true.
+    ![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/config-api.png)
+4) [For Paper Trading] Log into the [Interactive Brokers Web Interface](https://interactivebrokers.com/).
+5) [For Paper Trading] In the [Interactive Brokers Web Interface](https://interactivebrokers.com/), navigate to `Account->Settings->Paper Trading Account` and make sure that "Share real-time market data subscriptions with paper trading account?" is set to true.
+6) Once [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) is launched (see [below](#launch)), accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
+![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/allow-connections.png)
 
+## Virtual Environment
 
-## Launch
-To launch the system:
+Interactive Brokers does not make their Python wheels available via PyPI, and the wheels are not redistributable.
+As a result, installing [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) requires a Python script to build the wheels locally before installation.
+The script installs `deephaven-ib`, `ibapi`, and `deephaven` into the environment.
 
-### Launch with Docker
+To keep your development environment clean, the script creates a virtual environment for [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
+Follow the directions below to build and activate the virtual environment using the [./dhib_env.py](./dhib_env.py) script.
 
-This is the most tested way to launch.
+An existing virtual environment can be used with the `--create_venv false` and `--path_venv <path>` options.
 
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-2) Accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
-![](docs/assets/allow-connections.png)
-3) Create a directory for your data and scripts
-    ```bash
-    mkdir data
-    ```
-4) Launch the system (Option 1):
-    * On Mac:
+If you prefer to install directly into your system Python without a virtual environment, 
+you can use the `--use_venv false` option to [./dhib_env.py](./dhib_env.py).
+
+
+### Build the Virtual Environment
+
+1) Install Java 17 and set the appropriate `JAVA_HOME` environment variable.    
+2) Check out [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib)
     ```bash
     git clone git@github.com:deephaven-examples/deephaven-ib.git
-    cd deephaven-ib/docker/dev/build.sh
-    # Set jvm_args to the desired JVM memory for Deephaven
-    docker run -it -v data:/data -p 10000:10000 deephaven-examples/deephaven-ib:dev python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
     ```
-    * On other platforms:
+3) Change to the deephaven-ib directory:
     ```bash
-    # Set jvm_args to the desired JVM memory for Deephaven
-    docker run -it -v data:/data -p 10000:10000 ghcr.io/deephaven-examples/deephaven-ib python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
+    cd deephaven-ib
     ```
-5) Launch the system and execute a custom script (Option 2):
-    * On Mac:
-    ```bash
-    git clone git@github.com:deephaven-examples/deephaven-ib.git
-    cd deephaven-ib/docker/dev/build.sh
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    cp path/to/your_script.py data/your_script.py
-    docker run -it -v data:/data -p 10000:10000 deephaven-examples/deephaven-ib:dev python3 -i /data/your_script.py
-    ```
-    * On other platforms:
+4) Build a [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) virtual environment:
+
+   First, install the dependencies needed to run the script:
     ```bash
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    cp path/to/your_script.py data/your_script.py
-    docker run -it -v data:/data -p 10000:10000 ghcr.io/deephaven-examples/deephaven-ib python3 -i /data/your_script.py
+    python3 -m pip install -r requirements_dhib_env.txt
     ```
-7) Launch the [Deephaven IDE](https://github.com/deephaven/deephaven-core/blob/main/README.md#run-deephaven-ide) by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in a browser.
 
-### Launch with a local installation (No Docker)
-
-> **_NOTE:_**  Deephaven pip install is not yet supported on all architectures.  This launch should work on Linux (AMD64 and ARM64) and Windows WSL.  It is not yet supported on Windows without WSL or Mac.  For these architectures, you should use the Docker installation.  As soon as Deephaven supports these architectures for pip, [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) will work.
-
-It is possible to use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) without docker, but this is a 
-new feature and has not been well tested.  To do this:
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-2) Accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
-![](docs/assets/allow-connections.png)
-3) Install `ibapi`:
+   To see all options:
     ```bash
-    # pip installed version of ibapi is too old.  You must download and install a more recent version.
-    curl -o ./api.zip "https://interactivebrokers.github.io/downloads/twsapi_macunix.1016.01.zip"
-    unzip api.zip
-    cd ./IBJts/source/pythonclient
-    python3 setup.py install
+    python3 ./dhib_env.py --help
     ```
-4) Install [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib):
+
+   To install the latest production release version of [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) from PyPi plus the release-specified `ibapi` and `deephaven` versions: 
     ```bash
-    pip3 install --upgrade pip setuptools wheel
-    pip3 install deephaven-ib
+    python3 ./dhib_env.py release
     ```
-5) Install Java 11 and set the appropriate `JAVA_HOME` environment variable.    
-6) Launch the system (Option 1):
+   
+   To install the latest development version of [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) from source plus the default `ibapi` and `deephaven` versions:
     ```bash
-    # Set jvm_args to the desired JVM memory for Deephaven
-    python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
+    python3 ./dhib_env.py dev
     ```
-7) Launch the system and execute a custom script (Option 2):
+
+   To create a venv for developing [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) in PyCharm: (This will not install `deephaven-ib`, but it will install the default `ibapi` and `deephaven` versions.)
     ```bash
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    python3 -i /data/your_script.py
+    python3 ./dhib_env.py dev --install_dhib false
     ```
-8) Launch the [Deephaven IDE](https://github.com/deephaven/deephaven-core/blob/main/README.md#run-deephaven-ide) by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in a browser.
-9) Use `host=localhost` for the hostname in the examples
+   
+5) In the logs, take note of where the virtual environment is located.  It will be in a directory like `./venv-<versiondetails>`.
+   
+### Activate the Virtual Environment
+
+To activate the virtual environment:
+```bash
+source ./venv-<versiondetails>/bin/activate
+```
+
+Once the virtual environment is activated, `python` and `pip` will use the virtual environment's Python and packages --
+including everything needed to run [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
+
+### Deactivate the Virtual Environment
+
+To deactivate the virtual environment:
+```bash
+deactivate
+```
+
+Once the virtual environment is deactivated, `python` and `pip` will use the system's Python and packages.
+[deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) will not be available.
+
 
 # Use deephaven-ib
 
-To use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), you will need to open the [Deephaven Web IDE](http://localhost:10000/ide/) 
-by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in your web browser.  The following commands
-can be executed in the console.
+To use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), you need to start a [Deephaven](https://deephaven.io) server and connect to 
+[IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
+You can optionally use the Deephaven IDE to visualize data and run queries.
+
+## Start Deephaven
+
+First, start a [Deephaven](https://deephaven.io) server.  This server will be used to process data and run queries.
+
+The documentation and examples here illustrate using Deephaven's [Pre-Shared Key (PSK) authentication](https://deephaven.io/core/docs/how-to-guides/authentication/auth-psk/)
+with the password `DeephavenRocks!`.  Other types of Deephaven authentication can also work.  
+See the [Deephaven Documentation](https://deephaven.io/core/docs/) for details.
+
+
+### Option 1: Use the `deephaven` command
+
+The easiest way to start a deephaven server is using `deephaven` on the command line.
+The `deephaven` command was added to the virtual environment when it was created.
+It is available in [Deephaven](https://deephaven.io) versions `>= 0.34.0`.
+
+This command will start a deephaven server with 4GB of memory and the password `DeephavenRocks!`.
+It will also automatically open the Deephaven IDE in a web browser.
+
+```bash
+source ./venv-<versiondetails>/bin/activate
+deephaven server --jvm-args "-Xmx4g -Dauthentication.psk=DeephavenRocks! -Dstorage.path=~/.deephaven"
+```
+
+
+### Option 2: Use a Python script
+
+An alternative way to launch a deephaven server is to use a Python script.  This works with all versions of 
+[Deephaven](https://deephaven.io) and can be used to populate the server with queries.  
+See [Deephaven's Installation Guide for pip](https://deephaven.io/core/docs/tutorials/pip-install/) for more details on 
+running [Deephaven](https://deephaven.io) this way.
+
+To start Python with the virtual environment, run:
+```bash
+source ./venv-<versiondetails>/bin/activate
+python
+```
+
+Once Python is running, you can start a deephaven server with the following script:
+```python
+import os
+from time import sleep
+from deephaven_server import Server
+
+_server = Server(port=10000, jvm_args=['-Xmx4g','-Dauthentication.psk=DeephavenRocks!','-Dstorage.path=' + os.path.expanduser('~/.deephaven')])
+_server.start()
+
+# You can insert queries here
+
+# Keep the server running
+while True:
+    sleep(1)
+```
+> :warning: These deephaven server commands **must** be run before importing `deephaven` or `deephaven_ib`.
+
+At the indicated place in the script, you can put queries that you want to run when the server starts.  
+This could be code to conenct to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), request data, analyze data, visualize data, or trade.  
+See the examples below for more details.
+
+
+## Launch the Deephaven IDE
+
+Once the Deephaven server is started, you can launch the Deephaven IDE.
+If you used the `deephaven` command to start the server, the Deephaven IDE will automatically open in your web browser.
+
+The Deephaven IDE is a web-based interface for working with Deephaven.
+Once in the IDE, you can run queries, create notebooks, and visualize data.
+You can also run all of the example code below and the more complex examples in [./examples](./examples).
+
+To launch the Deephaven IDE, navigate to [http://localhost:10000/ide/](http://localhost:10000/ide/) in your web browser.
+Chrome, Edge, Chrome-based, and Firefox browsers are supported.  Safari is not supported.
+How you authenticate will depend upon how authentication is configured.  
+In the examples here, you will use the password `DeephavenRocks!`.
+
 
 ## Connect to TWS
 
 All [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) sessions need to first create a client for interacting 
 with [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
 
-`host` is the computer to connect to.  When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) inside
+`host` is the computer to connect to.  When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) locally, `host` is usually set to `localhost`.
+When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) inside
 of Docker, `host` should be set to `host.docker.internal`.  
 
 `port` is the network port [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 communicates on.  This value can be found in the [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 settings.  By default, production trading uses port 7496, and paper trading uses port 7497.  See [Setup](#setup) and [TWS Initial Setup](https://interactivebrokers.github.io/tws-api/initial_setup.html) for more details.
 
 `read_only` is a boolean value that is used to enable trading.  By default `read_only=True`, preventing trading.  Use `read_only=False` to enable trading.
@@ -282,36 +370,36 @@
 * `OrderIdStrategy.BASIC` - Request a new order ID from TWS every time one is needed.  Does not retry, so it may deadlock if TWS does not respond.
 * `OrderIdStrategy.INCREMENT` - Use the initial order ID sent by TWS and increment the value upon every request.  This is fast, but it may fail for multiple, concurrent sessions connected to TWS.
 
 For a read-write session that allows trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=False)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=False)
 client.connect()
 ```
 
 For a read-only session that does not allow trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=True)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=True)
 client.connect()
 ```
 
 For a read-only financial advisor (FA) session that does not allow trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=True, is_fa=True)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=True, is_fa=True)
 client.connect()
 ```
 
 After `client.connect()` is called, TWS requires that the connection be accepted.
-![](docs/assets/accept-connection.png)
+![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/accept-connection.png)
 
 ## Get data
 
 [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) data is stored in
 the [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) client as two dictionaries of tables:
 * `tables` contains the tables most users will want.  
 * `tables_raw` contains raw [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
@@ -442,16 +530,16 @@
 contract.secType = "STK"
 contract.currency = "USD"
 contract.exchange = "SMART"
 
 rc = client.get_registered_contract(contract)
 print(contract)
 
-start = to_datetime("2021-01-01T00:00:00 NY")
-end = to_datetime("2021-01-10T00:00:00 NY")
+start = "2021-01-01T00:00:00 ET"
+end = "2021-01-10T00:00:00 ET"
 client.request_news_historical(rc, start=start, end=end)
 
 client.request_news_article(provider_code="BRFUPDN", article_id="BRFUPDN$107d53ea")
 ```
 
 [./examples/example_all_functionality.py](./examples/example_all_functionality.py) illustrates requesting
 news data.
@@ -550,15 +638,15 @@
 bars_dia = bars_realtime.where("Symbol=`DIA`")
 bars_spy = bars_realtime.where("Symbol=`SPY`")
 bars_joined = bars_dia.view(["Timestamp", "TimestampEnd", "Dia=Close"]) \
     .natural_join(bars_spy, on="TimestampEnd", joins="Spy=Close") \
     .update("Ratio = Dia/Spy")
 ```
 
-![DIA SPY Ratio](docs/assets/dia_spy_ratio.png)
+![DIA SPY Ratio](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/dia_spy_ratio.png)
 
 ## Plotting
 
 [Deephaven](https://deephaven.io) has very powerful plotting functionality for both static and real-time data.
 The example below plots the bid and ask prices of `AAPL` for every tick in the market.
 
 For more details, see the [Deephaven Coummunity Core Documentation](https://deephaven.io/core/docs/).
@@ -585,15 +673,15 @@
 from deephaven.plot import Figure
 
 plot_aapl = Figure().plot_xy("Bid",  t=ticks_bid_ask, x="ReceiveTime", y="BidPrice") \
     .plot_xy("Ask",  t=ticks_bid_ask, x="ReceiveTime", y="AskPrice") \
     .show()
 ```
 
-![AAPL Bid Ask](docs/assets/aapl_bid_ask.png)
+![AAPL Bid Ask](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/aapl_bid_ask.png)
 
 ## Help!
 
 ### Error Table
 
 [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) logs all [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 errors to the `errors` table.  This table should be monitored when using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
@@ -627,12 +715,28 @@
 If you can not solve your problems through either the `errors` table or through logging, you can try:
 
 * [deephaven-ib API Documentation](https://deephaven-examples.github.io/deephaven-ib/)
 * [Interactive Brokers Support](https://www.interactivebrokers.com/en/support/individuals.php)
 * [Gitter: A relaxed chat room about all things Deephaven](https://gitter.im/deephaven/deephaven)
 * [Deephaven Community Slack](https://deephaven.io/slack)
 
+### `Takes N positional arguments but M were given`
+
+You may encounter an error that looks like: `Takes N positional arguments but M were given`.  
+If you see a problem like this, your `ibapi` version does not match the version needed by [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).  
+The [`ibapi` version in PyPI](https://pypi.org/project/ibapi/) is ancient and appears to have been abandoned by [Interactive Brokers](https://www.interactivebrokers.com/).  
+Currently [Interactive Brokers](https://www.interactivebrokers.com/) is delivering `ibapi` either via the [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) 
+download or via git. 
+
+To check your `ibapi` version:
+```python
+import ibapi
+print(ibapi.__version__)
+```
+
+The `ibapi` API is very unstable.  If your version does not exactly match the version needed by [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), 
+you will need to install the correct version.  Regenerate your virtual environment as described above.
 
 # Examples
 
 Examples can be found in [./examples](./examples).
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/__init__.py` & `deephaven_ib-0.3.1/src/deephaven_ib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from enum import Enum
-from typing import Dict, List, Callable
+from typing import Union, Dict, List, Callable, Optional
+import json
+import datetime
+import numpy
+import pandas
 
 from deephaven.table import Table
-from deephaven.dtypes import DateTime
+from deephaven.constants import NULL_DOUBLE
+from deephaven.dtypes import Instant
 from ibapi.contract import Contract, ContractDetails
 from ibapi.order import Order
 
-from ._query_inputs import *
 from ._tws import IbTwsClient
 from ._tws.order_id_queue import OrderIdStrategy
-from .time import dh_to_ib_datetime
+from .time import to_ib_datetime
 
 __all__ = ["MarketDataType", "TickDataType", "BarDataType", "BarSize", "Duration", "OrderIdStrategy",
            "Request", "RegisteredContract", "IbSessionTws"]
 
 
 class MarketDataType(Enum):
     """Type of market data to use."""
@@ -399,15 +403,15 @@
         * **ticks_string**: real-time tick market data of string values requested via ``request_market_data``.
         * **ticks_efp**: real-time tick market data of exchange for physical (EFP) values requested via ``request_market_data``.
         * **ticks_generic**: real-time tick market data of generic floating point values requested via ``request_market_data``.
         * **ticks_option_computation**: real-time tick market data of option computations requested via ``request_market_data``.
         * **ticks_trade**: real-time tick market data of trade prices requested via ``request_tick_data_historical`` or ``request_tick_data_realtime``.
         * **ticks_bid_ask**: real-time tick market data of bid and ask prices requested via ``request_tick_data_historical`` or ``request_tick_data_realtime``.
         * **ticks_mid_point**: real-time tick market data of mid-point prices requested via ``request_tick_data_historical`` or ``request_tick_data_realtime``.
-        * **bars_historical**: historical price bars requested via ``request_bars_historical``.
+        * **bars_historical**: historical price bars requested via ``request_bars_historical``.  Real-time bars change as new data arrives.
         * **bars_realtime**: real-time price bars requested via ``request_bars_realtime``.
 
         ####
         # Order Management System (OMS)
         ####
 
         * **orders_submitted**: submitted orders **FOR THE THE CLIENT ID**.  A client ID of 0 contains manually entered orders.  Automatically populated.
@@ -421,15 +425,15 @@
     _port: int
     _client_id: int
     _read_only: bool
     _client: IbTwsClient
     _tables_raw: Dict[str, Table]
     _tables: Dict[str, Table]
 
-    def __init__(self, host: str = "", port: int = 7497, client_id: int = 0, download_short_rates: bool = True, order_id_strategy: OrderIdStrategy = OrderIdStrategy.RETRY, read_only: bool = True, is_fa: bool = False):
+    def __init__(self, host: str = "", port: int = 7497, client_id: int = 0, download_short_rates: bool = True, order_id_strategy: OrderIdStrategy = OrderIdStrategy.INCREMENT, read_only: bool = True, is_fa: bool = False):
         self._host = host
         self._port = port
         self._client_id = client_id
         self._read_only = read_only
         self._client = IbTwsClient(download_short_rates=download_short_rates, order_id_strategy=order_id_strategy, read_only=read_only, is_fa=is_fa)
         self._tables_raw = {f"raw_{k}": v for k, v in self._client.tables.items()}
         self._tables = dict(sorted(IbSessionTws._make_tables(self._tables_raw).items()))
@@ -542,14 +546,31 @@
                 else:
                     rst = rst.move_columns_up(["RequestId", "ReceiveTime", "Timestamp"])
             else:
                 rst = rst.move_columns_up(["RequestId", "ReceiveTime"])
 
             return rst
 
+        def deephaven_ib_float_value(s: Optional[str]) -> Optional[float]:
+            if not s:
+                return NULL_DOUBLE
+
+            try:
+                return float(s)
+            except ValueError:
+                return NULL_DOUBLE
+
+        def deephaven_ib_parse_note(note:str, key:str) -> Optional[str]:
+            dict = json.loads(note)
+
+            if key in dict:
+                return dict[key]
+
+            return None
+
         return {
             "requests": tables_raw["raw_requests"] \
                 .move_columns_up(["RequestId", "ReceiveTime"]),
             "errors": tables_raw["raw_errors"] \
                 .natural_join(tables_raw["raw_requests"] \
                              .drop_columns("Note").rename_columns("RequestTime=ReceiveTime"), on="RequestId") \
                 .move_columns_up(["RequestId", "ReceiveTime"]),
@@ -566,61 +587,62 @@
             "accounts_managed": tables_raw["raw_accounts_managed"] \
                 .select_distinct("Account"),
             "accounts_positions": tables_raw["raw_accounts_positions"] \
                 .last_by(["RequestId", "Account", "ModelCode", "ContractId"]) \
                 .move_columns_up(["RequestId", "ReceiveTime"]),
             "accounts_overview": tables_raw["raw_accounts_overview"] \
                 .last_by(["RequestId", "Account", "Currency", "Key"]) \
-                .update("DoubleValue = (double)__deephaven_ib_float_value.apply(Value)") \
+                .update("DoubleValue = (double)deephaven_ib_float_value(Value)") \
                 .move_columns_up(["RequestId", "ReceiveTime"]),
             "accounts_summary": tables_raw["raw_accounts_summary"] \
                 .natural_join(tables_raw["raw_requests"], on="RequestId", joins="Note") \
-                .update("GroupName=(String)__deephaven_ib_parse_note.apply(new String[]{Note,`groupName`})") \
+                .update("GroupName=(String)deephaven_ib_parse_note(Note,`groupName`)") \
                 .drop_columns("Note") \
-                .update("DoubleValue = (double)__deephaven_ib_float_value.apply(Value)") \
+                .update("DoubleValue = (double)deephaven_ib_float_value(Value)") \
                 .last_by(["RequestId", "GroupName", "Account", "Tag"]) \
                 .move_columns_up(["RequestId", "ReceiveTime", "GroupName"]),
             "accounts_pnl": tables_raw["raw_accounts_pnl"] \
                 .natural_join(tables_raw["raw_requests"], on="RequestId", joins="Note") \
                 .update([
-                    "Account=(String)__deephaven_ib_parse_note.apply(new String[]{Note,`account`})",
-                    "ModelCode=(String)__deephaven_ib_parse_note.apply(new String[]{Note,`model_code`})"]) \
+                    "Account=(String)deephaven_ib_parse_note(Note,`account`)",
+                    "ModelCode=(String)deephaven_ib_parse_note(Note,`model_code`)"]) \
                 .move_columns_up(["RequestId", "ReceiveTime", "Account", "ModelCode"]) \
                 .drop_columns("Note") \
                 .last_by("RequestId"),
             "contracts_matching": tables_raw["raw_contracts_matching"] \
                 .natural_join(tables_raw["raw_requests"], on="RequestId", joins="Pattern=Note") \
                 .move_columns_up(["RequestId", "ReceiveTime", "Pattern"]) \
-                .update("Pattern=(String)__deephaven_ib_parse_note.apply(new String[]{Pattern,`pattern`})"),
+                .update("Pattern=(String)deephaven_ib_parse_note(Pattern,`pattern`)"),
             "market_rules": tables_raw["raw_market_rules"].select_distinct(["MarketRuleId", "LowEdge", "Increment"]),
             "news_bulletins": tables_raw["raw_news_bulletins"],
             "news_providers": tables_raw["raw_news_providers"] \
                 .drop_columns("ReceiveTime"),
             "news_articles": tables_raw["raw_news_articles"] \
                 .move_columns_up(["RequestId", "ReceiveTime"]),
             "news_historical": tables_raw["raw_news_historical"] \
                 .natural_join(tables_raw["raw_requests"], on="RequestId", joins=["ContractId","SecType","Symbol","LocalSymbol"]) \
                 .move_columns_up(["RequestId", "ReceiveTime", "Timestamp", "ContractId", "SecType", "Symbol",
                                "LocalSymbol"]),
             "orders_completed": tables_raw["raw_orders_completed"] \
                 .move_columns_up(["ReceiveTime", "OrderId", "ClientId", "PermId", "ParentId"]),
             "orders_exec_commission_report": tables_raw["raw_orders_exec_commission_report"],
             "orders_exec_details": tables_raw["raw_orders_exec_details"] \
-                .move_columns_up(["RequestId", "ReceiveTime", "Timestamp", "ExecId", "AcctNumber"]),
+                .move_columns_up(["RequestId", "ReceiveTime", "Timestamp", "ExecId", "AcctNumber"]) \
+                .rename_columns("Account=AcctNumber"),
             # The status on raw_orders_submitted is buggy, so using the status from raw_orders_status
             "orders_submitted": tables_raw["raw_orders_submitted"] \
                 .last_by("PermId") \
                 .drop_columns("Status") \
                 .natural_join(tables_raw["raw_orders_status"].last_by("PermId"), on="PermId", joins="Status")
                 .move_columns_up(["ReceiveTime", "Account", "ModelCode", "PermId", "ClientId", "OrderId", "ParentId",
                                "Status"]),
             "orders_status": tables_raw["raw_orders_status"] \
                 .last_by("PermId") \
                 .move_columns_up(["ReceiveTime", "PermId", "ClientId", "OrderId", "ParentId"]),
-            "bars_historical": annotate_ticks(tables_raw["raw_bars_historical"]),
+            "bars_historical": annotate_ticks(tables_raw["raw_bars_historical"]).last_by(["RequestId", "Timestamp", "ContractId"]),
             "bars_realtime": annotate_ticks(tables_raw["raw_bars_realtime"]),
             "ticks_efp": annotate_ticks(tables_raw["raw_ticks_efp"]),
             "ticks_generic": annotate_ticks(tables_raw["raw_ticks_generic"]),
             "ticks_mid_point": annotate_ticks(tables_raw["raw_ticks_mid_point"]),
             "ticks_option_computation": annotate_ticks(tables_raw["raw_ticks_option_computation"]),
             "ticks_price": annotate_ticks(tables_raw["raw_ticks_price"]),
             "ticks_size": annotate_ticks(tables_raw["raw_ticks_size"]),
@@ -666,16 +688,20 @@
             A contract that has been registered with deephaven-ib.
 
         Raises:
               Exception: problem executing action.
         """
 
         self._assert_connected()
-        cd = self._client.contract_registry.request_contract_details_blocking(contract)
-        return RegisteredContract(query_contract=contract, contract_details=cd)
+
+        try:
+            cd = self._client.contract_registry.request_contract_details_blocking(contract)
+            return RegisteredContract(query_contract=contract, contract_details=cd)
+        except Exception as e:
+            raise Exception(f"Error getting registered contract: contract={contract} {e}")
 
     def request_contracts_matching(self, pattern: str) -> Request:
         """Request contracts matching a pattern.  Results are returned in the ``contracts_matching`` table.
 
         Args:
             pattern (str): pattern to search for.  Can include part of a ticker or part of the company name.
 
@@ -753,25 +779,27 @@
 
     ####################################################################################################################
     ####################################################################################################################
     ## News
     ####################################################################################################################
     ####################################################################################################################
 
-    def request_news_historical(self, contract: RegisteredContract, start: DateTime, end: DateTime,
+    def request_news_historical(self, contract: RegisteredContract,
+                                start: Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp],
+                                end: Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp],
                                 provider_codes: List[str] = None, total_results: int = 100) -> List[Request]:
         """ Request historical news for a contract.  Results are returned in the ``news_historical`` table.
 
         Registered contracts that are associated with multiple contract details produce multiple requests.
 
         Args:
             contract (RegisteredContract): contract data is requested for
             provider_codes (List[str]): a list of provider codes.  By default, all subscribed codes are used.
-            start (DateTime): marks the (exclusive) start of the date range.
-            end (DateTime): marks the (inclusive) end of the date range.
+            start (Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp]): marks the (exclusive) start of the date range.  See https://deephaven.io/core/pydoc/code/deephaven.time.html#deephaven.time.to_j_instant for supported inputs.
+            end (Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp]): marks the (inclusive) end of the date range.  See https://deephaven.io/core/pydoc/code/deephaven.time.html#deephaven.time.to_j_instant for supported inputs.
             total_results (int): the maximum number of headlines to fetch (1 - 300)
 
         Returns:
             All of the requests created by the action.
 
         Raises:
               Exception: problem executing action.
@@ -787,16 +815,16 @@
 
         for cd in contract.contract_details:
             req_id = self._client.request_id_manager.next_id()
             self._client.log_request(req_id, "HistoricalNews", cd.contract,
                                      {"provider_codes": provider_codes, "start": start, "end": end,
                                       "total_results": total_results})
             self._client.reqHistoricalNews(reqId=req_id, conId=cd.contract.conId, providerCodes=pc,
-                                           startDateTime=dh_to_ib_datetime(start, sub_sec=False),
-                                           endDateTime=dh_to_ib_datetime(end, sub_sec=False),
+                                           startDateTime=to_ib_datetime(start, sub_sec=False),
+                                           endDateTime=to_ib_datetime(end, sub_sec=False),
                                            totalResults=total_results, historicalNewsOptions=[])
             requests.append(Request(request_id=req_id))
 
         return requests
 
     def request_news_article(self, provider_code: str, article_id: str) -> Request:
         """ Request the text of a news article.  Results are returned in the ``news_articles`` table.
@@ -895,24 +923,24 @@
         """
 
         self._assert_connected()
         self._client.cancelMktData(reqId=req_id)
 
     def request_bars_historical(self, contract: RegisteredContract,
                                 duration: Duration, bar_size: BarSize, bar_type: BarDataType,
-                                end: DateTime = None,
+                                end: Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp] = None,
                                 market_data_type: MarketDataType = MarketDataType.FROZEN,
                                 keep_up_to_date: bool = True) -> List[Request]:
         """Requests historical bars for a contract.  Results are returned in the ``bars_historical`` table.
 
         Registered contracts that are associated with multiple contract details produce multiple requests.
 
         Args:
             contract (RegisteredContract): contract data is requested for
-            end (DateTime): Ending timestamp of the requested data.
+            end (Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp]): Ending timestamp of the requested data.  See https://deephaven.io/core/pydoc/code/deephaven.time.html#deephaven.time.to_j_instant for supported inputs.
             duration (Duration): Duration of data being requested by the query.
             bar_size (BarSize): Size of the bars that will be returned.
             bar_type (BarDataType): Type of bars that will be returned.
             market_data_type (MarketDataType): Type of market data to return after the close.
             keep_up_to_date (bool): True to continuously update bars
 
         Returns:
@@ -933,15 +961,15 @@
                                          "duration": duration,
                                          "bar_size": bar_size,
                                          "bar_type": bar_type,
                                          "market_data_type": market_data_type,
                                          "keep_up_to_date": keep_up_to_date,
                                      })
             self._client.reqHistoricalData(reqId=req_id, contract=cd.contract,
-                                           endDateTime=dh_to_ib_datetime(end, sub_sec=False),
+                                           endDateTime=to_ib_datetime(end, sub_sec=False),
                                            durationStr=duration.value, barSizeSetting=bar_size.value,
                                            whatToShow=bar_type.name, useRTH=(market_data_type == MarketDataType.FROZEN),
                                            formatDate=2, keepUpToDate=keep_up_to_date, chartOptions=[])
             requests.append(Request(request_id=req_id))
 
         return requests
 
@@ -1046,26 +1074,27 @@
         """
 
         self._assert_connected()
         self._client.cancelTickByTickData(reqId=req_id)
 
     def request_tick_data_historical(self, contract: RegisteredContract,
                                      tick_type: TickDataType, number_of_ticks: int,
-                                     start: DateTime = None, end: DateTime = None,
+                                     start: Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp] = None,
+                                     end: Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp] = None,
                                      market_data_type: MarketDataType = MarketDataType.FROZEN,
                                      ignore_size: bool = False) -> List[Request]:
         """Requests historical tick-by-tick data. Results are returned in the ``ticks_trade``, ``ticks_bid_ask``,
         and ``ticks_mid_point`` tables.
 
         Registered contracts that are associated with multiple contract details produce multiple requests.
 
         Args:
             contract (RegisteredContract): contract data is requested for
-            start (DateTime): marks the (exclusive) start of the date range.
-            end (DateTime): marks the (inclusive) end of the date range.
+            start (Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp]): marks the (exclusive) start of the date range.  See https://deephaven.io/core/pydoc/code/deephaven.time.html#deephaven.time.to_j_instant for supported inputs.
+            end (Union[None, Instant, int, str, datetime.datetime, numpy.datetime64, pandas.Timestamp]): marks the (inclusive) end of the date range.  See https://deephaven.io/core/pydoc/code/deephaven.time.html#deephaven.time.to_j_instant for supported inputs.
             tick_type (TickDataType): Type of market data to return.
             number_of_ticks (int): Number of historical ticks to request.
             market_data_type (MarketDataType): Type of market data to return after the close.
             ignore_size (bool): should size values be ignored.
 
         Returns:
             All of the requests created by this action.
@@ -1088,16 +1117,16 @@
                                       "end": end,
                                       "tick_type": tick_type,
                                       "number_of_ticks": number_of_ticks,
                                       "market_data_type": market_data_type,
                                       "ignore_size": ignore_size,
                                       })
             self._client.reqHistoricalTicks(reqId=req_id, contract=cd.contract,
-                                            startDateTime=dh_to_ib_datetime(start, sub_sec=False),
-                                            endDateTime=dh_to_ib_datetime(end, sub_sec=False),
+                                            startDateTime=to_ib_datetime(start, sub_sec=False),
+                                            endDateTime=to_ib_datetime(end, sub_sec=False),
                                             numberOfTicks=number_of_ticks, whatToShow=what_to_show,
                                             useRth=market_data_type.value,
                                             ignoreSize=ignore_size, miscOptions=[])
             requests.append(Request(request_id=req_id))
 
         return requests
 
@@ -1144,15 +1173,15 @@
 
         Raises:
               Exception: problem executing action.
         """
 
         self._assert_connected()
         self._assert_read_write()
-        self._client.cancelOrder(orderId=order_id)
+        self._client.cancelOrder(orderId=order_id, manualCancelOrderTime="")
 
     def order_cancel_all(self) -> None:
         """Cancel all open orders.
 
         Returns:
             None
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_internal/error_codes.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_internal/error_codes.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         10089: "Requested market data requires additional subscription for API.See link in 'Market Data Connections' dialog for more details.",
         10147: "OrderId that needs to be cancelled is not found.",
         10168: "Requested market data is not subscribed.Delayed market data is not enabled.",
         10172: "Failed to request news article: No data available",
         10187: "Failed to request historical ticks",
         10189: "Failed to request tick-by-tick data",
         10190: "Maxnumber of tick-by-tick requests has been reached.",
+        10311: "This order will be directly routed to NYSE. Direct routed orders may result in higher trade fees. Restriction is specified in Precautionary Settings of Global Configuration/API.",
     }
 
     for k, v in overrides.items():
         if k not in error_messages:
             error_messages[k] = v
             error_notes[k] = ""
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_internal/short_rates.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_internal/short_rates.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         else:
             self.file.write(f"{self.source}|{line}\n")
 
 
 def load_short_rates() -> Table:
     """Downloads the short rates from the IB FTP site and returns them as a table."""
 
-    host: str = "ftp3.interactivebrokers.com"
+    # See: https://www.ibkrguides.com/kb/article-2024.htm
+    host: str = "ftp2.interactivebrokers.com"
     user: str = "shortstock"
 
     with ftplib.FTP(host=host, user=user) as ftp, IBFtpWriter() as p:
         try:
             files = ftp.nlst("*.txt")
 
             for file in files:
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_internal/tablewriter.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_internal/tablewriter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functionality for creating Deephaven tables."""
 
 import logging
-from typing import List, Any, Sequence, Union, Set
+from typing import List, Any, Sequence, Optional, Set
 import collections
 
-from deephaven.time import now
+from deephaven.time import dh_now
 import jpy
 from deephaven import DynamicTableWriter
 from deephaven.table import Table
 from deephaven import dtypes
 from deephaven.dtypes import DType
 import decimal
 from decimal import Decimal
@@ -30,15 +30,15 @@
         TableWriter._check_for_duplicate_names(names)
         self.names = names
         self.types = types
         self._receive_time = receive_time
 
         if receive_time:
             self.names.insert(0, "ReceiveTime")
-            self.types.insert(0, dtypes.DateTime)
+            self.types.insert(0, dtypes.Instant)
 
         col_defs = {name: type for name, type in zip(names, types)}
         self._dtw = DynamicTableWriter(col_defs)
         self._string_indices = [i for (i, t) in enumerate(types) if t == dtypes.string]
 
     @staticmethod
     def _check_for_duplicate_names(names: List[str]) -> None:
@@ -63,27 +63,37 @@
         """Gets the table data is logged to."""
         return self._dtw.table
 
     def write_row(self, values: List) -> None:
         """Writes a row of data.  The input values may be modified."""
 
         if self._receive_time:
-            values.insert(0, now())
+            values.insert(0, dh_now())
 
         for i in range(len(values)):
             if  isinstance(values[i], decimal.Decimal): 
                 values[i] = float(values[i])
 
         self._check_logged_value_types(values)
 
         for i in self._string_indices:
             if values[i] == "":
                 values[i] = None
 
-        self._dtw.write_row(values)
+        try:
+            self._dtw.write_row(*values)
+        except Exception as e:
+            msg = f"Problem logging row:\n"
+
+            for i, v in enumerate(values):
+                msg += f"\t{i} {type(v)} {v}\n"
+
+            logging.error(msg)
+
+            raise e
 
 
 ArrayStringSet = jpy.get_type("io.deephaven.stringset.ArrayStringSet")
 
 _unmapped_values_already_logged:Set[str] = set()
 
 def map_values(value, map, default=lambda v: f"UNKNOWN({v})") -> Any:
@@ -100,23 +110,23 @@
         if msg not in _unmapped_values_already_logged:
             _unmapped_values_already_logged.add(msg)
             logging.error(msg)
 
         return default(value)
 
 
-def to_string_val(value) -> Union[str, None]:
+def to_string_val(value) -> Optional[str]:
     """ Converts a value to a string. """
 
     if value is None:
         return None
 
     return str(value)
 
 
-def to_string_set(value: Sequence) -> Union[ArrayStringSet, None]:
+def to_string_set(value: Sequence) -> Optional[ArrayStringSet]:
     """ Converts an iterable to a string set. """
 
     if value is None:
         return None
 
     return ArrayStringSet(list({to_string_val(v) for v in value}))
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_internal/threading.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_internal/threading.py`

 * *Files identical despite different names*

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_internal/trace.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_internal/trace.py`

 * *Files identical despite different names*

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_tws/contract_registry.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_tws/contract_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,17 @@
 
         with self._lock:
             if not req_id in self._requests_by_id:
                 return
 
             contract, event = self._requests_by_id[req_id]
             self._update_error(contract, req_id, error_string)
-            event.set()
+
+            if event:
+                event.set()
 
     def request_end(self, req_id: int) -> None:
         """Indicate that the request is over and all data has been received."""
 
         with self._lock:
             if not req_id in self._requests_by_id:
                 return
@@ -195,14 +197,17 @@
             None
         """
 
         key = str(contract)
 
         with self._lock:
             if key not in self._contracts:
+                if contract.conId < 0:
+                    raise Exception("Requesting contract details for a contract with a negative conId.  This is almost certainly a bug.  Please submit a bug report with this stack trace: {contract}")
+
                 req_id = self._client.request_id_manager.next_id()
                 req = (contract, event)
                 self._requests_by_id[req_id] = req
                 self._requests_by_key[key] = req
                 self._client.log_request(req_id, "ContractDetails", contract, None)
                 self._client.reqContractDetails(reqId=req_id, contract=contract)
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_tws/ib_type_logger.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_tws/ib_type_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Functionality for logging IB types to Deephaven tables."""
 
 import sys
-from typing import Any, List, Tuple, Dict, Callable, Union
+from typing import Any, List, Tuple, Dict, Callable, Optional
 
 from deephaven import dtypes
 
 from .._internal.tablewriter import map_values, to_string_val, to_string_set
-from ..time import unix_sec_to_dh_datetime, ib_to_dh_datetime
+from ..time import unix_sec_to_j_instant, ib_to_j_instant
 
 
 class IbComplexTypeLogger:
     """ Base class for logging complex IB types. """
 
     ib_type: str
     column_details: List[Tuple[str, Any, Callable]]
@@ -69,35 +69,41 @@
 
 
 ####
 
 def _details_contract() -> List[Tuple]:
     """ Details for logging Contract. """
 
-    def map_right(right: str) -> Union[str, None]:
+    def map_right(right: str) -> Optional[str]:
         if right == "?":
             return None
 
         return right
 
+    def map_multiplier(multiplier: str) -> float:
+        if multiplier is None or multiplier == "":
+            return 1.0
+
+        return float(multiplier)
+
     return [
         ("ContractId", dtypes.int64, lambda contract: contract.conId),
         ("SecId", dtypes.string, lambda contract: contract.secId),
         ("SecIdType", dtypes.string, lambda contract: contract.secIdType),
         ("SecType", dtypes.string, lambda contract: contract.secType),
         ("Symbol", dtypes.string, lambda contract: contract.symbol),
         ("LocalSymbol", dtypes.string, lambda contract: contract.localSymbol),
         ("TradingClass", dtypes.string, lambda contract: contract.tradingClass),
         ("Currency", dtypes.string, lambda contract: contract.currency),
         ("Exchange", dtypes.string, lambda contract: contract.exchange),
         ("PrimaryExchange", dtypes.string, lambda contract: contract.primaryExchange),
         ("LastTradeDateOrContractMonth", dtypes.string, lambda contract: contract.lastTradeDateOrContractMonth),
         ("Strike", dtypes.float64, lambda contract: float(contract.strike)),
         ("Right", dtypes.string, lambda contract: map_right(contract.right)),
-        ("Multiplier", dtypes.string, lambda contract: contract.multiplier),
+        ("Multiplier", dtypes.float64, lambda contract: map_multiplier(contract.multiplier)),
 
         # combos
         ("ComboLegsDescrip", dtypes.string, lambda contract: contract.comboLegsDescrip),
         ("ComboLegs", dtypes.StringSet, lambda contract: to_string_set(contract.comboLegs)),
         ("DeltaNeutralContract", dtypes.string, lambda contract: to_string_val(contract.deltaNeutralContract)),
     ]
 
@@ -106,15 +112,15 @@
 
 
 ####
 
 def _details_contract_details() -> List[Tuple]:
     """Details for logging ContractDetails."""
 
-    def map_null_int(value: int) -> Union[int, None]:
+    def map_null_int(value: int) -> Optional[int]:
 
         if value == 2147483647:
             return None
 
         return value
 
     def map_sec_id_list(value):
@@ -153,15 +159,15 @@
         ("CUSIP", dtypes.string, lambda cd: cd.cusip),
         ("Ratings", dtypes.string, lambda cd: cd.ratings),
         ("DescAppend", dtypes.string, lambda cd: cd.descAppend),
         ("BondType", dtypes.string, lambda cd: cd.bondType),
         ("CouponType", dtypes.string, lambda cd: cd.couponType),
         ("Callable", dtypes.bool_, lambda cd: cd.callable),
         ("Putable", dtypes.bool_, lambda cd: cd.putable),
-        ("Coupon", dtypes.int64, lambda cd: cd.coupon),
+        ("Coupon", dtypes.double, lambda cd: float(cd.coupon)),
         ("Convertible", dtypes.bool_, lambda cd: cd.convertible),
         ("Maturity", dtypes.string, lambda cd: cd.maturity),
         # TODO: convert date time?  Values are not provided in TWS, and the format is not documented. (https://github.com/deephaven-examples/deephaven-ib/issues/10)
         ("IssueDate", dtypes.string, lambda cd: cd.issueDate),
         # TODO: convert date time?  Values are not provided in TWS, and the format is not documented. (https://github.com/deephaven-examples/deephaven-ib/issues/10)
         ("NextOptionDate", dtypes.string, lambda cd: cd.nextOptionDate),
         # TODO: convert date time?  Values are not provided in TWS, and the format is not documented. (https://github.com/deephaven-examples/deephaven-ib/issues/10)
@@ -202,21 +208,21 @@
     def parse_timestamp(bd):
         if len(bd.date) is 8:
             # bd.date is a date string
             year = bd.date[0:4]
             month = bd.date[4:6]
             day = bd.date[6:]
             time_string = f"{year}{month}{day} 23:59:59"
-            return ib_to_dh_datetime(time_string)
+            return ib_to_j_instant(time_string)
         else:
             # bd.date is unix sec
-            return unix_sec_to_dh_datetime(int(bd.date))
+            return unix_sec_to_j_instant(int(bd.date))
 
     return [
-        ("Timestamp", dtypes.DateTime, parse_timestamp),
+        ("Timestamp", dtypes.Instant, parse_timestamp),
         ("Open", dtypes.float64, lambda bd: bd.open),
         ("High", dtypes.float64, lambda bd: bd.high),
         ("Low", dtypes.float64, lambda bd: bd.low),
         ("Close", dtypes.float64, lambda bd: bd.close),
         ("Volume", dtypes.float64, lambda bd: map_null(bd.volume)),
         ("BarCount", dtypes.int64, lambda bd: map_null(bd.barCount)),
         ("WAP", dtypes.float64, lambda bd: map_null(bd.wap)),
@@ -234,16 +240,16 @@
     def map_null(val):
         if val <= 0:
             return None
 
         return val
 
     return [
-        ("Timestamp", dtypes.DateTime, lambda bd: unix_sec_to_dh_datetime(bd.time)),
-        ("TimestampEnd", dtypes.DateTime, lambda bd: unix_sec_to_dh_datetime(bd.endTime)),
+        ("Timestamp", dtypes.Instant, lambda bd: unix_sec_to_j_instant(bd.time)),
+        ("TimestampEnd", dtypes.Instant, lambda bd: unix_sec_to_j_instant(bd.endTime)),
         ("Open", dtypes.float64, lambda bd: bd.open_),
         ("High", dtypes.float64, lambda bd: bd.high),
         ("Low", dtypes.float64, lambda bd: bd.low),
         ("Close", dtypes.float64, lambda bd: bd.close),
         ("Volume", dtypes.float64, lambda bd: map_null(bd.volume)),
         ("WAP", dtypes.float64, lambda bd: map_null(bd.wap)),
         ("Count", dtypes.int64, lambda bd: map_null(bd.count)),
@@ -323,15 +329,15 @@
         if not special_conditions:
             return None
 
         return to_string_set([map_values(v, special_conditions_codes) for v in "".join(special_conditions.split())])
 
 
     return [
-        ("Timestamp", dtypes.DateTime, lambda t: unix_sec_to_dh_datetime(t.time)),
+        ("Timestamp", dtypes.Instant, lambda t: unix_sec_to_j_instant(t.time)),
         ("Price", dtypes.float64, lambda t: t.price),
         ("Size", dtypes.float64, lambda t: t.size),
         *_include_details(_details_tick_attrib_last(), lambda t: t.tickAttribLast),
         ("Exchange", dtypes.string, lambda t: t.exchange),
         ("SpecialConditions", dtypes.StringSet, lambda t: map_special_conditions(t.specialConditions))
     ]
 
@@ -355,19 +361,19 @@
 
 ####
 
 def _details_historical_tick_bid_ask() -> List[Tuple]:
     """Details for logging HistoricalTickBidAsk."""
 
     return [
-        ("Timestamp", dtypes.DateTime, lambda t: unix_sec_to_dh_datetime(t.time)),
+        ("Timestamp", dtypes.Instant, lambda t: unix_sec_to_j_instant(t.time)),
         ("BidPrice", dtypes.float64, lambda t: t.priceBid),
         ("AskPrice", dtypes.float64, lambda t: t.priceAsk),
-        ("BidSize", dtypes.int64, lambda t: t.sizeBid),
-        ("AskSize", dtypes.int64, lambda t: t.sizeAsk),
+        ("BidSize", dtypes.float64, lambda t: t.sizeBid),
+        ("AskSize", dtypes.float64, lambda t: t.sizeAsk),
         *_include_details(_details_tick_attrib_bid_ask(), lambda t: t.tickAttribBidAsk),
     ]
 
 
 logger_hist_tick_bid_ask = IbComplexTypeLogger("HistoricalTickBidAsk", _details_historical_tick_bid_ask())
 
 
@@ -441,17 +447,14 @@
         ("OpenClose", dtypes.string, lambda o: map_values(o.openClose, open_close_values)),
         ("Origin", dtypes.string, lambda o: map_values(o.origin, origin_values)),
         ("ShortSaleSlot", dtypes.string, lambda o: map_values(o.shortSaleSlot, short_sale_slot_values)),
         ("ExemptCode", dtypes.int64, lambda o: o.exemptCode),
 
         # SMART routing only
         ("DiscretionaryAmt", dtypes.float64, lambda o: o.discretionaryAmt),
-        ("ETradeOnly", dtypes.bool_, lambda o: o.eTradeOnly),
-        ("FirmQuoteOnly", dtypes.bool_, lambda o: o.firmQuoteOnly),
-        ("NbboPriceCap", dtypes.float64, lambda o: o.nbboPriceCap),
         ("OptOutSmarRouting", dtypes.bool_, lambda o: o.optOutSmartRouting),
 
         # BOX exchange orders only
         ("AuctionStrategy", dtypes.string, lambda o: map_values(o.auctionStrategy, auction_stragey_values)),
         ("StartingPrice", dtypes.float64, lambda o: o.startingPrice),
         ("StockRefPrice", dtypes.float64, lambda o: o.stockRefPrice),
         ("Delta", dtypes.float64, lambda o: o.delta),
@@ -619,15 +622,15 @@
 ####
 
 def _details_execution() -> List[Tuple]:
     """ Details for logging Execution. """
 
     return [
         ("ExecId", dtypes.string, lambda e: e.execId),
-        ("Timestamp", dtypes.DateTime, lambda e: ib_to_dh_datetime(e.time)),
+        ("Timestamp", dtypes.Instant, lambda e: ib_to_j_instant(e.time)),
         ("AcctNumber", dtypes.string, lambda e: e.acctNumber),
         ("Exchange", dtypes.string, lambda e: e.exchange),
         ("Side", dtypes.string, lambda e: e.side),
         ("Shares", dtypes.float64, lambda e: e.shares),
         ("Price", dtypes.float64, lambda e: e.price),
         ("PermId", dtypes.int64, lambda e: e.permId),
         ("ClientId", dtypes.int64, lambda e: e.clientId),
@@ -646,25 +649,25 @@
 logger_execution = IbComplexTypeLogger("Execution", _details_execution())
 
 ####
 
 def _details_commission_report() -> List[Tuple]:
     """ Details for logging CommissionReport. """
 
-    def format_yield_redemption_date(date: int) -> Union[str, None]:
+    def format_yield_redemption_date(date: int) -> Optional[str]:
         if date == 0:
             return None
 
         # YYYYMMDD format
         d = date % 100
         m = int((date / 100) % 100)
         y = int(date / 10000)
         return f"{y:04}-{m:02}-{d:02}"
 
-    def map_null_value(value: float) -> Union[float, None]:
+    def map_null_value(value: float) -> Optional[float]:
 
         if value == sys.float_info.max:
             return None
 
         return value
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_tws/order_id_queue.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_tws/order_id_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     _events: List[Event]
     _values: List[int]
     _lock: LoggingLock
     _strategy: OrderIdStrategy
     _last_value: int
     _request_thread: Thread
 
-    def __init__(self, client: 'IbTwsClient', strategy: OrderIdStrategy = OrderIdStrategy.RETRY):
+    def __init__(self, client: 'IbTwsClient', strategy: OrderIdStrategy):
         self._events = []
         self._values = []
         self._lock = LoggingLock("OrderIdEventQueue")
         self._client = client
         self._strategy = strategy
         self._last_value = None
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_tws/requests.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_tws/requests.py`

 * *Files identical despite different names*

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib/_tws/tws_client.py` & `deephaven_ib-0.3.1/src/deephaven_ib/_tws/tws_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import time
 import types
 # noinspection PyPep8Naming
 import xml.etree.ElementTree as ET
 from functools import wraps
 from threading import Thread
-from typing import Set
+from typing import Set, Optional
 
 import decimal
 from decimal import Decimal
 
 from deephaven.table import Table
 from deephaven import dtypes
 
@@ -32,15 +32,15 @@
 from .contract_registry import ContractRegistry
 from .ib_type_logger import *
 from .order_id_queue import OrderIdEventQueue, OrderIdStrategy
 from .requests import RequestIdManager
 from .._internal.error_codes import load_error_codes
 from .._internal.short_rates import load_short_rates
 from .._internal.tablewriter import TableWriter
-from ..time import unix_sec_to_dh_datetime
+from ..time import unix_sec_to_j_instant
 
 _error_code_message_map, _error_code_note_map = load_error_codes()
 _news_msgtype_map: Dict[int, str] = {news.NEWS_MSG: "NEWS", news.EXCHANGE_AVAIL_MSG: "EXCHANGE_AVAILABLE",
                                      news.EXCHANGE_UNAVAIL_MSG: "EXCHANGE_UNAVAILABLE"}
 
 
 # Rate limit is 50 per second.  Limiting to 45 per second.
@@ -195,15 +195,15 @@
 
         table_writers["news_articles"] = TableWriter(
             ["RequestId", "ArticleType", "ArticleText"],
             [dtypes.int64, dtypes.string, dtypes.string])
 
         table_writers["news_historical"] = TableWriter(
             ["RequestId", "Timestamp", "ProviderCode", "ArticleId", "Headline"],
-            [dtypes.int64, dtypes.DateTime, dtypes.string, dtypes.string, dtypes.string])
+            [dtypes.int64, dtypes.Instant, dtypes.string, dtypes.string, dtypes.string])
 
         ####
         # Market Data
         ####
 
         table_writers["ticks_price"] = TableWriter(
             ["RequestId", "TickType", "Price", *logger_tick_attrib.names()],
@@ -240,15 +240,15 @@
 
         table_writers["ticks_bid_ask"] = TableWriter(
             ["RequestId", *logger_hist_tick_bid_ask.names()],
             [dtypes.int64, *logger_hist_tick_bid_ask.types()])
 
         table_writers["ticks_mid_point"] = TableWriter(
             ["RequestId", "Timestamp", "MidPoint"],
-            [dtypes.int64, dtypes.DateTime, dtypes.float64])
+            [dtypes.int64, dtypes.Instant, dtypes.float64])
 
         table_writers["bars_historical"] = TableWriter(
             ["RequestId", *logger_bar_data.names()],
             [dtypes.int64, *logger_bar_data.types()])
 
         table_writers["bars_realtime"] = TableWriter(
             ["RequestId", *logger_real_time_bar_data.names()],
@@ -388,16 +388,16 @@
 
     ####################################################################################################################
     ####################################################################################################################
     ## General
     ####################################################################################################################
     ####################################################################################################################
 
-    def log_request(self, req_id: int, request_type: str, contract: Union[Contract, None],
-                    notes: Union[Dict[str, Any], None]):
+    def log_request(self, req_id: int, request_type: str, contract: Optional[Contract],
+                    notes: Optional[Dict[str, Any]]):
         """Log a data request."""
 
         if notes is None:
             note_string = None
         else:
             note_string = json.dumps(dict({k: str(v) for (k, v) in notes.items()}.items()))
 
@@ -466,15 +466,18 @@
 
     def symbolSamples(self, reqId: int, contractDescriptions: ListOfContractDescription):
         EWrapper.symbolSamples(self, reqId, contractDescriptions)
 
         for cd in contractDescriptions:
             self._table_writers["contracts_matching"].write_row([reqId, *logger_contract.vals(cd.contract),
                                                                  to_string_set(cd.derivativeSecTypes)])
-            self.contract_registry.request_contract_details_nonblocking(cd.contract)
+
+            # Negative contract IDs seem to be for malformed contracts that yield errors when requesting details
+            if cd.contract.conId >= 0:
+                self.contract_registry.request_contract_details_nonblocking(cd.contract)
 
     ####
     # reqMarketRule
     ####
 
     def marketRule(self, marketRuleId: int, priceIncrements: ListOfPriceIncrements):
         EWrapper.marketRule(self, marketRuleId, priceIncrements)
@@ -777,15 +780,15 @@
 
         if len(h) == 1:
             headline_clean = h[0]
         else:
             headline_clean = h[1]
 
         self._table_writers["news_historical"].write_row(
-            [requestId, ib_to_dh_datetime(timestamp), providerCode, articleId,
+            [requestId, ib_to_j_instant(timestamp), providerCode, articleId,
              headline_clean])
 
     def historicalNewsEnd(self, requestId: int, hasMore: bool):
         # do not need to implement
         EWrapper.historicalNewsEnd(self, requestId, hasMore)
 
     ####################################################################################################################
@@ -888,34 +891,38 @@
     def historicalTicksBidAsk(self, reqId: int, ticks: ListOfHistoricalTickBidAsk, done: bool):
 
         for t in ticks:
             self._table_writers["ticks_bid_ask"].write_row([reqId, *logger_hist_tick_bid_ask.vals(t)])
 
     def tickByTickMidPoint(self, reqId: int, timestamp: int, midPoint: float):
         EWrapper.tickByTickMidPoint(self, reqId, timestamp, midPoint)
-        self._table_writers["ticks_mid_point"].write_row([reqId, unix_sec_to_dh_datetime(timestamp), midPoint])
+        self._table_writers["ticks_mid_point"].write_row([reqId, unix_sec_to_j_instant(timestamp), midPoint])
 
     def historicalTicks(self, reqId: int, ticks: ListOfHistoricalTick, done: bool):
         EWrapper.historicalTicks(self, reqId, ticks, done)
 
         for t in ticks:
-            self._table_writers["ticks_mid_point"].write_row([reqId, unix_sec_to_dh_datetime(t.time), t.price])
+            self._table_writers["ticks_mid_point"].write_row([reqId, unix_sec_to_j_instant(t.time), t.price])
 
     ####
     # reqHistoricalData
     ####
 
     def historicalData(self, reqId: int, bar: BarData):
         EWrapper.historicalData(self, reqId, bar)
         self._table_writers["bars_historical"].write_row([reqId, *logger_bar_data.vals(bar)])
 
     def historicalDataEnd(self, reqId: int, start: str, end: str):
         # do not ned to implement
         EWrapper.historicalDataEnd(self, reqId, start, end)
 
+    def historicalDataUpdate(self, reqId: int, bar: BarData):
+        EWrapper.historicalDataUpdate(self, reqId, bar)
+        self._table_writers["bars_historical"].write_row([reqId, *logger_bar_data.vals(bar)])
+
     ####
     # reqRealTimeBars
     ####
 
     def reqRealTimeBars(self, reqId: TickerId, contract: Contract, barSize: int,
                         whatToShow: str, useRTH: bool,
                         realTimeBarsOptions: TagValueList):
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib.egg-info/PKG-INFO` & `deephaven_ib-0.3.1/src/deephaven_ib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-ib
-Version: 0.2.9
+Version: 0.3.1
 Summary: An Interactive Brokers integration for Deephaven
 Home-page: https://github.com/deephaven-examples/deephaven-ib
 Author: David R. (Chip) Kent IV
 Author-email: chipkent@deephaven.io
 Project-URL: Deephaven, https://deephaven.io
 Project-URL: Deephaven GitHub, https://github.com/deephaven/deephaven-core
 Project-URL: GitHub Issues, https://github.com/deephaven-examples/deephaven-ib/issues
@@ -13,21 +13,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # deephaven-ib
 
-![Deephaven Data Labs Logo](docs/assets/Deephaven-Logo-Wordmark-Community-OnLight.png)
+![Deephaven Data Labs Logo](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/Deephaven-Logo-Wordmark-Community-OnLight.png)
 
 ![Build CI](https://github.com/deephaven-examples/deephaven-ib/actions/workflows/build-and-publish.yml/badge.svg?branch=main)
 
 An [Interactive Brokers](https://www.interactivebrokers.com/) integration for [Deephaven](https://deephaven.io).
 
 [Interactive Brokers](https://www.interactivebrokers.com/) is a very popular brokerage in the quantitative finance world,
 with about $200B of customer equity.  Quants and hedge funds often choose [Interactive Brokers](https://www.interactivebrokers.com/) because of its low trading costs and API that facilitates automated trading.  With low minimum account balances, 
@@ -57,15 +57,15 @@
 * Bonds
 * Foreign Exchange (Forex or FX)
 * Cryptocurrency
 * Contracts for Differences (CFDs)
 * Warrants
 * Commodities
 
-![Overview Image](docs/assets/overview.png)
+![Overview Image](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/overview.png)
 
 **WARNING: Automated trading can go horribly wrong very quickly.  Verify your code on a paper trading account before 
 unleashing trading on an account where money can be lost.  If you think this can not happen to you, read
 [The Rise and Fall of Knight Capital](https://medium.com/dataseries/the-rise-and-fall-of-knight-capital-buy-high-sell-low-rinse-and-repeat-ae17fae780f6).
 The [Setup](#setup) section shows configurations to prevent accidental trade submission.**
 
 For more details, see:
@@ -135,15 +135,15 @@
     * `ticks_string`: real-time tick market data of string values requested via `request_market_data`.
     * `ticks_efp`: real-time tick market data of exchange for physical (EFP) values requested via `request_market_data`.
     * `ticks_generic`: real-time tick market data of generic floating point values requested via `request_market_data`.
     * `ticks_option_computation`: real-time tick market data of option computations requested via `request_market_data`.
     * `ticks_trade`: real-time tick market data of trade prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
     * `ticks_bid_ask`: real-time tick market data of bid and ask prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
     * `ticks_mid_point`: real-time tick market data of mid-point prices requested via `request_tick_data_historical` or `request_tick_data_realtime`.
-    * `bars_historical`: historical price bars requested via `request_bars_historical`.
+    * `bars_historical`: historical price bars requested via `request_bars_historical`.  Real-time bars change as new data arrives.
     * `bars_realtime`: real-time price bars requested via `request_bars_realtime`.
 * Order Management System (OMS)
     * `orders_submitted`: submitted orders **FOR THE THE CLIENT'S ID**.  A client ID of 0 contains manually entered orders.  Automatically populated.
     * `orders_status`: order statuses.  Automatically populated.
     * `orders_completed`: completed orders.  Automatically populated.
     * `orders_exec_details`: order execution details.  Automatically populated.
     * `orders_exec_commission_report`: order execution commission report.  Automatically populated.
@@ -154,142 +154,207 @@
 
 You may want to combine data from other sources with your IB data.  [Deephaven](https://deephaven.io) can load data from:
 * [CSV](https://deephaven.io/core/docs/how-to-guides/csv-import/)
 * [Parquet](https://deephaven.io/core/docs/how-to-guides/parquet-flat/) 
 * [Kafka](https://deephaven.io/core/docs/how-to-guides/kafka-topics/).  
 See the [Deephaven Documentation](https://deephaven.io/core/docs) for details.
 
-Files placed in the `./docker/data/` directory are visible in the Docker container at `/data/`.  
-See [Access your file system with Docker data volumes](https://deephaven.io/core/docs/conceptual/docker-data-volumes/) for details.
-
 # Run deephaven-ib
 
-Follow these steps to run a [Deephaven](https://deephaven.io) plus [Interactive Brokers](https://interactivebrokers.com) system. 
+Follow these steps to run a [Deephaven](https://deephaven.io) plus [Interactive Brokers](https://interactivebrokers.com) system.
 
-`<deephaven_version>` is the version of [Deephaven](https://deephaven.io) to run (e.g., `0.11.0`).  A list of available versions 
-can be found on the [Deephaven Releases GitHub page](https://github.com/deephaven/deephaven-core/releases).  
-Version `0.11.0` or higher must be used.
+These instructions produce a virtual environment with [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), [Deephaven](https://deephaven.io), and `ibapi` installed.
+For more details on using pip-installed Deephaven, see [Deephaven's Installation Guide for pip](https://deephaven.io/core/docs/tutorials/pip-install/).
 
-**Windows users need to run the commands in WSL.**
+| :exclamation:  Windows users _must_ run these commands in WSL.   |
+|------------------------------------------------------------------|
 
-## Setup
+## Setup IB
 To setup and configure the system:
 
-1) Follow the [Deephaven Quick Start Guide](https://deephaven.io/core/docs/tutorials/quickstart/) to get [Deephaven](https://deephaven.io) running.  
 1) Follow the [TWS Installation Instructions](https://www.interactivebrokers.com/en/trading/tws.php) to get [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) running.
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-1) In [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), click on the gear in the
-upper right corner.  ![](docs/assets/config-gear.png)  
+2) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
+3) In [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), click on the gear in the
+upper right corner.  ![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/config-gear.png)  
   In `API->Settings`, make sure:
 
     * "Enable ActiveX and Socket Clients" is selected.
     * "Allow connections from localhost only" is not selected.
     * "Read-Only API" is selected if you want to prevent trade submission from [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).  
         
     Also, note the "Socket port" value.  It is needed when connecting [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
-    ![](docs/assets/config-api.png)
-1) [For Paper Trading] Log into the [Interactive Brokers Web Interface](https://interactivebrokers.com/).
-1) [For Paper Trading] In the [Interactive Brokers Web Interface](https://interactivebrokers.com/), navigate to `Account->Settings->Paper Trading Account` and make sure that "Share real-time market data subscriptions with paper trading account?" is set to true.
+    ![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/config-api.png)
+4) [For Paper Trading] Log into the [Interactive Brokers Web Interface](https://interactivebrokers.com/).
+5) [For Paper Trading] In the [Interactive Brokers Web Interface](https://interactivebrokers.com/), navigate to `Account->Settings->Paper Trading Account` and make sure that "Share real-time market data subscriptions with paper trading account?" is set to true.
+6) Once [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) is launched (see [below](#launch)), accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
+![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/allow-connections.png)
 
+## Virtual Environment
 
-## Launch
-To launch the system:
+Interactive Brokers does not make their Python wheels available via PyPI, and the wheels are not redistributable.
+As a result, installing [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) requires a Python script to build the wheels locally before installation.
+The script installs `deephaven-ib`, `ibapi`, and `deephaven` into the environment.
 
-### Launch with Docker
+To keep your development environment clean, the script creates a virtual environment for [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
+Follow the directions below to build and activate the virtual environment using the [./dhib_env.py](./dhib_env.py) script.
 
-This is the most tested way to launch.
+An existing virtual environment can be used with the `--create_venv false` and `--path_venv <path>` options.
 
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-2) Accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
-![](docs/assets/allow-connections.png)
-3) Create a directory for your data and scripts
-    ```bash
-    mkdir data
-    ```
-4) Launch the system (Option 1):
-    * On Mac:
+If you prefer to install directly into your system Python without a virtual environment, 
+you can use the `--use_venv false` option to [./dhib_env.py](./dhib_env.py).
+
+
+### Build the Virtual Environment
+
+1) Install Java 17 and set the appropriate `JAVA_HOME` environment variable.    
+2) Check out [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib)
     ```bash
     git clone git@github.com:deephaven-examples/deephaven-ib.git
-    cd deephaven-ib/docker/dev/build.sh
-    # Set jvm_args to the desired JVM memory for Deephaven
-    docker run -it -v data:/data -p 10000:10000 deephaven-examples/deephaven-ib:dev python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    ```
-    * On other platforms:
-    ```bash
-    # Set jvm_args to the desired JVM memory for Deephaven
-    docker run -it -v data:/data -p 10000:10000 ghcr.io/deephaven-examples/deephaven-ib python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
     ```
-5) Launch the system and execute a custom script (Option 2):
-    * On Mac:
+3) Change to the deephaven-ib directory:
     ```bash
-    git clone git@github.com:deephaven-examples/deephaven-ib.git
-    cd deephaven-ib/docker/dev/build.sh
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    cp path/to/your_script.py data/your_script.py
-    docker run -it -v data:/data -p 10000:10000 deephaven-examples/deephaven-ib:dev python3 -i /data/your_script.py
+    cd deephaven-ib
     ```
-    * On other platforms:
+4) Build a [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) virtual environment:
+
+   First, install the dependencies needed to run the script:
     ```bash
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    cp path/to/your_script.py data/your_script.py
-    docker run -it -v data:/data -p 10000:10000 ghcr.io/deephaven-examples/deephaven-ib python3 -i /data/your_script.py
+    python3 -m pip install -r requirements_dhib_env.txt
     ```
-7) Launch the [Deephaven IDE](https://github.com/deephaven/deephaven-core/blob/main/README.md#run-deephaven-ide) by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in a browser.
-
-### Launch with a local installation (No Docker)
 
-> **_NOTE:_**  Deephaven pip install is not yet supported on all architectures.  This launch should work on Linux (AMD64 and ARM64) and Windows WSL.  It is not yet supported on Windows without WSL or Mac.  For these architectures, you should use the Docker installation.  As soon as Deephaven supports these architectures for pip, [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) will work.
-
-It is possible to use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) without docker, but this is a 
-new feature and has not been well tested.  To do this:
-1) Launch [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
-2) Accept incoming connections to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).  (May not be required for all sessions.)
-![](docs/assets/allow-connections.png)
-3) Install `ibapi`:
+   To see all options:
     ```bash
-    # pip installed version of ibapi is too old.  You must download and install a more recent version.
-    curl -o ./api.zip "https://interactivebrokers.github.io/downloads/twsapi_macunix.1016.01.zip"
-    unzip api.zip
-    cd ./IBJts/source/pythonclient
-    python3 setup.py install
+    python3 ./dhib_env.py --help
     ```
-4) Install [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib):
+
+   To install the latest production release version of [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) from PyPi plus the release-specified `ibapi` and `deephaven` versions: 
     ```bash
-    pip3 install --upgrade pip setuptools wheel
-    pip3 install deephaven-ib
+    python3 ./dhib_env.py release
     ```
-5) Install Java 11 and set the appropriate `JAVA_HOME` environment variable.    
-6) Launch the system (Option 1):
+   
+   To install the latest development version of [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) from source plus the default `ibapi` and `deephaven` versions:
     ```bash
-    # Set jvm_args to the desired JVM memory for Deephaven
-    python3 -i -c "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
+    python3 ./dhib_env.py dev
     ```
-7) Launch the system and execute a custom script (Option 2):
+
+   To create a venv for developing [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) in PyCharm: (This will not install `deephaven-ib`, but it will install the default `ibapi` and `deephaven` versions.)
     ```bash
-    # your_script.py must begin with: "from deephaven_server import Server; _server = Server(port=10000, jvm_args=['-Xmx4g']); _server.start()"
-    # Set jvm_args to the desired JVM memory for Deephaven
-    python3 -i /data/your_script.py
+    python3 ./dhib_env.py dev --install_dhib false
     ```
-8) Launch the [Deephaven IDE](https://github.com/deephaven/deephaven-core/blob/main/README.md#run-deephaven-ide) by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in a browser.
-9) Use `host=localhost` for the hostname in the examples
+   
+5) In the logs, take note of where the virtual environment is located.  It will be in a directory like `./venv-<versiondetails>`.
+   
+### Activate the Virtual Environment
+
+To activate the virtual environment:
+```bash
+source ./venv-<versiondetails>/bin/activate
+```
+
+Once the virtual environment is activated, `python` and `pip` will use the virtual environment's Python and packages --
+including everything needed to run [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
+
+### Deactivate the Virtual Environment
+
+To deactivate the virtual environment:
+```bash
+deactivate
+```
+
+Once the virtual environment is deactivated, `python` and `pip` will use the system's Python and packages.
+[deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) will not be available.
+
 
 # Use deephaven-ib
 
-To use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), you will need to open the [Deephaven Web IDE](http://localhost:10000/ide/) 
-by navigating to [http://localhost:10000/ide/](http://localhost:10000/ide/) in your web browser.  The following commands
-can be executed in the console.
+To use [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), you need to start a [Deephaven](https://deephaven.io) server and connect to 
+[IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
+You can optionally use the Deephaven IDE to visualize data and run queries.
+
+## Start Deephaven
+
+First, start a [Deephaven](https://deephaven.io) server.  This server will be used to process data and run queries.
+
+The documentation and examples here illustrate using Deephaven's [Pre-Shared Key (PSK) authentication](https://deephaven.io/core/docs/how-to-guides/authentication/auth-psk/)
+with the password `DeephavenRocks!`.  Other types of Deephaven authentication can also work.  
+See the [Deephaven Documentation](https://deephaven.io/core/docs/) for details.
+
+
+### Option 1: Use the `deephaven` command
+
+The easiest way to start a deephaven server is using `deephaven` on the command line.
+The `deephaven` command was added to the virtual environment when it was created.
+It is available in [Deephaven](https://deephaven.io) versions `>= 0.34.0`.
+
+This command will start a deephaven server with 4GB of memory and the password `DeephavenRocks!`.
+It will also automatically open the Deephaven IDE in a web browser.
+
+```bash
+source ./venv-<versiondetails>/bin/activate
+deephaven server --jvm-args "-Xmx4g -Dauthentication.psk=DeephavenRocks! -Dstorage.path=~/.deephaven"
+```
+
+
+### Option 2: Use a Python script
+
+An alternative way to launch a deephaven server is to use a Python script.  This works with all versions of 
+[Deephaven](https://deephaven.io) and can be used to populate the server with queries.  
+See [Deephaven's Installation Guide for pip](https://deephaven.io/core/docs/tutorials/pip-install/) for more details on 
+running [Deephaven](https://deephaven.io) this way.
+
+To start Python with the virtual environment, run:
+```bash
+source ./venv-<versiondetails>/bin/activate
+python
+```
+
+Once Python is running, you can start a deephaven server with the following script:
+```python
+import os
+from time import sleep
+from deephaven_server import Server
+
+_server = Server(port=10000, jvm_args=['-Xmx4g','-Dauthentication.psk=DeephavenRocks!','-Dstorage.path=' + os.path.expanduser('~/.deephaven')])
+_server.start()
+
+# You can insert queries here
+
+# Keep the server running
+while True:
+    sleep(1)
+```
+> :warning: These deephaven server commands **must** be run before importing `deephaven` or `deephaven_ib`.
+
+At the indicated place in the script, you can put queries that you want to run when the server starts.  
+This could be code to conenct to [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php), request data, analyze data, visualize data, or trade.  
+See the examples below for more details.
+
+
+## Launch the Deephaven IDE
+
+Once the Deephaven server is started, you can launch the Deephaven IDE.
+If you used the `deephaven` command to start the server, the Deephaven IDE will automatically open in your web browser.
+
+The Deephaven IDE is a web-based interface for working with Deephaven.
+Once in the IDE, you can run queries, create notebooks, and visualize data.
+You can also run all of the example code below and the more complex examples in [./examples](./examples).
+
+To launch the Deephaven IDE, navigate to [http://localhost:10000/ide/](http://localhost:10000/ide/) in your web browser.
+Chrome, Edge, Chrome-based, and Firefox browsers are supported.  Safari is not supported.
+How you authenticate will depend upon how authentication is configured.  
+In the examples here, you will use the password `DeephavenRocks!`.
+
 
 ## Connect to TWS
 
 All [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) sessions need to first create a client for interacting 
 with [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php).
 
-`host` is the computer to connect to.  When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) inside
+`host` is the computer to connect to.  When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) locally, `host` is usually set to `localhost`.
+When using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) inside
 of Docker, `host` should be set to `host.docker.internal`.  
 
 `port` is the network port [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 communicates on.  This value can be found in the [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 settings.  By default, production trading uses port 7496, and paper trading uses port 7497.  See [Setup](#setup) and [TWS Initial Setup](https://interactivebrokers.github.io/tws-api/initial_setup.html) for more details.
 
 `read_only` is a boolean value that is used to enable trading.  By default `read_only=True`, preventing trading.  Use `read_only=False` to enable trading.
@@ -305,36 +370,36 @@
 * `OrderIdStrategy.BASIC` - Request a new order ID from TWS every time one is needed.  Does not retry, so it may deadlock if TWS does not respond.
 * `OrderIdStrategy.INCREMENT` - Use the initial order ID sent by TWS and increment the value upon every request.  This is fast, but it may fail for multiple, concurrent sessions connected to TWS.
 
 For a read-write session that allows trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=False)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=False)
 client.connect()
 ```
 
 For a read-only session that does not allow trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=True)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=True)
 client.connect()
 ```
 
 For a read-only financial advisor (FA) session that does not allow trading:
 ```python
 import deephaven_ib as dhib
 
-client = dhib.IbSessionTws(host="host.docker.internal", port=7497, read_only=True, is_fa=True)
+client = dhib.IbSessionTws(host="localhost", port=7497, read_only=True, is_fa=True)
 client.connect()
 ```
 
 After `client.connect()` is called, TWS requires that the connection be accepted.
-![](docs/assets/accept-connection.png)
+![](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/accept-connection.png)
 
 ## Get data
 
 [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) data is stored in
 the [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) client as two dictionaries of tables:
 * `tables` contains the tables most users will want.  
 * `tables_raw` contains raw [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
@@ -465,16 +530,16 @@
 contract.secType = "STK"
 contract.currency = "USD"
 contract.exchange = "SMART"
 
 rc = client.get_registered_contract(contract)
 print(contract)
 
-start = to_datetime("2021-01-01T00:00:00 NY")
-end = to_datetime("2021-01-10T00:00:00 NY")
+start = "2021-01-01T00:00:00 ET"
+end = "2021-01-10T00:00:00 ET"
 client.request_news_historical(rc, start=start, end=end)
 
 client.request_news_article(provider_code="BRFUPDN", article_id="BRFUPDN$107d53ea")
 ```
 
 [./examples/example_all_functionality.py](./examples/example_all_functionality.py) illustrates requesting
 news data.
@@ -573,15 +638,15 @@
 bars_dia = bars_realtime.where("Symbol=`DIA`")
 bars_spy = bars_realtime.where("Symbol=`SPY`")
 bars_joined = bars_dia.view(["Timestamp", "TimestampEnd", "Dia=Close"]) \
     .natural_join(bars_spy, on="TimestampEnd", joins="Spy=Close") \
     .update("Ratio = Dia/Spy")
 ```
 
-![DIA SPY Ratio](docs/assets/dia_spy_ratio.png)
+![DIA SPY Ratio](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/dia_spy_ratio.png)
 
 ## Plotting
 
 [Deephaven](https://deephaven.io) has very powerful plotting functionality for both static and real-time data.
 The example below plots the bid and ask prices of `AAPL` for every tick in the market.
 
 For more details, see the [Deephaven Coummunity Core Documentation](https://deephaven.io/core/docs/).
@@ -608,15 +673,15 @@
 from deephaven.plot import Figure
 
 plot_aapl = Figure().plot_xy("Bid",  t=ticks_bid_ask, x="ReceiveTime", y="BidPrice") \
     .plot_xy("Ask",  t=ticks_bid_ask, x="ReceiveTime", y="AskPrice") \
     .show()
 ```
 
-![AAPL Bid Ask](docs/assets/aapl_bid_ask.png)
+![AAPL Bid Ask](https://raw.githubusercontent.com/deephaven-examples/deephaven-ib/main/docs/assets/aapl_bid_ask.png)
 
 ## Help!
 
 ### Error Table
 
 [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib) logs all [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php)
 errors to the `errors` table.  This table should be monitored when using [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).
@@ -650,12 +715,28 @@
 If you can not solve your problems through either the `errors` table or through logging, you can try:
 
 * [deephaven-ib API Documentation](https://deephaven-examples.github.io/deephaven-ib/)
 * [Interactive Brokers Support](https://www.interactivebrokers.com/en/support/individuals.php)
 * [Gitter: A relaxed chat room about all things Deephaven](https://gitter.im/deephaven/deephaven)
 * [Deephaven Community Slack](https://deephaven.io/slack)
 
+### `Takes N positional arguments but M were given`
+
+You may encounter an error that looks like: `Takes N positional arguments but M were given`.  
+If you see a problem like this, your `ibapi` version does not match the version needed by [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib).  
+The [`ibapi` version in PyPI](https://pypi.org/project/ibapi/) is ancient and appears to have been abandoned by [Interactive Brokers](https://www.interactivebrokers.com/).  
+Currently [Interactive Brokers](https://www.interactivebrokers.com/) is delivering `ibapi` either via the [IB Trader Workstation (TWS)](https://www.interactivebrokers.com/en/trading/tws.php) 
+download or via git. 
+
+To check your `ibapi` version:
+```python
+import ibapi
+print(ibapi.__version__)
+```
+
+The `ibapi` API is very unstable.  If your version does not exactly match the version needed by [deephaven-ib](https://github.com/deephaven-examples/deephaven-ib), 
+you will need to install the correct version.  Regenerate your virtual environment as described above.
 
 # Examples
 
 Examples can be found in [./examples](./examples).
```

### Comparing `deephaven_ib-0.2.9/src/deephaven_ib.egg-info/SOURCES.txt` & `deephaven_ib-0.3.1/src/deephaven_ib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/deephaven_ib/__init__.py
-src/deephaven_ib/_query_inputs.py
 src/deephaven_ib/time.py
 src/deephaven_ib.egg-info/PKG-INFO
 src/deephaven_ib.egg-info/SOURCES.txt
 src/deephaven_ib.egg-info/dependency_links.txt
 src/deephaven_ib.egg-info/requires.txt
 src/deephaven_ib.egg-info/top_level.txt
 src/deephaven_ib/_internal/__init__.py
```


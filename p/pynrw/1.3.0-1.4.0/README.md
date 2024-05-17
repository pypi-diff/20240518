# Comparing `tmp/pynrw-1.3.0.tar.gz` & `tmp/pynrw-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrw-1.3.0.tar", last modified: Tue May 14 21:37:29 2024, max compression
+gzip compressed data, was "pynrw-1.4.0.tar", last modified: Fri May 17 23:32:38 2024, max compression
```

## Comparing `pynrw-1.3.0.tar` & `pynrw-1.4.0.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-14 21:37:19.000000 pynrw-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-14 21:37:29.260302 pynrw-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-05-14 21:37:19.000000 pynrw-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.256302 pynrw-1.3.0/nrw/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.256302 pynrw-1.3.0/nrw/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/_traversal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/nrw/database/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/_query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/msaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/msaccess.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/mysql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/sqlite.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/nrw/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_comparable_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/pynrw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-14 21:37:19.000000 pynrw-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 21:37:19.000000 pynrw-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:37:29.260302 pynrw-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:38.834775 pynrw-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-17 23:32:29.000000 pynrw-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-17 23:32:38.834775 pynrw-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-05-17 23:32:29.000000 pynrw-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:38.826775 pynrw-1.4.0/nrw/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:38.830775 pynrw-1.4.0/nrw/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/algorithms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/algorithms/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/algorithms/_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/algorithms/_traversal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:38.830775 pynrw-1.4.0/nrw/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/_query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/msaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/msaccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/database/sqlite.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:38.830775 pynrw-1.4.0/nrw/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_comparable_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/datastructures/_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:38.834775 pynrw-1.4.0/nrw/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/network/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/network/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/network/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/network/_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:29.000000 pynrw-1.4.0/nrw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:32:38.834775 pynrw-1.4.0/pynrw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-17 23:32:38.000000 pynrw-1.4.0/pynrw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 23:32:38.000000 pynrw-1.4.0/pynrw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:32:38.000000 pynrw-1.4.0/pynrw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-17 23:32:38.000000 pynrw-1.4.0/pynrw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 23:32:38.000000 pynrw-1.4.0/pynrw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-17 23:32:29.000000 pynrw-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-17 23:32:29.000000 pynrw-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:32:38.834775 pynrw-1.4.0/setup.cfg
```

### Comparing `pynrw-1.3.0/LICENSE` & `pynrw-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrw-1.3.0/PKG-INFO` & `pynrw-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.3.0
+Version: 1.4.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: pyodbc; platform_python_implementation == "CPython"
 Requires-Dist: pypyodbc; platform_python_implementation == "PyPy"
+Requires-Dist: typing_extensions>=4.4.0; python_version < "3.12"
 
 # pynrw
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/realshouzy/pynrw/main.svg)](https://results.pre-commit.ci/latest/github/realshouzy/pynrw/main)
 [![pylint status](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml)
 [![test status](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml)
 [![CodeQL](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml)
@@ -87,15 +88,15 @@
 - [`Queue`](/nrw/datastructures/_queue.py)
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
-Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
+Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d. h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
 
 Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar) `ComparableContentT` zur Verfügung.
 
 Außerdem implementieren die Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht (besonders für `Binary(Search)Tree`) und `__repr__`, welches eine grobe Idee der internen Strukture gibt, z.B.:
 
 ```python
 from nrw.datastructures import BinarySearchTree
@@ -156,14 +157,24 @@
 Hierbei ist zu beachten, dass der `DatabaseConnector` für MSAccess den Microsoft Access Driver benötigt und passwortgeschützte Datenbanken nicht unterstüzt.
 Des weiteren gilt für `QueryResult`, dass die Daten und die Spaltentypen nicht unbedingt als String wiedergegeben werden. Die Daten werden als Python-Äquivalenten Datentypen wiedergegeben, und für die Spaltentypen gilt:
 
 - SQLite: immer `None`, da SQLite dynamisch typisiert ist
 - MySQL: die entsprechenden Datentypen von MySQL als String
 - MSAccess: die entsprechenden Datentypen (Klassen) von Python
 
+### Netzklassen
+
+Die Netzklassen sind ebenfalls semantisch identisch zu den Netzklassen des Landes. Diese sind in [`nrw.network`](/nrw/network/) zu definiert:
+
+- [`Connection`](/nrw/network/_connection.py)
+- [`Client`](/nrw/network/_client.py)
+- [`Server`](/nrw/network/_server.py)
+
+Die letzteren beiden sind [`ABCs`](https://docs.python.org/3/library/abc.html). Bei diesen weicht die interne Implementation von der Java Implementation des Landes ab, da deren Ansatz nicht eins-zu-eins in Python übertragen werden kann; somit ist der Quellcode für Fortgeschrittene. Nichtsdestotrotz ist die Anwendung und der Funktionsumfang der Selbe wie vom Land.
+
 ### Allgemein
 
 Für mehr Information zu einem beliebigen Objekt kann `help` genutzt werden, z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
```

### Comparing `pynrw-1.3.0/README.md` & `pynrw-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 - [`Queue`](/nrw/datastructures/_queue.py)
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
-Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
+Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d. h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
 
 Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar) `ComparableContentT` zur Verfügung.
 
 Außerdem implementieren die Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht (besonders für `Binary(Search)Tree`) und `__repr__`, welches eine grobe Idee der internen Strukture gibt, z.B.:
 
 ```python
 from nrw.datastructures import BinarySearchTree
@@ -131,14 +131,24 @@
 Hierbei ist zu beachten, dass der `DatabaseConnector` für MSAccess den Microsoft Access Driver benötigt und passwortgeschützte Datenbanken nicht unterstüzt.
 Des weiteren gilt für `QueryResult`, dass die Daten und die Spaltentypen nicht unbedingt als String wiedergegeben werden. Die Daten werden als Python-Äquivalenten Datentypen wiedergegeben, und für die Spaltentypen gilt:
 
 - SQLite: immer `None`, da SQLite dynamisch typisiert ist
 - MySQL: die entsprechenden Datentypen von MySQL als String
 - MSAccess: die entsprechenden Datentypen (Klassen) von Python
 
+### Netzklassen
+
+Die Netzklassen sind ebenfalls semantisch identisch zu den Netzklassen des Landes. Diese sind in [`nrw.network`](/nrw/network/) zu definiert:
+
+- [`Connection`](/nrw/network/_connection.py)
+- [`Client`](/nrw/network/_client.py)
+- [`Server`](/nrw/network/_server.py)
+
+Die letzteren beiden sind [`ABCs`](https://docs.python.org/3/library/abc.html). Bei diesen weicht die interne Implementation von der Java Implementation des Landes ab, da deren Ansatz nicht eins-zu-eins in Python übertragen werden kann; somit ist der Quellcode für Fortgeschrittene. Nichtsdestotrotz ist die Anwendung und der Funktionsumfang der Selbe wie vom Land.
+
 ### Allgemein
 
 Für mehr Information zu einem beliebigen Objekt kann `help` genutzt werden, z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
```

### Comparing `pynrw-1.3.0/nrw/algorithms/__init__.py` & `pynrw-1.4.0/nrw/algorithms/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Nützliche Algorithmen für die Datenstrukturen."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str, ...]] = (
+__all__: Final[list[str]] = [
     "linear_search",
     "depth_first_search",
     "breadth_first_search",
     "bubble_sort",
     "selection_sort",
     "insertion_sort",
     "merge_sort",
     "quick_sort",
     "preorder",
     "inorder",
     "postorder",
     "levelorder",
     "reverse_inorder",
-)
+]
 
 from typing import Final
 
 from nrw.algorithms._searching import (
     breadth_first_search,
     depth_first_search,
     linear_search,
```

### Comparing `pynrw-1.3.0/nrw/algorithms/__init__.pyi` & `pynrw-1.4.0/nrw/algorithms/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # pylint: skip-file
-__all__: Final[tuple[str, ...]] = (
+__all__: Final[list[str]] = [
     "linear_search",
     "depth_first_search",
     "breadth_first_search",
     "bubble_sort",
     "selection_sort",
     "insertion_sort",
     "merge_sort",
     "quick_sort",
     "preorder",
     "inorder",
     "postorder",
     "levelorder",
     "reverse_inorder",
-)
+]
 
 from typing import Final, TypeVar, overload
 
 from nrw.datastructures import (
     BinarySearchTree,
     BinaryTree,
     ComparableContentT,
```

### Comparing `pynrw-1.3.0/nrw/algorithms/_searching.py` & `pynrw-1.4.0/nrw/algorithms/_searching.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Suchalgorithmen für `List[ComparableContentT]`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str, ...]] = (
+__all__: Final[list[str]] = [
     "linear_search",
     "depth_first_search",
     "breadth_first_search",
-)
+]
 
 from typing import TYPE_CHECKING, Final, TypeVar
 
 from nrw.datastructures._list import List
 
 if TYPE_CHECKING:
     from nrw.datastructures._edge import Edge
```

### Comparing `pynrw-1.3.0/nrw/algorithms/_sorting.py` & `pynrw-1.4.0/nrw/algorithms/_sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Sortieralgorithmen für `List[ComparableContentT]`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str, ...]] = (
+__all__: Final[list[str]] = [
     "bubble_sort",
     "selection_sort",
     "insertion_sort",
     "merge_sort",
     "quick_sort",
-)
+]
 
 from typing import TYPE_CHECKING, Final
 
 from nrw.datastructures._list import List
 
 if TYPE_CHECKING:
     from nrw.datastructures._comparable_content import ComparableContentT
```

### Comparing `pynrw-1.3.0/nrw/algorithms/_traversal.py` & `pynrw-1.4.0/nrw/algorithms/_traversal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Traversierung für Binär Bäume."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str, ...]] = (
+__all__: Final[list[str]] = [
     "preorder",
     "inorder",
     "postorder",
     "levelorder",
     "reverse_inorder",
-)
+]
 
 from typing import Final, TypeVar
 from warnings import warn
 
 from nrw.datastructures import BinarySearchTree, BinaryTree, ComparableContentT, List
 
 _T = TypeVar("_T")
@@ -26,20 +26,20 @@
     result: List[_T | ComparableContentT] = List()
 
     if tree.is_empty:
         return result
 
     if not reverse:
         result.append(tree.content)
-        result.concat(preorder(tree.left_tree))
-        result.concat(preorder(tree.right_tree))
+        result.concat(preorder(tree.left_tree, reverse=reverse))
+        result.concat(preorder(tree.right_tree, reverse=reverse))
     else:
         result.append(tree.content)
-        result.concat(preorder(tree.right_tree))
-        result.concat(preorder(tree.left_tree))
+        result.concat(preorder(tree.right_tree, reverse=reverse))
+        result.concat(preorder(tree.left_tree, reverse=reverse))
 
     return result
 
 
 def inorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
     *,
@@ -47,21 +47,21 @@
 ) -> List[_T | ComparableContentT]:
     result: List[_T | ComparableContentT] = List()
 
     if tree.is_empty:
         return result
 
     if not reverse:
-        result.concat(preorder(tree.left_tree))
+        result.concat(inorder(tree.left_tree, reverse=reverse))
         result.append(tree.content)
-        result.concat(preorder(tree.right_tree))
+        result.concat(inorder(tree.right_tree, reverse=reverse))
     else:
-        result.concat(preorder(tree.right_tree))
+        result.concat(inorder(tree.right_tree, reverse=reverse))
         result.append(tree.content)
-        result.concat(preorder(tree.left_tree))
+        result.concat(inorder(tree.left_tree, reverse=reverse))
 
     return result
 
 
 def reverse_inorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
 ) -> List[_T | ComparableContentT]:  # pragma: no cover
@@ -76,20 +76,20 @@
 ) -> List[_T | ComparableContentT]:
     result: List[_T | ComparableContentT] = List()
 
     if tree.is_empty:
         return result
 
     if not reverse:
-        result.concat(preorder(tree.left_tree))
-        result.concat(preorder(tree.right_tree))
+        result.concat(postorder(tree.left_tree, reverse=reverse))
+        result.concat(postorder(tree.right_tree, reverse=reverse))
         result.append(tree.content)
     else:
-        result.concat(preorder(tree.right_tree))
-        result.concat(preorder(tree.left_tree))
+        result.concat(postorder(tree.right_tree, reverse=reverse))
+        result.concat(postorder(tree.left_tree, reverse=reverse))
         result.append(tree.content)
 
     return result
 
 
 def levelorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
```

### Comparing `pynrw-1.3.0/nrw/database/_query_result.py` & `pynrw-1.4.0/nrw/database/_query_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Klasse `QueryResult`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("QueryResult",)
+__all__: Final[list[str]] = ["QueryResult"]
 
 from typing import Any, Final
 
 
 class QueryResult:
     """Ein Objekt der Klasse `QueryResult` stellt die Ergebnistabelle einer
     Datenbankanfrage mit Hilfe
@@ -28,30 +28,29 @@
         self._column_names: tuple[str, ...] = column_names
         self._column_types: tuple[type | str | None, ...] = column_types
 
     @property
     def data(self) -> list[tuple[Any, ...]]:
         """Die Anfrage liefert die Einträge der Ergebnistabelle als eine `list`
         welche wiederum `tuple` enthält. Der erste Index stellt die Zeile und der zweite
-        die Spalte dar (d.h. Object[zeile][spalte]).
+        die Spalte dar (d. h. Object[zeile][spalte]).
         """
         return self._data
 
     @property
     def column_names(self) -> tuple[str, ...]:
         """Die Anfrage liefert die Bezeichner der Spalten der Ergebnistabelle als
         `tuple` vom Typ `str` zurück.
         """
         return self._column_names
 
     @property
     def column_types(self) -> tuple[type | str | None, ...]:
         """Die Anfrage liefert (wenn möglich) die Typenbezeichnung der Spalten der
         Ergebnistabelle als `tuple` vom jeweiligen Typ zurück.
-        Die Bezeichnungen entsprechen den Angaben in der `MySQL`-Datenbank.
         """
         return self._column_types
 
     @property
     def row_count(self) -> int:
         """Die Anfrage liefert die Anzahl der Zeilen der Ergebnistabelle als `int`."""
         return len(self._data) if self._data is not None else 0
```

### Comparing `pynrw-1.3.0/nrw/database/_query_result.pyi` & `pynrw-1.4.0/nrw/database/_query_result.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pylint: skip-file
-__all__: Final[tuple[str]] = ("QueryResult",)
+__all__: Final[list[str]] = ["QueryResult"]
 
 from typing import Any, Final
 
 class QueryResult:
     __slots__: Final[tuple[str, str, str]] = ("_data", "_column_names", "_column_types")
     def __init__(
         self,
```

### Comparing `pynrw-1.3.0/nrw/database/msaccess.py` & `pynrw-1.4.0/nrw/database/msaccess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Klasse `DatabaseConnector`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("DatabaseConnector",)
+__all__: Final[list[str]] = ["DatabaseConnector"]
 
 from typing import Final
 
 import pyodbc  # type: ignore[import-not-found]
 
 from nrw.database._query_result import QueryResult
```

### Comparing `pynrw-1.3.0/nrw/database/msaccess.pyi` & `pynrw-1.4.0/nrw/database/msaccess.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pylint: skip-file
-__all__: Final[tuple[str]] = ("DatabaseConnector",)
+__all__: Final[list[str]] = ["DatabaseConnector"]
 
 from typing import Final
 
 from nrw.database._query_result import QueryResult
 
 class DatabaseConnector:
     __slots__: Final[tuple[str, str, str]] = (
```

### Comparing `pynrw-1.3.0/nrw/database/mysql.py` & `pynrw-1.4.0/nrw/database/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Klasse `DatabaseConnector`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("DatabaseConnector",)
+__all__: Final[list[str]] = ["DatabaseConnector"]
 
 from typing import TYPE_CHECKING, Final
 
 import mysql.connector
 from mysql.connector import FieldType
 
 from nrw.database._query_result import QueryResult
```

### Comparing `pynrw-1.3.0/nrw/database/mysql.pyi` & `pynrw-1.4.0/nrw/database/sqlite.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # pylint: skip-file
-__all__: Final[tuple[str]] = ("DatabaseConnector",)
+__all__: Final[list[str]] = ["DatabaseConnector"]
 
 from typing import Final
 
 from nrw.database._query_result import QueryResult
 
 class DatabaseConnector:
-
     __slots__: Final[tuple[str, str, str]] = (
         "_connection",
         "_current_query_result",
         "_message",
     )
 
     def __init__(
         self,
-        ip: str,
-        port: int,
+        ip: None,
+        port: None,
         database: str,
-        username: str,
-        password: str,
+        username: None,
+        password: None,
     ) -> None: ...
     def execute_statement(self, sql_statement: str) -> None: ...
     @property
     def current_query_result(self) -> QueryResult | None: ...
     @property
     def error_message(self) -> str | None: ...
     def close(self) -> None: ...
```

### Comparing `pynrw-1.3.0/nrw/database/sqlite.py` & `pynrw-1.4.0/nrw/database/sqlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Klasse `DatabaseConnector`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("DatabaseConnector",)
+__all__: Final[list[str]] = ["DatabaseConnector"]
 
 import sqlite3
 from typing import Final
 
 from nrw.database._query_result import QueryResult
```

### Comparing `pynrw-1.3.0/nrw/datastructures/__init__.py` & `pynrw-1.4.0/nrw/datastructures/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Die Datenstrukturen nach den Vorgaben des Landes NRW."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str, ...]] = (
+__all__: Final[list[str]] = [
     "Stack",
     "Queue",
     "List",
     "BinaryTree",
     "ComparableContent",
     "ComparableContentT",
     "Vertex",
     "Edge",
     "BinarySearchTree",
     "Graph",
-)
+]
+
 
 from typing import Final
 
 from nrw.datastructures._binary_search_tree import BinarySearchTree
 from nrw.datastructures._binary_tree import BinaryTree
 from nrw.datastructures._comparable_content import ComparableContent, ComparableContentT
 from nrw.datastructures._edge import Edge
```

### Comparing `pynrw-1.3.0/nrw/datastructures/__init__.pyi` & `pynrw-1.4.0/nrw/datastructures/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pylint: skip-file
-__all__: Final[tuple[str, ...]] = (
+__all__: Final[list[str]] = [
     "Stack",
     "Queue",
     "List",
     "BinaryTree",
     "ComparableContent",
     "ComparableContentT",
     "Vertex",
     "Edge",
     "BinarySearchTree",
     "Graph",
-)
+]
 
 from typing import Final, Generic, TypeVar, overload
 
 from nrw.datastructures._comparable_content import ComparableContent, ComparableContentT
 
 _T = TypeVar("_T")
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_binary_search_tree.py` & `pynrw-1.4.0/nrw/datastructures/_binary_search_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Implementation der generischen Klasse `BinarySearchTree[ComparableContentT]`."""
 
 from __future__ import annotations
 
+__all__: Final[list[str]] = ["BinarySearchTree"]
+
 from typing import Final, Generic
 
 from nrw.datastructures._comparable_content import ComparableContentT
 from nrw.datastructures._utils import display_binary_node
 
 
 class _BSTNode(Generic[ComparableContentT]):
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_binary_tree.py` & `pynrw-1.4.0/nrw/datastructures/_binary_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation der generischen Klasse `BinaryTree[_T]`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("BinaryTree",)
+__all__: Final[list[str]] = ["BinaryTree"]
 
 from typing import Final, Generic, TypeVar
 
 from nrw.datastructures._utils import display_binary_node
 
 _T = TypeVar("_T")
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_comparable_content.py` & `pynrw-1.4.0/nrw/datastructures/_comparable_content.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation des generischen Protocols `ComparableContent[_T_contra]`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str, str]] = ("ComparableContent", "ComparableContentT")
+__all__: Final[list[str]] = ["ComparableContent", "ComparableContentT"]
 
 from typing import Any, Final, Protocol, TypeVar, runtime_checkable
 
 _T_contra = TypeVar("_T_contra", contravariant=True)
 
 
 @runtime_checkable
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_edge.py` & `pynrw-1.4.0/nrw/datastructures/_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation der Klasse `Edge`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("Edge",)
+__all__: Final[list[str]] = ["Edge"]
 
 from typing import TYPE_CHECKING, Final
 
 if TYPE_CHECKING:
     from nrw.datastructures._vertex import Vertex
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_graph.py` & `pynrw-1.4.0/nrw/datastructures/_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation der Klasse `Graph`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("Graph",)
+__all__: Final[list[str]] = ["Graph"]
 
 from io import StringIO
 from typing import TYPE_CHECKING, Final
 
 from nrw.datastructures._list import List
 
 if TYPE_CHECKING:
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_list.py` & `pynrw-1.4.0/nrw/datastructures/_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation der generischen Klasse `List[_T]`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("List",)
+__all__: Final[list[str]] = ["List"]
 
 from io import StringIO
 from typing import Final, Generic, TypeVar
 
 _T = TypeVar("_T")
 
 
@@ -103,15 +103,15 @@
         """
         return self._current is not None
 
     def next(self) -> None:
         """Falls die Liste nicht leer ist, es ein aktuelles Objekt gibt und dieses
         nicht das letzte Objekt der Liste ist, wird das dem aktuellen Objekt in
         der Liste folgende Objekt zum aktuellen Objekt, andernfalls gibt es nach
-        Ausführung des Auftrags kein aktuelles Objekt, d.h. `has_access` liefert
+        Ausführung des Auftrags kein aktuelles Objekt, d. h. `has_access` liefert
         den Wert `False`.
         """
         if not self.has_access:
             return
         self._current = self._current.next_node
 
     def to_first(self) -> None:
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_queue.py` & `pynrw-1.4.0/nrw/datastructures/_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation der generischen Klasse `Queue[_T]`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("Queue",)
+__all__: Final[list[str]] = ["Queue"]
 
 from io import StringIO
 from typing import Final, Generic, TypeVar
 
 _T = TypeVar("_T")
 
 
@@ -40,15 +40,15 @@
     @next_node.setter
     def next_node(self, new_next_node: _QueueNode[_T] | None) -> None:
         self._next_node = new_next_node
 
 
 class Queue(Generic[_T]):
     """Objekte der generischen Klasse `Queue` (Warteschlange) verwalten beliebige
-    Objekte nach dem First-In-First-Out-Prinzip, d.h., das
+    Objekte nach dem First-In-First-Out-Prinzip, d. h., das
     zuerst abgelegte Objekt wird als erstes wieder entnommen. Alle Methoden haben
     eine konstante Laufzeit, unabhängig von der Anzahl der verwalteten Objekte.
     """
 
     __slots__: Final[tuple[str, str]] = ("_head", "_tail")
     __hash__ = None  # type: ignore[assignment]
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_stack.py` & `pynrw-1.4.0/nrw/datastructures/_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation der generischen Klasse `Stack[_T]`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("Stack",)
+__all__: Final[list[str]] = ["Stack"]
 
 from io import StringIO
 from typing import Final, Generic, TypeVar
 
 _T = TypeVar("_T")
 
 
@@ -40,15 +40,15 @@
     @next_node.setter
     def next_node(self, new_next_node: _StackNode[_T] | None) -> None:
         self._next_node = new_next_node
 
 
 class Stack(Generic[_T]):
     """Objekte der generischen Klasse `Stack` (Keller, Stapel) verwalten beliebige
-    Objekte nach dem Last-In-First-Out-Prinzip, d.h., das
+    Objekte nach dem Last-In-First-Out-Prinzip, d. h., das
     zuletzt abgelegte Objekt wird als erstes wieder entnommen. Alle Methoden
     haben eine konstante Laufzeit, unabhängig von der Anzahl der verwalteten
     Objekte.
     """
 
     __slots__: Final[tuple[str]] = ("_head",)
     __hash__ = None  # type: ignore[assignment]
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_utils.py` & `pynrw-1.4.0/nrw/datastructures/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__all__: Final[tuple[str, ...]] = ("display_binary_node",)
+__all__: Final[list[str]] = ["display_binary_node"]
 
 from typing import TYPE_CHECKING, Final, TypeVar
 
 if TYPE_CHECKING:
     from nrw.datastructures._binary_search_tree import _BSTNode
     from nrw.datastructures._binary_tree import _BTNode
     from nrw.datastructures._comparable_content import ComparableContentT
```

### Comparing `pynrw-1.3.0/nrw/datastructures/_vertex.py` & `pynrw-1.4.0/nrw/datastructures/_vertex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation der Klasse `Vertex`."""
 
 from __future__ import annotations
 
-__all__: Final[tuple[str]] = ("Vertex",)
+__all__: Final[list[str]] = ["Vertex"]
 
 from typing import Final
 
 
 class Vertex:
     """Die Klasse Vertex stellt einen einzelnen Knoten eines Graphen dar. Jedes Objekt
     dieser Klasse verfügt über eine im Graphen eindeutige ID als String und kann diese
```

### Comparing `pynrw-1.3.0/pynrw.egg-info/PKG-INFO` & `pynrw-1.4.0/pynrw.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.3.0
+Version: 1.4.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: pyodbc; platform_python_implementation == "CPython"
 Requires-Dist: pypyodbc; platform_python_implementation == "PyPy"
+Requires-Dist: typing_extensions>=4.4.0; python_version < "3.12"
 
 # pynrw
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/realshouzy/pynrw/main.svg)](https://results.pre-commit.ci/latest/github/realshouzy/pynrw/main)
 [![pylint status](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml)
 [![test status](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml)
 [![CodeQL](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml)
@@ -87,15 +88,15 @@
 - [`Queue`](/nrw/datastructures/_queue.py)
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
-Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
+Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d. h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
 
 Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar) `ComparableContentT` zur Verfügung.
 
 Außerdem implementieren die Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht (besonders für `Binary(Search)Tree`) und `__repr__`, welches eine grobe Idee der internen Strukture gibt, z.B.:
 
 ```python
 from nrw.datastructures import BinarySearchTree
@@ -156,14 +157,24 @@
 Hierbei ist zu beachten, dass der `DatabaseConnector` für MSAccess den Microsoft Access Driver benötigt und passwortgeschützte Datenbanken nicht unterstüzt.
 Des weiteren gilt für `QueryResult`, dass die Daten und die Spaltentypen nicht unbedingt als String wiedergegeben werden. Die Daten werden als Python-Äquivalenten Datentypen wiedergegeben, und für die Spaltentypen gilt:
 
 - SQLite: immer `None`, da SQLite dynamisch typisiert ist
 - MySQL: die entsprechenden Datentypen von MySQL als String
 - MSAccess: die entsprechenden Datentypen (Klassen) von Python
 
+### Netzklassen
+
+Die Netzklassen sind ebenfalls semantisch identisch zu den Netzklassen des Landes. Diese sind in [`nrw.network`](/nrw/network/) zu definiert:
+
+- [`Connection`](/nrw/network/_connection.py)
+- [`Client`](/nrw/network/_client.py)
+- [`Server`](/nrw/network/_server.py)
+
+Die letzteren beiden sind [`ABCs`](https://docs.python.org/3/library/abc.html). Bei diesen weicht die interne Implementation von der Java Implementation des Landes ab, da deren Ansatz nicht eins-zu-eins in Python übertragen werden kann; somit ist der Quellcode für Fortgeschrittene. Nichtsdestotrotz ist die Anwendung und der Funktionsumfang der Selbe wie vom Land.
+
 ### Allgemein
 
 Für mehr Information zu einem beliebigen Objekt kann `help` genutzt werden, z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
```

### Comparing `pynrw-1.3.0/pynrw.egg-info/SOURCES.txt` & `pynrw-1.4.0/pynrw.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,12 +27,17 @@
 nrw/datastructures/_edge.py
 nrw/datastructures/_graph.py
 nrw/datastructures/_list.py
 nrw/datastructures/_queue.py
 nrw/datastructures/_stack.py
 nrw/datastructures/_utils.py
 nrw/datastructures/_vertex.py
+nrw/network/__init__.py
+nrw/network/__init__.pyi
+nrw/network/_client.py
+nrw/network/_connection.py
+nrw/network/_server.py
 pynrw.egg-info/PKG-INFO
 pynrw.egg-info/SOURCES.txt
 pynrw.egg-info/dependency_links.txt
 pynrw.egg-info/requires.txt
 pynrw.egg-info/top_level.txt
```

### Comparing `pynrw-1.3.0/pyproject.toml` & `pynrw-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -89,26 +89,28 @@
   "UP035",
   "UP036",
   "SLF001",
   "FBT001",
   "S101",
   "PYI026",
   "B905",
+  "S311",
 ]
 lint.fixable = ["ALL"]
 lint.unfixable = []
 show-fixes = true
 target-version = "py312"
 line-length = 88
 
 [tool.ruff.lint.extend-per-file-ignores]
-"./tests/*_test.py" = ["SLF001", "D100", "D103", "PLR2004", "D102"]
+"./tests/*_test.py" = ["SLF001", "D100", "D103", "PLR2004", "D102", "D101"]
 "./tests/*.py" = ["D104"]
 "./nrw/database/*.py" = ["BLE001", "PLR0913", "ARG002"]
 "./nrw/database/*.pyi" = ["PLR0913"]
+"./nrw/network/*.py" = ["BLE001"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["nrw"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
@@ -120,17 +122,18 @@
 [tool.bandit]
 skips = ["B101"]
 exclude_dirs = ["tests"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 python_files = ["*_test.py"]
+markers = ["networktest: Run network tests"]
 
 [tool.coverage.run]
-omit = ["./tests/*"]
+omit = ["./tests/*", "./nrw/network/*"]
 plugins = ["covdefaults"]
 
 [tool.coverage.report]
 exclude_also = [
   "except Exception as exception:",
   "if self._connection is None:",
 ]
```


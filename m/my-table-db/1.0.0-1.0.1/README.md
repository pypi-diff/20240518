# Comparing `tmp/my_table_db-1.0.0.tar.gz` & `tmp/my_table_db-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_table_db-1.0.0.tar", last modified: Sat May 18 19:56:12 2024, max compression
+gzip compressed data, was "my_table_db-1.0.1.tar", last modified: Sat May 18 19:59:17 2024, max compression
```

## Comparing `my_table_db-1.0.0.tar` & `my_table_db-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 19:56:12.927886 my_table_db-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-05-18 19:23:10.000000 my_table_db-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3886 2024-05-18 19:56:12.927886 my_table_db-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3648 2024-05-18 19:55:24.000000 my_table_db-1.0.0/README.md
--rw-rw-rw-   0        0        0     1879 2024-05-18 19:32:05.000000 my_table_db-1.0.0/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:56:12.926886 my_table_db-1.0.0/my_table_db.egg-info/
--rw-rw-rw-   0        0        0     3886 2024-05-18 19:56:12.000000 my_table_db-1.0.0/my_table_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-05-18 19:56:12.000000 my_table_db-1.0.0/my_table_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 19:56:12.000000 my_table_db-1.0.0/my_table_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-18 19:56:12.000000 my_table_db-1.0.0/my_table_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 19:56:12.927886 my_table_db-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      374 2024-05-18 19:23:10.000000 my_table_db-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:59:17.684671 my_table_db-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-18 19:23:10.000000 my_table_db-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3941 2024-05-18 19:59:17.683671 my_table_db-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1879 2024-05-18 19:32:05.000000 my_table_db-1.0.1/main.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:59:17.682671 my_table_db-1.0.1/my_table_db.egg-info/
+-rw-rw-rw-   0        0        0     3941 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 19:59:17.684671 my_table_db-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      374 2024-05-18 19:59:13.000000 my_table_db-1.0.1/setup.py
```

### Comparing `my_table_db-1.0.0/LICENSE` & `my_table_db-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.0/PKG-INFO` & `my_table_db-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -51,20 +51,21 @@
 ```shell
 ID:1         |        Name:Alice     |        Salary:50000
 
 ```
 
 ## Пример 2
 
-#### Содержимое таблицы
+Содержимое таблицы
 ```csv
 id  name    salary
 1   Alice   50000
 2   Bob     60000
 ```
+Код с использованием my_table_db
 
 ```python
 import psycopg2
 from my_table_db import my_table_db
 
 def fetch_data():
     conn = None
@@ -75,15 +76,15 @@
             password=...,
             host=...,
             port=...)
         cur = conn.cursor()
         cur.execute("SELECT * FROM employees")
         rows = cur.fetchall()
         for row in rows:
-            print(library('ID', row[0], 'Name', row[1], 'Salary', row[2]))
+            print(my_table_db('ID', row[0], 'Name', row[1], 'Salary', row[2]))
         cur.close()
     except (Exception, psycopg2.DatabaseError) as error:
         print(error)
     finally:
         if conn is not None:
             conn.close()
             print()
@@ -101,13 +102,13 @@
 
 Database connection closed.
 ```
 
 ***
 
 # Заключение
-#### Функция library полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
+#### Функция my_table_db полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
 
 ***
 ### Автор
 
 Автор: k0ng999
```

### Comparing `my_table_db-1.0.0/README.md` & `my_table_db-1.0.1/my_table_db.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: my_table_db
+Version: 1.0.1
+Summary: A small library for conclusion table db
+Author: k0ng999
+Author-email: baydar_14@mail.ru
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Функция Library
 
 Этот Python-скрипт определяет функцию library, которая форматирует набор именованных аргументов и их соответствующих значений в строку. Выходная строка структурирована с определенным форматом, где каждая пара имя-значение разделена символом | и дополнена до выравнивания в столбцах.
 
 ***
 ### Установка
 ` pip install my_table_db `
@@ -41,20 +51,21 @@
 ```shell
 ID:1         |        Name:Alice     |        Salary:50000
 
 ```
 
 ## Пример 2
 
-#### Содержимое таблицы
+Содержимое таблицы
 ```csv
 id  name    salary
 1   Alice   50000
 2   Bob     60000
 ```
+Код с использованием my_table_db
 
 ```python
 import psycopg2
 from my_table_db import my_table_db
 
 def fetch_data():
     conn = None
@@ -65,15 +76,15 @@
             password=...,
             host=...,
             port=...)
         cur = conn.cursor()
         cur.execute("SELECT * FROM employees")
         rows = cur.fetchall()
         for row in rows:
-            print(library('ID', row[0], 'Name', row[1], 'Salary', row[2]))
+            print(my_table_db('ID', row[0], 'Name', row[1], 'Salary', row[2]))
         cur.close()
     except (Exception, psycopg2.DatabaseError) as error:
         print(error)
     finally:
         if conn is not None:
             conn.close()
             print()
@@ -91,13 +102,13 @@
 
 Database connection closed.
 ```
 
 ***
 
 # Заключение
-#### Функция library полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
+#### Функция my_table_db полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
 
 ***
 ### Автор
 
 Автор: k0ng999
```

### Comparing `my_table_db-1.0.0/main.py` & `my_table_db-1.0.1/main.py`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.0/my_table_db.egg-info/PKG-INFO` & `my_table_db-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: my_table_db
-Version: 1.0.0
-Summary: A small library for conclusion table db
-Author: k0ng999
-Author-email: baydar_14@mail.ru
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Функция Library
 
 Этот Python-скрипт определяет функцию library, которая форматирует набор именованных аргументов и их соответствующих значений в строку. Выходная строка структурирована с определенным форматом, где каждая пара имя-значение разделена символом | и дополнена до выравнивания в столбцах.
 
 ***
 ### Установка
 ` pip install my_table_db `
@@ -51,20 +41,21 @@
 ```shell
 ID:1         |        Name:Alice     |        Salary:50000
 
 ```
 
 ## Пример 2
 
-#### Содержимое таблицы
+Содержимое таблицы
 ```csv
 id  name    salary
 1   Alice   50000
 2   Bob     60000
 ```
+Код с использованием my_table_db
 
 ```python
 import psycopg2
 from my_table_db import my_table_db
 
 def fetch_data():
     conn = None
@@ -75,15 +66,15 @@
             password=...,
             host=...,
             port=...)
         cur = conn.cursor()
         cur.execute("SELECT * FROM employees")
         rows = cur.fetchall()
         for row in rows:
-            print(library('ID', row[0], 'Name', row[1], 'Salary', row[2]))
+            print(my_table_db('ID', row[0], 'Name', row[1], 'Salary', row[2]))
         cur.close()
     except (Exception, psycopg2.DatabaseError) as error:
         print(error)
     finally:
         if conn is not None:
             conn.close()
             print()
@@ -101,13 +92,13 @@
 
 Database connection closed.
 ```
 
 ***
 
 # Заключение
-#### Функция library полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
+#### Функция my_table_db полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
 
 ***
 ### Автор
 
 Автор: k0ng999
```


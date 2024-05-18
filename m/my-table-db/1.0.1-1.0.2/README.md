# Comparing `tmp/my_table_db-1.0.1.tar.gz` & `tmp/my_table_db-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_table_db-1.0.1.tar", last modified: Sat May 18 19:59:17 2024, max compression
+gzip compressed data, was "my_table_db-1.0.2.tar", last modified: Sat May 18 20:22:52 2024, max compression
```

## Comparing `my_table_db-1.0.1.tar` & `my_table_db-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 19:59:17.684671 my_table_db-1.0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-18 19:23:10.000000 my_table_db-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3941 2024-05-18 19:59:17.683671 my_table_db-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.1/README.md
--rw-rw-rw-   0        0        0     1879 2024-05-18 19:32:05.000000 my_table_db-1.0.1/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:59:17.682671 my_table_db-1.0.1/my_table_db.egg-info/
--rw-rw-rw-   0        0        0     3941 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-18 19:59:17.000000 my_table_db-1.0.1/my_table_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 19:59:17.684671 my_table_db-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      374 2024-05-18 19:59:13.000000 my_table_db-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:22:52.560645 my_table_db-1.0.2/
+-rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3941 2024-05-18 20:22:52.559645 my_table_db-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1906 2024-05-18 20:22:33.000000 my_table_db-1.0.2/main.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:22:52.558643 my_table_db-1.0.2/my_table_db.egg-info/
+-rw-rw-rw-   0        0        0     3941 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 20:22:52.560645 my_table_db-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-18 20:22:50.000000 my_table_db-1.0.2/setup.py
```

### Comparing `my_table_db-1.0.1/LICENSE` & `my_table_db-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `my_table_db-1.0.1/PKG-INFO` & `my_table_db-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `my_table_db-1.0.1/README.md` & `my_table_db-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.1/main.py` & `my_table_db-1.0.2/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+__all__ = ['my_table_bd']
 def my_table_bd(name_arg1=None, arg1=None, name_arg2=None, arg2=None, name_arg3=None, arg3=None, arg4=None,
             name_arg4=None, name_arg5=None, arg5=None, name_arg6=None, arg6=None, name_arg7=None, arg7=None):
     if (name_arg1 and name_arg2 and name_arg3 and name_arg4 and name_arg5 and name_arg6 and name_arg7) is not None:
         return (
             f'{name_arg1}:{str(arg1):10}{'|':9}{name_arg2}:{str(arg2):10}{'|':9}{name_arg3}:{str(arg3):10}{'|':9}{arg4}:{str(name_arg4):10}{'|':9}{arg5}:{str(name_arg5):10}{'|':9}{arg6}:{str(name_arg6):10}{'|':9}{arg7}:{str(name_arg7):10}')
     elif (name_arg1 and name_arg2 and name_arg3 and name_arg4 and name_arg5 and name_arg6) is not None:
         return (
```

### Comparing `my_table_db-1.0.1/my_table_db.egg-info/PKG-INFO` & `my_table_db-1.0.2/my_table_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


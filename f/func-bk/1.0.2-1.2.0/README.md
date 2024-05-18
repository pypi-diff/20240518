# Comparing `tmp/func_bk-1.0.2.tar.gz` & `tmp/func_bk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.0.2.tar", last modified: Sat Apr 20 12:52:51 2024, max compression
+gzip compressed data, was "func_bk-1.2.0.tar", last modified: Sat May 18 13:28:55 2024, max compression
```

## Comparing `func_bk-1.0.2.tar` & `func_bk-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 12:52:51.640498 func_bk-1.0.2/
--rw-rw-rw-   0        0        0     1783 2024-04-20 12:52:51.639499 func_bk-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1566 2024-04-20 12:50:24.000000 func_bk-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 12:52:51.634498 func_bk-1.0.2/func_bk/
--rw-rw-rw-   0        0        0     2876 2024-04-20 12:50:17.000000 func_bk-1.0.2/func_bk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:52:51.639499 func_bk-1.0.2/func_bk.egg-info/
--rw-rw-rw-   0        0        0     1783 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-14 13:47:26.000000 func_bk-1.0.2/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-04-20 12:52:51.640498 func_bk-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-04-14 13:46:14.000000 func_bk-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 13:28:55.546787 func_bk-1.2.0/
+-rw-rw-rw-   0        0        0     2701 2024-05-18 13:28:55.545787 func_bk-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2484 2024-05-18 13:15:48.000000 func_bk-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 13:28:55.539787 func_bk-1.2.0/func_bk/
+-rw-rw-rw-   0        0        0     4121 2024-05-18 13:06:54.000000 func_bk-1.2.0/func_bk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 13:28:55.544788 func_bk-1.2.0/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     2701 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-14 13:47:26.000000 func_bk-1.2.0/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-18 13:28:55.546787 func_bk-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-05-18 13:16:54.000000 func_bk-1.2.0/setup.py
```

### Comparing `func_bk-1.0.2/PKG-INFO` & `func_bk-1.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.0.2
+Version: 1.2.0
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
@@ -22,30 +22,65 @@
 
 
 find(lst,sim) - lst=list sim=obj for searching, find obj inlist and return he index
  
 listrand(min,max,kol): return random list
 
 
-def IsKeyInDict(data, key): return bool: isvalid key in data
+IsKeyInDict(data, key): return bool: isvalid key in data
 
 
 
-def stepen(number,stepan): degree of number
+stepen(number,stepan): degree of number
 	
-def faktorial(number): you know
+faktorial(number): you know
 	
-def chibo(number): number of chibonachi
+chibo(number): number of chibonachi
 	
-def summa(number):summ 
+summa(number):summ 
 example:
     a=12
     print(summ(a))
 this code return 3
 
+
+
+call_methods_by_partial_name(class_instance, partial_name, *args, **kwargs): use all METHODS(function in class) with partial name
+
+
+CFBPN=call_methods_by_partial_name
+Mcall=call_methods_by_partial_name
+
+
+
+call_functions_by_partial_name(partial_name, *args, **kwargs): use all function with partial name
+
+CFBPN=call_functions_by_partial_name
+Fcall=call_functions_by_partial_name
+
+
+
+
+function for django:
+
+
+allpath(route: str, view, name: str): It is used to create a list of URL routes that support both the presence and absence of a trailing slash
+
+example_1:
+    urlpatterns = [
+        path('', views.index, name='index'),
+        *allpath('post/', views.post.as_view(), name='post'), ]
+
+example_2:
+    urlpatterns = [
+        path('', views.index, name='index'),
+        *allpath('post', views.post.as_view(), name='post'), ]
+
+note: since it returns the list, you need to use * to unpack the list
+
 class for django:
 
 
 Color:
     abstract model
     for inheritance models add to model variable: color and function: isdarker, iswhite, hexrgb, rgbtofloat
```

### Comparing `func_bk-1.0.2/func_bk.egg-info/PKG-INFO` & `func_bk-1.2.0/func_bk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.0.2
+Version: 1.2.0
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
@@ -22,30 +22,65 @@
 
 
 find(lst,sim) - lst=list sim=obj for searching, find obj inlist and return he index
  
 listrand(min,max,kol): return random list
 
 
-def IsKeyInDict(data, key): return bool: isvalid key in data
+IsKeyInDict(data, key): return bool: isvalid key in data
 
 
 
-def stepen(number,stepan): degree of number
+stepen(number,stepan): degree of number
 	
-def faktorial(number): you know
+faktorial(number): you know
 	
-def chibo(number): number of chibonachi
+chibo(number): number of chibonachi
 	
-def summa(number):summ 
+summa(number):summ 
 example:
     a=12
     print(summ(a))
 this code return 3
 
+
+
+call_methods_by_partial_name(class_instance, partial_name, *args, **kwargs): use all METHODS(function in class) with partial name
+
+
+CFBPN=call_methods_by_partial_name
+Mcall=call_methods_by_partial_name
+
+
+
+call_functions_by_partial_name(partial_name, *args, **kwargs): use all function with partial name
+
+CFBPN=call_functions_by_partial_name
+Fcall=call_functions_by_partial_name
+
+
+
+
+function for django:
+
+
+allpath(route: str, view, name: str): It is used to create a list of URL routes that support both the presence and absence of a trailing slash
+
+example_1:
+    urlpatterns = [
+        path('', views.index, name='index'),
+        *allpath('post/', views.post.as_view(), name='post'), ]
+
+example_2:
+    urlpatterns = [
+        path('', views.index, name='index'),
+        *allpath('post', views.post.as_view(), name='post'), ]
+
+note: since it returns the list, you need to use * to unpack the list
+
 class for django:
 
 
 Color:
     abstract model
     for inheritance models add to model variable: color and function: isdarker, iswhite, hexrgb, rgbtofloat
```


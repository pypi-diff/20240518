# Comparing `tmp/otonagai_dl-1.0.4.tar.gz` & `tmp/otonagai_dl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otonagai_dl-1.0.4.tar", max compression
+gzip compressed data, was "otonagai_dl-1.0.5.tar", max compression
```

## Comparing `otonagai_dl-1.0.4.tar` & `otonagai_dl-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1092 2024-05-18 19:18:50.337113 otonagai_dl-1.0.4/LICENSE
--rw-r--r--   0        0        0      226 2024-05-17 06:29:48.933720 otonagai_dl-1.0.4/otonagai_dl/main.py
--rw-r--r--   0        0        0        0 2024-05-07 09:23:59.995430 otonagai_dl-1.0.4/otonagai_dl/src/__init__.py
--rw-r--r--   0        0        0     7945 2024-05-18 19:20:10.491876 otonagai_dl-1.0.4/otonagai_dl/src/controller.py
--rw-r--r--   0        0        0        0 2024-05-07 09:25:40.767261 otonagai_dl-1.0.4/otonagai_dl/src/hobby_link_jp_scraper/__init__.py
--rw-r--r--   0        0        0     1347 2024-05-17 05:46:07.038979 otonagai_dl-1.0.4/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py
--rw-r--r--   0        0        0     4383 2024-05-17 06:32:03.828672 otonagai_dl-1.0.4/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py
--rw-r--r--   0        0        0     2554 2024-05-15 10:46:22.439118 otonagai_dl-1.0.4/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py
--rw-r--r--   0        0        0      380 2024-05-18 13:24:14.953354 otonagai_dl-1.0.4/otonagai_dl/src/log_system.py
--rw-r--r--   0        0        0     3695 2024-05-18 19:24:33.402713 otonagai_dl-1.0.4/otonagai_dl/src/menu.py
--rw-r--r--   0        0        0     9271 2024-05-18 19:42:05.305401 otonagai_dl-1.0.4/otonagai_dl/src/model.py
--rw-r--r--   0        0        0     3314 2024-05-18 19:24:17.225266 otonagai_dl-1.0.4/otonagai_dl/src/utils.py
--rw-r--r--   0        0        0     7860 2024-05-18 19:19:56.618750 otonagai_dl-1.0.4/otonagai_dl/src/view.py
--rw-r--r--   0        0        0      561 2024-05-18 19:44:05.983854 otonagai_dl-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      695 2024-05-17 06:43:17.878317 otonagai_dl-1.0.4/README.md
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 otonagai_dl-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-18 19:18:50.337113 otonagai_dl-1.0.5/LICENSE
+-rw-r--r--   0        0        0      226 2024-05-17 06:29:48.933720 otonagai_dl-1.0.5/otonagai_dl/main.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:23:59.995430 otonagai_dl-1.0.5/otonagai_dl/src/__init__.py
+-rw-r--r--   0        0        0     8001 2024-05-18 20:10:54.421099 otonagai_dl-1.0.5/otonagai_dl/src/controller.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:25:40.767261 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/__init__.py
+-rw-r--r--   0        0        0     1347 2024-05-17 05:46:07.038979 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py
+-rw-r--r--   0        0        0     4383 2024-05-17 06:32:03.828672 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py
+-rw-r--r--   0        0        0     2554 2024-05-15 10:46:22.439118 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py
+-rw-r--r--   0        0        0      380 2024-05-18 13:24:14.953354 otonagai_dl-1.0.5/otonagai_dl/src/log_system.py
+-rw-r--r--   0        0        0     4103 2024-05-18 20:17:29.741962 otonagai_dl-1.0.5/otonagai_dl/src/menu.py
+-rw-r--r--   0        0        0     9271 2024-05-18 19:42:05.305401 otonagai_dl-1.0.5/otonagai_dl/src/model.py
+-rw-r--r--   0        0        0     3314 2024-05-18 20:16:26.731409 otonagai_dl-1.0.5/otonagai_dl/src/utils.py
+-rw-r--r--   0        0        0     7860 2024-05-18 19:19:56.618750 otonagai_dl-1.0.5/otonagai_dl/src/view.py
+-rw-r--r--   0        0        0      561 2024-05-18 19:50:44.829733 otonagai_dl-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      695 2024-05-17 06:43:17.878317 otonagai_dl-1.0.5/README.md
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 otonagai_dl-1.0.5/PKG-INFO
```

### Comparing `otonagai_dl-1.0.4/LICENSE` & `otonagai_dl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/controller.py` & `otonagai_dl-1.0.5/otonagai_dl/src/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         search_result, flag = basic_or_advanced_search(self.model)
 
         # check if data is available in the db
         if flag is None:
             self.no_data_warning(search_result)
 
         # clear the console
-        self.console.clear()
+        os.system("cls" if os.name == "nt" else "clear")
 
         with Live(
             self.view.create_table(self.console, search_result, selected),
             auto_refresh=False,
             screen=True,
         ) as live:
 
@@ -170,15 +170,15 @@
 
     def navigate_table(self):
         selected = 0
 
         log_result = self.model.view_table()
         self.no_data_warning(log_result)
 
-        self.console.clear()
+        os.system("cls" if os.name == "nt" else "clear")
         with Live(
             self.view.create_table(
                 self.console,
                 log_result,
                 selected,
             ),
             auto_refresh=False,
```

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py` & `otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py` & `otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py` & `otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/menu.py` & `otonagai_dl-1.0.5/otonagai_dl/src/menu.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from InquirerPy import inquirer
 from .controller import search_table_navigation, log_table_navigation
 import sys
 from .hobby_link_jp_scraper.hlj_ui import HLJ_scraper_ui
 from .model import gunpla_log_db, gunpla_search_db, web_to_db_bridge
-from .view import Search_Table_View, Log_Table_View
+from .view import Search_Table_View, Log_Table_View, no_downloads
 from .utils import (
     use_edit_file,
     extract_from_page_links,
     filter_urls,
     add_to_search_db,
     extract_urls_from_file,
     add_page_nos,
@@ -42,69 +42,75 @@
             vi_mode=True,
         ).execute()
 
         log_msg(f'Selected "{menu_choice}"')
 
         if menu_choice == "Merchandise Database":
 
-            console.clear()
+            os.system("cls" if os.name == "nt" else "clear")
 
             # Open up the search database
             search_view = Search_Table_View(search_db.view_table())
             search_table_navigation(
                 console=console, model=search_db, view=search_view
             ).navigate_table()
 
         elif menu_choice == "Merchandise Log":
 
-            console.clear()
+            os.system("cls" if os.name == "nt" else "clear")
 
             # Open up the log database
             log_view = Log_Table_View(log_db.view_table())
             log_table_navigation(
                 model=log_db, view=log_view, console=console
             ).navigate_table()
 
         elif menu_choice == "URLs to download":
-            console.clear()
+            os.system("cls" if os.name == "nt" else "clear")
             # open the file that contains the urls
-            use_edit_file(console, inquirer)
+            use_edit_file(inquirer)
 
         elif menu_choice == "Exit":
 
             sys.exit()
 
         # Extract the product info from the product urls
         elif menu_choice == "Extract Merch info":
-            console.clear()
+            os.system("cls" if os.name == "nt" else "clear")
 
             text_urls = extract_urls_from_file()
+            text_urls = set(text_urls)
 
             # page_urls : URLs that consist of multiple pages
             # non_page_urls : URLs for a single product
             page_urls, non_page_urls = filter_urls(text_urls)
 
             for url in page_urls:
 
-                print(f"Please add the pages to extract the products from {url}\n")
-                start_page = input("Please enter the starting page : ")
-                end_page = input("Please enter the ending page : ")
-
-                # Extract the product urls from each page
-                start_page, end_page = add_page_nos(start_page, end_page)
-                log_msg(
-                    f"{url} starting with page {start_page} and ending with {end_page}"
-                )
-                end_page += 1
-                if start_page is not None and end_page is not None:
-                    non_page_urls.extend(
-                        extract_from_page_links(
-                            url, start_page=start_page, end_page=end_page
-                        )
+                try:
+                    print(
+                        f"\n Please add the pages to extract the products from {url}\n"
+                    )
+                    start_page = int(input("Please enter the starting page : "))
+                    end_page = int(input("Please enter the ending page : "))
+
+                    # Extract the product urls from each page
+                    start_page, end_page = add_page_nos(start_page, end_page)
+                    log_msg(
+                        f"{url} starting with page {start_page} and ending with {end_page}"
                     )
+                    end_page += 1
+                    if start_page is not None and end_page is not None:
+                        non_page_urls.extend(
+                            extract_from_page_links(
+                                url, start_page=start_page, end_page=end_page
+                            )
+                        )
+                except Exception:
+                    Console().print(no_downloads())
 
             # add all the product information to the search database
             add_to_search_db(
                 extracted_urls=non_page_urls,
                 scraper_ui=HLJ_scraper_ui(),
                 search_db_conn=web_to_db_bridge(),
             )
```

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/model.py` & `otonagai_dl-1.0.5/otonagai_dl/src/model.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/utils.py` & `otonagai_dl-1.0.5/otonagai_dl/src/utils.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/otonagai_dl/src/view.py` & `otonagai_dl-1.0.5/otonagai_dl/src/view.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/pyproject.toml` & `otonagai_dl-1.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "otonagai-dl"
-version = "1.0.4"
+version = "1.0.5"
 description = "A basic CLI tool to keep track of your favourite anime/manga/comics/pop culture merchandise"
 authors = ["Clavin Dsouza <clavind12@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `otonagai_dl-1.0.4/README.md` & `otonagai_dl-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.4/PKG-INFO` & `otonagai_dl-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otonagai-dl
-Version: 1.0.4
+Version: 1.0.5
 Summary: A basic CLI tool to keep track of your favourite anime/manga/comics/pop culture merchandise
 License: MIT
 Author: Clavin Dsouza
 Author-email: clavind12@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


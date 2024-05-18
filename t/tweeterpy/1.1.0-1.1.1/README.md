# Comparing `tmp/tweeterpy-1.1.0.tar.gz` & `tmp/tweeterpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-1.1.0.tar", last modified: Fri May 17 15:34:54 2024, max compression
+gzip compressed data, was "tweeterpy-1.1.1.tar", last modified: Sat May 18 07:28:36 2024, max compression
```

## Comparing `tweeterpy-1.1.0.tar` & `tweeterpy-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3967 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1499 2024-05-17 15:30:12.000000 tweeterpy-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:34:53.989662 tweeterpy-1.1.0/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.1.0/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     8241 2024-01-02 14:26:34.000000 tweeterpy-1.1.0/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0     2505 2023-10-11 13:49:03.000000 tweeterpy-1.1.0/tweeterpy/config.py
--rw-rw-rw-   0        0        0     3855 2024-05-17 15:23:46.000000 tweeterpy-1.1.0/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.1.0/tweeterpy/logging_util.py
--rw-rw-rw-   0        0        0     9024 2023-10-10 14:44:59.000000 tweeterpy-1.1.0/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1984 2024-01-04 12:34:59.000000 tweeterpy-1.1.0/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2481 2023-09-07 09:39:56.000000 tweeterpy-1.1.0/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    32367 2024-05-17 15:23:49.000000 tweeterpy-1.1.0/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0    15955 2024-05-17 15:29:39.000000 tweeterpy-1.1.0/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3967 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 07:28:36.492667 tweeterpy-1.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3967 2024-05-18 07:28:36.492667 tweeterpy-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 07:28:36.492667 tweeterpy-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2024-05-18 07:25:08.000000 tweeterpy-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:28:36.445787 tweeterpy-1.1.1/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.1.1/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     8241 2024-01-02 14:26:34.000000 tweeterpy-1.1.1/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0     2505 2023-10-11 13:49:03.000000 tweeterpy-1.1.1/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     3855 2024-05-17 15:23:46.000000 tweeterpy-1.1.1/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.1.1/tweeterpy/logging_util.py
+-rw-rw-rw-   0        0        0     9024 2023-10-10 14:44:59.000000 tweeterpy-1.1.1/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1984 2024-01-04 12:34:59.000000 tweeterpy-1.1.1/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2481 2023-09-07 09:39:56.000000 tweeterpy-1.1.1/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    32367 2024-05-17 15:23:49.000000 tweeterpy-1.1.1/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0    16546 2024-05-18 07:23:11.000000 tweeterpy-1.1.1/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:28:36.492667 tweeterpy-1.1.1/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3967 2024-05-18 07:28:36.000000 tweeterpy-1.1.1/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-18 07:28:36.000000 tweeterpy-1.1.1/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 07:28:36.000000 tweeterpy-1.1.1/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2024-05-18 07:28:36.000000 tweeterpy-1.1.1/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 07:28:36.000000 tweeterpy-1.1.1/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-1.1.0/LICENSE` & `tweeterpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/PKG-INFO` & `tweeterpy-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.0 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.1 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tweeterpy-1.1.0/README.md` & `tweeterpy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/setup.py` & `tweeterpy-1.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-1.1.0/tweeterpy/api_util.py` & `tweeterpy-1.1.1/tweeterpy/api_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/config.py` & `tweeterpy-1.1.1/tweeterpy/config.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/constants.py` & `tweeterpy-1.1.1/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/logging_util.py` & `tweeterpy-1.1.1/tweeterpy/logging_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/login_util.py` & `tweeterpy-1.1.1/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/request_util.py` & `tweeterpy-1.1.1/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/session_util.py` & `tweeterpy-1.1.1/tweeterpy/session_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/tweeterpy.py` & `tweeterpy-1.1.1/tweeterpy/tweeterpy.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.0/tweeterpy/util.py` & `tweeterpy-1.1.1/tweeterpy/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,17 +94,23 @@
         return guest_token
     except Exception as error:
         logger.error(error)
         raise
 
 def handle_x_migration(session):
     home_page = None
+    migration_redirection_regex = re.compile(r"""(http(?:s)?://(?:www\.)?(twitter|x){1}\.com(/x)?/migrate([/?])?tok=[a-zA-Z0-9%\-_]+)+""", re.VERBOSE)
     try:
         response = session.request(method="GET", url=Path.BASE_URL)
         home_page = bs4.BeautifulSoup(response.content, 'lxml')
+        migration_url = home_page.select_one("meta[http-equiv='refresh']")
+        migration_redirection_url = re.search(migration_redirection_regex, str(migration_url)) or re.search(migration_redirection_regex, str(response.content))
+        if migration_redirection_url:
+            response = session.request(method="GET", url=migration_redirection_url.group(0))
+            home_page = bs4.BeautifulSoup(response.content, 'lxml')
         migration_form = home_page.select_one("form[name='f']") or home_page.select_one(f"form[action='{Path.X_MIGRATE_URL}']")
         if migration_form:
             url = migration_form.attrs.get("action", Path.X_MIGRATE_URL)
             method = migration_form.attrs.get("method", "POST")
             request_payload = {input_field.get("name"):input_field.get("value") for input_field in migration_form.select("input")}
             response = session.request(method=method, url=url, data=request_payload)
             home_page = bs4.BeautifulSoup(response.content, 'lxml')
```

### Comparing `tweeterpy-1.1.0/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-1.1.1/tweeterpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.0 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.1 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```


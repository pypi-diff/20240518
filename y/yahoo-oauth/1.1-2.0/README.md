# Comparing `tmp/yahoo_oauth-1.1.tar.gz` & `tmp/yahoo_oauth-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yahoo_oauth-1.1.tar", last modified: Thu Oct  1 14:54:06 2020, max compression
+gzip compressed data, was "yahoo_oauth-2.0.tar", last modified: Tue Oct  4 14:55:19 2022, max compression
```

## Comparing `yahoo_oauth-1.1.tar` & `yahoo_oauth-2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 jkouka    (1000) jkouka    (1000)        0 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)     3893 2020-03-14 21:47:59.000000 yahoo_oauth-1.1/README.rst
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)       79 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/setup.cfg
-drwxrwxr-x   0 jkouka    (1000) jkouka    (1000)        0 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/yahoo_oauth/
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)      129 2020-03-14 22:12:38.000000 yahoo_oauth-1.1/yahoo_oauth/__init__.py
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)     2058 2020-05-24 14:20:51.000000 yahoo_oauth-1.1/yahoo_oauth/utils.py
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)     8812 2020-10-01 14:18:48.000000 yahoo_oauth-1.1/yahoo_oauth/oauth.py
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)      725 2020-03-14 21:47:59.000000 yahoo_oauth-1.1/yahoo_oauth/logger.py
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)       63 2020-03-14 21:58:33.000000 yahoo_oauth-1.1/MANIFEST.in
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)     5620 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/PKG-INFO
-drwxrwxr-x   0 jkouka    (1000) jkouka    (1000)        0 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/yahoo_oauth.egg-info/
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)      331 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/yahoo_oauth.egg-info/SOURCES.txt
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)       12 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/yahoo_oauth.egg-info/requires.txt
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)        1 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/yahoo_oauth.egg-info/dependency_links.txt
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)     5620 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/yahoo_oauth.egg-info/PKG-INFO
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)       12 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/yahoo_oauth.egg-info/top_level.txt
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)       84 2020-10-01 14:54:06.000000 yahoo_oauth-1.1/version.py
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)     1983 2020-10-01 14:54:04.000000 yahoo_oauth-1.1/setup.py
--rw-rw-r--   0 jkouka    (1000) jkouka    (1000)       12 2020-03-14 21:57:21.000000 yahoo_oauth-1.1/requirements.txt
+drwxrwxr-x   0 yosuke    (1000) yosuke    (1000)        0 2022-10-04 14:55:19.222472 yahoo_oauth-2.0/
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)     1079 2020-03-14 21:47:59.000000 yahoo_oauth-2.0/LICENSE
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)       63 2020-03-14 21:58:33.000000 yahoo_oauth-2.0/MANIFEST.in
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)     4823 2022-10-04 14:55:19.222472 yahoo_oauth-2.0/PKG-INFO
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)     3893 2020-03-14 21:47:59.000000 yahoo_oauth-2.0/README.rst
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)       12 2020-03-14 21:57:21.000000 yahoo_oauth-2.0/requirements.txt
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)       79 2022-10-04 14:55:19.226472 yahoo_oauth-2.0/setup.cfg
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)     1983 2022-10-04 14:50:20.000000 yahoo_oauth-2.0/setup.py
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)       84 2022-10-04 14:55:19.000000 yahoo_oauth-2.0/version.py
+drwxrwxr-x   0 yosuke    (1000) yosuke    (1000)        0 2022-10-04 14:55:19.222472 yahoo_oauth-2.0/yahoo_oauth/
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)      129 2020-03-14 22:12:38.000000 yahoo_oauth-2.0/yahoo_oauth/__init__.py
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)      725 2020-03-14 21:47:59.000000 yahoo_oauth-2.0/yahoo_oauth/logger.py
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)     8933 2022-10-04 14:50:20.000000 yahoo_oauth-2.0/yahoo_oauth/oauth.py
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)     2082 2022-10-04 14:50:20.000000 yahoo_oauth-2.0/yahoo_oauth/utils.py
+drwxrwxr-x   0 yosuke    (1000) yosuke    (1000)        0 2022-10-04 14:55:19.222472 yahoo_oauth-2.0/yahoo_oauth.egg-info/
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)     4823 2022-10-04 14:55:19.000000 yahoo_oauth-2.0/yahoo_oauth.egg-info/PKG-INFO
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)      339 2022-10-04 14:55:19.000000 yahoo_oauth-2.0/yahoo_oauth.egg-info/SOURCES.txt
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)        1 2022-10-04 14:55:19.000000 yahoo_oauth-2.0/yahoo_oauth.egg-info/dependency_links.txt
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)       12 2022-10-04 14:55:19.000000 yahoo_oauth-2.0/yahoo_oauth.egg-info/requires.txt
+-rw-rw-r--   0 yosuke    (1000) yosuke    (1000)       12 2022-10-04 14:55:19.000000 yahoo_oauth-2.0/yahoo_oauth.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yahoo_oauth-1.1/README.rst` & `yahoo_oauth-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `yahoo_oauth-1.1/yahoo_oauth/utils.py` & `yahoo_oauth-2.0/yahoo_oauth/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         AUTHORIZE_TOKEN_URL = "https://api.login.yahoo.com/oauth2/request_auth",
         ACCESS_TOKEN_URL = "https://api.login.yahoo.com/oauth2/get_token"
     )
 }
 
 CALLBACK_URI = 'oob'
 
+STORE_FILE_FLAG = True
+
 def get_file_extension(filename):
     return os.path.splitext(filename)
 
 def get_data(filename):
     """Calls right function according to file extension
     """
     name, ext = get_file_extension(filename)
```

### Comparing `yahoo_oauth-1.1/yahoo_oauth/oauth.py` & `yahoo_oauth-2.0/yahoo_oauth/oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import logging
 import webbrowser
 
 import base64
 
 from rauth.utils import parse_utf8_qsl
 
-from yahoo_oauth.utils import services, CALLBACK_URI
+from yahoo_oauth.utils import services, CALLBACK_URI, STORE_FILE_FLAG
 from yahoo_oauth.utils import get_data, write_data
 from yahoo_oauth.logger import YahooLogger
 
 logging.setLoggerClass(YahooLogger)
 logger = logging.getLogger('yahoo_oauth')
 logger.propagate = False
 
@@ -49,14 +49,15 @@
             self.consumer_key = consumer_key
             self.consumer_secret = consumer_secret
 
         vars(self).update(kwargs)
 
         self.oauth_version = oauth_version
         self.callback_uri = vars(self).get('callback_uri', CALLBACK_URI)
+        self.store_file = vars(self).get('store_file', STORE_FILE_FLAG)
 
         if 'browser_callback' in kwargs.keys():
             self.browser_callback = kwargs.get('browser_callback')
         else:
             self.browser_callback = True
 
         # Init OAuth
@@ -93,15 +94,16 @@
 
         # Getting session
         if self.oauth_version == 'oauth1':
             self.session = self.oauth.get_session((self.access_token, self.access_token_secret))
         else:
             self.session = self.oauth.get_session(token=self.access_token)
 
-        write_data(data, vars(self).get('from_file', 'secrets.json'))
+        if self.store_file:
+            write_data(data, vars(self).get('from_file', 'secrets.json'))
 
     def handler(self,):
         """* get request token if OAuth1
             * Get user authorization
             * Get access token
         """
```

### Comparing `yahoo_oauth-1.1/yahoo_oauth/logger.py` & `yahoo_oauth-2.0/yahoo_oauth/logger.py`

 * *Files identical despite different names*

### Comparing `yahoo_oauth-1.1/PKG-INFO` & `yahoo_oauth-2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,126 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yahoo_oauth
-Version: 1.1
+Version: 2.0
 Summary: Python Yahoo OAuth Library. Supports OAuth1 and OAuth2
 Home-page: https://github.com/josuebrunel/yahoo-oauth
 Author: Josue Kouka
 Author-email: josuebrunel@gmail.com
 License: MIT
-Download-URL: https://github.com/josuebrunel/yahoo-oauth/archive/1.1.tar.gz
-Description: yahoo\_oauth
-        ============
-        
-        |Build Status| |Documentation Status|
-        
-        Yahoo\_OAuth is a very easy to use OAuth python library for Yahoo! APIs.
-        
-        Installation
-        ------------
-        
-        .. code:: python
-        
-            pip install yahoo_oauth
-        
-        Quickstart
-        ----------
-        
-        Wether you use **OAuth1** or **OAuth2**, only **2** parameters are
-        required.
-        
-        -  ***consumer*\ key**\ \_
-        -  ***consumer*\ secret**\ \_
-        
-        I recommend putting those two into a file. Only ***json*** and ***yaml*** files are
-        supported
-        
-        .. code:: json
-        
-            {
-                "consumer_key": "my_very_long_and_weird_consumer_key",
-                "consumer_secret": "my_not_that_long_consumer_secret"
-            }
-        
-        Once you acquired your access\_token, this file will look like :
-        
-        -  **OAuth1**
-        
-        .. code:: json
-        
-            {
-                "access_token": "A=5ZnN5xXY5yKacQp1QtUF68MlEmXVIF8fRplkc7W1QMVYeLJ2DdBmNyH7SxVgUbAjdv5edCnk_DEUbfr6GpqezsSAuE9h36wfh.J45twIo1sA.bqMk7Bta6IisI9z1_h8D0QZzWYmjybxlQcuNgd7TY4nJuu_Afj_8ED787BQbjg6OqRotV.eM4_YyBCjP1K8G6rG44iX2PGNj.JSEJrocgvglABkTTVA_8t.JoLH7NHSgxCQXhakBsk3_K.6Rkgm_Nkc7.ZD02pYy3dJAfBh1fFvtrCwIOqDIplri305dZ1UY430X6SfPnZIFJNiTWkMH8_QRhcnfizG5TZugN_.0ib2VnnUzspeFT0_86p6WMP3uFOLYXspdEOryhSJwFJ3AHZN9n.t8euRQOxanpsvw5M5ffBs6P0dI5FijGw3fibbqoheJOSUE_BRUNEL_KOUKAJSsJCH(^_^)JHllHmJUptK9k5ifiqJOpTbodnW8EsyyNhthDOusv5Bp6142mvCPnC7HX7PkTodHqfgVyAUOvOqSsqMGyc65OY8roLORKpUWObw9bjd8YsU40jwSaGZtWmvVhYV9RxUA779bRuE1k0BL_fvXQ_tlZnxPhtIFBB64szQ9AwA9HT_nZKq8q1rOfUcBIZJ7Zu1jwpZUAOkHsfmHWCW2gK8BC4wjk0WuJg95FpZ2z741mhRcdma2bVYpdh3k2DdaBVYRTDT36Q4SBtreb_GNi1Mctg.RhSqopCTTvW4jjXAkt2SHnscUi37v0yo4JVex0cnVmVTFL7TRl1JMLl9jt0XmaLaKuS4nhR4A--", 
-                "access_token_secret": "99a20a82e99THE_A_Tf803cb153f3d98", 
-                "consumer_key": "dj0yJmk9e_THIS_IS_THE_CK_RGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--", 
-                "consumer_secret": "08802b459abTHIS_IS_THE_CS4b75789f7", 
-                "session_handle": "APIENFXij.bjFW_MY_SESSION_EXn.4.DOIYOR37", 
-                "token_time": 1433546792.343515
-            }
-        
-        -  **OAuth2**
-        
-        .. code:: json
-        
-            {
-                "access_token": "DELvMgOYvwPQJS8eFW_2hRN5rJxz6dnHAOk2s.qB0iMIeRg5.ZpW3xZF0p8CABLjZ2gfNdE602dCN2wTHdGHHLtChF3ls9BUuZ1QDdqIVq.yWclfweleyZSq6dAzlPEHiskWmfItjHK5VERY_LONG_ACCESS_TOKEN_oyyD4cIKvdNJsJ9k779mAUqN02_5ugBeDfCLebqjL8uVuunObew0ERa2MxE6jywNY0TTCe9W0nqTd6n0lKoN4PSP1Dw_Ifwx6enGuhUUAhhpa7nNMyhNy_pe6PfDf7IJ5gbkdtw3mD1o2T218ZTV0owdrKDLSF9oZrNvZ75xDlqaaI5yeW_.L63zk11PjsWUd5K8LGhWSTgRbyhffCDBcqVwTYEqHwCyVqHX4z2kgHhGsc0ies6WMG33kSw5Cgun0fnPbdDuHBgQziXU.GMv4hIDoIDMSLGpzpcpkyx4GS1CC_RUQwKxLilR3MQy7X2gI3cJA4lhRPlXEOdhS5HIQiQTgMWO9nWt7.RR7XtXVg-",
-                "consumer_key": "dj0yJmk9eFJINERDYWMY_CONSUMER_KEYmRGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--",
-                "consumer_secret": "08802b459ab48eeaMY_CONSUMER_SECRET_0af6a4b75789f7",
-                "refresh_token": "APIENFXij.bjFW1tEcr2THE_REFRESH_TOKEN_Xn.4.DOIYOR37",
-                "token_time": 1433553339.706037,
-                "token_type": "bearer"
-            }
-        
-        With that you should be good to go.
-        
-        Normally, once your got all that, you can ***use the same credentials
-        FOREVER***, you just have to ***REFRESH THEM***.
-        
-        OAuth1
-        ~~~~~~
-        
-        .. code:: python
-        
-            from yahoo_oauth import OAuth1
-            oauth = OAuth1(None, None, from_file='oauth1.json')
-            ...
-        
-            if not oauth.token_is_valid():
-                oauth.refresh_access_token()
-        
-            # Example
-            response = oauth.session.post(url, data=body)
-        
-        OAuth2
-        ~~~~~~
-        
-        .. code:: python
-        
-            from yahoo_oauth import OAuth2
-            oauth = OAuth2(None, None, from_file='oauth2.json')
-            ...
-        
-            if not oauth.token_is_valid():
-                oauth.refresh_access_token()
-            # Example
-            response = oauth.session.get(url, params=payload)
-        
-        .. |Build Status| image:: https://travis-ci.org/josuebrunel/yahoo-oauth.svg?branch=master
-           :target: https://travis-ci.org/josuebrunel/yahoo-oauth
-        .. |Documentation Status| image:: https://readthedocs.org/projects/yahoo-oauth/badge/?version=latest
-           :target: https://readthedocs.org/projects/yahoo-oauth/?badge=latest
-        
-        
-        
+Download-URL: https://github.com/josuebrunel/yahoo-oauth/archive/2.0.tar.gz
 Keywords: yahoo,oauth,oauth1,oauth2
 Platform: Any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE
+
+yahoo\_oauth
+============
+
+|Build Status| |Documentation Status|
+
+Yahoo\_OAuth is a very easy to use OAuth python library for Yahoo! APIs.
+
+Installation
+------------
+
+.. code:: python
+
+    pip install yahoo_oauth
+
+Quickstart
+----------
+
+Wether you use **OAuth1** or **OAuth2**, only **2** parameters are
+required.
+
+-  ***consumer*\ key**\ \_
+-  ***consumer*\ secret**\ \_
+
+I recommend putting those two into a file. Only ***json*** and ***yaml*** files are
+supported
+
+.. code:: json
+
+    {
+        "consumer_key": "my_very_long_and_weird_consumer_key",
+        "consumer_secret": "my_not_that_long_consumer_secret"
+    }
+
+Once you acquired your access\_token, this file will look like :
+
+-  **OAuth1**
+
+.. code:: json
+
+    {
+        "access_token": "A=5ZnN5xXY5yKacQp1QtUF68MlEmXVIF8fRplkc7W1QMVYeLJ2DdBmNyH7SxVgUbAjdv5edCnk_DEUbfr6GpqezsSAuE9h36wfh.J45twIo1sA.bqMk7Bta6IisI9z1_h8D0QZzWYmjybxlQcuNgd7TY4nJuu_Afj_8ED787BQbjg6OqRotV.eM4_YyBCjP1K8G6rG44iX2PGNj.JSEJrocgvglABkTTVA_8t.JoLH7NHSgxCQXhakBsk3_K.6Rkgm_Nkc7.ZD02pYy3dJAfBh1fFvtrCwIOqDIplri305dZ1UY430X6SfPnZIFJNiTWkMH8_QRhcnfizG5TZugN_.0ib2VnnUzspeFT0_86p6WMP3uFOLYXspdEOryhSJwFJ3AHZN9n.t8euRQOxanpsvw5M5ffBs6P0dI5FijGw3fibbqoheJOSUE_BRUNEL_KOUKAJSsJCH(^_^)JHllHmJUptK9k5ifiqJOpTbodnW8EsyyNhthDOusv5Bp6142mvCPnC7HX7PkTodHqfgVyAUOvOqSsqMGyc65OY8roLORKpUWObw9bjd8YsU40jwSaGZtWmvVhYV9RxUA779bRuE1k0BL_fvXQ_tlZnxPhtIFBB64szQ9AwA9HT_nZKq8q1rOfUcBIZJ7Zu1jwpZUAOkHsfmHWCW2gK8BC4wjk0WuJg95FpZ2z741mhRcdma2bVYpdh3k2DdaBVYRTDT36Q4SBtreb_GNi1Mctg.RhSqopCTTvW4jjXAkt2SHnscUi37v0yo4JVex0cnVmVTFL7TRl1JMLl9jt0XmaLaKuS4nhR4A--", 
+        "access_token_secret": "99a20a82e99THE_A_Tf803cb153f3d98", 
+        "consumer_key": "dj0yJmk9e_THIS_IS_THE_CK_RGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--", 
+        "consumer_secret": "08802b459abTHIS_IS_THE_CS4b75789f7", 
+        "session_handle": "APIENFXij.bjFW_MY_SESSION_EXn.4.DOIYOR37", 
+        "token_time": 1433546792.343515
+    }
+
+-  **OAuth2**
+
+.. code:: json
+
+    {
+        "access_token": "DELvMgOYvwPQJS8eFW_2hRN5rJxz6dnHAOk2s.qB0iMIeRg5.ZpW3xZF0p8CABLjZ2gfNdE602dCN2wTHdGHHLtChF3ls9BUuZ1QDdqIVq.yWclfweleyZSq6dAzlPEHiskWmfItjHK5VERY_LONG_ACCESS_TOKEN_oyyD4cIKvdNJsJ9k779mAUqN02_5ugBeDfCLebqjL8uVuunObew0ERa2MxE6jywNY0TTCe9W0nqTd6n0lKoN4PSP1Dw_Ifwx6enGuhUUAhhpa7nNMyhNy_pe6PfDf7IJ5gbkdtw3mD1o2T218ZTV0owdrKDLSF9oZrNvZ75xDlqaaI5yeW_.L63zk11PjsWUd5K8LGhWSTgRbyhffCDBcqVwTYEqHwCyVqHX4z2kgHhGsc0ies6WMG33kSw5Cgun0fnPbdDuHBgQziXU.GMv4hIDoIDMSLGpzpcpkyx4GS1CC_RUQwKxLilR3MQy7X2gI3cJA4lhRPlXEOdhS5HIQiQTgMWO9nWt7.RR7XtXVg-",
+        "consumer_key": "dj0yJmk9eFJINERDYWMY_CONSUMER_KEYmRGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--",
+        "consumer_secret": "08802b459ab48eeaMY_CONSUMER_SECRET_0af6a4b75789f7",
+        "refresh_token": "APIENFXij.bjFW1tEcr2THE_REFRESH_TOKEN_Xn.4.DOIYOR37",
+        "token_time": 1433553339.706037,
+        "token_type": "bearer"
+    }
+
+With that you should be good to go.
+
+Normally, once your got all that, you can ***use the same credentials
+FOREVER***, you just have to ***REFRESH THEM***.
+
+OAuth1
+~~~~~~
+
+.. code:: python
+
+    from yahoo_oauth import OAuth1
+    oauth = OAuth1(None, None, from_file='oauth1.json')
+    ...
+
+    if not oauth.token_is_valid():
+        oauth.refresh_access_token()
+
+    # Example
+    response = oauth.session.post(url, data=body)
+
+OAuth2
+~~~~~~
+
+.. code:: python
+
+    from yahoo_oauth import OAuth2
+    oauth = OAuth2(None, None, from_file='oauth2.json')
+    ...
+
+    if not oauth.token_is_valid():
+        oauth.refresh_access_token()
+    # Example
+    response = oauth.session.get(url, params=payload)
+
+.. |Build Status| image:: https://travis-ci.org/josuebrunel/yahoo-oauth.svg?branch=master
+   :target: https://travis-ci.org/josuebrunel/yahoo-oauth
+.. |Documentation Status| image:: https://readthedocs.org/projects/yahoo-oauth/badge/?version=latest
+   :target: https://readthedocs.org/projects/yahoo-oauth/?badge=latest
+
+
+
+
```

### Comparing `yahoo_oauth-1.1/yahoo_oauth.egg-info/PKG-INFO` & `yahoo_oauth-2.0/yahoo_oauth.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,126 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yahoo-oauth
-Version: 1.1
+Version: 2.0
 Summary: Python Yahoo OAuth Library. Supports OAuth1 and OAuth2
 Home-page: https://github.com/josuebrunel/yahoo-oauth
 Author: Josue Kouka
 Author-email: josuebrunel@gmail.com
 License: MIT
-Download-URL: https://github.com/josuebrunel/yahoo-oauth/archive/1.1.tar.gz
-Description: yahoo\_oauth
-        ============
-        
-        |Build Status| |Documentation Status|
-        
-        Yahoo\_OAuth is a very easy to use OAuth python library for Yahoo! APIs.
-        
-        Installation
-        ------------
-        
-        .. code:: python
-        
-            pip install yahoo_oauth
-        
-        Quickstart
-        ----------
-        
-        Wether you use **OAuth1** or **OAuth2**, only **2** parameters are
-        required.
-        
-        -  ***consumer*\ key**\ \_
-        -  ***consumer*\ secret**\ \_
-        
-        I recommend putting those two into a file. Only ***json*** and ***yaml*** files are
-        supported
-        
-        .. code:: json
-        
-            {
-                "consumer_key": "my_very_long_and_weird_consumer_key",
-                "consumer_secret": "my_not_that_long_consumer_secret"
-            }
-        
-        Once you acquired your access\_token, this file will look like :
-        
-        -  **OAuth1**
-        
-        .. code:: json
-        
-            {
-                "access_token": "A=5ZnN5xXY5yKacQp1QtUF68MlEmXVIF8fRplkc7W1QMVYeLJ2DdBmNyH7SxVgUbAjdv5edCnk_DEUbfr6GpqezsSAuE9h36wfh.J45twIo1sA.bqMk7Bta6IisI9z1_h8D0QZzWYmjybxlQcuNgd7TY4nJuu_Afj_8ED787BQbjg6OqRotV.eM4_YyBCjP1K8G6rG44iX2PGNj.JSEJrocgvglABkTTVA_8t.JoLH7NHSgxCQXhakBsk3_K.6Rkgm_Nkc7.ZD02pYy3dJAfBh1fFvtrCwIOqDIplri305dZ1UY430X6SfPnZIFJNiTWkMH8_QRhcnfizG5TZugN_.0ib2VnnUzspeFT0_86p6WMP3uFOLYXspdEOryhSJwFJ3AHZN9n.t8euRQOxanpsvw5M5ffBs6P0dI5FijGw3fibbqoheJOSUE_BRUNEL_KOUKAJSsJCH(^_^)JHllHmJUptK9k5ifiqJOpTbodnW8EsyyNhthDOusv5Bp6142mvCPnC7HX7PkTodHqfgVyAUOvOqSsqMGyc65OY8roLORKpUWObw9bjd8YsU40jwSaGZtWmvVhYV9RxUA779bRuE1k0BL_fvXQ_tlZnxPhtIFBB64szQ9AwA9HT_nZKq8q1rOfUcBIZJ7Zu1jwpZUAOkHsfmHWCW2gK8BC4wjk0WuJg95FpZ2z741mhRcdma2bVYpdh3k2DdaBVYRTDT36Q4SBtreb_GNi1Mctg.RhSqopCTTvW4jjXAkt2SHnscUi37v0yo4JVex0cnVmVTFL7TRl1JMLl9jt0XmaLaKuS4nhR4A--", 
-                "access_token_secret": "99a20a82e99THE_A_Tf803cb153f3d98", 
-                "consumer_key": "dj0yJmk9e_THIS_IS_THE_CK_RGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--", 
-                "consumer_secret": "08802b459abTHIS_IS_THE_CS4b75789f7", 
-                "session_handle": "APIENFXij.bjFW_MY_SESSION_EXn.4.DOIYOR37", 
-                "token_time": 1433546792.343515
-            }
-        
-        -  **OAuth2**
-        
-        .. code:: json
-        
-            {
-                "access_token": "DELvMgOYvwPQJS8eFW_2hRN5rJxz6dnHAOk2s.qB0iMIeRg5.ZpW3xZF0p8CABLjZ2gfNdE602dCN2wTHdGHHLtChF3ls9BUuZ1QDdqIVq.yWclfweleyZSq6dAzlPEHiskWmfItjHK5VERY_LONG_ACCESS_TOKEN_oyyD4cIKvdNJsJ9k779mAUqN02_5ugBeDfCLebqjL8uVuunObew0ERa2MxE6jywNY0TTCe9W0nqTd6n0lKoN4PSP1Dw_Ifwx6enGuhUUAhhpa7nNMyhNy_pe6PfDf7IJ5gbkdtw3mD1o2T218ZTV0owdrKDLSF9oZrNvZ75xDlqaaI5yeW_.L63zk11PjsWUd5K8LGhWSTgRbyhffCDBcqVwTYEqHwCyVqHX4z2kgHhGsc0ies6WMG33kSw5Cgun0fnPbdDuHBgQziXU.GMv4hIDoIDMSLGpzpcpkyx4GS1CC_RUQwKxLilR3MQy7X2gI3cJA4lhRPlXEOdhS5HIQiQTgMWO9nWt7.RR7XtXVg-",
-                "consumer_key": "dj0yJmk9eFJINERDYWMY_CONSUMER_KEYmRGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--",
-                "consumer_secret": "08802b459ab48eeaMY_CONSUMER_SECRET_0af6a4b75789f7",
-                "refresh_token": "APIENFXij.bjFW1tEcr2THE_REFRESH_TOKEN_Xn.4.DOIYOR37",
-                "token_time": 1433553339.706037,
-                "token_type": "bearer"
-            }
-        
-        With that you should be good to go.
-        
-        Normally, once your got all that, you can ***use the same credentials
-        FOREVER***, you just have to ***REFRESH THEM***.
-        
-        OAuth1
-        ~~~~~~
-        
-        .. code:: python
-        
-            from yahoo_oauth import OAuth1
-            oauth = OAuth1(None, None, from_file='oauth1.json')
-            ...
-        
-            if not oauth.token_is_valid():
-                oauth.refresh_access_token()
-        
-            # Example
-            response = oauth.session.post(url, data=body)
-        
-        OAuth2
-        ~~~~~~
-        
-        .. code:: python
-        
-            from yahoo_oauth import OAuth2
-            oauth = OAuth2(None, None, from_file='oauth2.json')
-            ...
-        
-            if not oauth.token_is_valid():
-                oauth.refresh_access_token()
-            # Example
-            response = oauth.session.get(url, params=payload)
-        
-        .. |Build Status| image:: https://travis-ci.org/josuebrunel/yahoo-oauth.svg?branch=master
-           :target: https://travis-ci.org/josuebrunel/yahoo-oauth
-        .. |Documentation Status| image:: https://readthedocs.org/projects/yahoo-oauth/badge/?version=latest
-           :target: https://readthedocs.org/projects/yahoo-oauth/?badge=latest
-        
-        
-        
+Download-URL: https://github.com/josuebrunel/yahoo-oauth/archive/2.0.tar.gz
 Keywords: yahoo,oauth,oauth1,oauth2
 Platform: Any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE
+
+yahoo\_oauth
+============
+
+|Build Status| |Documentation Status|
+
+Yahoo\_OAuth is a very easy to use OAuth python library for Yahoo! APIs.
+
+Installation
+------------
+
+.. code:: python
+
+    pip install yahoo_oauth
+
+Quickstart
+----------
+
+Wether you use **OAuth1** or **OAuth2**, only **2** parameters are
+required.
+
+-  ***consumer*\ key**\ \_
+-  ***consumer*\ secret**\ \_
+
+I recommend putting those two into a file. Only ***json*** and ***yaml*** files are
+supported
+
+.. code:: json
+
+    {
+        "consumer_key": "my_very_long_and_weird_consumer_key",
+        "consumer_secret": "my_not_that_long_consumer_secret"
+    }
+
+Once you acquired your access\_token, this file will look like :
+
+-  **OAuth1**
+
+.. code:: json
+
+    {
+        "access_token": "A=5ZnN5xXY5yKacQp1QtUF68MlEmXVIF8fRplkc7W1QMVYeLJ2DdBmNyH7SxVgUbAjdv5edCnk_DEUbfr6GpqezsSAuE9h36wfh.J45twIo1sA.bqMk7Bta6IisI9z1_h8D0QZzWYmjybxlQcuNgd7TY4nJuu_Afj_8ED787BQbjg6OqRotV.eM4_YyBCjP1K8G6rG44iX2PGNj.JSEJrocgvglABkTTVA_8t.JoLH7NHSgxCQXhakBsk3_K.6Rkgm_Nkc7.ZD02pYy3dJAfBh1fFvtrCwIOqDIplri305dZ1UY430X6SfPnZIFJNiTWkMH8_QRhcnfizG5TZugN_.0ib2VnnUzspeFT0_86p6WMP3uFOLYXspdEOryhSJwFJ3AHZN9n.t8euRQOxanpsvw5M5ffBs6P0dI5FijGw3fibbqoheJOSUE_BRUNEL_KOUKAJSsJCH(^_^)JHllHmJUptK9k5ifiqJOpTbodnW8EsyyNhthDOusv5Bp6142mvCPnC7HX7PkTodHqfgVyAUOvOqSsqMGyc65OY8roLORKpUWObw9bjd8YsU40jwSaGZtWmvVhYV9RxUA779bRuE1k0BL_fvXQ_tlZnxPhtIFBB64szQ9AwA9HT_nZKq8q1rOfUcBIZJ7Zu1jwpZUAOkHsfmHWCW2gK8BC4wjk0WuJg95FpZ2z741mhRcdma2bVYpdh3k2DdaBVYRTDT36Q4SBtreb_GNi1Mctg.RhSqopCTTvW4jjXAkt2SHnscUi37v0yo4JVex0cnVmVTFL7TRl1JMLl9jt0XmaLaKuS4nhR4A--", 
+        "access_token_secret": "99a20a82e99THE_A_Tf803cb153f3d98", 
+        "consumer_key": "dj0yJmk9e_THIS_IS_THE_CK_RGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--", 
+        "consumer_secret": "08802b459abTHIS_IS_THE_CS4b75789f7", 
+        "session_handle": "APIENFXij.bjFW_MY_SESSION_EXn.4.DOIYOR37", 
+        "token_time": 1433546792.343515
+    }
+
+-  **OAuth2**
+
+.. code:: json
+
+    {
+        "access_token": "DELvMgOYvwPQJS8eFW_2hRN5rJxz6dnHAOk2s.qB0iMIeRg5.ZpW3xZF0p8CABLjZ2gfNdE602dCN2wTHdGHHLtChF3ls9BUuZ1QDdqIVq.yWclfweleyZSq6dAzlPEHiskWmfItjHK5VERY_LONG_ACCESS_TOKEN_oyyD4cIKvdNJsJ9k779mAUqN02_5ugBeDfCLebqjL8uVuunObew0ERa2MxE6jywNY0TTCe9W0nqTd6n0lKoN4PSP1Dw_Ifwx6enGuhUUAhhpa7nNMyhNy_pe6PfDf7IJ5gbkdtw3mD1o2T218ZTV0owdrKDLSF9oZrNvZ75xDlqaaI5yeW_.L63zk11PjsWUd5K8LGhWSTgRbyhffCDBcqVwTYEqHwCyVqHX4z2kgHhGsc0ies6WMG33kSw5Cgun0fnPbdDuHBgQziXU.GMv4hIDoIDMSLGpzpcpkyx4GS1CC_RUQwKxLilR3MQy7X2gI3cJA4lhRPlXEOdhS5HIQiQTgMWO9nWt7.RR7XtXVg-",
+        "consumer_key": "dj0yJmk9eFJINERDYWMY_CONSUMER_KEYmRGTnpZbWNHbzlNQS0tJnM9Y29uc3VtZXJzZWNyZXQmeD1iNQ--",
+        "consumer_secret": "08802b459ab48eeaMY_CONSUMER_SECRET_0af6a4b75789f7",
+        "refresh_token": "APIENFXij.bjFW1tEcr2THE_REFRESH_TOKEN_Xn.4.DOIYOR37",
+        "token_time": 1433553339.706037,
+        "token_type": "bearer"
+    }
+
+With that you should be good to go.
+
+Normally, once your got all that, you can ***use the same credentials
+FOREVER***, you just have to ***REFRESH THEM***.
+
+OAuth1
+~~~~~~
+
+.. code:: python
+
+    from yahoo_oauth import OAuth1
+    oauth = OAuth1(None, None, from_file='oauth1.json')
+    ...
+
+    if not oauth.token_is_valid():
+        oauth.refresh_access_token()
+
+    # Example
+    response = oauth.session.post(url, data=body)
+
+OAuth2
+~~~~~~
+
+.. code:: python
+
+    from yahoo_oauth import OAuth2
+    oauth = OAuth2(None, None, from_file='oauth2.json')
+    ...
+
+    if not oauth.token_is_valid():
+        oauth.refresh_access_token()
+    # Example
+    response = oauth.session.get(url, params=payload)
+
+.. |Build Status| image:: https://travis-ci.org/josuebrunel/yahoo-oauth.svg?branch=master
+   :target: https://travis-ci.org/josuebrunel/yahoo-oauth
+.. |Documentation Status| image:: https://readthedocs.org/projects/yahoo-oauth/badge/?version=latest
+   :target: https://readthedocs.org/projects/yahoo-oauth/?badge=latest
+
+
+
+
```

### Comparing `yahoo_oauth-1.1/setup.py` & `yahoo_oauth-2.0/setup.py`

 * *Files identical despite different names*


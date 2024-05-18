# Comparing `tmp/Radicale-3.1.9.tar.gz` & `tmp/radicale-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Radicale-3.1.9.tar", last modified: Mon Mar 18 05:00:27 2024, max compression
+gzip compressed data, was "radicale-3.2.0.tar", last modified: Sat May 18 19:40:55 2024, max compression
```

## Comparing `Radicale-3.1.9.tar` & `radicale-3.2.0.tar`

### file list

```diff
@@ -1,89 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.993492 Radicale-3.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-03-18 05:00:22.000000 Radicale-3.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-03-18 05:00:22.000000 Radicale-3.1.9/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (127)    48555 2024-03-18 05:00:22.000000 Radicale-3.1.9/DOCUMENTATION.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-18 05:00:22.000000 Radicale-3.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-03-18 05:00:26.993492 Radicale-3.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-18 05:00:22.000000 Radicale-3.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.993492 Radicale-3.1.9/Radicale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-03-18 05:00:26.000000 Radicale-3.1.9/Radicale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-18 05:00:26.000000 Radicale-3.1.9/Radicale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 05:00:26.000000 Radicale-3.1.9/Radicale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-18 05:00:26.000000 Radicale-3.1.9/Radicale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-18 05:00:26.000000 Radicale-3.1.9/Radicale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-18 05:00:26.000000 Radicale-3.1.9/Radicale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-18 05:00:22.000000 Radicale-3.1.9/config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.985492 Radicale-3.1.9/radicale/
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.989492 Radicale-3.1.9/radicale/app/
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/mkcalendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/mkcol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    17664 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/propfind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/proppatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/put.py
--rw-r--r--   0 runner    (1001) docker     (127)    13872 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/app/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.989492 Radicale-3.1.9/radicale/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/auth/htpasswd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/auth/http_x_remote_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/auth/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/auth/remote_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/httputils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.989492 Radicale-3.1.9/radicale/item/
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/item/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/pathutils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.989492 Radicale-3.1.9/radicale/rights/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/rights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/rights/authenticated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/rights/from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/rights/owner_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/rights/owner_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.989492 Radicale-3.1.9/radicale/storage/
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.993492 Radicale-3.1.9/radicale/storage/multifilesystem/
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/create_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/move.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/storage/multifilesystem_nolock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.993492 Radicale-3.1.9/radicale/web/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/web/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.993492 Radicale-3.1.9/radicale/web/internal_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 05:00:26.993492 Radicale-3.1.9/radicale/web/internal_data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/web/internal_data/css/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/web/internal_data/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)    40643 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/web/internal_data/fn.js
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/web/internal_data/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/web/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale/xmlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-18 05:00:22.000000 Radicale-3.1.9/radicale.wsgi
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-18 05:00:22.000000 Radicale-3.1.9/rights
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-18 05:00:26.997492 Radicale-3.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-18 05:00:22.000000 Radicale-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.830116 radicale-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-05-18 19:40:52.000000 radicale-3.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-05-18 19:40:52.000000 radicale-3.2.0/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    49606 2024-05-18 19:40:52.000000 radicale-3.2.0/DOCUMENTATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-18 19:40:52.000000 radicale-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-18 19:40:55.830116 radicale-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-18 19:40:52.000000 radicale-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.830116 radicale-3.2.0/Radicale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-18 19:40:55.000000 radicale-3.2.0/Radicale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-18 19:40:55.000000 radicale-3.2.0/Radicale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:40:55.000000 radicale-3.2.0/Radicale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-18 19:40:55.000000 radicale-3.2.0/Radicale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 19:40:55.000000 radicale-3.2.0/Radicale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 19:40:55.000000 radicale-3.2.0/Radicale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-18 19:40:52.000000 radicale-3.2.0/config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.822116 radicale-3.2.0/radicale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.822116 radicale-3.2.0/radicale/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/mkcalendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/mkcol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18605 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/propfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/proppatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/put.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/app/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.826116 radicale-3.2.0/radicale/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/auth/htpasswd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/auth/http_x_remote_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/auth/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/auth/remote_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.826116 radicale-3.2.0/radicale/hook/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/hook/none.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.826116 radicale-3.2.0/radicale/hook/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/hook/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/httputils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.826116 radicale-3.2.0/radicale/item/
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/item/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/pathutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.826116 radicale-3.2.0/radicale/rights/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/rights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/rights/authenticated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/rights/from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/rights/owner_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/rights/owner_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.826116 radicale-3.2.0/radicale/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.830116 radicale-3.2.0/radicale/storage/multifilesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/create_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/storage/multifilesystem_nolock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.830116 radicale-3.2.0/radicale/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/web/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.830116 radicale-3.2.0/radicale/web/internal_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:40:55.830116 radicale-3.2.0/radicale/web/internal_data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/web/internal_data/css/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/web/internal_data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51712 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/web/internal_data/fn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8669 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/web/internal_data/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/web/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale/xmlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-18 19:40:52.000000 radicale-3.2.0/radicale.wsgi
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-18 19:40:52.000000 radicale-3.2.0/rights
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-18 19:40:55.834117 radicale-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-18 19:40:52.000000 radicale-3.2.0/setup.py
```

### Comparing `Radicale-3.1.9/CHANGELOG.md` & `radicale-3.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## 3.2.0
+
+* Enhancement: add hook support for event changes+deletion hooks (initial support: "rabbitmq")
+* Dependency: pika >= 1.1.0
+* Enhancement: add support for webcal subscriptions
+* Enhancement: major update of WebUI (design+features)
+* Adjust: change default loglevel to "info"
+* Enhancement: support "expand-property" on REPORT request
+* Drop: support for Python 3.7 (EOSL, can't be tested anymore)
+* Fix: allow quoted-printable encoding for vObjects
+
 ## 3.1.9
 
 * Add: support for Python 3.11 + 3.12
 * Drop: support for Python 3.6
 * Fix: MOVE in case listen on non-standard ports or behind reverse proxy
 * Fix: stricter requirements of Python 3.11
 * Fix: HTML pages
```

### Comparing `Radicale-3.1.9/COPYING.md` & `radicale-3.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/DOCUMENTATION.md` & `radicale-3.2.0/DOCUMENTATION.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 #### Installation
 
 Radicale is really easy to install and works out-of-the-box.
 
 ```bash
 python3 -m pip install --upgrade https://github.com/Kozea/Radicale/archive/master.tar.gz
-python3 -m radicale --storage-filesystem-folder=~/.var/lib/radicale/collections
+python3 -m radicale --logging-level info --storage-filesystem-folder=~/.var/lib/radicale/collections
 ```
 
 When the server is launched, open <http://localhost:5232> in your browser!
 You can login with any username and password.
 
 Want more? Check the [tutorials](#tutorials) and the
 [documentation](#documentation-1).
@@ -782,14 +782,21 @@
 
 ##### realm
 
 Message displayed in the client when a password is needed.
 
 Default: `Radicale - Password Required`
 
+##### lc_username
+
+Сonvert username to lowercase, must be true for case-insensitive auth 
+providers like ldap, kerberos
+
+Default: `False`
+
 #### rights
 
 ##### type
 
 The backend that is used to check the access rights of collections.
 
 The recommended backend is `owner_only`. If access to calendars
@@ -902,15 +909,49 @@
 
 An example to relax the same-origin policy:
 
 ```ini
 Access-Control-Allow-Origin = *
 ```
 
-### Supported Clients
+#### hook
+##### type
+
+Hook binding for event changes and deletion notifications.
+
+Available types:
+
+`none`
+: Disabled. Nothing will be notified.
+
+`rabbitmq`
+: Push the message to the rabbitmq server.
+
+Default: `none`
+
+#### rabbitmq_endpoint
+
+End-point address for rabbitmq server.
+Ex: amqp://user:password@localhost:5672/
+
+Default:
+
+#### rabbitmq_topic
+
+RabbitMQ topic to publish message.
+
+Default:
+
+#### rabbitmq_queue_type
+
+RabbitMQ queue type for the topic.
+
+Default: classic
+
+## Supported Clients
 
 Radicale has been tested with:
 
 * [Android](https://android.com/) with
   [DAVx⁵](https://www.davx5.com/) (formerly DAVdroid)
 * [GNOME Calendar](https://wiki.gnome.org/Apps/Calendar),
   [Contacts](https://wiki.gnome.org/Apps/Contacts) and
@@ -933,24 +974,29 @@
 
 #### DAVx⁵
 
 Enter the URL of the Radicale server (e.g. `http://localhost:5232`) and your
 username. DAVx⁵ will show all existing calendars and address books and you
 can create new.
 
-#### GNOME Calendar, Contacts and Evolution
+#### GNOME Calendar, Contacts
 
-**GNOME Calendar** and **Contacts** do not support adding WebDAV calendars
-and address books directly, but you can add them in **Evolution**.
+GNOME 46 added CalDAV and CardDAV support to _GNOME Online Accounts_.
+
+Open GNOME Settings, navigate to _Online Accounts_ > _Connect an Account_ > _Calendar, Contacts and Files_. Enter the URL (e.g. `https://example.com/radicale`) and your credentials then click _Sign In_. In the pop-up dialog, turn off _Files_. After adding Radicale in _GNOME Online Accounts_, it should be available in GNOME Contacts and GNOME Calendar.
+
+#### Evolution
 
 In **Evolution** add a new calendar and address book respectively with WebDAV.
 Enter the URL of the Radicale server (e.g. `http://localhost:5232`) and your
 username. Clicking on the search button will list the existing calendars and
 address books.
 
+Adding CalDAV and CardDAV accounts in Evolution will automatically make them available in GNOME Contacts and GNOME Calendar.
+
 #### Thunderbird
 
 Add a new calendar on the network. Enter your username and the URL of the
 Radicale server (e.g. `http://localhost:5232`). After asking for your password,
 it will list the existing calendars.
 
 ##### Adress books with CardBook add-on
```

### Comparing `Radicale-3.1.9/PKG-INFO` & `radicale-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Radicale
-Version: 3.1.9
+Version: 3.2.0
 Summary: CalDAV and CardDAV Server
 Home-page: https://radicale.org/
 Author: Guillaume Ayoub
 Author-email: guillaume.ayoub@kozea.fr
 License: GNU GPL v3
 Keywords: calendar,addressbook,CalDAV,CardDAV
 Platform: Any
@@ -12,30 +12,30 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business :: Groupware
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: COPYING.md
 Requires-Dist: defusedxml
 Requires-Dist: passlib
 Requires-Dist: vobject>=0.9.6
 Requires-Dist: python-dateutil>=2.7.3
+Requires-Dist: pika>=1.1.0
 Requires-Dist: setuptools; python_version < "3.9"
 Provides-Extra: test
 Requires-Dist: pytest<7; extra == "test"
 Requires-Dist: typeguard<3; extra == "test"
 Requires-Dist: waitress; extra == "test"
 Requires-Dist: bcrypt; extra == "test"
 Provides-Extra: bcrypt
```

### Comparing `Radicale-3.1.9/README.md` & `radicale-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/Radicale.egg-info/PKG-INFO` & `radicale-3.2.0/Radicale.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Radicale
-Version: 3.1.9
+Version: 3.2.0
 Summary: CalDAV and CardDAV Server
 Home-page: https://radicale.org/
 Author: Guillaume Ayoub
 Author-email: guillaume.ayoub@kozea.fr
 License: GNU GPL v3
 Keywords: calendar,addressbook,CalDAV,CardDAV
 Platform: Any
@@ -12,30 +12,30 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business :: Groupware
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: COPYING.md
 Requires-Dist: defusedxml
 Requires-Dist: passlib
 Requires-Dist: vobject>=0.9.6
 Requires-Dist: python-dateutil>=2.7.3
+Requires-Dist: pika>=1.1.0
 Requires-Dist: setuptools; python_version < "3.9"
 Provides-Extra: test
 Requires-Dist: pytest<7; extra == "test"
 Requires-Dist: typeguard<3; extra == "test"
 Requires-Dist: waitress; extra == "test"
 Requires-Dist: bcrypt; extra == "test"
 Provides-Extra: bcrypt
```

### Comparing `Radicale-3.1.9/Radicale.egg-info/SOURCES.txt` & `radicale-3.2.0/Radicale.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 radicale/app/put.py
 radicale/app/report.py
 radicale/auth/__init__.py
 radicale/auth/htpasswd.py
 radicale/auth/http_x_remote_user.py
 radicale/auth/none.py
 radicale/auth/remote_user.py
+radicale/hook/__init__.py
+radicale/hook/none.py
+radicale/hook/rabbitmq/__init__.py
 radicale/item/__init__.py
 radicale/item/filter.py
 radicale/rights/__init__.py
 radicale/rights/authenticated.py
 radicale/rights/from_file.py
 radicale/rights/owner_only.py
 radicale/rights/owner_write.py
```

### Comparing `Radicale-3.1.9/config` & `radicale-3.2.0/config`

 * *Files 18% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 
 # Incorrect authentication delay (seconds)
 #delay = 1
 
 # Message displayed in the client when a password is needed
 #realm = Radicale - Password Required
 
+# Сonvert username to lowercase, must be true for case-insensitive auth providers
+#lc_username = False
+
 
 [rights]
 
 # Rights backend
 # Value: none | authenticated | owner_only | owner_write | from_file
 #type = owner_only
 
@@ -108,17 +111,26 @@
 #type = internal
 
 
 [logging]
 
 # Threshold for the logger
 # Value: debug | info | warning | error | critical
-#level = warning
+#level = info
 
 # Don't include passwords in logs
 #mask_passwords = True
 
 
 [headers]
 
 # Additional HTTP headers
 #Access-Control-Allow-Origin = *
+
+[hook]
+
+# Hook types
+# Value: none | rabbitmq
+#type = none
+#rabbitmq_endpoint =
+#rabbitmq_topic =
+#rabbitmq_queue_type = classic
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Radicale-3.1.9/radicale/__init__.py` & `radicale-3.2.0/radicale/__init__.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/__main__.py` & `radicale-3.2.0/radicale/__main__.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/__init__.py` & `radicale-3.2.0/radicale/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/base.py` & `radicale-3.2.0/radicale/app/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import io
 import logging
 import posixpath
 import sys
 import xml.etree.ElementTree as ET
 from typing import Optional
 
-from radicale import (auth, config, httputils, pathutils, rights, storage,
-                      types, web, xmlutils)
+from radicale import (auth, config, hook, httputils, pathutils, rights,
+                      storage, types, web, xmlutils)
 from radicale.log import logger
 
 # HACK: https://github.com/tiran/defusedxml/issues/54
 import defusedxml.ElementTree as DefusedET  # isort:skip
 sys.modules["xml.etree"].ElementTree = ET  # type:ignore[attr-defined]
 
 
@@ -35,22 +35,24 @@
     configuration: config.Configuration
     _auth: auth.BaseAuth
     _storage: storage.BaseStorage
     _rights: rights.BaseRights
     _web: web.BaseWeb
     _encoding: str
     _permit_delete_collection: bool
+    _hook: hook.BaseHook
 
     def __init__(self, configuration: config.Configuration) -> None:
         self.configuration = configuration
         self._auth = auth.load(configuration)
         self._storage = storage.load(configuration)
         self._rights = rights.load(configuration)
         self._web = web.load(configuration)
         self._encoding = configuration.get("encoding", "request")
+        self._hook = hook.load(configuration)
 
     def _read_xml_request_body(self, environ: types.WSGIEnviron
                                ) -> Optional[ET.Element]:
         content = httputils.decode_request(
             self.configuration, environ,
             httputils.read_raw_request_body(self.configuration, environ))
         if not content:
```

### Comparing `Radicale-3.1.9/radicale/app/delete.py` & `radicale-3.2.0/radicale/app/delete.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import xml.etree.ElementTree as ET
 from http import client
 from typing import Optional
 
 from radicale import httputils, storage, types, xmlutils
 from radicale.app.base import Access, ApplicationBase
+from radicale.hook import HookNotificationItem, HookNotificationItemTypes
 
 
 def xml_delete(base_prefix: str, path: str, collection: storage.BaseCollection,
                item_href: Optional[str] = None) -> ET.Element:
     """Read and answer DELETE requests.
 
     Read rfc4918-9.6 for info.
@@ -63,19 +64,37 @@
                 return httputils.NOT_FOUND
             if not access.check("w", item):
                 return httputils.NOT_ALLOWED
             if_match = environ.get("HTTP_IF_MATCH", "*")
             if if_match not in ("*", item.etag):
                 # ETag precondition not verified, do not delete item
                 return httputils.PRECONDITION_FAILED
+            hook_notification_item_list = []
             if isinstance(item, storage.BaseCollection):
                 if self._permit_delete_collection:
+                    for i in item.get_all():
+                        hook_notification_item_list.append(
+                            HookNotificationItem(
+                                HookNotificationItemTypes.DELETE,
+                                access.path,
+                                i.uid
+                            )
+                        )
                     xml_answer = xml_delete(base_prefix, path, item)
                 else:
                     return httputils.NOT_ALLOWED
             else:
                 assert item.collection is not None
                 assert item.href is not None
+                hook_notification_item_list.append(
+                    HookNotificationItem(
+                        HookNotificationItemTypes.DELETE,
+                        access.path,
+                        item.uid
+                    )
+                )
                 xml_answer = xml_delete(
                     base_prefix, path, item.collection, item.href)
+            for notification_item in hook_notification_item_list:
+                self._hook.notify(notification_item)
             headers = {"Content-Type": "text/xml; charset=%s" % self._encoding}
             return client.OK, headers, self._xml_response(xml_answer)
```

### Comparing `Radicale-3.1.9/radicale/app/get.py` & `radicale-3.2.0/radicale/app/get.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/head.py` & `radicale-3.2.0/radicale/app/head.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/mkcalendar.py` & `radicale-3.2.0/radicale/app/mkcalendar.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/mkcol.py` & `radicale-3.2.0/radicale/app/mkcol.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/move.py` & `radicale-3.2.0/radicale/app/move.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/options.py` & `radicale-3.2.0/radicale/app/options.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/post.py` & `radicale-3.2.0/radicale/app/post.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/app/propfind.py` & `radicale-3.2.0/radicale/app/propfind.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         propname: bool = False, allprop: bool = False) -> ET.Element:
     """Build and return a PROPFIND response."""
     if propname and allprop or (props and (propname or allprop)):
         raise ValueError("Only use one of props, propname and allprops")
 
     if isinstance(item, storage.BaseCollection):
         is_collection = True
-        is_leaf = item.tag in ("VADDRESSBOOK", "VCALENDAR")
+        is_leaf = item.tag in ("VADDRESSBOOK", "VCALENDAR", "VSUBSCRIBED")
         collection = item
         # Some clients expect collections to end with `/`
         uri = pathutils.unstrip_path(item.path, True)
     else:
         is_collection = is_leaf = False
         assert item.collection is not None
         assert item.href
@@ -255,23 +255,33 @@
                         child_element = ET.Element(
                             xmlutils.make_clark("CR:addressbook"))
                         element.append(child_element)
                     elif collection.tag == "VCALENDAR":
                         child_element = ET.Element(
                             xmlutils.make_clark("C:calendar"))
                         element.append(child_element)
+                    elif collection.tag == "VSUBSCRIBED":
+                        child_element = ET.Element(
+                            xmlutils.make_clark("CS:subscribed"))
+                        element.append(child_element)
                 child_element = ET.Element(xmlutils.make_clark("D:collection"))
                 element.append(child_element)
             elif tag == xmlutils.make_clark("RADICALE:displayname"):
                 # Only for internal use by the web interface
                 displayname = collection.get_meta("D:displayname")
                 if displayname is not None:
                     element.text = displayname
                 else:
                     is404 = True
+            elif tag == xmlutils.make_clark("RADICALE:getcontentcount"):
+                # Only for internal use by the web interface
+                if isinstance(item, storage.BaseCollection) and not collection.is_principal:
+                    element.text = str(sum(1 for x in item.get_all()))
+                else:
+                    is404 = True
             elif tag == xmlutils.make_clark("D:displayname"):
                 displayname = collection.get_meta("D:displayname")
                 if not displayname and is_leaf:
                     displayname = collection.path
                 if displayname is not None:
                     element.text = displayname
                 else:
@@ -282,14 +292,21 @@
                 else:
                     is404 = True
             elif tag == xmlutils.make_clark("D:sync-token"):
                 if is_leaf:
                     element.text, _ = collection.sync()
                 else:
                     is404 = True
+            elif tag == xmlutils.make_clark("CS:source"):
+                if is_leaf:
+                    child_element = ET.Element(xmlutils.make_clark("D:href"))
+                    child_element.text = collection.get_meta('CS:source')
+                    element.append(child_element)
+                else:
+                    is404 = True
             else:
                 human_tag = xmlutils.make_human_tag(tag)
                 tag_text = collection.get_meta(human_tag)
                 if tag_text is not None:
                     element.text = tag_text
                 else:
                     is404 = True
```

### Comparing `Radicale-3.1.9/radicale/app/proppatch.py` & `radicale-3.2.0/radicale/app/proppatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 # along with Radicale.  If not, see <http://www.gnu.org/licenses/>.
 
 import socket
 import xml.etree.ElementTree as ET
 from http import client
 from typing import Dict, Optional, cast
 
+import defusedxml.ElementTree as DefusedET
+
 import radicale.item as radicale_item
 from radicale import httputils, storage, types, xmlutils
 from radicale.app.base import Access, ApplicationBase
+from radicale.hook import HookNotificationItem, HookNotificationItemTypes
 from radicale.log import logger
 
 
 def xml_proppatch(base_prefix: str, path: str,
                   xml_request: Optional[ET.Element],
                   collection: storage.BaseCollection) -> ET.Element:
     """Read and answer PROPPATCH requests.
@@ -89,12 +92,22 @@
             if not isinstance(item, storage.BaseCollection):
                 return httputils.FORBIDDEN
             headers = {"DAV": httputils.DAV_HEADERS,
                        "Content-Type": "text/xml; charset=%s" % self._encoding}
             try:
                 xml_answer = xml_proppatch(base_prefix, path, xml_content,
                                            item)
+                if xml_content is not None:
+                    hook_notification_item = HookNotificationItem(
+                        HookNotificationItemTypes.CPATCH,
+                        access.path,
+                        DefusedET.tostring(
+                            xml_content,
+                            encoding=self._encoding
+                        ).decode(encoding=self._encoding)
+                    )
+                    self._hook.notify(hook_notification_item)
             except ValueError as e:
                 logger.warning(
                     "Bad PROPPATCH request on %r: %s", path, e, exc_info=True)
                 return httputils.BAD_REQUEST
             return client.MULTI_STATUS, headers, self._xml_response(xml_answer)
```

### Comparing `Radicale-3.1.9/radicale/app/put.py` & `radicale-3.2.0/radicale/app/put.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from typing import Iterator, List, Mapping, MutableMapping, Optional, Tuple
 
 import vobject
 
 import radicale.item as radicale_item
 from radicale import httputils, pathutils, rights, storage, types, xmlutils
 from radicale.app.base import Access, ApplicationBase
+from radicale.hook import HookNotificationItem, HookNotificationItemTypes
 from radicale.log import logger
 
 MIMETYPE_TAGS: Mapping[str, str] = {value: key for key, value in
                                     xmlutils.MIMETYPES.items()}
 
 
 def prepare(vobject_items: List[vobject.base.Component], path: str,
@@ -202,14 +203,21 @@
                     exc_info=prepared_exc_info)
                 return httputils.BAD_REQUEST
 
             if write_whole_collection:
                 try:
                     etag = self._storage.create_collection(
                         path, prepared_items, props).etag
+                    for item in prepared_items:
+                        hook_notification_item = HookNotificationItem(
+                            HookNotificationItemTypes.UPSERT,
+                            access.path,
+                            item.serialize()
+                        )
+                        self._hook.notify(hook_notification_item)
                 except ValueError as e:
                     logger.warning(
                         "Bad PUT request on %r: %s", path, e, exc_info=True)
                     return httputils.BAD_REQUEST
             else:
                 assert not isinstance(item, storage.BaseCollection)
                 prepared_item, = prepared_items
@@ -218,14 +226,20 @@
                     return self._webdav_error_response(
                         client.CONFLICT, "%s:no-uid-conflict" % (
                             "C" if tag == "VCALENDAR" else "CR"))
 
                 href = posixpath.basename(pathutils.strip_path(path))
                 try:
                     etag = parent_item.upload(href, prepared_item).etag
+                    hook_notification_item = HookNotificationItem(
+                        HookNotificationItemTypes.UPSERT,
+                        access.path,
+                        prepared_item.serialize()
+                    )
+                    self._hook.notify(hook_notification_item)
                 except ValueError as e:
                     logger.warning(
                         "Bad PUT request on %r: %s", path, e, exc_info=True)
                     return httputils.BAD_REQUEST
 
             headers = {"ETag": etag}
             return client.CREATED, headers, None
```

### Comparing `Radicale-3.1.9/radicale/app/report.py` & `radicale-3.2.0/radicale/app/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,21 +14,27 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Radicale.  If not, see <http://www.gnu.org/licenses/>.
 
 import contextlib
+import copy
+import datetime
 import posixpath
 import socket
 import xml.etree.ElementTree as ET
 from http import client
-from typing import Callable, Iterable, Iterator, Optional, Sequence, Tuple
+from typing import (Callable, Iterable, Iterator, List, Optional, Sequence,
+                    Tuple, Union)
 from urllib.parse import unquote, urlparse
 
+import vobject.base
+from vobject.base import ContentLine
+
 import radicale.item as radicale_item
 from radicale import httputils, pathutils, storage, types, xmlutils
 from radicale.app.base import Access, ApplicationBase
 from radicale.item import filter as radicale_filter
 from radicale.log import logger
 
 
@@ -60,17 +66,16 @@
             root.tag == xmlutils.make_clark("CR:addressbook-multiget") and
             collection.tag != "VADDRESSBOOK" or
             root.tag == xmlutils.make_clark("D:sync-collection") and
             collection.tag not in ("VADDRESSBOOK", "VCALENDAR")):
         logger.warning("Invalid REPORT method %r on %r requested",
                        xmlutils.make_human_tag(root.tag), path)
         return client.FORBIDDEN, xmlutils.webdav_error("D:supported-report")
-    prop_element = root.find(xmlutils.make_clark("D:prop"))
-    props = ([prop.tag for prop in prop_element]
-             if prop_element is not None else [])
+
+    props: Union[ET.Element, List] = root.find(xmlutils.make_clark("D:prop")) or []
 
     hreferences: Iterable[str]
     if root.tag in (
             xmlutils.make_clark("C:calendar-multiget"),
             xmlutils.make_clark("CR:addressbook-multiget")):
         # Read rfc4791-7.9 for info
         hreferences = set()
@@ -134,40 +139,145 @@
             except Exception as e:
                 raise RuntimeError("Failed to filter item %r from %r: %s" %
                                    (item.href, collection.path, e)) from e
 
         found_props = []
         not_found_props = []
 
-        for tag in props:
-            element = ET.Element(tag)
-            if tag == xmlutils.make_clark("D:getetag"):
+        for prop in props:
+            element = ET.Element(prop.tag)
+            if prop.tag == xmlutils.make_clark("D:getetag"):
                 element.text = item.etag
                 found_props.append(element)
-            elif tag == xmlutils.make_clark("D:getcontenttype"):
+            elif prop.tag == xmlutils.make_clark("D:getcontenttype"):
                 element.text = xmlutils.get_content_type(item, encoding)
                 found_props.append(element)
-            elif tag in (
+            elif prop.tag in (
                     xmlutils.make_clark("C:calendar-data"),
                     xmlutils.make_clark("CR:address-data")):
                 element.text = item.serialize()
-                found_props.append(element)
+
+                expand = prop.find(xmlutils.make_clark("C:expand"))
+                if expand is not None:
+                    start = expand.get('start')
+                    end = expand.get('end')
+
+                    if (start is None) or (end is None):
+                        return client.FORBIDDEN, \
+                            xmlutils.webdav_error("C:expand")
+
+                    start = datetime.datetime.strptime(
+                        start, '%Y%m%dT%H%M%SZ'
+                    ).replace(tzinfo=datetime.timezone.utc)
+                    end = datetime.datetime.strptime(
+                        end, '%Y%m%dT%H%M%SZ'
+                    ).replace(tzinfo=datetime.timezone.utc)
+
+                    expanded_element = _expand(
+                        element, copy.copy(item), start, end)
+                    found_props.append(expanded_element)
+                else:
+                    found_props.append(element)
             else:
                 not_found_props.append(element)
 
         assert item.href
         uri = pathutils.unstrip_path(
             posixpath.join(collection.path, item.href))
         multistatus.append(xml_item_response(
             base_prefix, uri, found_props=found_props,
             not_found_props=not_found_props, found_item=True))
 
     return client.MULTI_STATUS, multistatus
 
 
+def _expand(
+        element: ET.Element,
+        item: radicale_item.Item,
+        start: datetime.datetime,
+        end: datetime.datetime,
+) -> ET.Element:
+    rruleset = None
+    if hasattr(item.vobject_item.vevent, 'rrule'):
+        rruleset = item.vobject_item.vevent.getrruleset()
+
+    expanded_item = _make_vobject_expanded_item(item)
+
+    if rruleset:
+        recurrences = rruleset.between(start, end)
+
+        expanded: vobject.base.Component = copy.copy(expanded_item.vobject_item)
+        is_expanded_filled: bool = False
+
+        for recurrence_dt in recurrences:
+            recurrence_utc = recurrence_dt.astimezone(datetime.timezone.utc)
+
+            vevent = copy.deepcopy(expanded.vevent)
+            vevent.recurrence_id = ContentLine(
+                name='RECURRENCE-ID',
+                value=recurrence_utc.strftime('%Y%m%dT%H%M%SZ'), params={}
+            )
+
+            if is_expanded_filled is False:
+                expanded.vevent = vevent
+                is_expanded_filled = True
+            else:
+                expanded.add(vevent)
+
+        element.text = expanded.serialize()
+    else:
+        element.text = expanded_item.vobject_item.serialize()
+
+    return element
+
+
+def _make_vobject_expanded_item(
+        item: radicale_item.Item
+) -> radicale_item.Item:
+    # https://www.rfc-editor.org/rfc/rfc4791#section-9.6.5
+    # The returned calendar components MUST NOT use recurrence
+    #       properties (i.e., EXDATE, EXRULE, RDATE, and RRULE) and MUST NOT
+    #       have reference to or include VTIMEZONE components.  Date and local
+    #       time with reference to time zone information MUST be converted
+    #       into date with UTC time.
+
+    item = copy.copy(item)
+    vevent = item.vobject_item.vevent
+
+    start_utc = vevent.dtstart.value.astimezone(datetime.timezone.utc)
+    vevent.dtstart = ContentLine(
+        name='DTSTART',
+        value=start_utc.strftime('%Y%m%dT%H%M%SZ'), params={})
+
+    dt_end = getattr(vevent, 'dtend', None)
+    if dt_end is not None:
+        end_utc = dt_end.value.astimezone(datetime.timezone.utc)
+        vevent.dtend = ContentLine(
+            name='DTEND',
+            value=end_utc.strftime('%Y%m%dT%H%M%SZ'), params={})
+
+    timezones_to_remove = []
+    for component in item.vobject_item.components():
+        if component.name == 'VTIMEZONE':
+            timezones_to_remove.append(component)
+
+    for timezone in timezones_to_remove:
+        item.vobject_item.remove(timezone)
+
+    try:
+        delattr(item.vobject_item.vevent, 'rrule')
+        delattr(item.vobject_item.vevent, 'exdate')
+        delattr(item.vobject_item.vevent, 'exrule')
+        delattr(item.vobject_item.vevent, 'rdate')
+    except AttributeError:
+        pass
+
+    return item
+
+
 def xml_item_response(base_prefix: str, href: str,
                       found_props: Sequence[ET.Element] = (),
                       not_found_props: Sequence[ET.Element] = (),
                       found_item: bool = True) -> ET.Element:
     response = ET.Element(xmlutils.make_clark("D:response"))
 
     href_element = ET.Element(xmlutils.make_clark("D:href"))
```

### Comparing `Radicale-3.1.9/radicale/auth/__init__.py` & `radicale-3.2.0/radicale/auth/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,42 +40,48 @@
     """Load the authentication module chosen in configuration."""
     return utils.load_plugin(INTERNAL_TYPES, "auth", "Auth", BaseAuth,
                              configuration)
 
 
 class BaseAuth:
 
+    _lc_username: bool
+
     def __init__(self, configuration: "config.Configuration") -> None:
         """Initialize BaseAuth.
 
         ``configuration`` see ``radicale.config`` module.
         The ``configuration`` must not change during the lifetime of
         this object, it is kept as an internal reference.
 
         """
         self.configuration = configuration
+        self._lc_username = configuration.get("auth", "lc_username")
 
     def get_external_login(self, environ: types.WSGIEnviron) -> Union[
             Tuple[()], Tuple[str, str]]:
         """Optionally provide the login and password externally.
 
         ``environ`` a dict with the WSGI environment
 
         If ``()`` is returned, Radicale handles HTTP authentication.
         Otherwise, returns a tuple ``(login, password)``. For anonymous users
         ``login`` must be ``""``.
 
         """
         return ()
 
-    def login(self, login: str, password: str) -> str:
+    def _login(self, login: str, password: str) -> str:
         """Check credentials and map login to internal user
 
         ``login`` the login name
 
         ``password`` the password
 
         Returns the username or ``""`` for invalid credentials.
 
         """
 
         raise NotImplementedError
+
+    def login(self, login: str, password: str) -> str:
+        return self._login(login, password).lower() if self._lc_username else self._login(login, password)
```

### Comparing `Radicale-3.1.9/radicale/auth/htpasswd.py` & `radicale-3.2.0/radicale/auth/htpasswd.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         elif encryption == "sha512":
             self._verify = self._sha512
         elif encryption == "bcrypt" or encryption == "autodetect":
             try:
                 import bcrypt
             except ImportError as e:
                 raise RuntimeError(
-                    "The htpasswd encryption method 'bcrypt' or 'auto' requires "
+                    "The htpasswd encryption method 'bcrypt' or 'autodetect' requires "
                     "the bcrypt module.") from e
             if encryption == "bcrypt":
                 self._verify = functools.partial(self._bcrypt, bcrypt)
             else:
                 self._verify = self._autodetect
                 self._verify_bcrypt = functools.partial(self._bcrypt, bcrypt)
         else:
@@ -123,15 +123,15 @@
         elif hash_value.startswith("$6$", 0, 3) and len(hash_value) == 106:
             # SHA-512
             return self._sha512(hash_value, password)
         else:
             # assumed plaintext
             return self._plain(hash_value, password)
 
-    def login(self, login: str, password: str) -> str:
+    def _login(self, login: str, password: str) -> str:
         """Validate credentials.
 
         Iterate through htpasswd credential file until login matches, extract
         hash (encrypted password) and check hash against password,
         using the method specified in the Radicale config.
 
         The content of the file is not cached because reading is generally a
```

### Comparing `Radicale-3.1.9/radicale/auth/http_x_remote_user.py` & `radicale-3.2.0/radicale/auth/http_x_remote_user.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/auth/none.py` & `radicale-3.2.0/radicale/auth/none.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 """
 
 from radicale import auth
 
 
 class Auth(auth.BaseAuth):
 
-    def login(self, login: str, password: str) -> str:
+    def _login(self, login: str, password: str) -> str:
         return login
```

### Comparing `Radicale-3.1.9/radicale/auth/remote_user.py` & `radicale-3.2.0/radicale/auth/remote_user.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/config.py` & `radicale-3.2.0/radicale/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import string
 import sys
 from collections import OrderedDict
 from configparser import RawConfigParser
 from typing import (Any, Callable, ClassVar, Iterable, List, Optional,
                     Sequence, Tuple, TypeVar, Union)
 
-from radicale import auth, rights, storage, types, web
+from radicale import auth, hook, rights, storage, types, web
 
 DEFAULT_CONFIG_PATH: str = os.pathsep.join([
     "?/etc/radicale/config",
     "?~/.config/radicale/config"])
 
 
 def positive_int(value: Any) -> int:
@@ -173,15 +173,19 @@
         ("realm", {
             "value": "Radicale - Password Required",
             "help": "message displayed when a password is needed",
             "type": str}),
         ("delay", {
             "value": "1",
             "help": "incorrect authentication delay",
-            "type": positive_float})])),
+            "type": positive_float}),
+        ("lc_username", {
+            "value": "False",
+            "help": "convert username to lowercase, must be true for case-insensitive auth providers",
+            "type": bool})])),
     ("rights", OrderedDict([
         ("type", {
             "value": "owner_only",
             "help": "rights backend",
             "type": str_or_callable,
             "internal": rights.INTERNAL_TYPES}),
         ("permit_delete_collection", {
@@ -210,23 +214,41 @@
             "value": "",
             "help": "command that is run after changes to storage",
             "type": str}),
         ("_filesystem_fsync", {
             "value": "True",
             "help": "sync all changes to filesystem during requests",
             "type": bool})])),
+    ("hook", OrderedDict([
+        ("type", {
+            "value": "none",
+            "help": "hook backend",
+            "type": str,
+            "internal": hook.INTERNAL_TYPES}),
+        ("rabbitmq_endpoint", {
+            "value": "",
+            "help": "endpoint where rabbitmq server is running",
+            "type": str}),
+        ("rabbitmq_topic", {
+            "value": "",
+            "help": "topic to declare queue",
+            "type": str}),
+        ("rabbitmq_queue_type", {
+            "value": "",
+            "help": "queue type for topic declaration",
+            "type": str})])),
     ("web", OrderedDict([
         ("type", {
             "value": "internal",
             "help": "web interface backend",
             "type": str_or_callable,
             "internal": web.INTERNAL_TYPES})])),
     ("logging", OrderedDict([
         ("level", {
-            "value": "warning",
+            "value": "info",
             "help": "threshold for the logger",
             "type": logging_level}),
         ("mask_passwords", {
             "value": "True",
             "help": "mask passwords in logs",
             "type": bool})])),
     ("headers", OrderedDict([
```

### Comparing `Radicale-3.1.9/radicale/httputils.py` & `radicale-3.2.0/radicale/httputils.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/item/__init__.py` & `radicale-3.2.0/radicale/item/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 def read_components(s: str) -> List[vobject.base.Component]:
     """Wrapper for vobject.readComponents"""
     # Workaround for bug in InfCloud
     # PHOTO is a data URI
     s = re.sub(r"^(PHOTO(?:;[^:\r\n]*)?;ENCODING=b(?:;[^:\r\n]*)?:)"
                r"data:[^;,\r\n]*;base64,", r"\1", s,
                flags=re.MULTILINE | re.IGNORECASE)
-    return list(vobject.readComponents(s))
+    return list(vobject.readComponents(s, allowQP=True))
 
 
 def predict_tag_of_parent_collection(
         vobject_items: Sequence[vobject.base.Component]) -> Optional[str]:
     """Returns the predicted tag or `None`"""
     if len(vobject_items) != 1:
         return None
@@ -87,15 +87,15 @@
 
     ``is_collection`` indicates that vobject_item contains unrelated
     components.
 
     The ``tag`` of the collection.
 
     """
-    if tag and tag not in ("VCALENDAR", "VADDRESSBOOK"):
+    if tag and tag not in ("VCALENDAR", "VADDRESSBOOK", "VSUBSCRIBED"):
         raise ValueError("Unsupported collection tag: %r" % tag)
     if not is_collection and len(vobject_items) != 1:
         raise ValueError("Item contains %d components" % len(vobject_items))
     if tag == "VCALENDAR":
         if len(vobject_items) > 1:
             raise RuntimeError("VCALENDAR collection contains %d "
                                "components" % len(vobject_items))
@@ -226,15 +226,15 @@
         if not isinstance(v, str):
             if v is None:
                 del props[k]
                 continue
             raise ValueError("Value of %r must be %r not %r: %r" % (
                 k, str.__name__, type(v).__name__, v))
         if k == "tag":
-            if v not in ("", "VCALENDAR", "VADDRESSBOOK"):
+            if v not in ("", "VCALENDAR", "VADDRESSBOOK", "VSUBSCRIBED"):
                 raise ValueError("Unsupported collection tag: %r" % v)
     return props
 
 
 def find_available_uid(exists_fn: Callable[[str], bool], suffix: str = ""
                        ) -> str:
     """Generate a pseudo-random UID"""
```

### Comparing `Radicale-3.1.9/radicale/item/filter.py` & `radicale-3.2.0/radicale/item/filter.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/log.py` & `radicale-3.2.0/radicale/log.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/pathutils.py` & `radicale-3.2.0/radicale/pathutils.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/rights/__init__.py` & `radicale-3.2.0/radicale/rights/__init__.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/rights/authenticated.py` & `radicale-3.2.0/radicale/rights/authenticated.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/rights/from_file.py` & `radicale-3.2.0/radicale/rights/from_file.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/rights/owner_only.py` & `radicale-3.2.0/radicale/rights/owner_only.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/rights/owner_write.py` & `radicale-3.2.0/radicale/rights/owner_write.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/server.py` & `radicale-3.2.0/radicale/server.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/__init__.py` & `radicale-3.2.0/radicale/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/__init__.py` & `radicale-3.2.0/radicale/storage/multifilesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/base.py` & `radicale-3.2.0/radicale/storage/multifilesystem/base.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/cache.py` & `radicale-3.2.0/radicale/storage/multifilesystem/cache.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/create_collection.py` & `radicale-3.2.0/radicale/storage/multifilesystem/create_collection.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/delete.py` & `radicale-3.2.0/radicale/storage/multifilesystem/delete.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/discover.py` & `radicale-3.2.0/radicale/storage/multifilesystem/discover.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/get.py` & `radicale-3.2.0/radicale/storage/multifilesystem/get.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/history.py` & `radicale-3.2.0/radicale/storage/multifilesystem/history.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/lock.py` & `radicale-3.2.0/radicale/storage/multifilesystem/lock.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/meta.py` & `radicale-3.2.0/radicale/storage/multifilesystem/meta.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/move.py` & `radicale-3.2.0/radicale/storage/multifilesystem/move.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/sync.py` & `radicale-3.2.0/radicale/storage/multifilesystem/sync.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/upload.py` & `radicale-3.2.0/radicale/storage/multifilesystem/upload.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem/verify.py` & `radicale-3.2.0/radicale/storage/multifilesystem/verify.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/storage/multifilesystem_nolock.py` & `radicale-3.2.0/radicale/storage/multifilesystem_nolock.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/types.py` & `radicale-3.2.0/radicale/types.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/utils.py` & `radicale-3.2.0/radicale/utils.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/web/__init__.py` & `radicale-3.2.0/radicale/web/__init__.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/web/internal.py` & `radicale-3.2.0/radicale/web/internal.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/web/internal_data/css/icon.png` & `radicale-3.2.0/radicale/web/internal_data/css/icon.png`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/web/internal_data/fn.js` & `radicale-3.2.0/radicale/web/internal_data/fn.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /**
  * This file is part of Radicale Server - Calendar Server
- * Copyright © 2017-2018 Unrud <unrud@outlook.com>
+ * Copyright © 2017-2024 Unrud <unrud@outlook.com>
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
@@ -24,22 +24,29 @@
 const SERVER = location.origin;
 
 /**
  * Path of the root collection on the server (must end with /)
  * @const
  * @type {string}
  */
-const ROOT_PATH = (new URL("..", location.href)).pathname;
+const ROOT_PATH = location.pathname.replace(new RegExp("/+[^/]+/*(/index\\.html?)?$"), "") + '/';
 
 /**
  * Regex to match and normalize color
  * @const
  */
 const COLOR_RE = new RegExp("^(#[0-9A-Fa-f]{6})(?:[0-9A-Fa-f]{2})?$");
 
+
+/**
+ * The text needed to confirm deleting a collection
+ * @const
+ */
+const DELETE_CONFIRMATION_TEXT = "DELETE";
+
 /**
  * Escape string for usage in XML
  * @param {string} s
  * @return {string}
  */
 function escape_xml(s) {
     return (s
@@ -59,14 +66,15 @@
     CALENDAR_JOURNAL_TASKS: "CALENDAR_JOURNAL_TASKS",
     CALENDAR_JOURNAL: "CALENDAR_JOURNAL",
     CALENDAR_TASKS: "CALENDAR_TASKS",
     JOURNAL_TASKS: "JOURNAL_TASKS",
     CALENDAR: "CALENDAR",
     JOURNAL: "JOURNAL",
     TASKS: "TASKS",
+    WEBCAL: "WEBCAL",
     is_subset: function(a, b) {
         let components = a.split("_");
         for (let i = 0; i < components.length; i++) {
             if (b.search(components[i]) === -1) {
                 return false;
             }
         }
@@ -85,33 +93,56 @@
         }
         if (a.search(this.JOURNAL) !== -1 || b.search(this.JOURNAL) !== -1) {
             union.push(this.JOURNAL);
         }
         if (a.search(this.TASKS) !== -1 || b.search(this.TASKS) !== -1) {
             union.push(this.TASKS);
         }
+        if (a.search(this.WEBCAL) !== -1 || b.search(this.WEBCAL) !== -1) {
+            union.push(this.WEBCAL);
+        }
         return union.join("_");
+    },
+    valid_options_for_type: function(a) {
+        a = a.trim().toUpperCase();
+        switch (a) {
+            case CollectionType.CALENDAR_JOURNAL_TASKS:
+            case CollectionType.CALENDAR_JOURNAL:
+            case CollectionType.CALENDAR_TASKS:
+            case CollectionType.JOURNAL_TASKS:
+            case CollectionType.CALENDAR:
+            case CollectionType.JOURNAL:
+            case CollectionType.TASKS:
+                return [CollectionType.CALENDAR_JOURNAL_TASKS, CollectionType.CALENDAR_JOURNAL, CollectionType.CALENDAR_TASKS, CollectionType.JOURNAL_TASKS, CollectionType.CALENDAR, CollectionType.JOURNAL, CollectionType.TASKS];
+            case CollectionType.ADDRESSBOOK:
+            case CollectionType.WEBCAL:
+            default:
+                return [a];
+        }
     }
 };
 
 /**
  * @constructor
  * @struct
  * @param {string} href Must always start and end with /.
  * @param {CollectionType} type
  * @param {string} displayname
  * @param {string} description
  * @param {string} color
  */
-function Collection(href, type, displayname, description, color) {
+function Collection(href, type, displayname, description, color, contentcount, size, source) {
     this.href = href;
     this.type = type;
     this.displayname = displayname;
     this.color = color;
     this.description = description;
+    this.source = source;
+    this.contentcount = contentcount;
+    this.size = size;
 }
 
 /**
  * Find the principal collection.
  * @param {string} user
  * @param {string} password
  * @param {function(?Collection, ?string)} callback Returns result or error
@@ -130,14 +161,15 @@
             let displayname_element = xml.querySelector("*|multistatus:root > *|response:first-of-type > *|propstat > *|prop > *|displayname");
             if (principal_element) {
                 callback(new Collection(
                     principal_element.textContent,
                     CollectionType.PRINCIPAL,
                     displayname_element ? displayname_element.textContent : "",
                     "",
+                    0,
                     ""), null);
             } else {
                 callback(null, "Internal error");
             }
         } else {
             callback(null, request.status + " " + request.statusText);
         }
@@ -179,53 +211,68 @@
                 let resourcetype_query = response_query + " > *|propstat > *|prop > *|resourcetype";
                 let resourcetype_element = response.querySelector(resourcetype_query);
                 let displayname_element = response.querySelector(response_query + " > *|propstat > *|prop > *|displayname");
                 let calendarcolor_element = response.querySelector(response_query + " > *|propstat > *|prop > *|calendar-color");
                 let addressbookcolor_element = response.querySelector(response_query + " > *|propstat > *|prop > *|addressbook-color");
                 let calendardesc_element = response.querySelector(response_query + " > *|propstat > *|prop > *|calendar-description");
                 let addressbookdesc_element = response.querySelector(response_query + " > *|propstat > *|prop > *|addressbook-description");
+                let contentcount_element = response.querySelector(response_query + " > *|propstat > *|prop > *|getcontentcount");
+                let contentlength_element = response.querySelector(response_query + " > *|propstat > *|prop > *|getcontentlength");
+                let webcalsource_element = response.querySelector(response_query + " > *|propstat > *|prop > *|source");
                 let components_query = response_query + " > *|propstat > *|prop > *|supported-calendar-component-set";
                 let components_element = response.querySelector(components_query);
                 let href = href_element ? href_element.textContent : "";
                 let displayname = displayname_element ? displayname_element.textContent : "";
                 let type = "";
                 let color = "";
                 let description = "";
+                let source = "";
+                let count = 0;
+                let size = 0;
                 if (resourcetype_element) {
                     if (resourcetype_element.querySelector(resourcetype_query + " > *|addressbook")) {
                         type = CollectionType.ADDRESSBOOK;
                         color = addressbookcolor_element ? addressbookcolor_element.textContent : "";
                         description = addressbookdesc_element ? addressbookdesc_element.textContent : "";
+                        count = contentcount_element ? parseInt(contentcount_element.textContent) : 0;
+                        size = contentlength_element ? parseInt(contentlength_element.textContent) : 0;
+                    } else if (resourcetype_element.querySelector(resourcetype_query + " > *|subscribed")) {
+                        type = CollectionType.WEBCAL;
+                        source = webcalsource_element ? webcalsource_element.textContent : "";
+                        color = calendarcolor_element ? calendarcolor_element.textContent : "";
+                        description = calendardesc_element ? calendardesc_element.textContent : "";
                     } else if (resourcetype_element.querySelector(resourcetype_query + " > *|calendar")) {
                         if (components_element) {
                             if (components_element.querySelector(components_query + " > *|comp[name=VEVENT]")) {
                                 type = CollectionType.union(type, CollectionType.CALENDAR);
                             }
                             if (components_element.querySelector(components_query + " > *|comp[name=VJOURNAL]")) {
                                 type = CollectionType.union(type, CollectionType.JOURNAL);
                             }
                             if (components_element.querySelector(components_query + " > *|comp[name=VTODO]")) {
                                 type = CollectionType.union(type, CollectionType.TASKS);
                             }
                         }
                         color = calendarcolor_element ? calendarcolor_element.textContent : "";
                         description = calendardesc_element ? calendardesc_element.textContent : "";
+                        count = contentcount_element ? parseInt(contentcount_element.textContent) : 0;
+                        size = contentlength_element ? parseInt(contentlength_element.textContent) : 0;
                     }
                 }
                 let sane_color = color.trim();
                 if (sane_color) {
                     let color_match = COLOR_RE.exec(sane_color);
                     if (color_match) {
                         sane_color = color_match[1];
                     } else {
                         sane_color = "";
                     }
                 }
                 if (href.substr(-1) === "/" && href !== collection.href && type) {
-                    collections.push(new Collection(href, type, displayname, description, sane_color));
+                    collections.push(new Collection(href, type, displayname, description, sane_color, count, size, source));
                 }
             }
             collections.sort(function(a, b) {
                 /** @type {string} */
                 let ca = a.displayname || a.href;
                 /** @type {string} */
                 let cb = b.displayname || b.href;
@@ -233,27 +280,34 @@
             });
             callback(collections, null);
         } else {
             callback(null, request.status + " " + request.statusText);
         }
     };
     request.send('<?xml version="1.0" encoding="utf-8" ?>' +
-        '<propfind xmlns="DAV:" xmlns:C="urn:ietf:params:xml:ns:caldav" ' +
+        '<propfind ' +
+        'xmlns="DAV:" ' +
+        'xmlns:C="urn:ietf:params:xml:ns:caldav" ' +
         'xmlns:CR="urn:ietf:params:xml:ns:carddav" ' +
+        'xmlns:CS="http://calendarserver.org/ns/" ' +
         'xmlns:I="http://apple.com/ns/ical/" ' +
         'xmlns:INF="http://inf-it.com/ns/ab/" ' +
-        'xmlns:RADICALE="http://radicale.org/ns/">' +
+        'xmlns:RADICALE="http://radicale.org/ns/"' +
+        '>' +
         '<prop>' +
         '<resourcetype />' +
         '<RADICALE:displayname />' +
         '<I:calendar-color />' +
         '<INF:addressbook-color />' +
         '<C:calendar-description />' +
         '<C:supported-calendar-component-set />' +
         '<CR:addressbook-description />' +
+        '<CS:source />' +
+        '<RADICALE:getcontentcount />' +
+        '<getcontentlength />' +
         '</prop>' +
         '</propfind>');
     return request;
 }
 
 /**
  * @param {string} user
@@ -327,20 +381,26 @@
         }
     };
     let displayname = escape_xml(collection.displayname);
     let calendar_color = "";
     let addressbook_color = "";
     let calendar_description = "";
     let addressbook_description = "";
+    let calendar_source = "";
     let resourcetype;
     let components = "";
     if (collection.type === CollectionType.ADDRESSBOOK) {
         addressbook_color = escape_xml(collection.color + (collection.color ? "ff" : ""));
         addressbook_description = escape_xml(collection.description);
         resourcetype = '<CR:addressbook />';
+    } else if (collection.type === CollectionType.WEBCAL) {
+        calendar_color = escape_xml(collection.color + (collection.color ? "ff" : ""));
+        calendar_description = escape_xml(collection.description);
+        resourcetype = '<CS:subscribed />';
+        calendar_source = collection.source;
     } else {
         calendar_color = escape_xml(collection.color + (collection.color ? "ff" : ""));
         calendar_description = escape_xml(collection.description);
         resourcetype = '<C:calendar />';
         if (CollectionType.is_subset(CollectionType.CALENDAR, collection.type)) {
             components += '<C:comp name="VEVENT" />';
         }
@@ -349,24 +409,25 @@
         }
         if (CollectionType.is_subset(CollectionType.TASKS, collection.type)) {
             components += '<C:comp name="VTODO" />';
         }
     }
     let xml_request = create ? "mkcol" : "propertyupdate";
     request.send('<?xml version="1.0" encoding="UTF-8" ?>' +
-        '<' + xml_request + ' xmlns="DAV:" xmlns:C="urn:ietf:params:xml:ns:caldav" xmlns:CR="urn:ietf:params:xml:ns:carddav" xmlns:I="http://apple.com/ns/ical/" xmlns:INF="http://inf-it.com/ns/ab/">' +
+        '<' + xml_request + ' xmlns="DAV:" xmlns:C="urn:ietf:params:xml:ns:caldav" xmlns:CR="urn:ietf:params:xml:ns:carddav" xmlns:CS="http://calendarserver.org/ns/" xmlns:I="http://apple.com/ns/ical/" xmlns:INF="http://inf-it.com/ns/ab/">' +
         '<set>' +
         '<prop>' +
         (create ? '<resourcetype><collection />' + resourcetype + '</resourcetype>' : '') +
         (components ? '<C:supported-calendar-component-set>' + components + '</C:supported-calendar-component-set>' : '') +
         (displayname ? '<displayname>' + displayname + '</displayname>' : '') +
         (calendar_color ? '<I:calendar-color>' + calendar_color + '</I:calendar-color>' : '') +
         (addressbook_color ? '<INF:addressbook-color>' + addressbook_color + '</INF:addressbook-color>' : '') +
         (addressbook_description ? '<CR:addressbook-description>' + addressbook_description + '</CR:addressbook-description>' : '') +
         (calendar_description ? '<C:calendar-description>' + calendar_description + '</C:calendar-description>' : '') +
+        (calendar_source ? '<CS:source>' + calendar_source + '</CS:source>' : '') +
         '</prop>' +
         '</set>' +
         (!create ? ('<remove>' +
             '<prop>' +
             (!components ? '<C:supported-calendar-component-set />' : '') +
             (!displayname ? '<displayname />' : '') +
             (!calendar_color ? '<I:calendar-color />' : '') +
@@ -479,15 +540,16 @@
     let html_scene = document.getElementById("loginscene");
     let form = html_scene.querySelector("[data-name=form]");
     let user_form = html_scene.querySelector("[data-name=user]");
     let password_form = html_scene.querySelector("[data-name=password]");
     let error_form = html_scene.querySelector("[data-name=error]");
     let logout_view = document.getElementById("logoutview");
     let logout_user_form = logout_view.querySelector("[data-name=user]");
-    let logout_btn = logout_view.querySelector("[data-name=link]");
+    let logout_btn = logout_view.querySelector("[data-name=logout]");
+    let refresh_btn = logout_view.querySelector("[data-name=refresh]");
 
     /** @type {?number} */
     let scene_index = null;
     let user = "";
     let error = "";
     /** @type {?XMLHttpRequest} */
     let principal_req = null;
@@ -495,27 +557,33 @@
     function read_form() {
         user = user_form.value;
     }
 
     function fill_form() {
         user_form.value = user;
         password_form.value = "";
-        error_form.textContent = error ? "Error: " + error : "";
+        if (error) {
+            error_form.textContent = "Error: " + error;
+            error_form.classList.remove("hidden");
+        } else {
+            error_form.classList.add("hidden");
+        }
     }
 
     function onlogin() {
         try {
             read_form();
             let password = password_form.value;
             if (user) {
                 error = "";
                 // setup logout
                 logout_view.classList.remove("hidden");
                 logout_btn.onclick = onlogout;
-                logout_user_form.textContent = user;
+                refresh_btn.onclick = refresh;
+                logout_user_form.textContent = user + "'s Collections";
                 // Fetch principal
                 let loading_scene = new LoadingScene();
                 push_scene(loading_scene, false);
                 principal_req = get_principal(user, password, function(collection, error1) {
                     if (scene_index === null) {
                         return;
                     }
@@ -558,17 +626,25 @@
         }
         return false;
     }
 
     function remove_logout() {
         logout_view.classList.add("hidden");
         logout_btn.onclick = null;
+        refresh_btn.onclick = null;
         logout_user_form.textContent = "";
     }
 
+    function refresh() {
+        //The easiest way to refresh is to push a LoadingScene onto the stack and then pop it
+        //forcing the scene below it, the Collections Scene to refresh itself.
+        push_scene(new LoadingScene(), false);
+        pop_scene(scene_stack.length - 2);
+    }
+
     this.show = function() {
         remove_logout();
         fill_form();
         form.onsubmit = onlogin;
         html_scene.classList.remove("hidden");
         scene_index = scene_stack.length - 1;
         user_form.focus();
@@ -623,43 +699,29 @@
     let scene_index = null;
     /** @type {?XMLHttpRequest} */
     let collections_req = null;
     /** @type {?Array<Collection>} */
     let collections = null;
     /** @type {Array<Node>} */
     let nodes = [];
-    let filesInput = document.createElement("input");
-    filesInput.setAttribute("type", "file");
-    filesInput.setAttribute("accept", ".ics, .vcf");
-    filesInput.setAttribute("multiple", "");
-    let filesInputForm = document.createElement("form");
-    filesInputForm.appendChild(filesInput);
 
     function onnew() {
         try {
             let create_collection_scene = new CreateEditCollectionScene(user, password, collection);
             push_scene(create_collection_scene, false);
         } catch (err) {
             console.error(err);
         }
         return false;
     }
 
     function onupload() {
-        filesInput.click();
-        return false;
-    }
-
-    function onfileschange() {
         try {
-            let files = filesInput.files;
-            if (files.length > 0) {
-                let upload_scene = new UploadCollectionScene(user, password, collection, files);
-                push_scene(upload_scene);
-            }
+            let upload_scene = new UploadCollectionScene(user, password, collection);
+            push_scene(upload_scene);
         } catch (err) {
             console.error(err);
         }
         return false;
     }
 
     function onedit(collection) {
@@ -679,29 +741,32 @@
         } catch (err) {
             console.error(err);
         }
         return false;
     }
 
     function show_collections(collections) {
+        let heightOfNavBar = document.querySelector("#logoutview").offsetHeight + "px";
+        html_scene.style.marginTop = heightOfNavBar;
+        html_scene.style.height = "calc(100vh - " + heightOfNavBar + ")";
         collections.forEach(function(collection) {
             let node = template.cloneNode(true);
             node.classList.remove("hidden");
             let title_form = node.querySelector("[data-name=title]");
             let description_form = node.querySelector("[data-name=description]");
+            let contentcount_form = node.querySelector("[data-name=contentcount]");
             let url_form = node.querySelector("[data-name=url]");
             let color_form = node.querySelector("[data-name=color]");
             let delete_btn = node.querySelector("[data-name=delete]");
             let edit_btn = node.querySelector("[data-name=edit]");
+            let download_btn = node.querySelector("[data-name=download]");
             if (collection.color) {
-                color_form.style.color = collection.color;
-            } else {
-                color_form.classList.add("hidden");
+                color_form.style.background = collection.color;
             }
-            let possible_types = [CollectionType.ADDRESSBOOK];
+            let possible_types = [CollectionType.ADDRESSBOOK, CollectionType.WEBCAL];
             [CollectionType.CALENDAR, ""].forEach(function(e) {
                 [CollectionType.union(e, CollectionType.JOURNAL), e].forEach(function(e) {
                     [CollectionType.union(e, CollectionType.TASKS), e].forEach(function(e) {
                         if (e) {
                             possible_types.push(e);
                         }
                     });
@@ -709,18 +774,34 @@
             });
             possible_types.forEach(function(e) {
                 if (e !== collection.type) {
                     node.querySelector("[data-name=" + e + "]").classList.add("hidden");
                 }
             });
             title_form.textContent = collection.displayname || collection.href;
+            if (title_form.textContent.length > 30) {
+                title_form.classList.add("smalltext");
+            }
             description_form.textContent = collection.description;
+            if (description_form.textContent.length > 150) {
+                description_form.classList.add("smalltext");
+            }
+            if (collection.type != CollectionType.WEBCAL) {
+                let contentcount_form_txt = (collection.contentcount > 0 ? Number(collection.contentcount).toLocaleString() : "No") + " item" + (collection.contentcount == 1 ? "" : "s") + " in collection";
+                if (collection.contentcount > 0) {
+                    contentcount_form_txt += " (" + bytesToHumanReadable(collection.size) + ")";
+                }
+                contentcount_form.textContent = contentcount_form_txt;
+            }
             let href = SERVER + collection.href;
-            url_form.href = href;
-            url_form.textContent = href;
+            url_form.value = href;
+            download_btn.href = href;
+            if (collection.type == CollectionType.WEBCAL) {
+                download_btn.parentElement.classList.add("hidden");
+            }
             delete_btn.onclick = function() {
                 return ondelete(collection);
             };
             edit_btn.onclick = function() {
                 return onedit(collection);
             };
             node.classList.remove("hidden");
@@ -747,94 +828,136 @@
         });
     }
 
     this.show = function() {
         html_scene.classList.remove("hidden");
         new_btn.onclick = onnew;
         upload_btn.onclick = onupload;
-        filesInputForm.reset();
-        filesInput.onchange = onfileschange;
         if (collections === null) {
             update();
         } else {
             // from update loading scene
             show_collections(collections);
         }
     };
     this.hide = function() {
         html_scene.classList.add("hidden");
         scene_index = scene_stack.length - 1;
         new_btn.onclick = null;
         upload_btn.onclick = null;
-        filesInput.onchange = null;
         collections = null;
         // remove collection
         nodes.forEach(function(node) {
             node.parentNode.removeChild(node);
         });
         nodes = [];
     };
     this.release = function() {
         scene_index = null;
         if (collections_req !== null) {
             collections_req.abort();
             collections_req = null;
         }
         collections = null;
-        filesInputForm.reset();
     };
 }
 
 /**
  * @constructor
  * @implements {Scene}
  * @param {string} user
  * @param {string} password
  * @param {Collection} collection parent collection
  * @param {Array<File>} files
  */
-function UploadCollectionScene(user, password, collection, files) {
+function UploadCollectionScene(user, password, collection) {
     let html_scene = document.getElementById("uploadcollectionscene");
     let template = html_scene.querySelector("[data-name=filetemplate]");
+    let upload_btn = html_scene.querySelector("[data-name=submit]");
     let close_btn = html_scene.querySelector("[data-name=close]");
+    let uploadfile_form = html_scene.querySelector("[data-name=uploadfile]");
+    let uploadfile_lbl = html_scene.querySelector("label[for=uploadfile]");
+    let href_form = html_scene.querySelector("[data-name=href]");
+    let href_label = html_scene.querySelector("label[for=href]");
+    let hreflimitmsg_html = html_scene.querySelector("[data-name=hreflimitmsg]");
+    let pending_html = html_scene.querySelector("[data-name=pending]");
+
+    let files = uploadfile_form.files;
+    href_form.addEventListener("keydown", cleanHREFinput);
+    upload_btn.onclick = upload_start;
+    uploadfile_form.onchange = onfileschange;
+
+    let href = random_uuid();
+    href_form.value = href;
 
     /** @type {?number} */
     let scene_index = null;
     /** @type {?XMLHttpRequest} */
     let upload_req = null;
     /** @type {Array<string>} */
-    let errors = [];
+    let results = [];
     /** @type {?Array<Node>} */
     let nodes = null;
 
+    function upload_start() {
+        try {
+            if (!read_form()) {
+                return false;
+            }
+            uploadfile_form.classList.add("hidden");
+            uploadfile_lbl.classList.add("hidden");
+            href_form.classList.add("hidden");
+            href_label.classList.add("hidden");
+            hreflimitmsg_html.classList.add("hidden");
+            upload_btn.classList.add("hidden");
+            close_btn.classList.add("hidden");
+
+            pending_html.classList.remove("hidden");
+
+            nodes = [];
+            for (let i = 0; i < files.length; i++) {
+                let file = files[i];
+                let node = template.cloneNode(true);
+                node.classList.remove("hidden");
+                let name_form = node.querySelector("[data-name=name]");
+                name_form.textContent = file.name;
+                node.classList.remove("hidden");
+                nodes.push(node);
+                updateFileStatus(i);
+                template.parentNode.insertBefore(node, template);
+            }
+            upload_next();
+        } catch (err) {
+            console.error(err);
+        }
+        return false;
+    }
+
     function upload_next() {
         try {
-            if (files.length === errors.length) {
-                if (errors.every(error => error === null)) {
-                    pop_scene(scene_index - 1);
-                } else {
-                    close_btn.classList.remove("hidden");
-                }
+            if (files.length === results.length) {
+                pending_html.classList.add("hidden");
+                close_btn.classList.remove("hidden");
+                return;
             } else {
-                let file = files[errors.length];
-                let upload_href = collection.href + random_uuid() + "/";
-                upload_req = upload_collection(user, password, upload_href, file, function(error) {
-                    if (scene_index === null) {
-                        return;
-                    }
+                let file = files[results.length];
+                if (files.length > 1 || href.length == 0) {
+                    href = random_uuid();
+                }
+                let upload_href = collection.href + "/" + href + "/";
+                upload_req = upload_collection(user, password, upload_href, file, function(result) {
                     upload_req = null;
-                    errors.push(error);
-                    updateFileStatus(errors.length - 1);
+                    results.push(result);
+                    updateFileStatus(results.length - 1);
                     upload_next();
                 });
             }
         } catch (err) {
             console.error(err);
         }
-        return false;
     }
 
     function onclose() {
         try {
             pop_scene(scene_index - 1);
         } catch (err) {
             console.error(err);
@@ -842,62 +965,85 @@
         return false;
     }
 
     function updateFileStatus(i) {
         if (nodes === null) {
             return;
         }
-        let pending_form = nodes[i].querySelector("[data-name=pending]");
         let success_form = nodes[i].querySelector("[data-name=success]");
         let error_form = nodes[i].querySelector("[data-name=error]");
-        if (errors.length > i) {
-            pending_form.classList.add("hidden");
-            if (errors[i]) {
+        if (results.length > i) {
+            if (results[i]) {
                 success_form.classList.add("hidden");
-                error_form.textContent = "Error: " + errors[i];
+                error_form.textContent = "Error: " + results[i];
                 error_form.classList.remove("hidden");
             } else {
                 success_form.classList.remove("hidden");
                 error_form.classList.add("hidden");
             }
         } else {
-            pending_form.classList.remove("hidden");
             success_form.classList.add("hidden");
             error_form.classList.add("hidden");
         }
     }
 
+    function read_form() {
+        cleanHREFinput(href_form);
+        let newhreftxtvalue = href_form.value.trim().toLowerCase();
+        if (!isValidHREF(newhreftxtvalue)) {
+            alert("You must enter a valid HREF");
+            return false;
+        }
+        href = newhreftxtvalue;
+
+        if (uploadfile_form.files.length == 0) {
+            alert("You must select at least one file to upload");
+            return false;
+        }
+        files = uploadfile_form.files;
+        return true;
+    }
+
+    function onfileschange() {
+        files = uploadfile_form.files;
+        if (files.length > 1) {
+            hreflimitmsg_html.classList.remove("hidden");
+            href_form.classList.add("hidden");
+            href_label.classList.add("hidden");
+        } else {
+            hreflimitmsg_html.classList.add("hidden");
+            href_form.classList.remove("hidden");
+            href_label.classList.remove("hidden");
+        }
+        return false;
+    }
+
     this.show = function() {
+        scene_index = scene_stack.length - 1;
         html_scene.classList.remove("hidden");
-        if (errors.length < files.length) {
-            close_btn.classList.add("hidden");
-        }
         close_btn.onclick = onclose;
-        nodes = [];
-        for (let i = 0; i < files.length; i++) {
-            let file = files[i];
-            let node = template.cloneNode(true);
-            node.classList.remove("hidden");
-            let name_form = node.querySelector("[data-name=name]");
-            name_form.textContent = file.name;
-            node.classList.remove("hidden");
-            nodes.push(node);
-            updateFileStatus(i);
-            template.parentNode.insertBefore(node, template);
-        }
-        if (scene_index === null) {
-            scene_index = scene_stack.length - 1;
-            upload_next();
-        }
     };
 
     this.hide = function() {
         html_scene.classList.add("hidden");
         close_btn.classList.remove("hidden");
+        upload_btn.classList.remove("hidden");
+        uploadfile_form.classList.remove("hidden");
+        uploadfile_lbl.classList.remove("hidden");
+        href_form.classList.remove("hidden");
+        href_label.classList.remove("hidden");
+        hreflimitmsg_html.classList.add("hidden");
+        pending_html.classList.add("hidden");
         close_btn.onclick = null;
+        upload_btn.onclick = null;
+        href_form.value = "";
+        uploadfile_form.value = "";
+        if (nodes == null) {
+            return;
+        }
         nodes.forEach(function(node) {
             node.parentNode.removeChild(node);
         });
         nodes = null;
     };
     this.release = function() {
         scene_index = null;
@@ -915,24 +1061,35 @@
  * @param {string} password
  * @param {Collection} collection
  */
 function DeleteCollectionScene(user, password, collection) {
     let html_scene = document.getElementById("deletecollectionscene");
     let title_form = html_scene.querySelector("[data-name=title]");
     let error_form = html_scene.querySelector("[data-name=error]");
+    let confirmation_txt = html_scene.querySelector("[data-name=confirmationtxt]");
+    let delete_confirmation_lbl = html_scene.querySelector("[data-name=deleteconfirmationtext]");
     let delete_btn = html_scene.querySelector("[data-name=delete]");
     let cancel_btn = html_scene.querySelector("[data-name=cancel]");
 
+    delete_confirmation_lbl.innerHTML = DELETE_CONFIRMATION_TEXT;
+    confirmation_txt.value = "";
+    confirmation_txt.addEventListener("keydown", onkeydown);
+
     /** @type {?number} */
     let scene_index = null;
     /** @type {?XMLHttpRequest} */
     let delete_req = null;
     let error = "";
 
     function ondelete() {
+        let confirmation_text_value = confirmation_txt.value;
+        if (confirmation_text_value != DELETE_CONFIRMATION_TEXT) {
+            alert("Please type the confirmation text to delete this collection.");
+            return;
+        }
         try {
             let loading_scene = new LoadingScene();
             push_scene(loading_scene);
             delete_req = delete_collection(user, password, collection, function(error1) {
                 if (scene_index === null) {
                     return;
                 }
@@ -955,22 +1112,35 @@
             pop_scene(scene_index - 1);
         } catch (err) {
             console.error(err);
         }
         return false;
     }
 
+    function onkeydown(event) {
+        if (event.keyCode !== 13) {
+            return;
+        }
+        ondelete();
+    }
+
     this.show = function() {
         this.release();
         scene_index = scene_stack.length - 1;
         html_scene.classList.remove("hidden");
         title_form.textContent = collection.displayname || collection.href;
-        error_form.textContent = error ? "Error: " + error : "";
         delete_btn.onclick = ondelete;
         cancel_btn.onclick = oncancel;
+        if (error) {
+            error_form.textContent = "Error: " + error;
+            error_form.classList.remove("hidden");
+        } else {
+            error_form.classList.add("hidden");
+        }
+
     };
     this.hide = function() {
         html_scene.classList.add("hidden");
         cancel_btn.onclick = null;
         delete_btn.onclick = null;
     };
     this.release = function() {
@@ -1003,80 +1173,118 @@
  *                                Otherwise the collection will be edited.
  */
 function CreateEditCollectionScene(user, password, collection) {
     let edit = collection.type !== CollectionType.PRINCIPAL;
     let html_scene = document.getElementById(edit ? "editcollectionscene" : "createcollectionscene");
     let title_form = edit ? html_scene.querySelector("[data-name=title]") : null;
     let error_form = html_scene.querySelector("[data-name=error]");
+    let href_form = html_scene.querySelector("[data-name=href]");
+    let href_label = html_scene.querySelector("label[for=href]");
     let displayname_form = html_scene.querySelector("[data-name=displayname]");
+    let displayname_label = html_scene.querySelector("label[for=displayname]");
     let description_form = html_scene.querySelector("[data-name=description]");
+    let description_label = html_scene.querySelector("label[for=description]");
+    let source_form = html_scene.querySelector("[data-name=source]");
+    let source_label = html_scene.querySelector("label[for=source]");
     let type_form = html_scene.querySelector("[data-name=type]");
+    let type_label = html_scene.querySelector("label[for=type]");
     let color_form = html_scene.querySelector("[data-name=color]");
+    let color_label = html_scene.querySelector("label[for=color]");
     let submit_btn = html_scene.querySelector("[data-name=submit]");
     let cancel_btn = html_scene.querySelector("[data-name=cancel]");
 
+
     /** @type {?number} */
     let scene_index = null;
     /** @type {?XMLHttpRequest} */
     let create_edit_req = null;
     let error = "";
     /** @type {?Element} */
     let saved_type_form = null;
 
     let href = edit ? collection.href : collection.href + random_uuid() + "/";
     let displayname = edit ? collection.displayname : "";
     let description = edit ? collection.description : "";
+    let source = edit ? collection.source : "";
     let type = edit ? collection.type : CollectionType.CALENDAR_JOURNAL_TASKS;
     let color = edit && collection.color ? collection.color : "#" + random_hex(6);
 
+    if (!edit) {
+        href_form.addEventListener("keydown", cleanHREFinput);
+    }
+
     function remove_invalid_types() {
         if (!edit) {
             return;
         }
         /** @type {HTMLOptionsCollection} */
         let options = type_form.options;
         // remove all options that are not supersets
+        let valid_type_options = CollectionType.valid_options_for_type(type);
         for (let i = options.length - 1; i >= 0; i--) {
-            if (!CollectionType.is_subset(type, options[i].value)) {
+            if (valid_type_options.indexOf(options[i].value) < 0) {
                 options.remove(i);
             }
         }
     }
 
     function read_form() {
+        if (!edit) {
+            cleanHREFinput(href_form);
+            let newhreftxtvalue = href_form.value.trim().toLowerCase();
+            if (!isValidHREF(newhreftxtvalue)) {
+                alert("You must enter a valid HREF");
+                return false;
+            }
+            href = collection.href + "/" + newhreftxtvalue + "/";
+        }
         displayname = displayname_form.value;
         description = description_form.value;
+        source = source_form.value;
         type = type_form.value;
         color = color_form.value;
+        return true;
     }
 
     function fill_form() {
+        if (!edit) {
+            href_form.value = random_uuid();
+        }
         displayname_form.value = displayname;
         description_form.value = description;
+        source_form.value = source;
         type_form.value = type;
         color_form.value = color;
-        error_form.textContent = error ? "Error: " + error : "";
+        if (error) {
+            error_form.textContent = "Error: " + error;
+            error_form.classList.remove("hidden");
+        }
+        error_form.classList.add("hidden");
+        onTypeChange();
+        type_form.addEventListener("change", onTypeChange);
     }
 
     function onsubmit() {
         try {
-            read_form();
+            if (!read_form()) {
+                return false;
+            }
             let sane_color = color.trim();
             if (sane_color) {
                 let color_match = COLOR_RE.exec(sane_color);
                 if (!color_match) {
                     error = "Invalid color";
                     fill_form();
                     return false;
                 }
                 sane_color = color_match[1];
             }
             let loading_scene = new LoadingScene();
             push_scene(loading_scene);
-            let collection = new Collection(href, type, displayname, description, sane_color);
+            let collection = new Collection(href, type, displayname, description, sane_color, 0, 0, source);
             let callback = function(error1) {
                 if (scene_index === null) {
                     return;
                 }
                 create_edit_req = null;
                 if (error1) {
                     error = error1;
@@ -1101,14 +1309,25 @@
             pop_scene(scene_index - 1);
         } catch (err) {
             console.error(err);
         }
         return false;
     }
 
+
+    function onTypeChange(e) {
+        if (type_form.value == CollectionType.WEBCAL) {
+            source_label.classList.remove("hidden");
+            source_form.classList.remove("hidden");
+        } else {
+            source_label.classList.add("hidden");
+            source_form.classList.add("hidden");
+        }
+    }
+
     this.show = function() {
         this.release();
         scene_index = scene_stack.length - 1;
         // Clone type_form because it's impossible to hide options without removing them
         saved_type_form = type_form;
         type_form = type_form.cloneNode(true);
         saved_type_form.parentNode.replaceChild(type_form, saved_type_form);
@@ -1136,14 +1355,65 @@
         if (create_edit_req !== null) {
             create_edit_req.abort();
             create_edit_req = null;
         }
     };
 }
 
+/**
+ * Removed invalid HREF characters for a collection HREF.
+ *
+ * @param a A valid Input element or an onchange Event of an Input element.
+ */
+function cleanHREFinput(a) {
+    let href_form = a;
+    if (a.target) {
+        href_form = a.target;
+    }
+    let currentTxtVal = href_form.value.trim().toLowerCase();
+    //Clean the HREF to remove non lowercase letters and dashes
+    currentTxtVal = currentTxtVal.replace(/(?![0-9a-z\-\_])./g, '');
+    href_form.value = currentTxtVal;
+}
+
+/**
+ * Checks if a proposed HREF for a collection has a valid format and syntax.
+ *
+ * @param href String of the porposed HREF.
+ *
+ * @return Boolean results if the HREF is valid.
+ */
+function isValidHREF(href) {
+    if (href.length < 1) {
+        return false;
+    }
+    if (href.indexOf("/") != -1) {
+        return false;
+    }
+
+    return true;
+}
+
+/**
+ * Format bytes to human-readable text.
+ *
+ * @param bytes Number of bytes.
+ *
+ * @return Formatted string.
+ */
+function bytesToHumanReadable(bytes, dp = 1) {
+    let isNumber = !isNaN(parseFloat(bytes)) && !isNaN(bytes - 0);
+    if (!isNumber) {
+        return "";
+    }
+    var i = bytes == 0 ? 0 : Math.floor(Math.log(bytes) / Math.log(1024));
+    return (bytes / Math.pow(1024, i)).toFixed(dp) * 1 + ' ' + ['b', 'kb', 'mb', 'gb', 'tb'][i];
+}
+
+
 function main() {
     // Hide startup loading message
     document.getElementById("loadingscene").classList.add("hidden");
     push_scene(new LoginScene(), false);
 }
 
 window.addEventListener("load", main);
```

### Comparing `Radicale-3.1.9/radicale/web/none.py` & `radicale-3.2.0/radicale/web/none.py`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/radicale/xmlutils.py` & `radicale-3.2.0/radicale/xmlutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 from typing import Dict, Mapping, Optional
 from urllib.parse import quote
 
 from radicale import item, pathutils
 
 MIMETYPES: Mapping[str, str] = {
     "VADDRESSBOOK": "text/vcard",
-    "VCALENDAR": "text/calendar"}
+    "VCALENDAR": "text/calendar",
+    "VSUBSCRIBED": "text/calendar"}
 
 OBJECT_MIMETYPES: Mapping[str, str] = {
     "VCARD": "text/vcard",
     "VLIST": "text/x-vlist",
     "VCALENDAR": "text/calendar"}
 
 NAMESPACES: Mapping[str, str] = {
@@ -173,14 +174,17 @@
         if prop.tag == make_clark("D:resourcetype"):
             key = "tag"
             if is_set:
                 for resource_type in prop:
                     if resource_type.tag == make_clark("C:calendar"):
                         value = "VCALENDAR"
                         break
+                    if resource_type.tag == make_clark("CS:subscribed"):
+                        value = "VSUBSCRIBED"
+                        break
                     if resource_type.tag == make_clark("CR:addressbook"):
                         value = "VADDRESSBOOK"
                         break
         elif prop.tag == make_clark("C:supported-calendar-component-set"):
             if is_set:
                 value = ",".join(
                     supported_comp.attrib["name"] for supported_comp in prop
```

### Comparing `Radicale-3.1.9/rights` & `radicale-3.2.0/rights`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/setup.cfg` & `radicale-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `Radicale-3.1.9/setup.py` & `radicale-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 # You should have received a copy of the GNU General Public License
 # along with Radicale.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
 # When the version is updated, a new section in the CHANGELOG.md file must be
 # added too.
-VERSION = "3.1.9"
+VERSION = "3.2.0"
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 web_files = ["web/internal_data/css/icon.png",
              "web/internal_data/css/main.css",
              "web/internal_data/fn.js",
              "web/internal_data/index.html"]
 
 install_requires = ["defusedxml", "passlib", "vobject>=0.9.6",
                     "python-dateutil>=2.7.3",
+                    "pika>=1.1.0",
                     "setuptools; python_version<'3.9'"]
 bcrypt_requires = ["bcrypt"]
 # typeguard requires pytest<7
 test_requires = ["pytest<7", "typeguard<3", "waitress", *bcrypt_requires]
 
 setup(
     name="Radicale",
@@ -49,25 +50,24 @@
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     package_data={"radicale": [*web_files, "py.typed"]},
     entry_points={"console_scripts": ["radicale = radicale.__main__:run"]},
     install_requires=install_requires,
     extras_require={"test": test_requires, "bcrypt": bcrypt_requires},
     keywords=["calendar", "addressbook", "CalDAV", "CardDAV"],
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
```


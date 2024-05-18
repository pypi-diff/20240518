# Comparing `tmp/ntdgotv_langtools-0.1.tar.gz` & `tmp/ntdgotv_langtools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdgotv_langtools-0.1.tar", last modified: Fri May 17 18:22:53 2024, max compression
+gzip compressed data, was "ntdgotv_langtools-0.1.1.tar", last modified: Fri May 17 19:47:28 2024, max compression
```

## Comparing `ntdgotv_langtools-0.1.tar` & `ntdgotv_langtools-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:22:53.211194 ntdgotv_langtools-0.1/
--rw-rw-rw-   0        0        0       62 2024-05-17 18:22:53.208665 ntdgotv_langtools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-05-17 17:44:40.000000 ntdgotv_langtools-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 18:22:53.185718 ntdgotv_langtools-0.1/ntdgotv_langtools/
--rw-rw-rw-   0        0        0       25 2024-05-17 18:05:47.000000 ntdgotv_langtools-0.1/ntdgotv_langtools/__init__.py
--rw-rw-rw-   0        0        0       58 2024-05-17 18:05:24.000000 ntdgotv_langtools-0.1/ntdgotv_langtools/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:22:53.207666 ntdgotv_langtools-0.1/ntdgotv_langtools.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-17 18:22:53.000000 ntdgotv_langtools-0.1/ntdgotv_langtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-17 18:22:53.000000 ntdgotv_langtools-0.1/ntdgotv_langtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:22:53.000000 ntdgotv_langtools-0.1/ntdgotv_langtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-17 18:22:53.000000 ntdgotv_langtools-0.1/ntdgotv_langtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 18:22:53.211194 ntdgotv_langtools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      140 2024-05-17 18:08:01.000000 ntdgotv_langtools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:47:28.997179 ntdgotv_langtools-0.1.1/
+-rw-rw-rw-   0        0        0      194 2024-05-17 19:47:28.995187 ntdgotv_langtools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-05-17 17:44:40.000000 ntdgotv_langtools-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 19:47:28.969253 ntdgotv_langtools-0.1.1/ntdgotv_langtools/
+-rw-rw-rw-   0        0        0       25 2024-05-17 19:38:58.000000 ntdgotv_langtools-0.1.1/ntdgotv_langtools/__init__.py
+-rw-rw-rw-   0        0        0       58 2024-05-17 19:38:58.000000 ntdgotv_langtools-0.1.1/ntdgotv_langtools/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:47:28.994189 ntdgotv_langtools-0.1.1/ntdgotv_langtools.egg-info/
+-rw-rw-rw-   0        0        0      194 2024-05-17 19:47:28.000000 ntdgotv_langtools-0.1.1/ntdgotv_langtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-17 19:47:28.000000 ntdgotv_langtools-0.1.1/ntdgotv_langtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 19:47:28.000000 ntdgotv_langtools-0.1.1/ntdgotv_langtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-17 19:47:28.000000 ntdgotv_langtools-0.1.1/ntdgotv_langtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 19:47:28.997179 ntdgotv_langtools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      294 2024-05-17 19:46:44.000000 ntdgotv_langtools-0.1.1/setup.py
```


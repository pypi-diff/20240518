# Comparing `tmp/nomadnet-0.4.8.tar.gz` & `tmp/nomadnet-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomadnet-0.4.8.tar", last modified: Sun Mar  3 23:33:55 2024, max compression
+gzip compressed data, was "nomadnet-0.4.9.tar", last modified: Sat May 18 17:15:07 2024, max compression
```

## Comparing `nomadnet-0.4.8.tar` & `nomadnet-0.4.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.259896 nomadnet-0.4.8/
--rwxrwxr-x   0 markqvist  (1000) markqvist  (1000)       77 2021-05-04 09:07:03.000000 nomadnet-0.4.8/.dockerignore
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.253229 nomadnet-0.4.8/.github/
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.253229 nomadnet-0.4.8/.github/workflows/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1130 2022-05-17 11:11:15.000000 nomadnet-0.4.8/.github/workflows/publish-container.yml
--rwxrwxr-x   0 markqvist  (1000) markqvist  (1000)       77 2021-05-04 09:07:03.000000 nomadnet-0.4.8/.gitignore
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      735 2024-02-16 16:48:53.000000 nomadnet-0.4.8/Dockerfile
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    35149 2021-07-06 07:21:04.000000 nomadnet-0.4.8/LICENSE
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      410 2021-12-01 18:35:41.000000 nomadnet-0.4.8/Makefile
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10714 2024-03-03 23:33:55.259896 nomadnet-0.4.8/PKG-INFO
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    10192 2024-02-16 16:53:34.000000 nomadnet-0.4.8/README.md
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.253229 nomadnet-0.4.8/docs/
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.256563 nomadnet-0.4.8/docs/screenshots/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    80551 2021-09-18 13:03:03.000000 nomadnet-0.4.8/docs/screenshots/1.png
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    83305 2021-09-18 12:28:55.000000 nomadnet-0.4.8/docs/screenshots/2.png
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    87591 2021-09-18 12:37:05.000000 nomadnet-0.4.8/docs/screenshots/3.png
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    86223 2021-09-18 12:45:47.000000 nomadnet-0.4.8/docs/screenshots/4.png
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    70156 2021-09-18 12:45:33.000000 nomadnet-0.4.8/docs/screenshots/5.png
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.256563 nomadnet-0.4.8/nomadnet/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    15306 2023-11-02 11:25:04.000000 nomadnet-0.4.8/nomadnet/Conversation.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    15147 2024-03-02 07:56:42.000000 nomadnet-0.4.8/nomadnet/Directory.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    11044 2024-01-07 22:29:59.000000 nomadnet-0.4.8/nomadnet/Node.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49442 2024-03-01 23:03:26.000000 nomadnet-0.4.8/nomadnet/NomadNetworkApp.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      357 2021-08-26 14:39:59.000000 nomadnet-0.4.8/nomadnet/__init__.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       22 2024-03-03 23:31:10.000000 nomadnet-0.4.8/nomadnet/_version.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.253229 nomadnet-0.4.8/nomadnet/examples/
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.256563 nomadnet-0.4.8/nomadnet/examples/messageboard/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1790 2023-02-04 15:26:07.000000 nomadnet-0.4.8/nomadnet/examples/messageboard/README.md
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1185 2023-02-04 15:06:30.000000 nomadnet-0.4.8/nomadnet/examples/messageboard/messageboard.mu
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6741 2023-02-04 15:06:30.000000 nomadnet-0.4.8/nomadnet/examples/messageboard/messageboard.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1881 2022-05-18 14:26:01.000000 nomadnet-0.4.8/nomadnet/nomadnet.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.256563 nomadnet-0.4.8/nomadnet/ui/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      159 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/ui/GraphicalUI.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      177 2022-05-17 10:05:15.000000 nomadnet-0.4.8/nomadnet/ui/MenuUI.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      536 2022-05-18 14:32:40.000000 nomadnet-0.4.8/nomadnet/ui/NoneUI.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    14325 2023-09-19 10:18:15.000000 nomadnet-0.4.8/nomadnet/ui/TextUI.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      147 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/ui/WebUI.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1246 2022-05-17 10:35:35.000000 nomadnet-0.4.8/nomadnet/ui/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.259896 nomadnet-0.4.8/nomadnet/ui/textui/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45564 2024-02-29 17:41:14.000000 nomadnet-0.4.8/nomadnet/ui/textui/Browser.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3021 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Config.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    54622 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Conversations.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      599 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Directory.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      607 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Extras.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49942 2024-03-01 23:10:45.000000 nomadnet-0.4.8/nomadnet/ui/textui/Guide.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1419 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Log.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8165 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Main.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      569 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Map.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    29250 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/MicronParser.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    70424 2024-01-18 14:38:48.000000 nomadnet-0.4.8/nomadnet/ui/textui/Network.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      166 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/ui/textui/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.259896 nomadnet-0.4.8/nomadnet/vendor/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    18373 2024-01-15 17:40:53.000000 nomadnet-0.4.8/nomadnet/vendor/Scrollable.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      166 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.259896 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1063 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/LICENSE
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      358 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.259896 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/assisting_modules/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       48 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/assisting_modules/__init__.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      706 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/assisting_modules/modifier_key.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1716 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/assisting_modules/useful_functions.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.259896 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       48 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/__init__.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    19363 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/date_picker.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    21741 2024-01-18 14:46:18.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/indicative_listbox.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    12935 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/integer_picker.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1699 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/message_dialog.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1667 2021-05-27 08:44:54.000000 nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/selectable_row.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    89634 2021-10-17 17:06:56.000000 nomadnet-0.4.8/nomadnet/vendor/configobj.py
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      500 2023-02-04 15:36:58.000000 nomadnet-0.4.8/nomadnet/vendor/quotes.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-03 23:33:55.259896 nomadnet-0.4.8/nomadnet.egg-info/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10714 2024-03-03 23:33:55.000000 nomadnet-0.4.8/nomadnet.egg-info/PKG-INFO
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     2044 2024-03-03 23:33:55.000000 nomadnet-0.4.8/nomadnet.egg-info/SOURCES.txt
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)        1 2024-03-03 23:33:55.000000 nomadnet-0.4.8/nomadnet.egg-info/dependency_links.txt
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       52 2024-03-03 23:33:55.000000 nomadnet-0.4.8/nomadnet.egg-info/entry_points.txt
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       51 2024-03-03 23:33:55.000000 nomadnet-0.4.8/nomadnet.egg-info/requires.txt
--rw-rw-r--   0 markqvist  (1000) markqvist  (1000)        9 2024-03-03 23:33:55.000000 nomadnet-0.4.8/nomadnet.egg-info/top_level.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2024-03-03 23:33:55.259896 nomadnet-0.4.8/setup.cfg
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      949 2024-03-03 23:31:37.000000 nomadnet-0.4.8/setup.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.492314 nomadnet-0.4.9/
+-rwxrwxr-x   0 markqvist  (1000) markqvist  (1000)       77 2021-05-04 09:07:03.000000 nomadnet-0.4.9/.dockerignore
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.485647 nomadnet-0.4.9/.github/
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.488980 nomadnet-0.4.9/.github/workflows/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1130 2022-05-17 11:11:15.000000 nomadnet-0.4.9/.github/workflows/publish-container.yml
+-rwxrwxr-x   0 markqvist  (1000) markqvist  (1000)       77 2021-05-04 09:07:03.000000 nomadnet-0.4.9/.gitignore
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      735 2024-02-16 16:48:53.000000 nomadnet-0.4.9/Dockerfile
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    35149 2021-07-06 07:21:04.000000 nomadnet-0.4.9/LICENSE
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      410 2021-12-01 18:35:41.000000 nomadnet-0.4.9/Makefile
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10706 2024-05-18 17:15:07.492314 nomadnet-0.4.9/PKG-INFO
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    10192 2024-02-16 16:53:34.000000 nomadnet-0.4.9/README.md
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.485647 nomadnet-0.4.9/docs/
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.488980 nomadnet-0.4.9/docs/screenshots/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    80551 2021-09-18 13:03:03.000000 nomadnet-0.4.9/docs/screenshots/1.png
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    83305 2021-09-18 12:28:55.000000 nomadnet-0.4.9/docs/screenshots/2.png
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    87591 2021-09-18 12:37:05.000000 nomadnet-0.4.9/docs/screenshots/3.png
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    86223 2021-09-18 12:45:47.000000 nomadnet-0.4.9/docs/screenshots/4.png
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    70156 2021-09-18 12:45:33.000000 nomadnet-0.4.9/docs/screenshots/5.png
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.488980 nomadnet-0.4.9/nomadnet/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    15306 2023-11-02 11:25:04.000000 nomadnet-0.4.9/nomadnet/Conversation.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    15147 2024-03-02 07:56:42.000000 nomadnet-0.4.9/nomadnet/Directory.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    11044 2024-01-07 22:29:59.000000 nomadnet-0.4.9/nomadnet/Node.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49442 2024-03-01 23:03:26.000000 nomadnet-0.4.9/nomadnet/NomadNetworkApp.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      357 2021-08-26 14:39:59.000000 nomadnet-0.4.9/nomadnet/__init__.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       22 2024-05-05 18:12:50.000000 nomadnet-0.4.9/nomadnet/_version.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.485647 nomadnet-0.4.9/nomadnet/examples/
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.488980 nomadnet-0.4.9/nomadnet/examples/messageboard/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1790 2023-02-04 15:26:07.000000 nomadnet-0.4.9/nomadnet/examples/messageboard/README.md
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1185 2023-02-04 15:06:30.000000 nomadnet-0.4.9/nomadnet/examples/messageboard/messageboard.mu
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6741 2023-02-04 15:06:30.000000 nomadnet-0.4.9/nomadnet/examples/messageboard/messageboard.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1881 2022-05-18 14:26:01.000000 nomadnet-0.4.9/nomadnet/nomadnet.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.488980 nomadnet-0.4.9/nomadnet/ui/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      159 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/ui/GraphicalUI.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      177 2022-05-17 10:05:15.000000 nomadnet-0.4.9/nomadnet/ui/MenuUI.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      536 2022-05-18 14:32:40.000000 nomadnet-0.4.9/nomadnet/ui/NoneUI.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    14344 2024-05-18 12:54:15.000000 nomadnet-0.4.9/nomadnet/ui/TextUI.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      147 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/ui/WebUI.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1246 2022-05-17 10:35:35.000000 nomadnet-0.4.9/nomadnet/ui/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.492314 nomadnet-0.4.9/nomadnet/ui/textui/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45564 2024-02-29 17:41:14.000000 nomadnet-0.4.9/nomadnet/ui/textui/Browser.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3021 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Config.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    54622 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Conversations.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      599 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Directory.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      607 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Extras.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49955 2024-05-18 12:45:31.000000 nomadnet-0.4.9/nomadnet/ui/textui/Guide.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1419 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Log.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8165 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Main.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      569 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Map.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    29250 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/MicronParser.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    70424 2024-01-18 14:38:48.000000 nomadnet-0.4.9/nomadnet/ui/textui/Network.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      166 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/ui/textui/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.492314 nomadnet-0.4.9/nomadnet/vendor/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    18373 2024-01-15 17:40:53.000000 nomadnet-0.4.9/nomadnet/vendor/Scrollable.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      166 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.492314 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1063 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/LICENSE
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      358 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.492314 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/assisting_modules/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       48 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/assisting_modules/__init__.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      706 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/assisting_modules/modifier_key.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1716 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/assisting_modules/useful_functions.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.492314 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       48 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/__init__.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    19363 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/date_picker.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    21741 2024-01-18 14:46:18.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/indicative_listbox.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    12935 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/integer_picker.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1699 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/message_dialog.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     1667 2021-05-27 08:44:54.000000 nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/selectable_row.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)    89634 2021-10-17 17:06:56.000000 nomadnet-0.4.9/nomadnet/vendor/configobj.py
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)      500 2023-02-04 15:36:58.000000 nomadnet-0.4.9/nomadnet/vendor/quotes.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-18 17:15:07.492314 nomadnet-0.4.9/nomadnet.egg-info/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10706 2024-05-18 17:15:07.000000 nomadnet-0.4.9/nomadnet.egg-info/PKG-INFO
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)     2044 2024-05-18 17:15:07.000000 nomadnet-0.4.9/nomadnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)        1 2024-05-18 17:15:07.000000 nomadnet-0.4.9/nomadnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       52 2024-05-18 17:15:07.000000 nomadnet-0.4.9/nomadnet.egg-info/entry_points.txt
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)       43 2024-05-18 17:15:07.000000 nomadnet-0.4.9/nomadnet.egg-info/requires.txt
+-rw-rw-r--   0 markqvist  (1000) markqvist  (1000)        9 2024-05-18 17:15:07.000000 nomadnet-0.4.9/nomadnet.egg-info/top_level.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2024-05-18 17:15:07.492314 nomadnet-0.4.9/setup.cfg
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      941 2024-05-18 13:15:12.000000 nomadnet-0.4.9/setup.py
```

### Comparing `nomadnet-0.4.8/.github/workflows/publish-container.yml` & `nomadnet-0.4.9/.github/workflows/publish-container.yml`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/Dockerfile` & `nomadnet-0.4.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/LICENSE` & `nomadnet-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/PKG-INFO` & `nomadnet-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nomadnet
-Version: 0.4.8
+Version: 0.4.9
 Summary: Communicate Freely
 Home-page: https://github.com/markqvist/nomadnet
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: rns>=0.7.2
-Requires-Dist: lxmf>=0.4.1
-Requires-Dist: urwid!=2.4.3,>=2.4.2
+Requires-Dist: rns>=0.7.5
+Requires-Dist: lxmf>=0.4.3
+Requires-Dist: urwid>=2.4.4
 Requires-Dist: qrcode
 
 # Nomad Network - Communicate Freely
 
 Off-grid, resilient mesh communication with strong encryption, forward secrecy and extreme privacy.
 
 ![Screenshot](https://github.com/markqvist/NomadNet/raw/master/docs/screenshots/1.png)
```

### Comparing `nomadnet-0.4.8/README.md` & `nomadnet-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/docs/screenshots/1.png` & `nomadnet-0.4.9/docs/screenshots/1.png`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/docs/screenshots/2.png` & `nomadnet-0.4.9/docs/screenshots/2.png`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/docs/screenshots/3.png` & `nomadnet-0.4.9/docs/screenshots/3.png`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/docs/screenshots/4.png` & `nomadnet-0.4.9/docs/screenshots/4.png`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/docs/screenshots/5.png` & `nomadnet-0.4.9/docs/screenshots/5.png`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/Conversation.py` & `nomadnet-0.4.9/nomadnet/Conversation.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/Directory.py` & `nomadnet-0.4.9/nomadnet/Directory.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/Node.py` & `nomadnet-0.4.9/nomadnet/Node.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/NomadNetworkApp.py` & `nomadnet-0.4.9/nomadnet/NomadNetworkApp.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/examples/messageboard/README.md` & `nomadnet-0.4.9/nomadnet/examples/messageboard/README.md`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/examples/messageboard/messageboard.mu` & `nomadnet-0.4.9/nomadnet/examples/messageboard/messageboard.mu`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/examples/messageboard/messageboard.py` & `nomadnet-0.4.9/nomadnet/examples/messageboard/messageboard.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/nomadnet.py` & `nomadnet-0.4.9/nomadnet/nomadnet.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/NoneUI.py` & `nomadnet-0.4.9/nomadnet/ui/NoneUI.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/TextUI.py` & `nomadnet-0.4.9/nomadnet/ui/TextUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,43 +93,43 @@
 GLYPHSETS = {
     "plain": 1,
     "unicode": 2,
     "nerdfont": 3
 }
 
 if platform.system() == "Darwin":
-    urm_char = " \uf0e0 "
+    urm_char = " \uf0e0"
     ur_char = "\uf0e0 "
 else:
-    urm_char = " \uf003 "
+    urm_char = " \uf003"
     ur_char = "\uf003 "
 
 GLYPHS = {
     # Glyph name        # Plain      # Unicode      # Nerd Font
     ("check",           "=",         "\u2713",      "\u2713"),
     ("cross",           "X",         "\u2715",      "\u2715"),
     ("unknown",         "?",         "?",           "?"),
     ("encrypted",       "",          "\u26BF",      "\uf023"),
     ("plaintext",       "!",         "!",           "\uf06e "),
     ("arrow_r",         "->",        "\u2192",      "\u2192"),
     ("arrow_l",         "<-",        "\u2190",      "\u2190"),
     ("arrow_u",         "/\\",       "\u2191",      "\u2191"),
     ("arrow_d",         "\\/",       "\u2193",      "\u2193"),
     ("warning",         "!",         "\u26a0",      "\uf12a"),
-    ("info",            "i",         "\u2139",      "\ufb4d"),
+    ("info",            "i",         "\u2139",      "\U000f064e"),
     ("unread",          "[!]",       "\u2709",      ur_char),
     ("divider1",        "-",         "\u2504",      "\u2504"),
     ("peer",            "[P]",       "\u24c5 ",     "\uf415"),
-    ("node",            "[N]",       "\u24c3 ",     "\uf502"),
+    ("node",            "[N]",       "\u24c3 ",     "\U000f0002"),
     ("page",            "",          "\u25a4 ",     "\uf719 "),
-    ("speed",           "",          "\u25F7 ",     "\uf9c4"),
-    ("decoration_menu", " +",        " +",          " \uf93a"),
+    ("speed",           "",          "\u25F7 ",     "\U000f04c5 "),
+    ("decoration_menu", " +",        " +",          " \U000f043b"),
     ("unread_menu",     " !",        " \u2709",     urm_char),
     ("globe",           "",          "",            "\uf484"),
-    ("sent",            "/\\",       "\u2191",      "\ufbf4"),
+    ("sent",            "/\\",       "\u2191",      "\U000f0cd8"),
     ("papermsg",        "P",         "\u25a4",      "\uf719"),
     ("qrcode",          "QR",        "\u25a4",      "\uf029"),
 }
 
 class TextUI:
 
     def __init__(self):
```

### Comparing `nomadnet-0.4.8/nomadnet/ui/__init__.py` & `nomadnet-0.4.9/nomadnet/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Browser.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Browser.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Config.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Config.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Conversations.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Conversations.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Directory.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Directory.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Extras.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Extras.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Guide.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Guide.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,15 +779,15 @@
 `B001 `B002 `B003 `B004 `B005 `B006 `B007 `B008 `B009 `B00a `B00b `B00c `B00d `B00e `B00f`b
 
 The following line should contain a grayscale gradient bar:
 `Bg06 `Bg13 `Bg20 `Bg26 `Bg33 `Bg40 `Bg46 `Bg53 `Bg59 `Bg66 `Bg73 `Bg79 `Bg86 `Bg92 `Bg99`b
 
 Unicode Glyphs   : \u2713  \u2715  \u26a0  \u24c3  \u2193
 
-Nerd Font Glyphs : \uf484  \uf9c4 \uf719  \uf502  \uf415  \uf023  \uf06e
+Nerd Font Glyphs : \uf484  \U000f04c5  \U000f0219  \U000f0002  \uf415  \uf023  \uf06e
 '''
 
 
 TOPIC_LICENSES = '''>Thanks, Acknowledgements and Licenses
 
 This program uses various other software components, without which Nomad Network would not have been possible. Sincere thanks to the authors and contributors of the following projects
```

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Log.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Log.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Main.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Main.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Map.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Map.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/MicronParser.py` & `nomadnet-0.4.9/nomadnet/ui/textui/MicronParser.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/ui/textui/Network.py` & `nomadnet-0.4.9/nomadnet/ui/textui/Network.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/Scrollable.py` & `nomadnet-0.4.9/nomadnet/vendor/Scrollable.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/LICENSE` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/LICENSE`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/assisting_modules/modifier_key.py` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/assisting_modules/modifier_key.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/assisting_modules/useful_functions.py` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/assisting_modules/useful_functions.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/date_picker.py` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/date_picker.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/indicative_listbox.py` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/indicative_listbox.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/integer_picker.py` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/integer_picker.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/message_dialog.py` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/message_dialog.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/additional_urwid_widgets/widgets/selectable_row.py` & `nomadnet-0.4.9/nomadnet/vendor/additional_urwid_widgets/widgets/selectable_row.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet/vendor/configobj.py` & `nomadnet-0.4.9/nomadnet/vendor/configobj.py`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/nomadnet.egg-info/PKG-INFO` & `nomadnet-0.4.9/nomadnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nomadnet
-Version: 0.4.8
+Version: 0.4.9
 Summary: Communicate Freely
 Home-page: https://github.com/markqvist/nomadnet
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: rns>=0.7.2
-Requires-Dist: lxmf>=0.4.1
-Requires-Dist: urwid!=2.4.3,>=2.4.2
+Requires-Dist: rns>=0.7.5
+Requires-Dist: lxmf>=0.4.3
+Requires-Dist: urwid>=2.4.4
 Requires-Dist: qrcode
 
 # Nomad Network - Communicate Freely
 
 Off-grid, resilient mesh communication with strong encryption, forward secrecy and extreme privacy.
 
 ![Screenshot](https://github.com/markqvist/NomadNet/raw/master/docs/screenshots/1.png)
```

### Comparing `nomadnet-0.4.8/nomadnet.egg-info/SOURCES.txt` & `nomadnet-0.4.9/nomadnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomadnet-0.4.8/setup.py` & `nomadnet-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,10 +26,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points= {
         'console_scripts': ['nomadnet=nomadnet.nomadnet:main']
     },
-    install_requires=["rns>=0.7.2", "lxmf>=0.4.1", "urwid>=2.4.2,!=2.4.3", "qrcode"],
+    install_requires=["rns>=0.7.5", "lxmf>=0.4.3", "urwid>=2.4.4", "qrcode"],
     python_requires=">=3.6",
 )
```


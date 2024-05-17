# Comparing `tmp/WPyrogram-2.0.142.tar.gz` & `tmp/wpyrogram-2.0.143.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPyrogram-2.0.142.tar", last modified: Thu Mar 28 17:32:35 2024, max compression
+gzip compressed data, was "wpyrogram-2.0.143.tar", last modified: Fri May 17 22:14:10 2024, max compression
```

## Comparing `WPyrogram-2.0.142.tar` & `wpyrogram-2.0.143.tar`

### file list

```diff
@@ -1,609 +1,609 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.806670 WPyrogram-2.0.142/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-28 17:32:35.806670 WPyrogram-2.0.142/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.806670 WPyrogram-2.0.142/WPyrogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-28 17:32:35.000000 WPyrogram-2.0.142/WPyrogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23901 2024-03-28 17:32:35.000000 WPyrogram-2.0.142/WPyrogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:32:35.000000 WPyrogram-2.0.142/WPyrogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:32:35.000000 WPyrogram-2.0.142/WPyrogram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 17:32:35.000000 WPyrogram-2.0.142/WPyrogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 17:32:35.000000 WPyrogram-2.0.142/WPyrogram.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.714670 WPyrogram-2.0.142/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.714670 WPyrogram-2.0.142/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22485 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.714670 WPyrogram-2.0.142/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (127)   198251 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.718670 WPyrogram-2.0.142/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.718670 WPyrogram-2.0.142/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22165 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.718670 WPyrogram-2.0.142/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.718670 WPyrogram-2.0.142/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.718670 WPyrogram-2.0.142/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    24066 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.718670 WPyrogram-2.0.142/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.722670 WPyrogram-2.0.142/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.722670 WPyrogram-2.0.142/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.722670 WPyrogram-2.0.142/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.722670 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.722670 WPyrogram-2.0.142/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    14813 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)   208021 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.726670 WPyrogram-2.0.142/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/business_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/folder_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/profile_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/reply_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/stories_privacy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.726670 WPyrogram-2.0.142/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    26811 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.730670 WPyrogram-2.0.142/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/conversation_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/story_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.730670 WPyrogram-2.0.142/pyrogram/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.730670 WPyrogram-2.0.142/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.730670 WPyrogram-2.0.142/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.734670 WPyrogram-2.0.142/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.738670 WPyrogram-2.0.142/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.746670 WPyrogram-2.0.142/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/delete_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/export_folder_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/get_similar_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/join_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/leave_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_ttl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/toggle_folder_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/toggle_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/toggle_join_to_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/update_chat_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/update_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/chats/update_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.746670 WPyrogram-2.0.142/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.750670 WPyrogram-2.0.142/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_story.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.754670 WPyrogram-2.0.142/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.762670 WPyrogram-2.0.142/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_message_by_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_scheduled_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/get_stickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/read_mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/read_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13142 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    22322 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/send_web_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/start_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/wait_for_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/messages/wait_for_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.762670 WPyrogram-2.0.142/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.762670 WPyrogram-2.0.142/pyrogram/methods/premium/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/premium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/premium/apply_boost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/premium/get_boosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/premium/get_boosts_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.766670 WPyrogram-2.0.142/pyrogram/methods/stories/
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/can_send_story.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/copy_story.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/delete_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/edit_story_caption.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/edit_story_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/edit_story_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/export_story_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/forward_story.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/get_all_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/get_chat_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/get_pinned_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/get_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/get_stories_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/hide_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/increment_story_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/pin_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/read_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)    13967 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/stories/send_story.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.770670 WPyrogram-2.0.142/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/check_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/update_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/users/update_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.770670 WPyrogram-2.0.142/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    61915 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.770670 WPyrogram-2.0.142/pyrogram/nav/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/nav/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.774670 WPyrogram-2.0.142/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.774670 WPyrogram-2.0.142/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.774670 WPyrogram-2.0.142/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.774670 WPyrogram-2.0.142/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.774670 WPyrogram-2.0.142/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.778670 WPyrogram-2.0.142/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.778670 WPyrogram-2.0.142/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.778670 WPyrogram-2.0.142/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.778670 WPyrogram-2.0.142/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.782670 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13343 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_channel_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_chat_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_poll_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/requested_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.786670 WPyrogram-2.0.142/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.790670 WPyrogram-2.0.142/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.790670 WPyrogram-2.0.142/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_message_content/input_reply_to_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_message_content/input_reply_to_story.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.798669 WPyrogram-2.0.142/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/boosts_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/giveaway_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (127)   186030 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_story.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/my_boost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)    72101 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/user_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/pyromod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.802670 WPyrogram-2.0.142/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_recipients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_weekly_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_working_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    40588 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    22160 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:32:35.806670 WPyrogram-2.0.142/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.802670 WPyrogram-2.0.142/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.802670 WPyrogram-2.0.142/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:32:35.806670 WPyrogram-2.0.142/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/tests/parser/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-03-28 17:32:08.000000 WPyrogram-2.0.142/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/WPyrogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-17 22:14:10.000000 wpyrogram-2.0.143/WPyrogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23901 2024-05-17 22:14:10.000000 wpyrogram-2.0.143/WPyrogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:14:10.000000 wpyrogram-2.0.143/WPyrogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:14:10.000000 wpyrogram-2.0.143/WPyrogram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 22:14:10.000000 wpyrogram-2.0.143/WPyrogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 22:14:10.000000 wpyrogram-2.0.143/WPyrogram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.900670 wpyrogram-2.0.143/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.900670 wpyrogram-2.0.143/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22485 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.900670 wpyrogram-2.0.143/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (127)   198251 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.900670 wpyrogram-2.0.143/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.900670 wpyrogram-2.0.143/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22165 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.900670 wpyrogram-2.0.143/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.904670 wpyrogram-2.0.143/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.904670 wpyrogram-2.0.143/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    24066 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.904670 wpyrogram-2.0.143/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.904670 wpyrogram-2.0.143/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.908670 wpyrogram-2.0.143/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.908670 wpyrogram-2.0.143/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.908670 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.908670 wpyrogram-2.0.143/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14813 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)   208021 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.912670 wpyrogram-2.0.143/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/business_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/folder_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/profile_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/reply_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/stories_privacy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.912670 wpyrogram-2.0.143/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26811 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.916670 wpyrogram-2.0.143/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/conversation_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/story_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.916670 wpyrogram-2.0.143/pyrogram/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.916670 wpyrogram-2.0.143/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.916670 wpyrogram-2.0.143/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.920670 wpyrogram-2.0.143/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.920670 wpyrogram-2.0.143/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.932670 wpyrogram-2.0.143/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/delete_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/export_folder_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/get_similar_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/join_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/leave_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/toggle_folder_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/toggle_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/toggle_join_to_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/update_chat_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/update_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/chats/update_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.932670 wpyrogram-2.0.143/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.936670 wpyrogram-2.0.143/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.936670 wpyrogram-2.0.143/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.948670 wpyrogram-2.0.143/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_message_by_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_scheduled_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/get_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/read_mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/read_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13142 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22322 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/send_web_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/start_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/wait_for_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/messages/wait_for_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.948670 wpyrogram-2.0.143/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.948670 wpyrogram-2.0.143/pyrogram/methods/premium/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/premium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/premium/apply_boost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/premium/get_boosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/premium/get_boosts_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.952670 wpyrogram-2.0.143/pyrogram/methods/stories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/can_send_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/copy_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/delete_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/edit_story_caption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/edit_story_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/edit_story_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/export_story_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/forward_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/get_all_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/get_chat_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/get_pinned_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/get_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/get_stories_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/hide_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/increment_story_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/pin_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/read_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13967 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/stories/send_story.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.956670 wpyrogram-2.0.143/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/check_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/users/update_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.956670 wpyrogram-2.0.143/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61915 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.956670 wpyrogram-2.0.143/pyrogram/nav/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/nav/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.960670 wpyrogram-2.0.143/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.960670 wpyrogram-2.0.143/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.960670 wpyrogram-2.0.143/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.960670 wpyrogram-2.0.143/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.964670 wpyrogram-2.0.143/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.964670 wpyrogram-2.0.143/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.964670 wpyrogram-2.0.143/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.964670 wpyrogram-2.0.143/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.964670 wpyrogram-2.0.143/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.972670 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13343 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_channel_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_chat_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_poll_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/requested_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.976670 wpyrogram-2.0.143/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.976670 wpyrogram-2.0.143/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.976670 wpyrogram-2.0.143/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_message_content/input_reply_to_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_message_content/input_reply_to_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.984670 wpyrogram-2.0.143/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/boosts_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/giveaway_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)   186030 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/my_boost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72101 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/user_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/pyromod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_recipients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_weekly_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_working_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40588 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22160 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:14:10.992670 wpyrogram-2.0.143/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/tests/parser/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-17 22:13:46.000000 wpyrogram-2.0.143/tests/test_file_id.py
```

### Comparing `WPyrogram-2.0.142/COPYING` & `wpyrogram-2.0.143/COPYING`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/COPYING.lesser` & `wpyrogram-2.0.143/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/NOTICE` & `wpyrogram-2.0.143/NOTICE`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/PKG-INFO` & `wpyrogram-2.0.143/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPyrogram
-Version: 2.0.142
+Version: 2.0.143
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots - Woto's experimental fork
 Home-page: https://github.com/ALiwoto/WPyrogram
 Download-URL: https://github.com/ALiwoto/WPyrogram
 Author: Dan
 Author-email: dan@pyrogram.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/ALiwoto/WPyrogram/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WPyrogram Version: 2.0.142 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: WPyrogram Version: 2.0.143 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots -
 Woto's experimental fork Home-page: https://github.com/ALiwoto/WPyrogram
 Download-URL: https://github.com/ALiwoto/WPyrogram Author: Dan Author-email:
 dan@pyrogram.org License: LGPLv3 Project-URL: Tracker, https://github.com/
 ALiwoto/WPyrogram/issues Project-URL: Community, https://t.me/Pyrogram Project-
 URL: Source, https://github.com/ALiwoto/WPyrogram Project-URL: Documentation,
 https://docs.pyrogram.org Keywords: telegram chat messenger mtproto api client
```

### Comparing `WPyrogram-2.0.142/README.md` & `wpyrogram-2.0.143/README.md`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/WPyrogram.egg-info/PKG-INFO` & `wpyrogram-2.0.143/WPyrogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPyrogram
-Version: 2.0.142
+Version: 2.0.143
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots - Woto's experimental fork
 Home-page: https://github.com/ALiwoto/WPyrogram
 Download-URL: https://github.com/ALiwoto/WPyrogram
 Author: Dan
 Author-email: dan@pyrogram.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/ALiwoto/WPyrogram/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WPyrogram Version: 2.0.142 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: WPyrogram Version: 2.0.143 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots -
 Woto's experimental fork Home-page: https://github.com/ALiwoto/WPyrogram
 Download-URL: https://github.com/ALiwoto/WPyrogram Author: Dan Author-email:
 dan@pyrogram.org License: LGPLv3 Project-URL: Tracker, https://github.com/
 ALiwoto/WPyrogram/issues Project-URL: Community, https://t.me/Pyrogram Project-
 URL: Source, https://github.com/ALiwoto/WPyrogram Project-URL: Documentation,
 https://docs.pyrogram.org Keywords: telegram chat messenger mtproto api client
```

### Comparing `WPyrogram-2.0.142/WPyrogram.egg-info/SOURCES.txt` & `wpyrogram-2.0.143/WPyrogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/__init__.py` & `wpyrogram-2.0.143/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/api/__init__.py` & `wpyrogram-2.0.143/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/api/compiler.py` & `wpyrogram-2.0.143/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/api/source/auth_key.tl` & `wpyrogram-2.0.143/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/api/source/main_api.tl` & `wpyrogram-2.0.143/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/api/source/sys_msgs.tl` & `wpyrogram-2.0.143/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/api/template/combinator.txt` & `wpyrogram-2.0.143/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/api/template/type.txt` & `wpyrogram-2.0.143/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/docs/__init__.py` & `wpyrogram-2.0.143/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/docs/compiler.py` & `wpyrogram-2.0.143/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/__init__.py` & `wpyrogram-2.0.143/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/compiler.py` & `wpyrogram-2.0.143/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/sort.py` & `wpyrogram-2.0.143/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/source/400_BAD_REQUEST.tsv` & `wpyrogram-2.0.143/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/source/401_UNAUTHORIZED.tsv` & `wpyrogram-2.0.143/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/source/403_FORBIDDEN.tsv` & `wpyrogram-2.0.143/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `wpyrogram-2.0.143/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/source/420_FLOOD.tsv` & `wpyrogram-2.0.143/compiler/errors/source/420_FLOOD.tsv`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `wpyrogram-2.0.143/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/__init__.py` & `wpyrogram-2.0.143/pyrogram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "2.0.142"
+__version__ = "2.0.143"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `WPyrogram-2.0.142/pyrogram/client.py` & `wpyrogram-2.0.143/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/__init__.py` & `wpyrogram-2.0.143/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/connection.py` & `wpyrogram-2.0.143/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/__init__.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/tcp/__init__.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_abridged.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_full.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `wpyrogram-2.0.143/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/crypto/__init__.py` & `wpyrogram-2.0.143/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/crypto/aes.py` & `wpyrogram-2.0.143/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/crypto/mtproto.py` & `wpyrogram-2.0.143/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/crypto/prime.py` & `wpyrogram-2.0.143/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/crypto/rsa.py` & `wpyrogram-2.0.143/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/dispatcher.py` & `wpyrogram-2.0.143/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/emoji.py` & `wpyrogram-2.0.143/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/__init__.py` & `wpyrogram-2.0.143/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/auto_name.py` & `wpyrogram-2.0.143/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/business_schedule.py` & `wpyrogram-2.0.143/pyrogram/enums/business_schedule.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/chat_action.py` & `wpyrogram-2.0.143/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/chat_event_action.py` & `wpyrogram-2.0.143/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/chat_member_status.py` & `wpyrogram-2.0.143/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/chat_members_filter.py` & `wpyrogram-2.0.143/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/chat_type.py` & `wpyrogram-2.0.143/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/folder_color.py` & `wpyrogram-2.0.143/pyrogram/enums/folder_color.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/message_entity_type.py` & `wpyrogram-2.0.143/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/message_media_type.py` & `wpyrogram-2.0.143/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/message_service_type.py` & `wpyrogram-2.0.143/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/messages_filter.py` & `wpyrogram-2.0.143/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/next_code_type.py` & `wpyrogram-2.0.143/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/parse_mode.py` & `wpyrogram-2.0.143/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/poll_type.py` & `wpyrogram-2.0.143/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/profile_color.py` & `wpyrogram-2.0.143/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/reply_color.py` & `wpyrogram-2.0.143/pyrogram/enums/reply_color.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/sent_code_type.py` & `wpyrogram-2.0.143/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/stories_privacy_rules.py` & `wpyrogram-2.0.143/pyrogram/enums/stories_privacy_rules.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/enums/user_status.py` & `wpyrogram-2.0.143/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/errors/__init__.py` & `wpyrogram-2.0.143/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/errors/rpc_error.py` & `wpyrogram-2.0.143/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/file_id.py` & `wpyrogram-2.0.143/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/filters.py` & `wpyrogram-2.0.143/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/__init__.py` & `wpyrogram-2.0.143/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/callback_query_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/chat_join_request_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/chat_member_updated_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/chosen_inline_result_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/conversation_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/deleted_messages_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/disconnect_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/edited_message_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/inline_query_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/message_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/poll_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/raw_update_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/story_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/story_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/handlers/user_status_handler.py` & `wpyrogram-2.0.143/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/helpers/__init__.py` & `wpyrogram-2.0.143/pyrogram/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/helpers/helpers.py` & `wpyrogram-2.0.143/pyrogram/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/advanced/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/advanced/invoke.py` & `wpyrogram-2.0.143/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/advanced/resolve_peer.py` & `wpyrogram-2.0.143/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/advanced/save_file.py` & `wpyrogram-2.0.143/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/accept_terms_of_service.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/check_password.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/connect.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/disconnect.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/get_password_hint.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/initialize.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/log_out.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/recover_password.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/resend_code.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/send_code.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/send_recovery_code.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/sign_in.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/sign_in_bot.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/sign_up.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/auth/terminate.py` & `wpyrogram-2.0.143/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/answer_callback_query.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/answer_inline_query.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/answer_web_app_query.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/delete_bot_commands.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/get_bot_commands.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/get_bot_default_privileges.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/get_chat_menu_button.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/get_game_high_scores.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/get_inline_bot_results.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/request_callback_answer.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/send_game.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/send_inline_bot_result.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/set_bot_commands.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/set_bot_default_privileges.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/set_chat_menu_button.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/bots/set_game_score.py` & `wpyrogram-2.0.143/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/add_chat_members.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/archive_chats.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/ban_chat_member.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/close_forum_topic.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/create_channel.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/create_forum_topic.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/create_group.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/create_supergroup.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/delete_channel.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/delete_chat_photo.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/delete_folder.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/delete_folder.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/delete_forum_topic.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/delete_supergroup.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/delete_user_history.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/edit_forum_topic.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/export_folder_link.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/export_folder_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_chat.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_event_log.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_member.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_members.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_members_count.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_chat_online_count.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_dialogs.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_dialogs_count.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_folders.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_folders.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_forum_topics.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_forum_topics_by_id.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,34 +66,39 @@
         r = await self.invoke(
             raw.functions.channels.GetForumTopicsByID(
                 channel=await self.resolve_peer(chat_id),
                 topics=ids
             )
         )
 
-        topics = types.List()
+        topics_list = []
+        parsed_messages = {}
         users = {u.id: u for u in getattr(r, "users", [])}
         chats = {c.id: c for c in getattr(r, "chats", [])}
+        topics = {t.id: t for t in getattr(r, "topics", [])}
         messages = {m.id: m for m in getattr(r, "messages", [])}
 
-        for message in messages:
+        for message in messages.values():
             if isinstance(message, raw.types.MessageEmpty):
                 continue
 
-            messages[message.id] = await types.Message._parse(
-                client=self, 
-                message=message, 
-                users=users,
-                chats=chats,
-                replies=0
-            )
+            try:
+                parsed_messages[message.id] = await types.Message._parse(
+                    client=self, 
+                    message=message, 
+                    users=users,
+                    chats=chats,
+                    replies=0,
+                    from_topic=True if len(topics_list) != 1 else topics_list[topic_ids[0]]
+                )
+            except: pass
 
-        for current in getattr(r, "topics", []):
-            topics.append(types.ForumTopic._parse(
+        for current in topics.values():
+            topics_list.append(types.ForumTopic._parse(
                 self, 
                 forum_topic=current,
-                messages=messages,
+                messages=parsed_messages,
                 users=users, 
                 chats=chats
             ))
 
         return topics if is_iterable else topics[0] if topics else None
```

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_nearby_chats.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_send_as_chats.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/get_similar_channels.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/get_similar_channels.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/join_chat.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/join_folder.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/join_folder.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/leave_chat.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/leave_folder.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/leave_folder.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/mark_chat_unread.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/pin_chat_message.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/promote_chat_member.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/restrict_chat_member.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_administrator_title.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_description.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_permissions.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_photo.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_protected_content.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_title.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_ttl.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_ttl.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_chat_username.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_send_as_chat.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/set_slow_mode.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/toggle_folder_tags.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/toggle_folder_tags.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/toggle_forum_topics.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/toggle_forum_topics.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/toggle_join_to_send.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/toggle_join_to_send.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/unarchive_chats.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/unban_chat_member.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/unpin_all_chat_messages.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/unpin_chat_message.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/update_chat_notifications.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/update_chat_notifications.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/update_color.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/update_color.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/chats/update_folder.py` & `wpyrogram-2.0.143/pyrogram/methods/chats/update_folder.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/contacts/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/contacts/add_contact.py` & `wpyrogram-2.0.143/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/contacts/delete_contacts.py` & `wpyrogram-2.0.143/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/contacts/get_contacts.py` & `wpyrogram-2.0.143/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/contacts/get_contacts_count.py` & `wpyrogram-2.0.143/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/contacts/import_contacts.py` & `wpyrogram-2.0.143/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_callback_query.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_chat_join_request.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_chat_member_updated.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_chosen_inline_result.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_deleted_messages.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_disconnect.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_edited_message.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_inline_query.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_message.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_poll.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_raw_update.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_story.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/decorators/on_user_status.py` & `wpyrogram-2.0.143/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/approve_chat_join_request.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/create_chat_invite_link.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/decline_chat_join_request.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/export_chat_invite_link.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_invite_link.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/get_chat_join_requests.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `wpyrogram-2.0.143/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/copy_media_group.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/copy_message.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/delete_messages.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/download_media.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_caption.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_media.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_reply_markup.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_inline_text.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_caption.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_media.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_reply_markup.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/edit_message_text.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/forward_messages.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_chat_history.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_chat_history_count.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_discussion_message.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_discussion_replies.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_discussion_replies_count.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_history.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_history.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_media_group.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_message_by_link.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_message_by_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_messages.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_scheduled_messages.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_scheduled_messages.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/get_stickers.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/get_stickers.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/inline_session.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/read_chat_history.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/read_mentions.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/read_mentions.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/read_reactions.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/read_reactions.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/retract_vote.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/search_global.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/search_global_count.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/search_messages.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/search_messages_count.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_animation.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_audio.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_cached_media.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_chat_action.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_contact.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_dice.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_document.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_location.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_media_group.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_message.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_photo.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_poll.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_reaction.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_sticker.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_venue.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_video.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_video_note.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_voice.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/send_web_page.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/send_web_page.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/start_bot.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/start_bot.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/stop_poll.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/stream_media.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/vote_poll.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/wait_for_callback_query.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/messages/wait_for_message.py` & `wpyrogram-2.0.143/pyrogram/methods/messages/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/password/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/password/change_cloud_password.py` & `wpyrogram-2.0.143/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/password/enable_cloud_password.py` & `wpyrogram-2.0.143/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/password/remove_cloud_password.py` & `wpyrogram-2.0.143/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/premium/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/premium/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/premium/apply_boost.py` & `wpyrogram-2.0.143/pyrogram/methods/premium/apply_boost.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/premium/get_boosts.py` & `wpyrogram-2.0.143/pyrogram/methods/premium/get_boosts.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/premium/get_boosts_status.py` & `wpyrogram-2.0.143/pyrogram/methods/premium/get_boosts_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/can_send_story.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/can_send_story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/copy_story.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/copy_story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/delete_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/delete_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/edit_story_caption.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/edit_story_caption.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/edit_story_media.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/edit_story_media.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/edit_story_privacy.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/edit_story_privacy.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/export_story_link.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/export_story_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/forward_story.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/forward_story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/get_all_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/get_all_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/get_chat_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/get_chat_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/get_pinned_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/get_pinned_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/get_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/get_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/get_stories_archive.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/get_stories_archive.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/hide_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/hide_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/increment_story_views.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/increment_story_views.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/pin_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/pin_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/read_stories.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/read_stories.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/stories/send_story.py` & `wpyrogram-2.0.143/pyrogram/methods/stories/send_story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/block_user.py` & `wpyrogram-2.0.143/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/check_username.py` & `wpyrogram-2.0.143/pyrogram/methods/users/check_username.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/delete_profile_photos.py` & `wpyrogram-2.0.143/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/get_chat_photos.py` & `wpyrogram-2.0.143/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/get_chat_photos_count.py` & `wpyrogram-2.0.143/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/get_common_chats.py` & `wpyrogram-2.0.143/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/get_default_emoji_statuses.py` & `wpyrogram-2.0.143/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/get_me.py` & `wpyrogram-2.0.143/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/get_users.py` & `wpyrogram-2.0.143/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/set_emoji_status.py` & `wpyrogram-2.0.143/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/set_profile_photo.py` & `wpyrogram-2.0.143/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/set_username.py` & `wpyrogram-2.0.143/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/unblock_user.py` & `wpyrogram-2.0.143/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/update_profile.py` & `wpyrogram-2.0.143/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/users/update_status.py` & `wpyrogram-2.0.143/pyrogram/methods/users/update_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/__init__.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/add_handler.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/compose.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/export_session_string.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/idle.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/remove_handler.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/restart.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/run.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/start.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/stop.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/methods/utilities/stop_transmission.py` & `wpyrogram-2.0.143/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/mime_types.py` & `wpyrogram-2.0.143/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/nav/__init__.py` & `wpyrogram-2.0.143/pyrogram/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/nav/pagination.py` & `wpyrogram-2.0.143/pyrogram/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/parser/__init__.py` & `wpyrogram-2.0.143/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/parser/html.py` & `wpyrogram-2.0.143/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/parser/markdown.py` & `wpyrogram-2.0.143/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/parser/parser.py` & `wpyrogram-2.0.143/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/parser/utils.py` & `wpyrogram-2.0.143/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/__init__.py` & `wpyrogram-2.0.143/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/__init__.py` & `wpyrogram-2.0.143/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/future_salt.py` & `wpyrogram-2.0.143/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/future_salts.py` & `wpyrogram-2.0.143/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/gzip_packed.py` & `wpyrogram-2.0.143/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/list.py` & `wpyrogram-2.0.143/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/message.py` & `wpyrogram-2.0.143/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/msg_container.py` & `wpyrogram-2.0.143/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/primitives/__init__.py` & `wpyrogram-2.0.143/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/primitives/bool.py` & `wpyrogram-2.0.143/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/primitives/bytes.py` & `wpyrogram-2.0.143/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/primitives/double.py` & `wpyrogram-2.0.143/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/primitives/int.py` & `wpyrogram-2.0.143/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/primitives/string.py` & `wpyrogram-2.0.143/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/primitives/vector.py` & `wpyrogram-2.0.143/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/raw/core/tl_object.py` & `wpyrogram-2.0.143/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/__init__.py` & `wpyrogram-2.0.143/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/auth.py` & `wpyrogram-2.0.143/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/internals/__init__.py` & `wpyrogram-2.0.143/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/internals/data_center.py` & `wpyrogram-2.0.143/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/internals/msg_factory.py` & `wpyrogram-2.0.143/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/internals/msg_id.py` & `wpyrogram-2.0.143/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/internals/seq_no.py` & `wpyrogram-2.0.143/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/session/session.py` & `wpyrogram-2.0.143/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/storage/__init__.py` & `wpyrogram-2.0.143/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/storage/file_storage.py` & `wpyrogram-2.0.143/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/storage/memory_storage.py` & `wpyrogram-2.0.143/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/storage/sqlite_storage.py` & `wpyrogram-2.0.143/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/storage/storage.py` & `wpyrogram-2.0.143/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/sync.py` & `wpyrogram-2.0.143/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/authorization/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/authorization/sent_code.py` & `wpyrogram-2.0.143/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/authorization/terms_of_service.py` & `wpyrogram-2.0.143/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/callback_game.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/callback_query.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/force_reply.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/game_high_score.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/login_url.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_channel_info.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_channel_info.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_chat_info.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_chat_info.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_poll_info.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_poll_info.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/request_user_info.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/request_user_info.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/requested_chats.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/requested_chats.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/bots_and_keyboards/web_app_info.py` & `wpyrogram-2.0.143/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/chosen_inline_result.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_animation.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_article.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_audio.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_contact.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_document.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_location.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_photo.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_venue.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_video.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/inline_mode/inline_query_result_voice.py` & `wpyrogram-2.0.143/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/input_media.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/input_media_animation.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/input_media_audio.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/input_media_document.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/input_media_photo.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/input_media_video.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_media/input_phone_contact.py` & `wpyrogram-2.0.143/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_message_content/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_message_content/input_message_content.py` & `wpyrogram-2.0.143/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_message_content/input_reply_to_message.py` & `wpyrogram-2.0.143/pyrogram/types/input_message_content/input_reply_to_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_message_content/input_reply_to_story.py` & `wpyrogram-2.0.143/pyrogram/types/input_message_content/input_reply_to_story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/input_message_content/input_text_message_content.py` & `wpyrogram-2.0.143/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/list.py` & `wpyrogram-2.0.143/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/animation.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/audio.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/auto_name.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/auto_name.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/boosts_status.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/boosts_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_action.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_action.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_event_action.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_member_status.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_members_filter.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/chat_type.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/chat_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/contact.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/dice.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/document.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_closed.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_created.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_edited.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/forum_topic_reopened.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/game.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/general_forum_topic_hidden.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/general_forum_topic_unhidden.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/gift_code.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/gift_code.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/giveaway.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/giveaway_result.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/giveaway_result.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/location.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/message.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_entity.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_entity_type.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_media_type.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_media_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_reactions.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_service_type.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_service_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/message_story.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/message_story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/messages_filter.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/messages_filter.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/my_boost.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/my_boost.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/next_code_type.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/next_code_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/parse_mode.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/parse_mode.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/photo.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/poll.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/poll_option.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/poll_type.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/poll_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/reaction.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/sent_code_type.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/sticker.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/story.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/thumbnail.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/user_status.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/user_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/venue.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/video.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/video_note.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/voice.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/web_app_data.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/messages_and_media/web_page.py` & `wpyrogram-2.0.143/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/object.py` & `wpyrogram-2.0.143/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/update.py` & `wpyrogram-2.0.143/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/__init__.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_info.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_info.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_message.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_message.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_recipients.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_recipients.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_weekly_open.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_weekly_open.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/business_working_hours.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/business_working_hours.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_color.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_event.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_event_filter.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_invite_link.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_join_request.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_joiner.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_member.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_member_updated.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_permissions.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_photo.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_preview.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_privileges.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/chat_reactions.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/dialog.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/emoji_status.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/folder.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/folder.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/invite_link_importer.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/restriction.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/user.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/username.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_ended.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/types/user_and_chats/video_chat_started.py` & `wpyrogram-2.0.143/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/pyrogram/utils.py` & `wpyrogram-2.0.143/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/setup.py` & `wpyrogram-2.0.143/setup.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/tests/__init__.py` & `wpyrogram-2.0.143/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/tests/filters/__init__.py` & `wpyrogram-2.0.143/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/tests/filters/test_command.py` & `wpyrogram-2.0.143/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/tests/parser/__init__.py` & `wpyrogram-2.0.143/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/tests/parser/test_html.py` & `wpyrogram-2.0.143/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/tests/parser/test_markdown.py` & `wpyrogram-2.0.143/tests/parser/test_markdown.py`

 * *Files identical despite different names*

### Comparing `WPyrogram-2.0.142/tests/test_file_id.py` & `wpyrogram-2.0.143/tests/test_file_id.py`

 * *Files identical despite different names*


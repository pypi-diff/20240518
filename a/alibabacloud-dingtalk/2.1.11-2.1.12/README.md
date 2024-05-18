# Comparing `tmp/alibabacloud_dingtalk-2.1.11.tar.gz` & `tmp/alibabacloud_dingtalk-2.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.11.tar", last modified: Tue May 14 12:53:56 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.12.tar", last modified: Sat May 18 17:22:34 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.1.11.tar` & `alibabacloud_dingtalk-2.1.12.tar`

### file list

```diff
@@ -1,429 +1,429 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/
--rw-r--r--   0 root         (0) root         (0)   129543 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2575 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2660 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10220 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15463 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25446 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24061 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46094 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    51351 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11812 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23886 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69836 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171793 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15310 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19568 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30918 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47170 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31278 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27481 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114212 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   145728 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248134 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413198 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53158 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    64382 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6152 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4135 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   306758 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   657929 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98018 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   115937 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11616 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9944 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191860 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   398319 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34906 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42901 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89960 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   237978 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10504 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88282 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124205 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185660 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   224123 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71002 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   126248 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   408970 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   425714 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25686 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43876 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40206 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44858 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21312 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30666 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23500 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10844 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14576 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6516 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10302 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   315868 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   638801 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5774 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7253 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37328 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46524 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494304 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515207 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134392 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   150282 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16480 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15793 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70120 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56029 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79025 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81667 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   313048 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322887 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260012 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385294 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23366 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168538 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   200479 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   672294 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   877133 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89270 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113792 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104118 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121491 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22157 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20888 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   461632 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538069 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191008 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   320947 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21190 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28705 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42854 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53610 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5681 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5155 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12390 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9744 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98153 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137888 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20603 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18299 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84750 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124476 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   176297 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   226839 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   365994 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   376047 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28815 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33507 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107508 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91958 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   815324 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   937150 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75114 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157606 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78582 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108065 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   110044 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133326 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11628 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18311 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23610 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181489 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   173547 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62895 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53887 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71486 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63136 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42982 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44105 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10832 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7243 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107234 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167406 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93818 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123438 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69184 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    59069 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35028 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68771 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   319400 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   411401 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21787 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30496 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44394 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164608 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172757 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115490 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105876 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129630 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168457 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47742 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46647 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   460426 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   551312 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38532 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26120 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54274 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95239 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   226462 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   350226 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70068 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95695 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16918 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28519 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84018 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152968 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17044 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16445 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17118 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22383 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16528 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17427 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91210 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135827 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92596 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111817 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40437 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40791 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10216 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21704 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79864 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129013 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6226 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8459 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50430 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43338 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   241480 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   422344 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3678 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   590500 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   761218 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4472 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14206 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-05-14 12:53:56.000000 alibabacloud_dingtalk-2.1.11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/
+-rw-r--r--   0 root         (0) root         (0)   131089 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10220 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15463 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25446 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24061 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51732 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    55896 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23886 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69836 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171793 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19974 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25370 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30918 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47170 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31278 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27481 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114212 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   145728 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248134 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413198 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53158 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    64382 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   306758 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   657929 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98018 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   115937 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191860 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   398319 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34906 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42901 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89960 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   237978 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88282 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124205 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185660 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   224275 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71002 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   126248 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   408970 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   425714 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25686 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43876 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40206 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44858 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21312 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30666 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23500 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14576 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6516 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10302 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   315868 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   638801 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7253 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37328 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46524 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494304 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515207 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134392 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   150282 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16480 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15793 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70120 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56029 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79025 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81667 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   313048 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322887 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260012 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385294 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23366 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168538 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   200479 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   672294 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   877133 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89270 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113792 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104118 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121491 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22157 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20888 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   477634 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552235 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191008 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   320947 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21190 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28705 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42854 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53610 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98153 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137888 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20603 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18299 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84750 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124476 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195023 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   271213 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   365994 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   376047 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28815 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33507 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107508 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91958 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   815324 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   937150 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75114 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157606 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78582 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108065 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   110044 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133326 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18311 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23610 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181489 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   173547 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62895 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53887 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71486 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63136 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42982 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44105 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107234 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167406 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93818 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123438 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69184 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    59069 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35028 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68771 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   319400 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   411401 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21787 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30496 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44394 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164608 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172757 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115490 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105876 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129630 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168457 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47742 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46647 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   460426 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   551312 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38532 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26120 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54274 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95239 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   226462 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   350226 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70068 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95695 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16918 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28519 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84018 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152968 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17044 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16445 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17118 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22383 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16528 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17427 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91210 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135827 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92596 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111817 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40437 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40791 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10216 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21704 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79864 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129013 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8459 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50430 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43338 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252082 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   441259 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3678 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   590500 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   761218 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4472 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-18 17:22:34.000000 alibabacloud_dingtalk-2.1.12/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-18 17:22:33.000000 alibabacloud_dingtalk-2.1.12/setup.py
```

### Comparing `alibabacloud_dingtalk-2.1.11/ChangeLog.md` & `alibabacloud_dingtalk-2.1.12/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-14 Version: 2.1.11
+- Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-05-09 Version: 2.1.10
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-26 Version: 2.0.99
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-23 Version: 2.0.98
```

### Comparing `alibabacloud_dingtalk-2.1.11/LICENSE` & `alibabacloud_dingtalk-2.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/PKG-INFO` & `alibabacloud_dingtalk-2.1.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.1.11
+Version: 2.1.12
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.11/README-CN.md` & `alibabacloud_dingtalk-2.1.12/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/README.md` & `alibabacloud_dingtalk-2.1.12/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -533,14 +533,144 @@
         @param request: LiandanluTextToImageModelRequest
         @return: LiandanluTextToImageModelResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkai_paa_s__1__0_models.LiandanluTextToImageModelHeaders()
         return await self.liandanlu_text_to_image_model_with_options_async(request, headers, runtime)
 
+    def n_lto_frame_service_with_options(
+        self,
+        request: dingtalkai_paa_s__1__0_models.NLToFrameServiceRequest,
+        headers: dingtalkai_paa_s__1__0_models.NLToFrameServiceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkai_paa_s__1__0_models.NLToFrameServiceResponse:
+        """
+        @summary 通过配置的指令，连接用户和系统，训练大模型
+        
+        @param request: NLToFrameServiceRequest
+        @param headers: NLToFrameServiceHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: NLToFrameServiceResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.extension_str):
+            body['extensionStr'] = request.extension_str
+        if not UtilClient.is_unset(request.is_new_model):
+            body['isNewModel'] = request.is_new_model
+        if not UtilClient.is_unset(request.model_id):
+            body['modelId'] = request.model_id
+        if not UtilClient.is_unset(request.model_name):
+            body['modelName'] = request.model_name
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='NLToFrameService',
+            version='aiPaaS_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/aiPaaS/ai/nl2frame',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkai_paa_s__1__0_models.NLToFrameServiceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def n_lto_frame_service_with_options_async(
+        self,
+        request: dingtalkai_paa_s__1__0_models.NLToFrameServiceRequest,
+        headers: dingtalkai_paa_s__1__0_models.NLToFrameServiceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkai_paa_s__1__0_models.NLToFrameServiceResponse:
+        """
+        @summary 通过配置的指令，连接用户和系统，训练大模型
+        
+        @param request: NLToFrameServiceRequest
+        @param headers: NLToFrameServiceHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: NLToFrameServiceResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.extension_str):
+            body['extensionStr'] = request.extension_str
+        if not UtilClient.is_unset(request.is_new_model):
+            body['isNewModel'] = request.is_new_model
+        if not UtilClient.is_unset(request.model_id):
+            body['modelId'] = request.model_id
+        if not UtilClient.is_unset(request.model_name):
+            body['modelName'] = request.model_name
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='NLToFrameService',
+            version='aiPaaS_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/aiPaaS/ai/nl2frame',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkai_paa_s__1__0_models.NLToFrameServiceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def n_lto_frame_service(
+        self,
+        request: dingtalkai_paa_s__1__0_models.NLToFrameServiceRequest,
+    ) -> dingtalkai_paa_s__1__0_models.NLToFrameServiceResponse:
+        """
+        @summary 通过配置的指令，连接用户和系统，训练大模型
+        
+        @param request: NLToFrameServiceRequest
+        @return: NLToFrameServiceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkai_paa_s__1__0_models.NLToFrameServiceHeaders()
+        return self.n_lto_frame_service_with_options(request, headers, runtime)
+
+    async def n_lto_frame_service_async(
+        self,
+        request: dingtalkai_paa_s__1__0_models.NLToFrameServiceRequest,
+    ) -> dingtalkai_paa_s__1__0_models.NLToFrameServiceResponse:
+        """
+        @summary 通过配置的指令，连接用户和系统，训练大模型
+        
+        @param request: NLToFrameServiceRequest
+        @return: NLToFrameServiceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkai_paa_s__1__0_models.NLToFrameServiceHeaders()
+        return await self.n_lto_frame_service_with_options_async(request, headers, runtime)
+
     def query_baymax_skill_log_with_options(
         self,
         request: dingtalkai_paa_s__1__0_models.QueryBaymaxSkillLogRequest,
         headers: dingtalkai_paa_s__1__0_models.QueryBaymaxSkillLogHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkai_paa_s__1__0_models.QueryBaymaxSkillLogResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -739,14 +739,168 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = LiandanluTextToImageModelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class NLToFrameServiceHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class NLToFrameServiceRequest(TeaModel):
+    def __init__(
+        self,
+        extension_str: str = None,
+        is_new_model: bool = None,
+        model_id: str = None,
+        model_name: str = None,
+        user_id: int = None,
+    ):
+        self.extension_str = extension_str
+        self.is_new_model = is_new_model
+        # This parameter is required.
+        self.model_id = model_id
+        # This parameter is required.
+        self.model_name = model_name
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extension_str is not None:
+            result['extensionStr'] = self.extension_str
+        if self.is_new_model is not None:
+            result['isNewModel'] = self.is_new_model
+        if self.model_id is not None:
+            result['modelId'] = self.model_id
+        if self.model_name is not None:
+            result['modelName'] = self.model_name
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('extensionStr') is not None:
+            self.extension_str = m.get('extensionStr')
+        if m.get('isNewModel') is not None:
+            self.is_new_model = m.get('isNewModel')
+        if m.get('modelId') is not None:
+            self.model_id = m.get('modelId')
+        if m.get('modelName') is not None:
+            self.model_name = m.get('modelName')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class NLToFrameServiceResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: str = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class NLToFrameServiceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: NLToFrameServiceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = NLToFrameServiceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryBaymaxSkillLogHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,128 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def amdp_emp_role_data_push_with_options(
+        self,
+        request: dingtalkamdp__1__0_models.AmdpEmpRoleDataPushRequest,
+        headers: dingtalkamdp__1__0_models.AmdpEmpRoleDataPushHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkamdp__1__0_models.AmdpEmpRoleDataPushResponse:
+        """
+        @summary 人员角色数据推送
+        
+        @param request: AmdpEmpRoleDataPushRequest
+        @param headers: AmdpEmpRoleDataPushHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AmdpEmpRoleDataPushResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.param):
+            body['param'] = request.param
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AmdpEmpRoleDataPush',
+            version='amdp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/amdp/employeeRoles/datas/push',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkamdp__1__0_models.AmdpEmpRoleDataPushResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def amdp_emp_role_data_push_with_options_async(
+        self,
+        request: dingtalkamdp__1__0_models.AmdpEmpRoleDataPushRequest,
+        headers: dingtalkamdp__1__0_models.AmdpEmpRoleDataPushHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkamdp__1__0_models.AmdpEmpRoleDataPushResponse:
+        """
+        @summary 人员角色数据推送
+        
+        @param request: AmdpEmpRoleDataPushRequest
+        @param headers: AmdpEmpRoleDataPushHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AmdpEmpRoleDataPushResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.param):
+            body['param'] = request.param
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AmdpEmpRoleDataPush',
+            version='amdp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/amdp/employeeRoles/datas/push',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkamdp__1__0_models.AmdpEmpRoleDataPushResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def amdp_emp_role_data_push(
+        self,
+        request: dingtalkamdp__1__0_models.AmdpEmpRoleDataPushRequest,
+    ) -> dingtalkamdp__1__0_models.AmdpEmpRoleDataPushResponse:
+        """
+        @summary 人员角色数据推送
+        
+        @param request: AmdpEmpRoleDataPushRequest
+        @return: AmdpEmpRoleDataPushResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkamdp__1__0_models.AmdpEmpRoleDataPushHeaders()
+        return self.amdp_emp_role_data_push_with_options(request, headers, runtime)
+
+    async def amdp_emp_role_data_push_async(
+        self,
+        request: dingtalkamdp__1__0_models.AmdpEmpRoleDataPushRequest,
+    ) -> dingtalkamdp__1__0_models.AmdpEmpRoleDataPushResponse:
+        """
+        @summary 人员角色数据推送
+        
+        @param request: AmdpEmpRoleDataPushRequest
+        @return: AmdpEmpRoleDataPushResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkamdp__1__0_models.AmdpEmpRoleDataPushHeaders()
+        return await self.amdp_emp_role_data_push_with_options_async(request, headers, runtime)
+
     def amdp_employee_data_push_with_options(
         self,
         request: dingtalkamdp__1__0_models.AmdpEmployeeDataPushRequest,
         headers: dingtalkamdp__1__0_models.AmdpEmployeeDataPushHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkamdp__1__0_models.AmdpEmployeeDataPushResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,212 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
+class AmdpEmpRoleDataPushHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class AmdpEmpRoleDataPushRequestParam(TeaModel):
+    def __init__(
+        self,
+        dept_id: str = None,
+        is_delete: str = None,
+        role_code: str = None,
+        user_id: str = None,
+    ):
+        self.dept_id = dept_id
+        self.is_delete = is_delete
+        self.role_code = role_code
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.is_delete is not None:
+            result['isDelete'] = self.is_delete
+        if self.role_code is not None:
+            result['roleCode'] = self.role_code
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('isDelete') is not None:
+            self.is_delete = m.get('isDelete')
+        if m.get('roleCode') is not None:
+            self.role_code = m.get('roleCode')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class AmdpEmpRoleDataPushRequest(TeaModel):
+    def __init__(
+        self,
+        param: List[AmdpEmpRoleDataPushRequestParam] = None,
+    ):
+        self.param = param
+
+    def validate(self):
+        if self.param:
+            for k in self.param:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['param'] = []
+        if self.param is not None:
+            for k in self.param:
+                result['param'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.param = []
+        if m.get('param') is not None:
+            for k in m.get('param'):
+                temp_model = AmdpEmpRoleDataPushRequestParam()
+                self.param.append(temp_model.from_map(k))
+        return self
+
+
+class AmdpEmpRoleDataPushResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        result: bool = None,
+        status: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.result = result
+        self.status = status
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.result is not None:
+            result['result'] = self.result
+        if self.status is not None:
+            result['status'] = self.status
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class AmdpEmpRoleDataPushResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AmdpEmpRoleDataPushResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AmdpEmpRoleDataPushResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AmdpEmployeeDataPushHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -738,17 +738,20 @@
         self,
         cool_app_code: str = None,
         creator_union_id: str = None,
         extension_app_biz_data: str = None,
         schedule_conference_id: str = None,
         use_extension_app: bool = None,
     ):
+        # This parameter is required.
         self.cool_app_code = cool_app_code
+        # This parameter is required.
         self.creator_union_id = creator_union_id
         self.extension_app_biz_data = extension_app_biz_data
+        # This parameter is required.
         self.schedule_conference_id = schedule_conference_id
         self.use_extension_app = use_extension_app
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4838,14 +4841,15 @@
 
 
 class QueryScheduleConfSettingsRequest(TeaModel):
     def __init__(
         self,
         schedule_conference_id: str = None,
     ):
+        # This parameter is required.
         self.schedule_conference_id = schedule_conference_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1441,14 +1441,136 @@
         @param request: DistributePartnerAppRequest
         @return: DistributePartnerAppResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkexclusive__1__0_models.DistributePartnerAppHeaders()
         return await self.distribute_partner_app_with_options_async(request, headers, runtime)
 
+    def exchange_main_admin_with_options(
+        self,
+        request: dingtalkexclusive__1__0_models.ExchangeMainAdminRequest,
+        headers: dingtalkexclusive__1__0_models.ExchangeMainAdminHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.ExchangeMainAdminResponse:
+        """
+        @summary 更换组织主管理员
+        
+        @param request: ExchangeMainAdminRequest
+        @param headers: ExchangeMainAdminHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExchangeMainAdminResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.new_admin_user_id):
+            body['newAdminUserId'] = request.new_admin_user_id
+        if not UtilClient.is_unset(request.old_admin_user_id):
+            body['oldAdminUserId'] = request.old_admin_user_id
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ExchangeMainAdmin',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/orgnizations/mainAdministrators/exchange',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.ExchangeMainAdminResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def exchange_main_admin_with_options_async(
+        self,
+        request: dingtalkexclusive__1__0_models.ExchangeMainAdminRequest,
+        headers: dingtalkexclusive__1__0_models.ExchangeMainAdminHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.ExchangeMainAdminResponse:
+        """
+        @summary 更换组织主管理员
+        
+        @param request: ExchangeMainAdminRequest
+        @param headers: ExchangeMainAdminHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExchangeMainAdminResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.new_admin_user_id):
+            body['newAdminUserId'] = request.new_admin_user_id
+        if not UtilClient.is_unset(request.old_admin_user_id):
+            body['oldAdminUserId'] = request.old_admin_user_id
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ExchangeMainAdmin',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/orgnizations/mainAdministrators/exchange',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.ExchangeMainAdminResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def exchange_main_admin(
+        self,
+        request: dingtalkexclusive__1__0_models.ExchangeMainAdminRequest,
+    ) -> dingtalkexclusive__1__0_models.ExchangeMainAdminResponse:
+        """
+        @summary 更换组织主管理员
+        
+        @param request: ExchangeMainAdminRequest
+        @return: ExchangeMainAdminResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.ExchangeMainAdminHeaders()
+        return self.exchange_main_admin_with_options(request, headers, runtime)
+
+    async def exchange_main_admin_async(
+        self,
+        request: dingtalkexclusive__1__0_models.ExchangeMainAdminRequest,
+    ) -> dingtalkexclusive__1__0_models.ExchangeMainAdminResponse:
+        """
+        @summary 更换组织主管理员
+        
+        @param request: ExchangeMainAdminRequest
+        @return: ExchangeMainAdminResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.ExchangeMainAdminHeaders()
+        return await self.exchange_main_admin_with_options_async(request, headers, runtime)
+
     def exclusive_create_ding_portal_with_options(
         self,
         request: dingtalkexclusive__1__0_models.ExclusiveCreateDingPortalRequest,
         headers: dingtalkexclusive__1__0_models.ExclusiveCreateDingPortalHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkexclusive__1__0_models.ExclusiveCreateDingPortalResponse:
         """
@@ -7395,14 +7517,140 @@
         @param request: LogoutRequest
         @return: LogoutResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkexclusive__1__0_models.LogoutHeaders()
         return await self.logout_with_options_async(request, headers, runtime)
 
+    def open_benefit_package_with_options(
+        self,
+        request: dingtalkexclusive__1__0_models.OpenBenefitPackageRequest,
+        headers: dingtalkexclusive__1__0_models.OpenBenefitPackageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.OpenBenefitPackageResponse:
+        """
+        @summary 购买权益包
+        
+        @param request: OpenBenefitPackageRequest
+        @param headers: OpenBenefitPackageHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenBenefitPackageResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.benefit_package):
+            body['benefitPackage'] = request.benefit_package
+        if not UtilClient.is_unset(request.end_date):
+            body['endDate'] = request.end_date
+        if not UtilClient.is_unset(request.start_date):
+            body['startDate'] = request.start_date
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenBenefitPackage',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/benefitPackages/purchase',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.OpenBenefitPackageResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def open_benefit_package_with_options_async(
+        self,
+        request: dingtalkexclusive__1__0_models.OpenBenefitPackageRequest,
+        headers: dingtalkexclusive__1__0_models.OpenBenefitPackageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.OpenBenefitPackageResponse:
+        """
+        @summary 购买权益包
+        
+        @param request: OpenBenefitPackageRequest
+        @param headers: OpenBenefitPackageHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenBenefitPackageResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.benefit_package):
+            body['benefitPackage'] = request.benefit_package
+        if not UtilClient.is_unset(request.end_date):
+            body['endDate'] = request.end_date
+        if not UtilClient.is_unset(request.start_date):
+            body['startDate'] = request.start_date
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='OpenBenefitPackage',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/benefitPackages/purchase',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.OpenBenefitPackageResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def open_benefit_package(
+        self,
+        request: dingtalkexclusive__1__0_models.OpenBenefitPackageRequest,
+    ) -> dingtalkexclusive__1__0_models.OpenBenefitPackageResponse:
+        """
+        @summary 购买权益包
+        
+        @param request: OpenBenefitPackageRequest
+        @return: OpenBenefitPackageResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.OpenBenefitPackageHeaders()
+        return self.open_benefit_package_with_options(request, headers, runtime)
+
+    async def open_benefit_package_async(
+        self,
+        request: dingtalkexclusive__1__0_models.OpenBenefitPackageRequest,
+    ) -> dingtalkexclusive__1__0_models.OpenBenefitPackageResponse:
+        """
+        @summary 购买权益包
+        
+        @param request: OpenBenefitPackageRequest
+        @return: OpenBenefitPackageResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.OpenBenefitPackageHeaders()
+        return await self.open_benefit_package_with_options_async(request, headers, runtime)
+
     def prevent_cheating_check_risk_with_options(
         self,
         request: dingtalkexclusive__1__0_models.PreventCheatingCheckRiskRequest,
         headers: dingtalkexclusive__1__0_models.PreventCheatingCheckRiskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkexclusive__1__0_models.PreventCheatingCheckRiskResponse:
         """
@@ -10688,7 +10936,125 @@
         
         @param request: UpdateStorageModeRequest
         @return: UpdateStorageModeResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkexclusive__1__0_models.UpdateStorageModeHeaders()
         return await self.update_storage_mode_with_options_async(request, headers, runtime)
+
+    def update_voice_msg_ctrl_status_with_options(
+        self,
+        request: dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusRequest,
+        headers: dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusResponse:
+        """
+        @summary 允许三方调用该API，决定对应的语音消息管控状态
+        
+        @param request: UpdateVoiceMsgCtrlStatusRequest
+        @param headers: UpdateVoiceMsgCtrlStatusHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateVoiceMsgCtrlStatusResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.status):
+            body['status'] = request.status
+        if not UtilClient.is_unset(request.voice_msg_ctrl_info):
+            body['voiceMsgCtrlInfo'] = request.voice_msg_ctrl_info
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateVoiceMsgCtrlStatus',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/voiceMessages/ctrlStatuses',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def update_voice_msg_ctrl_status_with_options_async(
+        self,
+        request: dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusRequest,
+        headers: dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusResponse:
+        """
+        @summary 允许三方调用该API，决定对应的语音消息管控状态
+        
+        @param request: UpdateVoiceMsgCtrlStatusRequest
+        @param headers: UpdateVoiceMsgCtrlStatusHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateVoiceMsgCtrlStatusResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.status):
+            body['status'] = request.status
+        if not UtilClient.is_unset(request.voice_msg_ctrl_info):
+            body['voiceMsgCtrlInfo'] = request.voice_msg_ctrl_info
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateVoiceMsgCtrlStatus',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/voiceMessages/ctrlStatuses',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def update_voice_msg_ctrl_status(
+        self,
+        request: dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusRequest,
+    ) -> dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusResponse:
+        """
+        @summary 允许三方调用该API，决定对应的语音消息管控状态
+        
+        @param request: UpdateVoiceMsgCtrlStatusRequest
+        @return: UpdateVoiceMsgCtrlStatusResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusHeaders()
+        return self.update_voice_msg_ctrl_status_with_options(request, headers, runtime)
+
+    async def update_voice_msg_ctrl_status_async(
+        self,
+        request: dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusRequest,
+    ) -> dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusResponse:
+        """
+        @summary 允许三方调用该API，决定对应的语音消息管控状态
+        
+        @param request: UpdateVoiceMsgCtrlStatusRequest
+        @return: UpdateVoiceMsgCtrlStatusResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.UpdateVoiceMsgCtrlStatusHeaders()
+        return await self.update_voice_msg_ctrl_status_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1726,14 +1726,157 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DistributePartnerAppResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ExchangeMainAdminHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class ExchangeMainAdminRequest(TeaModel):
+    def __init__(
+        self,
+        new_admin_user_id: str = None,
+        old_admin_user_id: str = None,
+        target_corp_id: str = None,
+    ):
+        # This parameter is required.
+        self.new_admin_user_id = new_admin_user_id
+        # This parameter is required.
+        self.old_admin_user_id = old_admin_user_id
+        # This parameter is required.
+        self.target_corp_id = target_corp_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.new_admin_user_id is not None:
+            result['newAdminUserId'] = self.new_admin_user_id
+        if self.old_admin_user_id is not None:
+            result['oldAdminUserId'] = self.old_admin_user_id
+        if self.target_corp_id is not None:
+            result['targetCorpId'] = self.target_corp_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('newAdminUserId') is not None:
+            self.new_admin_user_id = m.get('newAdminUserId')
+        if m.get('oldAdminUserId') is not None:
+            self.old_admin_user_id = m.get('oldAdminUserId')
+        if m.get('targetCorpId') is not None:
+            self.target_corp_id = m.get('targetCorpId')
+        return self
+
+
+class ExchangeMainAdminResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class ExchangeMainAdminResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ExchangeMainAdminResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ExchangeMainAdminResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ExclusiveCreateDingPortalHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -12587,14 +12730,164 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = LogoutResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class OpenBenefitPackageHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class OpenBenefitPackageRequest(TeaModel):
+    def __init__(
+        self,
+        benefit_package: int = None,
+        end_date: int = None,
+        start_date: int = None,
+        target_corp_id: str = None,
+    ):
+        # This parameter is required.
+        self.benefit_package = benefit_package
+        # This parameter is required.
+        self.end_date = end_date
+        # This parameter is required.
+        self.start_date = start_date
+        # This parameter is required.
+        self.target_corp_id = target_corp_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.benefit_package is not None:
+            result['benefitPackage'] = self.benefit_package
+        if self.end_date is not None:
+            result['endDate'] = self.end_date
+        if self.start_date is not None:
+            result['startDate'] = self.start_date
+        if self.target_corp_id is not None:
+            result['targetCorpId'] = self.target_corp_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('benefitPackage') is not None:
+            self.benefit_package = m.get('benefitPackage')
+        if m.get('endDate') is not None:
+            self.end_date = m.get('endDate')
+        if m.get('startDate') is not None:
+            self.start_date = m.get('startDate')
+        if m.get('targetCorpId') is not None:
+            self.target_corp_id = m.get('targetCorpId')
+        return self
+
+
+class OpenBenefitPackageResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class OpenBenefitPackageResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: OpenBenefitPackageResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = OpenBenefitPackageResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PreventCheatingCheckRiskHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -17270,7 +17563,188 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateStorageModeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateVoiceMsgCtrlStatusHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UpdateVoiceMsgCtrlStatusRequestVoiceMsgCtrlInfo(TeaModel):
+    def __init__(
+        self,
+        open_conversation_id: str = None,
+        open_msg_id: str = None,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.open_conversation_id = open_conversation_id
+        # This parameter is required.
+        self.open_msg_id = open_msg_id
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.open_msg_id is not None:
+            result['openMsgId'] = self.open_msg_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('openMsgId') is not None:
+            self.open_msg_id = m.get('openMsgId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class UpdateVoiceMsgCtrlStatusRequest(TeaModel):
+    def __init__(
+        self,
+        status: int = None,
+        voice_msg_ctrl_info: UpdateVoiceMsgCtrlStatusRequestVoiceMsgCtrlInfo = None,
+    ):
+        # This parameter is required.
+        self.status = status
+        # This parameter is required.
+        self.voice_msg_ctrl_info = voice_msg_ctrl_info
+
+    def validate(self):
+        if self.voice_msg_ctrl_info:
+            self.voice_msg_ctrl_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.status is not None:
+            result['status'] = self.status
+        if self.voice_msg_ctrl_info is not None:
+            result['voiceMsgCtrlInfo'] = self.voice_msg_ctrl_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('voiceMsgCtrlInfo') is not None:
+            temp_model = UpdateVoiceMsgCtrlStatusRequestVoiceMsgCtrlInfo()
+            self.voice_msg_ctrl_info = temp_model.from_map(m['voiceMsgCtrlInfo'])
+        return self
+
+
+class UpdateVoiceMsgCtrlStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        # This parameter is required.
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class UpdateVoiceMsgCtrlStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateVoiceMsgCtrlStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateVoiceMsgCtrlStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,160 @@
         self._client = GatewayClientClient()
         self._spi = self._client
         self._signature_algorithm = 'v2'
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def add_hrm_legal_entity_with_options(
+        self,
+        request: dingtalkhrm__1__0_models.AddHrmLegalEntityRequest,
+        headers: dingtalkhrm__1__0_models.AddHrmLegalEntityHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.AddHrmLegalEntityResponse:
+        """
+        @summary 新增法人公司
+        
+        @param request: AddHrmLegalEntityRequest
+        @param headers: AddHrmLegalEntityHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddHrmLegalEntityResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ding_tenant_id):
+            query['dingTenantId'] = request.ding_tenant_id
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.create_user_id):
+            body['createUserId'] = request.create_user_id
+        if not UtilClient.is_unset(request.ext):
+            body['ext'] = request.ext
+        if not UtilClient.is_unset(request.legal_entity_name):
+            body['legalEntityName'] = request.legal_entity_name
+        if not UtilClient.is_unset(request.legal_entity_short_name):
+            body['legalEntityShortName'] = request.legal_entity_short_name
+        if not UtilClient.is_unset(request.legal_entity_status):
+            body['legalEntityStatus'] = request.legal_entity_status
+        if not UtilClient.is_unset(request.legal_person_name):
+            body['legalPersonName'] = request.legal_person_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AddHrmLegalEntity',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/masters/legalEntities/companies',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.AddHrmLegalEntityResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def add_hrm_legal_entity_with_options_async(
+        self,
+        request: dingtalkhrm__1__0_models.AddHrmLegalEntityRequest,
+        headers: dingtalkhrm__1__0_models.AddHrmLegalEntityHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.AddHrmLegalEntityResponse:
+        """
+        @summary 新增法人公司
+        
+        @param request: AddHrmLegalEntityRequest
+        @param headers: AddHrmLegalEntityHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddHrmLegalEntityResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ding_tenant_id):
+            query['dingTenantId'] = request.ding_tenant_id
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.create_user_id):
+            body['createUserId'] = request.create_user_id
+        if not UtilClient.is_unset(request.ext):
+            body['ext'] = request.ext
+        if not UtilClient.is_unset(request.legal_entity_name):
+            body['legalEntityName'] = request.legal_entity_name
+        if not UtilClient.is_unset(request.legal_entity_short_name):
+            body['legalEntityShortName'] = request.legal_entity_short_name
+        if not UtilClient.is_unset(request.legal_entity_status):
+            body['legalEntityStatus'] = request.legal_entity_status
+        if not UtilClient.is_unset(request.legal_person_name):
+            body['legalPersonName'] = request.legal_person_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AddHrmLegalEntity',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/masters/legalEntities/companies',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.AddHrmLegalEntityResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def add_hrm_legal_entity(
+        self,
+        request: dingtalkhrm__1__0_models.AddHrmLegalEntityRequest,
+    ) -> dingtalkhrm__1__0_models.AddHrmLegalEntityResponse:
+        """
+        @summary 新增法人公司
+        
+        @param request: AddHrmLegalEntityRequest
+        @return: AddHrmLegalEntityResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.AddHrmLegalEntityHeaders()
+        return self.add_hrm_legal_entity_with_options(request, headers, runtime)
+
+    async def add_hrm_legal_entity_async(
+        self,
+        request: dingtalkhrm__1__0_models.AddHrmLegalEntityRequest,
+    ) -> dingtalkhrm__1__0_models.AddHrmLegalEntityResponse:
+        """
+        @summary 新增法人公司
+        
+        @param request: AddHrmLegalEntityRequest
+        @return: AddHrmLegalEntityResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.AddHrmLegalEntityHeaders()
+        return await self.add_hrm_legal_entity_with_options_async(request, headers, runtime)
+
     def add_hrm_preentry_with_options(
         self,
         request: dingtalkhrm__1__0_models.AddHrmPreentryRequest,
         headers: dingtalkhrm__1__0_models.AddHrmPreentryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkhrm__1__0_models.AddHrmPreentryResponse:
         """
@@ -4051,14 +4197,282 @@
         @param request: SyncTaskTemplateRequest
         @return: SyncTaskTemplateResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkhrm__1__0_models.SyncTaskTemplateHeaders()
         return await self.sync_task_template_with_options_async(request, headers, runtime)
 
+    def update_hrm_legal_entity_name_with_options(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameRequest,
+        headers: dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameResponse:
+        """
+        @summary 更新法人公司名称
+        
+        @param request: UpdateHrmLegalEntityNameRequest
+        @param headers: UpdateHrmLegalEntityNameHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateHrmLegalEntityNameResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ding_tenant_id):
+            query['dingTenantId'] = request.ding_tenant_id
+        if not UtilClient.is_unset(request.legal_entity_name):
+            query['legalEntityName'] = request.legal_entity_name
+        if not UtilClient.is_unset(request.origin_legal_entity_name):
+            query['originLegalEntityName'] = request.origin_legal_entity_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateHrmLegalEntityName',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/masters/legalEntities/companyNames',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def update_hrm_legal_entity_name_with_options_async(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameRequest,
+        headers: dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameResponse:
+        """
+        @summary 更新法人公司名称
+        
+        @param request: UpdateHrmLegalEntityNameRequest
+        @param headers: UpdateHrmLegalEntityNameHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateHrmLegalEntityNameResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ding_tenant_id):
+            query['dingTenantId'] = request.ding_tenant_id
+        if not UtilClient.is_unset(request.legal_entity_name):
+            query['legalEntityName'] = request.legal_entity_name
+        if not UtilClient.is_unset(request.origin_legal_entity_name):
+            query['originLegalEntityName'] = request.origin_legal_entity_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateHrmLegalEntityName',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/masters/legalEntities/companyNames',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def update_hrm_legal_entity_name(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameRequest,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameResponse:
+        """
+        @summary 更新法人公司名称
+        
+        @param request: UpdateHrmLegalEntityNameRequest
+        @return: UpdateHrmLegalEntityNameResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameHeaders()
+        return self.update_hrm_legal_entity_name_with_options(request, headers, runtime)
+
+    async def update_hrm_legal_entity_name_async(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameRequest,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameResponse:
+        """
+        @summary 更新法人公司名称
+        
+        @param request: UpdateHrmLegalEntityNameRequest
+        @return: UpdateHrmLegalEntityNameResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.UpdateHrmLegalEntityNameHeaders()
+        return await self.update_hrm_legal_entity_name_with_options_async(request, headers, runtime)
+
+    def update_hrm_legal_entity_without_name_with_options(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameRequest,
+        headers: dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameResponse:
+        """
+        @summary 更新法人公司
+        
+        @param request: UpdateHrmLegalEntityWithoutNameRequest
+        @param headers: UpdateHrmLegalEntityWithoutNameHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateHrmLegalEntityWithoutNameResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ding_tenant_id):
+            query['dingTenantId'] = request.ding_tenant_id
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.create_user_id):
+            body['createUserId'] = request.create_user_id
+        if not UtilClient.is_unset(request.ext):
+            body['ext'] = request.ext
+        if not UtilClient.is_unset(request.legal_entity_name):
+            body['legalEntityName'] = request.legal_entity_name
+        if not UtilClient.is_unset(request.legal_entity_short_name):
+            body['legalEntityShortName'] = request.legal_entity_short_name
+        if not UtilClient.is_unset(request.legal_entity_status):
+            body['legalEntityStatus'] = request.legal_entity_status
+        if not UtilClient.is_unset(request.legal_person_name):
+            body['legalPersonName'] = request.legal_person_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateHrmLegalEntityWithoutName',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/masters/legalEntities/companies',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def update_hrm_legal_entity_without_name_with_options_async(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameRequest,
+        headers: dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameResponse:
+        """
+        @summary 更新法人公司
+        
+        @param request: UpdateHrmLegalEntityWithoutNameRequest
+        @param headers: UpdateHrmLegalEntityWithoutNameHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateHrmLegalEntityWithoutNameResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ding_tenant_id):
+            query['dingTenantId'] = request.ding_tenant_id
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.create_user_id):
+            body['createUserId'] = request.create_user_id
+        if not UtilClient.is_unset(request.ext):
+            body['ext'] = request.ext
+        if not UtilClient.is_unset(request.legal_entity_name):
+            body['legalEntityName'] = request.legal_entity_name
+        if not UtilClient.is_unset(request.legal_entity_short_name):
+            body['legalEntityShortName'] = request.legal_entity_short_name
+        if not UtilClient.is_unset(request.legal_entity_status):
+            body['legalEntityStatus'] = request.legal_entity_status
+        if not UtilClient.is_unset(request.legal_person_name):
+            body['legalPersonName'] = request.legal_person_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateHrmLegalEntityWithoutName',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/masters/legalEntities/companies',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def update_hrm_legal_entity_without_name(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameRequest,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameResponse:
+        """
+        @summary 更新法人公司
+        
+        @param request: UpdateHrmLegalEntityWithoutNameRequest
+        @return: UpdateHrmLegalEntityWithoutNameResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameHeaders()
+        return self.update_hrm_legal_entity_without_name_with_options(request, headers, runtime)
+
+    async def update_hrm_legal_entity_without_name_async(
+        self,
+        request: dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameRequest,
+    ) -> dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameResponse:
+        """
+        @summary 更新法人公司
+        
+        @param request: UpdateHrmLegalEntityWithoutNameRequest
+        @return: UpdateHrmLegalEntityWithoutNameResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.UpdateHrmLegalEntityWithoutNameHeaders()
+        return await self.update_hrm_legal_entity_without_name_with_options_async(request, headers, runtime)
+
     def update_isv_card_message_with_options(
         self,
         request: dingtalkhrm__1__0_models.UpdateIsvCardMessageRequest,
         headers: dingtalkhrm__1__0_models.UpdateIsvCardMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkhrm__1__0_models.UpdateIsvCardMessageResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,501 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List, Any
 
 
+class AddHrmLegalEntityHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class AddHrmLegalEntityRequestExtManageAddress(TeaModel):
+    def __init__(
+        self,
+        area_code: str = None,
+        area_name: str = None,
+        city_code: str = None,
+        city_name: str = None,
+        country_code: str = None,
+        country_name: str = None,
+        detail_address: str = None,
+        global_area_type: str = None,
+        province_code: str = None,
+        province_name: str = None,
+    ):
+        self.area_code = area_code
+        self.area_name = area_name
+        self.city_code = city_code
+        self.city_name = city_name
+        self.country_code = country_code
+        self.country_name = country_name
+        self.detail_address = detail_address
+        self.global_area_type = global_area_type
+        self.province_code = province_code
+        self.province_name = province_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.area_code is not None:
+            result['areaCode'] = self.area_code
+        if self.area_name is not None:
+            result['areaName'] = self.area_name
+        if self.city_code is not None:
+            result['cityCode'] = self.city_code
+        if self.city_name is not None:
+            result['cityName'] = self.city_name
+        if self.country_code is not None:
+            result['countryCode'] = self.country_code
+        if self.country_name is not None:
+            result['countryName'] = self.country_name
+        if self.detail_address is not None:
+            result['detailAddress'] = self.detail_address
+        if self.global_area_type is not None:
+            result['globalAreaType'] = self.global_area_type
+        if self.province_code is not None:
+            result['provinceCode'] = self.province_code
+        if self.province_name is not None:
+            result['provinceName'] = self.province_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('areaCode') is not None:
+            self.area_code = m.get('areaCode')
+        if m.get('areaName') is not None:
+            self.area_name = m.get('areaName')
+        if m.get('cityCode') is not None:
+            self.city_code = m.get('cityCode')
+        if m.get('cityName') is not None:
+            self.city_name = m.get('cityName')
+        if m.get('countryCode') is not None:
+            self.country_code = m.get('countryCode')
+        if m.get('countryName') is not None:
+            self.country_name = m.get('countryName')
+        if m.get('detailAddress') is not None:
+            self.detail_address = m.get('detailAddress')
+        if m.get('globalAreaType') is not None:
+            self.global_area_type = m.get('globalAreaType')
+        if m.get('provinceCode') is not None:
+            self.province_code = m.get('provinceCode')
+        if m.get('provinceName') is not None:
+            self.province_name = m.get('provinceName')
+        return self
+
+
+class AddHrmLegalEntityRequestExtRegistrationAddress(TeaModel):
+    def __init__(
+        self,
+        area_code: str = None,
+        area_name: str = None,
+        city_code: str = None,
+        city_name: str = None,
+        country_code: str = None,
+        country_name: str = None,
+        detail_address: str = None,
+        global_area_type: str = None,
+        province_code: str = None,
+        province_name: str = None,
+    ):
+        self.area_code = area_code
+        self.area_name = area_name
+        self.city_code = city_code
+        self.city_name = city_name
+        self.country_code = country_code
+        self.country_name = country_name
+        self.detail_address = detail_address
+        self.global_area_type = global_area_type
+        self.province_code = province_code
+        self.province_name = province_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.area_code is not None:
+            result['areaCode'] = self.area_code
+        if self.area_name is not None:
+            result['areaName'] = self.area_name
+        if self.city_code is not None:
+            result['cityCode'] = self.city_code
+        if self.city_name is not None:
+            result['cityName'] = self.city_name
+        if self.country_code is not None:
+            result['countryCode'] = self.country_code
+        if self.country_name is not None:
+            result['countryName'] = self.country_name
+        if self.detail_address is not None:
+            result['detailAddress'] = self.detail_address
+        if self.global_area_type is not None:
+            result['globalAreaType'] = self.global_area_type
+        if self.province_code is not None:
+            result['provinceCode'] = self.province_code
+        if self.province_name is not None:
+            result['provinceName'] = self.province_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('areaCode') is not None:
+            self.area_code = m.get('areaCode')
+        if m.get('areaName') is not None:
+            self.area_name = m.get('areaName')
+        if m.get('cityCode') is not None:
+            self.city_code = m.get('cityCode')
+        if m.get('cityName') is not None:
+            self.city_name = m.get('cityName')
+        if m.get('countryCode') is not None:
+            self.country_code = m.get('countryCode')
+        if m.get('countryName') is not None:
+            self.country_name = m.get('countryName')
+        if m.get('detailAddress') is not None:
+            self.detail_address = m.get('detailAddress')
+        if m.get('globalAreaType') is not None:
+            self.global_area_type = m.get('globalAreaType')
+        if m.get('provinceCode') is not None:
+            self.province_code = m.get('provinceCode')
+        if m.get('provinceName') is not None:
+            self.province_name = m.get('provinceName')
+        return self
+
+
+class AddHrmLegalEntityRequestExt(TeaModel):
+    def __init__(
+        self,
+        legal_entity_en_name: str = None,
+        legal_entity_en_short_name: str = None,
+        legal_entity_type: str = None,
+        manage_address: AddHrmLegalEntityRequestExtManageAddress = None,
+        registration_address: AddHrmLegalEntityRequestExtRegistrationAddress = None,
+        registration_date: int = None,
+        unified_social_credit_code: str = None,
+        zip_code: str = None,
+    ):
+        self.legal_entity_en_name = legal_entity_en_name
+        self.legal_entity_en_short_name = legal_entity_en_short_name
+        self.legal_entity_type = legal_entity_type
+        self.manage_address = manage_address
+        self.registration_address = registration_address
+        self.registration_date = registration_date
+        self.unified_social_credit_code = unified_social_credit_code
+        self.zip_code = zip_code
+
+    def validate(self):
+        if self.manage_address:
+            self.manage_address.validate()
+        if self.registration_address:
+            self.registration_address.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.legal_entity_en_name is not None:
+            result['legalEntityEnName'] = self.legal_entity_en_name
+        if self.legal_entity_en_short_name is not None:
+            result['legalEntityEnShortName'] = self.legal_entity_en_short_name
+        if self.legal_entity_type is not None:
+            result['legalEntityType'] = self.legal_entity_type
+        if self.manage_address is not None:
+            result['manageAddress'] = self.manage_address.to_map()
+        if self.registration_address is not None:
+            result['registrationAddress'] = self.registration_address.to_map()
+        if self.registration_date is not None:
+            result['registrationDate'] = self.registration_date
+        if self.unified_social_credit_code is not None:
+            result['unifiedSocialCreditCode'] = self.unified_social_credit_code
+        if self.zip_code is not None:
+            result['zipCode'] = self.zip_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('legalEntityEnName') is not None:
+            self.legal_entity_en_name = m.get('legalEntityEnName')
+        if m.get('legalEntityEnShortName') is not None:
+            self.legal_entity_en_short_name = m.get('legalEntityEnShortName')
+        if m.get('legalEntityType') is not None:
+            self.legal_entity_type = m.get('legalEntityType')
+        if m.get('manageAddress') is not None:
+            temp_model = AddHrmLegalEntityRequestExtManageAddress()
+            self.manage_address = temp_model.from_map(m['manageAddress'])
+        if m.get('registrationAddress') is not None:
+            temp_model = AddHrmLegalEntityRequestExtRegistrationAddress()
+            self.registration_address = temp_model.from_map(m['registrationAddress'])
+        if m.get('registrationDate') is not None:
+            self.registration_date = m.get('registrationDate')
+        if m.get('unifiedSocialCreditCode') is not None:
+            self.unified_social_credit_code = m.get('unifiedSocialCreditCode')
+        if m.get('zipCode') is not None:
+            self.zip_code = m.get('zipCode')
+        return self
+
+
+class AddHrmLegalEntityRequest(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        create_user_id: str = None,
+        ext: AddHrmLegalEntityRequestExt = None,
+        legal_entity_name: str = None,
+        legal_entity_short_name: str = None,
+        legal_entity_status: int = None,
+        legal_person_name: str = None,
+        ding_tenant_id: int = None,
+    ):
+        # This parameter is required.
+        self.corp_id = corp_id
+        self.create_user_id = create_user_id
+        self.ext = ext
+        # This parameter is required.
+        self.legal_entity_name = legal_entity_name
+        self.legal_entity_short_name = legal_entity_short_name
+        # This parameter is required.
+        self.legal_entity_status = legal_entity_status
+        self.legal_person_name = legal_person_name
+        self.ding_tenant_id = ding_tenant_id
+
+    def validate(self):
+        if self.ext:
+            self.ext.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.create_user_id is not None:
+            result['createUserId'] = self.create_user_id
+        if self.ext is not None:
+            result['ext'] = self.ext.to_map()
+        if self.legal_entity_name is not None:
+            result['legalEntityName'] = self.legal_entity_name
+        if self.legal_entity_short_name is not None:
+            result['legalEntityShortName'] = self.legal_entity_short_name
+        if self.legal_entity_status is not None:
+            result['legalEntityStatus'] = self.legal_entity_status
+        if self.legal_person_name is not None:
+            result['legalPersonName'] = self.legal_person_name
+        if self.ding_tenant_id is not None:
+            result['dingTenantId'] = self.ding_tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('createUserId') is not None:
+            self.create_user_id = m.get('createUserId')
+        if m.get('ext') is not None:
+            temp_model = AddHrmLegalEntityRequestExt()
+            self.ext = temp_model.from_map(m['ext'])
+        if m.get('legalEntityName') is not None:
+            self.legal_entity_name = m.get('legalEntityName')
+        if m.get('legalEntityShortName') is not None:
+            self.legal_entity_short_name = m.get('legalEntityShortName')
+        if m.get('legalEntityStatus') is not None:
+            self.legal_entity_status = m.get('legalEntityStatus')
+        if m.get('legalPersonName') is not None:
+            self.legal_person_name = m.get('legalPersonName')
+        if m.get('dingTenantId') is not None:
+            self.ding_tenant_id = m.get('dingTenantId')
+        return self
+
+
+class AddHrmLegalEntityResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        gmt_create: int = None,
+        gmt_modified: int = None,
+        legal_entity_id: str = None,
+        legal_entity_name: str = None,
+        legal_entity_short_name: str = None,
+        legal_entity_status: int = None,
+        legal_person_name: str = None,
+    ):
+        self.corp_id = corp_id
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.legal_entity_id = legal_entity_id
+        self.legal_entity_name = legal_entity_name
+        self.legal_entity_short_name = legal_entity_short_name
+        self.legal_entity_status = legal_entity_status
+        self.legal_person_name = legal_person_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.gmt_create is not None:
+            result['gmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['gmtModified'] = self.gmt_modified
+        if self.legal_entity_id is not None:
+            result['legalEntityId'] = self.legal_entity_id
+        if self.legal_entity_name is not None:
+            result['legalEntityName'] = self.legal_entity_name
+        if self.legal_entity_short_name is not None:
+            result['legalEntityShortName'] = self.legal_entity_short_name
+        if self.legal_entity_status is not None:
+            result['legalEntityStatus'] = self.legal_entity_status
+        if self.legal_person_name is not None:
+            result['legalPersonName'] = self.legal_person_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('gmtCreate') is not None:
+            self.gmt_create = m.get('gmtCreate')
+        if m.get('gmtModified') is not None:
+            self.gmt_modified = m.get('gmtModified')
+        if m.get('legalEntityId') is not None:
+            self.legal_entity_id = m.get('legalEntityId')
+        if m.get('legalEntityName') is not None:
+            self.legal_entity_name = m.get('legalEntityName')
+        if m.get('legalEntityShortName') is not None:
+            self.legal_entity_short_name = m.get('legalEntityShortName')
+        if m.get('legalEntityStatus') is not None:
+            self.legal_entity_status = m.get('legalEntityStatus')
+        if m.get('legalPersonName') is not None:
+            self.legal_person_name = m.get('legalPersonName')
+        return self
+
+
+class AddHrmLegalEntityResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: AddHrmLegalEntityResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = AddHrmLegalEntityResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class AddHrmLegalEntityResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AddHrmLegalEntityResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AddHrmLegalEntityResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AddHrmPreentryHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -7104,14 +7592,721 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SyncTaskTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateHrmLegalEntityNameHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UpdateHrmLegalEntityNameRequest(TeaModel):
+    def __init__(
+        self,
+        ding_tenant_id: int = None,
+        legal_entity_name: str = None,
+        origin_legal_entity_name: str = None,
+    ):
+        self.ding_tenant_id = ding_tenant_id
+        # This parameter is required.
+        self.legal_entity_name = legal_entity_name
+        # This parameter is required.
+        self.origin_legal_entity_name = origin_legal_entity_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ding_tenant_id is not None:
+            result['dingTenantId'] = self.ding_tenant_id
+        if self.legal_entity_name is not None:
+            result['legalEntityName'] = self.legal_entity_name
+        if self.origin_legal_entity_name is not None:
+            result['originLegalEntityName'] = self.origin_legal_entity_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('dingTenantId') is not None:
+            self.ding_tenant_id = m.get('dingTenantId')
+        if m.get('legalEntityName') is not None:
+            self.legal_entity_name = m.get('legalEntityName')
+        if m.get('originLegalEntityName') is not None:
+            self.origin_legal_entity_name = m.get('originLegalEntityName')
+        return self
+
+
+class UpdateHrmLegalEntityNameResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        gmt_create: int = None,
+        gmt_modified: int = None,
+        legal_entity_id: str = None,
+        legal_entity_name: str = None,
+        legal_entity_short_name: str = None,
+        legal_entity_status: int = None,
+        legal_person_name: str = None,
+    ):
+        self.corp_id = corp_id
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.legal_entity_id = legal_entity_id
+        self.legal_entity_name = legal_entity_name
+        self.legal_entity_short_name = legal_entity_short_name
+        self.legal_entity_status = legal_entity_status
+        self.legal_person_name = legal_person_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.gmt_create is not None:
+            result['gmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['gmtModified'] = self.gmt_modified
+        if self.legal_entity_id is not None:
+            result['legalEntityId'] = self.legal_entity_id
+        if self.legal_entity_name is not None:
+            result['legalEntityName'] = self.legal_entity_name
+        if self.legal_entity_short_name is not None:
+            result['legalEntityShortName'] = self.legal_entity_short_name
+        if self.legal_entity_status is not None:
+            result['legalEntityStatus'] = self.legal_entity_status
+        if self.legal_person_name is not None:
+            result['legalPersonName'] = self.legal_person_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('gmtCreate') is not None:
+            self.gmt_create = m.get('gmtCreate')
+        if m.get('gmtModified') is not None:
+            self.gmt_modified = m.get('gmtModified')
+        if m.get('legalEntityId') is not None:
+            self.legal_entity_id = m.get('legalEntityId')
+        if m.get('legalEntityName') is not None:
+            self.legal_entity_name = m.get('legalEntityName')
+        if m.get('legalEntityShortName') is not None:
+            self.legal_entity_short_name = m.get('legalEntityShortName')
+        if m.get('legalEntityStatus') is not None:
+            self.legal_entity_status = m.get('legalEntityStatus')
+        if m.get('legalPersonName') is not None:
+            self.legal_person_name = m.get('legalPersonName')
+        return self
+
+
+class UpdateHrmLegalEntityNameResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: UpdateHrmLegalEntityNameResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = UpdateHrmLegalEntityNameResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class UpdateHrmLegalEntityNameResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateHrmLegalEntityNameResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateHrmLegalEntityNameResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameRequestExtManageAddress(TeaModel):
+    def __init__(
+        self,
+        area_code: str = None,
+        area_name: str = None,
+        city_code: str = None,
+        city_name: str = None,
+        country_code: str = None,
+        country_name: str = None,
+        detail_address: str = None,
+        global_area_type: str = None,
+        province_code: str = None,
+        province_name: str = None,
+    ):
+        self.area_code = area_code
+        self.area_name = area_name
+        self.city_code = city_code
+        self.city_name = city_name
+        self.country_code = country_code
+        self.country_name = country_name
+        self.detail_address = detail_address
+        self.global_area_type = global_area_type
+        self.province_code = province_code
+        self.province_name = province_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.area_code is not None:
+            result['areaCode'] = self.area_code
+        if self.area_name is not None:
+            result['areaName'] = self.area_name
+        if self.city_code is not None:
+            result['cityCode'] = self.city_code
+        if self.city_name is not None:
+            result['cityName'] = self.city_name
+        if self.country_code is not None:
+            result['countryCode'] = self.country_code
+        if self.country_name is not None:
+            result['countryName'] = self.country_name
+        if self.detail_address is not None:
+            result['detailAddress'] = self.detail_address
+        if self.global_area_type is not None:
+            result['globalAreaType'] = self.global_area_type
+        if self.province_code is not None:
+            result['provinceCode'] = self.province_code
+        if self.province_name is not None:
+            result['provinceName'] = self.province_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('areaCode') is not None:
+            self.area_code = m.get('areaCode')
+        if m.get('areaName') is not None:
+            self.area_name = m.get('areaName')
+        if m.get('cityCode') is not None:
+            self.city_code = m.get('cityCode')
+        if m.get('cityName') is not None:
+            self.city_name = m.get('cityName')
+        if m.get('countryCode') is not None:
+            self.country_code = m.get('countryCode')
+        if m.get('countryName') is not None:
+            self.country_name = m.get('countryName')
+        if m.get('detailAddress') is not None:
+            self.detail_address = m.get('detailAddress')
+        if m.get('globalAreaType') is not None:
+            self.global_area_type = m.get('globalAreaType')
+        if m.get('provinceCode') is not None:
+            self.province_code = m.get('provinceCode')
+        if m.get('provinceName') is not None:
+            self.province_name = m.get('provinceName')
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameRequestExtRegistrationAddress(TeaModel):
+    def __init__(
+        self,
+        area_code: str = None,
+        area_name: str = None,
+        city_code: str = None,
+        city_name: str = None,
+        country_code: str = None,
+        country_name: str = None,
+        detail_address: str = None,
+        global_area_type: str = None,
+        province_code: str = None,
+        province_name: str = None,
+    ):
+        self.area_code = area_code
+        self.area_name = area_name
+        self.city_code = city_code
+        self.city_name = city_name
+        self.country_code = country_code
+        self.country_name = country_name
+        self.detail_address = detail_address
+        self.global_area_type = global_area_type
+        self.province_code = province_code
+        self.province_name = province_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.area_code is not None:
+            result['areaCode'] = self.area_code
+        if self.area_name is not None:
+            result['areaName'] = self.area_name
+        if self.city_code is not None:
+            result['cityCode'] = self.city_code
+        if self.city_name is not None:
+            result['cityName'] = self.city_name
+        if self.country_code is not None:
+            result['countryCode'] = self.country_code
+        if self.country_name is not None:
+            result['countryName'] = self.country_name
+        if self.detail_address is not None:
+            result['detailAddress'] = self.detail_address
+        if self.global_area_type is not None:
+            result['globalAreaType'] = self.global_area_type
+        if self.province_code is not None:
+            result['provinceCode'] = self.province_code
+        if self.province_name is not None:
+            result['provinceName'] = self.province_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('areaCode') is not None:
+            self.area_code = m.get('areaCode')
+        if m.get('areaName') is not None:
+            self.area_name = m.get('areaName')
+        if m.get('cityCode') is not None:
+            self.city_code = m.get('cityCode')
+        if m.get('cityName') is not None:
+            self.city_name = m.get('cityName')
+        if m.get('countryCode') is not None:
+            self.country_code = m.get('countryCode')
+        if m.get('countryName') is not None:
+            self.country_name = m.get('countryName')
+        if m.get('detailAddress') is not None:
+            self.detail_address = m.get('detailAddress')
+        if m.get('globalAreaType') is not None:
+            self.global_area_type = m.get('globalAreaType')
+        if m.get('provinceCode') is not None:
+            self.province_code = m.get('provinceCode')
+        if m.get('provinceName') is not None:
+            self.province_name = m.get('provinceName')
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameRequestExt(TeaModel):
+    def __init__(
+        self,
+        legal_entity_en_name: str = None,
+        legal_entity_en_short_name: str = None,
+        legal_entity_type: str = None,
+        manage_address: UpdateHrmLegalEntityWithoutNameRequestExtManageAddress = None,
+        registration_address: UpdateHrmLegalEntityWithoutNameRequestExtRegistrationAddress = None,
+        registration_date: int = None,
+        unified_social_credit_code: str = None,
+        zip_code: str = None,
+    ):
+        self.legal_entity_en_name = legal_entity_en_name
+        self.legal_entity_en_short_name = legal_entity_en_short_name
+        self.legal_entity_type = legal_entity_type
+        self.manage_address = manage_address
+        self.registration_address = registration_address
+        self.registration_date = registration_date
+        self.unified_social_credit_code = unified_social_credit_code
+        self.zip_code = zip_code
+
+    def validate(self):
+        if self.manage_address:
+            self.manage_address.validate()
+        if self.registration_address:
+            self.registration_address.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.legal_entity_en_name is not None:
+            result['legalEntityEnName'] = self.legal_entity_en_name
+        if self.legal_entity_en_short_name is not None:
+            result['legalEntityEnShortName'] = self.legal_entity_en_short_name
+        if self.legal_entity_type is not None:
+            result['legalEntityType'] = self.legal_entity_type
+        if self.manage_address is not None:
+            result['manageAddress'] = self.manage_address.to_map()
+        if self.registration_address is not None:
+            result['registrationAddress'] = self.registration_address.to_map()
+        if self.registration_date is not None:
+            result['registrationDate'] = self.registration_date
+        if self.unified_social_credit_code is not None:
+            result['unifiedSocialCreditCode'] = self.unified_social_credit_code
+        if self.zip_code is not None:
+            result['zipCode'] = self.zip_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('legalEntityEnName') is not None:
+            self.legal_entity_en_name = m.get('legalEntityEnName')
+        if m.get('legalEntityEnShortName') is not None:
+            self.legal_entity_en_short_name = m.get('legalEntityEnShortName')
+        if m.get('legalEntityType') is not None:
+            self.legal_entity_type = m.get('legalEntityType')
+        if m.get('manageAddress') is not None:
+            temp_model = UpdateHrmLegalEntityWithoutNameRequestExtManageAddress()
+            self.manage_address = temp_model.from_map(m['manageAddress'])
+        if m.get('registrationAddress') is not None:
+            temp_model = UpdateHrmLegalEntityWithoutNameRequestExtRegistrationAddress()
+            self.registration_address = temp_model.from_map(m['registrationAddress'])
+        if m.get('registrationDate') is not None:
+            self.registration_date = m.get('registrationDate')
+        if m.get('unifiedSocialCreditCode') is not None:
+            self.unified_social_credit_code = m.get('unifiedSocialCreditCode')
+        if m.get('zipCode') is not None:
+            self.zip_code = m.get('zipCode')
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameRequest(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        create_user_id: str = None,
+        ext: UpdateHrmLegalEntityWithoutNameRequestExt = None,
+        legal_entity_name: str = None,
+        legal_entity_short_name: str = None,
+        legal_entity_status: int = None,
+        legal_person_name: str = None,
+        ding_tenant_id: int = None,
+    ):
+        # This parameter is required.
+        self.corp_id = corp_id
+        self.create_user_id = create_user_id
+        self.ext = ext
+        # This parameter is required.
+        self.legal_entity_name = legal_entity_name
+        self.legal_entity_short_name = legal_entity_short_name
+        # This parameter is required.
+        self.legal_entity_status = legal_entity_status
+        self.legal_person_name = legal_person_name
+        self.ding_tenant_id = ding_tenant_id
+
+    def validate(self):
+        if self.ext:
+            self.ext.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.create_user_id is not None:
+            result['createUserId'] = self.create_user_id
+        if self.ext is not None:
+            result['ext'] = self.ext.to_map()
+        if self.legal_entity_name is not None:
+            result['legalEntityName'] = self.legal_entity_name
+        if self.legal_entity_short_name is not None:
+            result['legalEntityShortName'] = self.legal_entity_short_name
+        if self.legal_entity_status is not None:
+            result['legalEntityStatus'] = self.legal_entity_status
+        if self.legal_person_name is not None:
+            result['legalPersonName'] = self.legal_person_name
+        if self.ding_tenant_id is not None:
+            result['dingTenantId'] = self.ding_tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('createUserId') is not None:
+            self.create_user_id = m.get('createUserId')
+        if m.get('ext') is not None:
+            temp_model = UpdateHrmLegalEntityWithoutNameRequestExt()
+            self.ext = temp_model.from_map(m['ext'])
+        if m.get('legalEntityName') is not None:
+            self.legal_entity_name = m.get('legalEntityName')
+        if m.get('legalEntityShortName') is not None:
+            self.legal_entity_short_name = m.get('legalEntityShortName')
+        if m.get('legalEntityStatus') is not None:
+            self.legal_entity_status = m.get('legalEntityStatus')
+        if m.get('legalPersonName') is not None:
+            self.legal_person_name = m.get('legalPersonName')
+        if m.get('dingTenantId') is not None:
+            self.ding_tenant_id = m.get('dingTenantId')
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        gmt_create: int = None,
+        gmt_modified: int = None,
+        legal_entity_id: str = None,
+        legal_entity_name: str = None,
+        legal_entity_short_name: str = None,
+        legal_entity_status: int = None,
+        legal_person_name: str = None,
+    ):
+        self.corp_id = corp_id
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.legal_entity_id = legal_entity_id
+        self.legal_entity_name = legal_entity_name
+        self.legal_entity_short_name = legal_entity_short_name
+        self.legal_entity_status = legal_entity_status
+        self.legal_person_name = legal_person_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.gmt_create is not None:
+            result['gmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['gmtModified'] = self.gmt_modified
+        if self.legal_entity_id is not None:
+            result['legalEntityId'] = self.legal_entity_id
+        if self.legal_entity_name is not None:
+            result['legalEntityName'] = self.legal_entity_name
+        if self.legal_entity_short_name is not None:
+            result['legalEntityShortName'] = self.legal_entity_short_name
+        if self.legal_entity_status is not None:
+            result['legalEntityStatus'] = self.legal_entity_status
+        if self.legal_person_name is not None:
+            result['legalPersonName'] = self.legal_person_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('gmtCreate') is not None:
+            self.gmt_create = m.get('gmtCreate')
+        if m.get('gmtModified') is not None:
+            self.gmt_modified = m.get('gmtModified')
+        if m.get('legalEntityId') is not None:
+            self.legal_entity_id = m.get('legalEntityId')
+        if m.get('legalEntityName') is not None:
+            self.legal_entity_name = m.get('legalEntityName')
+        if m.get('legalEntityShortName') is not None:
+            self.legal_entity_short_name = m.get('legalEntityShortName')
+        if m.get('legalEntityStatus') is not None:
+            self.legal_entity_status = m.get('legalEntityStatus')
+        if m.get('legalPersonName') is not None:
+            self.legal_person_name = m.get('legalPersonName')
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: UpdateHrmLegalEntityWithoutNameResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = UpdateHrmLegalEntityWithoutNameResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class UpdateHrmLegalEntityWithoutNameResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateHrmLegalEntityWithoutNameResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateHrmLegalEntityWithoutNameResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateIsvCardMessageHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -889,14 +889,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateIntegratedTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.activity_id):
             body['activityId'] = request.activity_id
+        if not UtilClient.is_unset(request.feature_config):
+            body['featureConfig'] = request.feature_config
         if not UtilClient.is_unset(request.process_instance_id):
             body['processInstanceId'] = request.process_instance_id
         if not UtilClient.is_unset(request.tasks):
             body['tasks'] = request.tasks
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -936,14 +938,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateIntegratedTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.activity_id):
             body['activityId'] = request.activity_id
+        if not UtilClient.is_unset(request.feature_config):
+            body['featureConfig'] = request.feature_config
         if not UtilClient.is_unset(request.process_instance_id):
             body['processInstanceId'] = request.process_instance_id
         if not UtilClient.is_unset(request.tasks):
             body['tasks'] = request.tasks
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -993,14 +997,132 @@
         @param request: CreateIntegratedTaskRequest
         @return: CreateIntegratedTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkworkflow__1__0_models.CreateIntegratedTaskHeaders()
         return await self.create_integrated_task_with_options_async(request, headers, runtime)
 
+    def delete_dir_with_options(
+        self,
+        request: dingtalkworkflow__1__0_models.DeleteDirRequest,
+        headers: dingtalkworkflow__1__0_models.DeleteDirHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.DeleteDirResponse:
+        """
+        @summary 删除分组
+        
+        @param request: DeleteDirRequest
+        @param headers: DeleteDirHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDirResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dir_id):
+            query['dirId'] = request.dir_id
+        if not UtilClient.is_unset(request.operate_user_id):
+            query['operateUserId'] = request.operate_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDir',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processCentres/directories',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.DeleteDirResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def delete_dir_with_options_async(
+        self,
+        request: dingtalkworkflow__1__0_models.DeleteDirRequest,
+        headers: dingtalkworkflow__1__0_models.DeleteDirHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.DeleteDirResponse:
+        """
+        @summary 删除分组
+        
+        @param request: DeleteDirRequest
+        @param headers: DeleteDirHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDirResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dir_id):
+            query['dirId'] = request.dir_id
+        if not UtilClient.is_unset(request.operate_user_id):
+            query['operateUserId'] = request.operate_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDir',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processCentres/directories',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.DeleteDirResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def delete_dir(
+        self,
+        request: dingtalkworkflow__1__0_models.DeleteDirRequest,
+    ) -> dingtalkworkflow__1__0_models.DeleteDirResponse:
+        """
+        @summary 删除分组
+        
+        @param request: DeleteDirRequest
+        @return: DeleteDirResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.DeleteDirHeaders()
+        return self.delete_dir_with_options(request, headers, runtime)
+
+    async def delete_dir_async(
+        self,
+        request: dingtalkworkflow__1__0_models.DeleteDirRequest,
+    ) -> dingtalkworkflow__1__0_models.DeleteDirResponse:
+        """
+        @summary 删除分组
+        
+        @param request: DeleteDirRequest
+        @return: DeleteDirResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.DeleteDirHeaders()
+        return await self.delete_dir_with_options_async(request, headers, runtime)
+
     def delete_process_with_options(
         self,
         request: dingtalkworkflow__1__0_models.DeleteProcessRequest,
         headers: dingtalkworkflow__1__0_models.DeleteProcessHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkworkflow__1__0_models.DeleteProcessResponse:
         """
@@ -2887,14 +3009,144 @@
         @param request: GrantProcessInstanceForDownloadFileRequest
         @return: GrantProcessInstanceForDownloadFileResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkworkflow__1__0_models.GrantProcessInstanceForDownloadFileHeaders()
         return await self.grant_process_instance_for_download_file_with_options_async(request, headers, runtime)
 
+    def insert_or_update_dir_with_options(
+        self,
+        request: dingtalkworkflow__1__0_models.InsertOrUpdateDirRequest,
+        headers: dingtalkworkflow__1__0_models.InsertOrUpdateDirHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.InsertOrUpdateDirResponse:
+        """
+        @summary 创建或更新分组
+        
+        @param request: InsertOrUpdateDirRequest
+        @param headers: InsertOrUpdateDirHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: InsertOrUpdateDirResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.biz_group):
+            body['bizGroup'] = request.biz_group
+        if not UtilClient.is_unset(request.description):
+            body['description'] = request.description
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
+        if not UtilClient.is_unset(request.name_18n):
+            body['name18n'] = request.name_18n
+        if not UtilClient.is_unset(request.operate_user_id):
+            body['operateUserId'] = request.operate_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='InsertOrUpdateDir',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processCentres/directories',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.InsertOrUpdateDirResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def insert_or_update_dir_with_options_async(
+        self,
+        request: dingtalkworkflow__1__0_models.InsertOrUpdateDirRequest,
+        headers: dingtalkworkflow__1__0_models.InsertOrUpdateDirHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.InsertOrUpdateDirResponse:
+        """
+        @summary 创建或更新分组
+        
+        @param request: InsertOrUpdateDirRequest
+        @param headers: InsertOrUpdateDirHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: InsertOrUpdateDirResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.biz_group):
+            body['bizGroup'] = request.biz_group
+        if not UtilClient.is_unset(request.description):
+            body['description'] = request.description
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
+        if not UtilClient.is_unset(request.name_18n):
+            body['name18n'] = request.name_18n
+        if not UtilClient.is_unset(request.operate_user_id):
+            body['operateUserId'] = request.operate_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='InsertOrUpdateDir',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processCentres/directories',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.InsertOrUpdateDirResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def insert_or_update_dir(
+        self,
+        request: dingtalkworkflow__1__0_models.InsertOrUpdateDirRequest,
+    ) -> dingtalkworkflow__1__0_models.InsertOrUpdateDirResponse:
+        """
+        @summary 创建或更新分组
+        
+        @param request: InsertOrUpdateDirRequest
+        @return: InsertOrUpdateDirResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.InsertOrUpdateDirHeaders()
+        return self.insert_or_update_dir_with_options(request, headers, runtime)
+
+    async def insert_or_update_dir_async(
+        self,
+        request: dingtalkworkflow__1__0_models.InsertOrUpdateDirRequest,
+    ) -> dingtalkworkflow__1__0_models.InsertOrUpdateDirResponse:
+        """
+        @summary 创建或更新分组
+        
+        @param request: InsertOrUpdateDirRequest
+        @return: InsertOrUpdateDirResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.InsertOrUpdateDirHeaders()
+        return await self.insert_or_update_dir_with_options_async(request, headers, runtime)
+
     def install_app_with_options(
         self,
         request: dingtalkworkflow__1__0_models.InstallAppRequest,
         headers: dingtalkworkflow__1__0_models.InstallAppHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkworkflow__1__0_models.InstallAppResponse:
         """
@@ -4791,14 +5043,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: SaveIntegratedInstanceResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.biz_data):
             body['bizData'] = request.biz_data
+        if not UtilClient.is_unset(request.feature_config):
+            body['featureConfig'] = request.feature_config
         if not UtilClient.is_unset(request.form_component_value_list):
             body['formComponentValueList'] = request.form_component_value_list
         if not UtilClient.is_unset(request.notifiers):
             body['notifiers'] = request.notifiers
         if not UtilClient.is_unset(request.originator_user_id):
             body['originatorUserId'] = request.originator_user_id
         if not UtilClient.is_unset(request.process_code):
@@ -4846,14 +5100,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: SaveIntegratedInstanceResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.biz_data):
             body['bizData'] = request.biz_data
+        if not UtilClient.is_unset(request.feature_config):
+            body['featureConfig'] = request.feature_config
         if not UtilClient.is_unset(request.form_component_value_list):
             body['formComponentValueList'] = request.form_component_value_list
         if not UtilClient.is_unset(request.notifiers):
             body['notifiers'] = request.notifiers
         if not UtilClient.is_unset(request.originator_user_id):
             body['originatorUserId'] = request.originator_user_id
         if not UtilClient.is_unset(request.process_code):
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1968,14 +1968,147 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
+class CreateIntegratedTaskRequestFeatureConfigFeaturesCallback(TeaModel):
+    def __init__(
+        self,
+        api_key: str = None,
+        app_uuid: str = None,
+        version: str = None,
+    ):
+        self.api_key = api_key
+        self.app_uuid = app_uuid
+        self.version = version
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_key is not None:
+            result['apiKey'] = self.api_key
+        if self.app_uuid is not None:
+            result['appUuid'] = self.app_uuid
+        if self.version is not None:
+            result['version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('apiKey') is not None:
+            self.api_key = m.get('apiKey')
+        if m.get('appUuid') is not None:
+            self.app_uuid = m.get('appUuid')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        return self
+
+
+class CreateIntegratedTaskRequestFeatureConfigFeatures(TeaModel):
+    def __init__(
+        self,
+        callback: CreateIntegratedTaskRequestFeatureConfigFeaturesCallback = None,
+        config: str = None,
+        mobile_url: str = None,
+        name: str = None,
+        pc_url: str = None,
+        run_type: str = None,
+    ):
+        self.callback = callback
+        self.config = config
+        self.mobile_url = mobile_url
+        self.name = name
+        self.pc_url = pc_url
+        self.run_type = run_type
+
+    def validate(self):
+        if self.callback:
+            self.callback.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.callback is not None:
+            result['callback'] = self.callback.to_map()
+        if self.config is not None:
+            result['config'] = self.config
+        if self.mobile_url is not None:
+            result['mobileUrl'] = self.mobile_url
+        if self.name is not None:
+            result['name'] = self.name
+        if self.pc_url is not None:
+            result['pcUrl'] = self.pc_url
+        if self.run_type is not None:
+            result['runType'] = self.run_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('callback') is not None:
+            temp_model = CreateIntegratedTaskRequestFeatureConfigFeaturesCallback()
+            self.callback = temp_model.from_map(m['callback'])
+        if m.get('config') is not None:
+            self.config = m.get('config')
+        if m.get('mobileUrl') is not None:
+            self.mobile_url = m.get('mobileUrl')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('pcUrl') is not None:
+            self.pc_url = m.get('pcUrl')
+        if m.get('runType') is not None:
+            self.run_type = m.get('runType')
+        return self
+
+
+class CreateIntegratedTaskRequestFeatureConfig(TeaModel):
+    def __init__(
+        self,
+        features: List[CreateIntegratedTaskRequestFeatureConfigFeatures] = None,
+    ):
+        self.features = features
+
+    def validate(self):
+        if self.features:
+            for k in self.features:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['features'] = []
+        if self.features is not None:
+            for k in self.features:
+                result['features'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.features = []
+        if m.get('features') is not None:
+            for k in m.get('features'):
+                temp_model = CreateIntegratedTaskRequestFeatureConfigFeatures()
+                self.features.append(temp_model.from_map(k))
+        return self
+
+
 class CreateIntegratedTaskRequestTasks(TeaModel):
     def __init__(
         self,
         custom_data: str = None,
         url: str = None,
         user_id: str = None,
     ):
@@ -2011,49 +2144,58 @@
         return self
 
 
 class CreateIntegratedTaskRequest(TeaModel):
     def __init__(
         self,
         activity_id: str = None,
+        feature_config: CreateIntegratedTaskRequestFeatureConfig = None,
         process_instance_id: str = None,
         tasks: List[CreateIntegratedTaskRequestTasks] = None,
     ):
         self.activity_id = activity_id
+        self.feature_config = feature_config
         # This parameter is required.
         self.process_instance_id = process_instance_id
         # This parameter is required.
         self.tasks = tasks
 
     def validate(self):
+        if self.feature_config:
+            self.feature_config.validate()
         if self.tasks:
             for k in self.tasks:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.activity_id is not None:
             result['activityId'] = self.activity_id
+        if self.feature_config is not None:
+            result['featureConfig'] = self.feature_config.to_map()
         if self.process_instance_id is not None:
             result['processInstanceId'] = self.process_instance_id
         result['tasks'] = []
         if self.tasks is not None:
             for k in self.tasks:
                 result['tasks'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('activityId') is not None:
             self.activity_id = m.get('activityId')
+        if m.get('featureConfig') is not None:
+            temp_model = CreateIntegratedTaskRequestFeatureConfig()
+            self.feature_config = temp_model.from_map(m['featureConfig'])
         if m.get('processInstanceId') is not None:
             self.process_instance_id = m.get('processInstanceId')
         self.tasks = []
         if m.get('tasks') is not None:
             for k in m.get('tasks'):
                 temp_model = CreateIntegratedTaskRequestTasks()
                 self.tasks.append(temp_model.from_map(k))
@@ -2171,14 +2313,150 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateIntegratedTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteDirHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class DeleteDirRequest(TeaModel):
+    def __init__(
+        self,
+        dir_id: str = None,
+        operate_user_id: str = None,
+    ):
+        # This parameter is required.
+        self.dir_id = dir_id
+        # This parameter is required.
+        self.operate_user_id = operate_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dir_id is not None:
+            result['dirId'] = self.dir_id
+        if self.operate_user_id is not None:
+            result['operateUserId'] = self.operate_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('dirId') is not None:
+            self.dir_id = m.get('dirId')
+        if m.get('operateUserId') is not None:
+            self.operate_user_id = m.get('operateUserId')
+        return self
+
+
+class DeleteDirResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class DeleteDirResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteDirResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteDirResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteProcessHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -5825,14 +6103,211 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GrantProcessInstanceForDownloadFileResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class InsertOrUpdateDirHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class InsertOrUpdateDirRequest(TeaModel):
+    def __init__(
+        self,
+        biz_group: str = None,
+        description: str = None,
+        name: str = None,
+        name_18n: str = None,
+        operate_user_id: str = None,
+    ):
+        # This parameter is required.
+        self.biz_group = biz_group
+        self.description = description
+        # This parameter is required.
+        self.name = name
+        # This parameter is required.
+        self.name_18n = name_18n
+        # This parameter is required.
+        self.operate_user_id = operate_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_group is not None:
+            result['bizGroup'] = self.biz_group
+        if self.description is not None:
+            result['description'] = self.description
+        if self.name is not None:
+            result['name'] = self.name
+        if self.name_18n is not None:
+            result['name18n'] = self.name_18n
+        if self.operate_user_id is not None:
+            result['operateUserId'] = self.operate_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizGroup') is not None:
+            self.biz_group = m.get('bizGroup')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('name18n') is not None:
+            self.name_18n = m.get('name18n')
+        if m.get('operateUserId') is not None:
+            self.operate_user_id = m.get('operateUserId')
+        return self
+
+
+class InsertOrUpdateDirResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        biz_group: str = None,
+        dir_id: str = None,
+    ):
+        self.biz_group = biz_group
+        self.dir_id = dir_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_group is not None:
+            result['bizGroup'] = self.biz_group
+        if self.dir_id is not None:
+            result['dirId'] = self.dir_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizGroup') is not None:
+            self.biz_group = m.get('bizGroup')
+        if m.get('dirId') is not None:
+            self.dir_id = m.get('dirId')
+        return self
+
+
+class InsertOrUpdateDirResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: InsertOrUpdateDirResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = InsertOrUpdateDirResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class InsertOrUpdateDirResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: InsertOrUpdateDirResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = InsertOrUpdateDirResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class InstallAppHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -11528,14 +12003,147 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
+class SaveIntegratedInstanceRequestFeatureConfigFeaturesCallback(TeaModel):
+    def __init__(
+        self,
+        api_key: str = None,
+        app_uuid: str = None,
+        version: str = None,
+    ):
+        self.api_key = api_key
+        self.app_uuid = app_uuid
+        self.version = version
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_key is not None:
+            result['apiKey'] = self.api_key
+        if self.app_uuid is not None:
+            result['appUuid'] = self.app_uuid
+        if self.version is not None:
+            result['version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('apiKey') is not None:
+            self.api_key = m.get('apiKey')
+        if m.get('appUuid') is not None:
+            self.app_uuid = m.get('appUuid')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        return self
+
+
+class SaveIntegratedInstanceRequestFeatureConfigFeatures(TeaModel):
+    def __init__(
+        self,
+        callback: SaveIntegratedInstanceRequestFeatureConfigFeaturesCallback = None,
+        config: str = None,
+        mobile_url: str = None,
+        name: str = None,
+        pc_url: str = None,
+        run_type: str = None,
+    ):
+        self.callback = callback
+        self.config = config
+        self.mobile_url = mobile_url
+        self.name = name
+        self.pc_url = pc_url
+        self.run_type = run_type
+
+    def validate(self):
+        if self.callback:
+            self.callback.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.callback is not None:
+            result['callback'] = self.callback.to_map()
+        if self.config is not None:
+            result['config'] = self.config
+        if self.mobile_url is not None:
+            result['mobileUrl'] = self.mobile_url
+        if self.name is not None:
+            result['name'] = self.name
+        if self.pc_url is not None:
+            result['pcUrl'] = self.pc_url
+        if self.run_type is not None:
+            result['runType'] = self.run_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('callback') is not None:
+            temp_model = SaveIntegratedInstanceRequestFeatureConfigFeaturesCallback()
+            self.callback = temp_model.from_map(m['callback'])
+        if m.get('config') is not None:
+            self.config = m.get('config')
+        if m.get('mobileUrl') is not None:
+            self.mobile_url = m.get('mobileUrl')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('pcUrl') is not None:
+            self.pc_url = m.get('pcUrl')
+        if m.get('runType') is not None:
+            self.run_type = m.get('runType')
+        return self
+
+
+class SaveIntegratedInstanceRequestFeatureConfig(TeaModel):
+    def __init__(
+        self,
+        features: List[SaveIntegratedInstanceRequestFeatureConfigFeatures] = None,
+    ):
+        self.features = features
+
+    def validate(self):
+        if self.features:
+            for k in self.features:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['features'] = []
+        if self.features is not None:
+            for k in self.features:
+                result['features'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.features = []
+        if m.get('features') is not None:
+            for k in m.get('features'):
+                temp_model = SaveIntegratedInstanceRequestFeatureConfigFeatures()
+                self.features.append(temp_model.from_map(k))
+        return self
+
+
 class SaveIntegratedInstanceRequestFormComponentValueList(TeaModel):
     def __init__(
         self,
         biz_alias: str = None,
         component_type: str = None,
         ext_value: str = None,
         id: str = None,
@@ -11622,33 +12230,37 @@
         return self
 
 
 class SaveIntegratedInstanceRequest(TeaModel):
     def __init__(
         self,
         biz_data: str = None,
+        feature_config: SaveIntegratedInstanceRequestFeatureConfig = None,
         form_component_value_list: List[SaveIntegratedInstanceRequestFormComponentValueList] = None,
         notifiers: List[SaveIntegratedInstanceRequestNotifiers] = None,
         originator_user_id: str = None,
         process_code: str = None,
         title: str = None,
         url: str = None,
     ):
         self.biz_data = biz_data
+        self.feature_config = feature_config
         self.form_component_value_list = form_component_value_list
         self.notifiers = notifiers
         # This parameter is required.
         self.originator_user_id = originator_user_id
         # This parameter is required.
         self.process_code = process_code
         self.title = title
         # This parameter is required.
         self.url = url
 
     def validate(self):
+        if self.feature_config:
+            self.feature_config.validate()
         if self.form_component_value_list:
             for k in self.form_component_value_list:
                 if k:
                     k.validate()
         if self.notifiers:
             for k in self.notifiers:
                 if k:
@@ -11658,14 +12270,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.biz_data is not None:
             result['bizData'] = self.biz_data
+        if self.feature_config is not None:
+            result['featureConfig'] = self.feature_config.to_map()
         result['formComponentValueList'] = []
         if self.form_component_value_list is not None:
             for k in self.form_component_value_list:
                 result['formComponentValueList'].append(k.to_map() if k else None)
         result['notifiers'] = []
         if self.notifiers is not None:
             for k in self.notifiers:
@@ -11680,14 +12294,17 @@
             result['url'] = self.url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('bizData') is not None:
             self.biz_data = m.get('bizData')
+        if m.get('featureConfig') is not None:
+            temp_model = SaveIntegratedInstanceRequestFeatureConfig()
+            self.feature_config = temp_model.from_map(m['featureConfig'])
         self.form_component_value_list = []
         if m.get('formComponentValueList') is not None:
             for k in m.get('formComponentValueList'):
                 temp_model = SaveIntegratedInstanceRequestFormComponentValueList()
                 self.form_component_value_list.append(temp_model.from_map(k))
         self.notifiers = []
         if m.get('notifiers') is not None:
@@ -11874,20 +12491,22 @@
         return self
 
 
 class SaveProcessRequestProcessFeatureConfigFeatures(TeaModel):
     def __init__(
         self,
         callback: SaveProcessRequestProcessFeatureConfigFeaturesCallback = None,
+        config: str = None,
         mobile_url: str = None,
         name: str = None,
         pc_url: str = None,
         run_type: str = None,
     ):
         self.callback = callback
+        self.config = config
         self.mobile_url = mobile_url
         self.name = name
         self.pc_url = pc_url
         self.run_type = run_type
 
     def validate(self):
         if self.callback:
@@ -11897,14 +12516,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.callback is not None:
             result['callback'] = self.callback.to_map()
+        if self.config is not None:
+            result['config'] = self.config
         if self.mobile_url is not None:
             result['mobileUrl'] = self.mobile_url
         if self.name is not None:
             result['name'] = self.name
         if self.pc_url is not None:
             result['pcUrl'] = self.pc_url
         if self.run_type is not None:
@@ -11912,14 +12533,16 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('callback') is not None:
             temp_model = SaveProcessRequestProcessFeatureConfigFeaturesCallback()
             self.callback = temp_model.from_map(m['callback'])
+        if m.get('config') is not None:
+            self.config = m.get('config')
         if m.get('mobileUrl') is not None:
             self.mobile_url = m.get('mobileUrl')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('pcUrl') is not None:
             self.pc_url = m.get('pcUrl')
         if m.get('runType') is not None:
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.1.11
+Version: 2.1.12
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.11/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.1.12/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.11/setup.py` & `alibabacloud_dingtalk-2.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 14/05/2024
+Created on 18/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```


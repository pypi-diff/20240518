# Comparing `tmp/dfiq-0.0.1.tar.gz` & `tmp/dfiq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfiq-0.0.1.tar", last modified: Sat Nov  5 19:48:09 2022, max compression
+gzip compressed data, was "dfiq-1.0.1.tar", last modified: Fri May 17 23:42:23 2024, max compression
```

## Comparing `dfiq-0.0.1.tar` & `dfiq-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,225 @@
-drwxrwxrwx   0        0        0        0 2022-11-05 19:48:09.154930 dfiq-0.0.1/
--rw-rw-rw-   0        0        0       51 2022-11-05 19:48:09.153932 dfiq-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      166 2022-11-05 19:42:50.000000 dfiq-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-05 19:48:09.154930 dfiq-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-05 19:48:09.139939 dfiq-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-11-05 19:48:09.141939 dfiq-0.0.1/src/dfiq/
--rw-rw-rw-   0        0        0        0 2022-11-05 19:31:55.000000 dfiq-0.0.1/src/dfiq/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-05 19:48:09.152945 dfiq-0.0.1/src/dfiq.egg-info/
--rw-rw-rw-   0        0        0       51 2022-11-05 19:48:09.000000 dfiq-0.0.1/src/dfiq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2022-11-05 19:48:09.000000 dfiq-0.0.1/src/dfiq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-05 19:48:09.000000 dfiq-0.0.1/src/dfiq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-11-05 19:48:09.000000 dfiq-0.0.1/src/dfiq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.408247 dfiq-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.368247 dfiq-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.368247 dfiq-1.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/ISSUE_TEMPLATE/1_DFIQ_Question.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/ISSUE_TEMPLATE/2_DFIQ_Facet.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/ISSUE_TEMPLATE/3_DFIQ_Scenario.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.372247 dfiq-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/workflows/code-style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-17 23:42:19.000000 dfiq-1.0.1/.github/workflows/yamale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 23:42:19.000000 dfiq-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-17 23:42:23.408247 dfiq-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-17 23:42:19.000000 dfiq-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.372247 dfiq-1.0.1/dfiq/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.368247 dfiq-1.0.1/dfiq/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.376247 dfiq-1.0.1/dfiq/data/approaches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1001.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1001.11.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1001.12.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1018.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1018.11.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1018.12.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1019.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1020.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1024.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1036.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1036.11.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1037.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1037.11.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1037.12.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1074.10.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/approaches/Q1074.11.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.380247 dfiq-1.0.1/dfiq/data/facets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1001.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1002.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1003.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1004.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1005.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1006.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1007.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1008.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1009.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1010.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1011.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1012.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1013.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1015.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1016.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1017.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1018.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1019.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1021.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1022.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1023.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1024.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1025.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1026.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1027.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1028.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1029.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/facets/F1030.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.400247 dfiq-1.0.1/dfiq/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1001.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1002.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1003.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1004.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1005.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1006.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1007.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1008.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1009.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1010.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1011.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1012.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1013.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1015.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1016.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1017.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1018.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1019.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1021.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1022.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1023.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1024.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1025.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1026.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1027.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1028.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1029.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1030.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1031.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1032.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1033.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1034.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1035.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1036.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1037.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1038.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1039.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1040.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1041.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1042.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1043.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1044.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1045.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1046.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1047.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1048.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1049.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1050.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1051.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1052.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1053.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1054.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1055.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1056.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1057.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1058.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1059.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1060.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1061.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1062.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1063.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1064.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1065.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1066.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1067.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1068.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1069.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1070.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1071.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1072.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1073.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1074.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1075.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1076.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1077.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1078.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1079.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1080.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1081.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1082.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1083.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1084.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1085.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1086.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1087.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1088.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1089.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/questions/Q1090.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.400247 dfiq-1.0.1/dfiq/data/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/scenarios/S1001.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/scenarios/S1002.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/scenarios/S1003.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/scenarios/S1005.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/scenarios/S1007.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/data/scenarios/S1008.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    25351 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/dfiq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.400247 dfiq-1.0.1/dfiq/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/scripts/generate_site_markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.400247 dfiq-1.0.1/dfiq/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/templates/approach_glossary.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/templates/question_with_approaches.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/templates/questions_index.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/templates/scenario.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.400247 dfiq-1.0.1/dfiq/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/utils/approach_spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/utils/facet_spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/utils/question_spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-17 23:42:19.000000 dfiq-1.0.1/dfiq/utils/scenario_spec.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.408247 dfiq-1.0.1/dfiq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-17 23:42:23.000000 dfiq-1.0.1/dfiq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-17 23:42:23.000000 dfiq-1.0.1/dfiq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:42:23.000000 dfiq-1.0.1/dfiq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 23:42:23.000000 dfiq-1.0.1/dfiq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 23:42:23.000000 dfiq-1.0.1/dfiq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.400247 dfiq-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-17 23:42:19.000000 dfiq-1.0.1/docs/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 23:42:19.000000 dfiq-1.0.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 23:42:19.000000 dfiq-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 23:42:19.000000 dfiq-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:42:23.408247 dfiq-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.400247 dfiq-1.0.1/site/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.404247 dfiq-1.0.1/site/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.404247 dfiq-1.0.1/site/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    39543 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/assets/dfiq-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/assets/dfiq-square.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/assets/dfiq.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.404247 dfiq-1.0.1/site/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/contributing/approach_glossary.md
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/contributing/specification.md
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.404247 dfiq-1.0.1/site/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/javascripts/tablesort.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.404247 dfiq-1.0.1/site/docs/questions/
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1001.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1018.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1019.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1020.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1024.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1036.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1037.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/Q1074.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/questions/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.408247 dfiq-1.0.1/site/docs/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/scenarios/S1001.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/scenarios/S1002.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/scenarios/S1003.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/scenarios/S1005.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/scenarios/S1007.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/scenarios/S1008.md
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/scenarios/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:42:23.408247 dfiq-1.0.1/site/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/docs/tags.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-17 23:42:19.000000 dfiq-1.0.1/site/mkdocs.yml
```


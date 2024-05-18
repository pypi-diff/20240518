# Comparing `tmp/trueseeing-2.2.2.tar.gz` & `tmp/trueseeing-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trueseeing-2.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "trueseeing-2.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `trueseeing-2.2.2.tar` & `trueseeing-2.2.4.tar`

### file list

```diff
@@ -1,84 +1,82 @@
--rw-r--r--   0        0        0       16 2023-11-26 16:54:25.486612 trueseeing-2.2.2/.dockerignore
--rw-r--r--   0        0        0     1657 2024-01-22 01:54:13.062912 trueseeing-2.2.2/.github/workflows/deploy.yaml
--rw-r--r--   0        0        0      529 2024-01-22 01:54:13.063170 trueseeing-2.2.2/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1595 2023-11-26 18:18:39.728412 trueseeing-2.2.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      841 2024-01-19 10:24:37.175838 trueseeing-2.2.2/.github/workflows/stale.yaml
--rw-r--r--   0        0        0       44 2023-11-26 01:27:36.667762 trueseeing-2.2.2/.gitignore
--rw-r--r--   0        0        0    35147 2017-07-31 13:42:43.000000 trueseeing-2.2.2/COPYING
--rw-r--r--   0        0        0     1345 2024-03-08 08:40:38.210247 trueseeing-2.2.2/Dockerfile
--rw-r--r--   0        0        0    11015 2024-03-19 19:14:28.902748 trueseeing-2.2.2/README.md
--rw-r--r--   0        0        0     1512 2024-03-19 19:14:28.902957 trueseeing-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      103 2024-03-19 19:14:28.903142 trueseeing-2.2.2/trueseeing/__init__.py
--rw-r--r--   0        0        0     9123 2024-03-19 12:42:27.434649 trueseeing-2.2.2/trueseeing/api.py
--rw-r--r--   0        0        0        0 2024-01-19 12:19:41.073814 trueseeing-2.2.2/trueseeing/app/__init__.py
--rw-r--r--   0        0        0      670 2024-02-07 08:13:53.327058 trueseeing-2.2.2/trueseeing/app/cmd/__init__.py
--rw-r--r--   0        0        0     4635 2024-02-02 13:13:46.930678 trueseeing-2.2.2/trueseeing/app/cmd/alias.py
--rw-r--r--   0        0        0     1312 2024-03-10 08:02:42.473006 trueseeing-2.2.2/trueseeing/app/cmd/analyze.py
--rw-r--r--   0        0        0        0 2024-01-31 06:00:56.916344 trueseeing-2.2.2/trueseeing/app/cmd/android/__init__.py
--rw-r--r--   0        0        0     7708 2024-03-19 12:44:48.564390 trueseeing-2.2.2/trueseeing/app/cmd/android/asm.py
--rw-r--r--   0        0        0    13537 2024-03-08 02:59:47.524321 trueseeing-2.2.2/trueseeing/app/cmd/android/device.py
--rw-r--r--   0        0        0    25841 2024-03-19 19:14:28.903555 trueseeing-2.2.2/trueseeing/app/cmd/android/exploit.py
--rw-r--r--   0        0        0     8760 2024-03-03 20:15:50.039416 trueseeing-2.2.2/trueseeing/app/cmd/android/search.py
--rw-r--r--   0        0        0     4706 2024-03-03 20:15:50.039628 trueseeing-2.2.2/trueseeing/app/cmd/android/show.py
--rw-r--r--   0        0        0     1817 2024-03-07 00:23:15.845945 trueseeing-2.2.2/trueseeing/app/cmd/config.py
--rw-r--r--   0        0        0     2134 2024-03-10 08:02:42.473442 trueseeing-2.2.2/trueseeing/app/cmd/info.py
--rw-r--r--   0        0        0     2954 2024-02-09 05:03:10.447760 trueseeing-2.2.2/trueseeing/app/cmd/report.py
--rw-r--r--   0        0        0     2486 2024-03-10 08:02:42.473752 trueseeing-2.2.2/trueseeing/app/cmd/scan.py
--rw-r--r--   0        0        0     2529 2024-02-19 20:44:58.678881 trueseeing-2.2.2/trueseeing/app/cmd/search.py
--rw-r--r--   0        0        0     1784 2024-02-19 04:58:33.651096 trueseeing-2.2.2/trueseeing/app/cmd/show.py
--rw-r--r--   0        0        0    11682 2024-03-19 19:14:28.903843 trueseeing-2.2.2/trueseeing/app/inspect.py
--rw-r--r--   0        0        0     2758 2024-03-19 12:42:27.435067 trueseeing-2.2.2/trueseeing/app/scan.py
--rw-r--r--   0        0        0     7006 2024-03-19 19:14:28.904058 trueseeing-2.2.2/trueseeing/app/shell.py
--rw-r--r--   0        0        0        0 2024-01-19 12:19:41.075163 trueseeing-2.2.2/trueseeing/core/__init__.py
--rw-r--r--   0        0        0        0 2024-01-31 06:00:56.918524 trueseeing-2.2.2/trueseeing/core/android/analysis/__init__.py
--rw-r--r--   0        0        0    12684 2024-03-19 12:25:17.852896 trueseeing-2.2.2/trueseeing/core/android/analysis/flow.py
--rw-r--r--   0        0        0     4344 2024-03-02 12:33:50.336346 trueseeing-2.2.2/trueseeing/core/android/analysis/smali.py
--rw-r--r--   0        0        0     4331 2024-03-10 08:02:42.474372 trueseeing-2.2.2/trueseeing/core/android/asm.py
--rw-r--r--   0        0        0     8443 2024-03-13 03:42:26.372332 trueseeing-2.2.2/trueseeing/core/android/context.py
--rw-r--r--   0        0        0    19046 2024-03-17 12:39:18.304258 trueseeing-2.2.2/trueseeing/core/android/db.py
--rw-r--r--   0        0        0     1640 2024-01-31 06:00:56.919581 trueseeing-2.2.2/trueseeing/core/android/device.py
--rw-r--r--   0        0        0        0 2024-01-31 06:00:56.919631 trueseeing-2.2.2/trueseeing/core/android/model/__init__.py
--rw-r--r--   0        0        0     1371 2024-01-31 06:00:56.919728 trueseeing-2.2.2/trueseeing/core/android/model/code.py
--rw-r--r--   0        0        0     1160 2024-03-13 03:40:22.701517 trueseeing-2.2.2/trueseeing/core/android/store.py
--rw-r--r--   0        0        0     1043 2024-01-31 06:00:56.920074 trueseeing-2.2.2/trueseeing/core/android/tools.py
--rw-r--r--   0        0        0      498 2024-02-13 05:01:30.370674 trueseeing-2.2.2/trueseeing/core/config.py
--rw-r--r--   0        0        0     5622 2024-03-19 12:44:48.564810 trueseeing-2.2.2/trueseeing/core/context.py
--rw-r--r--   0        0        0     2969 2024-02-04 00:39:02.249456 trueseeing-2.2.2/trueseeing/core/cvss.py
--rw-r--r--   0        0        0     8711 2024-03-09 17:22:53.707379 trueseeing-2.2.2/trueseeing/core/db.py
--rw-r--r--   0        0        0     1589 2024-03-17 12:39:18.307828 trueseeing-2.2.2/trueseeing/core/env.py
--rw-r--r--   0        0        0      331 2024-02-14 03:01:34.612404 trueseeing-2.2.2/trueseeing/core/exc.py
--rw-r--r--   0        0        0     5684 2024-02-13 16:22:25.463670 trueseeing-2.2.2/trueseeing/core/ext.py
--rw-r--r--   0        0        0        0 2024-01-31 07:08:15.326744 trueseeing-2.2.2/trueseeing/core/model/__init__.py
--rw-r--r--   0        0        0      550 2024-02-03 00:48:50.829277 trueseeing-2.2.2/trueseeing/core/model/cmd.py
--rw-r--r--   0        0        0     1131 2024-02-14 03:01:34.612591 trueseeing-2.2.2/trueseeing/core/model/issue.py
--rw-r--r--   0        0        0      353 2024-02-19 04:31:50.126798 trueseeing-2.2.2/trueseeing/core/model/sig.py
--rw-r--r--   0        0        0     6058 2024-03-02 12:33:50.337769 trueseeing-2.2.2/trueseeing/core/report.py
--rw-r--r--   0        0        0     5931 2024-03-09 02:44:12.734409 trueseeing-2.2.2/trueseeing/core/scan.py
--rw-r--r--   0        0        0     2048 2024-02-19 21:06:26.675270 trueseeing-2.2.2/trueseeing/core/store.py
--rw-r--r--   0        0        0     6385 2024-03-07 00:23:15.847071 trueseeing-2.2.2/trueseeing/core/tools.py
--rw-r--r--   0        0        0    13968 2024-03-07 00:23:15.847467 trueseeing-2.2.2/trueseeing/core/ui.py
--rw-r--r--   0        0        0      228 2024-02-19 20:06:27.692470 trueseeing-2.2.2/trueseeing/core/z.py
--rw-r--r--   0        0        0     1405 2024-01-24 10:24:57.762468 trueseeing-2.2.2/trueseeing/libs/LICENSE.md
--rw-r--r--   0        0        0  2327223 2024-01-31 06:00:56.932918 trueseeing-2.2.2/trueseeing/libs/android/abe.jar
--rw-r--r--   0        0        0  6611168 2024-02-06 07:11:34.328335 trueseeing-2.2.2/trueseeing/libs/android/apkeditor.jar
--rw-r--r--   0        0        0   466291 2024-01-31 06:00:56.953553 trueseeing-2.2.2/trueseeing/libs/android/apksigner.jar
--rw-r--r--   0        0        0      317 2024-03-08 02:59:47.525022 trueseeing-2.2.2/trueseeing/libs/android/frida-app.smali
--rw-r--r--   0        0        0      109 2024-03-08 02:59:47.525178 trueseeing-2.2.2/trueseeing/libs/android/frida-scriptdir.config
--rw-r--r--   0        0        0      269 2024-01-31 06:00:56.953712 trueseeing-2.2.2/trueseeing/libs/android/nsc.xml
--rw-r--r--   0        0        0      261 2024-03-17 12:39:18.308733 trueseeing-2.2.2/trueseeing/libs/android/store.0.sql
--rw-r--r--   0        0        0     4932 2024-03-17 12:39:18.309315 trueseeing-2.2.2/trueseeing/libs/android/store.1.sql
--rw-r--r--   0        0        0      266 2024-02-16 09:08:08.309814 trueseeing-2.2.2/trueseeing/libs/files.0.sql
--rw-r--r--   0        0        0   246779 2023-04-30 23:37:21.115188 trueseeing-2.2.2/trueseeing/libs/public_suffix_list.dat
--rw-r--r--   0        0        0      498 2024-02-16 22:57:35.426555 trueseeing-2.2.2/trueseeing/libs/store.0.sql
--rw-r--r--   0        0        0       51 2024-03-19 12:44:48.565143 trueseeing-2.2.2/trueseeing/libs/store.s.sql
--rw-r--r--   0        0        0     5384 2024-02-14 03:01:34.613520 trueseeing-2.2.2/trueseeing/libs/template/report.html
--rw-r--r--   0        0        0    10252 2022-01-12 05:19:53.968753 trueseeing-2.2.2/trueseeing/libs/tlds.txt
--rw-r--r--   0        0        0        0 2022-01-21 06:20:57.805686 trueseeing-2.2.2/trueseeing/py.typed
--rw-r--r--   0        0        0      678 2024-02-13 16:22:25.465751 trueseeing-2.2.2/trueseeing/sig/__init__.py
--rw-r--r--   0        0        0        0 2024-01-31 06:00:56.954153 trueseeing-2.2.2/trueseeing/sig/android/__init__.py
--rw-r--r--   0        0        0    12784 2024-03-15 21:20:45.023604 trueseeing-2.2.2/trueseeing/sig/android/crypto.py
--rw-r--r--   0        0        0    16300 2024-03-07 00:37:43.423661 trueseeing-2.2.2/trueseeing/sig/android/fingerprint.py
--rw-r--r--   0        0        0    17779 2024-02-19 04:58:33.653236 trueseeing-2.2.2/trueseeing/sig/android/manifest.py
--rw-r--r--   0        0        0     5227 2024-02-19 04:58:33.653499 trueseeing-2.2.2/trueseeing/sig/android/privacy.py
--rw-r--r--   0        0        0    31144 2024-02-19 04:58:33.653838 trueseeing-2.2.2/trueseeing/sig/android/security.py
--rw-r--r--   0        0        0    12239 1970-01-01 00:00:00.000000 trueseeing-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-11-26 16:54:25.486612 trueseeing-2.2.4/.dockerignore
+-rw-r--r--   0        0        0     1657 2024-01-22 01:54:13.062912 trueseeing-2.2.4/.github/workflows/deploy.yaml
+-rw-r--r--   0        0        0      529 2024-01-22 01:54:13.063170 trueseeing-2.2.4/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1595 2023-11-26 18:18:39.728412 trueseeing-2.2.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      841 2024-01-19 10:24:37.175838 trueseeing-2.2.4/.github/workflows/stale.yaml
+-rw-r--r--   0        0        0       44 2023-11-26 01:27:36.667762 trueseeing-2.2.4/.gitignore
+-rw-r--r--   0        0        0    35147 2017-07-31 13:42:43.000000 trueseeing-2.2.4/COPYING
+-rw-r--r--   0        0        0     1345 2024-03-08 08:40:38.210247 trueseeing-2.2.4/Dockerfile
+-rw-r--r--   0        0        0    11015 2024-05-18 12:18:09.964246 trueseeing-2.2.4/README.md
+-rw-r--r--   0        0        0     1565 2024-05-01 04:21:03.810494 trueseeing-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0      103 2024-05-18 12:18:09.964480 trueseeing-2.2.4/trueseeing/__init__.py
+-rw-r--r--   0        0        0     9312 2024-05-01 07:42:41.565057 trueseeing-2.2.4/trueseeing/api.py
+-rw-r--r--   0        0        0        0 2024-01-19 12:19:41.073814 trueseeing-2.2.4/trueseeing/app/__init__.py
+-rw-r--r--   0        0        0      617 2024-03-21 09:05:42.636173 trueseeing-2.2.4/trueseeing/app/cmd/__init__.py
+-rw-r--r--   0        0        0     4635 2024-02-02 13:13:46.930678 trueseeing-2.2.4/trueseeing/app/cmd/alias.py
+-rw-r--r--   0        0        0     1312 2024-03-10 08:02:42.473006 trueseeing-2.2.4/trueseeing/app/cmd/analyze.py
+-rw-r--r--   0        0        0        0 2024-01-31 06:00:56.916344 trueseeing-2.2.4/trueseeing/app/cmd/android/__init__.py
+-rw-r--r--   0        0        0     8017 2024-05-01 07:42:02.498728 trueseeing-2.2.4/trueseeing/app/cmd/android/asm.py
+-rw-r--r--   0        0        0    36867 2024-05-01 07:42:02.499768 trueseeing-2.2.4/trueseeing/app/cmd/android/engage.py
+-rw-r--r--   0        0        0    10666 2024-03-28 16:34:24.344193 trueseeing-2.2.4/trueseeing/app/cmd/android/recon.py
+-rw-r--r--   0        0        0     5867 2024-03-26 07:03:56.807508 trueseeing-2.2.4/trueseeing/app/cmd/android/search.py
+-rw-r--r--   0        0        0     4225 2024-03-26 23:05:25.433416 trueseeing-2.2.4/trueseeing/app/cmd/android/show.py
+-rw-r--r--   0        0        0     2710 2024-03-29 05:03:27.021040 trueseeing-2.2.4/trueseeing/app/cmd/config.py
+-rw-r--r--   0        0        0     1924 2024-03-26 22:58:30.543241 trueseeing-2.2.4/trueseeing/app/cmd/info.py
+-rw-r--r--   0        0        0     2954 2024-02-09 05:03:10.447760 trueseeing-2.2.4/trueseeing/app/cmd/report.py
+-rw-r--r--   0        0        0     2502 2024-03-29 05:03:27.021227 trueseeing-2.2.4/trueseeing/app/cmd/scan.py
+-rw-r--r--   0        0        0     2540 2024-05-01 05:06:47.872158 trueseeing-2.2.4/trueseeing/app/cmd/search.py
+-rw-r--r--   0        0        0     1784 2024-02-19 04:58:33.651096 trueseeing-2.2.4/trueseeing/app/cmd/show.py
+-rw-r--r--   0        0        0    14013 2024-05-01 05:58:26.237839 trueseeing-2.2.4/trueseeing/app/inspect.py
+-rw-r--r--   0        0        0     2758 2024-03-21 08:40:02.504890 trueseeing-2.2.4/trueseeing/app/scan.py
+-rw-r--r--   0        0        0     7210 2024-05-01 05:58:26.238069 trueseeing-2.2.4/trueseeing/app/shell.py
+-rw-r--r--   0        0        0        0 2024-01-19 12:19:41.075163 trueseeing-2.2.4/trueseeing/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-31 06:00:56.918524 trueseeing-2.2.4/trueseeing/core/android/analysis/__init__.py
+-rw-r--r--   0        0        0    13839 2024-04-06 19:20:15.061736 trueseeing-2.2.4/trueseeing/core/android/analysis/flow.py
+-rw-r--r--   0        0        0     1492 2024-03-21 09:05:42.637003 trueseeing-2.2.4/trueseeing/core/android/analysis/op.py
+-rw-r--r--   0        0        0     5358 2024-04-21 14:29:13.011139 trueseeing-2.2.4/trueseeing/core/android/asm.py
+-rw-r--r--   0        0        0    17561 2024-04-21 14:29:13.011535 trueseeing-2.2.4/trueseeing/core/android/context.py
+-rw-r--r--   0        0        0     8115 2024-03-26 07:03:56.810174 trueseeing-2.2.4/trueseeing/core/android/db.py
+-rw-r--r--   0        0        0     1870 2024-03-28 04:16:20.083391 trueseeing-2.2.4/trueseeing/core/android/device.py
+-rw-r--r--   0        0        0     1433 2024-04-21 14:29:13.011889 trueseeing-2.2.4/trueseeing/core/android/model.py
+-rw-r--r--   0        0        0     1160 2024-03-21 04:25:29.447701 trueseeing-2.2.4/trueseeing/core/android/store.py
+-rw-r--r--   0        0        0     1043 2024-01-31 06:00:56.920074 trueseeing-2.2.4/trueseeing/core/android/tools.py
+-rw-r--r--   0        0        0      498 2024-02-13 05:01:30.370674 trueseeing-2.2.4/trueseeing/core/config.py
+-rw-r--r--   0        0        0     6890 2024-05-01 05:58:26.238276 trueseeing-2.2.4/trueseeing/core/context.py
+-rw-r--r--   0        0        0     2969 2024-02-04 00:39:02.249456 trueseeing-2.2.4/trueseeing/core/cvss.py
+-rw-r--r--   0        0        0     8711 2024-03-09 17:22:53.707379 trueseeing-2.2.4/trueseeing/core/db.py
+-rw-r--r--   0        0        0     1589 2024-03-21 09:05:42.637865 trueseeing-2.2.4/trueseeing/core/env.py
+-rw-r--r--   0        0        0      331 2024-02-14 03:01:34.612404 trueseeing-2.2.4/trueseeing/core/exc.py
+-rw-r--r--   0        0        0     5684 2024-02-13 16:22:25.463670 trueseeing-2.2.4/trueseeing/core/ext.py
+-rw-r--r--   0        0        0        0 2024-01-31 07:08:15.326744 trueseeing-2.2.4/trueseeing/core/model/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-01 07:42:02.500758 trueseeing-2.2.4/trueseeing/core/model/cmd.py
+-rw-r--r--   0        0        0     1122 2024-03-21 09:05:42.638085 trueseeing-2.2.4/trueseeing/core/model/issue.py
+-rw-r--r--   0        0        0      353 2024-03-21 04:32:06.568731 trueseeing-2.2.4/trueseeing/core/model/sig.py
+-rw-r--r--   0        0        0     6058 2024-03-02 12:33:50.337769 trueseeing-2.2.4/trueseeing/core/report.py
+-rw-r--r--   0        0        0     5931 2024-03-09 02:44:12.734409 trueseeing-2.2.4/trueseeing/core/scan.py
+-rw-r--r--   0        0        0     2174 2024-03-26 07:03:56.810922 trueseeing-2.2.4/trueseeing/core/store.py
+-rw-r--r--   0        0        0     7111 2024-03-29 03:27:16.067150 trueseeing-2.2.4/trueseeing/core/tools.py
+-rw-r--r--   0        0        0    16133 2024-03-28 03:59:48.017410 trueseeing-2.2.4/trueseeing/core/ui.py
+-rw-r--r--   0        0        0      228 2024-02-19 20:06:27.692470 trueseeing-2.2.4/trueseeing/core/z.py
+-rw-r--r--   0        0        0     1405 2024-01-24 10:24:57.762468 trueseeing-2.2.4/trueseeing/libs/LICENSE.md
+-rw-r--r--   0        0        0  2327223 2024-01-31 06:00:56.932918 trueseeing-2.2.4/trueseeing/libs/android/abe.jar
+-rw-r--r--   0        0        0  6611168 2024-02-06 07:11:34.328335 trueseeing-2.2.4/trueseeing/libs/android/apkeditor.jar
+-rw-r--r--   0        0        0   466291 2024-01-31 06:00:56.953553 trueseeing-2.2.4/trueseeing/libs/android/apksigner.jar
+-rw-r--r--   0        0        0      317 2024-03-08 02:59:47.525022 trueseeing-2.2.4/trueseeing/libs/android/frida-app.smali
+-rw-r--r--   0        0        0      109 2024-03-08 02:59:47.525178 trueseeing-2.2.4/trueseeing/libs/android/frida-scriptdir.config
+-rw-r--r--   0        0        0      269 2024-01-31 06:00:56.953712 trueseeing-2.2.4/trueseeing/libs/android/nsc.xml
+-rw-r--r--   0        0        0      802 2024-03-21 09:05:42.638526 trueseeing-2.2.4/trueseeing/libs/android/store.0.sql
+-rw-r--r--   0        0        0      266 2024-02-16 09:08:08.309814 trueseeing-2.2.4/trueseeing/libs/files.0.sql
+-rw-r--r--   0        0        0   246779 2023-04-30 23:37:21.115188 trueseeing-2.2.4/trueseeing/libs/public_suffix_list.dat
+-rw-r--r--   0        0        0      498 2024-02-16 22:57:35.426555 trueseeing-2.2.4/trueseeing/libs/store.0.sql
+-rw-r--r--   0        0        0       81 2024-03-21 09:05:42.638721 trueseeing-2.2.4/trueseeing/libs/store.s.sql
+-rw-r--r--   0        0        0     5384 2024-02-14 03:01:34.613520 trueseeing-2.2.4/trueseeing/libs/template/report.html
+-rw-r--r--   0        0        0    10252 2022-01-12 05:19:53.968753 trueseeing-2.2.4/trueseeing/libs/tlds.txt
+-rw-r--r--   0        0        0        0 2022-01-21 06:20:57.805686 trueseeing-2.2.4/trueseeing/py.typed
+-rw-r--r--   0        0        0      623 2024-03-21 09:05:42.638929 trueseeing-2.2.4/trueseeing/sig/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 04:17:35.112369 trueseeing-2.2.4/trueseeing/sig/android/__init__.py
+-rw-r--r--   0        0        0    12948 2024-03-21 09:05:42.639171 trueseeing-2.2.4/trueseeing/sig/android/crypto.py
+-rw-r--r--   0        0        0    16193 2024-03-21 09:05:42.639409 trueseeing-2.2.4/trueseeing/sig/android/fingerprint.py
+-rw-r--r--   0        0        0    17594 2024-03-21 09:05:42.639673 trueseeing-2.2.4/trueseeing/sig/android/manifest.py
+-rw-r--r--   0        0        0     5225 2024-03-21 09:05:42.639941 trueseeing-2.2.4/trueseeing/sig/android/privacy.py
+-rw-r--r--   0        0        0    31001 2024-03-21 09:05:42.640205 trueseeing-2.2.4/trueseeing/sig/android/security.py
+-rw-r--r--   0        0        0    12280 1970-01-01 00:00:00.000000 trueseeing-2.2.4/PKG-INFO
```

### Comparing `trueseeing-2.2.2/.github/workflows/deploy.yaml` & `trueseeing-2.2.4/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/.github/workflows/lint.yaml` & `trueseeing-2.2.4/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/.github/workflows/publish.yaml` & `trueseeing-2.2.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/.github/workflows/stale.yaml` & `trueseeing-2.2.4/.github/workflows/stale.yaml`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/COPYING` & `trueseeing-2.2.4/COPYING`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/Dockerfile` & `trueseeing-2.2.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/README.md` & `trueseeing-2.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 ## Usage
 
 ### Interactive mode
 
 You can interactively scan/analyze/patch/etc. apps -- making it the ideal choice for manual analysis:
 
     $ trueseeing target.apk
-    [+] trueseeing 2.2.2
+    [+] trueseeing 2.2.4
     ts[target.apk]> ?
     ...
     ts[target.apk]> i                      # show generic information
     ...
     ts[target.apk]> pf AndroidManifest.xml # show manifest file
     ...
     ts[target.apk]> a                      # analyze resources too
```

### Comparing `trueseeing-2.2.2/pyproject.toml` & `trueseeing-2.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 ]
 readme = "README.md"
 keywords = ['android', 'security', 'pentest', 'hacking']
 dependencies = [
     "lxml~=5.0",
     "pyyaml~=6.0",
     "jinja2~=3.1",
-    "attrs~=23.2",
     "pypubsub~=4.0",
     "termcolor~=2.4",
     "progressbar2~=4.3",
     "importlib_metadata~=7.0",
     "asn1crypto~=1.5",
     "zstandard~=0.22",
     "aiohttp~=3.9",
     "lief~=0.14",
+    "pyaxmlparser~=0.3",
+    "prompt-toolkit~=3.0",
 ]
 requires-python = ">=3.9"
 dynamic = ['version', 'description']
 
 [project.optional-dependencies]
 dev = [
   "mypy~=1.7",
@@ -55,14 +56,15 @@
 
 [[tool.mypy.overrides]]
 module = [
   "lxml.*",
   "jinja2",
   "pubsub",
   "asn1crypto.*",
+  "pyaxmlparser.*",
 ]
 ignore_missing_imports = true
 
 # pyproject-flake8 (pflake8)
 [tool.flake8]
 extend-ignore = "E301,E302,E265,E114,E501,E231,E252,E261,E701,E722,E741"
 indent-size = 2
```

### Comparing `trueseeing-2.2.2/trueseeing/api.py` & `trueseeing-2.2.4/trueseeing/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,20 @@
   from collections import deque
   from typing import Any, TypedDict, Protocol, Optional, Callable, Coroutine, Union, List, Mapping, overload, Literal
   from typing_extensions import deprecated
   from trueseeing.core.context import Context, ContextType
   from trueseeing.core.android.context import APKContext
   from trueseeing.core.model.issue import Issue, IssueConfidence
 
+  ModifierEvent = Literal['begin', 'end']
+
   CommandEntrypoint = Callable[[deque[str]], Coroutine[Any, Any, None]]
   CommandlineEntrypoint = Callable[[str], Coroutine[Any, Any, None]]
   CommandPatternEntrypoints = Union[CommandEntrypoint, CommandlineEntrypoint]
+  ModifierListenerEntrypoint = Callable[[ModifierEvent, str], Coroutine[Any, Any, None]]
   SignatureEntrypoint = Callable[[], Coroutine[Any, Any, None]]
   FormatHandlerEntrypoint = Callable[[str], Optional[Context]]
   ConfigGetterEntrypoint = Callable[[], Any]
   ConfigSetterEntrypoint = Callable[[Any], None]
 
   class Entry(TypedDict, total=False):
     e: CommandEntrypoint
@@ -30,15 +33,15 @@
     e: CommandPatternEntrypoints  # type: ignore[misc]
     raw: bool
 
   class OptionEntry(Entry):
     pass
 
   class ModifierEntry(Entry):
-    pass
+    e: Optional[ModifierListenerEntrypoint]  # type: ignore[misc]
 
   class ConfigEntry(TypedDict):
     g: ConfigGetterEntrypoint
     s: ConfigSetterEntrypoint
     n: str
     d: str
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/__init__.py` & `trueseeing-2.2.4/trueseeing/app/cmd/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 if TYPE_CHECKING:
   from typing import Type, Iterator
   from trueseeing.api import Command
 
 def discover() -> Iterator[Type[Command]]:
   from trueseeing.api import Command
   from importlib import import_module
-  from trueseeing.core.model.cmd import CommandMixin
   from trueseeing.core.tools import get_public_subclasses, get_missing_methods, discover_modules_under
 
   for mod in discover_modules_under('trueseeing.app.cmd'):
     m = import_module(mod)
-    for c in get_public_subclasses(m, Command, [CommandMixin]):  # type:ignore[type-abstract]
+    for c in get_public_subclasses(m, Command, 'CommandMixin'):  # type:ignore[type-abstract]
       assert not get_missing_methods(c)
       yield c
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/alias.py` & `trueseeing-2.2.4/trueseeing/app/cmd/alias.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/analyze.py` & `trueseeing-2.2.4/trueseeing/app/cmd/analyze.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/android/asm.py` & `trueseeing-2.2.4/trueseeing/app/cmd/android/asm.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,24 +43,32 @@
 
     cmd = args.popleft()
 
     if not args:
       ui.fatal('need root path')
 
     import os
+    import re
     import time
     from tempfile import TemporaryDirectory
     from trueseeing.core.android.asm import APKAssembler
     from trueseeing.core.android.tools import move_apk
 
     root = args.popleft()
-    origapk = apk.replace('.apk', '.apk.orig')
+    origapk = re.sub(r'(\.x?apk)$', r'\1.orig', apk)
 
-    if os.path.exists(origapk) and not cmd.endswith('!'):
-      ui.fatal('backup file exists; force (!) to overwrite')
+    stem = re.sub(r'\.x?apk$', '', apk)
+    for typ in ['apk', 'xapk']:
+      print(origapk, f'{stem}.{typ}.orig')
+      if os.path.exists(f'{stem}.{typ}.orig') and not cmd.endswith('!'):
+        ui.fatal('backup file exists; force (!) to overwrite')
+
+    if apk.endswith('.xapk'):
+      ui.warn('assembling xapk is not supported; assembling as merged apk')
+      apk = apk.replace('.xapk', '.apk')
 
     opts = self._helper.get_effective_options(self._helper.get_modifiers(args))
 
     ui.info('assembling {root} -> {apk}'.format(root=root, apk=apk))
 
     at = time.time()
 
@@ -136,15 +144,15 @@
       self._warn_if_container('disassembling to directory could be slow in container builds (try disassembling to archives)')
 
     ui.info('disassembling {apk} -> {path}{nodex}'.format(apk=apk, path=path, nodex=' [res]' if nodex else ''))
 
     at = time.time()
 
     with TemporaryDirectory() as td:
-      await APKDisassembler.disassemble_to_path(apk, td, nodex=nodex)
+      await APKDisassembler.disassemble_to_path(apk, td, nodex=nodex, merge=apk.endswith('.xapk'))
 
       if not archive:
         with FileTransferProgressReporter('disassemble: writing').scoped() as progress:
           for nr in move_as_output(td, path, allow_orphans=True):
             progress.update(nr)
           progress.done()
       elif archive.startswith('tar'):
@@ -181,15 +189,15 @@
     archive = self._deduce_archive_format(root)
 
     if not archive:
       self._warn_if_container('exporting to directory could be slow in container builds (try exporting to archives)')
 
     at = time.time()
     extracted = 0
-    context = self._helper.get_context().require_type('apk')
+    context = self._helper.get_context()
     q = context.store().query()
 
     if not archive:
       for path,blob in q.file_enum(pat=pat, regex=True):
         target = os.path.join(root, *path.split('/'))
         if extracted % 10000 == 0:
           ui.info(' .. {nr} files'.format(nr=extracted))
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/android/exploit.py` & `trueseeing-2.2.4/trueseeing/app/cmd/android/engage.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,53 +3,63 @@
 
 from collections import deque
 
 from trueseeing.core.model.cmd import CommandMixin
 from trueseeing.core.ui import ui
 
 if TYPE_CHECKING:
-  from typing import Any, Optional, Dict, Mapping
+  from typing import Any, Optional, Dict, Mapping, List, Iterator, Tuple
   from trueseeing.api import CommandHelper, Command, CommandMap, OptionMap
   from trueseeing.core.android.context import APKContext
+  from trueseeing.core.android.model import XAPKManifest
 
-class ExploitCommand(CommandMixin):
+class EngageCommand(CommandMixin):
   def __init__(self, helper: CommandHelper) -> None:
     self._helper = helper
 
   @staticmethod
   def create(helper: CommandHelper) -> Command:
-    return ExploitCommand(helper)
+    return EngageCommand(helper)
 
   def get_commands(self) -> CommandMap:
     return {
-      'xq':dict(e=self._exploit_discard, n='xq', d='exploit: discard changes'),
-      'xx':dict(e=self._exploit_apply, n='xx[!]', d='exploit: apply and rebuild apk'),
-      'xx!':dict(e=self._exploit_apply),
-      'xf':dict(e=self._exploit_inject_frida, n='xf[!] [config]', d='exploit; inject frida gadget'),
-      'xf!':dict(e=self._exploit_inject_frida),
-      'xfs':dict(e=self._exploit_inject_frida_scriptdir, n='xfs[!] [path]', d='exploit; inject frida gadget in script dir mode'),
-      'xfs!':dict(e=self._exploit_inject_frida_scriptdir),
-      'xu':dict(e=self._exploit_disable_pinning, n='xu', d='exploit: disable SSL/TLS pinning'),
-      'xd':dict(e=self._exploit_enable_debug, n='xd', d='exploit: make debuggable'),
-      'xb':dict(e=self._exploit_enable_backup, n='xb', d='exploit: make backupable'),
-      'xt':dict(e=self._exploit_patch_target_api_level, n='xt[!] <api level>', d='exploit: patch target api level'),
-      'xt!':dict(e=self._exploit_patch_target_api_level),
-      'xp':dict(e=self._exploit_device_list_packages, n='xp', d='device: list installed packages'),
-      'xco':dict(e=self._exploit_device_copyout, n='xco[!] package [data.tar]', d='device: copy-out package data'),
-      'xco!':dict(e=self._exploit_device_copyout),
-      'xci':dict(e=self._exploit_device_copyin, n='xci[!] package [data.tar]', d='device: copy-in package data'),
-      'xci!':dict(e=self._exploit_device_copyin),
+      'xtq':dict(e=self._engage_tamper_discard, n='xtq', d='engage: discard changes'),
+      'xtx':dict(e=self._engage_tamper_apply, n='xtx[!]', d='engage: apply and rebuild apk'),
+      'xtx!':dict(e=self._engage_tamper_apply),
+      'xtf':dict(e=self._engage_tamper_inject_frida, n='xtf[!] [config]', d='engage; inject frida gadget'),
+      'xtf!':dict(e=self._engage_tamper_inject_frida),
+      'xtfs':dict(e=self._engage_tamper_inject_frida_scriptdir, n='xtfs[!] [path]', d='engage; inject frida gadget in script dir mode'),
+      'xtfs!':dict(e=self._engage_tamper_inject_frida_scriptdir),
+      'xtn':dict(e=self._engage_tamper_disable_pinning, n='xtn', d='engage: patch NSC to disable SSL/TLS pinning'),
+      'xtd':dict(e=self._engage_tamper_enable_debug, n='xtd', d='engage: make debuggable'),
+      'xtb':dict(e=self._engage_tamper_enable_backup, n='xtb', d='engage: make backupable'),
+      'xtt':dict(e=self._engage_tamper_patch_target_api_level, n='xtt[!] <api level>', d='engage: patch target api level'),
+      'xtt!':dict(e=self._engage_tamper_patch_target_api_level),
+      'xco':dict(e=self._engage_device_copyout, n='xco[!] package [data.tar]', d='engage: copy-out package data'),
+      'xco!':dict(e=self._engage_device_copyout),
+      'xci':dict(e=self._engage_device_copyin, n='xci[!] package [data.tar]', d='engage: copy-in package data'),
+      'xci!':dict(e=self._engage_device_copyin),
+      'xpd':dict(e=self._engage_deploy_package, n='xpd[!]', d='engage: deploy target package'),
+      'xpd!':dict(e=self._engage_deploy_package),
+      'xpu':dict(e=self._engage_undeploy_package, n='xpu', d='engage: remove target package'),
+      'xz':dict(e=self._engage_fuzz_intent, n='xz[!] "am-cmdline-template" [output.txt]', d='engage: fuzz intent'),
+      'xz!':dict(e=self._engage_fuzz_intent),
+      'xzr':dict(e=self._engage_fuzz_command, n='xzr[!] "cmdline-template" [output.txt]', d='engage: fuzz cmdline'),
+      'xzr!':dict(e=self._engage_fuzz_command),
+      'xg':dict(e=self._engage_grab_package, n='xg[!] package [output.apk]', d='engage: grab package'),
+      'xg!':dict(e=self._engage_grab_package),
     }
 
   def get_options(self) -> OptionMap:
     return {
-      'vers':dict(n='vers=X.Y.Z', d='specify frida-gadget version to use [xf,xfs]')
+      'vers':dict(n='vers=X.Y.Z', d='specify frida-gadget version to use [xf,xfs]'),
+      'w':dict(n='wNAME=FN', d='wordlist, use as {NAME} [xz]'),
     }
 
-  async def _exploit_discard(self, args: deque[str]) -> None:
+  async def _engage_tamper_discard(self, args: deque[str]) -> None:
     apk = self._helper.require_target()
 
     _ = args.popleft()
 
     import time
 
     at = time.time()
@@ -59,15 +69,15 @@
       if not q.patch_exists(None):
         ui.fatal('nothing to discard')
       ui.info('discarding patches to {apk}'.format(apk=apk))
       q.patch_clear()
 
     ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
 
-  async def _exploit_apply(self, args: deque[str]) -> None:
+  async def _engage_tamper_apply(self, args: deque[str]) -> None:
     apk = self._helper.require_target()
 
     cmd = args.popleft()
 
     import os
     import time
     from tempfile import TemporaryDirectory
@@ -103,15 +113,15 @@
 
         move_apk(outapk, apk)
 
       q.patch_clear()
 
     ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
 
-  async def _exploit_disable_pinning(self, args: deque[str]) -> None:
+  async def _engage_tamper_disable_pinning(self, args: deque[str]) -> None:
     apk = self._helper.require_target()
 
     _ = args.popleft()
 
     import time
     import random
     from importlib.resources import files
@@ -153,15 +163,15 @@
         n.attrib['id'] = f'0x{maxid+0x10000:08x}'
         n.attrib['type'] = 'xml'
         n.attrib['name'] = key
       q.patch_put(path, ET.tostring(root),z=True)
 
     ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
 
-  async def _exploit_enable_debug(self, args: deque[str]) -> None:
+  async def _engage_tamper_enable_debug(self, args: deque[str]) -> None:
     apk = self._helper.require_target()
 
     _ = args.popleft()
 
     import time
 
     ui.info('enabling debug {apk}'.format(apk=apk))
@@ -175,15 +185,15 @@
       manif = self._parsed_manifest(blob)
       for e in manif.xpath('.//application'):
         e.attrib['{http://schemas.android.com/apk/res/android}debuggable'] = "true"
       q.patch_put(path, self._manifest_as_xml(manif), z=True)
 
     ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
 
-  async def _exploit_enable_backup(self, args: deque[str]) -> None:
+  async def _engage_tamper_enable_backup(self, args: deque[str]) -> None:
     apk = self._helper.require_target()
 
     _ = args.popleft()
 
     import time
 
     ui.info('enabling full backup {apk}'.format(apk=apk))
@@ -199,15 +209,15 @@
         e.attrib['{http://schemas.android.com/apk/res/android}allowBackup'] = "true"
         if '{http://schemas.android.com/apk/res/android}fullBackupContent' in e.attrib:
           del e.attrib['{http://schemas.android.com/apk/res/android}fullBackupContent']
       q.patch_put(path, self._manifest_as_xml(manif), z=True)
 
     ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
 
-  async def _exploit_patch_target_api_level(self, args: deque[str]) -> None:
+  async def _engage_tamper_patch_target_api_level(self, args: deque[str]) -> None:
     apk = self._helper.require_target()
 
     cmd = args.popleft()
 
     try:
       level = int(args.popleft())
     except (IndexError, ValueError):
@@ -235,15 +245,15 @@
             ui.warn('downgrading the requirement')
             e.attrib['{http://schemas.android.com/apk/res/android}minSdkVersion'] = str(level)
       q.patch_put(path, self._manifest_as_xml(manif), z=True)
 
     ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
 
   # XXX: long and ugly
-  async def _exploit_inject_frida(self, args: deque[str], script_dir_mode: bool = False) -> None:
+  async def _engage_tamper_inject_frida(self, args: deque[str], script_dir_mode: bool = False) -> None:
     configfn: Optional[str] = None
     config_override: Optional[str] = None
     dev_frida_dir: Optional[str] = None
 
     apk = self._helper.require_target()
 
     cmd = args.popleft()
@@ -415,16 +425,16 @@
             lib=lib,
           ).encode('utf-8'),
           z=True
         )
 
     ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
 
-  async def _exploit_inject_frida_scriptdir(self, args: deque[str]) -> None:
-    await self._exploit_inject_frida(args, script_dir_mode=True)
+  async def _engage_tamper_inject_frida_scriptdir(self, args: deque[str]) -> None:
+    await self._engage_tamper_inject_frida(args, script_dir_mode=True)
 
   def _as_dalvik_classname(self, jn: str) -> str:
     return 'L{};'.format(jn.replace('.', '/'))
 
   def _as_smali_file_pattern(self, jn: str) -> str:
     return r'^smali/classes[0-9]+/{}.smali$'.format(jn.replace('.', '/'))
 
@@ -471,32 +481,15 @@
           if m:
             return m.group(1)
           else:
             raise InvalidResponseError()
       except ClientConnectionError:
         raise InvalidResponseError()
 
-  async def _exploit_device_list_packages(self, args: deque[str]) -> None:
-    _ = args.popleft()
-
-    ui.info('listing packages')
-
-    import time
-    import re
-    from trueseeing.core.android.device import AndroidDevice
-
-    at = time.time()
-    nr = 0
-    for m in re.finditer(r'^package:(.*)', await AndroidDevice().invoke_adb('shell pm list package'), re.MULTILINE):
-      p = m.group(1)
-      ui.info(p)
-      nr += 1
-    ui.success('done, {nr} packages found ({t:.02f} sec.)'.format(nr=nr, t=(time.time() - at)))
-
-  async def _exploit_device_copyout(self, args: deque[str]) -> None:
+  async def _engage_device_copyout(self, args: deque[str]) -> None:
     success: bool = False
 
     cmd = args.popleft()
     if not args:
       ui.fatal('need package name')
 
     target = args.popleft()
@@ -581,15 +574,15 @@
         success = True
 
     if success:
       ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
     else:
       ui.failure('copyout failed')
 
-  async def _exploit_device_copyin(self, args: deque[str]) -> None:
+  async def _engage_device_copyin(self, args: deque[str]) -> None:
     success: bool = False
 
     _ = args.popleft()
     if not args:
       ui.fatal('need package name')
 
     target = args.popleft()
@@ -673,14 +666,280 @@
         success = True
 
     if success:
       ui.success('done ({t:.02f} sec.)'.format(t=(time.time() - at)))
     else:
       ui.failure('copyin failed')
 
+  async def _engage_fuzz_command(self, args: deque[str], am: bool = False) -> None:
+    outfn: Optional[str] = None
+
+    cmd = args.popleft()
+
+    if not args:
+      if am:
+        ui.fatal('an "am" command line pattern required; try giving whatever you would to "adb shell am" (e.g. {} "start-activity .." ..)'.format(cmd))
+      else:
+        ui.fatal('command line pattern required; try giving you would to "adb shell"')
+
+    pat = args.popleft()
+    if am:
+      pat = f'am {pat}'
+
+    if args and not args[0].startswith('@'):
+      import os
+      outfn = args.popleft()
+      if os.path.exists(outfn) and not cmd.endswith('!'):
+        ui.fatal('outfile exists; force (!) to overwrite')
+
+    wordlist: Dict[str, List[str]] = dict()
+    for name, fn in self._helper.get_effective_options(self._helper.get_modifiers(args)).items():
+      if name.startswith('w'):
+        name = name[1:]
+        try:
+          with open(fn, 'r') as f:
+            wordlist[name] = [x.rstrip() for x in f]
+        except OSError as e:
+          ui.fatal(f'cannot open wordlist: {e}')
+
+    if not wordlist:
+      ui.fatal('need a wordlist (try @o:wNAME=FN)')
+
+    ui.info('wordlist built: {} words in {} keys ({})'.format(sum([len(v) for v in wordlist.values()]), len(wordlist), ','.join(wordlist.keys())))
+
+    def _expand(pat: str, wordlist: Mapping[str, List[str]]) -> Iterator[Tuple[int, int, str]]:
+      tries = min(len(v) for v in wordlist.values())
+      for nr in range(tries):
+        d = {k:v[nr] for k,v in wordlist.items()}
+        try:
+          yield nr, tries, pat.format(*[], **d)
+        except KeyError as e:
+          ui.fatal(f'unknown wordlist specified: {e}')
+
+    ui.info('starting fuzzing, opening log system-wide{}'.format(' [{}]'.format(outfn) if outfn else ''))
+
+    from trueseeing.core.android.device import AndroidDevice
+
+    dev = AndroidDevice()
+
+    async def _log(outfn: Optional[str]) -> None:
+      import sys
+      nr = 0
+
+      if not outfn:
+        f = sys.stdout.buffer
+      else:
+        f = open(outfn, 'wb')
+
+      try:
+        async for l in dev.invoke_adb_streaming('logcat -T1'):
+          f.write(l)
+          nr += 1
+          if outfn and nr % 256 == 0:
+            ui.info(' ... captured: {}')
+      finally:
+        if outfn:
+          f.close()
+
+    async def _fuzz(pat: str, wordlist: Mapping[str, List[str]]) -> None:
+      from asyncio import sleep
+      from subprocess import CalledProcessError
+      for nr, tries, t in _expand(pat, wordlist):
+        await sleep(.05)
+        prog = dict(nr=nr+1, max=tries, cmd=t)
+        try:
+          await dev.invoke_adb(f'shell {t}')
+          ui.info('[{nr}/{max}] {cmd}'.format(**prog))
+        except CalledProcessError as e:
+          ui.failure('[{nr}/{max}] {cmd}: failed: {code}'.format(code=e.returncode, **prog))
+
+    from asyncio import create_task, wait, FIRST_COMPLETED, ALL_COMPLETED
+    task_log = create_task(_log(outfn))
+    task_fuzz = create_task(_fuzz(pat, wordlist))
+
+    done, pending = await wait([task_log, task_fuzz], return_when=FIRST_COMPLETED)
+    for t in pending:
+      t.cancel()
+    done, _ = await wait([task_log, task_fuzz], return_when=ALL_COMPLETED)
+    for t in done:
+      exc = t.exception()
+      if exc:
+        ui.error('unhandled exception', exc=exc)
+
+  async def _engage_fuzz_intent(self, args: deque[str]) -> None:
+    await self._engage_fuzz_command(args, am=True)
+
+  async def _engage_deploy_package(self, args: deque[str]) -> None:
+    cmd = args.popleft()
+
+    context: APKContext = self._helper.get_context().require_type('apk')
+    apk = context.target
+
+    from time import time
+    from pubsub import pub
+    from trueseeing.core.ui import AndroidInstallProgressReporter
+    from trueseeing.core.android.device import AndroidDevice
+    from subprocess import CalledProcessError
+
+    dev = AndroidDevice()
+    at = time()
+    pkg = context.get_package_name()
+
+    ui.info(f'deploying package: {pkg}')
+
+    if cmd.endswith('!'):
+      try:
+        async for l in dev.invoke_adb_streaming(f'uninstall {pkg}', redir_stderr=True):
+          pub.sendMessage('progress.android.adb.update')
+          if b'success' in l.lower():
+            ui.warn('removing existing package')
+      except CalledProcessError as e:
+        ui.fatal('uninstall failed: {}'.format(e.stdout.decode().rstrip()))
+
+    with AndroidInstallProgressReporter().scoped():
+      pub.sendMessage('progress.android.adb.begin', what='installing ... ')
+      try:
+        async for l in dev.invoke_adb_streaming(f'install --no-streaming {apk}', redir_stderr=True):
+          pub.sendMessage('progress.android.adb.update')
+          if b'failure' in l.lower():
+            ui.stderr('')
+            if not cmd.endswith('!'):
+              ui.fatal('install failed; force (!) to replace ({})'.format(l.decode('UTF-8')))
+            else:
+              ui.fatal('install failed ({})'.format(l.decode('UTF-8')))
+
+        pub.sendMessage('progress.android.adb.done')
+      except CalledProcessError as e:
+        ui.fatal('install failed: {}'.format(e.stdout.decode().rstrip()))
+
+      ui.success('done ({t:.02f} sec){trailer}'.format(t=time() - at, trailer=' '*8))
+
+  async def _engage_undeploy_package(self, args: deque[str]) -> None:
+    _ = args.popleft()
+
+    context: APKContext = self._helper.get_context().require_type('apk')
+
+    from time import time
+    from pubsub import pub
+    from trueseeing.core.android.device import AndroidDevice
+    from subprocess import CalledProcessError
+
+    dev = AndroidDevice()
+    at = time()
+    pkg = context.get_package_name()
+
+    ui.info(f'removing package: {pkg}')
+
+    try:
+      async for l in dev.invoke_adb_streaming(f'uninstall {pkg}', redir_stderr=True):
+        pub.sendMessage('progress.android.adb.update')
+        if b'failure' in l.lower():
+          import re
+          packages = await dev.invoke_adb('shell pm list packages', redir_stderr=True)
+          if not re.match(f'{pkg}$', packages, re.MULTILINE):
+            ui.fatal('package not found')
+          else:
+            ui.fatal('uninstall failed ({})'.format(l.decode()))
+    except CalledProcessError as e:
+      ui.fatal('uninstall failed: {}'.format(e.stdout.decode().rstrip()))
+
+    ui.success('done ({t:.02f} sec)'.format(t=time() - at))
+
+  async def _engage_grab_package(self, args: deque[str]) -> None:
+    cmd = args.popleft()
+
+    import os
+    if not args:
+      ui.fatal('need the package name')
+
+    pkg = args.popleft()
+
+    if args:
+      outfn = args.popleft()
+    else:
+      outfn = f'{pkg}.apk'
+
+    if os.path.exists(outfn):
+      if not cmd.endswith('!'):
+        ui.fatal('output file exists; force (!) to overwrite')
+      else:
+        os.remove(outfn)
+
+    import re
+    from time import time
+    from tempfile import TemporaryDirectory
+    from pubsub import pub
+    from trueseeing.core.android.device import AndroidDevice
+
+    dev = AndroidDevice()
+    at = time()
+    outfn = os.path.realpath(outfn)
+
+    ui.info(f'grabbing package: {pkg} -> {outfn}')
+
+    basepath: Optional[bytes] = None
+    splits: List[bytes] = []
+
+    async for l in dev.invoke_adb_streaming(f'shell pm dump {pkg}', redir_stderr=True):
+      pub.sendMessage('progress.android.adb.update')
+      if f'unable to find package: {pkg}'.encode() in l.lower():
+        ui.fatal(f'package not found: {pkg}')
+
+      m = re.search(rb'codePath=(/.+)', l)
+      if m:
+        basepath = m.group(1)
+      m = re.search(rb'splits=\[(.+)\]', l)
+      if m:
+        splits = re.split(rb', *', m.group(1))
+
+    assert basepath
+    assert splits
+
+    with TemporaryDirectory() as td:
+      from os import chdir, getcwd
+      from shlex import quote
+      from zipfile import ZipFile, ZIP_STORED
+      cd = getcwd()
+      try:
+        chdir(td)
+        slicemap = dict()
+        if len(splits) == 1:
+          if outfn.endswith('.xapk'):
+            ui.warn('target has only one slice; using apk format')
+            outfn = outfn.replace('.xapk', '.apk')
+          ui.info('getting {nr} slice'.format(nr=len(splits)))
+          await dev.invoke_adb('pull {path}/base.apk {outfn}'.format(path=quote(basepath.decode()), outfn=outfn))
+        else:
+          if outfn.endswith('.apk'):
+            ui.warn('target has multiple slices; using xapk format')
+            outfn = outfn.replace('.apk', '.xapk')
+          ui.info('getting {nr} slices'.format(nr=len(splits)))
+          for s in splits:
+            slice = s.decode()
+            if slice == 'base':
+              fn = f'{pkg}.apk'
+            else:
+              fn = f'{slice}.apk'
+            await dev.invoke_adb('pull {path}/{typ}{slice}.apk {fn}'.format(
+              path=quote(basepath.decode()),
+              typ='' if slice == 'base' else 'split_',
+              slice=slice,
+              fn=fn,
+            ))
+            slicemap[slice] = fn
+          XAPKManifestGenerator(slicemap).generate()
+          with ZipFile(outfn, 'w', ZIP_STORED) as zf:
+            from glob import glob
+            for n in glob('*'):
+              with open(n, 'rb') as g:
+                zf.writestr(n, g.read())
+      finally:
+        chdir(cd)
+    ui.success('done ({t:.02f} sec)'.format(t=time() - at))
+
   def _generate_tempfilename_for_device(self, dir: Optional[str] = None) -> str:
     import random
     return (f'{dir}/' if dir is not None else '/data/local/tmp/') + ''.join(random.choices('abcdefghijklmnopqrstuvwxyz0123456789', k=16))
 
   def _parsed_manifest(self, blob: bytes) -> Any:
     import lxml.etree as ET
     return ET.fromstring(blob, parser=ET.XMLParser(recover=True))
@@ -688,7 +947,54 @@
   def _manifest_as_xml(self, manifest: Any) -> bytes:
     import lxml.etree as ET
     assert manifest is not None
     return ET.tostring(manifest) # type: ignore[no-any-return]
 
 class InvalidResponseError(Exception):
   pass
+
+class XAPKManifestGenerator:
+  def __init__(self, slicemap: Dict[str, str]) -> None:
+    self._slicemap = slicemap
+
+  def generate(self) -> None:
+    from os import stat
+    from pyaxmlparser import APK
+    manif: XAPKManifest = dict(
+      xapk_version='2',
+      total_size=0,
+      locales_name=dict(),
+      split_apks=[],
+    )
+
+    for slice, fn in self._slicemap.items():
+      conf = slice.split('.')[-1]
+      manif['total_size'] += stat(fn).st_size
+      manif['split_apks'].append(dict(id=slice, file=fn))
+      if slice == 'base':
+        apk = APK(fn)
+        manif.update(dict(
+          name=apk.get_app_name(),
+          icon='icon.png',
+          package_name=apk.get_package(),
+          version_code=apk.version_code,
+          version_name=apk.version_name,
+          min_sdk_version=apk.get_min_sdk_version(),
+          target_sdk_version=apk.get_target_sdk_version(),
+          permissions=apk.get_permissions(),
+        ))
+        with open('icon.png', 'wb') as f:
+          f.write(apk.icon_data)
+      elif len(conf) == 2:
+        apk = APK(fn)
+        country_code = conf
+        manif['locales_name'].update({
+          country_code:apk.get_app_name(),
+        })
+      if manif['locales_name']:
+        ln: Dict[str, str] = manif['locales_name']
+        for k in ln.keys():
+          if not ln[k]:
+            ln[k] = manif['name']
+    with open('manifest.json', 'w') as g:
+      from json import dumps
+      g.write(dumps(manif, separators=(',', ':')))
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/android/search.py` & `trueseeing-2.2.4/trueseeing/core/db.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,291 +1,218 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
-import re
-from collections import deque
-
-from trueseeing.core.model.cmd import CommandMixin
-from trueseeing.core.ui import ui
+from contextlib import contextmanager
+from trueseeing.core.model.issue import Issue
+from trueseeing.core.tools import noneif
+from trueseeing.core.z import ze, zd
 
 if TYPE_CHECKING:
-  from typing import Optional, Iterator, Iterable, Tuple
-  from trueseeing.api import CommandHelper, Command, CommandMap
-  from trueseeing.core.android.model.code import Op
-  from trueseeing.core.android.db import APKQuery
-
-class SearchCommand(CommandMixin):
-  def __init__(self, helper: CommandHelper) -> None:
-    self._helper = helper
-
-  @staticmethod
-  def create(helper: CommandHelper) -> Command:
-    return SearchCommand(helper)
-
-  def get_commands(self) -> CommandMap:
-    return {
-      '/c':dict(e=self._search_call, n='/c [pat]', d='search call for pattern'),
-      '/k':dict(e=self._search_const, n='/k insn [pat]', d='search consts for pattern'),
-      '/p':dict(e=self._search_put, n='/p[i] [pat]', d='search s/iputs for pattern'),
-      '/dp':dict(e=self._search_defined_package, n='/dp [pat]', d='search packages matching pattern'),
-      '/dc':dict(e=self._search_defined_class, n='/dc [pat]', d='search classes defined in packages matching pattern'),
-      '/dcx':dict(e=self._search_derived_class, n='/dcx classpat [methpat]', d='search classes defining methods and extending ones matching patterns'),
-      '/dci':dict(e=self._search_implementing_class, n='/dci ifacepat [methpat]', d='search classes defining methods and implementing interfaces matching patterns'),
-      '/dm':dict(e=self._search_defined_method, n='/dm pat', d='search classes defining methods matching pattern'),
-    }
-
-  def _output_as_tagged_listing(self, is_header: bool, line: str) -> None:
-    if is_header:
-      ui.info(ui.colored(line, color='green'))
-    else:
-      ui.info(line)
-
-  def _output_as_untagged_listing(self, is_header: bool, line: str) -> None:
-    if not is_header:
-      ui.info(line)
-
-  async def _search_call(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    _ = args.popleft()
-
-    if not args:
-      ui.fatal('need pattern')
-
-    pat = args.popleft()
-
-    from trueseeing.core.android.model.code import InvocationPattern
-    context = await self._helper.get_context().require_type('apk').analyze()
-
-    ui.info(f'searching call: {pat}')
-
-    with context.store().query().scoped() as q:
-      for is_header, line in OpFormatter(q).format(q.invocations(InvocationPattern('invoke-', pat))):
-        self._output_as_tagged_listing(is_header, line)
-
-  async def _search_const(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    _ = args.popleft()
-
-    if not args:
-      ui.fatal('need insn')
-
-    insn = args.popleft()
-    if args:
-      pat = args.popleft()
-    else:
-      pat = '.'
-
-    from trueseeing.core.android.model.code import InvocationPattern
-    context = await self._helper.get_context().require_type('apk').analyze()
-
-    ui.info(f'searching const: {pat} [{insn}]')
-
-    with context.store().query().scoped() as q:
-      for is_header, line in OpFormatter(q).format(q.consts(InvocationPattern(insn, pat))):
-        self._output_as_tagged_listing(is_header, line)
-
-  async def _search_put(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    cmd = args.popleft()
-
-    if args:
-      pat = args.popleft()
-    else:
-      pat = '.'
-
-    context = await self._helper.get_context().require_type('apk').analyze()
-    q = context.store().query()
-    if not cmd.endswith('i'):
-      fun = q.sputs
-      funtype = 's'
-    else:
-      fun = q.iputs
-      funtype = 'i'
-
-    ui.info(f'searching {funtype}puts: {pat}')
-
-    for is_header, line in OpFormatter(q).format(fun(pat)):
-      self._output_as_tagged_listing(is_header, line)
-
-  async def _search_defined_package(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    _ = args.popleft()
-
-    if args:
-      pat = args.popleft()
-    else:
-      pat = '.'
-
-    import os
-    context = await self._helper.get_context().require_type('apk').analyze()
-
-    ui.info(f'searching packages defining class: {pat}')
-
-    packages = set()
-    for fn in (context.source_name_of_disassembled_class(r) for r in context.disassembled_classes()):
-      if fn.endswith('.smali'):
-        packages.add(os.path.dirname(fn))
-    for pkg in sorted(packages):
-      if re.match(pat, pkg):
-        ui.info(pkg)
-
-  async def _search_defined_class(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    _ = args.popleft()
-
-    if not args:
-      ui.fatal('need pattern')
-
-    pat = args.popleft()
-
-    context = await self._helper.get_context().require_type('apk').analyze()
-
-    ui.info(f'searching classes in package: {pat}')
-
-    with context.store().query().scoped() as q:
-      for is_header, line in OpFormatter(q).format(q.classes_in_package_named(pat)):
-        self._output_as_untagged_listing(is_header, line)
-
-  async def _search_derived_class(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    _ = args.popleft()
-
-    if not args:
-      ui.fatal('need class')
-
-    base = args.popleft()
-    if args:
-      pat = args.popleft()
-    else:
-      pat = '.'
-
-    context = await self._helper.get_context().require_type('apk').analyze()
-
-    if pat == '.':
-      ui.info(f'searching classes deriving from: {base}')
-    else:
-      ui.info(f'searching classes deriving from: {base} [has method:{pat}]')
-
-    with context.store().query().scoped() as q:
-      for is_header, line in OpFormatter(q).format(q.classes_extends_has_method_named(pat, base)):
-        self._output_as_untagged_listing(is_header, line)
-
-  async def _search_implementing_class(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    _ = args.popleft()
-
-    if not args:
-      ui.fatal('need pattern')
-
-    interface = args.popleft()
-    if args:
-      pat = args.popleft()
-    else:
-      pat = '.'
-
-    if pat == '.':
-      ui.info(f'searching classes implementing: {interface}')
-    else:
-      ui.info(f'searching classes implementing: {interface} [has method:{pat}]')
-
-    context = await self._helper.get_context().require_type('apk').analyze()
-    q = context.store().query()
-    for is_header, line in OpFormatter(q).format(q.classes_implements_has_method_named(pat, interface)):
-      self._output_as_untagged_listing(is_header, line)
-
-  async def _search_defined_method(self, args: deque[str]) -> None:
-    self._helper.require_target()
-
-    _ = args.popleft()
-
-    if not args:
-      ui.fatal('need classname')
-
-    pat = args.popleft()
-
-    ui.info(f'searching classes defining method: {pat}')
-
-    context = await self._helper.get_context().require_type('apk').analyze()
-    q = context.store().query()
-    for is_header, line in OpFormatter(q).format(q.classes_has_method_named(pat)):
-      self._output_as_untagged_listing(is_header, line)
-
-class OpFormatter:
-  def __init__(self, q: APKQuery, indent: int = 4) -> None:
-    self._q = q
-    self._indent = indent
-
-  def format(self, ops: Iterable[Op]) -> Iterator[Tuple[bool, str]]:
-    focus: Optional[str] = None
-    for op in ops:
-      qn = self._q.qualname_of(op)
-      if qn is None:
-        qn = self._q.class_name_of(op)
-      if qn != focus:
-        yield True, f'{qn}:'
-        focus = qn
-      yield False, '{ind}{op}'.format(
-        ind=' '*self._indent,
-        op='{id:08x}{sep}{d}'.format(sep=' '*4, id=(op._id if op._id else 0xfffffff), d=self._op(op))
-      )
-
-  def _op(self, o: Op) -> str:
-    if o.t == 'directive':
-      return self._op_directive(o)
-    else:
-      if o.v.startswith('invoke'):
-        return self._op_invoke(o)
-      elif o.v.startswith('const-string'):
-        return self._op_const_str(o)
-      else:
-        return self._op_other(o)
-
-  def _op_invoke(self, o: Op) -> str:
-    regs = []
-    trailers = []
-    state = 0
-    for t in o.p:
-      if state == 0:
-        if t.t in ['reg', 'multireg']:
-          regs.append(t)
-        else:
-          state = 1
-      if state == 1:
-        if t.v == '{},': # XXX
-          continue
-        trailers.append(t)
-    return '{insn} {{{regs}}}, {trailers}'.format(
-      insn=o.v,
-      regs=', '.join([self._p(x) for x in regs]),
-      trailers=', '.join([self._p(x) for x in trailers]),
+  from typing import Any, Iterable, Tuple, Optional, Iterator, List, TypedDict
+  from typing_extensions import Self
+  from sqlite3 import Connection
+  from trueseeing.core.store import Store
+  from trueseeing.core.model.issue import IssueConfidence
+
+  class FileEntry(TypedDict):
+    path: str
+    blob: bytes
+    z: bool
+
+class StorePrep:
+  def __init__(self, c: Connection) -> None:
+    self.c = c
+
+  def stage0(self) -> None:
+    from importlib.resources import files
+    self.c.executescript((files('trueseeing')/'libs'/'store.s.sql').read_text())
+
+  def stage1(self) -> None:
+    from importlib.resources import files
+    self.c.execute('pragma user_version={}'.format(self._get_cache_schema_id()))
+    self.c.executescript((files('trueseeing')/'libs'/'store.0.sql').read_text())
+
+  def require_valid_schema(self) -> None:
+    v, = self.c.execute('pragma user_version').fetchone()
+    if v != self._get_cache_schema_id():
+      from trueseeing.core.exc import InvalidSchemaError
+      raise InvalidSchemaError()
+
+  def _get_cache_schema_id(self) -> int:
+    from trueseeing.core.env import get_cache_schema_id
+    return get_cache_schema_id()
+
+class FileTablePrep:
+  def __init__(self, c: Connection) -> None:
+    self.c = c
+
+  def prepare(self) -> None:
+    from importlib.resources import files
+    self.c.executescript((files('trueseeing')/'libs'/'files.0.sql').read_text())
+
+class Query:
+  def __init__(self, store: Store) -> None:
+    self.db = store.db
+
+  @contextmanager
+  def scoped(self) -> Iterator[Self]:
+    with self.db:
+      yield self
+
+  def file_find(self, pat: str, regex: bool = False) -> Iterable[str]:
+    for f, in self.db.execute('select path from files where path {op} :pat'.format(op=('like' if not regex else 'regexp')), dict(pat=pat)):
+      yield f
+
+  def file_get(self, path: str, default: Optional[bytes] = None, patched: bool = False) -> Optional[bytes]:
+    b: bytes
+    stmt0 = 'select z, blob from files where path=:path'
+    stmt1 = 'select A.z as z,coalesce(B.blob, A.blob) as blob from files as A full outer join patches as B using (path) where path=:path'
+    for z, b in self.db.execute(stmt1 if patched else stmt0, dict(path=path)):
+      return zd(b) if z else b
+    else:
+      return default
+
+  def file_get_xml(self, path: str, default: Any = None, patched: bool = False) -> Any:
+    import lxml.etree as ET
+    r = self.file_get(path, patched=patched)
+    if r is not None:
+      return ET.fromstring(r, parser=ET.XMLParser(recover=True))
+    else:
+      return default
+
+  def file_enum(self, pat: Optional[str], patched: bool = False, regex: bool = False) -> Iterable[Tuple[str, bytes]]:
+    if pat is not None:
+      stmt0 = 'select path, z, blob from files where path {op} :pat'.format(op=('like' if not regex else 'regexp'))
+      stmt1 = 'select path, coalesce(B.z, A.z) as z, coalesce(B.blob, A.blob) as blob from files as A full outer join patches as B using (path) where path {op} :pat'.format(op=('like' if not regex else 'regexp'))
+      for n, z, o in self.db.execute(stmt1 if patched else stmt0, dict(pat=pat)):
+        yield n, zd(o) if z else o
+    else:
+      stmt2 = 'select path, z, blob from files'
+      stmt3 = 'select path, coalesce(B.z, A.z) as z, coalesce(B.blob, A.blob) from files as A full outer join patches as B using (path)'
+      for n, z, o in self.db.execute(stmt3 if patched else stmt2):
+        yield n, zd(o) if z else o
+
+  def file_count(self, pat: Optional[str], patched: bool = False, regex: bool = False) -> int:
+    if pat is not None:
+      stmt0 = 'select count(1) from files where path {op} :pat'.format(op=('like' if not regex else 'regexp'))
+      stmt1 = 'select conut(1) from files as A full outer join patches as B using (path) where path {op} :pat'.format(op=('like' if not regex else 'regexp'))
+      for nr, in self.db.execute(stmt1 if patched else stmt0, dict(pat=pat)):
+        return nr # type:ignore[no-any-return]
+    else:
+      stmt2 = 'select count(1) from files'
+      stmt3 = 'select count(1) from files as A full outer join patches as B using (path)'
+      for nr, in self.db.execute(stmt3 if patched else stmt2):
+        return nr # type:ignore[no-any-return]
+    return 0
+
+  def file_put_batch(self, gen: Iterable[FileEntry]) -> None:
+    self.db.executemany(
+      'insert into files (path, blob, z) values (:path,:blob,:z)',
+      (dict(path=e['path'], blob=ze(e['blob']) if e['z'] else e['blob'], z=e['z']) for e in gen)
     )
 
-  def _op_const_str(self, o: Op) -> str:
-    reg = o.p[0]
-    cons = o.p[1]
-    return '{insn} {reg}, "{cons}"'.format(
-      insn=o.v,
-      reg=self._p(reg),
-      cons=self._p(cons),
+  def patch_enum(self, pat: Optional[str]) -> Iterable[Tuple[str, bytes]]:
+    if pat is not None:
+      stmt0 = 'select path, z, blob from patches where path like :pat'
+      for n, z, o in self.db.execute(stmt0, dict(pat=pat)):
+        yield n, zd(o) if z else o
+    else:
+      stmt1 = 'select path, z, blob from patches'
+      for n, z, o in self.db.execute(stmt1):
+        yield n, zd(o) if z else o
+
+  def patch_put(self, path: str, blob: bytes, z: bool) -> None:
+    self.db.execute(
+      'replace into patches (path, blob, z) values (:path,:blob,:z)',
+      dict(path=path, blob=ze(blob) if z else blob, z=z)
     )
 
-  def _op_other(self, o: Op) -> str:
-    return '{insn} {ps}'.format(
-      insn=o.v,
-      ps=', '.join([self._p(x) for x in o.p]),
-    )
+  def patch_exists(self, path: Optional[str]) -> bool:
+    stmt0 = 'select 1 from patches where path=:path'
+    stmt1 = 'select 1 from patches'
+    for r, in self.db.execute(stmt0 if path is not None else stmt1, dict(path=path)):
+      return True
+    else:
+      return False
+
+  def patch_clear(self) -> None:
+    self.db.execute('delete from patches')
+
+  def issue_count(self) -> int:
+    for nr, in self.db.execute('select count(1) from analysis_issues'):
+      return int(nr)
+    else:
+      return 0
+
+  def issue_raise(self, i: Issue) -> None:
+    assert i.score is not None
+    self.db.execute(
+      'insert or ignore into analysis_issues (sig, title, summary, descr, ref, sol, info0, info1, info2, cfd, score, cvss, aff0, aff1, aff2) values (:sigid, :title, :summary, :desc, :ref, :sol, :info0, :info1, :info2, :cfd, :score, :cvss, :aff0, :aff1, :aff2)',
+      dict(
+        sigid=i.sigid,
+        title=i.title,
+        cfd=self._issue_confidence_to_int(i.cfd),
+        cvss=i.cvss,
+        score=i.score,
+        summary=noneif(i.summary, ''),
+        desc=noneif(i.desc, ''),
+        ref=noneif(i.ref, ''),
+        sol=noneif(i.sol, ''),
+        info0=noneif(i.info0, ''),
+        info1=noneif(i.info1, ''),
+        info2=noneif(i.info2, ''),
+        aff0=noneif(i.aff0, ''),
+        aff1=noneif(i.aff1, ''),
+        aff2=noneif(i.aff2, ''),
+      ))
+
+  def issue_clear(self) -> None:
+    self.db.execute('delete from analysis_issues')
+
+  def issues(self) -> Iterable[Issue]:
+    for m in self.db.execute('select sig, title, summary, descr, ref, sol, info0, info1, info2, cfd, score, cvss, aff0, aff1, aff2 from analysis_issues'):
+      yield self._issue_from_row(m)
+
+  def findings_list(self) -> Iterable[Tuple[int, Tuple[str, str, Optional[str], Optional[str], Optional[str], Optional[str], float, str]]]:
+    for no, r in enumerate(self.db.execute('select distinct sig, title, summary, descr, ref, sol, score, cvss from analysis_issues order by score desc')):
+      yield no, (
+        r[0],
+        r[1],
+        r[2] if r[2] else None,
+        r[3] if r[3] else None,
+        r[4] if r[4] else None,
+        r[5] if r[5] else None,
+        r[6],
+        r[7],
+      )
 
-  def _op_directive(self, o: Op) -> str:
-    return '.{insn} {ps}'.format(
-      insn=o.v,
-      ps=' '.join([self._p(x) for x in o.p]),
+  def issues_by_group(self, *, sig: str, title: str) -> Iterable[Issue]:
+    for m in self.db.execute('select sig, title, summary, descr, ref, sol, info0, info1, info2, cfd, score, cvss, aff0, aff1, aff2 from analysis_issues where sig=:sig and title=:title order by score desc, cfd desc', dict(sig=sig, title=title)):
+      yield self._issue_from_row(m)
+
+  @classmethod
+  def _issue_confidence_to_int(cls, c: IssueConfidence) -> int:
+    return dict(certain=2, firm=1, tentative=0)[c]
+
+  @classmethod
+  def _issue_confidence_from_int(cls, c: int) -> IssueConfidence:
+    m: List[IssueConfidence] = ['tentative', 'firm', 'certain']
+    return m[c]
+
+  @classmethod
+  def _issue_from_row(cls, r: Tuple[Any, ...]) -> Issue:
+    return Issue(
+      sigid=r[0],
+      title=r[1],
+      cfd=cls._issue_confidence_from_int(r[9]),
+      cvss=r[11],
+      summary=r[2] if r[2] else None,
+      desc=r[3] if r[3] else None,
+      ref=r[4] if r[4] else None,
+      sol=r[5] if r[5] else None,
+      info0=r[6] if r[6] else None,
+      info1=r[7] if r[7] else None,
+      info2=r[8] if r[8] else None,
+      aff0=r[12] if r[12] else None,
+      aff1=r[13] if r[13] else None,
+      aff2=r[14] if r[14] else None,
     )
-
-  def _p(self, x: Op) -> str:
-    return '{}' if x.v == '{},' else x.v
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/android/show.py` & `trueseeing-2.2.4/trueseeing/app/cmd/android/show.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,154 +1,125 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, NamedTuple
 
 import re
-import sys
 from collections import deque
 
 from trueseeing.core.model.cmd import CommandMixin
-from trueseeing.core.ui import ui
+from trueseeing.core.ui import ui, OpFormatter, OpLister
 
 if TYPE_CHECKING:
-  from typing import Optional, TypedDict
+  from typing import Optional
   from trueseeing.api import CommandHelper, Command, CommandMap
   from trueseeing.core.android.context import APKContext
 
-  class QualNameInfo(TypedDict):
-    path: str
-    sig: str
+class QualNameInfo(NamedTuple):
+  clazz: str
+  method: Optional[str]
 
 class ShowCommand(CommandMixin):
   def __init__(self, helper: CommandHelper) -> None:
     self._helper = helper
 
   @staticmethod
   def create(helper: CommandHelper) -> Command:
     return ShowCommand(helper)
 
   def get_commands(self) -> CommandMap:
     return {
-      'pd':dict(e=self._show_disasm, n='pd[!] qualname [output.smali]', d='show disassembled class/method'),
-      'pd!':dict(e=self._show_disasm),
-      'pk':dict(e=self._show_solved_constant, n='pk 0xop index', d='guess and show what constant would flow into the index-th arg of op (!: try harder)'),
-      'pt':dict(e=self._show_solved_typeset, n='pt 0xop index', d='guess and show what type would flow into the index-th arg of op'),
+      'pd':dict(e=self._show_disasm, n='pd qualname', d='show disassembled class/method'),
+      'pk':dict(e=self._show_solved_constant, n='pk[!] 0xaddr index', d='guess and show what constant would flow into the index-th arg of op (!: try harder)'),
+      'pk!':dict(e=self._show_solved_constant),
+      'pt':dict(e=self._show_solved_typeset, n='pt 0xaddr index', d='guess and show what type would flow into the index-th arg of op'),
     }
 
   async def _show_disasm(self, args: deque[str]) -> None:
-    outfn: Optional[str] = None
-
     self._helper.require_target()
 
-    cmd = args.popleft()
+    _ = args.popleft()
 
-    if not args:
+    try:
+      qn = args.popleft()
+    except IndexError:
       ui.fatal('need a qualname')
 
-    qn = args.popleft()
-
-    import os
-
-    if args:
-      outfn = args.popleft()
-      if os.path.exists(outfn) and not cmd.endswith('!'):
-        ui.fatal('outfile exists; force (!) to overwrite')
-
     context: APKContext = self._helper.get_context().require_type('apk')
+    await context.analyze()
 
     try:
       c = self._parse_qualname(qn)
     except ValueError:
       ui.fatal(f'invalid qualname (try quoting): {qn}')
 
     with context.store().query().scoped() as q:
-      for _, d in q.file_enum('smali%/{}'.format(c['path'])):
-        if outfn is None:
-          f = sys.stdout.buffer
-        else:
-          f = open(outfn, 'wb')
-        try:
-          if not c['sig']:
-            f.write(d)
-          else:
-            from io import BytesIO
-            pat = r'\.method.*? {}$'.format(re.escape(c['sig'])).encode('utf-8')
-            state = 0
-            for l in BytesIO(d):
-              if state == 0:
-                if re.match(pat, l):
-                  f.write(l)
-                  state = 1
-              elif state == 1:
-                f.write(l)
-                if l == b'.end method\n':
-                  state = 2
-              elif state == 2:
-                break
-        finally:
-          if f != sys.stdout.buffer:
-            f.close()
+      OpLister(OpFormatter(q)).list_tagged(q.body(c.clazz, c.method))
 
   def _parse_qualname(self, n: str) -> QualNameInfo:
     m = re.fullmatch('(L[^ ]+?;)(->[^ ]+?)?', n)
     if m is None:
       raise ValueError('invalid dalvik name: {n}') # XXX
-    return dict(
-      path='{}.smali'.format(m.group(1)[1:-1]),
-      sig=m.group(2)[2:] if m.group(2) else '',
+    return QualNameInfo(
+      clazz=m.group(1),
+      method=m.group(2)[2:] if m.group(2) else None,
     )
 
   async def _show_solved_constant(self, args: deque[str]) -> None:
     self._helper.require_target()
 
     cmd = args.popleft()
 
     if len(args) < 2:
-      ui.fatal('need op and index')
+      ui.fatal('need addr and index')
 
-    opn = int(args.popleft(), 16)
+    addr = int(args.popleft(), 16)
     idx = int(args.popleft())
 
     limit = self._helper.get_graph_size_limit(self._helper.get_modifiers(args))
 
     from trueseeing.core.android.analysis.flow import DataFlow
     with DataFlow.apply_max_graph_size(limit):
       context = await self._helper.get_context().require_type('apk').analyze()
       store = context.store()
       q = store.query()
-      op = q.op_get(opn)
+      op = q.op_get(addr)
       if op is not None:
         if cmd.endswith('!'):
           vs = DataFlow(q).solved_possible_constant_data_in_invocation(op, idx)
           ui.info(repr(vs))
         else:
           try:
             v = DataFlow(q).solved_constant_data_in_invocation(op, idx)
             ui.info(repr(v))
+          except DataFlow.UnsolvableValueError as ce:
+            if not ui.is_debugging:
+              ui.error('value is not solvable (possibly not a compile-time constant); try enabling debug mode (e core.debug=true) to see the data graph')
+            else:
+              ui.error(f'value is not solvable (possibly not a compile-time constant), data graph: {ce.graph}')
           except DataFlow.NoSuchValueError as e:
             ui.error(str(e))
       else:
-        ui.error('op #{} not found'.format(opn))
+        ui.error('0x{:08x}: invalid address'.format(addr))
 
   async def _show_solved_typeset(self, args: deque[str]) -> None:
     self._helper.require_target()
 
     _ = args.popleft()
 
     if len(args) < 2:
-      ui.fatal('need op and index')
+      ui.fatal('need addr and index')
 
-    opn = int(args.popleft(), 16)
+    addr = int(args.popleft(), 16)
     idx = int(args.popleft())
 
     limit = self._helper.get_graph_size_limit(self._helper.get_modifiers(args))
 
     from trueseeing.core.android.analysis.flow import DataFlow
     with DataFlow.apply_max_graph_size(limit):
       context = await self._helper.get_context().require_type('apk').analyze()
       store = context.store()
       q = store.query()
-      op = q.op_get(opn)
+      op = q.op_get(addr)
       if op is not None:
         vs = DataFlow(q).solved_typeset_in_invocation(op, idx)
         ui.info(repr(vs))
       else:
-        ui.error('op #{} not found'.format(opn))
+        ui.error('0x{:08x}: invalid address'.format(addr))
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/config.py` & `trueseeing-2.2.4/trueseeing/app/cmd/show.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
+import sys
 from collections import deque
 
 from trueseeing.core.model.cmd import CommandMixin
 from trueseeing.core.ui import ui
 
 if TYPE_CHECKING:
-  from typing import Dict
-  from trueseeing.api import CommandHelper, Command, CommandMap, ConfigEntry
-
-class ConfigCommand(CommandMixin):
-  _confbag: Dict[str, ConfigEntry]
+  from typing import Optional
+  from trueseeing.api import CommandHelper, Command, CommandMap
 
+class ShowCommand(CommandMixin):
   def __init__(self, helper: CommandHelper) -> None:
     self._helper = helper
-    self._confbag = self._helper._confbag  # type:ignore[attr-defined]
 
   @staticmethod
   def create(helper: CommandHelper) -> Command:
-    return ConfigCommand(helper)
+    return ShowCommand(helper)
 
   def get_commands(self) -> CommandMap:
     return {
-      '?e?':dict(e=self._help, n='?e?', d='config help'),
-      'e':dict(e=self._manip, n='e key[=value]', d='get/set config'),
+      'pf':dict(e=self._show_file, n='pf[x][!] path [output.bin]', d='show file (x: hex)'),
+      'pf!':dict(e=self._show_file),
+      'pfx':dict(e=self._show_file),
+      'pfx!':dict(e=self._show_file),
     }
 
-  async def _help(self, args: deque[str]) -> None:
-    ui.success('Configs:')
-    if self._confbag:
-      width = (2 + max([len(e.get('d', '')) for e in self._confbag.values()]) // 4) * 4
-      for k in sorted(self._confbag):
-        e = self._confbag[k]
-        if 'n' in e:
-          ui.stderr(
-            f'{{n:<{width}s}}{{d}}'.format(n=e['n'], d=e['d'])
-          )
-
-  async def _manip(self, args: deque[str]) -> None:
-    from trueseeing.core.exc import InvalidConfigKeyError
-    _ = args.popleft()
+  async def _show_file(self, args: deque[str]) -> None:
+    outfn: Optional[str] = None
+
+    self._helper.require_target()
+
+    cmd = args.popleft()
+
     if not args:
-      ui.fatal('need a config key')
-    kv = args.popleft()
+      ui.fatal('need path')
+
+    path = args.popleft()
+
     if args:
-      ui.fatal('got an unexpected token (try e key=value to set)')
-    try:
-      if '=' not in kv:
-        key = kv
-        ui.info('{}: {}'.format(key, self._helper.get_config(key)))
-      else:
-        key, value = kv.split('=')
-        if not value:
-          ui.fatal('need a value')
-        self._helper.set_config(key, value)
-    except InvalidConfigKeyError:
-      ui.fatal(f'unknown key: {key}')
+      import os
+      outfn = args.popleft()
+      if os.path.exists(outfn) and not cmd.endswith('!'):
+        ui.fatal('outfile exists; force (!) to overwrite')
+
+    from binascii import hexlify
+
+    context = await self._helper.get_context().analyze(level=1)
+    level = context.get_analysis_level()
+    if level < 3:
+      ui.warn('detected analysis level: {} ({}) -- try analyzing fully (\'aa\') to maximize coverage'.format(level, self._helper.decode_analysis_level(level)))
+    d = context.store().query().file_get(path)
+    if d is None:
+      ui.fatal('file not found')
+    if outfn is None:
+      sys.stdout.buffer.write(d if 'x' not in cmd else hexlify(d))
+    else:
+      with open(outfn, 'wb') as f:
+        f.write(d if 'x' not in cmd else hexlify(d))
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/info.py` & `trueseeing-2.2.4/trueseeing/app/cmd/info.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,44 +16,40 @@
 
   @staticmethod
   def create(helper: CommandHelper) -> Command:
     return InfoCommand(helper)
 
   def get_commands(self) -> CommandMap:
     return {
-      'i':dict(e=self._info, n='i[i][i]', d='print info (ii: overall, iii: detailed)'),
+      'i':dict(e=self._info, n='i[i]', d='print info (ii: more info)'),
       'ii':dict(e=self._info2),
-      'iii':dict(e=self._info3),
     }
 
   def _read_field(self, x: Any) -> Any:
     boolmap = {True:'yes',False:'no','true':'yes','false':'no',1:'yes',0:'no', None:'?'}
     return boolmap.get(x, x)
 
-  async def _info(self, args: deque[str], level: int = 0) -> None:
+  async def _info(self, args: deque[str], extended: bool = False) -> None:
     target = self._helper.require_target()
 
     _ = args.popleft()
 
     analysisguidemap = {
-      0: 'try ii for more info',
-      1: 'try iii for more info',
-      2: 'try iii for more info',
+      0: 'try a;i for more info',
+      1: 'try a;i for more info',
+      2: 'try aa;i for more info',
       3: 'try aaa;i for more info',
     }
 
     context = self._helper.get_context()
     analyzed = context.get_analysis_level()
-    if analyzed < level:
-      await context.analyze(level=level)
-      analyzed = level
 
     ui.info(f'info on {target}')
 
-    async for m in context._get_info():
+    async for m in context._get_info(extended):
       for k, v in m.items():
         if v is None:
           continue
         if not k.startswith('_'):
           ui.info('{:12s} {}'.format(k, self._read_field(v)))
         elif k == '_patch':
           ui.info('{:12s} {}'.format('has patch?', self._read_field(v)))
@@ -61,11 +57,8 @@
           ui.info('{:12s} {}{}'.format(
             'analyzed?',
             self._helper.decode_analysis_level(analyzed),
             ' ({})'.format(analysisguidemap[analyzed]) if analyzed < 4 else '',
           ))
 
   async def _info2(self, args: deque[str]) -> None:
-    return await self._info(args, level=1)
-
-  async def _info3(self, args: deque[str]) -> None:
-    return await self._info(args, level=3)
+    return await self._info(args, extended=True)
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/report.py` & `trueseeing-2.2.4/trueseeing/app/cmd/report.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/scan.py` & `trueseeing-2.2.4/trueseeing/app/cmd/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
       '?s?':dict(e=self._help_signature, n='?s?', d='signature help'),
       'as':dict(e=self._scan, n='as[!]', d='run a scan (!: clear current issues)'),
       'as!':dict(e=self._scan),
     }
 
   def get_modifiers(self) -> ModifierMap:
     return {
-      's':dict(n='@s:sig', d='include sig'),
-      'x':dict(n='@x:pa.ckage.name', d='exclude package'),
+      's':dict(n='@s:sig', d='include sig', e=None),
+      'x':dict(n='@x:pa.ckage.name', d='exclude package', e=None),
     }
 
   async def _help_signature(self, args: deque[str]) -> None:
     from trueseeing.core.scan import Scanner
     ui.success('Signatures:')
     sigs = Scanner.get_all_signatures()
     width = 2 + max([len(k) for k in sigs.keys()])
```

### Comparing `trueseeing-2.2.2/trueseeing/app/cmd/search.py` & `trueseeing-2.2.4/trueseeing/app/cmd/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,11 +67,11 @@
         for m0 in re.finditer(pat.encode('latin1'), blob):
           ui.info('{}:+{:08x}: {!r}'.format(path, m0.start(), m0.group(0)))
       else:
         from io import BytesIO
         for nr, t in enumerate(l.rstrip() for l in BytesIO(blob)):
           m = re.search(pat.encode('utf-8'), t)
           if m:
-            ui.info('{}:{:d}:{:d}: {}'.format(path, nr+1, m.start(), t.decode('utf-8')))
+            ui.info('{}:{:d}:{:d}: {}'.format(path, nr+1, m.start(), t.decode('utf-8', 'replace')))
 
   def _looks_binary(self, b: bytes) -> bool:
     return b'\x00' in b
```

### Comparing `trueseeing-2.2.2/trueseeing/app/inspect.py` & `trueseeing-2.2.4/trueseeing/app/inspect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
+from code import InteractiveConsole
 from collections import deque
 import asyncio
+from functools import cache
 from shlex import shlex
 import sys
 import re
 from trueseeing.core.context import FileOpener
 from trueseeing.core.ui import ui, CoreProgressReporter
 from trueseeing.core.exc import FatalError, InvalidSchemaError
 
 if TYPE_CHECKING:
   from typing import Mapping, Optional, Any, NoReturn, List, Dict, Awaitable, Type
+  from prompt_toolkit.styles import Style
   from trueseeing.core.context import ContextType
-  from trueseeing.api import Entry, Command, CommandHelper, CommandEntry, CommandPatternEntry, ModifierEntry, OptionEntry
+  from trueseeing.api import Entry, Command, CommandHelper, CommandEntry, CommandPatternEntry, ModifierEntry, OptionEntry, ConfigMap, ModifierEvent
 
 class InspectMode:
   def do(
       self,
       target: Optional[str],
       batch: bool = False,
       cmdlines: List[str] = [],
@@ -42,51 +45,63 @@
       self,
       target: Optional[str],
       batch: bool,
       cmdlines: List[str],
       abort_on_errors: bool,
       force_opener: Optional[str],
   ) -> int:
-    from code import InteractiveConsole
-
-    sein = self
     runner = Runner(target, abort_on_errors=abort_on_errors, force_opener=force_opener)
 
     for line in cmdlines:
-      asyncio.run(sein._worker(runner.run(line)))
+      asyncio.run(LambdaConsole._worker(runner.run(line)))
 
     if batch:
       return 0
 
     if not ui.is_tty(stdin=True):
       ui.fatal('requires a tty')
 
     asyncio.run(runner.greeting())
 
-    class LambdaConsole(InteractiveConsole):
-      def runsource(self, source: str, filename: Optional[str]=None, symbol: Optional[str]=None) -> bool:
-        try:
-          asyncio.run(sein._worker(runner.run(source)))
-        except FatalError:
-          pass
-        return False
-
-    try:
-      import readline
-    except ImportError:
-      readline = None # type: ignore[assignment] # noqa: F841
     ps1, ps2 = getattr(sys, 'ps1', None), getattr(sys, 'ps2', None)
     try:
-      runner.reset_prompt()
-      LambdaConsole(locals=locals(), filename='<input>').interact(banner='', exitmsg='')
+      LambdaConsole(locals=locals(), runner=runner).interact(banner='', exitmsg='')
       return 0
     finally:
       sys.ps1, sys.ps2 = ps1, ps2
 
-  async def _worker(self, coro: Any) -> None:
+class LambdaConsole(InteractiveConsole):
+  def __init__(self, /, runner: Runner, locals: Optional[Mapping[str, Any]] = None) -> None:
+    super().__init__(locals=locals, filename='<input>')
+    from prompt_toolkit import PromptSession
+    self._sess: Any = PromptSession()
+    self._runner = runner
+
+  def runsource(self, source: str, filename: Optional[str]=None, symbol: Optional[str]=None) -> bool:
+    try:
+      asyncio.run(self._worker(self._runner.run(source)))
+    except FatalError:
+      pass
+    return False
+
+  def raw_input(self, prompt: str = "") -> str:
+    target = self._runner.get_target()
+    return self._sess.prompt(  # type: ignore[no-any-return]
+      message=[('class:p', f'ts[{target}]> ' if target else 'ts> ')],
+      prompt_continuation=[('class:p', '... ')],
+      style=self._get_prompt_style(),
+    )
+
+  @cache
+  def _get_prompt_style(self) -> Style:
+    from prompt_toolkit.styles import Style
+    return Style.from_dict({'p': '#888800'})
+
+  @classmethod
+  async def _worker(cls, coro: Any) -> None:
     tasks = [asyncio.create_task(coro)]
     done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
     for t in pending:
       t.cancel()
     if pending:
       _, _ = await asyncio.wait(pending)
     for t in done:
@@ -110,37 +125,41 @@
   _mods: Dict[str, ModifierEntry]
   _opts: Dict[str, OptionEntry]
   _quiet: bool = False
   _verbose: bool = False
   _target: Optional[str]
   _abort_on_errors: bool = False
   _helper: CommandHelper
+  _loglevel: int
 
   def __init__(self, target: Optional[str], *, abort_on_errors: bool = False, force_opener: Optional[str] = None) -> None:
     from trueseeing.core.config import Configs
     self._target = target
     self._cmds = {
       '?':dict(e=self._help, n='?', d='help'),
       '?@?':dict(e=self._help_mod, n='?@?', d='modifier help'),
       '?o?':dict(e=self._help_opt, n='?o?', d='options help'),
+      '?f?':dict(e=self._help_formats, n='?f?', d='supported file formats'),
       '!':dict(e=self._shell, n='!', d='shell'),
       'o':dict(e=self._set_target, n='o /path/to/target', d='set target file'),
       'q':dict(e=self._quit, n='q', d='quit'),
     }
     self._cmdpats = {}
     self._mods = {
-      'o':dict(n='@o:option', d='pass option'),
-      'gs':dict(n='@gs:<int>[kmKM]', d='set graph size limit'),
+      'o':dict(n='@o:option', d='pass option', e=None),
+      'gs':dict(n='@gs:<int>[kmKM]', d='set graph size limit', e=None),
     }
     self._confbag = Configs.get().bag
+    self._confbag.update(self._get_configs())
     self._opts = {}
     if abort_on_errors:
       self._abort_on_errors = True
 
     self._helper = CommandHelperImpl(self, force_opener=force_opener)
+    self._loglevel = ui.level
 
     self._init_cmds()
 
   def _init_cmds(self) -> None:
     from trueseeing.core.ext import Extension
     from trueseeing.app.cmd import discover
 
@@ -157,27 +176,51 @@
     self._mods.update(t.get_modifiers())
     self._opts.update(t.get_options())
     self._confbag.update(t.get_configs())
 
   def get_target(self) -> Optional[str]:
     return self._target
 
+  def _get_configs(self) -> ConfigMap:
+    return {
+      'core.debug':dict(g=self._config_get_debug, s=self._config_set_debug, n='core.debug', d='toggle debug mode (true, false)'),
+      'core.quiet':dict(g=self._config_get_quiet, s=self._config_set_quiet, n='core.quiet', d='toggle quiet mode (true, false)'),
+    }
+
+  def _config_get_debug(self) -> str:
+    return 'true' if (ui.level == ui.DEBUG) else 'false'
+
+  def _config_set_debug(self, v: Any) -> None:
+    try:
+      self._loglevel = dict(true=ui.DEBUG, false=ui.INFO)[v]
+      self._reset_loglevel()
+    except KeyError:
+      ui.fatal(f'invalid value: {v}')
+
+  def _config_get_quiet(self) -> str:
+    return 'true' if (ui.level == ui.WARN) else 'false'
+
+  def _config_set_quiet(self, v: Any) -> None:
+    try:
+      self._loglevel = dict(true=ui.WARN, false=ui.INFO)[v]
+    except KeyError:
+      ui.fatal(f'invalid value: {v}')
+
   async def greeting(self) -> None:
     from trueseeing import __version__ as version
     ui.success(f"Trueseeing {version}")
 
   async def run(self, s: str) -> None:
     try:
       try:
         await self._run(s)
       except InvalidSchemaError:
         ui.fatal('invalid schema detected, forced reanalysis needed (try a!)')
     finally:
       self._reset_loglevel()
-      self.reset_prompt()
 
   async def _run(self, s: str) -> None:
     if not await self._run_raw(s):
       o: deque[str] = deque()
       lex = shlex(s, posix=True, punctuation_chars=';')
       lex.wordchars += '@:,=!$'
       for t in lex:
@@ -220,44 +263,58 @@
       c = tokens[0]
       if c in self._cmds:
         ent = self._cmds[c]
 
     if ent is None:
       return False
     else:
-      await self._as_cmd(ent['e'](args=tokens))
-      return True
+      await self._notify_modifiers('begin', tokens)
+      try:
+        await self._as_cmd(ent['e'](args=tokens))
+        return True
+      finally:
+        await self._notify_modifiers('end', tokens)
 
   async def _as_cmd(self, coro: Awaitable[Any]) -> None:
     try:
       try:
         await coro
       except KeyboardInterrupt:
         ui.fatal('interrupted')
     except FatalError:
       if self._abort_on_errors:
         raise QuitSession(1)
 
-  def _reset_loglevel(self, debug:bool = False) -> None:
-    ui.set_level(ui.INFO)
+  async def _notify_modifiers(self, ev: ModifierEvent, tokens: deque[str]) -> None:
+    for mod in self._get_modifiers(tokens):
+      typ, val = mod[1:].split(':', maxsplit=1)
+
+      for et, ee in self._mods.items():
+        if et == typ:
+          if ee['e'] is not None:
+            await ee['e'](ev, val)
 
-  def reset_prompt(self) -> None:
-    if self._target:
-      sys.ps1, sys.ps2 = ui.colored(f'ts[{self.get_target()}]> ', color='yellow'), ui.colored('... ', color='yellow')
-    else:
-      sys.ps1, sys.ps2 = ui.colored('ts> ', color='yellow'), ui.colored('... ', color='yellow')
+  def _get_modifiers(self, args: deque[str]) -> List[str]:
+    o = []
+    for m in args:
+      if m.startswith('@'):
+        o.append(m)
+    return o
+
+  def _reset_loglevel(self, debug:bool = False) -> None:
+    ui.set_level(self._loglevel)
 
   async def _help(self, args: deque[str]) -> None:
     ents: Dict[str, Entry] = dict()
     ents.update(self._cmds)
     ents.update(self._cmdpats)  # type: ignore[arg-type]
     await self._help_on('Commands:', ents)
 
   async def _help_mod(self, args: deque[str]) -> None:
-    await self._help_on('Modifiers:', self._mods)
+    await self._help_on('Modifiers:', self._mods) # type: ignore[arg-type]
 
   async def _help_opt(self, args: deque[str]) -> None:
     await self._help_on('Options:', self._opts)
 
   async def _help_on(self, topic: str, entries: Dict[str, Entry]) -> None:
     ui.success(topic)
     if entries:
@@ -265,14 +322,24 @@
       for k in sorted(entries):
         e = entries[k]
         if 'n' in e:
           ui.stderr(
             f'{{n:<{width}s}}{{d}}'.format(n=e['n'], d=e['d'])
           )
 
+  async def _help_formats(self, args: deque[str]) -> None:
+    from trueseeing.core.context import FileOpener
+    ui.success('File formats:')
+    formats = list(FileOpener().get_formats())
+    width = 2 + max([len(e['n']) for e in formats])
+    for e in formats:
+      ui.stderr(
+        f'{{n:<{width}s}}{{d}}'.format(n=e['n'], d=e['d'])
+      )
+
   async def _shell(self, args: deque[str]) -> None:
     from trueseeing.core.env import get_shell
     from asyncio import create_subprocess_exec
     await (await create_subprocess_exec(get_shell())).wait()
 
   async def _quit(self, args: deque[str]) -> None:
     raise QuitSession(0)
@@ -330,19 +397,15 @@
   async def run(self, s: str) -> None:
     await self._r._run(s)
 
   async def run_cmd(self, tokens: deque[str], line: Optional[str]) -> bool:
     return await self._r._run_cmd(tokens, line)
 
   def get_modifiers(self, args: deque[str]) -> List[str]:
-    o = []
-    for m in args:
-      if m.startswith('@'):
-        o.append(m)
-    return o
+    return self._r._get_modifiers(args)
 
   def get_effective_options(self, mods: List[str]) -> Mapping[str, str]:
     o = {}
     for m in mods:
       if m.startswith('@o:'):
         for a in m[3:].split(','):
           c: List[str] = a.split('=', maxsplit=1)
```

### Comparing `trueseeing-2.2.2/trueseeing/app/scan.py` & `trueseeing-2.2.4/trueseeing/app/scan.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/app/shell.py` & `trueseeing-2.2.4/trueseeing/app/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     cmdlines = []
 
     parser = ArgumentParser(description='Non-decompiling Android app vulnerability scanner')
     args_mut0 = parser.add_mutually_exclusive_group()
     args_mut1 = parser.add_mutually_exclusive_group()
     parser.add_argument('fn', nargs='?', metavar='FILE', help='Target APK file')
     parser.add_argument('--help-signatures', action='store_true', help='Show signatures')
+    parser.add_argument('--help-formats', action='store_true', help='Show supported file formats')
     parser.add_argument('--version', action='store_true', help='Version information')
     parser.add_argument('--norc', action='store_true', help='Ignore startup file')
     parser.add_argument('--noext', action='store_true', help='Ignore extensions')
     parser.add_argument('--quiet', action='store_true', help='Be less verbose')
     parser.add_argument('-d', '--debug', action='store_true', help='Debug mode')
     parser.add_argument('-e', '--abort-on-errors', action='store_true', help='Abort on errors')
     parser.add_argument('-F', dest='force_opener', help='Open target as specified format')
@@ -97,14 +98,18 @@
     if args.version:
       ui.stderr(self._version())
       return 0
     if args.help_signatures:
       args.no_target = True
       args.mode = 'batch'
       cmdlines = ['?s?']
+    if args.help_formats:
+      args.no_target = True
+      args.mode = 'batch'
+      cmdlines = ['?f?']
 
     ui.set_level(log_level)
 
     if not args.fn:
       if args.no_target:
         args.fn = '/dev/null'
       else:
```

### Comparing `trueseeing-2.2.2/trueseeing/core/android/analysis/flow.py` & `trueseeing-2.2.4/trueseeing/core/android/analysis/flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 import itertools
 from contextlib import contextmanager
 
 from trueseeing.core.ui import ui
-from trueseeing.core.android.model.code import Op
+from trueseeing.core.android.model import Op
+from trueseeing.core.android.analysis.op import OpAnalyzer
 
 if TYPE_CHECKING:
   from typing import List, Any, Iterable, Mapping, Set, Optional, FrozenSet, Union, Dict, Iterator
   from typing_extensions import Final
   from trueseeing.core.android.db import APKQuery
+  from trueseeing.core.android.model import Token
 
   DataGraph = Union[Op, Mapping[Op, Any]]
 
 class CodeFlow:
   def __init__(self, q: APKQuery) -> None:
     self._q = q
 
-  def callers_of(self, method: Op) -> Iterable[Op]:
-    yield from self._q.callers_of(method)
+  def callers_of(self, method_addr: int) -> Iterator[Op]:
+    yield from self._q.callers_of(method_addr)
 
-  def callstacks_of(self, method: Op) -> Mapping[Op, Any]:
+  def callstacks_of(self, method_addr: int) -> Mapping[Op, Any]:
     o = dict()
-    for m in self.callers_of(method):
-      o[m] = self.callstacks_of(m)
+    for caller in self.callers_of(method_addr):
+      o[caller] = self.callstacks_of(caller.addr)
     return o
 
 class DataFlow:
   _q: APKQuery
   _default_max_graph_size: Final[int] = 2 * 1048576
+  _an = OpAnalyzer()
 
   _max_graph_size: int = _default_max_graph_size
 
   class NoSuchValueError(Exception):
     pass
 
+  class UnsolvableValueError(NoSuchValueError):
+    def __init__(self, graph: Optional[DataGraph]) -> None:
+      self.graph = graph
+
   class RegisterDecodeError(Exception):
     pass
 
   class GraphSizeError(Exception):
     pass
 
   def __init__(self, q: APKQuery) -> None:
@@ -67,19 +74,19 @@
       yield None
     finally:
       cls.set_max_graph_size(o)
 
   def likely_calling_in(self, ops: List[Op]) -> None:
     pass
 
-  def into(self, o: Op) -> Optional[Union[Op, Mapping[Op, Any]]]:
+  def into(self, o: Op) -> Optional[DataGraph]:
     return self.analyze(o)
 
   @classmethod
-  def _decoded_registers_of(cls, ref: Op, type_: Any = frozenset) -> Any:
+  def _decoded_registers_of(cls, ref: Token, type_: Any = frozenset) -> Any:
     if ref.t == 'multireg':
       regs = ref.v
       if ' .. ' in regs:
         from_, to_ = regs.split(' .. ')
         return type_([f'{from_[0]}{c:d}' for c in range(int(from_[1:]), int(to_[1:]) + 1)])
       elif ',' in regs:
         return type_([r.strip() for r in regs.split(',')])
@@ -90,96 +97,97 @@
       return type_([regs.strip()])
     elif ref.t == 'reflike' and ref.v == '{},': # XXX
       return type_([])
     else:
       raise cls.RegisterDecodeError(f"unknown type of reference: {ref.t}, {ref.v}")
 
   @classmethod
-  def decoded_registers_of_list(cls, ref: Op) -> List[str]:
+  def decoded_registers_of_list(cls, ref: Token) -> List[str]:
     o: List[str] = cls._decoded_registers_of(ref, list)
     return o
 
   @classmethod
-  def decoded_registers_of_set(cls, ref: Op) -> FrozenSet[str]:
+  def decoded_registers_of_set(cls, ref: Token) -> FrozenSet[str]:
     o: FrozenSet[str] = cls._decoded_registers_of(ref, frozenset)
     return o
 
   # TBD: pack as SQL function
-  def looking_behind_from(self, op: Op) -> Iterable[Op]:
+  def looking_behind_from(self, op: Op) -> Iterator[Op]:
     focus = None
-    for o in self._q.reversed_insns_in_method(op):
+    for o in self._q.reversed_insns_in_method(op.addr):
+      xs = list(self._an.tokenize(o))
+      stem = xs[0]
       if focus is None:
-        if o.t != 'label':
+        if stem.t != 'label':
           yield o
         else:
-          if not o.v.startswith("try_"):
-            focus = o.v
+          if not stem.v.startswith("try_"):
+            focus = stem.v
       else:
-        if o.t != 'id' or not any(p.v == focus for p in o.p):
+        if stem.t != 'id' or not any(p.v == focus for p in xs[1:]):
           continue
         else:
           focus = None
 
   def solved_constant_data_in_invocation(self, invokation_op: Op, index: int) -> str:
-    assert invokation_op.t == 'id' and invokation_op.v.startswith('invoke')
+    assert self._an.get_insn(invokation_op).startswith('invoke')
     graph = self.analyze(invokation_op)
     try:
-      reg = self.decoded_registers_of_list(invokation_op.p[0])[index + (0 if ('-static' in invokation_op.v) else 1)]
+      reg = self.decoded_registers_of_list(self._an.get_param(invokation_op, 0))[index + (0 if ('-static' in self._an.get_insn(invokation_op)) else 1)]
     except IndexError:
       raise self.NoSuchValueError(f'argument not found at index {index}')
     if graph:
       try:
-        arg = graph[invokation_op][reg] # type: ignore[index]
-        if arg.t == 'id' and arg.v.startswith('const'):
-          return arg.p[1].v # type: ignore[no-any-return]
+        arg: Op = graph[invokation_op][reg] # type: ignore
+        if self._an.get_insn(arg).startswith('const'):
+          return self._an.get_param(arg, 1).v
         else:
-          raise self.NoSuchValueError(f'not a compile-time constant: {arg!r}')
+          raise self.UnsolvableValueError(graph=arg)
       except (KeyError, AttributeError):
-        raise self.NoSuchValueError(f'not a compile-time constant: {arg!r}')
+        raise self.UnsolvableValueError(graph=graph)
     else:
-      raise self.NoSuchValueError(f'not a compile-time constant: {arg!r}')
+      raise self.UnsolvableValueError(graph=None)
 
   @classmethod
   def walk_dict_values(cls, d: DataGraph) -> Iterable[Optional[Op]]:
     try:
       for v in d.values(): # type: ignore[union-attr]
         yield from cls.walk_dict_values(v)
     except AttributeError:
       yield d # type:ignore[misc]
 
   def solved_possible_constant_data_in_invocation(self, invokation_op: Op, index: int) -> Set[str]:
-    assert invokation_op.t == 'id' and invokation_op.v.startswith('invoke')
+    assert self._an.get_insn(invokation_op).startswith('invoke')
     graph = self.analyze(invokation_op)
-    reg = self.decoded_registers_of_list(invokation_op.p[0])[index + (0 if ('-static' in invokation_op.v) else 1)]
+    reg = self.decoded_registers_of_list(self._an.get_param(invokation_op, 0))[index + (0 if ('-static' in self._an.get_insn(invokation_op)) else 1)]
     if graph:
-      n = graph[invokation_op][reg] # type: ignore[index]
-      return {x.p[1].v for x in self.walk_dict_values(n) if x is not None and x.t == 'id' and x.v.startswith('const')}
+      n: DataGraph = graph[invokation_op][reg] # type: ignore
+      return {self._an.get_param(x, 1).v for x in self.walk_dict_values(n) if x is not None and self._an.get_insn(x).startswith('const')}
     else:
       return set()
 
   def solved_typeset_in_invocation(self, invokation_op: Op, index: int) -> Set[Any]:
-    assert invokation_op.t == 'id' and invokation_op.v.startswith('invoke')
+    assert self._an.get_insn(invokation_op).startswith('invoke')
     graph = self.analyze(invokation_op)
-    reg = self.decoded_registers_of_list(invokation_op.p[0])[index + (0 if ('-static' in invokation_op.v) else 1)]
+    reg = self.decoded_registers_of_list(self._an.get_param(invokation_op, 0))[index + (0 if ('-static' in self._an.get_insn(invokation_op)) else 1)]
     if graph:
-      arg = graph[invokation_op][reg] # type: ignore[index]
-
-      return {self._assumed_target_type_of_op(x) for x in self.walk_dict_values(arg) if x is not None and x.t == 'id'}
+      arg: DataGraph = graph[invokation_op][reg] # type: ignore
+      return {self._assumed_target_type_of_op(x) for x in self.walk_dict_values(arg) if x is not None}
     else:
       return set()
 
-  @staticmethod
-  def _assumed_target_type_of_op(x: Op) -> str:
-    assert x.t == 'id'
-    if x.v.startswith('const/4'):
+  @classmethod
+  def _assumed_target_type_of_op(cls, x: Op) -> str:
+    mn = cls._an.get_insn(x)
+    if mn.startswith('const/4'):
       return 'Ljava/lang/Integer;'
-    elif x.v.startswith('const-string'):
+    elif mn.startswith('const-string'):
       return 'Ljava/lang/String;'
-    elif x.v.startswith('new-array'):
-      return x.p[2].v
+    elif mn.startswith('new-array'):
+      return cls._an.get_param(x, 2).v
     else:
       return 'Ljava/lang/Object;'
 
   @classmethod
   def _approximated_size_of_graph(cls, d: Optional[DataGraph], *, _cache:Optional[Dict[int, int]] = None) -> int:
     if _cache is None:
       _cache = dict()
@@ -189,22 +197,22 @@
     elif isinstance(d, Op):
       return 1
     elif isinstance(d, dict):
       o = 0
       assert len(d) == 1
       for k,v in d.items():
         assert isinstance(k, Op)
-        assert k._id is not None
-        if k._id in _cache:
-          return _cache[k._id]
+        assert k.addr is not None
+        if k.addr in _cache:
+          return _cache[k.addr]
         else:
           for vk, vv in v.items():
             assert isinstance(vk, str)
             o += cls._approximated_size_of_graph(vv, _cache=_cache)
-          _cache[k._id] = o
+          _cache[k.addr] = o
       return o
     else:
       assert False
 
   @classmethod
   def _check_graph(cls, d: Optional[DataGraph]) -> int:
     n = cls._approximated_size_of_graph(d)
@@ -216,116 +224,134 @@
     if op is None or stage > 64: # XXX: Is it sufficient? Might be better if we make it tunable?
       return None
     if state is None:
       state = dict()
 
     o: Optional[DataGraph] = None
 
-    if op.t == 'id':
-      assert op._id is not None
-      if op._id in state:
-        return state[op._id] # type: ignore[no-any-return]
-      try:
-        if any(op.v.startswith(x) for x in ['const','new-','move-exception']):
-          o = op
-          state[op._id] = o
-          return o
-        elif op.v in ['move', 'array-length']:
-          o = {op:{k:self.analyze(self.analyze_recent_load_of(op, k), state, stage=stage+1) for k in self.decoded_registers_of_set(op.p[1])}}
-          ui.debug('analyze: op #{id} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='move', id=op._id, stage=stage, nodes=self._check_graph(o)))
-          state[op._id] = o
-          return o
-        elif any(op.v.startswith(x) for x in ['aget-']):
-          assert len(op.p) == 3
-          o = {op:{k:self.analyze(self.analyze_recent_array_load_of(op, k), state, stage=stage+1) for k in (self.decoded_registers_of_set(op.p[1]) | self.decoded_registers_of_set(op.p[2]))}}
-          ui.debug('analyze: op #{id} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='aget', id=op._id, stage=stage, nodes=self._check_graph(o)))
-          state[op._id] = o
-          return o
-        elif any(op.v.startswith(x) for x in ['sget-']):
-          assert len(op.p) == 2
-          o = {op:{k:self.analyze(self.analyze_recent_static_load_of(op), state, stage=stage+1) for k in self.decoded_registers_of_set(op.p[0])}}
-          ui.debug('analyze: op #{id} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='sget', id=op._id, stage=stage, nodes=self._check_graph(o)))
-          state[op._id] = o
-          return o
-        elif any(op.v.startswith(x) for x in ['iget-']):
-          assert len(op.p) == 3
-          o = {op:{k:self.analyze(self.analyze_recent_instance_load_of(op), state, stage=stage+1) for k in self.decoded_registers_of_set(op.p[0])}}
-          ui.debug('analyze: op #{id} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='iget', id=op._id, stage=stage, nodes=self._check_graph(o)))
-          state[op._id] = o
-          return o
-        elif op.v.startswith('move-result'):
-          o = self.analyze(self.analyze_recent_invocation(op), state, stage=stage+1)
-          ui.debug('analyze: op #{id} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='move-result', id=op._id, stage=stage, nodes=self._check_graph(o)))
-          state[op._id] = o
+    mn = self._an.get_insn(op)
+    addr = op.addr
+
+    assert addr is not None
+    if addr in state:
+      return state[addr] # type: ignore[no-any-return]
+    try:
+      if any(mn.startswith(x) for x in ['const','new-','move-exception']):
+        o = op
+        state[addr] = o
+        return o
+      elif mn in ['move', 'array-length']:
+        o = {op:{k:self.analyze(self.analyze_recent_load_of(op, k), state, stage=stage+1) for k in self.decoded_registers_of_set(self._an.get_param(op, 1))}}
+        ui.debug('analyze: 0x{addr:08x} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='move', addr=addr, stage=stage, nodes=self._check_graph(o)))
+        state[addr] = o
+        return o
+      elif any(mn.startswith(x) for x in ['aget-']):
+        assert self._an.get_param_count(op) == 3
+        o = {op:{k:self.analyze(self.analyze_recent_array_load_of(op, k), state, stage=stage+1) for k in (self.decoded_registers_of_set(self._an.get_param(op, 1)) | self.decoded_registers_of_set(self._an.get_param(op, 2)))}}
+        ui.debug('analyze: 0x{addr:08x} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='aget', addr=addr, stage=stage, nodes=self._check_graph(o)))
+        state[addr] = o
+        return o
+      elif any(mn.startswith(x) for x in ['sget-']):
+        assert self._an.get_param_count(op) == 2
+        o = {op:{k:self.analyze(self.analyze_recent_static_load_of(op), state, stage=stage+1) for k in self.decoded_registers_of_set(self._an.get_param(op, 0))}}
+        ui.debug('analyze: 0x{addr:08x} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='sget', addr=addr, stage=stage, nodes=self._check_graph(o)))
+        state[addr] = o
+        return o
+      elif any(mn.startswith(x) for x in ['iget-']):
+        assert self._an.get_param_count(op) == 3
+        o = {op:{k:self.analyze(self.analyze_recent_instance_load_of(op), state, stage=stage+1) for k in self.decoded_registers_of_set(self._an.get_param(op, 0))}}
+        ui.debug('analyze: 0x{addr:08x} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='iget', addr=addr, stage=stage, nodes=self._check_graph(o)))
+        state[addr] = o
+        return o
+      elif mn.startswith('move-result'):
+        o = self.analyze(self.analyze_recent_invocation(op), state, stage=stage+1)
+        ui.debug('analyze: 0x{addr:08x} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='move-result', addr=addr, stage=stage, nodes=self._check_graph(o)))
+        state[addr] = o
+        return o
+      else:
+        try:
+          o = {op:{k:self.analyze(self.analyze_recent_load_of(op, k), state, stage=stage+1) for k in self.decoded_registers_of_set(self._an.get_param(op, 0))}}
+          ui.debug('analyze: 0x{addr:08x} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='gen.', addr=addr, stage=stage, nodes=self._check_graph(o)))
+          state[addr] = o
           return o
-        else:
-          try:
-            o = {op:{k:self.analyze(self.analyze_recent_load_of(op, k), state, stage=stage+1) for k in self.decoded_registers_of_set(op.p[0])}}
-            ui.debug('analyze: op #{id} stage: {stage} ({mode}) -> nodes: {nodes}'.format(mode='gen.', id=op._id, stage=stage, nodes=self._check_graph(o)))
-            state[op._id] = o
-            return o
-          except self.RegisterDecodeError:
-            state[op._id] = None
-            return None
-      except self.GraphSizeError:
-        ui.warn('analyze: op #{id} stage: {stage}: too many nodes'.format(id=op._id, stage=stage))
-        state[op._id] = None
-        return None
-    else:
+        except self.RegisterDecodeError:
+          state[addr] = None
+          return None
+    except self.GraphSizeError:
+      ui.warn('analyze: 0x{addr:08x} stage: {stage}: too many nodes'.format(addr=addr, stage=stage))
+      state[addr] = None
       return None
 
   def analyze_recent_static_load_of(self, op: Op) -> Optional[Op]:
-    assert op.t == 'id' and any(op.v.startswith(x) for x in ['sget-'])
-    target = op.p[1].v
+    assert self._an.get_insn(op).startswith('sget-')
+    target = self._an.get_param(op, 1).v
     for o in itertools.chain(self.looking_behind_from(op), self._q.sputs(target)):
-      if o.t == 'id' and o.v.startswith('sput-'):
-        if o.p[1].v == target:
-          return o
+      try:
+        if self._an.get_insn(o).startswith('sput-'):
+          if self._an.get_param(o, 1).v == target:
+            return o
+      except ValueError:
+        pass
     else:
       ui.debug(f"analyze_recent_static_load_of: failed static trace: {op!r}")
       return None
 
   def analyze_load(self, op: Op) -> FrozenSet[str]:
-    if op.t == 'id':
-      if any(op.v.startswith(x) for x in ['const','new-','move','array-length','aget-','sget-','iget-']):
-        return self.decoded_registers_of_set(op.p[0])
-      elif any(op.v.startswith(x) for x in ['invoke-direct', 'invoke-virtual', 'invoke-interface']):
+    try:
+      v = self._an.get_insn(op)
+    except ValueError:
+      return frozenset()
+    else:
+      if any(v.startswith(x) for x in ['const','new-','move','array-length','aget-','sget-','iget-']):
+        return self.decoded_registers_of_set(self._an.get_param(op, 0))
+      elif any(v.startswith(x) for x in ['invoke-direct', 'invoke-virtual', 'invoke-interface']):
         # Imply modification of "this"
-        return frozenset(self.decoded_registers_of_list(op.p[0])[:1])
-    return frozenset()
+        return frozenset(self.decoded_registers_of_list(self._an.get_param(op, 0))[:1])
+      return frozenset()
 
   def analyze_recent_load_of(self, from_: Op, reg: str, stage: int = 0) -> Optional[Op]:
     for o in self.looking_behind_from(from_):
-      if o.t == 'id':
+      if self._an.get_mnemonic(o).t == 'id':
         if reg in self.analyze_load(o):
           return o
     if reg.startswith('p'):
       index = int(reg.replace('p', ''))
-      for caller in CodeFlow(self._q).callers_of(from_):
-        if self._q.qualname_of(from_) != self._q.qualname_of(caller):
-          caller_reg = self.decoded_registers_of_list(caller.p[0])[index]
-          ui.debug(f"analyze_recent_load_of: retrace: {from_!r} [{reg}] <-> {caller!r} [{caller_reg}] [stage: {stage}]")
+      for caller in CodeFlow(self._q).callers_of(from_.addr):
+        if not self._q.in_same_mod(from_.addr, caller.addr):
+          caller_reg = self.decoded_registers_of_list(self._an.get_param(caller, 0))[index]
+          if ui.is_debugging:
+            ui.debug('analyze_recent_load_of: retracing [{stage}]: {reg} 0x{addr:08x} [{qn}] -> {caller_reg} 0x{caller_addr:08x} [{caller_qn}] {{{caller_l}}}'.format(
+              stage=stage, reg=reg, addr=from_.addr, qn=self._q.qualname_of(from_.addr),
+              caller_reg=caller_reg, caller_addr=caller.addr, caller_qn=self._q.qualname_of(caller.addr),
+              caller_l=self._q.op_get(caller.addr).l,
+            ))
           if stage < 5:
             retraced = self.analyze_recent_load_of(caller, caller_reg, stage=stage+1)
             if retraced:
               return retraced
     return None
 
   # TBD: tracing on static-array fields
   def analyze_recent_array_load_of(self, from_: Op, reg: str) -> Optional[Op]:
     return self.analyze_recent_load_of(from_, reg)
 
   # TBD: tracing on static-instance fields
   def analyze_recent_instance_load_of(self, op: Op) -> Optional[Op]:
-    assert len(op.p) == 3
-    assert op.t == 'id' and any(op.v.startswith(x) for x in ['iget-'])
-    field = op.p[2].v
+    assert self._an.get_param_count(op) == 3
+    assert self._an.get_insn(op).startswith('iget-')
+    field = self._an.get_param(op, 2).v
     for o in itertools.chain(self.looking_behind_from(op), self._q.iputs(field)):
-      if o.t == 'id' and o.v.startswith('iput-') and o.p[2].v == field:
-        return o
+      try:
+        if self._an.get_insn(o).startswith('iput-') and self._an.get_param(o, 2).v == field:
+          return o
+      except ValueError:
+        pass
     return None
 
   def analyze_recent_invocation(self, from_: Op) -> Optional[Op]:
     for o in self.looking_behind_from(from_):
-      if o.t == 'id' and o.v.startswith('invoke'):
-        return o
+      try:
+        if self._an.get_insn(o).startswith('invoke'):
+          return o
+      except ValueError:
+        pass
     return None
```

### Comparing `trueseeing-2.2.2/trueseeing/core/android/asm.py` & `trueseeing-2.2.4/trueseeing/core/android/asm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 import os
 import os.path
+import shlex
 
 from pubsub import pub
 
 from trueseeing.core.env import get_home_dir
 from trueseeing.core.ui import ui
 
 if TYPE_CHECKING:
-  from typing import Tuple
+  from typing import Tuple, Optional
   from trueseeing.core.context import Context
   from trueseeing.core.db import FileEntry
 
 class APKDisassembler:
   _context: Context
 
-  def __init__(self, context: Context):
+  def __init__(self, context: Context, target: Optional[str] = None):
     self._context = context
+    if target:
+      self._target = target
+    else:
+      self._target = context.target
 
   async def disassemble(self, level: int = 4) -> None:
     await self._do(level)
 
   async def _do(self, level: int) -> None:
     import glob
     import shutil
     from trueseeing.core.tools import invoke_streaming
     from trueseeing.core.android.tools import toolchains
 
-    apk = 'target.apk'
-
     cwd = os.getcwd()
 
     pub.sendMessage('progress.core.asm.lift.begin')
 
     try:
       os.chdir(self._context.wd)
 
       with self._context.store().query().scoped() as query:
         with toolchains() as tc:
           async for l in invoke_streaming(r'java -jar {apkeditor} d -i {apk} {suppressor} -o files'.format(
               apkeditor=tc['apkeditor'],
-              apk=apk,
+              apk=shlex.quote(self._target),
               suppressor='-dex' if level < 3 else '',
           ), redir_stderr=True):
             pub.sendMessage('progress.core.asm.lift.update')
 
           os.chdir('files')
 
         def read_as_row(fn: str) -> FileEntry:
@@ -67,24 +70,49 @@
     finally:
       os.chdir(cwd)
       pub.sendMessage('progress.core.asm.lift.update')
       shutil.rmtree(os.path.join(self._context.wd, 'files'), ignore_errors=True)
       pub.sendMessage('progress.core.asm.lift.done')
 
   @classmethod
-  async def disassemble_to_path(cls, apk: str, path: str, nodex: bool = False) -> None:
+  async def disassemble_to_path(cls, target: str, path: str, nodex: bool = False, merge: bool = False) -> None:
+    import os
+    from tempfile import TemporaryDirectory
     from trueseeing.core.tools import invoke_streaming
     from trueseeing.core.android.tools import toolchains
 
     pub.sendMessage('progress.core.asm.disasm.begin')
 
-    with toolchains() as tc:
+    with TemporaryDirectory() as td:
+      with toolchains() as tc:
+        apk = target
+        if target.endswith('.xapk'):
+          if not merge:
+            raise ValueError('cannot disassemble xapk without merging')
+          with TemporaryDirectory() as td2:
+            from zipfile import ZipFile
+            with ZipFile(target) as zf:
+              for n in zf.namelist():
+                zf.extract(n, path=td2)
+            tmpapk = os.path.join(td, 'merged.apk')
+            async for l in invoke_streaming(
+              '(java -jar {apkeditor} m -i {path} -o {tmpapk})'.format(
+                apkeditor=tc['apkeditor'],
+                path=td2,
+                tmpapk=tmpapk,
+              )
+            ):
+              print(l)
+          apk = tmpapk
+        else:
+          apk = target
+
       async for l in invoke_streaming(
         '(java -jar {apkeditor} d -o {path} -i {apk} {s})'.format(
-          apk=apk,
+          apk=shlex.quote(apk),
           s='-dex' if nodex else '',
           apkeditor=tc['apkeditor'],
           path=path,
         ), redir_stderr=True
       ):
         pub.sendMessage('progress.core.asm.disasm.update')
 
@@ -98,15 +126,15 @@
     from trueseeing.core.android.tools import toolchains
 
     pub.sendMessage('progress.core.asm.asm.begin')
 
     with toolchains() as tc:
       async for l in invoke_streaming(
         '(java -jar {apkeditor} b -i {path} -o {wd}/output.apk && java -jar {apksigner} sign --ks {keystore} --ks-pass pass:android {wd}/output.apk)'.format(
-          wd=wd, path=path,
+          wd=wd, path=shlex.quote(path),
           apkeditor=tc['apkeditor'],
           apksigner=tc['apksigner'],
           keystore=await SigningKey().key(),
         ), redir_stderr=True
       ):
         pub.sendMessage('progress.core.asm.asm.update')
```

### Comparing `trueseeing-2.2.2/trueseeing/core/android/device.py` & `trueseeing-2.2.4/trueseeing/core/android/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,48 +3,54 @@
 
 from functools import cache
 from trueseeing.core.env import get_adb_host
 from trueseeing.core.tools import invoke, invoke_passthru, invoke_streaming
 from trueseeing.core.ui import ui
 
 if TYPE_CHECKING:
-  from typing import Optional, AsyncIterator
+  from typing import Optional, AsyncIterator, Any
 
 class AndroidDevice:
   def __init__(self) -> None:
     pass
 
-  async def invoke_adb(self, cmd: str) -> str:
+  async def invoke_adb(self, cmd: str, **kwargs: Any) -> str:
     self._require_adb()
     line = self._get_adb_cmdline(cmd)
     ui.debug("invoking: {line}")
-    return await invoke(line)
+    return await invoke(line, **kwargs)
 
-  async def invoke_adb_passthru(self, cmd: str) -> None:
+  async def invoke_adb_passthru(self, cmd: str, **kwargs: Any) -> None:
     self._require_adb()
     line = self._get_adb_cmdline(cmd)
     ui.debug("invoking: {line}")
-    await invoke_passthru(line)
+    await invoke_passthru(line, **kwargs)
 
-  async def invoke_adb_streaming(self, cmd: str) -> AsyncIterator[bytes]:
+  async def invoke_adb_streaming(self, cmd: str, **kwargs: Any) -> AsyncIterator[bytes]:
     self._require_adb()
     line = self._get_adb_cmdline(cmd)
     ui.debug("invoking: {line}")
-    async for l in invoke_streaming(line):
+    async for l in invoke_streaming(line, **kwargs):
       yield l
 
+  def get_adb_cmdline(self, cmd: str) -> str:
+    return self._get_adb_cmdline(cmd)
+
   def _get_adb_cmdline(self, cmd: str) -> str:
     host: Optional[str] = get_adb_host()
 
     line = 'adb {host} {cmd}'.format(
       host=f'-L {host}' if host else '',
       cmd=cmd
     )
     return line
 
+  def require_adb(self) -> None:
+    return self._require_adb()
+
   @cache
   def _require_adb(self) -> None:
     from trueseeing.core.tools import require_in_path
     require_in_path('adb', 'adb version')
 
   async def is_fullbackup_available(self) -> bool:
     out = await self.invoke_adb('backup 2>&1 || exit 0')
```

### Comparing `trueseeing-2.2.2/trueseeing/core/android/store.py` & `trueseeing-2.2.4/trueseeing/core/android/store.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/core/android/tools.py` & `trueseeing-2.2.4/trueseeing/core/android/tools.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/core/context.py` & `trueseeing-2.2.4/trueseeing/core/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, overload
 
 import os.path
 from abc import ABC, abstractmethod
-from trueseeing.core.env import get_cache_dir
 
 if TYPE_CHECKING:
-  from typing import List, Dict, Optional, Set, Literal, Any, Mapping, AsyncIterator, Tuple
+  from typing import List, Dict, Optional, Set, Literal, Any, Mapping, AsyncIterator, Tuple, Iterator
   from typing_extensions import Self
   from trueseeing.api import FormatEntry
   from trueseeing.core.store import Store
   from trueseeing.core.android.context import APKContext
 
   ContextType = str
   ContextInfo = Mapping[str, Any]
@@ -49,50 +48,59 @@
     else:
       if self._force_opener in self._formats:
         c = self._formats[self._force_opener]['e'](path)
         if c is not None:
           return c
       raise InvalidFileFormatError()
 
+  def get_formats(self) -> Iterator[Mapping[str, str]]:
+    for k,v in self._formats.items():
+      yield dict(n=k, d=v['d'])
+
   def _init_formats(self) -> None:
     from trueseeing.core.ext import Extension
 
     self._formats.update({
-      'apk':dict(e=self._handle_apk, r=r'\.apk$', d='apk'),
+      'apk':dict(e=self._handle_apk, r=r'\.apk$', d='Android application package'),
+      'xapk':dict(e=self._handle_xapk, r=r'\.xapk$', d='Android appllication bundle'),
     })
 
     for clazz in Extension.get().get_fileformathandlers():
       t = clazz.create()
       self._formats.update(t.get_formats())
       self._confbag.update(t.get_configs())
 
   def _handle_apk(self, path: str) -> Optional[Context]:
     from trueseeing.core.android.context import APKContext
     return APKContext(path)
 
+  def _handle_xapk(self, path: str) -> Optional[Context]:
+    from trueseeing.core.android.context import XAPKContext
+    return XAPKContext(path)
+
 class Context(ABC):
   _path: str
   _excludes: List[str]
   _store: Optional[Store] = None
   _wd: Optional[str] = None
 
   def __init__(self, path: str) -> None:
-    self._path = path
+    self._path = os.path.realpath(path)
     self._excludes = []
     # FIXME: is there a strict need of caching here?
     _ = self.wd
 
   @property
   def target(self) -> str:
     return self._path
 
   @property
   def wd(self) -> str:
     if self._wd is None:
-      self._wd = self._workdir_of()
+      self._wd = self._get_workdir()
     return self._wd
 
   @property
   def excludes(self) -> List[str]:
     return self._excludes
 
   @excludes.setter
@@ -110,17 +118,14 @@
   def require_type(self, typ: ContextType) -> Context: ...
   def require_type(self, typ: ContextType) -> Any:
     if typ in self.type:
       return self
     from trueseeing.core.exc import InvalidContextError
     raise InvalidContextError()
 
-  def _workdir_of(self) -> str:
-    return os.path.join(get_cache_dir(), self.fingerprint_of())
-
   def store(self) -> Store:
     if self._store is None:
       assert self.wd is not None
       from trueseeing.core.store import Store
       self._store = Store(self.wd)
     return self._store
 
@@ -144,42 +149,74 @@
 
   def has_patches(self) -> bool:
     if self.exists():
       return self.store().query().patch_exists(None)
     else:
       return False
 
+  def _get_identity(self) -> bytes:
+    from os import stat
+    c = stat(self._path)
+    return f'0,{c.st_size},{c.st_mtime_ns}'.encode()
+
   def _get_analysis_flag_name(self, level: int) -> str:
     return f'.done{level}' if level < 4 else '.done'
 
   def get_analysis_level(self) -> int:
     for level in range(4, 0, -1):
-      if os.path.exists(os.path.join(self.wd, self._get_analysis_flag_name(level))):
-        return level
+      fn = os.path.join(self.wd, self._get_analysis_flag_name(level))
+      if os.path.exists(fn):
+        with open(fn, 'rb') as f:
+          expected = f.read()
+        if not expected:
+          with open(fn, 'wb') as g:
+            from trueseeing.core.ui import ui
+            ui.warn('old style flags detected; marking them as for current target')
+            g.write(self._get_identity())
+          return level
+        else:
+          if expected == self._get_identity():
+            return level
+          else:
+            return 0
     return 0
 
+  def _mark_analysis_done(self, level: int) -> None:
+    flagfn = self._get_analysis_flag_name(level)
+    with open(os.path.join(self.wd, flagfn), 'wb') as f:
+      f.write(self._get_identity())
+
   async def analyze(self, level: int = 4) -> Self:
     from trueseeing.core.ui import ui
     if self.get_analysis_level() >= level:
       await self._recheck_schema()
       ui.debug('analyzed once')
     else:
-      flagfn = self._get_analysis_flag_name(level)
       if os.path.exists(self.wd):
         ui.info('analyze: removing leftover')
         self.remove()
 
       if level > 0:
         self.create()
         await self._analyze(level=level)
+      else:
+        self.invalidate()
 
-      with open(os.path.join(self.wd, flagfn), 'w'):
-        pass
+      self._mark_analysis_done(level)
     return self
 
+  def invalidate(self) -> None:
+    for level in range(4, 0, -1):
+      flag = os.path.join(self.wd, self._get_analysis_flag_name(level))
+      if os.path.exists(flag):
+        os.remove(flag)
+
+  @abstractmethod
+  def _get_workdir(self) -> str: ...
+
   @abstractmethod
   def _get_size(self) -> Optional[int]: ...
 
   @abstractmethod
   def _get_fingerprint(self) -> str: ...
 
   @abstractmethod
@@ -187,15 +224,15 @@
 
   @abstractmethod
   async def _recheck_schema(self) -> None: ...
 
   @abstractmethod
   async def _analyze(self, level: int) -> None: ...
 
-  async def _get_info(self) -> AsyncIterator[ContextInfo]:
+  async def _get_info(self, extended: bool) -> AsyncIterator[ContextInfo]:
     yield dict(path=self._path)
     size = self.size_of()
     if size:
       yield dict(size=size)
     yield dict(fp=self.fingerprint_of())
     yield dict(ctx=self.wd)
     yield dict(_patch=self.has_patches())
```

### Comparing `trueseeing-2.2.2/trueseeing/core/cvss.py` & `trueseeing-2.2.4/trueseeing/core/cvss.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/core/env.py` & `trueseeing-2.2.4/trueseeing/core/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 
 @cache
 def get_device_frida_dir(package_name: str) -> str:
   return '/data/local/tmp/ts2/{pkg}/frida'.format(pkg=package_name)
 
 @cache
 def get_cache_schema_id() -> int:
-  return 0x0657d048  # FIXME: remember to randomize this whenever incompatible changes occur on cache file structure, or DB schema
+  return 0x190b4df6  # FIXME: remember to randomize this whenever incompatible changes occur on cache file structure, or DB schema
```

### Comparing `trueseeing-2.2.2/trueseeing/core/ext.py` & `trueseeing-2.2.4/trueseeing/core/ext.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/core/model/cmd.py` & `trueseeing-2.2.4/trueseeing/core/model/cmd.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/core/model/issue.py` & `trueseeing-2.2.4/trueseeing/core/model/issue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional
-
-import attr
+from typing import TYPE_CHECKING, NamedTuple
 
 from trueseeing.core.cvss import CVSS3Scoring
 
 if TYPE_CHECKING:
+  from typing import Optional
   from typing_extensions import Literal
   IssueSeverity = Literal['critical', 'high', 'medium', 'low', 'info']
   IssueConfidence = Literal['certain', 'firm', 'tentative']
 
-@attr.s(auto_attribs=True, frozen=True)
-class Issue:
+class Issue(NamedTuple):
   sigid: str
   cvss: str
   title: str
   cfd: IssueConfidence = 'firm'
   summary: Optional[str] = None
   desc: Optional[str] = None
   ref: Optional[str] = None
```

### Comparing `trueseeing-2.2.2/trueseeing/core/report.py` & `trueseeing-2.2.4/trueseeing/core/report.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/core/scan.py` & `trueseeing-2.2.4/trueseeing/core/scan.py`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/core/store.py` & `trueseeing-2.2.4/trueseeing/core/store.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,20 @@
   db: Connection
 
   def __init__(self, path: str) -> None:
     self._path = path
     self.db = self._open_db()
     self._check_schema()
 
+  def invalidate(self) -> None:
+    if self.db:
+      self.db.close()
+    self.db = self._open_db()
+    self._check_schema()
+
   def _open_db(self) -> Connection:
     import sqlite3
     store_path = os.path.join(self._path, self._fn)
     is_creating = not os.path.exists(store_path)
     o = sqlite3.connect(store_path)
     o.create_function("REGEXP", 2, self._re_fn, deterministic=True)
     o.create_function("MZMATCHES", 3, self._mzmatches_fn, deterministic=True)
```

### Comparing `trueseeing-2.2.2/trueseeing/core/tools.py` & `trueseeing-2.2.4/trueseeing/core/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
+import asyncio
 from functools import cache
 from trueseeing.core.ui import ui
 
 if TYPE_CHECKING:
-  from pathlib import Path
-  from typing import Any, Optional, TypeVar, Iterator, TypedDict, AsyncIterator, Type, Iterable, FrozenSet, Dict, Set
+  from typing import Any, Optional, TypeVar, Iterator, AsyncIterator, Type, FrozenSet, Dict, Set, Union, SupportsIndex
+  from typing_extensions import Buffer
   T = TypeVar('T')
 
-  class Toolchain(TypedDict):
-    apkeditor: Path
-    apksigner: Path
-    abe: Path
-
 def noneif(x: Any, defaulter: Any) -> Any:
   if x is not None:
     return x
   else:
     if callable(defaulter):
       return defaulter()
     else:
@@ -37,48 +33,60 @@
 def require_in_path(cmd: str, cmdline: str) -> None:
   from subprocess import run, CalledProcessError
   try:
     run(cmdline, capture_output=True, check=True, shell=True)
   except CalledProcessError:
     ui.fatal('not found: {cmd}')
 
-async def invoke(as_: str, redir_stderr: bool = False) -> str:
+async def invoke(as_: str, redir_stderr: bool = False, catch_stderr: bool = False) -> str:
   from asyncio import create_subprocess_shell
   from subprocess import PIPE, STDOUT
-  p = await create_subprocess_shell(as_, stdout=PIPE, stderr=(STDOUT if redir_stderr else None))
-  out, _ = await p.communicate()
-  _check_return_code(p, as_, out, None)
+  p = await create_subprocess_shell(as_, stdout=PIPE, stderr=(STDOUT if redir_stderr else (PIPE if catch_stderr else None)))
+  out, err = await p.communicate()
+  _check_return_code(p, as_, out, err)
   return out.decode('UTF-8')
 
 async def invoke_passthru(as_: str, nocheck: bool = False) -> None:
   from asyncio import create_subprocess_shell
   p = await create_subprocess_shell(as_)
   await p.communicate()
   if not nocheck:
     _check_return_code(p, as_, None, None)
 
+class _UniversalBufferPatch(bytearray):
+  def find(self, __sub: Union[Buffer, SupportsIndex], __start: Optional[SupportsIndex] = None, __end: Optional[SupportsIndex] = None) -> int:
+    return super().replace(b'\r', b'\n').find(__sub, __start, __end)
+
 async def invoke_streaming(as_: str, redir_stderr: bool = False) -> AsyncIterator[bytes]:
-  import asyncio
   from subprocess import PIPE, STDOUT
   p = await asyncio.create_subprocess_shell(as_, stdout=PIPE, stderr=(STDOUT if redir_stderr else None))
+  p.stdout._buffer = _UniversalBufferPatch(p.stdout._buffer) # type: ignore[union-attr]
   try:
+    l: Optional[bytes] = None
     if p.stdout is not None:
       async for l in p.stdout:
         yield l
-    _check_return_code(await p.wait(), as_, None, None)
+    _check_return_code(await p.wait(), as_, l, None)
   finally:
     if p.returncode is None:
       try:
         t = asyncio.create_task(p.wait())
         await asyncio.wait([t], timeout=3., return_when=asyncio.ALL_COMPLETED)
       except asyncio.TimeoutError:
         ui.warn('process does not seem to terminate, killing it')
         p.kill()
         await p.wait()
 
+def invoke_sync(as_: str, redir_stderr: bool = False, catch_stderr: bool = False) -> str:
+  from subprocess import PIPE, STDOUT, run
+  p = run(as_, shell=True, stdout=PIPE, stderr=(STDOUT if redir_stderr else (PIPE if catch_stderr else None)))
+  out, err = p.stdout, p.stderr
+  _check_return_code(p, as_, out, err)
+  return out.decode('UTF-8')
+
 async def try_invoke(as_: str) -> Optional[str]:
   from subprocess import CalledProcessError
   try:
     return await invoke(as_)
   except CalledProcessError:
     return None
 
@@ -160,18 +168,19 @@
         tf.add(os.path.join(sp, fn), arcname=os.path.join(dp, fn), recursive=False)
         if not allow_orphans:
           os.remove(os.path.join(sp, fn))
         if divisor is None or (nr % divisor == 0):
           yield nr
         nr += 1
 
-def get_public_subclasses(mod: Any, typ: Type[T], typs: Iterable[Type[T]] = []) -> Iterator[Type[T]]:
+def get_public_subclasses(mod: Any, typ: Type[T], nopat: Optional[str] = None) -> Iterator[Type[T]]:
+  import re
   from inspect import getmembers, isclass
-  for n, clazz in getmembers(mod, lambda x: isclass(x) and x != typ and (x not in typs) and issubclass(x, typ)):
-    if not n.startswith('_'):
+  for n, clazz in getmembers(mod, lambda x: isclass(x) and x != typ and issubclass(x, typ)):
+    if not n.startswith('_') and not (nopat and re.search(nopat, n)):
       yield clazz
 
 def get_missing_methods(clazz: Any) -> FrozenSet[str]:
   from inspect import isclass
   assert isclass(clazz)
   return getattr(clazz, '__abstractmethods__', frozenset())
```

### Comparing `trueseeing-2.2.2/trueseeing/core/ui.py` & `trueseeing-2.2.4/trueseeing/core/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import sys
 from contextlib import contextmanager
 from functools import cache
 from pubsub import pub
 from trueseeing.core.exc import FatalError
 
 if TYPE_CHECKING:
-  from typing import NoReturn, Optional, TextIO, Set, Any, Iterator
+  from typing import NoReturn, Optional, TextIO, Set, Any, Iterator, Iterable, Tuple
   from typing_extensions import Final
   from progressbar import ProgressBar
   from trueseeing.core.model.issue import Issue
+  from trueseeing.core.android.model import Op
+  from trueseeing.core.android.db import APKQuery
 
 class UI:
   DEBUG: Final = 0
   INFO: Final = 1
   WARN: Final = 2
   ERROR: Final = 3
   CRITICAL: Final = 4
@@ -394,9 +396,82 @@
       for k, v in submap.items():
         pub.unsubscribe(v, k)
       pass
 
   def _issue(self, issue: Issue) -> None:
     self._CN.note(issue)
 
+class AndroidInstallProgressReporter:
+  _bar: Optional[ProgressBar] = None
+
+  @contextmanager
+  def scoped(self) -> Iterator[None]:
+    submap = {
+      'progress.android.adb.begin':self._begin,
+      'progress.android.adb.update':self._update,
+      'progress.android.adb.done':self._done,
+    }
+    try:
+      for k, v in submap.items():
+        pub.subscribe(v, k)
+      yield None
+    finally:
+      for k, v in submap.items():
+        pub.unsubscribe(v, k)
+      pass
+
+  def _begin(self, what: str) -> None:
+    if ui.is_tty():
+      from progressbar import ProgressBar, RotatingMarker
+      self._bar = ProgressBar(widgets=[
+        ui.bullet('info'),
+        what + ' ',
+        RotatingMarker()   # type:ignore[no-untyped-call]
+      ])
+    else:
+      self._bar = None
+
+  def _update(self) -> None:
+    if self._bar is not None:
+      self._bar.next()   # type:ignore[no-untyped-call]
+
+  def _done(self) -> None:
+    if self._bar:
+      self._bar.finish(end='\r')   # type:ignore[no-untyped-call]
+
+class OpFormatter:
+  def __init__(self, q: APKQuery, indent: int = 4) -> None:
+    self._q = q
+    self._indent = indent
+
+  def format(self, ops: Iterable[Op]) -> Iterator[Tuple[bool, str]]:
+    focus: Optional[str] = None
+    for op in ops:
+      qn = self._q.qualname_of(op.addr)
+      if qn is None:
+        qn = self._q.class_name_of(op.addr)
+      if qn != focus:
+        yield True, f'{qn}:'
+        focus = qn
+      yield False, '{ind}{op}'.format(
+        ind=' '*self._indent,
+        op='{id:08x}{sep}{l}'.format(sep=' '*4, id=op.addr, l=op.l.lstrip())
+      )
+
+class OpLister:
+  def __init__(self, formatter: OpFormatter) -> None:
+    self._formatter = formatter
+
+  def list_tagged(self, ops: Iterable[Op]) -> None:
+    for is_header, line in self._formatter.format(ops):
+      if is_header:
+        ui.info(ui.colored(line, color='green'))
+      else:
+        ui.info(line)
+
+  def list_untagged(self, ops: Iterable[Op]) -> None:
+    for is_header, line in self._formatter.format(ops):
+      if not is_header:
+        ui.info(line)
+
 
 ui = UI()
```

### Comparing `trueseeing-2.2.2/trueseeing/libs/LICENSE.md` & `trueseeing-2.2.4/trueseeing/libs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/libs/android/abe.jar` & `trueseeing-2.2.4/trueseeing/libs/android/abe.jar`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/libs/android/apkeditor.jar` & `trueseeing-2.2.4/trueseeing/libs/android/apkeditor.jar`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/libs/android/apksigner.jar` & `trueseeing-2.2.4/trueseeing/libs/android/apksigner.jar`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/libs/public_suffix_list.dat` & `trueseeing-2.2.4/trueseeing/libs/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/libs/template/report.html` & `trueseeing-2.2.4/trueseeing/libs/template/report.html`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/libs/tlds.txt` & `trueseeing-2.2.4/trueseeing/libs/tlds.txt`

 * *Files identical despite different names*

### Comparing `trueseeing-2.2.2/trueseeing/sig/__init__.py` & `trueseeing-2.2.4/trueseeing/sig/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 if TYPE_CHECKING:
   from typing import Type, Iterator
   from trueseeing.api import Signature
 
 def discover() -> Iterator[Type[Signature]]:
   from trueseeing.api import Signature
-  from trueseeing.core.model.sig import SignatureMixin
   from importlib import import_module
   from trueseeing.core.tools import get_public_subclasses, get_missing_methods, discover_modules_under
 
   for mod in discover_modules_under('trueseeing.sig'):
     m = import_module(mod)
-    for c in get_public_subclasses(m, Signature, [SignatureMixin]):  # type:ignore[type-abstract]
+    for c in get_public_subclasses(m, Signature, 'SignatureMixin'):  # type:ignore[type-abstract]
       assert not get_missing_methods(c)
       yield c
```

### Comparing `trueseeing-2.2.2/trueseeing/sig/android/crypto.py` & `trueseeing-2.2.4/trueseeing/sig/android/crypto.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from typing import TYPE_CHECKING
 
 import asyncio
 import re
 import math
 from functools import cache
 
-from trueseeing.core.model.sig import SignatureMixin
-from trueseeing.core.android.model.code import InvocationPattern
+from trueseeing.core.android.model import InvocationPattern
+from trueseeing.core.android.model import SignatureMixin
 from trueseeing.core.android.analysis.flow import DataFlow
 
 if TYPE_CHECKING:
   from typing import Dict, Iterable, Optional, Any
-  from trueseeing.core.android.model.code import Op
   from trueseeing.core.android.store import APKStore
+  from trueseeing.core.android.db import APKQuery
+  from trueseeing.core.android.model import Op
   from trueseeing.api import Signature, SignatureHelper, SignatureMap
 
 class CryptoStaticKeyDetector(SignatureMixin):
   _id = 'crypto-static-keys'
   _cvss = 'CVSS:3.0/AV:P/AC:L/PR:N/UI:N/S:C/C:L/I:L/A:N/'
   _cvss_nonkey = 'CVSS:3.0/AV:P/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:N/'
   _cvss_pubkey = 'CVSS:3.0/AV:P/AC:H/PR:N/UI:N/S:C/C:N/I:L/A:N/'
@@ -44,39 +45,38 @@
   @classmethod
   def _assumed_randomness_of(cls, string: str) -> float:
     try:
       return cls._entropy_of(string) / float(math.log(len(string)) / math.log(2))
     except ValueError:
       return 0
 
-  @classmethod
-  def _important_args_on_invocation(cls, k: Op) -> Iterable[int]:
-    method_name = k.p[1].v
+  def _important_args_on_invocation(self, k: Op) -> Iterable[int]:
+    method_name = self._an.get_param(k, 1).v
     if re.match('L.*/(SecretKey|(Iv|GCM)Parameter|(PKCS8|X509)EncodedKey)Spec-><init>|L.*/MessageDigest;->update', method_name):
       yield 0
     else:
-      yield from range(len(DataFlow.decoded_registers_of_set(k.p[0])))
+      yield from range(len(DataFlow.decoded_registers_of_set(self._an.get_param(k, 0))))
 
   async def detect(self) -> None:
     await asyncio.gather(self._do_detect_case1(), self._do_detect_case2())
 
   async def _do_detect_case1(self) -> None:
     import base64
     import binascii
 
     def looks_like_real_key(k: str) -> bool:
       # XXX: silly
       return len(k) >= 8 and not any(x in k for x in ('Padding', 'SHA1', 'PBKDF2', 'Hmac', 'emulator'))
 
     pat_case2 = '^M[C-I][0-9A-Za-z+/=-]{48,}'
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.invocations(InvocationPattern('invoke-', '^Ljavax?.*/(SecretKey|(Iv|GCM)Parameter|(PKCS8|X509)EncodedKey)Spec|^Ljavax?.*/MessageDigest;->(update|digest)')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         for nr in self._important_args_on_invocation(cl):
           for found in DataFlow(q).solved_possible_constant_data_in_invocation(cl, nr):
             try:
               if re.search(pat_case2, found):
@@ -89,15 +89,15 @@
 
             if looks_like_real_key(found):
               self._helper.raise_issue(self._helper.build_issue(
                 sigid=self._id,
                 cvss=self._cvss,
                 title='insecure cryptography: static keys detected',
                 info0=info0,
-                info1=q.method_call_target_of(cl),
+                info1=q.method_call_target_of(cl.addr),
                 aff0=qn,
                 summary='Traces of cryptographic material has been found the application binary.',
                 desc='''\
 Traces of cryptographic material has been found in the application binary.  If cryptographic material is hardcoded, attackers can extract or replace them.
 ''',
                 sol='''\
 Use a device or installation specific information, or obfuscate them.
@@ -106,42 +106,42 @@
             else:
               self._helper.raise_issue(self._helper.build_issue(
                 sigid=self._id,
                 cvss=self._cvss_nonkey,
                 cfd='tentative',
                 title='Cryptographic constants detected',
                 info0=info0,
-                info1=q.method_call_target_of(cl),
+                info1=q.method_call_target_of(cl.addr),
                 aff0=qn,
                 summary='Possible cryptographic constants have been found.',
                 desc='''\
 Possible cryptographic constants has been found in the application binary.
 '''
               ))
       except IndexError:
         pass
 
   async def _do_detect_case2(self) -> None:
     # XXX: Crude detection
     def should_be_secret(store: APKStore, k: Op, val: str) -> bool:
-      name = store.query().qualname_of(k)
+      name = store.query().qualname_of(k.addr)
       if name:
         return name.lower() in ['inapp','billing','iab','sku','store','key']
       else:
         return False
 
     pat = '^M[C-I][0-9A-Za-z+/=-]{48,}'
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.consts(InvocationPattern('const-string', pat)):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
-      val = cl.p[1].v
+      val = self._an.get_param(cl, 1).v
       typ = self._inspect_value_type(val)
       param = self._build_template_params(val, typ)
       self._helper.raise_issue(self._helper.build_issue(
         sigid=self._id,
         cvss=self._cvss_nonkey if param['nonkey'] else (self._cvss_pubkey if not param['private'] else self._cvss_privkey),
         cfd='certain' if typ else ('firm' if should_be_secret(store, cl, val) else 'tentative'),
         title=('insecure cryptography: {key} detected' if not param['nonkey'] else '{key} detected').format(**param),
@@ -251,76 +251,77 @@
         return algo.upper()
       else:
         if x.curve[0] == 'named':
           return '{} [{}]'.format(algo.upper(), str(x.curve[1]))
         else:
           return '{}'.format(algo.upper())
 
-
 class CryptoEcbDetector(SignatureMixin):
   _id = 'crypto-ecb'
   _cvss = 'CVSS:3.0/AV:P/AC:H/PR:N/UI:N/S:U/C:L/I:L/A:L/'
 
   @staticmethod
   def create(helper: SignatureHelper) -> Signature:
     return CryptoEcbDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id: dict(e=self.detect, d='Detects ECB mode ciphers')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
-    store = context.store()
-    q = store.query()
-    for cl in q.invocations(InvocationPattern('invoke-static', r'Ljavax/crypto/Cipher;->getInstance\(Ljava/lang/String;.*?\)')):
-      qn = q.qualname_of(cl)
-      if context.is_qualname_excluded(qn):
-        continue
-      try:
-        target_val = DataFlow(q).solved_possible_constant_data_in_invocation(cl, 0)
-        if any((('ECB' in x or '/' not in x) and 'RSA' not in x) for x in target_val):
-          self._helper.raise_issue(self._helper.build_issue(
-            sigid=self._id,
-            cvss=self._cvss,
-            cfd='certain',
-            title='insecure cryptography: cipher might be operating in ECB mode',
-            info0=','.join(target_val),
-            aff0=qn,
-            summary='The application might be using ciphers in ECB mode.',
-            desc='''\
-            The application might be using symmetric ciphers in ECB mode.  ECB mode is the most basic operating mode that independently transform data blocks.  Indepent transformation leaks information about distribution in plaintext.
-''',
-            sol='''\
-Use CBC or CTR mode.
-'''
-          ))
-      except (DataFlow.NoSuchValueError):
-        pass
+    q: APKQuery
+    context = self._get_context()
+    with context.store().query().scoped() as q:
+      for cl in q.invocations(InvocationPattern('invoke-static', r'Ljavax/crypto/Cipher;->getInstance\(Ljava/lang/String;.*?\)')):
+        qn = q.qualname_of(cl.addr)
+        if context.is_qualname_excluded(qn):
+          continue
+        try:
+          target_val = DataFlow(q).solved_possible_constant_data_in_invocation(cl, 0)
+          if any((('ECB' in x or '/' not in x) and 'RSA' not in x) for x in target_val):
+            self._helper.raise_issue(self._helper.build_issue(
+              sigid=self._id,
+              cvss=self._cvss,
+              cfd='certain',
+              title='insecure cryptography: cipher might be operating in ECB mode',
+              info0=','.join(target_val),
+              aff0=qn,
+              summary='The application might be using ciphers in ECB mode.',
+              desc='''\
+              The application might be using symmetric ciphers in ECB mode.  ECB mode is the most basic operating mode that independently transform data blocks.  Indepent transformation leaks information about distribution in plaintext.
+  ''',
+              sol='''\
+  Use CBC or CTR mode.
+  '''
+            ))
+        except DataFlow.NoSuchValueError:
+          pass
 
 class CryptoNonRandomXorDetector(SignatureMixin):
   _id = 'crypto-xor'
   _cvss = 'CVSS:3.0/AV:P/AC:L/PR:N/UI:N/S:C/C:L/I:L/A:L/'
 
   @staticmethod
   def create(helper: SignatureHelper) -> Signature:
     return CryptoNonRandomXorDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id: dict(e=self.detect, d='Detects Vernum cipher usage with static keys')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
-    store = context.store()
-    q = store.query()
-    for cl in q.ops_of('xor-int/lit8'):
-      qn = q.qualname_of(cl)
-      if context.is_qualname_excluded(qn):
-        continue
-      target_val = int(cl.p[2].v, 16)
-      if (cl.p[0].v == cl.p[1].v) and target_val > 1:
-        self._helper.raise_issue(self._helper.build_issue(
-          sigid=self._id,
-          cvss=self._cvss,
-          title='insecure cryptography: non-random XOR cipher',
-          info0=f'0x{target_val:02x}',
-          aff0=q.qualname_of(cl)
-        ))
+    q: APKQuery
+    context = self._get_context()
+    with context.store().query().scoped() as q:
+      for cl in q.ops_of('xor-int/lit8'):
+        qn = q.qualname_of(cl.addr)
+        if context.is_qualname_excluded(qn):
+          continue
+        m = re.search(r'([pv][0-9]+), \1, (0x[0-9a-f]+)$', cl.l)
+        if m:
+          target_val = int(m.group(2), 16)
+          if target_val > 1:
+            self._helper.raise_issue(self._helper.build_issue(
+              sigid=self._id,
+              cvss=self._cvss,
+              title='insecure cryptography: non-random XOR cipher',
+              info0=f'0x{target_val:02x}',
+              aff0=qn
+            ))
```

### Comparing `trueseeing-2.2.2/trueseeing/sig/android/fingerprint.py` & `trueseeing-2.2.4/trueseeing/sig/android/fingerprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import io
 import os
 import re
 
-from trueseeing.core.model.sig import SignatureMixin
-from trueseeing.core.android.model.code import InvocationPattern
+from trueseeing.core.android.model import InvocationPattern
+from trueseeing.core.android.model import SignatureMixin
 from trueseeing.core.android.analysis.flow import DataFlow
 
 if TYPE_CHECKING:
   from typing import Iterable, Optional, List, Dict, Any, Set
   from trueseeing.api import Signature, SignatureHelper, SignatureMap
   from trueseeing.core.model.issue import IssueConfidence
 
@@ -99,15 +99,15 @@
       return not cls._suffixes_top.looks_public(shared)
     elif len(shared) > 2:
       return True
     else:
       return not cls._suffixes_public.looks_public(shared)
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     q = context.store().query()
     package = context.parsed_manifest().xpath('/manifest/@package', namespaces=dict(android='http://schemas.android.com/apk/res/android'))[0]
 
     packages: Dict[str, List[str]] = dict()
     for fn in (context.source_name_of_disassembled_class(r) for r in context.disassembled_classes()):
       # XXX exclude packages
       family = self._package_family_of(self._package_name_of(fn))
@@ -126,15 +126,15 @@
         cvss=self._cvss,
         title='detected library',
         info0=f'{p} (score: {len(packages[p])})',
       ))
 
     for p in reversed(sorted(packages.keys(), key=len)):
       for k in q.consts_in_package(p, InvocationPattern('const-string', r'[0-9]+\.[0-9]+|(19|20)[0-9]{2}[ /-]')):
-        ver = k.p[1].v
+        ver = self._an.get_param(k, 1).v
         if not re.search(r'^/|:[0-9]+|\\|://', ver):
           comps = ver.split('.')
           if len(comps) > 4:
             continue
           if ' and ' not in ver and re.match('^[0-9]|^v[0-9]', ver):
             if len(comps) < 4 or self._comp4_looks_like_version(comps):
               self._helper.raise_issue(self._helper.build_issue(
@@ -205,15 +205,15 @@
     return {self._id:dict(e=self.detect, d='Detects obfuscators')}
 
   @classmethod
   def _class_name_of(self, path: str) -> str:
     return path.replace('.smali', '').replace('/', '.')
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     for c in (self._class_name_of(context.source_name_of_disassembled_class(r)) for r in context.disassembled_classes()):
       m = re.search(r'(?:^|\.)(.)$', c)
       if m and m.group(1) not in self._whitelist:
         self._helper.raise_issue(self._helper.build_issue(sigid=self._id, cfd='certain', cvss=self._cvss_true, title='detected obfuscator', info0='ProGuard'))
         break
     else:
       self._helper.raise_issue(self._helper.build_issue(sigid=self._id, cvss=self._cvss_false, title='lack of obfuscation'))
@@ -261,21 +261,21 @@
             yield dict(type_='possible FQDN', value=[hostlike], cfd=confidence)
 
   async def detect(self) -> None:
     from importlib.resources import files
     with (files('trueseeing')/'libs'/'tlds.txt').open('r', encoding='utf-8') as f:
       self._re_tlds = re.compile('^(?:{})$'.format('|'.join(re.escape(l.strip()) for l in f if l and not l.startswith('#'))), flags=re.IGNORECASE)
 
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     q = context.store().query()
     for cl in q.consts(InvocationPattern('const-string', r'://|^/[{}$%a-zA-Z0-9_-]+(/[{}$%a-zA-Z0-9_-]+)+|^[a-zA-Z0-9-]+(\.[a-zA-Z0-9-]+)+(:[0-9]+)?$')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
-      for match in self._analyzed(cl.p[1].v, qn):
+      for match in self._analyzed(self._an.get_param(cl, 1).v, qn):
         for v in match['value']:
           self._helper.raise_issue(self._helper.build_issue(sigid=self._id, cfd=match['cfd'], cvss=match.get('cvss', self._cvss), title=f'detected {match["type_"]}', info0=v, aff0=qn))
     for name, val in context.string_resources():
       for match in self._analyzed(val):
         for v in match['value']:
           self._helper.raise_issue(self._helper.build_issue(sigid=self._id, cfd=match['cfd'], cvss=match.get('cvss', self._cvss), title=f'detected {match["type_"]}', info0=v, aff0=f'R.string.{name}'))
 
@@ -290,24 +290,24 @@
   def create(helper: SignatureHelper) -> Signature:
     return NativeMethodDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects natively defined methods')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for op in q.methods_with_modifier('native'):
       self._helper.raise_issue(self._helper.build_issue(
         sigid=self._id,
         cvss=self._cvss,
         title=self._summary,
         summary=self._synopsis,
-        aff0=q.qualname_of(op)
+        aff0=q.qualname_of(op.addr)
       ))
 
 class NativeArchDetector(SignatureMixin):
   _id = 'detect-native-arch'
   _cvss = 'CVSS:3.0/AV:P/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:N/'
   _summary = 'Supported architectures'
   _synopsis = "The application has native codes for some architectures."
@@ -316,15 +316,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return NativeArchDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects supported architectures')}
 
   async def detect(self) -> None:
-    for d in self._helper.get_context().require_type('apk').store().query().file_find('root/lib/%'):
+    for d in self._get_context().store().query().file_find('root/lib/%'):
       if re.search(r'arm|x86|mips', d):
         arch = d.split('/')[2]
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cvss=self._cvss,
           title=self._summary,
           info0=arch,
@@ -364,25 +364,25 @@
   def create(helper: SignatureHelper) -> Signature:
     return ReflectionDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects reflections')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.invocations(InvocationPattern('invoke-', '^Ljavax?.*/(Class|Method|Field);->|^Ljava/lang/[A-Za-z]*?ClassLoader;->')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if qn:
         if context.is_qualname_excluded(qn):
           continue
         if any(re.match(x, qn) for x in self._blacklist_caller):
           continue
-      ct = q.method_call_target_of(cl)
+      ct = q.method_call_target_of(cl.addr)
       if ct is None:
         continue
       if any(re.match(x, ct) for x in self._blacklist_meth):
         continue
       if 'ClassLoader;->' in ct:
         try:
           xs = DataFlow(q).solved_possible_constant_data_in_invocation(cl, 0)
```

### Comparing `trueseeing-2.2.2/trueseeing/sig/android/manifest.py` & `trueseeing-2.2.4/trueseeing/sig/android/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 import itertools
 import re
 
-from trueseeing.core.model.sig import SignatureMixin
+from trueseeing.core.android.model import SignatureMixin
 
 if TYPE_CHECKING:
   from trueseeing.api import Signature, SignatureHelper, SignatureMap
 
 class ManifestOpenPermissionDetector(SignatureMixin):
   _id = 'manifest-open-permission'
   _cvss = 'CVSS:3.0/AV:P/AC:H/PR:N/UI:R/S:U/C:N/I:N/A:N/'
@@ -17,15 +17,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ManifestOpenPermissionDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects declarated permissions')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
 
     # TBD: compare with actual permission needs
     for p in context.permissions_declared():
       self._helper.raise_issue(self._helper.build_issue(
         sigid=self._id,
         cfd='certain',
         cvss=self._cvss,
@@ -59,15 +59,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ManifestManipActivity(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects exported Activity')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     policy = ComponentNamePolicy()
     ns = dict(android='http://schemas.android.com/apk/res/android')
 
     for name in set(itertools.chain(
         context.parsed_manifest().xpath('//activity[not(@android:permission)]/intent-filter/../@android:name', namespaces=ns),
         context.parsed_manifest().xpath('//activity[not(@android:permission) and (@android:exported="true")]/@android:name', namespaces=ns),
     )):
@@ -107,15 +107,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ManifestManipBroadcastReceiver(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects exported BroadcastReceiver')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     policy = ComponentNamePolicy()
     ns = dict(android='http://schemas.android.com/apk/res/android')
 
     # FIXME: catch API < 9
     for name in set(itertools.chain(
         context.parsed_manifest().xpath('//receiver[not(@android:permission) and not(@android:exported="false")]/intent-filter/../@android:name', namespaces=ns),
         context.parsed_manifest().xpath('//receiver[not(@android:permission) and (@android:exported="true")]/@android:name', namespaces=ns),
@@ -156,15 +156,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ManifestManipContentProvider(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects exported ContentProvider')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     policy = ComponentNamePolicy()
     ns = dict(android='http://schemas.android.com/apk/res/android')
 
     for name in set(itertools.chain(
         context.parsed_manifest().xpath('//provider[not(@android:permission)]/intent-filter/../@android:name', namespaces=dict(android='http://schemas.android.com/apk/res/android')),
         context.parsed_manifest().xpath('//provider[not(@android:permission) and (@android:exported="true")]/@android:name', namespaces=dict(android='http://schemas.android.com/apk/res/android')),
     )):
@@ -211,15 +211,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ManifestManipBackup(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects enabled backup bit')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     manif = context.parsed_manifest()
     for e in manif.xpath('//application[not(@android:allowBackup="false")]', namespaces=dict(android='http://schemas.android.com/apk/res/android')):
       if min(context.get_target_sdk_version(), context.get_min_sdk_version()) < 31:
         fbc_exists = (e.attrib.get('{{{ns}}}fullBackupContent'.format(ns='http://schemas.android.com/apk/res/android')) is not None)
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cfd='certain' if not fbc_exists else 'tentative',
@@ -249,15 +249,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ManifestDebuggable(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects enabled debug bits')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     if context.parsed_manifest().xpath('//application[@android:debuggable="true"]', namespaces=dict(android='http://schemas.android.com/apk/res/android')):
       self._helper.raise_issue(self._helper.build_issue(
         sigid=self._id,
         cfd='certain',
         cvss=self._cvss,
         title='app is debuggable',
         aff0='AndroidManifest.xml',
@@ -278,15 +278,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ManifestCleartextPermitted(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects usesCleartextTraffic flag')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     manif = context.parsed_manifest()
     api_level = context.get_min_sdk_version()
     if api_level < 24:
       if not manif.xpath('//application[@android:usesCleartextTraffic="false"]', namespaces=dict(android='http://schemas.android.com/apk/res/android')):
         self._raise('AndroidManifest.xml')
     else:
       for e in manif.xpath('//application', namespaces=dict(android='http://schemas.android.com/apk/res/android')):
```

### Comparing `trueseeing-2.2.2/trueseeing/sig/android/privacy.py` & `trueseeing-2.2.4/trueseeing/sig/android/privacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 import re
 
-from trueseeing.core.android.model.code import InvocationPattern
+from trueseeing.core.android.model import InvocationPattern
 from trueseeing.core.android.analysis.flow import DataFlow
-from trueseeing.core.model.sig import SignatureMixin
+from trueseeing.core.android.model import SignatureMixin
 
 if TYPE_CHECKING:
   from typing import Optional
+  from trueseeing.core.android.model import Op
   from trueseeing.core.android.db import APKQuery
-  from trueseeing.core.android.model.code import Op
   from trueseeing.api import Signature, SignatureHelper, SignatureMap
 
 class PrivacyDeviceIdDetector(SignatureMixin):
   _id = 'privacy-device-id'
   description = 'Detects device fingerprinting behavior'
   _cvss = 'CVSS:3.0/AV:N/AC:H/PR:L/UI:R/S:C/C:L/I:N/A:N/'
   _summary = 'privacy concerns'
@@ -23,15 +23,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return PrivacyDeviceIdDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects device fingerprinting behavior')}
 
   def analyzed(self, q: APKQuery, op: Op) -> Optional[str]:
-    x = op.p[1].v
+    x = self._an.get_param(op, 1).v
     if re.search(r'Landroid/provider/Settings\$Secure;->getString\(Landroid/content/ContentResolver;Ljava/lang/String;\)Ljava/lang/String;', x):
       try:
         if DataFlow(q).solved_constant_data_in_invocation(op, 1) == 'android_id':
           return 'ANDROID_ID'
         else:
           return None
       except DataFlow.NoSuchValueError:
@@ -45,30 +45,30 @@
     elif re.search(r'Landroid/bluetooth/BluetoothAdapter;->getAddress\(\)Ljava/lang/String;', x):
       return 'L2 address (Bluetooth)'
     elif re.search(r'Landroid/net/wifi/WifiInfo;->getMacAddress\(\)Ljava/lang/String;|Ljava/net/NetworkInterface;->getHardwareAddress\(\)', x):
       return 'L2 address (Wi-Fi)'
     return None
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for op in q.invocations(InvocationPattern('invoke-', r'Landroid/provider/Settings\$Secure;->getString\(Landroid/content/ContentResolver;Ljava/lang/String;\)Ljava/lang/String;|Landroid/telephony/TelephonyManager;->getDeviceId\(\)Ljava/lang/String;|Landroid/telephony/TelephonyManager;->getSubscriberId\(\)Ljava/lang/String;|Landroid/telephony/TelephonyManager;->getLine1Number\(\)Ljava/lang/String;|Landroid/bluetooth/BluetoothAdapter;->getAddress\(\)Ljava/lang/String;|Landroid/net/wifi/WifiInfo;->getMacAddress\(\)Ljava/lang/String;|Ljava/net/NetworkInterface;->getHardwareAddress\(\)')):
-      qn = q.qualname_of(op)
+      qn = q.qualname_of(op.addr)
       if context.is_qualname_excluded(qn):
         continue
       val_type = self.analyzed(q, op)
       if val_type is not None:
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cfd='certain',
           cvss=self._cvss,
           title=self._summary,
           info0=f'getting {val_type}',
-          aff0=q.qualname_of(op)
+          aff0=q.qualname_of(op.addr)
         ))
 
 class PrivacySMSDetector(SignatureMixin):
   _id = 'privacy-sms'
   _cvss = 'CVSS:3.0/AV:N/AC:H/PR:L/UI:R/S:C/C:L/I:N/A:N/'
   _summary = 'privacy concerns'
 
@@ -76,51 +76,51 @@
   def create(helper: SignatureHelper) -> Signature:
     return PrivacySMSDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects SMS-related behavior')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for op in q.invocations(InvocationPattern('invoke-', r'Landroid/net/Uri;->parse\(Ljava/lang/String;\)Landroid/net/Uri;')):
-      qn = q.qualname_of(op)
+      qn = q.qualname_of(op.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         if DataFlow(q).solved_constant_data_in_invocation(op, 0).startswith('content://sms/'):
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cfd='certain',
             cvss=self._cvss,
             title=self._summary,
             info0='accessing SMS',
-            aff0=q.qualname_of(op)
+            aff0=q.qualname_of(op.addr)
           ))
       except DataFlow.NoSuchValueError:
         pass
 
     for op in q.invocations(InvocationPattern('invoke-', r'Landroid/telephony/SmsManager;->send')):
-      qn = q.qualname_of(op)
+      qn = q.qualname_of(op.addr)
       if context.is_qualname_excluded(qn):
         continue
       self._helper.raise_issue(self._helper.build_issue(
         sigid=self._id,
         cfd='certain',
         cvss=self._cvss,
         title=self._summary,
         info0='sending SMS',
-        aff0=q.qualname_of(op)
+        aff0=q.qualname_of(op.addr)
       ))
 
     for op in q.invocations(InvocationPattern('invoke-', r'Landroid/telephony/SmsMessage;->createFromPdu\(')):
-      qn = q.qualname_of(op)
+      qn = q.qualname_of(op.addr)
       if context.is_qualname_excluded(qn):
         continue
       self._helper.raise_issue(self._helper.build_issue(
         sigid=self._id,
         cvss=self._cvss,
         title=self._summary,
         info0='intercepting incoming SMS',
-        aff0=q.qualname_of(op)
+        aff0=q.qualname_of(op.addr)
       ))
```

### Comparing `trueseeing-2.2.2/trueseeing/sig/android/security.py` & `trueseeing-2.2.4/trueseeing/sig/android/security.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import TYPE_CHECKING
 
 import itertools
 import io
 import re
 import os
 
-from trueseeing.core.android.model.code import InvocationPattern
+from trueseeing.core.android.model import InvocationPattern
+from trueseeing.core.android.model import SignatureMixin
 from trueseeing.core.android.analysis.flow import DataFlow
-from trueseeing.core.model.sig import SignatureMixin
 from trueseeing.core.ui import ui
 
 if TYPE_CHECKING:
   from typing import Iterable, Optional, Set, Tuple, Any, TypeVar, Dict
   from trueseeing.api import Signature, SignatureHelper, SignatureMap
   from trueseeing.core.model.issue import IssueConfidence
   T = TypeVar('T')
@@ -26,31 +26,31 @@
   def create(helper: SignatureHelper) -> Signature:
     return SecurityFilePermissionDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects insecure file creation')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.invocations(InvocationPattern('invoke-virtual', r'Landroid/content/Context;->openFileOutput\(Ljava/lang/String;I\)')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         target_val = int(DataFlow(q).solved_constant_data_in_invocation(cl, 1), 16)
         if target_val & 3:
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cfd='certain',
             cvss=self._cvss,
             title=self._summary,
             info0={1: 'MODE_WORLD_READABLE', 2: 'MODE_WORLD_WRITEABLE'}[target_val],
-            aff0=q.qualname_of(cl)
+            aff0=q.qualname_of(cl.addr)
           ))
       except (DataFlow.NoSuchValueError):
         pass
 
 
 class SecurityTlsInterceptionDetector(SignatureMixin):
   _id = 'security-tls-interception'
@@ -62,15 +62,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return SecurityTlsInterceptionDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects certificate (non-)pinning')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     pin_nsc = False
     if context.get_min_sdk_version() > 23:
       if not context.parsed_manifest().xpath('//application[@android:debuggable="true"]', namespaces=dict(android='http://schemas.android.com/apk/res/android')):
         pin_nsc = True
 
     for fn, xp in context.xml_resources():
       if 'network-security-config' in xp.tag.lower():
@@ -100,25 +100,25 @@
             sigid=self._id,
             cvss=self._cvss,
             title=self._summary,
             info0='no pinning detected'
           ))
 
   def _do_detect_plain_pins_x509(self) -> Set[str]:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     pins: Set[str] = set()
     store = context.store()
     q = store.query()
-    for m in q.methods_in_class('checkServerTrusted', 'X509TrustManager'):
-      if any(q.matches_in_method(m, InvocationPattern('verify', ''))):
-        classname = q.class_name_of(q.class_of_method(m))
+    for addr in q.methods_in_class('checkServerTrusted', 'X509TrustManager'):
+      if any(q.matches_in_method(addr, InvocationPattern('verify', ''))):
+        classname = q.class_name_of(addr)
         if classname:
           pins.add(classname)
-      if any(q.matches_in_method(m, InvocationPattern('throw', ''))):
-        classname = q.class_name_of(q.class_of_method(m))
+      if any(q.matches_in_method(addr, InvocationPattern('throw', ''))):
+        classname = q.class_name_of(addr)
         if classname:
           pins.add(classname)
 
     if pins:
       # XXX crude detection
       custom_sslcontext_detected = False
       for cl in q.invocations(InvocationPattern('invoke-virtual', 'Ljavax/net/ssl/SSLContext;->init')):
@@ -129,20 +129,20 @@
         return set()
       else:
         return pins
     else:
       return pins
 
   def _do_detect_plain_pins_hostnameverifier(self) -> Set[str]:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     pins: Set[str] = set()
     q = context.store().query()
-    for m in itertools.chain(q.methods_in_class('verify(Ljava/lang/String;Ljavax/net/ssl/SSLSession;)Z', 'HostnameVerifier')):
-      if any(q.matches_in_method(m, InvocationPattern('invoke', 'contains|equals|verify|Ljavax/net/ssl/SSLSession;->getPeerCertificates'))):
-        classname = q.class_name_of(q.class_of_method(m))
+    for addr in itertools.chain(q.methods_in_class('verify(Ljava/lang/String;Ljavax/net/ssl/SSLSession;)Z', 'HostnameVerifier')):
+      if any(q.matches_in_method(addr, InvocationPattern('invoke', 'contains|equals|verify|Ljavax/net/ssl/SSLSession;->getPeerCertificates'))):
+        classname = q.class_name_of(addr)
         if classname:
           pins.add(classname)
     return pins
 
 
 class LayoutSizeGuesser:
   _xmlns_android = '{http://schemas.android.com/apk/res/android}'
@@ -233,15 +233,15 @@
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects tamperable WebView')}
 
   async def detect(self) -> None:
     import lxml.etree as ET
     from functools import reduce
 
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     targets = {'WebView','XWalkView','GeckoView'}
 
     more = True
     while more:
       more = False
@@ -266,26 +266,26 @@
               aff0=context.source_name_of_disassembled_resource(fn)
             ))
           except KeyError as e:
             ui.warn(f'SecurityTamperableWebViewDetector.do_detect: missing key {e}')
 
     # XXX: crude detection
     for op in q.invocations(InvocationPattern('invoke-', ';->loadUrl')):
-      qn = q.qualname_of(op)
+      qn = q.qualname_of(op.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         v = DataFlow(q).solved_constant_data_in_invocation(op, 0)
         if v.startswith('http://'):
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cvss=self._cvss2,
             title=self._summary2,
             info0=v,
-            aff0=q.qualname_of(op)
+            aff0=q.qualname_of(op.addr)
           ))
       except DataFlow.NoSuchValueError:
         pass
 
 
 class SecurityInsecureWebViewDetector(SignatureMixin):
   _id = 'security-insecure-webview'
@@ -314,99 +314,99 @@
   def _first(cls, xs: Iterable[T], default: Optional[T] = None) -> Optional[T]:
     try:
       return list(itertools.islice(xs, 1))[0]
     except IndexError:
       return default
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     query = store.query()
 
     targets = set()
     seeds = {'WebView','XWalkView','GeckoView'}
 
     more = True
     while more:
       more = False
-      for cl in store.query().related_classes('|'.join(seeds)):
-        name = store.query().class_name_of(cl)
+      for addr in store.query().related_classes('|'.join(seeds)):
+        name = store.query().class_name_of(addr)
         if name not in targets:
           targets.add(name)
           more = True
     for seed in seeds:
       targets.add(f'L.*{seed};')
 
     # XXX: Crude detection
     # https://developer.android.com/reference/android/webkit/WebView.html#addJavascriptInterface(java.lang.Object,%2520java.lang.String)
     if context.get_min_sdk_version() <= 16:
       for p in query.invocations(InvocationPattern('invoke-virtual', 'Landroid/webkit/WebSettings;->setJavaScriptEnabled')):
-        qn = query.qualname_of(p)
+        qn = query.qualname_of(p.addr)
         if context.is_qualname_excluded(qn):
           continue
         try:
           if DataFlow(query).solved_constant_data_in_invocation(p, 0):
             for target in targets:
-              for q in query.invocations_in_class(p, InvocationPattern('invoke-virtual', f'{target}->addJavascriptInterface')):
+              for q in query.invocations_in_class(p.addr, InvocationPattern('invoke-virtual', f'{target}->addJavascriptInterface')):
                 try:
                   if DataFlow(query).solved_constant_data_in_invocation(q, 0):
                     self._helper.raise_issue(self._helper.build_issue(
                       sigid=self._id,
                       cvss=self._cvss,
                       title=self._summary1,
-                      aff0=query.qualname_of(q)
+                      aff0=query.qualname_of(q.addr)
                     ))
                 except (DataFlow.NoSuchValueError):
                   self._helper.raise_issue(self._helper.build_issue(
                     sigid=self._id,
                     cfd='tentative',
                     cvss=self._cvss,
                     title=self._summary1,
-                    aff0=query.qualname_of(q)
+                    aff0=query.qualname_of(q.addr)
                   ))
         except (DataFlow.NoSuchValueError):
           pass
 
     # https://developer.android.com/reference/android/webkit/WebSettings#setMixedContentMode(int)
     if context.get_min_sdk_version() >= 21:
       for q in query.invocations(InvocationPattern('invoke-virtual', 'Landroid/webkit/WebSettings;->setMixedContentMode')):
-        qn = query.qualname_of(q)
+        qn = query.qualname_of(q.addr)
         if context.is_qualname_excluded(qn):
           continue
         try:
           val = int(DataFlow(query).solved_constant_data_in_invocation(q, 0), 16)
           if val == 0:
             self._helper.raise_issue(self._helper.build_issue(
               sigid=self._id,
               cvss=self._cvss2,
               title=self._summary2,
               info0='MIXED_CONTENT_ALWAYS_ALLOW',
-              aff0=query.qualname_of(q)))
+              aff0=query.qualname_of(q.addr)))
           elif val == 2:
             self._helper.raise_issue(self._helper.build_issue(
               sigid=self._id,
               cvss=self._cvss2b,
               title=self._summary2b,
               info0='MIXED_CONTENT_COMPATIBILITY_MODE',
-              aff0=query.qualname_of(q)))
+              aff0=query.qualname_of(q.addr)))
         except (DataFlow.NoSuchValueError):
           pass
     else:
       for target in targets:
         for q in query.invocations(InvocationPattern('invoke-virtual', f'{target}->loadUrl')):
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cvss=self._cvss,
             title=self._summary2,
             info0='mixed mode always enabled in API < 21',
-            aff0=query.qualname_of(q)
+            aff0=query.qualname_of(q.addr)
           ))
 
     for op in query.invocations(InvocationPattern('invoke-', ';->loadUrl')):
-      qn = query.qualname_of(op)
+      qn = query.qualname_of(op.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         v = DataFlow(query).solved_constant_data_in_invocation(op, 0)
         if v.startswith('file:///android_asset/'):
           path = v.replace('file:///android_asset/', 'assets/')
           blob = query.file_get(f'root/{path}')
@@ -417,24 +417,24 @@
             if csp is None or any([(x in csp.lower()) for x in ('unsafe', 'http:')]):
               self._helper.raise_issue(self._helper.build_issue(
                 sigid=self._id,
                 cvss=self._cvss3,
                 title=self._summary3,
                 info0=path,
                 info1='default' if csp is None else csp,
-                aff0=query.qualname_of(op)
+                aff0=query.qualname_of(op.addr)
               ))
             else:
               self._helper.raise_issue(self._helper.build_issue(
                 sigid=self._id,
                 cvss=self._cvss4,
                 title=self._summary4,
                 info0=path,
                 info1=csp,
-                aff0=query.qualname_of(op)
+                aff0=query.qualname_of(op.addr)
               ))
       except DataFlow.NoSuchValueError:
         pass
 
 class FormatStringDetector(SignatureMixin):
   _id = 'security-format-string'
   _summary = 'detected format string'
@@ -449,28 +449,28 @@
 
   def _analyzed(self, x: str) -> Iterable[Dict[str, Any]]:
     if re.search(r'%s', x):
       if re.search(r'(://|[<>/&?])', x):
         yield dict(cfd='firm', value=x)
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     q = context.store().query()
     for cl in q.consts(InvocationPattern('const-string', r'%s')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
-      for t in self._analyzed(cl.p[1].v):
+      for t in self._analyzed(self._an.get_param(cl, 1).v):
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cfd=t['cfd'],
           cvss=self._cvss,
           title=self._summary,
           info0=t['value'],
-          aff0=q.qualname_of(cl)
+          aff0=q.qualname_of(cl.addr)
         ))
     for name, val in context.string_resources():
       for t in self._analyzed(val):
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cfd=t['cfd'],
           cvss=self._cvss,
@@ -488,69 +488,71 @@
   def create(helper: SignatureHelper) -> Signature:
     return LogDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects logging activities')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.invocations(InvocationPattern('invoke-', r'L.*->([dwie]|debug|error|exception|warning|info|notice|wtf)\(Ljava/lang/String;Ljava/lang/String;.*?Ljava/lang/(Throwable|.*?Exception);|L.*;->print(ln)?\(Ljava/lang/String;|LException;->printStackTrace\(')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
-      if 'print' not in cl.p[1].v:
+
+      func = self._an.get_param(cl, 1).v
+      if 'print' not in func:
         try:
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cfd='tentative',
             cvss=self._cvss,
             title=self._summary,
-            info0=cl.p[1].v,
+            info0=func,
             info1=DataFlow(q).solved_constant_data_in_invocation(cl, 1),
-            aff0=q.qualname_of(cl)
+            aff0=q.qualname_of(cl.addr)
           ))
         except (DataFlow.NoSuchValueError):
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cfd='tentative',
             cvss=self._cvss,
             title=self._summary,
-            info0=cl.p[1].v,
-            aff0=q.qualname_of(cl)
+            info0=func,
+            aff0=q.qualname_of(cl.addr)
           ))
-      elif 'Exception;->' not in cl.p[1].v:
+      elif 'Exception;->' not in func:
         try:
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cfd='tentative',
             cvss=self._cvss,
             title=self._summary,
-            info0=cl.p[1].v,
+            info0=func,
             info1=DataFlow(q).solved_constant_data_in_invocation(cl, 0),
-            aff0=q.qualname_of(cl)
+            aff0=q.qualname_of(cl.addr)
           ))
         except (DataFlow.NoSuchValueError):
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cfd='tentative',
             cvss=self._cvss,
             title=self._summary,
-            info0=cl.p[1].v,
-            aff0=q.qualname_of(cl)
+            info0=func,
+            aff0=q.qualname_of(cl.addr)
           ))
       else:
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cfd='tentative',
           cvss=self._cvss,
           title=self._summary,
-          info0=cl.p[1].v,
-          aff0=q.qualname_of(cl)
+          info0=func,
+          aff0=q.qualname_of(cl.addr)
         ))
 
 class ADBProbeDetector(SignatureMixin):
   _id = 'security-adb-detect'
   _cvss = 'CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:N/'
   _summary = 'USB debugging detection'
   _synopsis = 'The application is probing for USB debugging (adbd.)'
@@ -559,28 +561,28 @@
   def create(helper: SignatureHelper) -> Signature:
     return ADBProbeDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects probe of adbd status.')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.invocations(InvocationPattern('invoke-', r'^Landroid/provider/Settings\$(Global|Secure);->getInt\(')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       for found in DataFlow(q).solved_possible_constant_data_in_invocation(cl, 1):
         if found == 'adb_enabled':
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cvss=self._cvss,
             title=self._summary,
-            aff0=q.qualname_of(cl),
+            aff0=q.qualname_of(cl.addr),
             summary=self._synopsis,
           ))
 
 class ClientXSSJQDetector(SignatureMixin):
   _id = 'security-cxss-jq'
   _cvss = 'CVSS:3.0/AV:N/AC:H/PR:N/UI:R/S:U/C:L/I:L/A:N/'
   _summary = 'Potential client-side XSS (JQuery)'
@@ -590,15 +592,15 @@
   def create(helper: SignatureHelper) -> Signature:
     return ClientXSSJQDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects potential client-side XSS vector in JQuery-based apps')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     for fn, blob in context.store().query().file_enum(pat='root/assets/%.js'):
       f = io.StringIO(blob.decode('utf-8', errors='ignore'))
       for l in f:
         for m in re.finditer(r'\.html\(', l):
           self._helper.raise_issue(self._helper.build_issue(
             sigid=self._id,
             cvss=self._cvss,
@@ -620,19 +622,19 @@
   def create(helper: SignatureHelper) -> Signature:
     return SecurityFileWriteDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects file creation')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.invocations(InvocationPattern('invoke-virtual', r'Landroid/content/Context;->openFileOutput\(Ljava/lang/String;I\)')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         target_val = DataFlow(q).solved_constant_data_in_invocation(cl, 0)
       except DataFlow.NoSuchValueError:
         target_val = '(unknown name)'
 
@@ -640,44 +642,44 @@
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cfd='certain',
           cvss=self._cvss1,
           title=self._summary1,
           summary=self._synopsis1,
           info0=target_val,
-          aff0=q.qualname_of(cl)
+          aff0=q.qualname_of(cl.addr)
         ))
       else:
         self._helper.raise_issue(self._helper.build_issue(
           sigid=self._id,
           cfd='certain',
           cvss=self._cvss2,
           title=self._summary2,
           summary=self._synopsis2,
           info0=target_val,
-          aff0=q.qualname_of(cl)
+          aff0=q.qualname_of(cl.addr)
         ))
 
     for cl in q.invocations(InvocationPattern('invoke-direct', r'java/io/File(Writer|OutputStream)?;-><init>\(Ljava/lang/String;\)')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         target_val = DataFlow(q).solved_constant_data_in_invocation(cl, 0)
 
         if re.search(r'debug|log|info|report|screen|err|tomb|drop', target_val):
           if not re.search(r'^/proc/|^/sys/', target_val):
             self._helper.raise_issue(self._helper.build_issue(
               sigid=self._id,
               cfd='tentative',
               cvss=self._cvss1,
               title=self._summary1,
               summary=self._synopsis1,
               info0=target_val,
-              aff0=q.qualname_of(cl)
+              aff0=q.qualname_of(cl.addr)
             ))
       except DataFlow.NoSuchValueError:
         target_val = '(unknown name)'
 
 class SecurityInsecureRootedDetector(SignatureMixin):
   _id = 'security-insecure-rooted'
   _cvss = 'CVSS:3.0/AV:P/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:N/'
@@ -689,37 +691,37 @@
   def create(helper: SignatureHelper) -> Signature:
     return SecurityInsecureRootedDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects insecure rooted device probes')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
 
     attestations: Dict[str, Any] = dict()
     path_based_detection_attempt: Dict[str, Any] = dict()
     confidence: Dict[str, IssueConfidence] = dict()
 
     for cl in q.invocations(InvocationPattern('invoke-', r'Lcom/google/android/gms/safetynet/SafetyNetClient;->attest\(\[BLjava/lang/String;\)')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       # XXX: crude detection
-      verdict_accesses = list(q.consts_in_class(cl, InvocationPattern('const-string', r'ctsProfileMatch|basicIntegrity')))
+      verdict_accesses = list(q.consts_in_class(cl.addr, InvocationPattern('const-string', r'ctsProfileMatch|basicIntegrity')))
       if verdict_accesses and qn is not None:
         attestations[qn] = verdict_accesses
 
     for cl in q.consts(InvocationPattern('const-string', self._pat_path)):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       if qn is not None:
-        attempts = self._get_attempts(cl.p[1].v)
+        attempts = self._get_attempts(self._an.get_param(cl, 1).v)
         if attempts:
           confidence[qn] = 'firm'
           if qn not in path_based_detection_attempt:
             path_based_detection_attempt[qn] = attempts
           else:
             path_based_detection_attempt[qn].update(attempts)
     for name, val in context.string_resources():
@@ -758,19 +760,19 @@
   def create(helper: SignatureHelper) -> Signature:
     return SecuritySharedPreferencesDetector(helper)
 
   def get_sigs(self) -> SignatureMap:
     return {self._id:dict(e=self.detect, d='Detects SharedPreferences access')}
 
   async def detect(self) -> None:
-    context = self._helper.get_context().require_type('apk')
+    context = self._get_context()
     store = context.store()
     q = store.query()
     for cl in q.invocations(InvocationPattern('invoke-interface', r'Landroid/content/SharedPreferences;->get(Boolean|Float|Int|String|StringSet)\(Ljava/lang/String;')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         target_val = DataFlow(q).solved_constant_data_in_invocation(cl, 0)
       except DataFlow.NoSuchValueError:
         target_val = '(unknown name)'
 
@@ -778,19 +780,19 @@
         sigid=self._id,
         cfd='certain',
         cvss=self._cvss,
         title=self._summary,
         summary=self._synopsis,
         info0=target_val,
         info1='read',
-        aff0=q.qualname_of(cl)
+        aff0=q.qualname_of(cl.addr)
       ))
 
     for cl in q.invocations(InvocationPattern('invoke-interface', r'Landroid/content/SharedPreferences\$Editor;->put(Boolean|Float|Int|String|StringSet)\(Ljava/lang/String;')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         target_val = DataFlow(q).solved_constant_data_in_invocation(cl, 0)
       except DataFlow.NoSuchValueError:
         target_val = '(unknown name)'
 
@@ -798,19 +800,19 @@
         sigid=self._id,
         cfd='certain',
         cvss=self._cvss,
         title=self._summary,
         summary=self._synopsis,
         info0=target_val,
         info1='write',
-        aff0=q.qualname_of(cl)
+        aff0=q.qualname_of(cl.addr)
       ))
 
     for cl in q.invocations(InvocationPattern('invoke-interface', r'Landroid/content/SharedPreferences/Editor;->remove\(Ljava/lang/String;')):
-      qn = q.qualname_of(cl)
+      qn = q.qualname_of(cl.addr)
       if context.is_qualname_excluded(qn):
         continue
       try:
         target_val = DataFlow(q).solved_constant_data_in_invocation(cl, 0)
       except DataFlow.NoSuchValueError:
         target_val = '(unknown name)'
 
@@ -818,9 +820,9 @@
         sigid=self._id,
         cfd='certain',
         cvss=self._cvss,
         title=self._summary,
         summary=self._synopsis,
         info0=target_val,
         info1='delete',
-        aff0=q.qualname_of(cl)
+        aff0=q.qualname_of(cl.addr)
       ))
```

### Comparing `trueseeing-2.2.2/PKG-INFO` & `trueseeing-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trueseeing
-Version: 2.2.2
+Version: 2.2.4
 Summary: Trueseeing is a non-decompiling Android application vulnerability scanner.
 Keywords: android,security,pentest,hacking
 Author-email: Takahiro Yoshimura <alterakey@protonmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Topic :: Security
 Classifier: Environment :: Console
@@ -12,23 +12,24 @@
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Android
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: lxml~=5.0
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: jinja2~=3.1
-Requires-Dist: attrs~=23.2
 Requires-Dist: pypubsub~=4.0
 Requires-Dist: termcolor~=2.4
 Requires-Dist: progressbar2~=4.3
 Requires-Dist: importlib_metadata~=7.0
 Requires-Dist: asn1crypto~=1.5
 Requires-Dist: zstandard~=0.22
 Requires-Dist: aiohttp~=3.9
 Requires-Dist: lief~=0.14
+Requires-Dist: pyaxmlparser~=0.3
+Requires-Dist: prompt-toolkit~=3.0
 Requires-Dist: mypy~=1.7 ; extra == "dev"
 Requires-Dist: pyproject-flake8~=6.1 ; extra == "dev"
 Requires-Dist: typing_extensions~=4.1 ; extra == "dev"
 Project-URL: Source, https://github.com/alterakey/trueseeing
 Provides-Extra: dev
 
 # README
@@ -79,15 +80,15 @@
 ## Usage
 
 ### Interactive mode
 
 You can interactively scan/analyze/patch/etc. apps -- making it the ideal choice for manual analysis:
 
     $ trueseeing target.apk
-    [+] trueseeing 2.2.2
+    [+] trueseeing 2.2.4
     ts[target.apk]> ?
     ...
     ts[target.apk]> i                      # show generic information
     ...
     ts[target.apk]> pf AndroidManifest.xml # show manifest file
     ...
     ts[target.apk]> a                      # analyze resources too
```


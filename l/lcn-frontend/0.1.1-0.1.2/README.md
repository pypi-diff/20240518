# Comparing `tmp/lcn_frontend-0.1.1.tar.gz` & `tmp/lcn_frontend-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcn_frontend-0.1.1.tar", last modified: Wed Jan 17 18:29:15 2024, max compression
+gzip compressed data, was "lcn_frontend-0.1.2.tar", last modified: Sat Jan 20 15:12:37 2024, max compression
```

## Comparing `lcn_frontend-0.1.1.tar` & `lcn_frontend-0.1.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:29:15.584266 lcn_frontend-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-17 18:26:43.000000 lcn_frontend-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-17 18:26:43.000000 lcn_frontend-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-17 18:29:15.584266 lcn_frontend-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-17 18:26:43.000000 lcn_frontend-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-17 18:26:55.000000 lcn_frontend-0.1.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:29:15.552266 lcn_frontend-0.1.1/lcn_frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/entrypoint-UP5lFvdJ.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/entrypoint-UP5lFvdJ.js.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:29:15.564266 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/
--rw-r--r--   0 runner    (1001) docker     (127)    56267 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/-Bo5aSaU.js
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/-Bo5aSaU.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/52ZGgRTb.js
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/52ZGgRTb.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/52ZGgRTb.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/6vdISARd.js
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/6vdISARd.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/8uDhd8eQ.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/8uDhd8eQ.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/9niMDe6j.js
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/9niMDe6j.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/9niMDe6j.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/DVZuMQTQ.js
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/DVZuMQTQ.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/DVZuMQTQ.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    22502 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NATIZehR.js
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NATIZehR.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/Niahov52.js
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/Niahov52.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/Niahov52.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    46832 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NmyD-jM4.js
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NmyD-jM4.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NmyD-jM4.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    28264 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/PJOjJOeb.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/PJOjJOeb.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/PJOjJOeb.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)   527605 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RIGgWZMd.js
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RIGgWZMd.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   113575 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RIGgWZMd.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    31148 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RaxGx9Oy.js
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RaxGx9Oy.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RaxGx9Oy.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    49288 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RlIVWY_9.js
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RlIVWY_9.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VCTfVQ_Y.js
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VCTfVQ_Y.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    23935 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VYXPimMw.js
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VYXPimMw.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    15164 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ZshdvKRY.js
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ZshdvKRY.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)   261529 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/entrypoint-IIGRb-2R.js
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/entrypoint-IIGRb-2R.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    75729 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/entrypoint-IIGRb-2R.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    19393 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/f67fx1_K.js
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/f67fx1_K.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/gWLSf6Uq.js
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/gWLSf6Uq.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    92082 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/kY1AJzRb.js
--rw-r--r--   0 runner    (1001) docker     (127)    29843 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/kY1AJzRb.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/nqy1LXz0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/nqy1LXz0.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/riIkKI3D.js
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/riIkKI3D.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/riIkKI3D.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    44874 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/xK5ZNMm1.js
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/xK5ZNMm1.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/xK5ZNMm1.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ye57YhXr.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ye57YhXr.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ye57YhXr.js.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:29:15.584266 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/AuN1Wwjr.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/AuN1Wwjr.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/AuN1Wwjr.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    21304 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/CHsIPDL8.js
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/CHsIPDL8.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/CHsIPDL8.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/CHsIPDL8.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   463570 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    97616 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)   253890 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/JAAifVse.js
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/JAAifVse.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/JAAifVse.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/JAAifVse.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    22106 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/PHB24J1t.js
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/PHB24J1t.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/PHB24J1t.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    19329 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/R9L2-V1R.js
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/R9L2-V1R.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/R9L2-V1R.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    29606 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/SaPEbRz1.js
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/SaPEbRz1.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/SaPEbRz1.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/SaPEbRz1.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/X5sZzGl8.js
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/X5sZzGl8.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/X5sZzGl8.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/ZRpJZyXB.js
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/ZRpJZyXB.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/ZRpJZyXB.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bZayZmh0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bZayZmh0.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bZayZmh0.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    61398 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/eOHcBlX_.js
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/eOHcBlX_.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    85359 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/eOHcBlX_.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   118258 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    32677 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    22076 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fP3U9roj.js
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fP3U9roj.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fP3U9roj.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    23283 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fP3U9roj.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    42007 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/hzhoTwCw.js
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/hzhoTwCw.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/hzhoTwCw.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/hzhoTwCw.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/mUrtGIle.js
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/mUrtGIle.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/mUrtGIle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oUOHqENt.js
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oUOHqENt.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oUOHqENt.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    17725 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oUOHqENt.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oyUFw0ts.js
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oyUFw0ts.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oyUFw0ts.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oyUFw0ts.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/sBNRM32J.js
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/sBNRM32J.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/sBNRM32J.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    24301 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/sBNRM32J.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    49739 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yvD5aARM.js
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yvD5aARM.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    64025 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yvD5aARM.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js.gz
--rw-r--r--   0 runner    (1001) docker     (127)    11572 2024-01-17 18:28:46.000000 lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js.map
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 18:28:52.000000 lcn_frontend-0.1.1/lcn_frontend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:29:15.552266 lcn_frontend-0.1.1/lcn_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-17 18:29:15.000000 lcn_frontend-0.1.1/lcn_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-01-17 18:29:15.000000 lcn_frontend-0.1.1/lcn_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 18:29:15.000000 lcn_frontend-0.1.1/lcn_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 18:29:14.000000 lcn_frontend-0.1.1/lcn_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-17 18:29:15.000000 lcn_frontend-0.1.1/lcn_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-17 18:26:43.000000 lcn_frontend-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 18:29:15.584266 lcn_frontend-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:12:37.237416 lcn_frontend-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-20 15:10:25.000000 lcn_frontend-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-20 15:10:25.000000 lcn_frontend-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-20 15:12:37.237416 lcn_frontend-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-01-20 15:10:25.000000 lcn_frontend-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-20 15:10:35.000000 lcn_frontend-0.1.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:12:37.205416 lcn_frontend-0.1.2/lcn_frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-20 15:12:14.000000 lcn_frontend-0.1.2/lcn_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-20 15:12:14.000000 lcn_frontend-0.1.2/lcn_frontend/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-20 15:12:14.000000 lcn_frontend-0.1.2/lcn_frontend/entrypoint-Wn7tXtT_.js
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-20 15:12:14.000000 lcn_frontend-0.1.2/lcn_frontend/entrypoint-Wn7tXtT_.js.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:12:37.217416 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/
+-rw-r--r--   0 runner    (1001) docker     (127)    21536 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/1JtEbuPe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/1JtEbuPe.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/52ZGgRTb.js
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/52ZGgRTb.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/52ZGgRTb.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/6vdISARd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/6vdISARd.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/79rx9Er-.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/79rx9Er-.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/8uDhd8eQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/8uDhd8eQ.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/9niMDe6j.js
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/9niMDe6j.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/9niMDe6j.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/DVZuMQTQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/DVZuMQTQ.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/DVZuMQTQ.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    49776 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/J71QpLgx.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/J71QpLgx.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/Niahov52.js
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/Niahov52.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/Niahov52.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    46832 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/NmyD-jM4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/NmyD-jM4.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/NmyD-jM4.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    28264 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/PJOjJOeb.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/PJOjJOeb.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/PJOjJOeb.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   527605 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RIGgWZMd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RIGgWZMd.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   113575 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RIGgWZMd.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    31148 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RaxGx9Oy.js
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RaxGx9Oy.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RaxGx9Oy.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VCTfVQ_Y.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VCTfVQ_Y.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    23935 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VYXPimMw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VYXPimMw.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    15164 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ZshdvKRY.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ZshdvKRY.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   266938 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/entrypoint-YtbOLj1f.js
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/entrypoint-YtbOLj1f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76983 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/entrypoint-YtbOLj1f.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    19393 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/f67fx1_K.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/f67fx1_K.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/gWLSf6Uq.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/gWLSf6Uq.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    92082 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/kY1AJzRb.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29843 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/kY1AJzRb.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/mNa8_BnN.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/mNa8_BnN.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/m_bQlMKv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/m_bQlMKv.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/m_bQlMKv.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44874 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/xK5ZNMm1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/xK5ZNMm1.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/xK5ZNMm1.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ye57YhXr.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ye57YhXr.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-01-20 15:12:13.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ye57YhXr.js.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:12:37.237416 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9VkUPPxQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9VkUPPxQ.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9VkUPPxQ.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    17762 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9VkUPPxQ.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    50213 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9yFFShGq.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9yFFShGq.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    64523 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9yFFShGq.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/AuN1Wwjr.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/AuN1Wwjr.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/AuN1Wwjr.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    21304 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/CHsIPDL8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/CHsIPDL8.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/CHsIPDL8.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/CHsIPDL8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   463570 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    97616 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   253890 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/JAAifVse.js
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/JAAifVse.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/JAAifVse.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/JAAifVse.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/Ntga-_EF.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/Ntga-_EF.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    10402 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/Ntga-_EF.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    22106 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/PHB24J1t.js
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/PHB24J1t.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/PHB24J1t.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    29606 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/SaPEbRz1.js
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/SaPEbRz1.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/SaPEbRz1.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/SaPEbRz1.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/X5sZzGl8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/X5sZzGl8.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/X5sZzGl8.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ZRpJZyXB.js
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ZRpJZyXB.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ZRpJZyXB.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   122549 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33810 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    22170 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fP3U9roj.js
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fP3U9roj.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fP3U9roj.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    23283 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fP3U9roj.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    42007 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/gwnfZ3wa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/gwnfZ3wa.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/gwnfZ3wa.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/hzhoTwCw.js
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/hzhoTwCw.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/hzhoTwCw.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/hzhoTwCw.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/mUrtGIle.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/mUrtGIle.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/mUrtGIle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    61405 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ovjKXg0y.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ovjKXg0y.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    84988 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ovjKXg0y.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/oyUFw0ts.js
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/oyUFw0ts.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/oyUFw0ts.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/oyUFw0ts.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/sBNRM32J.js
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/sBNRM32J.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/sBNRM32J.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    24301 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/sBNRM32J.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    11572 2024-01-20 15:12:08.000000 lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 15:12:14.000000 lcn_frontend-0.1.2/lcn_frontend/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:12:37.205416 lcn_frontend-0.1.2/lcn_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-20 15:12:37.000000 lcn_frontend-0.1.2/lcn_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-01-20 15:12:37.000000 lcn_frontend-0.1.2/lcn_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 15:12:37.000000 lcn_frontend-0.1.2/lcn_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 15:12:36.000000 lcn_frontend-0.1.2/lcn_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-20 15:12:37.000000 lcn_frontend-0.1.2/lcn_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-20 15:10:25.000000 lcn_frontend-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 15:12:37.237416 lcn_frontend-0.1.2/setup.cfg
```

### Comparing `lcn_frontend-0.1.1/LICENSE` & `lcn_frontend-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/-Bo5aSaU.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/79rx9Er-.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -3,16 +3,16 @@
     [527], {
         9828: function(e, n, t) {
             t.d(n, {
                 i: function() {
                     return b
                 }
             });
-            var a, i, l, r = t(33368),
-                o = t(71650),
+            var a, i, l, o = t(33368),
+                r = t(71650),
                 s = t(82390),
                 u = t(69205),
                 d = t(70906),
                 c = t(51565),
                 h = t(34541),
                 v = t(47838),
                 m = t(88962),
@@ -29,19 +29,19 @@
             (0, c.Z)([(0, k.Mo)("ha-dialog")], (function(e, n) {
                 var t = function(n) {
                     (0, u.Z)(a, n);
                     var t = (0, d.Z)(a);
 
                     function a() {
                         var n;
-                        (0, o.Z)(this, a);
-                        for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                        (0, r.Z)(this, a);
+                        for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                         return n = t.call.apply(t, [this].concat(l)), e((0, s.Z)(n)), n
                     }
-                    return (0, r.Z)(a)
+                    return (0, o.Z)(a)
                 }(n);
                 return {
                     F: t,
                     d: [{
                         kind: "field",
                         key: _.gA,
                         value: void 0
@@ -98,16 +98,16 @@
                     }]
                 }
             }), p.M)
         },
         48950: function(e, n, t) {
             var a, i = t(88962),
                 l = t(33368),
-                r = t(71650),
-                o = t(82390),
+                o = t(71650),
+                r = t(82390),
                 s = t(69205),
                 u = t(70906),
                 d = t(51565),
                 c = (t(97393), t(8485)),
                 h = t(92038),
                 v = t(68144),
                 m = t(73175),
@@ -115,17 +115,17 @@
             (0, d.Z)([(0, m.Mo)("ha-formfield")], (function(e, n) {
                 var t = function(n) {
                     (0, s.Z)(a, n);
                     var t = (0, u.Z)(a);
 
                     function a() {
                         var n;
-                        (0, r.Z)(this, a);
+                        (0, o.Z)(this, a);
                         for (var i = arguments.length, l = new Array(i), s = 0; s < i; s++) l[s] = arguments[s];
-                        return n = t.call.apply(t, [this].concat(l)), e((0, o.Z)(n)), n
+                        return n = t.call.apply(t, [this].concat(l)), e((0, r.Z)(n)), n
                     }
                     return (0, l.Z)(a)
                 }(n);
                 return {
                     F: t,
                     d: [{
                         kind: "method",
@@ -153,33 +153,33 @@
                     }]
                 }
             }), c.a)
         },
         19096: function(e, n, t) {
             var a, i = t(88962),
                 l = t(33368),
-                r = t(71650),
-                o = t(82390),
+                o = t(71650),
+                r = t(82390),
                 s = t(69205),
                 u = t(70906),
                 d = t(51565),
                 c = (t(97393), t(57463)),
                 h = t(44973),
                 v = t(68144),
                 m = t(73175);
             (0, d.Z)([(0, m.Mo)("ha-radio")], (function(e, n) {
                 var t = function(n) {
                     (0, s.Z)(a, n);
                     var t = (0, u.Z)(a);
 
                     function a() {
                         var n;
-                        (0, r.Z)(this, a);
+                        (0, o.Z)(this, a);
                         for (var i = arguments.length, l = new Array(i), s = 0; s < i; s++) l[s] = arguments[s];
-                        return n = t.call.apply(t, [this].concat(l)), e((0, o.Z)(n)), n
+                        return n = t.call.apply(t, [this].concat(l)), e((0, r.Z)(n)), n
                     }
                     return (0, l.Z)(a)
                 }(n);
                 return {
                     F: t,
                     d: [{
                         kind: "field",
@@ -191,16 +191,16 @@
                     }]
                 }
             }), c.J)
         },
         63638: function(e, n, t) {
             var a, i = t(88962),
                 l = t(33368),
-                r = t(71650),
-                o = t(82390),
+                o = t(71650),
+                r = t(82390),
                 s = t(69205),
                 u = t(70906),
                 d = t(51565),
                 c = t(34541),
                 h = t(47838),
                 v = (t(97393), t(53464)),
                 m = t(4301),
@@ -210,17 +210,17 @@
             (0, d.Z)([(0, f.Mo)("ha-switch")], (function(e, n) {
                 var t = function(n) {
                     (0, s.Z)(a, n);
                     var t = (0, u.Z)(a);
 
                     function a() {
                         var n;
-                        (0, r.Z)(this, a);
+                        (0, o.Z)(this, a);
                         for (var i = arguments.length, l = new Array(i), s = 0; s < i; s++) l[s] = arguments[s];
-                        return n = t.call.apply(t, [this].concat(l)), e((0, o.Z)(n)), n
+                        return n = t.call.apply(t, [this].concat(l)), e((0, r.Z)(n)), n
                     }
                     return (0, l.Z)(a)
                 }(n);
                 return {
                     F: t,
                     d: [{
                         kind: "field",
@@ -254,15 +254,15 @@
         },
         86527: function(e, n, t) {
             t.r(n), t.d(n, {
                 CreateEntityDialog: function() {
                     return ue
                 }
             });
-            var a, i, l, r, o, s, u, d, c, h, v, m, p, f, y, k, _, g, b, T, Z, x, C, R, w, A, S, D, z, E, P, U, L, O, V, B, M, N, I, H, Y, F, q = t(88962),
+            var a, i, l, o, r, s, u, d, c, h, v, m, p, f, y, k, _, g, b, T, Z, C, x, R, A, S, D, w, z, E, P, L, O, U, V, B, M, N, I, H, Y, F, q = t(88962),
                 G = t(99312),
                 j = t(81043),
                 K = t(33368),
                 W = t(71650),
                 X = t(82390),
                 J = t(69205),
                 Q = t(70906),
@@ -271,31 +271,31 @@
                 ne = t(68144),
                 te = t(73175),
                 ae = t(9828),
                 ie = function(e) {
                     return e.stopPropagation()
                 },
                 le = t(29950),
-                re = t(34541),
-                oe = t(47838),
+                oe = t(34541),
+                re = t(47838),
                 se = (t(85472), t(46798), t(9849), t(90126), (0, $.Z)([(0, te.Mo)("lcn-config-binary-sensor-element")], (function(e, n) {
-                    var t, o = function(n) {
+                    var t = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
-                        F: o,
+                        F: t,
                         d: [{
                             kind: "field",
                             decorators: [(0, te.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -494,28 +494,18 @@
                                     name: this.lcn.localize("binary-sensor-type-keys-locks"),
                                     value: this._keys,
                                     id: "key-locks"
                                 }]
                             }
                         }, {
                             kind: "method",
-                            key: "firstUpdated",
-                            value: (t = (0, j.Z)((0, G.Z)().mark((function e(n) {
-                                return (0, G.Z)().wrap((function(e) {
-                                    for (;;) switch (e.prev = e.next) {
-                                        case 0:
-                                            (0, re.Z)((0, oe.Z)(o.prototype), "firstUpdated", this).call(this, n), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0];
-                                        case 3:
-                                        case "end":
-                                            return e.stop()
-                                    }
-                                }), e, this)
-                            }))), function(e) {
-                                return t.apply(this, arguments)
-                            })
+                            key: "connectedCallback",
+                            value: function() {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "connectedCallback", this).call(this), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0]
+                            }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
                                 return this._sourceType || this._source ? (0, ne.dy)(a || (a = (0, q.Z)(['\n      <div class="sources">\n        <ha-select\n          id="source-type-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-select\n          id="source-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", "\n        </ha-select>\n      </div>\n    "])), this.lcn.localize("source-type"), this._sourceType.id, this._sourceTypeChanged, ie, this._sourceTypes.map((function(e) {
                                     return (0, ne.dy)(i || (i = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.id, e.name)
                                 })), this.lcn.localize("source"), this._source.value, this._sourceChanged, ie, this._sourceType.value.map((function(e) {
@@ -539,33 +529,33 @@
                                 })), this.domainData.source = this._source.value)
                             }
                         }, {
                             kind: "get",
                             static: !0,
                             key: "styles",
                             value: function() {
-                                return [le.yu, (0, ne.iv)(r || (r = (0, q.Z)(["\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      "])))]
+                                return [le.yu, (0, ne.iv)(o || (o = (0, q.Z)(["\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      "])))]
                             }
                         }]
                     }
                 }), ne.oi), t(76843), t(94570), t(51520), t(63638), (0, $.Z)([(0, te.Mo)("lcn-config-climate-element")], (function(e, n) {
-                    var t, a = function(n) {
+                    var t = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
-                        F: a,
+                        F: t,
                         d: [{
                             kind: "field",
                             decorators: [(0, te.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -721,49 +711,39 @@
                             kind: "get",
                             key: "_setpoints",
                             value: function() {
                                 return this._is2012 ? this._varSetpoints.concat(this._variablesNew) : this._varSetpoints
                             }
                         }, {
                             kind: "method",
-                            key: "firstUpdated",
-                            value: (t = (0, j.Z)((0, G.Z)().mark((function e(n) {
-                                return (0, G.Z)().wrap((function(e) {
-                                    for (;;) switch (e.prev = e.next) {
-                                        case 0:
-                                            (0, re.Z)((0, oe.Z)(a.prototype), "firstUpdated", this).call(this, n), this._source = this._sources[0], this._setpoint = this._setpoints[0], this._unit = this._varUnits[0];
-                                        case 4:
-                                        case "end":
-                                            return e.stop()
-                                    }
-                                }), e, this)
-                            }))), function(e) {
-                                return t.apply(this, arguments)
-                            })
+                            key: "connectedCallback",
+                            value: function() {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "connectedCallback", this).call(this), this._source = this._sources[0], this._setpoint = this._setpoints[0], this._unit = this._varUnits[0]
+                            }
                         }, {
                             kind: "method",
                             key: "willUpdate",
                             value: function(e) {
-                                (0, re.Z)((0, oe.Z)(a.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateMinTemp(this.domainData.min_temp) || !this._validateMaxTemp(this.domainData.max_temp)
+                                (0, oe.Z)((0, re.Z)(t.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateMinTemp(this.domainData.min_temp) || !this._validateMaxTemp(this.domainData.max_temp)
                             }
                         }, {
                             kind: "method",
                             key: "update",
                             value: function(e) {
-                                (0, re.Z)((0, oe.Z)(a.prototype), "update", this).call(this, e), this.dispatchEvent(new CustomEvent("validity-changed", {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "update", this).call(this, e), this.dispatchEvent(new CustomEvent("validity-changed", {
                                     detail: this._invalid,
                                     bubbles: !0,
                                     composed: !0
                                 }))
                             }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return this._source || this._setpoint || this._unit ? (0, ne.dy)(o || (o = (0, q.Z)(['\n      <div class="sources">\n        <ha-select\n          id="source-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-select\n          id="setpoint-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n      </div>\n\n      <div class="lockable">\n        <label>', ":</label>\n        <ha-switch\n          .checked=", "\n          @change=", '\n        ></ha-switch>\n      </div>\n\n      <ha-textfield\n        id="min-textfield"\n        .label=', '\n        type="number"\n        .value=', "\n        required\n        autoValidate\n        @input=", "\n        .validityTransform=", "\n        .validationMessage=", '\n      ></ha-textfield>\n\n      <ha-textfield\n        id="max-textfield"\n        .label=', '\n        type="number"\n        .value=', "\n        required\n        autoValidate\n        @input=", "\n        .validityTransform=", "\n        .validationMessage=", '\n      ></ha-textfield>\n\n      <ha-select\n        id="unit-select"\n        .label=', "\n        .value=", "\n        fixedMenuPosition\n        @selected=", "\n        @closed=", "\n      >\n        ", "\n      </ha-select>\n    "])), this.lcn.localize("source"), this._source.value, this._sourceChanged, ie, this._sources.map((function(e) {
+                                return this._source || this._setpoint || this._unit ? (0, ne.dy)(r || (r = (0, q.Z)(['\n      <div class="sources">\n        <ha-select\n          id="source-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-select\n          id="setpoint-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n      </div>\n\n      <div class="lockable">\n        <label>', ":</label>\n        <ha-switch\n          .checked=", "\n          @change=", '\n        ></ha-switch>\n      </div>\n\n      <ha-textfield\n        id="min-textfield"\n        .label=', '\n        type="number"\n        .value=', "\n        required\n        autoValidate\n        @input=", "\n        .validityTransform=", "\n        .validationMessage=", '\n      ></ha-textfield>\n\n      <ha-textfield\n        id="max-textfield"\n        .label=', '\n        type="number"\n        .value=', "\n        required\n        autoValidate\n        @input=", "\n        .validityTransform=", "\n        .validationMessage=", '\n      ></ha-textfield>\n\n      <ha-select\n        id="unit-select"\n        .label=', "\n        .value=", "\n        fixedMenuPosition\n        @selected=", "\n        @closed=", "\n      >\n        ", "\n      </ha-select>\n    "])), this.lcn.localize("source"), this._source.value, this._sourceChanged, ie, this._sources.map((function(e) {
                                     return (0, ne.dy)(s || (s = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.value, e.name)
                                 })), this.lcn.localize("setpoint"), this._setpoint.value, this._setpointChanged, ie, this._setpoints.map((function(e) {
                                     return (0, ne.dy)(u || (u = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.value, e.name)
                                 })), this.lcn.localize("dashboard-entities-dialog-climate-lockable"), this.domainData.lockable, this._lockableChanged, this.lcn.localize("dashboard-entities-dialog-climate-min-temperature"), this.domainData.min_temp.toString(), this._minTempChanged, this._validityTransformMinTemp, this.lcn.localize("dashboard-entities-dialog-climate-min-temperature-error"), this.lcn.localize("dashboard-entities-dialog-climate-max-temperature"), this.domainData.max_temp.toString(), this._maxTempChanged, this._validityTransformMaxTemp, this.lcn.localize("dashboard-entities-dialog-climate-max-temperature-error"), this.lcn.localize("dashboard-entities-dialog-unit-of-measurement"), this._unit.value, this._unitChanged, ie, this._varUnits.map((function(e) {
                                     return (0, ne.dy)(d || (d = (0, q.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.value, e.name)
                                 }))) : ne.Ld
                             }
@@ -851,28 +831,28 @@
                             key: "styles",
                             value: function() {
                                 return [le.yu, (0, ne.iv)(c || (c = (0, q.Z)(["\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .lockable {\n          margin-top: 10px;\n        }\n        ha-switch {\n          margin-left: 25px;\n        }\n      "])))]
                             }
                         }]
                     }
                 }), ne.oi), t(97221), t(33507), t(82943), (0, $.Z)([(0, te.Mo)("lcn-config-cover-element")], (function(e, n) {
-                    var t, a = function(n) {
+                    var t = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
-                        F: a,
+                        F: t,
                         d: [{
                             kind: "field",
                             decorators: [(0, te.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -940,28 +920,18 @@
                                 }, {
                                     name: "1200ms",
                                     value: "RT1200"
                                 }]
                             }
                         }, {
                             kind: "method",
-                            key: "firstUpdated",
-                            value: (t = (0, j.Z)((0, G.Z)().mark((function e(n) {
-                                return (0, G.Z)().wrap((function(e) {
-                                    for (;;) switch (e.prev = e.next) {
-                                        case 0:
-                                            (0, re.Z)((0, oe.Z)(a.prototype), "firstUpdated", this).call(this, n), this._motor = this._motors[0], this._reverseDelay = this._reverseDelays[0];
-                                        case 3:
-                                        case "end":
-                                            return e.stop()
-                                    }
-                                }), e, this)
-                            }))), function(e) {
-                                return t.apply(this, arguments)
-                            })
+                            key: "connectedCallback",
+                            value: function() {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "connectedCallback", this).call(this), this._motor = this._motors[0], this._reverseDelay = this._reverseDelays[0]
+                            }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
                                 return this._motor || this._reverseDelay ? (0, ne.dy)(h || (h = (0, q.Z)(['\n      <ha-select\n        id="motor-select"\n        .label=', "\n        .value=", "\n        fixedMenuPosition\n        @selected=", "\n        @closed=", "\n      >\n        ", "\n      </ha-select>\n\n      ", "\n    "])), this.lcn.localize("motor"), this._motor.value, this._motorChanged, ie, this._motors.map((function(e) {
                                     return (0, ne.dy)(v || (v = (0, q.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.value, e.name)
                                 })), "OUTPUTS" === this._motor.value ? (0, ne.dy)(m || (m = (0, q.Z)(['\n            <ha-select\n              id="reverse-delay-select"\n              .label=', "\n              .value=", "\n              fixedMenuPosition\n              @selected=", "\n              @closed=", "\n            >\n              ", "\n            </ha-select>\n          "])), this.lcn.localize("reverse-delay"), this._reverseDelay.value, this._reverseDelayChanged, ie, this._reverseDelays.map((function(e) {
@@ -990,28 +960,28 @@
                             key: "styles",
                             value: function() {
                                 return [le.yu, (0, ne.iv)(f || (f = (0, q.Z)(["\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      "])))]
                             }
                         }]
                     }
                 }), ne.oi), t(19096), t(48950), (0, $.Z)([(0, te.Mo)("lcn-config-light-element")], (function(e, n) {
-                    var t, a = function(n) {
+                    var t = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
-                        F: a,
+                        F: t,
                         d: [{
                             kind: "field",
                             decorators: [(0, te.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -1118,39 +1088,29 @@
                                     name: this.lcn.localize("relay"),
                                     value: this._relayPorts,
                                     id: "relay"
                                 }]
                             }
                         }, {
                             kind: "method",
-                            key: "firstUpdated",
-                            value: (t = (0, j.Z)((0, G.Z)().mark((function e(n) {
-                                return (0, G.Z)().wrap((function(e) {
-                                    for (;;) switch (e.prev = e.next) {
-                                        case 0:
-                                            (0, re.Z)((0, oe.Z)(a.prototype), "firstUpdated", this).call(this, n), this._portType = this._portTypes[0], this._port = this._portType.value[0];
-                                        case 3:
-                                        case "end":
-                                            return e.stop()
-                                    }
-                                }), e, this)
-                            }))), function(e) {
-                                return t.apply(this, arguments)
-                            })
+                            key: "connectedCallback",
+                            value: function() {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "connectedCallback", this).call(this), this._portType = this._portTypes[0], this._port = this._portType.value[0]
+                            }
                         }, {
                             kind: "method",
                             key: "willUpdate",
                             value: function(e) {
-                                (0, re.Z)((0, oe.Z)(a.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateTransition(this.domainData.transition)
+                                (0, oe.Z)((0, re.Z)(t.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateTransition(this.domainData.transition)
                             }
                         }, {
                             kind: "method",
                             key: "update",
                             value: function(e) {
-                                (0, re.Z)((0, oe.Z)(a.prototype), "update", this).call(this, e), this.dispatchEvent(new CustomEvent("validity-changed", {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "update", this).call(this, e), this.dispatchEvent(new CustomEvent("validity-changed", {
                                     detail: this._invalid,
                                     bubbles: !0,
                                     composed: !0
                                 }))
                             }
                         }, {
                             kind: "method",
@@ -1219,28 +1179,28 @@
                             key: "styles",
                             value: function() {
                                 return [le.yu, (0, ne.iv)(g || (g = (0, q.Z)(["\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        #dimmable {\n          margin-top: 16px;\n        }\n        #transition {\n          margin-top: 16px;\n        }\n      "])))]
                             }
                         }]
                     }
                 }), ne.oi), t(36513), t(87438), t(22890), t(40271), t(60163), t(74376), (0, $.Z)([(0, te.Mo)("lcn-config-scene-element")], (function(e, n) {
-                    var t, a = function(n) {
+                    var t = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
-                        F: a,
+                        F: t,
                         d: [{
                             kind: "field",
                             decorators: [(0, te.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -1403,39 +1363,29 @@
                                 }, {
                                     name: e + " 8",
                                     value: "RELAY8"
                                 }]
                             }
                         }, {
                             kind: "method",
-                            key: "firstUpdated",
-                            value: (t = (0, j.Z)((0, G.Z)().mark((function e(n) {
-                                return (0, G.Z)().wrap((function(e) {
-                                    for (;;) switch (e.prev = e.next) {
-                                        case 0:
-                                            (0, re.Z)((0, oe.Z)(a.prototype), "firstUpdated", this).call(this, n), this._register = this._registers[0], this._scene = this._scenes[0];
-                                        case 3:
-                                        case "end":
-                                            return e.stop()
-                                    }
-                                }), e, this)
-                            }))), function(e) {
-                                return t.apply(this, arguments)
-                            })
+                            key: "connectedCallback",
+                            value: function() {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "connectedCallback", this).call(this), this._register = this._registers[0], this._scene = this._scenes[0]
+                            }
                         }, {
                             kind: "method",
                             key: "willUpdate",
                             value: function(e) {
-                                (0, re.Z)((0, oe.Z)(a.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateTransition(this.domainData.transition)
+                                (0, oe.Z)((0, re.Z)(t.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateTransition(this.domainData.transition)
                             }
                         }, {
                             kind: "method",
                             key: "update",
                             value: function(e) {
-                                (0, re.Z)((0, oe.Z)(a.prototype), "update", this).call(this, e), this.dispatchEvent(new CustomEvent("validity-changed", {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "update", this).call(this, e), this.dispatchEvent(new CustomEvent("validity-changed", {
                                     detail: this._invalid,
                                     bubbles: !0,
                                     composed: !0
                                 }))
                             }
                         }, {
                             kind: "method",
@@ -1443,17 +1393,17 @@
                             value: function() {
                                 var e = this;
                                 return this._register || this._scene ? (0, ne.dy)(b || (b = (0, q.Z)(['\n      <div class="registers">\n        <ha-select\n          id="register-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-select\n          id="scene-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n      </div>\n\n      <div class="ports">\n        <label>', ":</label><br />\n        ", '\n      </div>\n\n      <div class="ports">\n        <label>', ":</label><br />\n        ", "\n      </div>\n\n      <ha-textfield\n        .label=", '\n        type="number"\n        .value=', '\n        min="0"\n        max="486"\n        required\n        autoValidate\n        @input=', "\n        .validityTransform=", "\n        .disabled=", "\n        .validationMessage=", "\n      ></ha-textfield>\n    "])), this.lcn.localize("register"), this._register.value, this._registerChanged, ie, this._registers.map((function(e) {
                                     return (0, ne.dy)(T || (T = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.value, e.name)
                                 })), this.lcn.localize("scene"), this._scene.value, this._sceneChanged, ie, this._scenes.map((function(e) {
                                     return (0, ne.dy)(Z || (Z = (0, q.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.value, e.name)
                                 })), this.lcn.localize("outputs"), this._outputPorts.map((function(n) {
-                                    return (0, ne.dy)(x || (x = (0, q.Z)(["\n            <ha-formfield label=", ">\n              <ha-checkbox .value=", " @change=", "></ha-checkbox>\n            </ha-formfield>\n          "])), n.name, n.value, e._portCheckedChanged)
-                                })), this.lcn.localize("relays"), this._relayPorts.map((function(n) {
                                     return (0, ne.dy)(C || (C = (0, q.Z)(["\n            <ha-formfield label=", ">\n              <ha-checkbox .value=", " @change=", "></ha-checkbox>\n            </ha-formfield>\n          "])), n.name, n.value, e._portCheckedChanged)
+                                })), this.lcn.localize("relays"), this._relayPorts.map((function(n) {
+                                    return (0, ne.dy)(x || (x = (0, q.Z)(["\n            <ha-formfield label=", ">\n              <ha-checkbox .value=", " @change=", "></ha-checkbox>\n            </ha-formfield>\n          "])), n.name, n.value, e._portCheckedChanged)
                                 })), this.lcn.localize("dashboard-entities-dialog-scene-transition"), this.domainData.transition.toString(), this._transitionChanged, this._validityTransformTransition, this._transitionDisabled, this.lcn.localize("dashboard-entities-dialog-scene-transition-error")) : ne.Ld
                             }
                         }, {
                             kind: "method",
                             key: "_registerChanged",
                             value: function(e) {
                                 var n = e.target; - 1 !== n.index && (this._register = this._registers.find((function(e) {
@@ -1517,28 +1467,28 @@
                             key: "styles",
                             value: function() {
                                 return [le.yu, (0, ne.iv)(R || (R = (0, q.Z)(["\n        .registers {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .ports {\n          margin-top: 10px;\n        }\n      "])))]
                             }
                         }]
                     }
                 }), ne.oi), (0, $.Z)([(0, te.Mo)("lcn-config-sensor-element")], (function(e, n) {
-                    var t, a = function(n) {
+                    var t = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
-                        F: a,
+                        F: t,
                         d: [{
                             kind: "field",
                             decorators: [(0, te.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -1895,38 +1845,28 @@
                                 }, {
                                     name: this.lcn.localize("unit-angle") + " (°)",
                                     value: "DEGREE"
                                 }]
                             }
                         }, {
                             kind: "method",
-                            key: "firstUpdated",
-                            value: (t = (0, j.Z)((0, G.Z)().mark((function e(n) {
-                                return (0, G.Z)().wrap((function(e) {
-                                    for (;;) switch (e.prev = e.next) {
-                                        case 0:
-                                            (0, re.Z)((0, oe.Z)(a.prototype), "firstUpdated", this).call(this, n), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0], this._unit = this._varUnits[0];
-                                        case 4:
-                                        case "end":
-                                            return e.stop()
-                                    }
-                                }), e, this)
-                            }))), function(e) {
-                                return t.apply(this, arguments)
-                            })
+                            key: "connectedCallback",
+                            value: function() {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "connectedCallback", this).call(this), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0], this._unit = this._varUnits[0]
+                            }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return this._sourceType || this._source ? (0, ne.dy)(w || (w = (0, q.Z)(['\n      <div class="sources">\n        <ha-select\n          id="source-type-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-select\n          id="source-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n      </div>\n\n      <ha-select\n        id="unit-select"\n        .label=', "\n        .value=", "\n        fixedMenuPosition\n        @selected=", "\n        @closed=", "\n      >\n        ", "\n      </ha-select>\n    "])), this.lcn.localize("source-type"), this._sourceType.id, this._sourceTypeChanged, ie, this._sourceTypes.map((function(e) {
-                                    return (0, ne.dy)(A || (A = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.id, e.name)
+                                return this._sourceType || this._source ? (0, ne.dy)(A || (A = (0, q.Z)(['\n      <div class="sources">\n        <ha-select\n          id="source-type-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-select\n          id="source-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n      </div>\n\n      <ha-select\n        id="unit-select"\n        .label=', "\n        .value=", "\n        fixedMenuPosition\n        @selected=", "\n        @closed=", "\n      >\n        ", "\n      </ha-select>\n    "])), this.lcn.localize("source-type"), this._sourceType.id, this._sourceTypeChanged, ie, this._sourceTypes.map((function(e) {
+                                    return (0, ne.dy)(S || (S = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.id, e.name)
                                 })), this.lcn.localize("source"), this._source.value, this._sourceChanged, ie, this._sourceType.value.map((function(e) {
-                                    return (0, ne.dy)(S || (S = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.value, e.name)
+                                    return (0, ne.dy)(D || (D = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.value, e.name)
                                 })), this.lcn.localize("dashboard-entities-dialog-unit-of-measurement"), this._unit.value, this._unitChanged, ie, this._varUnits.map((function(e) {
-                                    return (0, ne.dy)(D || (D = (0, q.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.value, e.name)
+                                    return (0, ne.dy)(w || (w = (0, q.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.value, e.name)
                                 }))) : ne.Ld
                             }
                         }, {
                             kind: "method",
                             key: "_sourceTypeChanged",
                             value: function(e) {
                                 var n = e.target; - 1 !== n.index && (this._sourceType = this._sourceTypes.find((function(e) {
@@ -1955,28 +1895,28 @@
                             key: "styles",
                             value: function() {
                                 return [le.yu, (0, ne.iv)(z || (z = (0, q.Z)(["\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      "])))]
                             }
                         }]
                     }
                 }), ne.oi), (0, $.Z)([(0, te.Mo)("lcn-config-switch-element")], (function(e, n) {
-                    var t, a = function(n) {
+                    var t = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
-                        F: a,
+                        F: t,
                         d: [{
                             kind: "field",
                             decorators: [(0, te.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -2075,28 +2015,18 @@
                                     name: this.lcn.localize("relay"),
                                     value: this._relayPorts,
                                     id: "relay"
                                 }]
                             }
                         }, {
                             kind: "method",
-                            key: "firstUpdated",
-                            value: (t = (0, j.Z)((0, G.Z)().mark((function e(n) {
-                                return (0, G.Z)().wrap((function(e) {
-                                    for (;;) switch (e.prev = e.next) {
-                                        case 0:
-                                            (0, re.Z)((0, oe.Z)(a.prototype), "firstUpdated", this).call(this, n), this._portType = this._portTypes[0], this._port = this._portType.value[0];
-                                        case 3:
-                                        case "end":
-                                            return e.stop()
-                                    }
-                                }), e, this)
-                            }))), function(e) {
-                                return t.apply(this, arguments)
-                            })
+                            key: "connectedCallback",
+                            value: function() {
+                                (0, oe.Z)((0, re.Z)(t.prototype), "connectedCallback", this).call(this), this._portType = this._portTypes[0], this._port = this._portType.value[0]
+                            }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
                                 return this._portType || this._port ? (0, ne.dy)(E || (E = (0, q.Z)(['\n      <div id="port-type">', "</div>\n\n      <ha-formfield label=", '>\n        <ha-radio\n          name="port"\n          value="output"\n          .checked=', "\n          @change=", "\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-formfield label=", '>\n        <ha-radio\n          name="port"\n          value="relay"\n          .checked=', "\n          @change=", '\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-select\n        id="port-select"\n        .label=', "\n        .value=", "\n        fixedMenuPosition\n        @selected=", "\n        @closed=", "\n      >\n        ", "\n      </ha-select>\n    "])), this.lcn.localize("port-type"), this.lcn.localize("output"), "output" === this._portType.id, this._portTypeChanged, this.lcn.localize("relay"), "relay" === this._portType.id, this._portTypeChanged, this.lcn.localize("port"), this._port.value, this._portChanged, ie, this._portType.value.map((function(e) {
                                     return (0, ne.dy)(P || (P = (0, q.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.value, e.name)
                                 }))) : ne.Ld
@@ -2119,28 +2049,28 @@
                                 })), this.domainData.output = this._port.value)
                             }
                         }, {
                             kind: "get",
                             static: !0,
                             key: "styles",
                             value: function() {
-                                return [le.yu, (0, ne.iv)(U || (U = (0, q.Z)(["\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      "])))]
+                                return [le.yu, (0, ne.iv)(L || (L = (0, q.Z)(["\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      "])))]
                             }
                         }]
                     }
                 }), ne.oi), t(11285)),
                 ue = (0, $.Z)([(0, te.Mo)("lcn-create-entity-dialog")], (function(e, n) {
                     var t, a, i = function(n) {
                         (0, J.Z)(a, n);
                         var t = (0, Q.Z)(a);
 
                         function a() {
                             var n;
                             (0, W.Z)(this, a);
-                            for (var i = arguments.length, l = new Array(i), r = 0; r < i; r++) l[r] = arguments[r];
+                            for (var i = arguments.length, l = new Array(i), o = 0; o < i; o++) l[o] = arguments[o];
                             return n = t.call.apply(t, [this].concat(l)), e((0, X.Z)(n)), n
                         }
                         return (0, K.Z)(a)
                     }(n);
                     return {
                         F: i,
                         d: [{
@@ -2226,16 +2156,16 @@
                             }))), function(e) {
                                 return a.apply(this, arguments)
                             })
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return this._params ? (0, ne.dy)(L || (L = (0, q.Z)(["\n      <ha-dialog\n        open\n        scrimClickAction\n        escapeKeyAction\n        .heading=", "\n        @closed=", '\n      >\n        <ha-select\n          id="domain-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-textfield\n          id="name-input"\n          label=', '\n          type="string"\n          prefix=', '\n          maxLength="20"\n          @input=', "\n        ></ha-textfield>\n\n        ", '\n\n        <div class="buttons">\n          <mwc-button\n            slot="secondaryAction"\n            @click=', "\n            .label=", '\n          ></mwc-button>\n          <mwc-button\n            slot="primaryAction"\n            .disabled=', "\n            @click=", "\n            .label=", "\n          ></mwc-button>\n        </div>\n      </ha-dialog>\n    "])), (0, ae.i)(this.hass, this.lcn.localize("dashboard-entities-dialog-create-title")), this._closeDialog, this.lcn.localize("domain"), this.domain, this._domainChanged, ie, this._domains.map((function(e) {
-                                    return (0, ne.dy)(O || (O = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.domain, e.name)
+                                return this._params ? (0, ne.dy)(O || (O = (0, q.Z)(["\n      <ha-dialog\n        open\n        scrimClickAction\n        escapeKeyAction\n        .heading=", "\n        @closed=", '\n      >\n        <ha-select\n          id="domain-select"\n          .label=', "\n          .value=", "\n          fixedMenuPosition\n          @selected=", "\n          @closed=", "\n        >\n          ", '\n        </ha-select>\n\n        <ha-textfield\n          id="name-input"\n          label=', '\n          type="string"\n          prefix=', '\n          maxLength="20"\n          @input=', "\n        ></ha-textfield>\n\n        ", '\n\n        <div class="buttons">\n          <mwc-button\n            slot="secondaryAction"\n            @click=', "\n            .label=", '\n          ></mwc-button>\n          <mwc-button\n            slot="primaryAction"\n            .disabled=', "\n            @click=", "\n            .label=", "\n          ></mwc-button>\n        </div>\n      </ha-dialog>\n    "])), (0, ae.i)(this.hass, this.lcn.localize("dashboard-entities-dialog-create-title")), this._closeDialog, this.lcn.localize("domain"), this.domain, this._domainChanged, ie, this._domains.map((function(e) {
+                                    return (0, ne.dy)(U || (U = (0, q.Z)(["\n              <ha-list-item .value=", "> ", " </ha-list-item>\n            "])), e.domain, e.name)
                                 })), this.lcn.localize("entity-id"), this.domain + ".", this._nameChanged, this.renderDomain(this.domain), this._closeDialog, this.lcn.localize("dismiss"), this._invalid, this._create, this.lcn.localize("create")) : ne.Ld
                             }
                         }, {
                             kind: "method",
                             key: "renderDomain",
                             value: function(e) {
                                 if (!this._params) return ne.Ld;
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/52ZGgRTb.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/52ZGgRTb.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/52ZGgRTb.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/52ZGgRTb.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/6vdISARd.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/6vdISARd.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/6vdISARd.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/6vdISARd.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/8uDhd8eQ.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/8uDhd8eQ.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/8uDhd8eQ.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/8uDhd8eQ.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/9niMDe6j.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/9niMDe6j.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/9niMDe6j.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/9niMDe6j.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/DVZuMQTQ.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/DVZuMQTQ.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/DVZuMQTQ.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/DVZuMQTQ.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/DVZuMQTQ.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/DVZuMQTQ.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NATIZehR.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/1JtEbuPe.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
 "use strict";
 (self.webpackChunklcn_frontend = self.webpackChunklcn_frontend || []).push([
-    [540], {
+    [770], {
         82136: function(n, t, e) {
             e.d(t, {
                 i: function() {
-                    return i
+                    return o
                 }
             });
             var a = function(n, t) {
                     var e, a = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2],
-                        i = !(arguments.length > 3 && void 0 !== arguments[3]) || arguments[3],
-                        o = 0,
+                        o = !(arguments.length > 3 && void 0 !== arguments[3]) || arguments[3],
+                        i = 0,
                         r = function() {
-                            for (var r = arguments.length, d = new Array(r), l = 0; l < r; l++) d[l] = arguments[l];
+                            for (var r = arguments.length, l = new Array(r), d = 0; d < r; d++) l[d] = arguments[d];
                             var s = Date.now();
-                            o || !1 !== a || (o = s);
-                            var c = t - (s - o);
-                            c <= 0 || c > t ? (e && (clearTimeout(e), e = void 0), o = s, n.apply(void 0, d)) : e || !1 === i || (e = window.setTimeout((function() {
-                                o = !1 === a ? 0 : Date.now(), e = void 0, n.apply(void 0, d)
+                            i || !1 !== a || (i = s);
+                            var c = t - (s - i);
+                            c <= 0 || c > t ? (e && (clearTimeout(e), e = void 0), i = s, n.apply(void 0, l)) : e || !1 === o || (e = window.setTimeout((function() {
+                                i = !1 === a ? 0 : Date.now(), e = void 0, n.apply(void 0, l)
                             }), c))
                         };
                     return r.cancel = function() {
-                        clearTimeout(e), e = void 0, o = 0
+                        clearTimeout(e), e = void 0, i = 0
                     }, r
                 }((function(n) {
                     history.replaceState({
                         scrollPosition: n
                     }, "")
                 }), 300),
-                i = function(n) {
+                o = function(n) {
                     return function(t) {
                         return {
                             kind: "method",
                             placement: "prototype",
                             key: t.key,
                             descriptor: {
                                 set: function(n) {
@@ -46,71 +46,71 @@
                                 configurable: !0
                             },
                             finisher: function(e) {
                                 var a = e.prototype.connectedCallback;
                                 e.prototype.connectedCallback = function() {
                                     var e = this;
                                     a.call(this);
-                                    var i = this[t.key];
-                                    i && this.updateComplete.then((function() {
+                                    var o = this[t.key];
+                                    o && this.updateComplete.then((function() {
                                         var t = e.renderRoot.querySelector(n);
                                         t && setTimeout((function() {
-                                            t.scrollTop = i
+                                            t.scrollTop = o
                                         }), 0)
                                     }))
                                 }
                             }
                         }
                     }
                 }
         },
         51750: function(n, t, e) {
             function a(n) {
                 var t = n.language || "en";
                 return n.translationMetadata.translations[t] && n.translationMetadata.translations[t].isRTL || !1
             }
 
-            function i(n) {
-                return o(a(n))
+            function o(n) {
+                return i(a(n))
             }
 
-            function o(n) {
+            function i(n) {
                 return n ? "rtl" : "ltr"
             }
             e.d(t, {
                 HE: function() {
                     return a
                 },
                 Zu: function() {
-                    return i
+                    return o
                 }
             })
         },
         68336: function(n, t, e) {
-            var a, i, o, r = e(88962),
-                d = e(33368),
-                l = e(71650),
+            var a, o, i, r = e(88962),
+                l = e(33368),
+                d = e(71650),
                 s = e(82390),
                 c = e(69205),
                 h = e(70906),
                 u = e(51565),
                 p = (e(97393), e(68144)),
                 v = e(73175);
             (0, u.Z)([(0, v.Mo)("ha-card")], (function(n, t) {
                 var e = function(t) {
                     (0, c.Z)(a, t);
                     var e = (0, h.Z)(a);
 
                     function a() {
                         var t;
-                        (0, l.Z)(this, a);
-                        for (var i = arguments.length, o = new Array(i), r = 0; r < i; r++) o[r] = arguments[r];
-                        return t = e.call.apply(e, [this].concat(o)), n((0, s.Z)(t)), t
+                        (0, d.Z)(this, a);
+                        for (var o = arguments.length, i = new Array(o), r = 0; r < o; r++) i[r] = arguments[r];
+                        return t = e.call.apply(e, [this].concat(i)), n((0, s.Z)(t)), t
                     }
-                    return (0, d.Z)(a)
+                    return (0, l.Z)(a)
                 }(t);
                 return {
                     F: e,
                     d: [{
                         kind: "field",
                         decorators: [(0, v.Cb)()],
                         key: "header",
@@ -132,95 +132,95 @@
                         value: function() {
                             return (0, p.iv)(a || (a = (0, r.Z)(["\n      :host {\n        background: var(\n          --ha-card-background,\n          var(--card-background-color, white)\n        );\n        box-shadow: var(--ha-card-box-shadow, none);\n        box-sizing: border-box;\n        border-radius: var(--ha-card-border-radius, 12px);\n        border-width: var(--ha-card-border-width, 1px);\n        border-style: solid;\n        border-color: var(\n          --ha-card-border-color,\n          var(--divider-color, #e0e0e0)\n        );\n        color: var(--primary-text-color);\n        display: block;\n        transition: all 0.3s ease-out;\n        position: relative;\n      }\n\n      :host([raised]) {\n        border: none;\n        box-shadow: var(\n          --ha-card-box-shadow,\n          0px 2px 1px -1px rgba(0, 0, 0, 0.2),\n          0px 1px 1px 0px rgba(0, 0, 0, 0.14),\n          0px 1px 3px 0px rgba(0, 0, 0, 0.12)\n        );\n      }\n\n      .card-header,\n      :host ::slotted(.card-header) {\n        color: var(--ha-card-header-color, --primary-text-color);\n        font-family: var(--ha-card-header-font-family, inherit);\n        font-size: var(--ha-card-header-font-size, 24px);\n        letter-spacing: -0.012em;\n        line-height: 48px;\n        padding: 12px 16px 16px;\n        display: block;\n        margin-block-start: 0px;\n        margin-block-end: 0px;\n        font-weight: normal;\n      }\n\n      :host ::slotted(.card-content:not(:first-child)),\n      slot:not(:first-child)::slotted(.card-content) {\n        padding-top: 0px;\n        margin-top: -8px;\n      }\n\n      :host ::slotted(.card-content) {\n        padding: 16px;\n      }\n\n      :host ::slotted(.card-actions) {\n        border-top: 1px solid var(--divider-color, #e8e8e8);\n        padding: 5px 16px;\n      }\n    "])))
                         }
                     }, {
                         kind: "method",
                         key: "render",
                         value: function() {
-                            return (0, p.dy)(i || (i = (0, r.Z)(["\n      ", "\n      <slot></slot>\n    "])), this.header ? (0, p.dy)(o || (o = (0, r.Z)(['<h1 class="card-header">', "</h1>"])), this.header) : p.Ld)
+                            return (0, p.dy)(o || (o = (0, r.Z)(["\n      ", "\n      <slot></slot>\n    "])), this.header ? (0, p.dy)(i || (i = (0, r.Z)(['<h1 class="card-header">', "</h1>"])), this.header) : p.Ld)
                         }
                     }]
                 }
             }), p.oi)
         },
         99040: function(n, t, e) {
-            var a, i, o, r = e(88962),
-                d = e(33368),
-                l = e(71650),
+            var a, o, i, r = e(88962),
+                l = e(33368),
+                d = e(71650),
                 s = e(82390),
                 c = e(69205),
                 h = e(70906),
                 u = e(51565),
                 p = e(34541),
                 v = e(47838),
                 f = (e(97393), e(48095)),
                 b = e(72477),
                 y = e(73175),
-                m = e(68144),
-                k = e(52138);
+                k = e(68144),
+                g = e(52138);
             (0, u.Z)([(0, y.Mo)("ha-fab")], (function(n, t) {
                 var e = function(t) {
                     (0, c.Z)(a, t);
                     var e = (0, h.Z)(a);
 
                     function a() {
                         var t;
-                        (0, l.Z)(this, a);
-                        for (var i = arguments.length, o = new Array(i), r = 0; r < i; r++) o[r] = arguments[r];
-                        return t = e.call.apply(e, [this].concat(o)), n((0, s.Z)(t)), t
+                        (0, d.Z)(this, a);
+                        for (var o = arguments.length, i = new Array(o), r = 0; r < o; r++) i[r] = arguments[r];
+                        return t = e.call.apply(e, [this].concat(i)), n((0, s.Z)(t)), t
                     }
-                    return (0, d.Z)(a)
+                    return (0, l.Z)(a)
                 }(t);
                 return {
                     F: e,
                     d: [{
                         kind: "method",
                         key: "firstUpdated",
                         value: function(n) {
                             (0, p.Z)((0, v.Z)(e.prototype), "firstUpdated", this).call(this, n), this.style.setProperty("--mdc-theme-secondary", "var(--primary-color)")
                         }
                     }, {
                         kind: "field",
                         static: !0,
                         key: "styles",
                         value: function() {
-                            return [b.W, (0, m.iv)(a || (a = (0, r.Z)(["\n      :host .mdc-fab--extended .mdc-fab__icon {\n        margin-inline-start: -8px;\n        margin-inline-end: 12px;\n        direction: var(--direction);\n      }\n    "]))), "rtl" === k.E.document.dir ? (0, m.iv)(i || (i = (0, r.Z)(["\n          :host .mdc-fab--extended .mdc-fab__icon {\n            direction: rtl;\n          }\n        "]))) : (0, m.iv)(o || (o = (0, r.Z)([""])))]
+                            return [b.W, (0, k.iv)(a || (a = (0, r.Z)(["\n      :host .mdc-fab--extended .mdc-fab__icon {\n        margin-inline-start: -8px;\n        margin-inline-end: 12px;\n        direction: var(--direction);\n      }\n    "]))), "rtl" === g.E.document.dir ? (0, k.iv)(o || (o = (0, r.Z)(["\n          :host .mdc-fab--extended .mdc-fab__icon {\n            direction: rtl;\n          }\n        "]))) : (0, k.iv)(i || (i = (0, r.Z)([""])))]
                         }
                     }]
                 }
             }), f._)
         },
         70657: function(n, t, e) {
-            var a, i, o, r, d, l, s, c, h, u, p, v, f, b = e(88962),
+            var a, o, i, r, l, d, s, c, h, u, p, v, f, b = e(88962),
                 y = e(33368),
-                m = e(71650),
-                k = e(82390),
-                g = e(69205),
+                k = e(71650),
+                g = e(82390),
+                m = e(69205),
                 x = e(70906),
                 w = e(51565),
-                _ = e(34541),
-                Z = e(47838),
+                Z = e(34541),
+                _ = e(47838),
                 C = (e(97393), e(87438), e(46798), e(9849), e(22890), e(22859), e(46349), e(70320), e(85472), e(90126), e(40271), e(60163), e(27763), e(68144)),
                 R = e(73175),
                 z = e(83448),
-                S = e(14516),
-                P = e(82136),
-                W = e(51750),
-                B = (e(33358), e(73957), e(37662), e(98734)),
-                T = e(30153),
-                A = ((0, w.Z)([(0, R.Mo)("ha-tab")], (function(n, t) {
+                P = e(14516),
+                B = e(82136),
+                T = e(51750),
+                A = (e(33358), e(73957), e(37662), e(98734)),
+                F = e(30153),
+                H = ((0, w.Z)([(0, R.Mo)("ha-tab")], (function(n, t) {
                     var e = function(t) {
-                        (0, g.Z)(a, t);
+                        (0, m.Z)(a, t);
                         var e = (0, x.Z)(a);
 
                         function a() {
                             var t;
-                            (0, m.Z)(this, a);
-                            for (var i = arguments.length, o = new Array(i), r = 0; r < i; r++) o[r] = arguments[r];
-                            return t = e.call.apply(e, [this].concat(o)), n((0, k.Z)(t)), t
+                            (0, k.Z)(this, a);
+                            for (var o = arguments.length, i = new Array(o), r = 0; r < o; r++) i[r] = arguments[r];
+                            return t = e.call.apply(e, [this].concat(i)), n((0, g.Z)(t)), t
                         }
                         return (0, y.Z)(a)
                     }(t);
                     return {
                         F: e,
                         d: [{
                             kind: "field",
@@ -259,22 +259,22 @@
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return (0, C.dy)(a || (a = (0, b.Z)(['\n      <div\n        tabindex="0"\n        role="tab"\n        aria-selected=', "\n        aria-label=", "\n        @focus=", "\n        @blur=", "\n        @mousedown=", "\n        @mouseup=", "\n        @mouseenter=", "\n        @mouseleave=", "\n        @touchstart=", "\n        @touchend=", "\n        @touchcancel=", "\n        @keydown=", "\n      >\n        ", '\n        <span class="name">', "</span>\n        ", "\n      </div>\n    "])), this.active, (0, T.o)(this.name), this.handleRippleFocus, this.handleRippleBlur, this.handleRippleActivate, this.handleRippleDeactivate, this.handleRippleMouseEnter, this.handleRippleMouseLeave, this.handleRippleActivate, this.handleRippleDeactivate, this.handleRippleDeactivate, this._handleKeyDown, this.narrow ? (0, C.dy)(i || (i = (0, b.Z)(['<slot name="icon"></slot>']))) : "", this.name, this._shouldRenderRipple ? (0, C.dy)(o || (o = (0, b.Z)(["<mwc-ripple></mwc-ripple>"]))) : "")
+                                return (0, C.dy)(a || (a = (0, b.Z)(['\n      <div\n        tabindex="0"\n        role="tab"\n        aria-selected=', "\n        aria-label=", "\n        @focus=", "\n        @blur=", "\n        @mousedown=", "\n        @mouseup=", "\n        @mouseenter=", "\n        @mouseleave=", "\n        @touchstart=", "\n        @touchend=", "\n        @touchcancel=", "\n        @keydown=", "\n      >\n        ", '\n        <span class="name">', "</span>\n        ", "\n      </div>\n    "])), this.active, (0, F.o)(this.name), this.handleRippleFocus, this.handleRippleBlur, this.handleRippleActivate, this.handleRippleDeactivate, this.handleRippleMouseEnter, this.handleRippleMouseLeave, this.handleRippleActivate, this.handleRippleDeactivate, this.handleRippleDeactivate, this._handleKeyDown, this.narrow ? (0, C.dy)(o || (o = (0, b.Z)(['<slot name="icon"></slot>']))) : "", this.name, this._shouldRenderRipple ? (0, C.dy)(i || (i = (0, b.Z)(["<mwc-ripple></mwc-ripple>"]))) : "")
                             }
                         }, {
                             kind: "field",
                             key: "_rippleHandlers",
                             value: function() {
                                 var n = this;
-                                return new B.A((function() {
+                                return new A.A((function() {
                                     return n._shouldRenderRipple = !0, n._ripple
                                 }))
                             }
                         }, {
                             kind: "method",
                             key: "_handleKeyDown",
                             value: function(n) {
@@ -327,22 +327,22 @@
                                 return (0, C.iv)(r || (r = (0, b.Z)(["\n      div {\n        padding: 0 32px;\n        display: flex;\n        flex-direction: column;\n        text-align: center;\n        box-sizing: border-box;\n        align-items: center;\n        justify-content: center;\n        width: 100%;\n        height: var(--header-height);\n        cursor: pointer;\n        position: relative;\n        outline: none;\n      }\n\n      .name {\n        white-space: nowrap;\n        overflow: hidden;\n        text-overflow: ellipsis;\n        max-width: 100%;\n      }\n\n      :host([active]) {\n        color: var(--primary-color);\n      }\n\n      :host(:not([narrow])[active]) div {\n        border-bottom: 2px solid var(--primary-color);\n      }\n\n      :host([narrow]) {\n        min-width: 0;\n        display: flex;\n        justify-content: center;\n        overflow: hidden;\n      }\n\n      :host([narrow]) div {\n        padding: 0 4px;\n      }\n    "])))
                             }
                         }]
                     }
                 }), C.oi), e(29950));
             (0, w.Z)([(0, R.Mo)("hass-tabs-subpage")], (function(n, t) {
                 var e = function(t) {
-                    (0, g.Z)(a, t);
+                    (0, m.Z)(a, t);
                     var e = (0, x.Z)(a);
 
                     function a() {
                         var t;
-                        (0, m.Z)(this, a);
-                        for (var i = arguments.length, o = new Array(i), r = 0; r < i; r++) o[r] = arguments[r];
-                        return t = e.call.apply(e, [this].concat(o)), n((0, k.Z)(t)), t
+                        (0, k.Z)(this, a);
+                        for (var o = arguments.length, i = new Array(o), r = 0; r < o; r++) i[r] = arguments[r];
+                        return t = e.call.apply(e, [this].concat(i)), n((0, g.Z)(t)), t
                     }
                     return (0, y.Z)(a)
                 }(t);
                 return {
                     F: e,
                     d: [{
                         kind: "field",
@@ -438,50 +438,50 @@
                     }, {
                         kind: "field",
                         decorators: [(0, R.SB)()],
                         key: "_activeTab",
                         value: void 0
                     }, {
                         kind: "field",
-                        decorators: [(0, P.i)(".content")],
+                        decorators: [(0, B.i)(".content")],
                         key: "_savedScrollPos",
                         value: void 0
                     }, {
                         kind: "field",
                         key: "_getTabs",
                         value: function() {
                             var n = this;
-                            return (0, S.Z)((function(t, e, a, i, o, r, s) {
+                            return (0, P.Z)((function(t, e, a, o, i, r, s) {
                                 var c = t.filter((function(t) {
-                                    return (!t.component || t.core || (e = n.hass, i = t.component, e && e.config.components.includes(i))) && (!t.advancedOnly || a);
-                                    var e, i
+                                    return (!t.component || t.core || (e = n.hass, o = t.component, e && e.config.components.includes(o))) && (!t.advancedOnly || a);
+                                    var e, o
                                 }));
                                 if (c.length < 2) {
                                     if (1 === c.length) {
                                         var h = c[0];
                                         return [h.translationKey ? s(h.translationKey) : h.name]
                                     }
                                     return [""]
                                 }
                                 return c.map((function(t) {
-                                    return (0, C.dy)(d || (d = (0, b.Z)(["\n          <a href=", ">\n            <ha-tab\n              .hass=", "\n              .active=", "\n              .narrow=", "\n              .name=", "\n            >\n              ", "\n            </ha-tab>\n          </a>\n        "])), t.path, n.hass, t.path === (null == e ? void 0 : e.path), n.narrow, t.translationKey ? s(t.translationKey) : t.name, t.iconPath ? (0, C.dy)(l || (l = (0, b.Z)(['<ha-svg-icon\n                    slot="icon"\n                    .path=', "\n                  ></ha-svg-icon>"])), t.iconPath) : "")
+                                    return (0, C.dy)(l || (l = (0, b.Z)(["\n          <a href=", ">\n            <ha-tab\n              .hass=", "\n              .active=", "\n              .narrow=", "\n              .name=", "\n            >\n              ", "\n            </ha-tab>\n          </a>\n        "])), t.path, n.hass, t.path === (null == e ? void 0 : e.path), n.narrow, t.translationKey ? s(t.translationKey) : t.name, t.iconPath ? (0, C.dy)(d || (d = (0, b.Z)(['<ha-svg-icon\n                    slot="icon"\n                    .path=', "\n                  ></ha-svg-icon>"])), t.iconPath) : "")
                                 }))
                             }))
                         }
                     }, {
                         kind: "method",
                         key: "willUpdate",
                         value: function(n) {
                             var t = this;
                             if (n.has("route") && (this._activeTab = this.tabs.find((function(n) {
                                     return "".concat(t.route.prefix).concat(t.route.path).includes(n.path)
                                 }))), n.has("hass")) {
                                 var a = n.get("hass");
-                                a && a.language === this.hass.language || (this.rtl = (0, W.HE)(this.hass))
-                            }(0, _.Z)((0, Z.Z)(e.prototype), "willUpdate", this).call(this, n)
+                                a && a.language === this.hass.language || (this.rtl = (0, T.HE)(this.hass))
+                            }(0, Z.Z)((0, _.Z)(e.prototype), "willUpdate", this).call(this, n)
                         }
                     }, {
                         kind: "method",
                         key: "render",
                         value: function() {
                             var n, t, e = this._getTabs(this.tabs, this._activeTab, null === (n = this.hass.userData) || void 0 === n ? void 0 : n.showAdvanced, this.hass.config.components, this.hass.language, this.narrow, this.localizeFunc || this.hass.localize),
                                 a = e.length > 1;
@@ -509,41 +509,41 @@
                             this.backCallback ? this.backCallback() : history.back()
                         }
                     }, {
                         kind: "get",
                         static: !0,
                         key: "styles",
                         value: function() {
-                            return [A.$c, (0, C.iv)(f || (f = (0, b.Z)(['\n        :host {\n          display: block;\n          height: 100%;\n          background-color: var(--primary-background-color);\n        }\n\n        :host([narrow]) {\n          width: 100%;\n          position: fixed;\n        }\n\n        ha-menu-button {\n          margin-right: 24px;\n        }\n\n        .toolbar {\n          display: flex;\n          align-items: center;\n          font-size: 20px;\n          height: var(--header-height);\n          background-color: var(--sidebar-background-color);\n          font-weight: 400;\n          border-bottom: 1px solid var(--divider-color);\n          padding: 8px 12px;\n          box-sizing: border-box;\n        }\n        @media (max-width: 599px) {\n          .toolbar {\n            padding: 4px;\n          }\n        }\n        .toolbar a {\n          color: var(--sidebar-text-color);\n          text-decoration: none;\n        }\n        .bottom-bar a {\n          width: 25%;\n        }\n\n        #tabbar {\n          display: flex;\n          font-size: 14px;\n          overflow: hidden;\n        }\n\n        #tabbar > a {\n          overflow: hidden;\n          max-width: 45%;\n        }\n\n        #tabbar.bottom-bar {\n          position: absolute;\n          bottom: 0;\n          left: 0;\n          padding: 0 16px;\n          box-sizing: border-box;\n          background-color: var(--sidebar-background-color);\n          border-top: 1px solid var(--divider-color);\n          justify-content: space-around;\n          z-index: 2;\n          font-size: 12px;\n          width: 100%;\n          padding-bottom: env(safe-area-inset-bottom);\n        }\n\n        #tabbar:not(.bottom-bar) {\n          flex: 1;\n          justify-content: center;\n        }\n\n        :host(:not([narrow])) #toolbar-icon {\n          min-width: 40px;\n        }\n\n        ha-menu-button,\n        ha-icon-button-arrow-prev,\n        ::slotted([slot="toolbar-icon"]) {\n          display: flex;\n          flex-shrink: 0;\n          pointer-events: auto;\n          color: var(--sidebar-icon-color);\n        }\n\n        .main-title {\n          flex: 1;\n          max-height: var(--header-height);\n          line-height: 20px;\n          color: var(--sidebar-text-color);\n          margin: var(--main-title-margin, 0 0 0 24px);\n        }\n\n        .content {\n          position: relative;\n          width: calc(\n            100% - env(safe-area-inset-left) - env(safe-area-inset-right)\n          );\n          margin-left: env(safe-area-inset-left);\n          margin-right: env(safe-area-inset-right);\n          height: calc(100% - 1px - var(--header-height));\n          height: calc(\n            100% - 1px - var(--header-height) - env(safe-area-inset-bottom)\n          );\n          overflow: auto;\n          -webkit-overflow-scrolling: touch;\n        }\n\n        :host([narrow]) .content.tabs {\n          height: calc(100% - 2 * var(--header-height));\n          height: calc(\n            100% - 2 * var(--header-height) - env(safe-area-inset-bottom)\n          );\n        }\n\n        #fab {\n          position: fixed;\n          right: calc(16px + env(safe-area-inset-right));\n          bottom: calc(16px + env(safe-area-inset-bottom));\n          z-index: 1;\n        }\n        :host([narrow]) #fab.tabs {\n          bottom: calc(84px + env(safe-area-inset-bottom));\n        }\n        #fab[is-wide] {\n          bottom: 24px;\n          right: 24px;\n        }\n        :host([rtl]) #fab {\n          right: auto;\n          left: calc(16px + env(safe-area-inset-left));\n        }\n        :host([rtl][is-wide]) #fab {\n          bottom: 24px;\n          left: 24px;\n          right: auto;\n        }\n      '])))]
+                            return [H.$c, (0, C.iv)(f || (f = (0, b.Z)(['\n        :host {\n          display: block;\n          height: 100%;\n          background-color: var(--primary-background-color);\n        }\n\n        :host([narrow]) {\n          width: 100%;\n          position: fixed;\n        }\n\n        ha-menu-button {\n          margin-right: 24px;\n        }\n\n        .toolbar {\n          display: flex;\n          align-items: center;\n          font-size: 20px;\n          height: var(--header-height);\n          background-color: var(--sidebar-background-color);\n          font-weight: 400;\n          border-bottom: 1px solid var(--divider-color);\n          padding: 8px 12px;\n          box-sizing: border-box;\n        }\n        @media (max-width: 599px) {\n          .toolbar {\n            padding: 4px;\n          }\n        }\n        .toolbar a {\n          color: var(--sidebar-text-color);\n          text-decoration: none;\n        }\n        .bottom-bar a {\n          width: 25%;\n        }\n\n        #tabbar {\n          display: flex;\n          font-size: 14px;\n          overflow: hidden;\n        }\n\n        #tabbar > a {\n          overflow: hidden;\n          max-width: 45%;\n        }\n\n        #tabbar.bottom-bar {\n          position: absolute;\n          bottom: 0;\n          left: 0;\n          padding: 0 16px;\n          box-sizing: border-box;\n          background-color: var(--sidebar-background-color);\n          border-top: 1px solid var(--divider-color);\n          justify-content: space-around;\n          z-index: 2;\n          font-size: 12px;\n          width: 100%;\n          padding-bottom: env(safe-area-inset-bottom);\n        }\n\n        #tabbar:not(.bottom-bar) {\n          flex: 1;\n          justify-content: center;\n        }\n\n        :host(:not([narrow])) #toolbar-icon {\n          min-width: 40px;\n        }\n\n        ha-menu-button,\n        ha-icon-button-arrow-prev,\n        ::slotted([slot="toolbar-icon"]) {\n          display: flex;\n          flex-shrink: 0;\n          pointer-events: auto;\n          color: var(--sidebar-icon-color);\n        }\n\n        .main-title {\n          flex: 1;\n          max-height: var(--header-height);\n          line-height: 20px;\n          color: var(--sidebar-text-color);\n          margin: var(--main-title-margin, 0 0 0 24px);\n        }\n\n        .content {\n          position: relative;\n          width: calc(\n            100% - env(safe-area-inset-left) - env(safe-area-inset-right)\n          );\n          margin-left: env(safe-area-inset-left);\n          margin-right: env(safe-area-inset-right);\n          height: calc(100% - 1px - var(--header-height));\n          height: calc(\n            100% - 1px - var(--header-height) - env(safe-area-inset-bottom)\n          );\n          overflow: auto;\n          -webkit-overflow-scrolling: touch;\n        }\n\n        :host([narrow]) .content.tabs {\n          height: calc(100% - 2 * var(--header-height));\n          height: calc(\n            100% - 2 * var(--header-height) - env(safe-area-inset-bottom)\n          );\n        }\n\n        #fab {\n          position: fixed;\n          right: calc(16px + env(safe-area-inset-right));\n          bottom: calc(16px + env(safe-area-inset-bottom));\n          z-index: 1;\n        }\n        :host([narrow]) #fab.tabs {\n          bottom: calc(84px + env(safe-area-inset-bottom));\n        }\n        #fab[is-wide] {\n          bottom: 24px;\n          right: 24px;\n        }\n        :host([rtl]) #fab {\n          right: auto;\n          left: calc(16px + env(safe-area-inset-left));\n        }\n        :host([rtl][is-wide]) #fab {\n          bottom: 24px;\n          left: 24px;\n          right: auto;\n        }\n      '])))]
                         }
                     }]
                 }
             }), C.oi)
         },
         31952: function(n, t, e) {
-            var a, i, o = e(88962),
+            var a, o, i = e(88962),
                 r = e(33368),
-                d = e(71650),
-                l = e(82390),
+                l = e(71650),
+                d = e(82390),
                 s = e(69205),
                 c = e(70906),
                 h = e(51565),
                 u = (e(97393), e(68144)),
                 p = e(73175),
                 v = e(83448);
             (0, h.Z)([(0, p.Mo)("ha-config-section")], (function(n, t) {
                 var e = function(t) {
                     (0, s.Z)(a, t);
                     var e = (0, c.Z)(a);
 
                     function a() {
                         var t;
-                        (0, d.Z)(this, a);
-                        for (var i = arguments.length, o = new Array(i), r = 0; r < i; r++) o[r] = arguments[r];
-                        return t = e.call.apply(e, [this].concat(o)), n((0, l.Z)(t)), t
+                        (0, l.Z)(this, a);
+                        for (var o = arguments.length, i = new Array(o), r = 0; r < o; r++) i[r] = arguments[r];
+                        return t = e.call.apply(e, [this].concat(i)), n((0, d.Z)(t)), t
                     }
                     return (0, r.Z)(a)
                 }(t);
                 return {
                     F: e,
                     d: [{
                         kind: "field",
@@ -571,116 +571,29 @@
                         value: function() {
                             return !1
                         }
                     }, {
                         kind: "method",
                         key: "render",
                         value: function() {
-                            return (0, u.dy)(a || (a = (0, o.Z)(['\n      <div\n        class="content ', '"\n      >\n        <div class="header"><slot name="header"></slot></div>\n        <div\n          class="together layout ', '"\n        >\n          <div class="intro"><slot name="introduction"></slot></div>\n          <div class="panel flex-auto"><slot></slot></div>\n        </div>\n      </div>\n    '])), (0, v.$)({
+                            return (0, u.dy)(a || (a = (0, i.Z)(['\n      <div\n        class="content ', '"\n      >\n        <div class="header"><slot name="header"></slot></div>\n        <div\n          class="together layout ', '"\n        >\n          <div class="intro"><slot name="introduction"></slot></div>\n          <div class="panel flex-auto"><slot></slot></div>\n        </div>\n      </div>\n    '])), (0, v.$)({
                                 narrow: !this.isWide,
                                 "full-width": this.fullWidth
                             }), (0, v.$)({
                                 narrow: !this.isWide,
                                 vertical: this.vertical || !this.isWide,
                                 horizontal: !this.vertical && this.isWide
                             }))
                         }
                     }, {
                         kind: "get",
                         static: !0,
                         key: "styles",
                         value: function() {
-                            return (0, u.iv)(i || (i = (0, o.Z)(["\n      :host {\n        display: block;\n      }\n      .content {\n        padding: 28px 20px 0;\n        max-width: 1040px;\n        margin: 0 auto;\n      }\n\n      .layout {\n        display: flex;\n      }\n\n      .horizontal {\n        flex-direction: row;\n      }\n\n      .vertical {\n        flex-direction: column;\n      }\n\n      .flex-auto {\n        flex: 1 1 auto;\n      }\n\n      .header {\n        font-family: var(--paper-font-headline_-_font-family);\n        -webkit-font-smoothing: var(\n          --paper-font-headline_-_-webkit-font-smoothing\n        );\n        font-size: var(--paper-font-headline_-_font-size);\n        font-weight: var(--paper-font-headline_-_font-weight);\n        letter-spacing: var(--paper-font-headline_-_letter-spacing);\n        line-height: var(--paper-font-headline_-_line-height);\n        opacity: var(--dark-primary-opacity);\n      }\n\n      .together {\n        margin-top: 32px;\n      }\n\n      .intro {\n        font-family: var(--paper-font-subhead_-_font-family);\n        -webkit-font-smoothing: var(\n          --paper-font-subhead_-_-webkit-font-smoothing\n        );\n        font-weight: var(--paper-font-subhead_-_font-weight);\n        line-height: var(--paper-font-subhead_-_line-height);\n        width: 100%;\n        opacity: var(--dark-primary-opacity);\n        font-size: 14px;\n        padding-bottom: 20px;\n      }\n\n      .horizontal .intro {\n        max-width: 400px;\n        margin-right: 40px;\n      }\n\n      .panel {\n        margin-top: -24px;\n      }\n\n      .panel ::slotted(*) {\n        margin-top: 24px;\n        display: block;\n      }\n\n      .narrow.content {\n        max-width: 640px;\n      }\n      .narrow .together {\n        margin-top: 20px;\n      }\n      .narrow .intro {\n        padding-bottom: 20px;\n        margin-right: 0;\n        max-width: 500px;\n      }\n\n      .full-width {\n        padding: 0;\n      }\n\n      .full-width .layout {\n        flex-direction: column;\n      }\n    "])))
+                            return (0, u.iv)(o || (o = (0, i.Z)(["\n      :host {\n        display: block;\n      }\n      .content {\n        padding: 28px 20px 0;\n        max-width: 1040px;\n        margin: 0 auto;\n      }\n\n      .layout {\n        display: flex;\n      }\n\n      .horizontal {\n        flex-direction: row;\n      }\n\n      .vertical {\n        flex-direction: column;\n      }\n\n      .flex-auto {\n        flex: 1 1 auto;\n      }\n\n      .header {\n        font-family: var(--paper-font-headline_-_font-family);\n        -webkit-font-smoothing: var(\n          --paper-font-headline_-_-webkit-font-smoothing\n        );\n        font-size: var(--paper-font-headline_-_font-size);\n        font-weight: var(--paper-font-headline_-_font-weight);\n        letter-spacing: var(--paper-font-headline_-_letter-spacing);\n        line-height: var(--paper-font-headline_-_line-height);\n        opacity: var(--dark-primary-opacity);\n      }\n\n      .together {\n        margin-top: 32px;\n      }\n\n      .intro {\n        font-family: var(--paper-font-subhead_-_font-family);\n        -webkit-font-smoothing: var(\n          --paper-font-subhead_-_-webkit-font-smoothing\n        );\n        font-weight: var(--paper-font-subhead_-_font-weight);\n        line-height: var(--paper-font-subhead_-_line-height);\n        width: 100%;\n        opacity: var(--dark-primary-opacity);\n        font-size: 14px;\n        padding-bottom: 20px;\n      }\n\n      .horizontal .intro {\n        max-width: 400px;\n        margin-right: 40px;\n      }\n\n      .panel {\n        margin-top: -24px;\n      }\n\n      .panel ::slotted(*) {\n        margin-top: 24px;\n        display: block;\n      }\n\n      .narrow.content {\n        max-width: 640px;\n      }\n      .narrow .together {\n        margin-top: 20px;\n      }\n      .narrow .intro {\n        padding-bottom: 20px;\n        margin-right: 0;\n        max-width: 500px;\n      }\n\n      .full-width {\n        padding: 0;\n      }\n\n      .full-width .layout {\n        flex-direction: column;\n      }\n    "])))
                         }
                     }]
                 }
             }), u.oi)
-        },
-        9051: function(n, t, e) {
-            e.d(t, {
-                Ce: function() {
-                    return d
-                },
-                Ks: function() {
-                    return l
-                },
-                LO: function() {
-                    return i
-                },
-                S6: function() {
-                    return s
-                },
-                V5: function() {
-                    return a
-                },
-                Vy: function() {
-                    return r
-                },
-                n1: function() {
-                    return c
-                },
-                rI: function() {
-                    return o
-                }
-            });
-            e(22859);
-            var a = function(n) {
-                    return n.callWS({
-                        type: "lcn/hosts"
-                    })
-                },
-                i = function(n, t) {
-                    return n.callWS({
-                        type: "lcn/devices",
-                        host_id: t
-                    })
-                },
-                o = function(n, t, e) {
-                    return n.callWS({
-                        type: "lcn/entities",
-                        host_id: t,
-                        address: e
-                    })
-                },
-                r = function(n, t) {
-                    return n.callWS({
-                        type: "lcn/devices/scan",
-                        host_id: t
-                    })
-                },
-                d = function(n, t, e) {
-                    return n.callWS({
-                        type: "lcn/entities/add",
-                        host_id: t,
-                        address: e.address,
-                        name: e.name,
-                        domain: e.domain,
-                        domain_data: e.domain_data
-                    })
-                },
-                l = function(n, t, e) {
-                    return n.callWS({
-                        type: "lcn/entities/delete",
-                        host_id: t,
-                        address: e.address,
-                        domain: e.domain,
-                        resource: e.resource
-                    })
-                },
-                s = function(n, t, e) {
-                    return n.callWS({
-                        type: "lcn/devices/add",
-                        host_id: t,
-                        address: e.address,
-                        name: e.name
-                    })
-                },
-                c = function(n, t, e) {
-                    return n.callWS({
-                        type: "lcn/devices/delete",
-                        host_id: t,
-                        address: e.address
-                    })
-                }
         }
     }
 ]);
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/Niahov52.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/Niahov52.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/Niahov52.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/Niahov52.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NmyD-jM4.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/NmyD-jM4.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NmyD-jM4.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/NmyD-jM4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/NmyD-jM4.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/NmyD-jM4.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/PJOjJOeb.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/PJOjJOeb.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/PJOjJOeb.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/PJOjJOeb.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RIGgWZMd.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RIGgWZMd.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RIGgWZMd.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RIGgWZMd.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RIGgWZMd.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RIGgWZMd.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RaxGx9Oy.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RaxGx9Oy.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RaxGx9Oy.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/RaxGx9Oy.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/RlIVWY_9.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/J71QpLgx.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -25,32 +25,32 @@
                         dialogParams: t
                     }), i
                 }
         },
         73394: function(e, t, n) {
             n.r(t), n.d(t, {
                 LCNConfigDashboard: function() {
-                    return Ae
+                    return Me
                 }
             });
             var a = n(88962),
                 i = n(99312),
                 r = n(81043),
                 l = n(33368),
                 o = n(71650),
                 c = n(82390),
                 d = n(69205),
                 s = n(70906),
                 h = n(51565),
                 u = n(34541),
                 f = n(47838),
                 b = (n(97393), n(46349), n(70320), n(22859), n(85472), n(46798), n(9849), n(90126), n(29950)),
-                _ = (n(87689), n(97221), n(99040), n(90532), n(71133), n(68144)),
-                v = n(73175),
-                m = n(11285),
+                v = (n(87689), n(97221), n(99040), n(90532), n(71133), n(68144)),
+                m = n(73175),
+                _ = n(11285),
                 p = (n(70657), n(31952), n(84776), n(68336), n(37662), n(9051)),
                 g = (n(51358), n(47084), n(5239), n(98490), n(18394)),
                 k = function() {
                     return Promise.all([n.e(597), n.e(812), n.e(244)]).then(n.bind(n, 77044))
                 },
                 y = n(58361),
                 w = (n(85717), n(14516)),
@@ -68,17 +68,17 @@
                 var t = {};
                 return Object.keys(e).forEach((function(n) {
                     t[n] = D(e[n])
                 })), t
             }
             var L, S, E, H = n(83448),
                 T = n(30153),
-                B = n(76538),
-                O = n(82136),
-                A = n(72218),
+                A = n(76538),
+                B = n(82136),
+                O = n(72218),
                 M = n(2537),
                 j = function() {
                     var e = (0, r.Z)((0, i.Z)().mark((function e() {
                         return (0, i.Z)().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
                                     e.prev = 0, new ResizeObserver((function() {})), e.next = 9;
@@ -113,15 +113,15 @@
                             }
                         }), e)
                     })));
                     return function() {
                         return e.apply(this, arguments)
                     }
                 }(),
-                F = (n(74376), n(54371), n(51520), (0, h.Z)([(0, v.Mo)("search-input")], (function(e, t) {
+                I = (n(74376), n(54371), n(51520), (0, h.Z)([(0, m.Mo)("search-input")], (function(e, t) {
                     var n, h, u, f = function(t) {
                         (0, d.Z)(a, t);
                         var n = (0, s.Z)(a);
 
                         function a() {
                             var t;
                             (0, o.Z)(this, a);
@@ -130,66 +130,66 @@
                         }
                         return (0, l.Z)(a)
                     }(t);
                     return {
                         F: f,
                         d: [{
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)()],
+                            decorators: [(0, m.Cb)()],
                             key: "filter",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean
                             })],
                             key: "suffix",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean
                             })],
                             key: "autofocus",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: String
                             })],
                             key: "label",
                             value: void 0
                         }, {
                             kind: "method",
                             key: "focus",
                             value: function() {
                                 var e;
                                 null === (e = this._input) || void 0 === e || e.focus()
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.IO)("ha-textfield", !0)],
+                            decorators: [(0, m.IO)("ha-textfield", !0)],
                             key: "_input",
                             value: void 0
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return (0, _.dy)(L || (L = (0, a.Z)(["\n      <ha-textfield\n        .autofocus=", "\n        .label=", "\n        .value=", "\n        icon\n        .iconTrailing=", "\n        @input=", '\n      >\n        <slot name="prefix" slot="leadingIcon">\n          <ha-svg-icon\n            tabindex="-1"\n            class="prefix"\n            .path=', '\n          ></ha-svg-icon>\n        </slot>\n        <div class="trailing" slot="trailingIcon">\n          ', '\n          <slot name="suffix"></slot>\n        </div>\n      </ha-textfield>\n    '])), this.autofocus, this.label || this.hass.localize("ui.common.search"), this.filter || "", this.filter || this.suffix, this._filterInputChanged, "M9.5,3A6.5,6.5 0 0,1 16,9.5C16,11.11 15.41,12.59 14.44,13.73L14.71,14H15.5L20.5,19L19,20.5L14,15.5V14.71L13.73,14.44C12.59,15.41 11.11,16 9.5,16A6.5,6.5 0 0,1 3,9.5A6.5,6.5 0 0,1 9.5,3M9.5,5C7,5 5,7 5,9.5C5,12 7,14 9.5,14C12,14 14,12 14,9.5C14,7 12,5 9.5,5Z", this.filter && (0, _.dy)(S || (S = (0, a.Z)(["\n            <ha-icon-button\n              @click=", "\n              .label=", "\n              .path=", '\n              class="clear-button"\n            ></ha-icon-button>\n          '])), this._clearSearch, this.hass.localize("ui.common.clear"), "M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z"))
+                                return (0, v.dy)(L || (L = (0, a.Z)(["\n      <ha-textfield\n        .autofocus=", "\n        .label=", "\n        .value=", "\n        icon\n        .iconTrailing=", "\n        @input=", '\n      >\n        <slot name="prefix" slot="leadingIcon">\n          <ha-svg-icon\n            tabindex="-1"\n            class="prefix"\n            .path=', '\n          ></ha-svg-icon>\n        </slot>\n        <div class="trailing" slot="trailingIcon">\n          ', '\n          <slot name="suffix"></slot>\n        </div>\n      </ha-textfield>\n    '])), this.autofocus, this.label || this.hass.localize("ui.common.search"), this.filter || "", this.filter || this.suffix, this._filterInputChanged, "M9.5,3A6.5,6.5 0 0,1 16,9.5C16,11.11 15.41,12.59 14.44,13.73L14.71,14H15.5L20.5,19L19,20.5L14,15.5V14.71L13.73,14.44C12.59,15.41 11.11,16 9.5,16A6.5,6.5 0 0,1 3,9.5A6.5,6.5 0 0,1 9.5,3M9.5,5C7,5 5,7 5,9.5C5,12 7,14 9.5,14C12,14 14,12 14,9.5C14,7 12,5 9.5,5Z", this.filter && (0, v.dy)(S || (S = (0, a.Z)(["\n            <ha-icon-button\n              @click=", "\n              .label=", "\n              .path=", '\n              class="clear-button"\n            ></ha-icon-button>\n          '])), this._clearSearch, this.hass.localize("ui.common.clear"), "M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z"))
                             }
                         }, {
                             kind: "method",
                             key: "_filterChanged",
                             value: (u = (0, r.Z)((0, i.Z)().mark((function e(t) {
                                 return (0, i.Z)().wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
@@ -238,20 +238,20 @@
                                 return n.apply(this, arguments)
                             })
                         }, {
                             kind: "get",
                             static: !0,
                             key: "styles",
                             value: function() {
-                                return (0, _.iv)(E || (E = (0, a.Z)(["\n      :host {\n        display: inline-flex;\n      }\n      ha-svg-icon,\n      ha-icon-button {\n        color: var(--primary-text-color);\n      }\n      ha-svg-icon {\n        outline: none;\n      }\n      .clear-button {\n        --mdc-icon-size: 20px;\n      }\n      ha-textfield {\n        display: inherit;\n      }\n      .trailing {\n        display: flex;\n        align-items: center;\n      }\n    "])))
+                                return (0, v.iv)(E || (E = (0, a.Z)(["\n      :host {\n        display: inline-flex;\n      }\n      ha-svg-icon,\n      ha-icon-button {\n        color: var(--primary-text-color);\n      }\n      ha-svg-icon {\n        outline: none;\n      }\n      .clear-button {\n        --mdc-icon-size: 20px;\n      }\n      ha-textfield {\n        display: inherit;\n      }\n      .trailing {\n        display: flex;\n        align-items: center;\n      }\n    "])))
                             }
                         }]
                     }
-                }), _.oi), n(31528), n(7695), n(44758), n(80354), n(68630), n(59202)),
-                I = n(40039),
+                }), v.oi), n(31528), n(7695), n(44758), n(80354), n(68630), n(59202)),
+                F = n(40039),
                 V = (n(58556), n(94738), n(98214), n(51467), n(96043), n(10999), n(52117), n(63789), n(82479), n(99397), n(89802), n(34997), n(12148), n(17692), n(39685), n(91989), n(86576), n(79894), n(76843), Symbol("Comlink.proxy")),
                 N = Symbol("Comlink.endpoint"),
                 W = Symbol("Comlink.releaseProxy"),
                 U = Symbol("Comlink.finalizer"),
                 q = Symbol("Comlink.thrown"),
                 Y = function(e) {
                     return "object" === (0, R.Z)(e) && null !== e || "function" == typeof e
@@ -300,15 +300,15 @@
 
             function G(e) {
                 var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : globalThis,
                     n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : ["*"];
                 t.addEventListener("message", (function a(i) {
                     if (i && i.data)
                         if (function(e, t) {
-                                var n, a = (0, I.Z)(e);
+                                var n, a = (0, F.Z)(e);
                                 try {
                                     for (a.s(); !(n = a.n()).done;) {
                                         var i = n.value;
                                         if (t === i || "*" === i) return !0;
                                         if (i instanceof RegExp && i.test(t)) return !0
                                     }
                                 } catch (r) {
@@ -342,23 +342,23 @@
                                     case "APPLY":
                                         r = u.apply(h, s);
                                         break;
                                     case "CONSTRUCT":
                                         var f;
                                         r = function(e) {
                                             return Object.assign(e, (0, Z.Z)({}, V, !0))
-                                        }((0, F.Z)(u, (0, z.Z)(s)));
+                                        }((0, I.Z)(u, (0, z.Z)(s)));
                                         break;
                                     case "ENDPOINT":
                                         var b = new MessageChannel,
-                                            _ = b.port1,
-                                            v = b.port2;
-                                        G(e, v), r = function(e, t) {
+                                            v = b.port1,
+                                            m = b.port2;
+                                        G(e, m), r = function(e, t) {
                                             return re.set(e, t), e
-                                        }(_, [_]);
+                                        }(v, [v]);
                                         break;
                                     case "RELEASE":
                                         r = void 0;
                                         break;
                                     default:
                                         return
                                 }
@@ -508,15 +508,15 @@
                 })), (t = n.map((function(e) {
                     return e[1]
                 })), Array.prototype.concat.apply([], t))]
             }
             var ie, re = new WeakMap;
 
             function le(e) {
-                var t, n = (0, I.Z)($);
+                var t, n = (0, F.Z)($);
                 try {
                     for (n.s(); !(t = n.n()).done;) {
                         var a = (0, C.Z)(t.value, 2),
                             i = a[0],
                             r = a[1];
                         if (r.canHandle(e)) {
                             var l = r.serialize(e),
@@ -556,194 +556,194 @@
                     e.addEventListener("message", (function t(n) {
                         n.data && n.data.id && n.data.id === i && (e.removeEventListener("message", t), a(n.data))
                     })), e.start && e.start(), e.postMessage(Object.assign({
                         id: i
                     }, t), n)
                 }))
             }
-            var de, se, he, ue, fe, be, _e, ve, me, pe, ge, ke, ye, we, xe, Ze, Ce, ze, Re, De, Le, Se, Ee, He = function() {
+            var de, se, he, ue, fe, be, ve, me, _e, pe, ge, ke, ye, we, xe, Ze, Ce, ze, Re, De, Le, Se, Ee, He, Te = function() {
                     return ie || (ie = K(new Worker(new URL(n.p + n.u(456), n.b)))), ie
                 },
-                Te = function(e, t, n, a, i) {
-                    return He().sortData(e, t, n, a, i)
+                Ae = function(e, t, n, a, i) {
+                    return Te().sortData(e, t, n, a, i)
                 },
-                Be = ((0, h.Z)([(0, v.Mo)("ha-data-table")], (function(e, t) {
-                    var n, h, m = function(t) {
+                Be = ((0, h.Z)([(0, m.Mo)("ha-data-table")], (function(e, t) {
+                    var n, h, _ = function(t) {
                         (0, d.Z)(a, t);
                         var n = (0, s.Z)(a);
 
                         function a() {
                             var t;
                             (0, o.Z)(this, a);
                             for (var i = arguments.length, r = new Array(i), l = 0; l < i; l++) r[l] = arguments[l];
                             return t = n.call.apply(n, [this].concat(r)), e((0, c.Z)(t)), t
                         }
                         return (0, l.Z)(a)
                     }(t);
                     return {
-                        F: m,
+                        F: _,
                         d: [{
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Object
                             })],
                             key: "columns",
                             value: function() {
                                 return {}
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Array
                             })],
                             key: "data",
                             value: function() {
                                 return []
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean
                             })],
                             key: "selectable",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean
                             })],
                             key: "clickable",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean
                             })],
                             key: "hasFab",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "appendRow",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean,
                                 attribute: "auto-height"
                             })],
                             key: "autoHeight",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: String
                             })],
                             key: "id",
                             value: function() {
                                 return "id"
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: String
                             })],
                             key: "noDataText",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: String
                             })],
                             key: "searchLabel",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean,
                                 attribute: "no-label-float"
                             })],
                             key: "noLabelFloat",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: String
                             })],
                             key: "filter",
                             value: function() {
                                 return ""
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_filterable",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_filter",
                             value: function() {
                                 return ""
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_sortColumn",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_sortDirection",
                             value: function() {
                                 return null
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_filteredData",
                             value: function() {
                                 return []
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_headerHeight",
                             value: function() {
                                 return 0
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.IO)("slot[name='header']")],
+                            decorators: [(0, m.IO)("slot[name='header']")],
                             key: "_header",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_items",
                             value: function() {
                                 return []
                             }
                         }, {
                             kind: "field",
                             key: "_checkableRowsCount",
@@ -764,52 +764,52 @@
                             kind: "field",
                             key: "curRequest",
                             value: function() {
                                 return 0
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, O.i)(".scroller")],
+                            decorators: [(0, B.i)(".scroller")],
                             key: "_savedScrollPos",
                             value: void 0
                         }, {
                             kind: "field",
                             key: "_debounceSearch",
                             value: function() {
                                 var e = this;
-                                return (0, A.D)((function(t) {
+                                return (0, O.D)((function(t) {
                                     e._filter = t
                                 }), 100, !1)
                             }
                         }, {
                             kind: "method",
                             key: "clearSelection",
                             value: function() {
                                 this._checkedRows = [], this._checkedRowsChanged()
                             }
                         }, {
                             kind: "method",
                             key: "connectedCallback",
                             value: function() {
-                                (0, u.Z)((0, f.Z)(m.prototype), "connectedCallback", this).call(this), this._items.length && (this._items = (0, z.Z)(this._items))
+                                (0, u.Z)((0, f.Z)(_.prototype), "connectedCallback", this).call(this), this._items.length && (this._items = (0, z.Z)(this._items))
                             }
                         }, {
                             kind: "method",
                             key: "firstUpdated",
                             value: function() {
                                 var e = this;
                                 this.updateComplete.then((function() {
                                     return e._calcTableHeight()
                                 }))
                             }
                         }, {
                             kind: "method",
                             key: "willUpdate",
                             value: function(e) {
-                                if ((0, u.Z)((0, f.Z)(m.prototype), "willUpdate", this).call(this, e), this.hasUpdated || P(), e.has("columns")) {
+                                if ((0, u.Z)((0, f.Z)(_.prototype), "willUpdate", this).call(this, e), this.hasUpdated || P(), e.has("columns")) {
                                     for (var t in this._filterable = Object.values(this.columns).some((function(e) {
                                             return e.filterable
                                         })), this.columns)
                                         if (this.columns[t].direction) {
                                             this._sortDirection = this.columns[t].direction, this._sortColumn = t;
                                             break
                                         } var n = D(this.columns);
@@ -822,35 +822,35 @@
                                 })).length), (e.has("data") || e.has("columns") || e.has("_filter") || e.has("_sortColumn") || e.has("_sortDirection")) && this._sortFilterData()
                             }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
                                 var e = this;
-                                return (0, _.dy)(de || (de = (0, a.Z)(['\n      <div class="mdc-data-table">\n        <slot name="header" @slotchange=', ">\n          ", '\n        </slot>\n        <div\n          class="mdc-data-table__table ', '"\n          role="table"\n          aria-rowcount=', "\n          style=", '\n        >\n          <div class="mdc-data-table__header-row" role="row" aria-rowindex="1">\n            ', "\n            ", "\n          </div>\n          ", "\n        </div>\n      </div>\n    "])), this._calcTableHeight, this._filterable ? (0, _.dy)(se || (se = (0, a.Z)(['\n                <div class="table-header">\n                  <search-input\n                    .hass=', "\n                    @value-changed=", "\n                    .label=", "\n                    .noLabelFloat=", "\n                  ></search-input>\n                </div>\n              "])), this.hass, this._handleSearchChange, this.searchLabel, this.noLabelFloat) : "", (0, H.$)({
+                                return (0, v.dy)(de || (de = (0, a.Z)(['\n      <div class="mdc-data-table">\n        <slot name="header" @slotchange=', ">\n          ", '\n        </slot>\n        <div\n          class="mdc-data-table__table ', '"\n          role="table"\n          aria-rowcount=', "\n          style=", '\n        >\n          <div class="mdc-data-table__header-row" role="row" aria-rowindex="1">\n            ', "\n            ", "\n          </div>\n          ", "\n        </div>\n      </div>\n    "])), this._calcTableHeight, this._filterable ? (0, v.dy)(se || (se = (0, a.Z)(['\n                <div class="table-header">\n                  <search-input\n                    .hass=', "\n                    @value-changed=", "\n                    .label=", "\n                    .noLabelFloat=", "\n                  ></search-input>\n                </div>\n              "])), this.hass, this._handleSearchChange, this.searchLabel, this.noLabelFloat) : "", (0, H.$)({
                                     "auto-height": this.autoHeight
-                                }), this._filteredData.length + 1, (0, B.V)({
+                                }), this._filteredData.length + 1, (0, A.V)({
                                     height: this.autoHeight ? "".concat(53 * (this._filteredData.length || 1) + 53, "px") : "calc(100% - ".concat(this._headerHeight, "px)")
-                                }), this.selectable ? (0, _.dy)(he || (he = (0, a.Z)(['\n                  <div\n                    class="mdc-data-table__header-cell mdc-data-table__header-cell--checkbox"\n                    role="columnheader"\n                  >\n                    <ha-checkbox\n                      class="mdc-data-table__row-checkbox"\n                      @change=', "\n                      .indeterminate=", "\n                      .checked=", "\n                    >\n                    </ha-checkbox>\n                  </div>\n                "])), this._handleHeaderRowCheckboxClick, this._checkedRows.length && this._checkedRows.length !== this._checkableRowsCount, this._checkedRows.length && this._checkedRows.length === this._checkableRowsCount) : "", Object.entries(this.columns).map((function(t) {
+                                }), this.selectable ? (0, v.dy)(he || (he = (0, a.Z)(['\n                  <div\n                    class="mdc-data-table__header-cell mdc-data-table__header-cell--checkbox"\n                    role="columnheader"\n                  >\n                    <ha-checkbox\n                      class="mdc-data-table__row-checkbox"\n                      @change=', "\n                      .indeterminate=", "\n                      .checked=", "\n                    >\n                    </ha-checkbox>\n                  </div>\n                "])), this._handleHeaderRowCheckboxClick, this._checkedRows.length && this._checkedRows.length !== this._checkableRowsCount, this._checkedRows.length && this._checkedRows.length === this._checkableRowsCount) : "", Object.entries(this.columns).map((function(t) {
                                     var n = (0, C.Z)(t, 2),
                                         i = n[0],
                                         r = n[1];
                                     if (r.hidden) return "";
                                     var l = i === e._sortColumn,
                                         o = {
                                             "mdc-data-table__header-cell--numeric": "numeric" === r.type,
                                             "mdc-data-table__header-cell--icon": "icon" === r.type,
                                             "mdc-data-table__header-cell--icon-button": "icon-button" === r.type,
                                             "mdc-data-table__header-cell--overflow-menu": "overflow-menu" === r.type,
                                             sortable: Boolean(r.sortable),
                                             "not-sorted": Boolean(r.sortable && !l),
                                             grows: Boolean(r.grows)
                                         };
-                                    return (0, _.dy)(ue || (ue = (0, a.Z)(["\n                <div\n                  aria-label=", '\n                  class="mdc-data-table__header-cell ', '"\n                  style=', '\n                  role="columnheader"\n                  aria-sort=', "\n                  @click=", "\n                  .columnId=", "\n                >\n                  ", "\n                  <span>", "</span>\n                </div>\n              "])), r.label, (0, H.$)(o), r.width ? (0, B.V)((0, Z.Z)((0, Z.Z)({}, r.grows ? "minWidth" : "width", r.width), "maxWidth", r.maxWidth || "")) : "", (0, T.o)(l ? "desc" === e._sortDirection ? "descending" : "ascending" : void 0), e._handleHeaderClick, i, r.sortable ? (0, _.dy)(fe || (fe = (0, a.Z)(["\n                        <ha-svg-icon\n                          .path=", "\n                        ></ha-svg-icon>\n                      "])), l && "desc" === e._sortDirection ? "M11,4H13V16L18.5,10.5L19.92,11.92L12,19.84L4.08,11.92L5.5,10.5L11,16V4Z" : "M13,20H11V8L5.5,13.5L4.08,12.08L12,4.16L19.92,12.08L18.5,13.5L13,8V20Z") : "", r.title)
-                                })), this._filteredData.length ? (0, _.dy)(_e || (_e = (0, a.Z)(['\n                <lit-virtualizer\n                  scroller\n                  class="mdc-data-table__content scroller ha-scrollbar"\n                  @scroll=', "\n                  .items=", "\n                  .keyFunction=", "\n                  .renderItem=", "\n                ></lit-virtualizer>\n              "])), this._saveScrollPos, this._items, this._keyFunction, this._renderRow) : (0, _.dy)(be || (be = (0, a.Z)(['\n                <div class="mdc-data-table__content">\n                  <div class="mdc-data-table__row" role="row">\n                    <div class="mdc-data-table__cell grows center" role="cell">\n                      ', "\n                    </div>\n                  </div>\n                </div>\n              "])), this.noDataText || this.hass.localize("ui.components.data-table.no-data")))
+                                    return (0, v.dy)(ue || (ue = (0, a.Z)(["\n                <div\n                  aria-label=", '\n                  class="mdc-data-table__header-cell ', '"\n                  style=', '\n                  role="columnheader"\n                  aria-sort=', "\n                  @click=", "\n                  .columnId=", "\n                >\n                  ", "\n                  <span>", "</span>\n                </div>\n              "])), r.label, (0, H.$)(o), r.width ? (0, A.V)((0, Z.Z)((0, Z.Z)({}, r.grows ? "minWidth" : "width", r.width), "maxWidth", r.maxWidth || "")) : "", (0, T.o)(l ? "desc" === e._sortDirection ? "descending" : "ascending" : void 0), e._handleHeaderClick, i, r.sortable ? (0, v.dy)(fe || (fe = (0, a.Z)(["\n                        <ha-svg-icon\n                          .path=", "\n                        ></ha-svg-icon>\n                      "])), l && "desc" === e._sortDirection ? "M11,4H13V16L18.5,10.5L19.92,11.92L12,19.84L4.08,11.92L5.5,10.5L11,16V4Z" : "M13,20H11V8L5.5,13.5L4.08,12.08L12,4.16L19.92,12.08L18.5,13.5L13,8V20Z") : "", r.title)
+                                })), this._filteredData.length ? (0, v.dy)(ve || (ve = (0, a.Z)(['\n                <lit-virtualizer\n                  scroller\n                  class="mdc-data-table__content scroller ha-scrollbar"\n                  @scroll=', "\n                  .items=", "\n                  .keyFunction=", "\n                  .renderItem=", "\n                ></lit-virtualizer>\n              "])), this._saveScrollPos, this._items, this._keyFunction, this._renderRow) : (0, v.dy)(be || (be = (0, a.Z)(['\n                <div class="mdc-data-table__content">\n                  <div class="mdc-data-table__row" role="row">\n                    <div class="mdc-data-table__cell grows center" role="cell">\n                      ', "\n                    </div>\n                  </div>\n                </div>\n              "])), this.noDataText || this.hass.localize("ui.components.data-table.no-data")))
                             }
                         }, {
                             kind: "field",
                             key: "_keyFunction",
                             value: function() {
                                 var e = this;
                                 return function(t) {
@@ -859,31 +859,31 @@
                             }
                         }, {
                             kind: "field",
                             key: "_renderRow",
                             value: function() {
                                 var e = this;
                                 return function(t, n) {
-                                    return t ? t.append ? (0, _.dy)(ve || (ve = (0, a.Z)(['<div class="mdc-data-table__row">', "</div>"])), t.content) : t.empty ? (0, _.dy)(me || (me = (0, a.Z)(['<div class="mdc-data-table__row"></div>']))) : (0, _.dy)(pe || (pe = (0, a.Z)(["\n      <div\n        aria-rowindex=", '\n        role="row"\n        .rowId=', "\n        @click=", '\n        class="mdc-data-table__row ', '"\n        aria-selected=', "\n        .selectable=", "\n      >\n        ", "\n        ", "\n      </div>\n    "])), n + 2, t[e.id], e._handleRowClick, (0, H.$)({
+                                    return t ? t.append ? (0, v.dy)(me || (me = (0, a.Z)(['<div class="mdc-data-table__row">', "</div>"])), t.content) : t.empty ? (0, v.dy)(_e || (_e = (0, a.Z)(['<div class="mdc-data-table__row"></div>']))) : (0, v.dy)(pe || (pe = (0, a.Z)(["\n      <div\n        aria-rowindex=", '\n        role="row"\n        .rowId=', "\n        @click=", '\n        class="mdc-data-table__row ', '"\n        aria-selected=', "\n        .selectable=", "\n      >\n        ", "\n        ", "\n      </div>\n    "])), n + 2, t[e.id], e._handleRowClick, (0, H.$)({
                                         "mdc-data-table__row--selected": e._checkedRows.includes(String(t[e.id])),
                                         clickable: e.clickable
-                                    }), (0, T.o)(!!e._checkedRows.includes(String(t[e.id])) || void 0), !1 !== t.selectable, e.selectable ? (0, _.dy)(ge || (ge = (0, a.Z)(['\n              <div\n                class="mdc-data-table__cell mdc-data-table__cell--checkbox"\n                role="cell"\n              >\n                <ha-checkbox\n                  class="mdc-data-table__row-checkbox"\n                  @change=', "\n                  .rowId=", "\n                  .disabled=", "\n                  .checked=", "\n                >\n                </ha-checkbox>\n              </div>\n            "])), e._handleRowCheckboxClick, t[e.id], !1 === t.selectable, e._checkedRows.includes(String(t[e.id]))) : "", Object.entries(e.columns).map((function(e) {
+                                    }), (0, T.o)(!!e._checkedRows.includes(String(t[e.id])) || void 0), !1 !== t.selectable, e.selectable ? (0, v.dy)(ge || (ge = (0, a.Z)(['\n              <div\n                class="mdc-data-table__cell mdc-data-table__cell--checkbox"\n                role="cell"\n              >\n                <ha-checkbox\n                  class="mdc-data-table__row-checkbox"\n                  @change=', "\n                  .rowId=", "\n                  .disabled=", "\n                  .checked=", "\n                >\n                </ha-checkbox>\n              </div>\n            "])), e._handleRowCheckboxClick, t[e.id], !1 === t.selectable, e._checkedRows.includes(String(t[e.id]))) : "", Object.entries(e.columns).map((function(e) {
                                         var n = (0, C.Z)(e, 2),
                                             i = n[0],
                                             r = n[1];
-                                        return r.hidden ? "" : (0, _.dy)(ke || (ke = (0, a.Z)(["\n            <div\n              role=", '\n              class="mdc-data-table__cell ', '"\n              style=', "\n            >\n              ", "\n            </div>\n          "])), r.main ? "rowheader" : "cell", (0, H.$)({
+                                        return r.hidden ? "" : (0, v.dy)(ke || (ke = (0, a.Z)(["\n            <div\n              role=", '\n              class="mdc-data-table__cell ', '"\n              style=', "\n            >\n              ", "\n            </div>\n          "])), r.main ? "rowheader" : "cell", (0, H.$)({
                                             "mdc-data-table__cell--flex": "flex" === r.type,
                                             "mdc-data-table__cell--numeric": "numeric" === r.type,
                                             "mdc-data-table__cell--icon": "icon" === r.type,
                                             "mdc-data-table__cell--icon-button": "icon-button" === r.type,
                                             "mdc-data-table__cell--overflow-menu": "overflow-menu" === r.type,
                                             grows: Boolean(r.grows),
                                             forceLTR: Boolean(r.forceLTR)
-                                        }), r.width ? (0, B.V)((0, Z.Z)((0, Z.Z)({}, r.grows ? "minWidth" : "width", r.width), "maxWidth", r.maxWidth ? r.maxWidth : "")) : "", r.template ? r.template(t) : t[i])
-                                    }))) : _.Ld
+                                        }), r.width ? (0, A.V)((0, Z.Z)((0, Z.Z)({}, r.grows ? "minWidth" : "width", r.width), "maxWidth", r.maxWidth ? r.maxWidth : "")) : "", r.template ? r.template(t) : t[i])
+                                    }))) : v.Ld
                                 }
                             }
                         }, {
                             kind: "method",
                             key: "_sortFilterData",
                             value: (h = (0, r.Z)((0, i.Z)().mark((function e() {
                                 var t, n, a, r, l, o, c, d, s, h;
@@ -894,15 +894,15 @@
                                                 e.next = 8;
                                                 break
                                             }
                                             return e.next = 7, this._memFilterData(this.data, this._sortColumns, this._filter);
                                         case 7:
                                             a = e.sent;
                                         case 8:
-                                            return r = this._sortColumn ? Te(a, this._sortColumns[this._sortColumn], this._sortDirection, this._sortColumn, this.hass.locale.language) : a, e.next = 11, Promise.all([r, M.y]);
+                                            return r = this._sortColumn ? Ae(a, this._sortColumns[this._sortColumn], this._sortDirection, this._sortColumn, this.hass.locale.language) : a, e.next = 11, Promise.all([r, M.y]);
                                         case 11:
                                             if (l = e.sent, o = (0, C.Z)(l, 1), c = o[0], d = (new Date).getTime(), !((s = d - t) < 100)) {
                                                 e.next = 19;
                                                 break
                                             }
                                             return e.next = 19, new Promise((function(e) {
                                                 setTimeout(e, 100 - s)
@@ -930,15 +930,15 @@
                             })
                         }, {
                             kind: "field",
                             key: "_memFilterData",
                             value: function() {
                                 return (0, w.Z)((function(e, t, n) {
                                     return function(e, t, n) {
-                                        return He().filterData(e, t, n)
+                                        return Te().filterData(e, t, n)
                                     }(e, t, n)
                                 }))
                             }
                         }, {
                             kind: "method",
                             key: "_handleHeaderClick",
                             value: function(e) {
@@ -1029,33 +1029,33 @@
                                     }
                                 }), e, this)
                             }))), function() {
                                 return n.apply(this, arguments)
                             })
                         }, {
                             kind: "method",
-                            decorators: [(0, v.hO)({
+                            decorators: [(0, m.hO)({
                                 passive: !0
                             })],
                             key: "_saveScrollPos",
                             value: function(e) {
                                 this._savedScrollPos = e.target.scrollTop
                             }
                         }, {
                             kind: "get",
                             static: !0,
                             key: "styles",
                             value: function() {
-                                return [b.$c, (0, _.iv)(ye || (ye = (0, a.Z)(['\n        /* default mdc styles, colors changed, without checkbox styles */\n        :host {\n          height: 100%;\n        }\n        .mdc-data-table__content {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.25rem;\n          font-weight: 400;\n          letter-spacing: 0.0178571429em;\n          text-decoration: inherit;\n          text-transform: inherit;\n        }\n\n        .mdc-data-table {\n          background-color: var(--data-table-background-color);\n          border-radius: 4px;\n          border-width: 1px;\n          border-style: solid;\n          border-color: var(--divider-color);\n          display: inline-flex;\n          flex-direction: column;\n          box-sizing: border-box;\n          overflow: hidden;\n        }\n\n        .mdc-data-table__row--selected {\n          background-color: rgba(var(--rgb-primary-color), 0.04);\n        }\n\n        .mdc-data-table__row {\n          display: flex;\n          width: 100%;\n          height: 52px;\n        }\n\n        .mdc-data-table__row ~ .mdc-data-table__row {\n          border-top: 1px solid var(--divider-color);\n        }\n\n        .mdc-data-table__row.clickable:not(\n            .mdc-data-table__row--selected\n          ):hover {\n          background-color: rgba(var(--rgb-primary-text-color), 0.04);\n        }\n\n        .mdc-data-table__header-cell {\n          color: var(--primary-text-color);\n        }\n\n        .mdc-data-table__cell {\n          color: var(--primary-text-color);\n        }\n\n        .mdc-data-table__header-row {\n          height: 56px;\n          display: flex;\n          width: 100%;\n          border-bottom: 1px solid var(--divider-color);\n          overflow-x: auto;\n        }\n\n        .mdc-data-table__header-row::-webkit-scrollbar {\n          display: none;\n        }\n\n        .mdc-data-table__cell,\n        .mdc-data-table__header-cell {\n          padding-right: 16px;\n          padding-left: 16px;\n          align-self: center;\n          overflow: hidden;\n          text-overflow: ellipsis;\n          flex-shrink: 0;\n          box-sizing: border-box;\n        }\n\n        .mdc-data-table__cell.mdc-data-table__cell--flex {\n          display: flex;\n          overflow: initial;\n        }\n\n        .mdc-data-table__cell.mdc-data-table__cell--icon {\n          overflow: initial;\n        }\n\n        .mdc-data-table__header-cell--checkbox,\n        .mdc-data-table__cell--checkbox {\n          /* @noflip */\n          padding-left: 16px;\n          /* @noflip */\n          padding-right: 0;\n          width: 60px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell--checkbox,\n        :host([dir="rtl"]) .mdc-data-table__cell--checkbox {\n          /* @noflip */\n          padding-left: 0;\n          /* @noflip */\n          padding-right: 16px;\n        }\n\n        .mdc-data-table__table {\n          height: 100%;\n          width: 100%;\n          border: 0;\n          white-space: nowrap;\n        }\n\n        .mdc-data-table__cell {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.25rem;\n          font-weight: 400;\n          letter-spacing: 0.0178571429em;\n          text-decoration: inherit;\n          text-transform: inherit;\n        }\n\n        .mdc-data-table__cell a {\n          color: inherit;\n          text-decoration: none;\n        }\n\n        .mdc-data-table__cell--numeric {\n          text-align: right;\n        }\n        :host([dir="rtl"]) .mdc-data-table__cell--numeric {\n          /* @noflip */\n          text-align: left;\n        }\n\n        .mdc-data-table__cell--icon {\n          color: var(--secondary-text-color);\n          text-align: center;\n        }\n\n        .mdc-data-table__header-cell--icon,\n        .mdc-data-table__cell--icon {\n          width: 54px;\n        }\n\n        .mdc-data-table__cell--icon img {\n          width: 24px;\n          height: 24px;\n        }\n\n        .mdc-data-table__header-cell.mdc-data-table__header-cell--icon {\n          text-align: center;\n        }\n\n        .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:hover,\n        .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:not(\n            .not-sorted\n          ) {\n          text-align: left;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:hover,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:not(\n            .not-sorted\n          ) {\n          text-align: right;\n        }\n\n        .mdc-data-table__cell--icon:first-child ha-icon,\n        .mdc-data-table__cell--icon:first-child img,\n        .mdc-data-table__cell--icon:first-child ha-state-icon,\n        .mdc-data-table__cell--icon:first-child ha-svg-icon {\n          margin-left: 8px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__cell--icon:first-child ha-icon,\n        :host([dir="rtl"])\n          .mdc-data-table__cell--icon:first-child\n          ha-state-icon,\n        :host([dir="rtl"])\n          .mdc-data-table__cell--icon:first-child\n          ha-svg-icon\n          :host([dir="rtl"])\n          .mdc-data-table__cell--icon:first-child\n          img {\n          margin-left: auto;\n          margin-right: 8px;\n        }\n\n        .mdc-data-table__cell--icon:first-child state-badge {\n          margin-right: -8px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__cell--icon:first-child state-badge {\n          margin-right: auto;\n          margin-left: -8px;\n        }\n\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__header-cell--overflow-menu,\n        .mdc-data-table__header-cell--icon-button,\n        .mdc-data-table__cell--icon-button {\n          padding: 8px;\n        }\n\n        .mdc-data-table__header-cell--icon-button,\n        .mdc-data-table__cell--icon-button {\n          width: 56px;\n        }\n\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__cell--icon-button {\n          color: var(--secondary-text-color);\n          text-overflow: clip;\n        }\n\n        .mdc-data-table__header-cell--icon-button:first-child,\n        .mdc-data-table__cell--icon-button:first-child,\n        .mdc-data-table__header-cell--icon-button:last-child,\n        .mdc-data-table__cell--icon-button:last-child {\n          width: 64px;\n        }\n\n        .mdc-data-table__cell--overflow-menu:first-child,\n        .mdc-data-table__header-cell--overflow-menu:first-child,\n        .mdc-data-table__header-cell--icon-button:first-child,\n        .mdc-data-table__cell--icon-button:first-child {\n          padding-left: 16px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--overflow-menu:first-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--overflow-menu:first-child,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--overflow-menu:first-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--overflow-menu:first-child {\n          padding-left: 8px;\n          padding-right: 16px;\n        }\n\n        .mdc-data-table__cell--overflow-menu:last-child,\n        .mdc-data-table__header-cell--overflow-menu:last-child,\n        .mdc-data-table__header-cell--icon-button:last-child,\n        .mdc-data-table__cell--icon-button:last-child {\n          padding-right: 16px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--overflow-menu:last-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--overflow-menu:last-child,\n        :host([dir="rtl"]) .mdc-data-table__header-cell--icon-button:last-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--icon-button:last-child {\n          padding-right: 8px;\n          padding-left: 16px;\n        }\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__header-cell--overflow-menu {\n          overflow: initial;\n        }\n        .mdc-data-table__cell--icon-button a {\n          color: var(--secondary-text-color);\n        }\n\n        .mdc-data-table__header-cell {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.375rem;\n          font-weight: 500;\n          letter-spacing: 0.0071428571em;\n          text-decoration: inherit;\n          text-transform: inherit;\n          text-align: left;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell {\n          /* @noflip */\n          text-align: right;\n        }\n\n        .mdc-data-table__header-cell--numeric {\n          text-align: right;\n        }\n        .mdc-data-table__header-cell--numeric.sortable:hover,\n        .mdc-data-table__header-cell--numeric.sortable:not(.not-sorted) {\n          text-align: left;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell--numeric {\n          /* @noflip */\n          text-align: left;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell--numeric.sortable:hover,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--numeric.sortable:not(.not-sorted) {\n          text-align: right;\n        }\n\n        /* custom from here */\n\n        :host {\n          display: block;\n        }\n\n        .mdc-data-table {\n          display: block;\n          border-width: var(--data-table-border-width, 1px);\n          height: 100%;\n        }\n        .mdc-data-table__header-cell {\n          overflow: hidden;\n          position: relative;\n        }\n        .mdc-data-table__header-cell span {\n          position: relative;\n          left: 0px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell span {\n          left: auto;\n          right: 0px;\n        }\n\n        .mdc-data-table__header-cell.sortable {\n          cursor: pointer;\n        }\n        .mdc-data-table__header-cell > * {\n          transition: left 0.2s ease;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell > * {\n          transition: right 0.2s ease;\n        }\n        .mdc-data-table__header-cell ha-svg-icon {\n          top: -3px;\n          position: absolute;\n        }\n        .mdc-data-table__header-cell.not-sorted ha-svg-icon {\n          left: -20px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell.not-sorted ha-svg-icon {\n          right: -20px;\n        }\n        .mdc-data-table__header-cell.sortable:not(.not-sorted) span,\n        .mdc-data-table__header-cell.sortable.not-sorted:hover span {\n          left: 24px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable:not(.not-sorted)\n          span,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable.not-sorted:hover\n          span {\n          left: auto;\n          right: 24px;\n        }\n        .mdc-data-table__header-cell.sortable:not(.not-sorted) ha-svg-icon,\n        .mdc-data-table__header-cell.sortable:hover.not-sorted ha-svg-icon {\n          left: 12px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable:not(.not-sorted)\n          ha-svg-icon,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable:hover.not-sorted\n          ha-svg-icon {\n          left: auto;\n          right: 12px;\n        }\n        .table-header {\n          border-bottom: 1px solid var(--divider-color);\n        }\n        search-input {\n          display: block;\n          flex: 1;\n        }\n        slot[name="header"] {\n          display: block;\n        }\n        .center {\n          text-align: center;\n        }\n        .secondary {\n          color: var(--secondary-text-color);\n        }\n        .scroller {\n          height: calc(100% - 57px);\n          overflow: overlay !important;\n        }\n\n        .mdc-data-table__table.auto-height .scroller {\n          overflow-y: hidden !important;\n        }\n        .grows {\n          flex-grow: 1;\n          flex-shrink: 1;\n        }\n        .forceLTR {\n          direction: ltr;\n        }\n        .clickable {\n          cursor: pointer;\n        }\n        lit-virtualizer {\n          contain: size layout !important;\n          overscroll-behavior: contain;\n        }\n      '])))]
+                                return [b.$c, (0, v.iv)(ye || (ye = (0, a.Z)(['\n        /* default mdc styles, colors changed, without checkbox styles */\n        :host {\n          height: 100%;\n        }\n        .mdc-data-table__content {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.25rem;\n          font-weight: 400;\n          letter-spacing: 0.0178571429em;\n          text-decoration: inherit;\n          text-transform: inherit;\n        }\n\n        .mdc-data-table {\n          background-color: var(--data-table-background-color);\n          border-radius: 4px;\n          border-width: 1px;\n          border-style: solid;\n          border-color: var(--divider-color);\n          display: inline-flex;\n          flex-direction: column;\n          box-sizing: border-box;\n          overflow: hidden;\n        }\n\n        .mdc-data-table__row--selected {\n          background-color: rgba(var(--rgb-primary-color), 0.04);\n        }\n\n        .mdc-data-table__row {\n          display: flex;\n          width: 100%;\n          height: 52px;\n        }\n\n        .mdc-data-table__row ~ .mdc-data-table__row {\n          border-top: 1px solid var(--divider-color);\n        }\n\n        .mdc-data-table__row.clickable:not(\n            .mdc-data-table__row--selected\n          ):hover {\n          background-color: rgba(var(--rgb-primary-text-color), 0.04);\n        }\n\n        .mdc-data-table__header-cell {\n          color: var(--primary-text-color);\n        }\n\n        .mdc-data-table__cell {\n          color: var(--primary-text-color);\n        }\n\n        .mdc-data-table__header-row {\n          height: 56px;\n          display: flex;\n          width: 100%;\n          border-bottom: 1px solid var(--divider-color);\n          overflow-x: auto;\n        }\n\n        .mdc-data-table__header-row::-webkit-scrollbar {\n          display: none;\n        }\n\n        .mdc-data-table__cell,\n        .mdc-data-table__header-cell {\n          padding-right: 16px;\n          padding-left: 16px;\n          align-self: center;\n          overflow: hidden;\n          text-overflow: ellipsis;\n          flex-shrink: 0;\n          box-sizing: border-box;\n        }\n\n        .mdc-data-table__cell.mdc-data-table__cell--flex {\n          display: flex;\n          overflow: initial;\n        }\n\n        .mdc-data-table__cell.mdc-data-table__cell--icon {\n          overflow: initial;\n        }\n\n        .mdc-data-table__header-cell--checkbox,\n        .mdc-data-table__cell--checkbox {\n          /* @noflip */\n          padding-left: 16px;\n          /* @noflip */\n          padding-right: 0;\n          width: 60px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell--checkbox,\n        :host([dir="rtl"]) .mdc-data-table__cell--checkbox {\n          /* @noflip */\n          padding-left: 0;\n          /* @noflip */\n          padding-right: 16px;\n        }\n\n        .mdc-data-table__table {\n          height: 100%;\n          width: 100%;\n          border: 0;\n          white-space: nowrap;\n        }\n\n        .mdc-data-table__cell {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.25rem;\n          font-weight: 400;\n          letter-spacing: 0.0178571429em;\n          text-decoration: inherit;\n          text-transform: inherit;\n        }\n\n        .mdc-data-table__cell a {\n          color: inherit;\n          text-decoration: none;\n        }\n\n        .mdc-data-table__cell--numeric {\n          text-align: right;\n        }\n        :host([dir="rtl"]) .mdc-data-table__cell--numeric {\n          /* @noflip */\n          text-align: left;\n        }\n\n        .mdc-data-table__cell--icon {\n          color: var(--secondary-text-color);\n          text-align: center;\n        }\n\n        .mdc-data-table__header-cell--icon,\n        .mdc-data-table__cell--icon {\n          width: 54px;\n        }\n\n        .mdc-data-table__cell--icon img {\n          width: 24px;\n          height: 24px;\n        }\n\n        .mdc-data-table__header-cell.mdc-data-table__header-cell--icon {\n          text-align: center;\n        }\n\n        .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:hover,\n        .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:not(\n            .not-sorted\n          ) {\n          text-align: left;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:hover,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:not(\n            .not-sorted\n          ) {\n          text-align: right;\n        }\n\n        .mdc-data-table__cell--icon:first-child ha-icon,\n        .mdc-data-table__cell--icon:first-child img,\n        .mdc-data-table__cell--icon:first-child ha-state-icon,\n        .mdc-data-table__cell--icon:first-child ha-svg-icon {\n          margin-left: 8px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__cell--icon:first-child ha-icon,\n        :host([dir="rtl"])\n          .mdc-data-table__cell--icon:first-child\n          ha-state-icon,\n        :host([dir="rtl"])\n          .mdc-data-table__cell--icon:first-child\n          ha-svg-icon\n          :host([dir="rtl"])\n          .mdc-data-table__cell--icon:first-child\n          img {\n          margin-left: auto;\n          margin-right: 8px;\n        }\n\n        .mdc-data-table__cell--icon:first-child state-badge {\n          margin-right: -8px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__cell--icon:first-child state-badge {\n          margin-right: auto;\n          margin-left: -8px;\n        }\n\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__header-cell--overflow-menu,\n        .mdc-data-table__header-cell--icon-button,\n        .mdc-data-table__cell--icon-button {\n          padding: 8px;\n        }\n\n        .mdc-data-table__header-cell--icon-button,\n        .mdc-data-table__cell--icon-button {\n          width: 56px;\n        }\n\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__cell--icon-button {\n          color: var(--secondary-text-color);\n          text-overflow: clip;\n        }\n\n        .mdc-data-table__header-cell--icon-button:first-child,\n        .mdc-data-table__cell--icon-button:first-child,\n        .mdc-data-table__header-cell--icon-button:last-child,\n        .mdc-data-table__cell--icon-button:last-child {\n          width: 64px;\n        }\n\n        .mdc-data-table__cell--overflow-menu:first-child,\n        .mdc-data-table__header-cell--overflow-menu:first-child,\n        .mdc-data-table__header-cell--icon-button:first-child,\n        .mdc-data-table__cell--icon-button:first-child {\n          padding-left: 16px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--overflow-menu:first-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--overflow-menu:first-child,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--overflow-menu:first-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--overflow-menu:first-child {\n          padding-left: 8px;\n          padding-right: 16px;\n        }\n\n        .mdc-data-table__cell--overflow-menu:last-child,\n        .mdc-data-table__header-cell--overflow-menu:last-child,\n        .mdc-data-table__header-cell--icon-button:last-child,\n        .mdc-data-table__cell--icon-button:last-child {\n          padding-right: 16px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--overflow-menu:last-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--overflow-menu:last-child,\n        :host([dir="rtl"]) .mdc-data-table__header-cell--icon-button:last-child,\n        :host([dir="rtl"]) .mdc-data-table__cell--icon-button:last-child {\n          padding-right: 8px;\n          padding-left: 16px;\n        }\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__header-cell--overflow-menu {\n          overflow: initial;\n        }\n        .mdc-data-table__cell--icon-button a {\n          color: var(--secondary-text-color);\n        }\n\n        .mdc-data-table__header-cell {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.375rem;\n          font-weight: 500;\n          letter-spacing: 0.0071428571em;\n          text-decoration: inherit;\n          text-transform: inherit;\n          text-align: left;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell {\n          /* @noflip */\n          text-align: right;\n        }\n\n        .mdc-data-table__header-cell--numeric {\n          text-align: right;\n        }\n        .mdc-data-table__header-cell--numeric.sortable:hover,\n        .mdc-data-table__header-cell--numeric.sortable:not(.not-sorted) {\n          text-align: left;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell--numeric {\n          /* @noflip */\n          text-align: left;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell--numeric.sortable:hover,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell--numeric.sortable:not(.not-sorted) {\n          text-align: right;\n        }\n\n        /* custom from here */\n\n        :host {\n          display: block;\n        }\n\n        .mdc-data-table {\n          display: block;\n          border-width: var(--data-table-border-width, 1px);\n          height: 100%;\n        }\n        .mdc-data-table__header-cell {\n          overflow: hidden;\n          position: relative;\n        }\n        .mdc-data-table__header-cell span {\n          position: relative;\n          left: 0px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell span {\n          left: auto;\n          right: 0px;\n        }\n\n        .mdc-data-table__header-cell.sortable {\n          cursor: pointer;\n        }\n        .mdc-data-table__header-cell > * {\n          transition: left 0.2s ease;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell > * {\n          transition: right 0.2s ease;\n        }\n        .mdc-data-table__header-cell ha-svg-icon {\n          top: -3px;\n          position: absolute;\n        }\n        .mdc-data-table__header-cell.not-sorted ha-svg-icon {\n          left: -20px;\n        }\n        :host([dir="rtl"]) .mdc-data-table__header-cell.not-sorted ha-svg-icon {\n          right: -20px;\n        }\n        .mdc-data-table__header-cell.sortable:not(.not-sorted) span,\n        .mdc-data-table__header-cell.sortable.not-sorted:hover span {\n          left: 24px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable:not(.not-sorted)\n          span,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable.not-sorted:hover\n          span {\n          left: auto;\n          right: 24px;\n        }\n        .mdc-data-table__header-cell.sortable:not(.not-sorted) ha-svg-icon,\n        .mdc-data-table__header-cell.sortable:hover.not-sorted ha-svg-icon {\n          left: 12px;\n        }\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable:not(.not-sorted)\n          ha-svg-icon,\n        :host([dir="rtl"])\n          .mdc-data-table__header-cell.sortable:hover.not-sorted\n          ha-svg-icon {\n          left: auto;\n          right: 12px;\n        }\n        .table-header {\n          border-bottom: 1px solid var(--divider-color);\n        }\n        search-input {\n          display: block;\n          flex: 1;\n        }\n        slot[name="header"] {\n          display: block;\n        }\n        .center {\n          text-align: center;\n        }\n        .secondary {\n          color: var(--secondary-text-color);\n        }\n        .scroller {\n          height: calc(100% - 57px);\n          overflow: overlay !important;\n        }\n\n        .mdc-data-table__table.auto-height .scroller {\n          overflow-y: hidden !important;\n        }\n        .grows {\n          flex-grow: 1;\n          flex-shrink: 1;\n        }\n        .forceLTR {\n          direction: ltr;\n        }\n        .clickable {\n          cursor: pointer;\n        }\n        lit-virtualizer {\n          contain: size layout !important;\n          overscroll-behavior: contain;\n        }\n      '])))]
                             }
                         }]
                     }
-                }), _.oi), n(38480)),
+                }), v.oi), n(38480)),
                 Oe = "M19,4H15.5L14.5,3H9.5L8.5,4H5V6H19M6,19A2,2 0 0,0 8,21H16A2,2 0 0,0 18,19V7H6V19Z",
-                Ae = ((0, h.Z)([(0, v.Mo)("lcn-devices-data-table")], (function(e, t) {
+                Me = ((0, h.Z)([(0, m.Mo)("lcn-devices-data-table")], (function(e, t) {
                     var n, h = function(t) {
                         (0, d.Z)(a, t);
                         var n = (0, s.Z)(a);
 
                         function a() {
                             var t;
                             (0, o.Z)(this, a);
@@ -1064,43 +1064,43 @@
                         }
                         return (0, l.Z)(a)
                     }(t);
                     return {
                         F: h,
                         d: [{
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "lcn",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "narrow",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "route",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "devices",
                             value: function() {
                                 return []
                             }
                         }, {
@@ -1133,15 +1133,15 @@
                                             grows: !0
                                         },
                                         delete: {
                                             title: "",
                                             sortable: !1,
                                             width: "80px",
                                             template: function(t) {
-                                                return (0, _.dy)(we || (we = (0, a.Z)(["\n                  <ha-icon-button\n                    .label=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), e.lcn.localize("dashboard-devices-table-delete"), Oe, (function(n) {
+                                                return (0, v.dy)(we || (we = (0, a.Z)(["\n                  <ha-icon-button\n                    .label=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), e.lcn.localize("dashboard-devices-table-delete"), Oe, (function(n) {
                                                     return e._onDeviceDelete(n, t)
                                                 }))
                                             }
                                         }
                                     } : {
                                         name: {
                                             title: e.lcn.localize("name"),
@@ -1169,15 +1169,15 @@
                                             width: "15%"
                                         },
                                         delete: {
                                             title: "",
                                             sortable: !1,
                                             width: "80px",
                                             template: function(t) {
-                                                return (0, _.dy)(xe || (xe = (0, a.Z)(["\n                  <ha-icon-button\n                    .label=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), e.lcn.localize("dashboard-devices-table-delete"), Oe, (function(n) {
+                                                return (0, v.dy)(xe || (xe = (0, a.Z)(["\n                  <ha-icon-button\n                    .label=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), e.lcn.localize("dashboard-devices-table-delete"), Oe, (function(n) {
                                                     return e._onDeviceDelete(n, t)
                                                 }))
                                             }
                                         }
                                     }
                                 }))
                             }
@@ -1187,15 +1187,15 @@
                             value: function(e) {
                                 (0, u.Z)((0, f.Z)(h.prototype), "firstUpdated", this).call(this, e), k()
                             }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return (0, _.dy)(Ze || (Ze = (0, a.Z)(["\n      <ha-data-table\n        .hass=", "\n        .columns=", "\n        .data=", "\n        .id=", "\n        .noDataText=", "\n        .dir=", "\n        auto-height\n        clickable\n        @row-click=", "\n      ></ha-data-table>\n    "])), this.hass, this._columns(this.narrow), this._devices(this.devices), "address", this.lcn.localize("dashboard-devices-table-no-data"), (0, x.Zu)(this.hass), this._rowClicked)
+                                return (0, v.dy)(Ze || (Ze = (0, a.Z)(["\n      <ha-data-table\n        .hass=", "\n        .columns=", "\n        .data=", "\n        .id=", "\n        .noDataText=", "\n        .dir=", "\n        auto-height\n        clickable\n        @row-click=", "\n      ></ha-data-table>\n    "])), this.hass, this._columns(this.narrow), this._devices(this.devices), "address", this.lcn.localize("dashboard-devices-table-no-data"), (0, x.Zu)(this.hass), this._rowClicked)
                             }
                         }, {
                             kind: "method",
                             key: "_rowClicked",
                             value: function(e) {
                                 this.lcn.address = e.detail.id, this._openDevice()
                             }
@@ -1226,17 +1226,17 @@
                             value: (n = (0, r.Z)((0, i.Z)().mark((function e(t) {
                                 var n;
                                 return (0, i.Z)().wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
                                         case 0:
                                             return n = this.devices.find((function(e) {
                                                 return e.address[0] === t[0] && e.address[1] === t[1] && e.address[2] === t[2]
-                                            })), e.next = 3, (0, m.g7)(this, {
+                                            })), e.next = 3, (0, _.g7)(this, {
                                                 title: "\n          ".concat(n.address[2] ? this.lcn.localize("dashboard-devices-dialog-delete-group-title") : this.lcn.localize("dashboard-devices-dialog-delete-module-title")),
-                                                text: (0, _.dy)(Ce || (Ce = (0, a.Z)(["", "\n          ", "\n          (", ":\n          ", " ", ", ", "\n          ", ")\n          <br />\n          ", ""])), this.lcn.localize("dashboard-devices-dialog-delete-text"), n.name ? "'".concat(n.name, "'") : "", n.address[2] ? this.lcn.localize("group") : this.lcn.localize("module"), this.lcn.localize("segment"), n.address[0], this.lcn.localize("id"), n.address[1], this.lcn.localize("dashboard-devices-dialog-delete-warning"))
+                                                text: (0, v.dy)(Ce || (Ce = (0, a.Z)(["", "\n          ", "\n          (", ":\n          ", " ", ", ", "\n          ", ")\n          <br />\n          ", ""])), this.lcn.localize("dashboard-devices-dialog-delete-text"), n.name ? "'".concat(n.name, "'") : "", n.address[2] ? this.lcn.localize("group") : this.lcn.localize("module"), this.lcn.localize("segment"), n.address[0], this.lcn.localize("id"), n.address[1], this.lcn.localize("dashboard-devices-dialog-delete-warning"))
                                             });
                                         case 3:
                                             if (e.sent) {
                                                 e.next = 5;
                                                 break
                                             }
                                             return e.abrupt("return");
@@ -1250,15 +1250,15 @@
                                     }
                                 }), e, this)
                             }))), function(e) {
                                 return n.apply(this, arguments)
                             })
                         }]
                     }
-                }), _.oi), (0, h.Z)([(0, v.Mo)("lcn-config-dashboard")], (function(e, t) {
+                }), v.oi), (0, h.Z)([(0, m.Mo)("lcn-config-dashboard")], (function(e, t) {
                     var n, h, w, x, Z, C = function(t) {
                         (0, d.Z)(a, t);
                         var n = (0, s.Z)(a);
 
                         function a() {
                             var t;
                             (0, o.Z)(this, a);
@@ -1267,132 +1267,122 @@
                         }
                         return (0, l.Z)(a)
                     }(t);
                     return {
                         F: C,
                         d: [{
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "lcn",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 type: Boolean
                             })],
                             key: "narrow",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
                                 attribute: !1
                             })],
                             key: "route",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, v.Cb)({
+                            decorators: [(0, m.Cb)({
+                                attribute: !1
+                            })],
+                            key: "hosts",
+                            value: void 0
+                        }, {
+                            kind: "field",
+                            decorators: [(0, m.Cb)({
                                 type: Array,
                                 reflect: !1
                             })],
                             key: "tabs",
                             value: function() {
                                 return []
                             }
                         }, {
                             kind: "field",
-                            decorators: [(0, v.SB)()],
-                            key: "_hosts",
-                            value: function() {
-                                return []
-                            }
-                        }, {
-                            kind: "field",
-                            decorators: [(0, v.SB)()],
+                            decorators: [(0, m.SB)()],
                             key: "_deviceConfigs",
                             value: function() {
                                 return []
                             }
                         }, {
-                            kind: "field",
-                            decorators: [(0, v.IO)("#host-select")],
-                            key: "_hostsSelect",
-                            value: void 0
-                        }, {
                             kind: "method",
                             key: "firstUpdated",
                             value: (Z = (0, r.Z)((0, i.Z)().mark((function e(t) {
                                 var n = this;
                                 return (0, i.Z)().wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
                                         case 0:
-                                            return (0, u.Z)((0, f.Z)(C.prototype), "firstUpdated", this).call(this, t), e.next = 3, this._fetchHosts();
-                                        case 3:
-                                            (0, y.z)(), k(), this._hostsSelect.value = this.lcn.host.id, this.addEventListener("lcn-config-changed", (0, r.Z)((0, i.Z)().mark((function e() {
+                                            (0, u.Z)((0, f.Z)(C.prototype), "firstUpdated", this).call(this, t), (0, y.z)(), k(), this.addEventListener("lcn-config-changed", (0, r.Z)((0, i.Z)().mark((function e() {
                                                 return (0, i.Z)().wrap((function(e) {
                                                     for (;;) switch (e.prev = e.next) {
                                                         case 0:
                                                             n._fetchDevices(n.lcn.host);
                                                         case 1:
                                                         case "end":
                                                             return e.stop()
                                                     }
                                                 }), e)
                                             }))));
-                                        case 7:
+                                        case 4:
                                         case "end":
                                             return e.stop()
                                     }
                                 }), e, this)
                             }))), function(e) {
                                 return Z.apply(this, arguments)
                             })
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return this.hass && this.lcn ? (0, _.dy)(Re || (Re = (0, a.Z)(["\n      <hass-tabs-subpage\n        .hass=", "\n        .narrow=", '\n        back-path="/lcn"\n        .route=', "\n        .tabs=", "\n      >\n        <ha-config-section .narrow=", '>\n          <span slot="header"> ', ' </span>\n\n          <span slot="introduction"> ', ' </span>\n\n          <div id="box">\n            <ha-select\n              id="host-select"\n              .label=', "\n              .value=", "\n              fixedMenuPosition\n              @selected=", "\n            >\n              ", '\n            </ha-select>\n\n            <mwc-button id="scan_devices" raised @click=', ">\n              ", '\n            </mwc-button>\n          </div>\n\n          <ha-card\n            header="', ": ", '"\n          >\n            <lcn-devices-data-table\n              .hass=', "\n              .lcn=", "\n              .devices=", "\n              .narrow=", '\n            ></lcn-devices-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot="fab"\n          @click=', "\n          .label=", '\n          extended\n        >\n          <ha-svg-icon slot="icon" .path=', "></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    "])), this.hass, this.narrow, this.route, this.tabs, this.narrow, this.lcn.localize("dashboard-devices-title"), this.lcn.localize("dashboard-devices-introduction"), this.lcn.localize("dashboard-devices-hosts"), this.lcn.host.id, this._hostChanged, this._hosts.map((function(e) {
-                                    return (0, _.dy)(De || (De = (0, a.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.id, e.name)
-                                })), this._scanDevices, this.lcn.localize("dashboard-devices-scan"), this.lcn.localize("dashboard-devices-for-host"), this.lcn.host.name, this.hass, this.lcn, this._deviceConfigs, this.narrow, this._addDevice, this.lcn.localize("dashboard-devices-add"), "M19,13H13V19H11V13H5V11H11V5H13V11H19V13Z") : (0, _.dy)(ze || (ze = (0, a.Z)([" <hass-loading-screen></hass-loading-screen> "])))
+                                return this.hass && this.lcn && this.hosts ? (0, v.dy)(Re || (Re = (0, a.Z)(["\n      <hass-tabs-subpage\n        .hass=", "\n        .narrow=", "\n        .route=", "\n        .tabs=", '\n        main-page\n      >\n        <span slot="header"> ', " </span>\n        <ha-config-section .narrow=", '>\n          <span slot="introduction"> ', ' </span>\n\n          <div id="box">\n            <ha-select\n              id="host-select"\n              .label=', "\n              .value=", "\n              fixedMenuPosition\n              @selected=", "\n            >\n              ", '\n            </ha-select>\n\n            <mwc-button id="scan_devices" raised @click=', ">\n              ", '\n            </mwc-button>\n          </div>\n\n          <ha-card\n            header="', ": ", '"\n          >\n            <lcn-devices-data-table\n              .hass=', "\n              .lcn=", "\n              .devices=", "\n              .narrow=", '\n            ></lcn-devices-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot="fab"\n          @click=', "\n          .label=", '\n          extended\n        >\n          <ha-svg-icon slot="icon" .path=', "></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    "])), this.hass, this.narrow, this.route, this.tabs, this.lcn.localize("dashboard-devices-title"), this.narrow, this.renderIntro(), this.lcn.localize("dashboard-devices-hosts"), this.lcn.host.id, this._hostChanged, this.hosts.map((function(e) {
+                                    return (0, v.dy)(De || (De = (0, a.Z)([" <ha-list-item .value=", "> ", " </ha-list-item> "])), e.id, e.name)
+                                })), this._scanDevices, this.lcn.localize("dashboard-devices-scan"), this.lcn.localize("dashboard-devices-for-host"), this.lcn.host.name, this.hass, this.lcn, this._deviceConfigs, this.narrow, this._addDevice, this.lcn.localize("dashboard-devices-add"), "M19,13H13V19H11V13H5V11H11V5H13V11H19V13Z") : (0, v.dy)(ze || (ze = (0, a.Z)([" <hass-loading-screen></hass-loading-screen> "])))
                             }
                         }, {
                             kind: "method",
-                            key: "_hostChanged",
-                            value: function(e) {
-                                var t = e.target,
-                                    n = this._hosts.find((function(e) {
-                                        return e.id === t.value
-                                    }));
-                                this.lcn.host = n, this._fetchDevices(this.lcn.host)
+                            key: "renderIntro",
+                            value: function() {
+                                return (0, v.dy)(Le || (Le = (0, a.Z)(["\n      <h2>", "</h2>\n      ", " <br />\n      <details>\n        <summary>", "</summary>\n        <ul>\n          <li>", "</li>\n          <li>", "</li>\n          <li>", "</li>\n          <li>", "</li>\n        </ul>\n      </details>\n    "])), this.lcn.localize("dashboard-devices-introduction"), this.lcn.localize("dashboard-devices-introduction-help-1"), this.lcn.localize("more-help"), this.lcn.localize("dashboard-devices-introduction-help-2"), this.lcn.localize("dashboard-devices-introduction-help-3"), this.lcn.localize("dashboard-devices-introduction-help-4"), this.lcn.localize("dashboard-devices-introduction-help-5"))
                             }
                         }, {
                             kind: "method",
-                            key: "_fetchHosts",
-                            value: (x = (0, r.Z)((0, i.Z)().mark((function e() {
+                            key: "_hostChanged",
+                            value: (x = (0, r.Z)((0, i.Z)().mark((function e(t) {
+                                var n, a;
                                 return (0, i.Z)().wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
                                         case 0:
-                                            return e.next = 2, (0, p.V5)(this.hass);
-                                        case 2:
-                                            this._hosts = e.sent;
-                                        case 3:
+                                            return n = t.target, a = this.hosts.find((function(e) {
+                                                return e.id === n.value
+                                            })), this.lcn.host = a, e.next = 5, this._fetchDevices(this.lcn.host);
+                                        case 5:
                                         case "end":
                                             return e.stop()
                                     }
                                 }), e, this)
-                            }))), function() {
+                            }))), function(e) {
                                 return x.apply(this, arguments)
                             })
                         }, {
                             kind: "method",
                             key: "_fetchDevices",
                             value: (w = (0, r.Z)((0, i.Z)().mark((function e(t) {
                                 return (0, i.Z)().wrap((function(e) {
@@ -1453,24 +1443,24 @@
                             value: (n = (0, r.Z)((0, i.Z)().mark((function e(t) {
                                 var n;
                                 return (0, i.Z)().wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
                                         case 0:
                                             return n = (0, y.Y)(this, {
                                                 title: this.lcn.localize("dashboard-devices-dialog-request-info-title"),
-                                                text: (0, _.dy)(Le || (Le = (0, a.Z)(["\n        ", "\n        <br />\n        ", "\n      "])), this.lcn.localize("dashboard-devices-dialog-request-info-text"), this.lcn.localize("dashboard-devices-dialog-request-info-hint"))
+                                                text: (0, v.dy)(Se || (Se = (0, a.Z)(["\n        ", "\n        <br />\n        ", "\n      "])), this.lcn.localize("dashboard-devices-dialog-request-info-text"), this.lcn.localize("dashboard-devices-dialog-request-info-hint"))
                                             }), e.next = 3, (0, p.S6)(this.hass, this.lcn.host.id, t);
                                         case 3:
                                             if (e.sent) {
                                                 e.next = 8;
                                                 break
                                             }
-                                            return n().closeDialog(), e.next = 7, (0, m.Ys)(this, {
+                                            return n().closeDialog(), e.next = 7, (0, _.Ys)(this, {
                                                 title: this.lcn.localize("dashboard-devices-dialog-add-alert-title"),
-                                                text: (0, _.dy)(Se || (Se = (0, a.Z)(["", "\n          (", ":\n          ", " ", ", ", "\n          ", ")\n          <br />\n          ", ""])), this.lcn.localize("dashboard-devices-dialog-add-alert-text"), t.address[2] ? this.lcn.localize("group") : this.lcn.localize("module"), this.lcn.localize("segment"), t.address[0], this.lcn.localize("id"), t.address[1], this.lcn.localize("dashboard-devices-dialog-add-alert-hint"))
+                                                text: (0, v.dy)(Ee || (Ee = (0, a.Z)(["", "\n          (", ":\n          ", " ", ", ", "\n          ", ")\n          <br />\n          ", ""])), this.lcn.localize("dashboard-devices-dialog-add-alert-text"), t.address[2] ? this.lcn.localize("group") : this.lcn.localize("module"), this.lcn.localize("segment"), t.address[0], this.lcn.localize("id"), t.address[1], this.lcn.localize("dashboard-devices-dialog-add-alert-hint"))
                                             });
                                         case 7:
                                             return e.abrupt("return");
                                         case 8:
                                             n().closeDialog(), this._fetchDevices(this.lcn.host);
                                         case 10:
                                         case "end":
@@ -1481,19 +1471,19 @@
                                 return n.apply(this, arguments)
                             })
                         }, {
                             kind: "get",
                             static: !0,
                             key: "styles",
                             value: function() {
-                                return [b.Qx, (0, _.iv)(Ee || (Ee = (0, a.Z)(["\n        #box {\n          display: flex;\n          justify-content: space-between;\n        }\n        #host-select {\n          width: 40%;\n          display: inline-block;\n        }\n        #scan-devices {\n          display: inline-block;\n          margin-top: 20px;\n          justify-content: center;\n        }\n      "])))]
+                                return [b.Qx, (0, v.iv)(He || (He = (0, a.Z)(["\n        #box {\n          display: flex;\n          justify-content: space-between;\n        }\n        #host-select {\n          width: 40%;\n          display: inline-block;\n        }\n        #scan-devices {\n          display: inline-block;\n          margin-top: 20px;\n          justify-content: center;\n        }\n        summary:hover {\n          text-decoration: underline;\n        }\n      "])))]
                             }
                         }]
                     }
-                }), _.oi))
+                }), v.oi))
         },
         79894: function(e, t, n) {
             n(68077)({
                 target: "Number",
                 stat: !0,
                 nonConfigurable: !0,
                 nonWritable: !0
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VCTfVQ_Y.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VCTfVQ_Y.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VCTfVQ_Y.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VCTfVQ_Y.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VYXPimMw.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VYXPimMw.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/VYXPimMw.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/VYXPimMw.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ZshdvKRY.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ZshdvKRY.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ZshdvKRY.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ZshdvKRY.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/entrypoint-IIGRb-2R.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/entrypoint-YtbOLj1f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see entrypoint-IIGRb-2R.js.LICENSE.txt */ ! function() {
+/*! For license information please see entrypoint-YtbOLj1f.js.LICENSE.txt */ ! function() {
     var t, e, r, n, o = {
             18394: function(t, e, r) {
                 "use strict";
                 r.d(e, {
                     B: function() {
                         return n
                     }
@@ -368,14 +368,102 @@
                         return {
                             proxy: new t(r, n),
                             revoke: e
                         }
                     }, t
                 }
             },
+            9051: function(t, e, r) {
+                "use strict";
+                r.d(e, {
+                    Ce: function() {
+                        return s
+                    },
+                    Ks: function() {
+                        return c
+                    },
+                    LO: function() {
+                        return o
+                    },
+                    S6: function() {
+                        return u
+                    },
+                    V5: function() {
+                        return n
+                    },
+                    Vy: function() {
+                        return a
+                    },
+                    n1: function() {
+                        return l
+                    },
+                    rI: function() {
+                        return i
+                    }
+                });
+                r(22859);
+                var n = function(t) {
+                        return t.callWS({
+                            type: "lcn/hosts"
+                        })
+                    },
+                    o = function(t, e) {
+                        return t.callWS({
+                            type: "lcn/devices",
+                            host_id: e
+                        })
+                    },
+                    i = function(t, e, r) {
+                        return t.callWS({
+                            type: "lcn/entities",
+                            host_id: e,
+                            address: r
+                        })
+                    },
+                    a = function(t, e) {
+                        return t.callWS({
+                            type: "lcn/devices/scan",
+                            host_id: e
+                        })
+                    },
+                    s = function(t, e, r) {
+                        return t.callWS({
+                            type: "lcn/entities/add",
+                            host_id: e,
+                            address: r.address,
+                            name: r.name,
+                            domain: r.domain,
+                            domain_data: r.domain_data
+                        })
+                    },
+                    c = function(t, e, r) {
+                        return t.callWS({
+                            type: "lcn/entities/delete",
+                            host_id: e,
+                            address: r.address,
+                            domain: r.domain,
+                            resource: r.resource
+                        })
+                    },
+                    u = function(t, e, r) {
+                        return t.callWS({
+                            type: "lcn/devices/add",
+                            host_id: e,
+                            address: r.address,
+                            name: r.name
+                        })
+                    },
+                    l = function(t, e, r) {
+                        return t.callWS({
+                            type: "lcn/devices/delete",
+                            host_id: e,
+                            address: r.address
+                        })
+                    }
+            },
             3355: function(t, e, r) {
                 function n(e) {
                     return t.exports = n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
                         return typeof t
                     } : function(t) {
                         return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
                     }, t.exports.__esModule = !0, t.exports.default = t.exports, n(e)
@@ -1077,26 +1165,26 @@
                             T = A[w](b ? {} : -0, 1) !== A,
                             O = p((function() {
                                 A.has(1)
                             })),
                             P = v((function(t) {
                                 new E(t)
                             })),
-                            R = !b && p((function() {
+                            C = !b && p((function() {
                                 for (var t = new E, e = 5; e--;) t[w](e, e);
                                 return !t.has(-0)
                             }));
                         P || ((_ = e((function(t, e) {
                             l(t, x);
                             var r = y(new E, t, _);
                             return h(e) || u(e, r[w], {
                                 that: r,
                                 AS_ENTRIES: m
                             }), r
-                        }))).prototype = x, x.constructor = _), (O || R) && (k("delete"), k("has"), m && k("get")), (R || T) && k(w), b && x.clear && delete x.clear
+                        }))).prototype = x, x.constructor = _), (O || C) && (k("delete"), k("has"), m && k("get")), (C || T) && k(w), b && x.clear && delete x.clear
                     }
                     return S[t] = _, n({
                         global: !0,
                         constructor: !0,
                         forced: _ !== E
                     }, S), g(_, t), b || r.setStrong(_, t, m), _
                 }
@@ -2181,33 +2269,33 @@
                         k = !(!r || !r.IS_RECORD),
                         A = !(!r || !r.IS_ITERATOR),
                         T = !(!r || !r.INTERRUPTED),
                         O = n(e, _),
                         P = function(t) {
                             return g && h(g, "normal", t), new p(!0, t)
                         },
-                        R = function(t) {
+                        C = function(t) {
                             return S ? (i(t), T ? O(t[0], t[1], P) : O(t[0], t[1])) : T ? O(t, P) : O(t)
                         };
                     if (k) g = t.iterator;
                     else if (A) g = t;
                     else {
                         if (!(y = f(t))) throw new d(a(t) + " is not iterable");
                         if (s(y)) {
                             for (m = 0, b = c(t); b > m; m++)
-                                if ((w = R(t[m])) && u(v, w)) return w;
+                                if ((w = C(t[m])) && u(v, w)) return w;
                             return new p(!1)
                         }
                         g = l(t, y)
                     }
                     for (E = k ? t.next : g.next; !(x = o(E, g)).done;) {
                         try {
-                            w = R(x.value)
-                        } catch (C) {
-                            h(g, "throw", C)
+                            w = C(x.value)
+                        } catch (R) {
+                            h(g, "throw", R)
                         }
                         if ("object" == typeof w && w && u(v, w)) return w
                     }
                     return new p(!1)
                 }
             },
             56208: function(t, e, r) {
@@ -2328,42 +2416,42 @@
                     _ = "values",
                     S = "entries",
                     k = function() {
                         return this
                     };
                 t.exports = function(t, e, r, a, p, g, A) {
                     c(r, e, a);
-                    var T, O, P, R = function(t) {
+                    var T, O, P, C = function(t) {
                             if (t === p && H) return H;
                             if (!w && t && t in L) return L[t];
                             switch (t) {
                                 case x:
                                 case _:
                                 case S:
                                     return function() {
                                         return new r(this, t)
                                     }
                             }
                             return function() {
                                 return new r(this)
                             }
                         },
-                        C = e + " Iterator",
+                        R = e + " Iterator",
                         I = !1,
                         L = t.prototype,
                         N = L[E] || L["@@iterator"] || p && L[p],
-                        H = !w && N || R(p),
-                        B = "Array" === e && L.entries || N;
-                    if (B && (T = u(B.call(new t))) !== Object.prototype && T.next && (i || u(T) === b || (l ? l(T, b) : s(T[E]) || d(T, E, k)), f(T, C, !0, !0), i && (v[C] = k)), y && p === _ && N && N.name !== _ && (!i && m ? h(L, "name", _) : (I = !0, H = function() {
+                        H = !w && N || C(p),
+                        M = "Array" === e && L.entries || N;
+                    if (M && (T = u(M.call(new t))) !== Object.prototype && T.next && (i || u(T) === b || (l ? l(T, b) : s(T[E]) || d(T, E, k)), f(T, R, !0, !0), i && (v[R] = k)), y && p === _ && N && N.name !== _ && (!i && m ? h(L, "name", _) : (I = !0, H = function() {
                             return o(N, this)
                         })), p)
                         if (O = {
-                                values: R(_),
-                                keys: g ? H : R(x),
-                                entries: R(S)
+                                values: C(_),
+                                keys: g ? H : C(x),
+                                entries: C(S)
                             }, A)
                             for (P in O)(w || I || !(P in L)) && d(L, P, O[P]);
                         else n({
                             target: e,
                             proto: !0,
                             forced: w || I
                         }, O);
@@ -3124,18 +3212,18 @@
                         p = h(d),
                         k = s(t),
                         A = p.raw;
                     if (A) return A.lastIndex = d.lastIndex, e = i(y, A, k), d.lastIndex = A.lastIndex, e;
                     var T = p.groups,
                         O = _ && d.sticky,
                         P = i(c, d),
-                        R = d.source,
-                        C = 0,
+                        C = d.source,
+                        R = 0,
                         I = k;
-                    if (O && (P = w(P, "y", ""), -1 === b(P, "g") && (P += "g"), I = E(k, d.lastIndex), d.lastIndex > 0 && (!d.multiline || d.multiline && "\n" !== m(k, d.lastIndex - 1)) && (R = "(?: " + R + ")", I = " " + I, C++), r = new RegExp("^(?:" + R + ")", P)), S && (r = new RegExp("^" + R + "$(?!\\s)", P)), x && (n = d.lastIndex), o = i(g, O ? r : d, I), O ? o ? (o.input = E(o.input, C), o[0] = E(o[0], C), o.index = d.lastIndex, d.lastIndex += o[0].length) : d.lastIndex = 0 : x && o && (d.lastIndex = d.global ? o.index + o[0].length : n), S && o && o.length > 1 && i(v, o[0], r, (function() {
+                    if (O && (P = w(P, "y", ""), -1 === b(P, "g") && (P += "g"), I = E(k, d.lastIndex), d.lastIndex > 0 && (!d.multiline || d.multiline && "\n" !== m(k, d.lastIndex - 1)) && (C = "(?: " + C + ")", I = " " + I, R++), r = new RegExp("^(?:" + C + ")", P)), S && (r = new RegExp("^" + C + "$(?!\\s)", P)), x && (n = d.lastIndex), o = i(g, O ? r : d, I), O ? o ? (o.input = E(o.input, R), o[0] = E(o[0], R), o.index = d.lastIndex, d.lastIndex += o[0].length) : d.lastIndex = 0 : x && o && (d.lastIndex = d.global ? o.index + o[0].length : n), S && o && o.length > 1 && i(v, o[0], r, (function() {
                             for (a = 1; a < arguments.length - 2; a++) void 0 === arguments[a] && (o[a] = void 0)
                         })), o && T)
                         for (o.groups = u = f(null), a = 0; a < T.length; a++) u[(l = T[a])[0]] = o[l[1]];
                     return o
                 }), t.exports = y
             },
             85891: function(t, e, r) {
@@ -3632,20 +3720,20 @@
                 }));
                 var P = function(t) {
                         if (f(T, t)) {
                             var e = T[t];
                             delete T[t], e()
                         }
                     },
-                    R = function(t) {
+                    C = function(t) {
                         return function() {
                             P(t)
                         }
                     },
-                    C = function(t) {
+                    R = function(t) {
                         P(t.data)
                     },
                     I = function(t) {
                         s.postMessage(k(t), n.protocol + "//" + n.host)
                     };
                 b && w || (b = function(t) {
                     g(arguments.length, 1);
@@ -3653,23 +3741,23 @@
                         r = p(arguments, 1);
                     return T[++A] = function() {
                         c(e, void 0, r)
                     }, o(A), A
                 }, w = function(t) {
                     delete T[t]
                 }, m ? o = function(t) {
-                    E.nextTick(R(t))
+                    E.nextTick(C(t))
                 } : x && x.now ? o = function(t) {
-                    x.now(R(t))
-                } : S && !y ? (a = (i = new S).port2, i.port1.onmessage = C, o = u(a.postMessage, a)) : s.addEventListener && l(s.postMessage) && !s.importScripts && n && "file:" !== n.protocol && !h(I) ? (o = I, s.addEventListener("message", C, !1)) : o = O in v("script") ? function(t) {
+                    x.now(C(t))
+                } : S && !y ? (a = (i = new S).port2, i.port1.onmessage = R, o = u(a.postMessage, a)) : s.addEventListener && l(s.postMessage) && !s.importScripts && n && "file:" !== n.protocol && !h(I) ? (o = I, s.addEventListener("message", R, !1)) : o = O in v("script") ? function(t) {
                     d.appendChild(v("script"))[O] = function() {
                         d.removeChild(this), P(t)
                     }
                 } : function(t) {
-                    setTimeout(R(t), 0)
+                    setTimeout(C(t), 0)
                 }), t.exports = {
                     set: b,
                     clear: w
                 }
             },
             29191: function(t, e, r) {
                 "use strict";
@@ -4623,35 +4711,35 @@
                             for (a = (i = A(u, 2)).length, s = 0; s < a; s++)
                                 if ((c = T(i, s)) < 48 || c > o) return NaN;
                             return parseInt(i, n)
                         }
                         return +u
                     },
                     P = u(E, !x(" 0o1") || !x("0b1") || x("+0x1")),
-                    R = function(t) {
+                    C = function(t) {
                         var e, r = arguments.length < 1 ? 0 : x(function(t) {
                             var e = p(t, "number");
                             return "bigint" == typeof e ? e : O(e)
                         }(t));
                         return h(S, e = this) && v((function() {
                             b(e)
-                        })) ? f(Object(r), this, R) : r
+                        })) ? f(Object(r), this, C) : r
                     };
-                R.prototype = S, P && !o && (S.constructor = R), n({
+                C.prototype = S, P && !o && (S.constructor = C), n({
                     global: !0,
                     constructor: !0,
                     wrap: !0,
                     forced: P
                 }, {
-                    Number: R
+                    Number: C
                 });
-                var C = function(t, e) {
+                var R = function(t, e) {
                     for (var r, n = i ? g(e) : "MAX_VALUE,MIN_VALUE,NaN,NEGATIVE_INFINITY,POSITIVE_INFINITY,EPSILON,MAX_SAFE_INTEGER,MIN_SAFE_INTEGER,isFinite,isInteger,isNaN,isSafeInteger,parseFloat,parseInt,fromString,range".split(","), o = 0; n.length > o; o++) l(e, r = n[o]) && !l(t, r) && m(t, r, y(e, r))
                 };
-                o && _ && C(s[E], _), (P || o) && C(s[E], x)
+                o && _ && R(s[E], _), (P || o) && R(s[E], x)
             },
             34281: function(t, e, r) {
                 "use strict";
                 r(68077)({
                     target: "Number",
                     stat: !0,
                     nonConfigurable: !0,
@@ -4991,22 +5079,22 @@
                     _ = r(70754),
                     S = r(29639),
                     k = r(12648),
                     A = r(44565),
                     T = r(15624),
                     O = r(1731),
                     P = "Promise",
-                    R = T.CONSTRUCTOR,
-                    C = T.REJECTION_EVENT,
+                    C = T.CONSTRUCTOR,
+                    R = T.REJECTION_EVENT,
                     I = T.SUBCLASSING,
                     L = k.getterFor(P),
                     N = k.set,
                     H = A && A.prototype,
-                    B = A,
-                    M = H,
+                    M = A,
+                    B = H,
                     j = u.TypeError,
                     D = u.document,
                     $ = u.process,
                     U = O.f,
                     Z = U,
                     F = !!(D && D.createEvent && u.dispatchEvent),
                     G = "unhandledrejection",
@@ -5034,15 +5122,15 @@
                         })))
                     },
                     K = function(t, e, r) {
                         var n, o;
                         F ? ((n = D.createEvent("Event")).promise = e, n.reason = r, n.initEvent(t, !1, !0), u.dispatchEvent(n)) : n = {
                             promise: e,
                             reason: r
-                        }, !C && (o = u["on" + t]) ? o(n) : t === G && x("Unhandled promise rejection", r)
+                        }, !R && (o = u["on" + t]) ? o(n) : t === G && x("Unhandled promise rejection", r)
                     },
                     X = function(t) {
                         l(w, u, (function() {
                             var e, r = t.facade,
                                 n = t.value;
                             if (Y(t) && (e = _((function() {
                                     c ? $.emit("unhandledRejection", n, r) : K(G, r, n)
@@ -5085,16 +5173,16 @@
                             } catch (o) {
                                 Q({
                                     done: !1
                                 }, o, t)
                             }
                         }
                     };
-                if (R && (M = (B = function(t) {
-                        m(this, M), v(t), l(n, this);
+                if (C && (B = (M = function(t) {
+                        m(this, B), v(t), l(n, this);
                         var e = L(this);
                         try {
                             t(J(tt, e), J(Q, e))
                         } catch (r) {
                             Q(e, r)
                         }
                     }).prototype, (n = function(t) {
@@ -5104,48 +5192,48 @@
                             notified: !1,
                             parent: !1,
                             reactions: new S,
                             rejection: !1,
                             state: 0,
                             value: void 0
                         })
-                    }).prototype = f(M, "then", (function(t, e) {
+                    }).prototype = f(B, "then", (function(t, e) {
                         var r = L(this),
-                            n = U(b(this, B));
+                            n = U(b(this, M));
                         return r.parent = !0, n.ok = !g(t) || t, n.fail = g(e) && e, n.domain = c ? $.domain : void 0, 0 === r.state ? r.reactions.add(n) : E((function() {
                             V(n, r)
                         })), n.promise
                     })), o = function() {
                         var t = new n,
                             e = L(t);
                         this.promise = t, this.resolve = J(tt, e), this.reject = J(Q, e)
                     }, O.f = U = function(t) {
-                        return t === B || undefined === t ? new o(t) : Z(t)
+                        return t === M || undefined === t ? new o(t) : Z(t)
                     }, !s && g(A) && H !== Object.prototype)) {
                     i = H.then, I || f(H, "then", (function(t, e) {
                         var r = this;
-                        return new B((function(t, e) {
+                        return new M((function(t, e) {
                             l(i, r, t, e)
                         })).then(t, e)
                     }), {
                         unsafe: !0
                     });
                     try {
                         delete H.constructor
                     } catch (et) {}
-                    h && h(H, M)
+                    h && h(H, B)
                 }
                 a({
                     global: !0,
                     constructor: !0,
                     wrap: !0,
-                    forced: R
+                    forced: C
                 }, {
-                    Promise: B
-                }), d(B, P, !1, !0), p(P)
+                    Promise: M
+                }), d(M, P, !1, !0), p(P)
             },
             47084: function(t, e, r) {
                 "use strict";
                 r(77280), r(75179), r(26900), r(34248), r(51941), r(80833)
             },
             34248: function(t, e, r) {
                 "use strict";
@@ -5320,35 +5408,35 @@
                     _ = r(70852),
                     S = E("match"),
                     k = o.RegExp,
                     A = k.prototype,
                     T = o.SyntaxError,
                     O = i(A.exec),
                     P = i("".charAt),
-                    R = i("".replace),
-                    C = i("".indexOf),
+                    C = i("".replace),
+                    R = i("".indexOf),
                     I = i("".slice),
                     L = /^\?<[^\s\d!#%&*+<=>@^][^\s!#%&*+<=>@^]*>/,
                     N = /a/g,
                     H = /a/g,
-                    B = new k(N) !== N,
-                    M = p.MISSED_STICKY,
+                    M = new k(N) !== N,
+                    B = p.MISSED_STICKY,
                     j = p.UNSUPPORTED_Y,
-                    D = n && (!B || M || x || _ || y((function() {
+                    D = n && (!M || B || x || _ || y((function() {
                         return H[S] = !1, k(N) !== N || k(H) === H || "/a/i" !== String(k(N, "i"))
                     })));
                 if (a("RegExp", D)) {
                     for (var $ = function(t, e) {
                             var r, n, o, i, a, u, p = l(A, this),
                                 v = f(t),
                                 g = void 0 === e,
                                 y = [],
                                 w = t;
                             if (!p && v && g && t.constructor === $) return t;
-                            if ((v || l(A, t)) && (t = t.source, g && (e = d(w))), t = void 0 === t ? "" : h(t), e = void 0 === e ? "" : h(e), w = t, x && "dotAll" in N && (n = !!e && C(e, "s") > -1) && (e = R(e, /s/g, "")), r = e, M && "sticky" in N && (o = !!e && C(e, "y") > -1) && j && (e = R(e, /y/g, "")), _ && (i = function(t) {
+                            if ((v || l(A, t)) && (t = t.source, g && (e = d(w))), t = void 0 === t ? "" : h(t), e = void 0 === e ? "" : h(e), w = t, x && "dotAll" in N && (n = !!e && R(e, "s") > -1) && (e = C(e, /s/g, "")), r = e, B && "sticky" in N && (o = !!e && R(e, "y") > -1) && j && (e = C(e, /y/g, "")), _ && (i = function(t) {
                                     for (var e, r = t.length, n = 0, o = "", i = [], a = {}, s = !1, c = !1, u = 0, l = ""; n <= r; n++) {
                                         if ("\\" === (e = P(t, n))) e += P(t, ++n);
                                         else if ("]" === e) s = !1;
                                         else if (!s) switch (!0) {
                                             case "[" === e:
                                                 s = !0;
                                                 break;
@@ -5643,24 +5731,24 @@
                         var p = u(o);
                         p || (o = d(o));
                         var g, b = a.global;
                         b && (g = a.unicode, a.lastIndex = 0);
                         for (var A, T = []; null !== (A = m(a, s)) && (_(T, A), b);) {
                             "" === d(A[0]) && (a.lastIndex = v(s, h(a.lastIndex), g))
                         }
-                        for (var O, P = "", R = 0, C = 0; C < T.length; C++) {
-                            for (var I, L = d((A = T[C])[0]), N = w(E(f(A.index), s.length), 0), H = [], B = 1; B < A.length; B++) _(H, void 0 === (O = A[B]) ? O : String(O));
-                            var M = A.groups;
+                        for (var O, P = "", C = 0, R = 0; R < T.length; R++) {
+                            for (var I, L = d((A = T[R])[0]), N = w(E(f(A.index), s.length), 0), H = [], M = 1; M < A.length; M++) _(H, void 0 === (O = A[M]) ? O : String(O));
+                            var B = A.groups;
                             if (p) {
                                 var j = x([L], H, N, s);
-                                void 0 !== M && _(j, M), I = d(n(o, void 0, j))
-                            } else I = y(L, s, N, H, M, o);
-                            N >= R && (P += k(s, R, N) + I, R = N + L.length)
+                                void 0 !== B && _(j, B), I = d(n(o, void 0, j))
+                            } else I = y(L, s, N, H, B, o);
+                            N >= C && (P += k(s, C, N) + I, C = N + L.length)
                         }
-                        return P + k(s, R)
+                        return P + k(s, C)
                     }]
                 }), !!s((function() {
                     var t = /./;
                     return t.exec = function() {
                         var t = [];
                         return t.groups = {
                             a: "7"
@@ -5888,25 +5976,25 @@
                     _ = r(25245),
                     S = r(54991),
                     k = r(44760),
                     A = r(60771),
                     T = r(73936),
                     O = r(40030),
                     P = r(82765),
-                    R = r(95292),
-                    C = r(46170),
+                    C = r(95292),
+                    R = r(46170),
                     I = r(92311),
                     L = r(10282),
                     N = r(97665),
                     H = r(80879),
-                    B = r(17497),
-                    M = r(48357),
+                    M = r(17497),
+                    B = r(48357),
                     j = r(12648),
                     D = r(78856).forEach,
-                    $ = R("hidden"),
+                    $ = C("hidden"),
                     U = "Symbol",
                     Z = "prototype",
                     F = j.set,
                     G = j.getterFor(U),
                     z = Object[Z],
                     V = o.Symbol,
                     W = V && V[Z],
@@ -5971,15 +6059,15 @@
                             return !o || !f(rt, n) || f(r, $) && r[$][n] || (o.enumerable = !0), o
                         }
                     },
                     dt = function(t) {
                         var e = Q(p(t)),
                             r = [];
                         return D(e, (function(t) {
-                            f(rt, t) || f(C, t) || et(r, t)
+                            f(rt, t) || f(R, t) || et(r, t)
                         })), r
                     },
                     pt = function(t) {
                         var e = t === z,
                             r = Q(e ? nt : p(t)),
                             n = [];
                         return D(r, (function(t) {
@@ -6053,15 +6141,15 @@
                     getOwnPropertyDescriptor: ht
                 }), n({
                     target: "Object",
                     stat: !0,
                     forced: !u
                 }, {
                     getOwnPropertyNames: dt
-                }), B(), M(V, U), C[$] = !0
+                }), M(), B(V, U), R[$] = !0
             },
             98214: function(t, e, r) {
                 "use strict";
                 var n = r(68077),
                     o = r(58849),
                     i = r(5813),
                     a = r(55418),
@@ -6200,42 +6288,42 @@
                     A = u("WeakMap", k, l),
                     T = A.prototype,
                     O = a(T.set);
                 if (p)
                     if (S) {
                         n = l.getConstructor(k, "WeakMap", !0), c.enable();
                         var P = a(T.delete),
-                            R = a(T.has),
-                            C = a(T.get);
+                            C = a(T.has),
+                            R = a(T.get);
                         s(T, {
                             delete: function(t) {
                                 if (f(t) && !y(t)) {
                                     var e = h(this);
                                     return e.frozen || (e.frozen = new n), P(this, t) || e.frozen.delete(t)
                                 }
                                 return P(this, t)
                             },
                             has: function(t) {
                                 if (f(t) && !y(t)) {
                                     var e = h(this);
-                                    return e.frozen || (e.frozen = new n), R(this, t) || e.frozen.has(t)
+                                    return e.frozen || (e.frozen = new n), C(this, t) || e.frozen.has(t)
                                 }
-                                return R(this, t)
+                                return C(this, t)
                             },
                             get: function(t) {
                                 if (f(t) && !y(t)) {
                                     var e = h(this);
-                                    return e.frozen || (e.frozen = new n), R(this, t) ? C(this, t) : e.frozen.get(t)
+                                    return e.frozen || (e.frozen = new n), C(this, t) ? R(this, t) : e.frozen.get(t)
                                 }
-                                return C(this, t)
+                                return R(this, t)
                             },
                             set: function(t, e) {
                                 if (f(t) && !y(t)) {
                                     var r = h(this);
-                                    r.frozen || (r.frozen = new n), R(this, t) ? O(this, t, e) : r.frozen.set(t, e)
+                                    r.frozen || (r.frozen = new n), C(this, t) ? O(this, t, e) : r.frozen.set(t, e)
                                 } else O(this, t, e);
                                 return this
                             }
                         })
                     } else o && d((function() {
                         var t = w([]);
                         return O(new A, t, 1), !m(t)
@@ -6449,16 +6537,16 @@
                     _ = a("Object", "keys"),
                     S = Object.getOwnPropertyDescriptor,
                     k = s("".charAt),
                     A = s("".slice),
                     T = s(/./.exec),
                     O = s([].push),
                     P = /^\d$/,
-                    R = /^[1-9]$/,
-                    C = /^(?:-|\d)$/,
+                    C = /^[1-9]$/,
+                    R = /^(?:-|\d)$/,
                     I = /^[\t\n\r ]$/,
                     L = function(t, e, r, n) {
                         var o, i, a, s, u, d = t[e],
                             v = n && d === n.value,
                             g = v && "string" == typeof n.source ? {
                                 source: n.source
                             } : {};
@@ -6478,27 +6566,27 @@
                             if (n && !n.configurable) return
                         }
                         void 0 === r ? delete t[e] : v(t, e, r)
                     },
                     H = function(t, e, r, n) {
                         this.value = t, this.end = e, this.source = r, this.nodes = n
                     },
-                    B = function(t, e) {
+                    M = function(t, e) {
                         this.source = t, this.index = e
                     };
-                B.prototype = {
+                M.prototype = {
                     fork: function(t) {
-                        return new B(this.source, t)
+                        return new M(this.source, t)
                     },
                     parse: function() {
                         var t = this.source,
                             e = this.skip(I, this.index),
                             r = this.fork(e),
                             n = k(t, e);
-                        if (T(C, n)) return r.number();
+                        if (T(R, n)) return r.number();
                         switch (n) {
                             case "{":
                                 return r.object();
                             case "[":
                                 return r.array();
                             case '"':
                                 return r.string();
@@ -6554,15 +6642,15 @@
                     },
                     number: function() {
                         var t = this.source,
                             e = this.index,
                             r = e;
                         if ("-" === k(t, r) && r++, "0" === k(t, r)) r++;
                         else {
-                            if (!T(R, k(t, r))) throw new E("Failed to parse number at: " + r);
+                            if (!T(C, k(t, r))) throw new E("Failed to parse number at: " + r);
                             r = this.skip(P, ++r)
                         }
                         if (("." === k(t, r) && (r = this.skip(P, ++r)), "e" === k(t, r) || "E" === k(t, r)) && (r++, "+" !== k(t, r) && "-" !== k(t, r) || r++, r === (r = this.skip(P, r)))) throw new E("Failed to parse number's exponent value at: " + r);
                         return this.node(0, w(A(t, e, r)), e, r)
                     },
                     keyword: function(t) {
                         var e = "" + t,
@@ -6578,32 +6666,32 @@
                     until: function(t, e) {
                         e = this.skip(I, e);
                         for (var r = k(this.source, e), n = 0; n < t.length; n++)
                             if (t[n] === r) return e;
                         throw new E('Unexpected character: "' + r + '" at: ' + e)
                     }
                 };
-                var M = g((function() {
+                var B = g((function() {
                         var t, e = "9007199254740993";
                         return x(e, (function(e, r, n) {
                             t = n.source
                         })), t !== e
                     })),
                     j = m && !g((function() {
                         return 1 / x("-0 \t") != -1 / 0
                     }));
                 n({
                     target: "JSON",
                     stat: !0,
-                    forced: M
+                    forced: B
                 }, {
                     parse: function(t, e) {
                         return j && !u(e) ? x(t) : function(t, e) {
                             t = d(t);
-                            var r = new B(t, 0, ""),
+                            var r = new M(t, 0, ""),
                                 n = r.parse(),
                                 o = n.value,
                                 i = r.skip(I, n.end);
                             if (i < t.length) throw new E('Unexpected extra character: "' + k(t, i) + '" after the parsed data at: ' + i);
                             return u(e) ? L({
                                 "": o
                             }, "", e, n) : o
@@ -7602,30 +7690,30 @@
                         if (o === t) return r.delegate = null, "throw" === n && e.iterator.return && (r.method = "return", r.arg = t, P(e, r), "throw" === r.method) || "return" !== n && (r.method = "throw", r.arg = new TypeError("The iterator does not provide a '" + n + "' method")), m;
                         var i = d(o, e.iterator, r.arg);
                         if ("throw" === i.type) return r.method = "throw", r.arg = i.arg, r.delegate = null, m;
                         var a = i.arg;
                         return a ? a.done ? (r[e.resultName] = a.value, r.next = e.nextLoc, "return" !== r.method && (r.method = "next", r.arg = t), r.delegate = null, m) : a : (r.method = "throw", r.arg = new TypeError("iterator result is not an object"), r.delegate = null, m)
                     }
 
-                    function R(t) {
+                    function C(t) {
                         var e = {
                             tryLoc: t[0]
                         };
                         1 in t && (e.catchLoc = t[1]), 2 in t && (e.finallyLoc = t[2], e.afterLoc = t[3]), this.tryEntries.push(e)
                     }
 
-                    function C(t) {
+                    function R(t) {
                         var e = t.completion || {};
                         e.type = "normal", delete e.arg, t.completion = e
                     }
 
                     function I(t) {
                         this.tryEntries = [{
                             tryLoc: "root"
-                        }], t.forEach(R, this), this.reset(!0)
+                        }], t.forEach(C, this), this.reset(!0)
                     }
 
                     function L(e) {
                         if (e || "" === e) {
                             var r = e[c];
                             if (r) return r.call(e);
                             if ("function" == typeof e.next) return e;
@@ -7679,15 +7767,15 @@
                                     if (n in e) return t.value = n, t.done = !1, t
                                 }
                                 return t.done = !0, t
                             }
                     }, e.values = L, I.prototype = {
                         constructor: I,
                         reset: function(e) {
-                            if (this.prev = 0, this.next = 0, this.sent = this._sent = t, this.done = !1, this.delegate = null, this.method = "next", this.arg = t, this.tryEntries.forEach(C), !e)
+                            if (this.prev = 0, this.next = 0, this.sent = this._sent = t, this.done = !1, this.delegate = null, this.method = "next", this.arg = t, this.tryEntries.forEach(R), !e)
                                 for (var r in this) "t" === r.charAt(0) && i.call(this, r) && !isNaN(+r.slice(1)) && (this[r] = t)
                         },
                         stop: function() {
                             this.done = !0;
                             var t = this.tryEntries[0].completion;
                             if ("throw" === t.type) throw t.arg;
                             return this.rval
@@ -7733,25 +7821,25 @@
                         complete: function(t, e) {
                             if ("throw" === t.type) throw t.arg;
                             return "break" === t.type || "continue" === t.type ? this.next = t.arg : "return" === t.type ? (this.rval = this.arg = t.arg, this.method = "return", this.next = "end") : "normal" === t.type && e && (this.next = e), m
                         },
                         finish: function(t) {
                             for (var e = this.tryEntries.length - 1; e >= 0; --e) {
                                 var r = this.tryEntries[e];
-                                if (r.finallyLoc === t) return this.complete(r.completion, r.afterLoc), C(r), m
+                                if (r.finallyLoc === t) return this.complete(r.completion, r.afterLoc), R(r), m
                             }
                         },
                         catch: function(t) {
                             for (var e = this.tryEntries.length - 1; e >= 0; --e) {
                                 var r = this.tryEntries[e];
                                 if (r.tryLoc === t) {
                                     var n = r.completion;
                                     if ("throw" === n.type) {
                                         var o = n.arg;
-                                        C(r)
+                                        R(r)
                                     }
                                     return o
                                 }
                             }
                             throw new Error("illegal catch attempt")
                         },
                         delegateYield: function(e, r, n) {
@@ -7999,15 +8087,15 @@
                     Al: function() {
                         return q
                     },
                     Jb: function() {
                         return H
                     },
                     Ld: function() {
-                        return B
+                        return M
                     },
                     YP: function() {
                         return N
                     },
                     dy: function() {
                         return L
                     },
@@ -8047,40 +8135,40 @@
                     },
                     S = "[ \t\n\f\r]",
                     k = /<(?:(!--|\/[^a-zA-Z])|(\/?[a-zA-Z][^>\s]*)|(\/?$))/g,
                     A = /-->/g,
                     T = />/g,
                     O = RegExp(">|".concat(S, "(?:([^\\s\"'>=/]+)(").concat(S, "*=").concat(S, "*(?:[^ \t\n\f\r\"'`<>=]|(\"|')|))|$)"), "g"),
                     P = /'/g,
-                    R = /"/g,
-                    C = /^(?:script|style|textarea|title)$/i,
+                    C = /"/g,
+                    R = /^(?:script|style|textarea|title)$/i,
                     I = function(t) {
                         return function(e) {
                             for (var r = arguments.length, n = new Array(r > 1 ? r - 1 : 0), o = 1; o < r; o++) n[o - 1] = arguments[o];
                             return {
                                 _$litType$: t,
                                 strings: e,
                                 values: n
                             }
                         }
                     },
                     L = I(1),
                     N = I(2),
                     H = Symbol.for("lit-noChange"),
-                    B = Symbol.for("lit-nothing"),
-                    M = new WeakMap,
+                    M = Symbol.for("lit-nothing"),
+                    B = new WeakMap,
                     j = b.createTreeWalker(b, 129, null, !1);
 
                 function D(t, e) {
                     if (!Array.isArray(t) || !t.hasOwnProperty("raw")) throw Error("invalid template strings array");
                     return void 0 !== p ? p.createHTML(e) : e
                 }
                 var $ = function(t, e) {
                         for (var r, n = t.length - 1, o = [], i = 2 === e ? "<svg>" : "", a = k, s = 0; s < n; s++) {
-                            for (var c = t[s], u = void 0, l = void 0, f = -1, h = 0; h < c.length && (a.lastIndex = h, null !== (l = a.exec(c)));) h = a.lastIndex, a === k ? "!--" === l[1] ? a = A : void 0 !== l[1] ? a = T : void 0 !== l[2] ? (C.test(l[2]) && (r = RegExp("</" + l[2], "g")), a = O) : void 0 !== l[3] && (a = O) : a === O ? ">" === l[0] ? (a = null != r ? r : k, f = -1) : void 0 === l[1] ? f = -2 : (f = a.lastIndex - l[2].length, u = l[1], a = void 0 === l[3] ? O : '"' === l[3] ? R : P) : a === R || a === P ? a = O : a === A || a === T ? a = k : (a = O, r = void 0);
+                            for (var c = t[s], u = void 0, l = void 0, f = -1, h = 0; h < c.length && (a.lastIndex = h, null !== (l = a.exec(c)));) h = a.lastIndex, a === k ? "!--" === l[1] ? a = A : void 0 !== l[1] ? a = T : void 0 !== l[2] ? (R.test(l[2]) && (r = RegExp("</" + l[2], "g")), a = O) : void 0 !== l[3] && (a = O) : a === O ? ">" === l[0] ? (a = null != r ? r : k, f = -1) : void 0 === l[1] ? f = -2 : (f = a.lastIndex - l[2].length, u = l[1], a = void 0 === l[3] ? O : '"' === l[3] ? C : P) : a === C || a === P ? a = O : a === A || a === T ? a = k : (a = O, r = void 0);
                             var d = a === O && t[s + 1].startsWith("/>") ? " " : "";
                             i += a === k ? c + m : f >= 0 ? (o.push(u), c.slice(0, f) + v + c.slice(f) + g + d) : c + g + (-2 === f ? (o.push(void 0), s) : d)
                         }
                         return [D(t, i + (t[n] || "<?>") + (2 === e ? "</svg>" : "")), o]
                     },
                     U = function() {
                         function t(e, r) {
@@ -8107,21 +8195,21 @@
                                             T = (0, a.Z)(n.getAttributeNames());
                                         try {
                                             for (T.s(); !(k = T.n()).done;) {
                                                 var O = k.value;
                                                 if (O.endsWith(v) || O.startsWith(g)) {
                                                     var P = x[f++];
                                                     if (A.push(O), void 0 !== P) {
-                                                        var R = n.getAttribute(P.toLowerCase() + v).split(g),
+                                                        var C = n.getAttribute(P.toLowerCase() + v).split(g),
                                                             I = /([.?@])?(.*)/.exec(P);
                                                         p.push({
                                                             type: 1,
                                                             index: l,
                                                             name: I[2],
-                                                            strings: R,
+                                                            strings: C,
                                                             ctor: "." === I[1] ? V : "?" === I[1] ? K : "@" === I[1] ? X : z
                                                         })
                                                     } else p.push({
                                                         type: 6,
                                                         index: l
                                                     })
                                                 }
@@ -8132,24 +8220,24 @@
                                             T.f()
                                         }
                                         for (var L = 0, N = A; L < N.length; L++) {
                                             var H = N[L];
                                             n.removeAttribute(H)
                                         }
                                     }
-                                    if (C.test(n.tagName)) {
-                                        var B = n.textContent.split(g),
-                                            M = B.length - 1;
-                                        if (M > 0) {
+                                    if (R.test(n.tagName)) {
+                                        var M = n.textContent.split(g),
+                                            B = M.length - 1;
+                                        if (B > 0) {
                                             n.textContent = d ? d.emptyScript : "";
-                                            for (var D = 0; D < M; D++) n.append(B[D], w()), j.nextNode(), p.push({
+                                            for (var D = 0; D < B; D++) n.append(M[D], w()), j.nextNode(), p.push({
                                                 type: 2,
                                                 index: ++l
                                             });
-                                            n.append(B[M], w())
+                                            n.append(M[B], w())
                                         }
                                     }
                                 } else if (8 === n.nodeType)
                                     if (n.data === y) p.push({
                                         type: 2,
                                         index: l
                                     });
@@ -8226,15 +8314,15 @@
                                 }
                             }
                         }]), t
                     }(),
                     G = function() {
                         function t(e, r, n, o) {
                             var i;
-                            (0, u.Z)(this, t), this.type = 2, this._$AH = B, this._$AN = void 0, this._$AA = e, this._$AB = r, this._$AM = n, this.options = o, this._$Cp = null === (i = null == o ? void 0 : o.isConnected) || void 0 === i || i
+                            (0, u.Z)(this, t), this.type = 2, this._$AH = M, this._$AN = void 0, this._$AA = e, this._$AB = r, this._$AM = n, this.options = o, this._$Cp = null === (i = null == o ? void 0 : o.isConnected) || void 0 === i || i
                         }
                         return (0, l.Z)(t, [{
                             key: "_$AU",
                             get: function() {
                                 var t, e;
                                 return null !== (e = null === (t = this._$AM) || void 0 === t ? void 0 : t._$AU) && void 0 !== e ? e : this._$Cp
                             }
@@ -8254,30 +8342,30 @@
                             key: "endNode",
                             get: function() {
                                 return this._$AB
                             }
                         }, {
                             key: "_$AI",
                             value: function(t) {
-                                t = Z(this, t, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this), E(t) ? t === B || null == t || "" === t ? (this._$AH !== B && this._$AR(), this._$AH = B) : t !== this._$AH && t !== H && this._(t) : void 0 !== t._$litType$ ? this.g(t) : void 0 !== t.nodeType ? this.$(t) : _(t) ? this.T(t) : this._(t)
+                                t = Z(this, t, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this), E(t) ? t === M || null == t || "" === t ? (this._$AH !== M && this._$AR(), this._$AH = M) : t !== this._$AH && t !== H && this._(t) : void 0 !== t._$litType$ ? this.g(t) : void 0 !== t.nodeType ? this.$(t) : _(t) ? this.T(t) : this._(t)
                             }
                         }, {
                             key: "k",
                             value: function(t) {
                                 return this._$AA.parentNode.insertBefore(t, this._$AB)
                             }
                         }, {
                             key: "$",
                             value: function(t) {
                                 this._$AH !== t && (this._$AR(), this._$AH = this.k(t))
                             }
                         }, {
                             key: "_",
                             value: function(t) {
-                                this._$AH !== B && E(this._$AH) ? this._$AA.nextSibling.data = t : this.$(b.createTextNode(t)), this._$AH = t
+                                this._$AH !== M && E(this._$AH) ? this._$AA.nextSibling.data = t : this.$(b.createTextNode(t)), this._$AH = t
                             }
                         }, {
                             key: "g",
                             value: function(t) {
                                 var e, r = t.values,
                                     n = t._$litType$,
                                     o = "number" == typeof n ? this._$AC(t) : (void 0 === n.el && (n.el = U.createElement(D(n.h, n.h[0]), this.options)), n);
@@ -8287,16 +8375,16 @@
                                         a = i.u(this.options);
                                     i.v(r), this.$(a), this._$AH = i
                                 }
                             }
                         }, {
                             key: "_$AC",
                             value: function(t) {
-                                var e = M.get(t.strings);
-                                return void 0 === e && M.set(t.strings, e = new U(t)), e
+                                var e = B.get(t.strings);
+                                return void 0 === e && B.set(t.strings, e = new U(t)), e
                             }
                         }, {
                             key: "T",
                             value: function(e) {
                                 x(this._$AH) || (this._$AH = [], this._$AR());
                                 var r, n, o = this._$AH,
                                     i = 0,
@@ -8329,15 +8417,15 @@
                                 var e;
                                 void 0 === this._$AM && (this._$Cp = t, null === (e = this._$AP) || void 0 === e || e.call(this, t))
                             }
                         }]), t
                     }(),
                     z = function() {
                         function t(e, r, n, o, i) {
-                            (0, u.Z)(this, t), this.type = 1, this._$AH = B, this._$AN = void 0, this.element = e, this.name = r, this._$AM = o, this.options = i, n.length > 2 || "" !== n[0] || "" !== n[1] ? (this._$AH = Array(n.length - 1).fill(new String), this.strings = n) : this._$AH = B
+                            (0, u.Z)(this, t), this.type = 1, this._$AH = M, this._$AN = void 0, this.element = e, this.name = r, this._$AM = o, this.options = i, n.length > 2 || "" !== n[0] || "" !== n[1] ? (this._$AH = Array(n.length - 1).fill(new String), this.strings = n) : this._$AH = M
                         }
                         return (0, l.Z)(t, [{
                             key: "tagName",
                             get: function() {
                                 return this.element.tagName
                             }
                         }, {
@@ -8352,37 +8440,37 @@
                                     r = arguments.length > 2 ? arguments[2] : void 0,
                                     n = arguments.length > 3 ? arguments[3] : void 0,
                                     o = this.strings,
                                     i = !1;
                                 if (void 0 === o) t = Z(this, t, e, 0), (i = !E(t) || t !== this._$AH && t !== H) && (this._$AH = t);
                                 else {
                                     var a, s, c = t;
-                                    for (t = o[0], a = 0; a < o.length - 1; a++)(s = Z(this, c[r + a], e, a)) === H && (s = this._$AH[a]), i || (i = !E(s) || s !== this._$AH[a]), s === B ? t = B : t !== B && (t += (null != s ? s : "") + o[a + 1]), this._$AH[a] = s
+                                    for (t = o[0], a = 0; a < o.length - 1; a++)(s = Z(this, c[r + a], e, a)) === H && (s = this._$AH[a]), i || (i = !E(s) || s !== this._$AH[a]), s === M ? t = M : t !== M && (t += (null != s ? s : "") + o[a + 1]), this._$AH[a] = s
                                 }
                                 i && !n && this.j(t)
                             }
                         }, {
                             key: "j",
                             value: function(t) {
-                                t === B ? this.element.removeAttribute(this.name) : this.element.setAttribute(this.name, null != t ? t : "")
+                                t === M ? this.element.removeAttribute(this.name) : this.element.setAttribute(this.name, null != t ? t : "")
                             }
                         }]), t
                     }(),
                     V = function(t) {
                         (0, o.Z)(r, t);
                         var e = (0, i.Z)(r);
 
                         function r() {
                             var t;
                             return (0, u.Z)(this, r), (t = e.apply(this, arguments)).type = 3, t
                         }
                         return (0, l.Z)(r, [{
                             key: "j",
                             value: function(t) {
-                                this.element[this.name] = t === B ? void 0 : t
+                                this.element[this.name] = t === M ? void 0 : t
                             }
                         }]), r
                     }(z),
                     W = d ? d.emptyScript : "",
                     K = function(t) {
                         (0, o.Z)(r, t);
                         var e = (0, i.Z)(r);
@@ -8390,15 +8478,15 @@
                         function r() {
                             var t;
                             return (0, u.Z)(this, r), (t = e.apply(this, arguments)).type = 4, t
                         }
                         return (0, l.Z)(r, [{
                             key: "j",
                             value: function(t) {
-                                t && t !== B ? this.element.setAttribute(this.name, W) : this.element.removeAttribute(this.name)
+                                t && t !== M ? this.element.setAttribute(this.name, W) : this.element.removeAttribute(this.name)
                             }
                         }]), r
                     }(z),
                     X = function(t) {
                         (0, o.Z)(r, t);
                         var e = (0, i.Z)(r);
 
@@ -8406,18 +8494,18 @@
                             var s;
                             return (0, u.Z)(this, r), (s = e.call(this, t, n, o, i, a)).type = 5, s
                         }
                         return (0, l.Z)(r, [{
                             key: "_$AI",
                             value: function(t) {
                                 var e;
-                                if ((t = null !== (e = Z(this, t, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this, 0)) && void 0 !== e ? e : B) !== H) {
+                                if ((t = null !== (e = Z(this, t, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this, 0)) && void 0 !== e ? e : M) !== H) {
                                     var r = this._$AH,
-                                        n = t === B && r !== B || t.capture !== r.capture || t.once !== r.once || t.passive !== r.passive,
-                                        o = t !== B && (r === B || n);
+                                        n = t === M && r !== M || t.capture !== r.capture || t.once !== r.once || t.passive !== r.passive,
+                                        o = t !== M && (r === M || n);
                                     n && this.element.removeEventListener(this.name, this, r), o && this.element.addEventListener(this.name, this, t), this._$AH = t
                                 }
                             }
                         }, {
                             key: "handleEvent",
                             value: function(t) {
                                 var e, r;
@@ -8655,18 +8743,18 @@
                     })
                 }
             },
             68144: function(t, e, r) {
                 "use strict";
                 r.d(e, {
                     oi: function() {
-                        return M
+                        return B
                     },
                     fl: function() {
-                        return R
+                        return C
                     },
                     iv: function() {
                         return w
                     },
                     dy: function() {
                         return L.dy
                     },
@@ -8795,15 +8883,15 @@
                         attribute: !0,
                         type: String,
                         converter: A,
                         reflect: !1,
                         hasChanged: T
                     },
                     P = "finalized",
-                    R = function(t) {
+                    C = function(t) {
                         (0, f.Z)(n, t);
                         var e, r = (0, h.Z)(n);
 
                         function n() {
                             var t;
                             return (0, u.Z)(this, n), (t = r.call(this))._$Ei = new Map, t.isUpdatePending = !1, t.hasUpdated = !1, t._$El = null, t._$Eu(), t
                         }
@@ -9103,70 +9191,70 @@
                             key: "_$Ep",
                             value: function(t, e) {
                                 var r = e.attribute;
                                 return !1 === r ? void 0 : "string" == typeof r ? r : "string" == typeof t ? t.toLowerCase() : void 0
                             }
                         }]), n
                     }((0, d.Z)(HTMLElement));
-                R[P] = !0, R.elementProperties = new Map, R.elementStyles = [], R.shadowRootOptions = {
+                C[P] = !0, C.elementProperties = new Map, C.elementStyles = [], C.shadowRootOptions = {
                     mode: "open"
                 }, null == k || k({
-                    ReactiveElement: R
+                    ReactiveElement: C
                 }), (null !== (n = x.reactiveElementVersions) && void 0 !== n ? n : x.reactiveElementVersions = []).push("1.6.3");
-                var C, I, L = r(15304),
+                var R, I, L = r(15304),
                     N = r(82390),
                     H = r(34541),
-                    B = r(47838),
-                    M = (r(89802), function(t) {
+                    M = r(47838),
+                    B = (r(89802), function(t) {
                         (0, f.Z)(r, t);
                         var e = (0, h.Z)(r);
 
                         function r() {
                             var t;
                             return (0, u.Z)(this, r), (t = e.apply(this, arguments)).renderOptions = {
                                 host: (0, N.Z)(t)
                             }, t._$Do = void 0, t
                         }
                         return (0, l.Z)(r, [{
                             key: "createRenderRoot",
                             value: function() {
-                                var t, e, n = (0, H.Z)((0, B.Z)(r.prototype), "createRenderRoot", this).call(this);
+                                var t, e, n = (0, H.Z)((0, M.Z)(r.prototype), "createRenderRoot", this).call(this);
                                 return null !== (t = (e = this.renderOptions).renderBefore) && void 0 !== t || (e.renderBefore = n.firstChild), n
                             }
                         }, {
                             key: "update",
                             value: function(t) {
                                 var e = this.render();
-                                this.hasUpdated || (this.renderOptions.isConnected = this.isConnected), (0, H.Z)((0, B.Z)(r.prototype), "update", this).call(this, t), this._$Do = (0, L.sY)(e, this.renderRoot, this.renderOptions)
+                                this.hasUpdated || (this.renderOptions.isConnected = this.isConnected), (0, H.Z)((0, M.Z)(r.prototype), "update", this).call(this, t), this._$Do = (0, L.sY)(e, this.renderRoot, this.renderOptions)
                             }
                         }, {
                             key: "connectedCallback",
                             value: function() {
                                 var t;
-                                (0, H.Z)((0, B.Z)(r.prototype), "connectedCallback", this).call(this), null === (t = this._$Do) || void 0 === t || t.setConnected(!0)
+                                (0, H.Z)((0, M.Z)(r.prototype), "connectedCallback", this).call(this), null === (t = this._$Do) || void 0 === t || t.setConnected(!0)
                             }
                         }, {
                             key: "disconnectedCallback",
                             value: function() {
                                 var t;
-                                (0, H.Z)((0, B.Z)(r.prototype), "disconnectedCallback", this).call(this), null === (t = this._$Do) || void 0 === t || t.setConnected(!1)
+                                (0, H.Z)((0, M.Z)(r.prototype), "disconnectedCallback", this).call(this), null === (t = this._$Do) || void 0 === t || t.setConnected(!1)
                             }
                         }, {
                             key: "render",
                             value: function() {
                                 return L.Jb
                             }
                         }]), r
-                    }(R));
-                M.finalized = !0, M._$litElement$ = !0, null === (C = globalThis.litElementHydrateSupport) || void 0 === C || C.call(globalThis, {
-                    LitElement: M
+                    }(C));
+                B.finalized = !0, B._$litElement$ = !0, null === (R = globalThis.litElementHydrateSupport) || void 0 === R || R.call(globalThis, {
+                    LitElement: B
                 });
                 var j = globalThis.litElementPolyfillSupport;
                 null == j || j({
-                    LitElement: M
+                    LitElement: B
                 });
                 (null !== (I = globalThis.litElementVersions) && void 0 !== I ? I : globalThis.litElementVersions = []).push("3.3.3")
             },
             43204: function(t, e, r) {
                 "use strict";
                 r.d(e, {
                     XA: function() {
@@ -9312,34 +9400,34 @@
             return Promise.all(Object.keys(a.f).reduce((function(e, r) {
                 return a.f[r](t, e), e
             }), []))
         }, a.u = function(t) {
             return {
                 210: "xK5ZNMm1",
                 226: "PJOjJOeb",
-                244: "riIkKI3D",
+                244: "m_bQlMKv",
                 338: "VCTfVQ_Y",
-                394: "RlIVWY_9",
+                394: "J71QpLgx",
                 430: "RaxGx9Oy",
                 442: "DVZuMQTQ",
                 456: "gWLSf6Uq",
-                527: "-Bo5aSaU",
-                540: "NATIZehR",
+                527: "79rx9Er-",
                 587: "RIGgWZMd",
                 597: "NmyD-jM4",
                 679: "6vdISARd",
                 689: "Niahov52",
                 719: "52ZGgRTb",
+                770: "1JtEbuPe",
                 776: "f67fx1_K",
                 812: "VYXPimMw",
                 879: "9niMDe6j",
                 886: "ye57YhXr",
                 925: "ZshdvKRY",
                 942: "8uDhd8eQ",
-                981: "nqy1LXz0"
+                981: "mNa8_BnN"
             } [t] + ".js"
         }, a.o = function(t, e) {
             return Object.prototype.hasOwnProperty.call(t, e)
         }, r = {}, n = "lcn-frontend:", a.l = function(t, e, o, i) {
             if (r[t]) r[t].push(e);
             else {
                 var s, c;
@@ -9824,22 +9912,22 @@
             if (/^((?!chrome|android).)*version\/14\.0\s.*safari/i.test(navigator.userAgent)) {
                 var O = window.Element.prototype.attachShadow;
                 window.Element.prototype.attachShadow = function(t) {
                     return t && t.delegatesFocus && delete t.delegatesFocus, O.apply(this, [t])
                 }
             }
             var P = a(33368),
-                R = a(71650),
-                C = a(82390),
+                C = a(71650),
+                R = a(82390),
                 I = a(69205),
                 L = a(70906),
                 N = a(51565),
                 H = a(34541),
-                B = a(47838),
-                M = (a(97393), a(85472), a(90126), a(85717), a(73175));
+                M = a(47838),
+                B = (a(97393), a(85472), a(90126), a(85717), a(73175));
             a(94738);
 
             function j(t, e) {
                 if (null == t) return {};
                 var r, n, o = function(t, e) {
                     if (null == t) return {};
                     var r, n, o = {},
@@ -10154,37 +10242,37 @@
                     var e = (0, Z.Z)(t, 2),
                         r = e[0],
                         n = e[1];
                     return "--".concat(r, ": ").concat(n, ";")
                 })).join(""))).toString()),
                 pt = document.createElement("style");
             pt.textContent = [dt, T].join(""), document.head.append(pt);
-            a(46097), a(37313), a(47084);
+            a(46097), a(37313);
             var vt, gt = a(99312),
                 yt = a(81043),
-                mt = a(76775),
+                mt = (a(47084), a(76775)),
                 bt = (a(35221), a(10733), a(14516)),
                 wt = (0, N.Z)(null, (function(t, e) {
                     var r, n = function(e) {
                         (0, I.Z)(n, e);
                         var r = (0, L.Z)(n);
 
                         function n() {
                             var e;
-                            (0, R.Z)(this, n);
+                            (0, C.Z)(this, n);
                             for (var o = arguments.length, i = new Array(o), a = 0; a < o; a++) i[a] = arguments[a];
-                            return e = r.call.apply(r, [this].concat(i)), t((0, C.Z)(e)), e
+                            return e = r.call.apply(r, [this].concat(i)), t((0, R.Z)(e)), e
                         }
                         return (0, P.Z)(n)
                     }(e);
                     return {
                         F: n,
                         d: [{
                             kind: "field",
-                            decorators: [(0, M.Cb)()],
+                            decorators: [(0, B.Cb)()],
                             key: "route",
                             value: void 0
                         }, {
                             kind: "field",
                             key: "routerOptions",
                             value: void 0
                         }, {
@@ -10231,15 +10319,15 @@
                                 return this
                             }
                         }, {
                             kind: "method",
                             key: "update",
                             value: function(t) {
                                 var e = this;
-                                (0, H.Z)((0, B.Z)(n.prototype), "update", this).call(this, t);
+                                (0, H.Z)((0, M.Z)(n.prototype), "update", this).call(this, t);
                                 var r = this.routerOptions || {
                                     routes: {}
                                 };
                                 if (!r || !r.initialLoad || this._initialLoadDone)
                                     if (t.has("route")) {
                                         var o = this.route,
                                             i = r.defaultPage;
@@ -10282,15 +10370,15 @@
                                     } else this.lastChild && !this._currentLoadProm && this.updatePageEl(this.lastChild, t)
                             }
                         }, {
                             kind: "method",
                             key: "firstUpdated",
                             value: function(t) {
                                 var e = this;
-                                (0, H.Z)((0, B.Z)(n.prototype), "firstUpdated", this).call(this, t);
+                                (0, H.Z)((0, M.Z)(n.prototype), "firstUpdated", this).call(this, t);
                                 var r = this.routerOptions;
                                 r && (r.preloadAll && Object.values(r.routes).forEach((function(t) {
                                     return "object" === (0, mt.Z)(t) && t.load && t.load()
                                 })), r.initialLoad && (setTimeout((function() {
                                     e._initialLoadDone || e.appendChild(e.createLoadingScreen())
                                 }), 400), r.initialLoad().then((function() {
                                     e._initialLoadDone = !0, e.requestUpdate("route")
@@ -10367,149 +10455,214 @@
                                 this.lastChild && this.removeChild(this.lastChild);
                                 var n = this._cache[e] || this.createElement(r.tag);
                                 this.updatePageEl(n), this.appendChild(n), (t.cacheAll || r.cache) && (this._cache[e] = n)
                             }
                         }]
                     }
                 }), A.fl),
-                Et = ((0, N.Z)([(0, M.Mo)("lcn-router")], (function(t, e) {
-                    var r = function(e) {
+                Et = function() {
+                    function t(e) {
+                        (0, C.Z)(this, t), this.prefix = void 0, this.prefix = e ? "[lcn.".concat(e, "]") : "[lcn]"
+                    }
+                    return (0, P.Z)(t, [{
+                        key: "info",
+                        value: function() {
+                            for (var t, e = arguments.length, r = new Array(e), n = 0; n < e; n++) r[n] = arguments[n];
+                            (t = console).info.apply(t, [this.prefix].concat(r))
+                        }
+                    }, {
+                        key: "log",
+                        value: function() {
+                            for (var t, e = arguments.length, r = new Array(e), n = 0; n < e; n++) r[n] = arguments[n];
+                            (t = console).log.apply(t, [this.prefix].concat(r))
+                        }
+                    }, {
+                        key: "debug",
+                        value: function() {
+                            for (var t, e = arguments.length, r = new Array(e), n = 0; n < e; n++) r[n] = arguments[n];
+                            (t = console).debug.apply(t, [this.prefix].concat(r))
+                        }
+                    }, {
+                        key: "warn",
+                        value: function() {
+                            for (var t, e = arguments.length, r = new Array(e), n = 0; n < e; n++) r[n] = arguments[n];
+                            (t = console).warn.apply(t, [this.prefix].concat(r))
+                        }
+                    }, {
+                        key: "error",
+                        value: function() {
+                            for (var t, e = arguments.length, r = new Array(e), n = 0; n < e; n++) r[n] = arguments[n];
+                            (t = console).error.apply(t, [this.prefix].concat(r))
+                        }
+                    }]), t
+                }(),
+                xt = a(9051),
+                _t = new Et("router"),
+                St = ((0, N.Z)([(0, B.Mo)("lcn-router")], (function(t, e) {
+                    var r, n = function(e) {
                         (0, I.Z)(n, e);
                         var r = (0, L.Z)(n);
 
                         function n() {
                             var e;
-                            (0, R.Z)(this, n);
+                            (0, C.Z)(this, n);
                             for (var o = arguments.length, i = new Array(o), a = 0; a < o; a++) i[a] = arguments[a];
-                            return e = r.call.apply(r, [this].concat(i)), t((0, C.Z)(e)), e
+                            return e = r.call.apply(r, [this].concat(i)), t((0, R.Z)(e)), e
                         }
                         return (0, P.Z)(n)
                     }(e);
                     return {
-                        F: r,
+                        F: n,
                         d: [{
                             kind: "field",
-                            decorators: [(0, M.Cb)({
+                            decorators: [(0, B.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, M.Cb)({
+                            decorators: [(0, B.Cb)({
                                 attribute: !1
                             })],
                             key: "lcn",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, M.Cb)({
+                            decorators: [(0, B.Cb)({
                                 attribute: !1
                             })],
                             key: "route",
                             value: void 0
                         }, {
                             kind: "field",
-                            decorators: [(0, M.Cb)({
-                                attribute: !1
+                            decorators: [(0, B.Cb)({
+                                type: Boolean
                             })],
                             key: "narrow",
                             value: void 0
                         }, {
                             kind: "field",
+                            decorators: [(0, B.SB)()],
+                            key: "hosts",
+                            value: void 0
+                        }, {
+                            kind: "field",
                             key: "routerOptions",
                             value: function() {
+                                var t = this;
                                 return {
                                     defaultPage: "devices",
                                     showLoading: !0,
                                     routes: {
                                         devices: {
                                             tag: "lcn-config-dashboard",
                                             load: function() {
-                                                return console.log("Importing lcn-config-dashboard"), Promise.all([a.e(210), a.e(689), a.e(587), a.e(430), a.e(776), a.e(540), a.e(925), a.e(394)]).then(a.bind(a, 73394))
+                                                return _t.debug("Importing lcn-config-dashboard"), Promise.all([a.e(210), a.e(689), a.e(587), a.e(430), a.e(776), a.e(770), a.e(925), a.e(394)]).then(a.bind(a, 73394))
                                             }
                                         },
                                         entities: {
                                             tag: "lcn-entities-page",
                                             load: function() {
-                                                return console.log("Importing lcn-entities-page"), Promise.all([a.e(210), a.e(430), a.e(776), a.e(540), a.e(981)]).then(a.bind(a, 70981))
+                                                return _t.debug("Importing lcn-entities-page"), Promise.all([a.e(210), a.e(430), a.e(776), a.e(770), a.e(981)]).then(a.bind(a, 70981))
                                             }
                                         }
+                                    },
+                                    initialLoad: function() {
+                                        return t._fetchHosts()
                                     }
                                 }
                             }
                         }, {
                             kind: "method",
                             key: "updatePageEl",
                             value: function(t) {
-                                t.hass = this.hass, t.lcn = this.lcn, t.route = this.routeTail, t.narrow = this.narrow, console.log("Current Page: ".concat(this._currentPage, " Route: ").concat(this.route.path))
+                                t.hass = this.hass, t.lcn = this.lcn, t.route = this.routeTail, t.narrow = this.narrow, "devices" === this._currentPage && (t.hosts = this.hosts), _t.debug("Current Page: ".concat(this._currentPage, " Route: ").concat(this.route.path))
                             }
+                        }, {
+                            kind: "method",
+                            key: "_fetchHosts",
+                            value: (r = (0, yt.Z)((0, gt.Z)().mark((function t() {
+                                return (0, gt.Z)().wrap((function(t) {
+                                    for (;;) switch (t.prev = t.next) {
+                                        case 0:
+                                            return t.next = 2, (0, xt.V5)(this.hass);
+                                        case 2:
+                                            this.hosts = t.sent;
+                                        case 3:
+                                        case "end":
+                                            return t.stop()
+                                    }
+                                }), t, this)
+                            }))), function() {
+                                return r.apply(this, arguments)
+                            })
                         }]
                     }
                 }), wt), a(40271), a(60163), a(43204));
             ! function(t) {
                 t[t.EXPECT_ARGUMENT_CLOSING_BRACE = 1] = "EXPECT_ARGUMENT_CLOSING_BRACE", t[t.EMPTY_ARGUMENT = 2] = "EMPTY_ARGUMENT", t[t.MALFORMED_ARGUMENT = 3] = "MALFORMED_ARGUMENT", t[t.EXPECT_ARGUMENT_TYPE = 4] = "EXPECT_ARGUMENT_TYPE", t[t.INVALID_ARGUMENT_TYPE = 5] = "INVALID_ARGUMENT_TYPE", t[t.EXPECT_ARGUMENT_STYLE = 6] = "EXPECT_ARGUMENT_STYLE", t[t.INVALID_NUMBER_SKELETON = 7] = "INVALID_NUMBER_SKELETON", t[t.INVALID_DATE_TIME_SKELETON = 8] = "INVALID_DATE_TIME_SKELETON", t[t.EXPECT_NUMBER_SKELETON = 9] = "EXPECT_NUMBER_SKELETON", t[t.EXPECT_DATE_TIME_SKELETON = 10] = "EXPECT_DATE_TIME_SKELETON", t[t.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE = 11] = "UNCLOSED_QUOTE_IN_ARGUMENT_STYLE", t[t.EXPECT_SELECT_ARGUMENT_OPTIONS = 12] = "EXPECT_SELECT_ARGUMENT_OPTIONS", t[t.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE = 13] = "EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE", t[t.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE = 14] = "INVALID_PLURAL_ARGUMENT_OFFSET_VALUE", t[t.EXPECT_SELECT_ARGUMENT_SELECTOR = 15] = "EXPECT_SELECT_ARGUMENT_SELECTOR", t[t.EXPECT_PLURAL_ARGUMENT_SELECTOR = 16] = "EXPECT_PLURAL_ARGUMENT_SELECTOR", t[t.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT = 17] = "EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT", t[t.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT = 18] = "EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT", t[t.INVALID_PLURAL_ARGUMENT_SELECTOR = 19] = "INVALID_PLURAL_ARGUMENT_SELECTOR", t[t.DUPLICATE_PLURAL_ARGUMENT_SELECTOR = 20] = "DUPLICATE_PLURAL_ARGUMENT_SELECTOR", t[t.DUPLICATE_SELECT_ARGUMENT_SELECTOR = 21] = "DUPLICATE_SELECT_ARGUMENT_SELECTOR", t[t.MISSING_OTHER_CLAUSE = 22] = "MISSING_OTHER_CLAUSE", t[t.INVALID_TAG = 23] = "INVALID_TAG", t[t.INVALID_TAG_NAME = 25] = "INVALID_TAG_NAME", t[t.UNMATCHED_CLOSING_TAG = 26] = "UNMATCHED_CLOSING_TAG", t[t.UNCLOSED_TAG = 27] = "UNCLOSED_TAG"
             }(vt || (vt = {}));
-            var xt, _t;
+            var kt, At;
             a(10999), a(52117), a(82479), a(40924), a(90465), a(4600), a(10187), a(62544), a(60309);
 
-            function St(t) {
-                return t.type === xt.literal
-            }
-
-            function kt(t) {
-                return t.type === xt.argument
-            }
-
-            function At(t) {
-                return t.type === xt.number
-            }
-
             function Tt(t) {
-                return t.type === xt.date
+                return t.type === kt.literal
             }
 
             function Ot(t) {
-                return t.type === xt.time
+                return t.type === kt.argument
             }
 
             function Pt(t) {
-                return t.type === xt.select
+                return t.type === kt.number
             }
 
-            function Rt(t) {
-                return t.type === xt.plural
+            function Ct(t) {
+                return t.type === kt.date
             }
 
-            function Ct(t) {
-                return t.type === xt.pound
+            function Rt(t) {
+                return t.type === kt.time
             }
 
             function It(t) {
-                return t.type === xt.tag
+                return t.type === kt.select
             }
 
             function Lt(t) {
-                return !(!t || "object" !== (0, mt.Z)(t) || t.type !== _t.number)
+                return t.type === kt.plural
             }
 
             function Nt(t) {
-                return !(!t || "object" !== (0, mt.Z)(t) || t.type !== _t.dateTime)
+                return t.type === kt.pound
+            }
+
+            function Ht(t) {
+                return t.type === kt.tag
+            }
+
+            function Mt(t) {
+                return !(!t || "object" !== (0, mt.Z)(t) || t.type !== At.number)
+            }
+
+            function Bt(t) {
+                return !(!t || "object" !== (0, mt.Z)(t) || t.type !== At.dateTime)
             }! function(t) {
                 t[t.literal = 0] = "literal", t[t.argument = 1] = "argument", t[t.number = 2] = "number", t[t.date = 3] = "date", t[t.time = 4] = "time", t[t.select = 5] = "select", t[t.plural = 6] = "plural", t[t.pound = 7] = "pound", t[t.tag = 8] = "tag"
-            }(xt || (xt = {})),
+            }(kt || (kt = {})),
             function(t) {
                 t[t.number = 0] = "number", t[t.dateTime = 1] = "dateTime"
-            }(_t || (_t = {}));
-            var Ht = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
-                Bt = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
+            }(At || (At = {}));
+            var jt = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
+                Dt = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
 
-            function Mt(t) {
+            function $t(t) {
                 var e = {};
-                return t.replace(Bt, (function(t) {
+                return t.replace(Dt, (function(t) {
                     var r = t.length;
                     switch (t[0]) {
                         case "G":
                             e.era = 4 === r ? "long" : 5 === r ? "narrow" : "short";
                             break;
                         case "y":
                             e.year = 2 === r ? "2-digit" : "numeric";
@@ -10589,28 +10742,28 @@
                         case "x":
                             throw new RangeError("`Z/O/v/V/X/x` (timeZone) patterns are not supported, use `z` instead")
                     }
                     return ""
                 })), e
             }
             a(57778);
-            var jt = /[\t-\r \x85\u200E\u200F\u2028\u2029]/i;
-            var Dt = /^\.(?:(0+)(\*)?|(#+)|(0+)(#+))$/g,
-                $t = /^(@+)?(\+|#+)?[rs]?$/g,
-                Ut = /(\*)(0+)|(#+)(0+)|(0+)/g,
-                Zt = /^(0+)$/;
+            var Ut = /[\t-\r \x85\u200E\u200F\u2028\u2029]/i;
+            var Zt = /^\.(?:(0+)(\*)?|(#+)|(0+)(#+))$/g,
+                Ft = /^(@+)?(\+|#+)?[rs]?$/g,
+                Gt = /(\*)(0+)|(#+)(0+)|(0+)/g,
+                zt = /^(0+)$/;
 
-            function Ft(t) {
+            function Vt(t) {
                 var e = {};
-                return "r" === t[t.length - 1] ? e.roundingPriority = "morePrecision" : "s" === t[t.length - 1] && (e.roundingPriority = "lessPrecision"), t.replace($t, (function(t, r, n) {
+                return "r" === t[t.length - 1] ? e.roundingPriority = "morePrecision" : "s" === t[t.length - 1] && (e.roundingPriority = "lessPrecision"), t.replace(Ft, (function(t, r, n) {
                     return "string" != typeof n ? (e.minimumSignificantDigits = r.length, e.maximumSignificantDigits = r.length) : "+" === n ? e.minimumSignificantDigits = r.length : "#" === r[0] ? e.maximumSignificantDigits = r.length : (e.minimumSignificantDigits = r.length, e.maximumSignificantDigits = r.length + ("string" == typeof n ? n.length : 0)), ""
                 })), e
             }
 
-            function Gt(t) {
+            function Wt(t) {
                 switch (t) {
                     case "sign-auto":
                         return {
                             signDisplay: "auto"
                         };
                     case "sign-accounting":
                     case "()":
@@ -10641,34 +10794,34 @@
                     case "+_":
                         return {
                             signDisplay: "never"
                         }
                 }
             }
 
-            function zt(t) {
+            function Kt(t) {
                 var e;
                 if ("E" === t[0] && "E" === t[1] ? (e = {
                         notation: "engineering"
                     }, t = t.slice(2)) : "E" === t[0] && (e = {
                         notation: "scientific"
                     }, t = t.slice(1)), e) {
                     var r = t.slice(0, 2);
-                    if ("+!" === r ? (e.signDisplay = "always", t = t.slice(2)) : "+?" === r && (e.signDisplay = "exceptZero", t = t.slice(2)), !Zt.test(t)) throw new Error("Malformed concise eng/scientific notation");
+                    if ("+!" === r ? (e.signDisplay = "always", t = t.slice(2)) : "+?" === r && (e.signDisplay = "exceptZero", t = t.slice(2)), !zt.test(t)) throw new Error("Malformed concise eng/scientific notation");
                     e.minimumIntegerDigits = t.length
                 }
                 return e
             }
 
-            function Vt(t) {
-                var e = Gt(t);
+            function Xt(t) {
+                var e = Wt(t);
                 return e || {}
             }
 
-            function Wt(t) {
+            function Yt(t) {
                 for (var e = {}, r = 0, n = t; r < n.length; r++) {
                     var o = n[r];
                     switch (o.stem) {
                         case "percent":
                         case "%":
                             e.style = "percent";
                             continue;
@@ -10695,25 +10848,25 @@
                             e.notation = "compact", e.compactDisplay = "short";
                             continue;
                         case "compact-long":
                         case "KK":
                             e.notation = "compact", e.compactDisplay = "long";
                             continue;
                         case "scientific":
-                            e = (0, Et.pi)((0, Et.pi)((0, Et.pi)({}, e), {
+                            e = (0, St.pi)((0, St.pi)((0, St.pi)({}, e), {
                                 notation: "scientific"
                             }), o.options.reduce((function(t, e) {
-                                return (0, Et.pi)((0, Et.pi)({}, t), Vt(e))
+                                return (0, St.pi)((0, St.pi)({}, t), Xt(e))
                             }), {}));
                             continue;
                         case "engineering":
-                            e = (0, Et.pi)((0, Et.pi)((0, Et.pi)({}, e), {
+                            e = (0, St.pi)((0, St.pi)((0, St.pi)({}, e), {
                                 notation: "engineering"
                             }), o.options.reduce((function(t, e) {
-                                return (0, Et.pi)((0, Et.pi)({}, t), Vt(e))
+                                return (0, St.pi)((0, St.pi)({}, t), Xt(e))
                             }), {}));
                             continue;
                         case "notation-simple":
                             e.notation = "standard";
                             continue;
                         case "unit-width-narrow":
                             e.currencyDisplay = "narrowSymbol", e.unitDisplay = "narrow";
@@ -10728,45 +10881,45 @@
                             e.currencyDisplay = "symbol";
                             continue;
                         case "scale":
                             e.scale = parseFloat(o.options[0]);
                             continue;
                         case "integer-width":
                             if (o.options.length > 1) throw new RangeError("integer-width stems only accept a single optional option");
-                            o.options[0].replace(Ut, (function(t, r, n, o, i, a) {
+                            o.options[0].replace(Gt, (function(t, r, n, o, i, a) {
                                 if (r) e.minimumIntegerDigits = n.length;
                                 else {
                                     if (o && i) throw new Error("We currently do not support maximum integer digits");
                                     if (a) throw new Error("We currently do not support exact integer digits")
                                 }
                                 return ""
                             }));
                             continue
                     }
-                    if (Zt.test(o.stem)) e.minimumIntegerDigits = o.stem.length;
-                    else if (Dt.test(o.stem)) {
+                    if (zt.test(o.stem)) e.minimumIntegerDigits = o.stem.length;
+                    else if (Zt.test(o.stem)) {
                         if (o.options.length > 1) throw new RangeError("Fraction-precision stems only accept a single optional option");
-                        o.stem.replace(Dt, (function(t, r, n, o, i, a) {
+                        o.stem.replace(Zt, (function(t, r, n, o, i, a) {
                             return "*" === n ? e.minimumFractionDigits = r.length : o && "#" === o[0] ? e.maximumFractionDigits = o.length : i && a ? (e.minimumFractionDigits = i.length, e.maximumFractionDigits = i.length + a.length) : (e.minimumFractionDigits = r.length, e.maximumFractionDigits = r.length), ""
                         }));
                         var i = o.options[0];
-                        "w" === i ? e = (0, Et.pi)((0, Et.pi)({}, e), {
+                        "w" === i ? e = (0, St.pi)((0, St.pi)({}, e), {
                             trailingZeroDisplay: "stripIfInteger"
-                        }) : i && (e = (0, Et.pi)((0, Et.pi)({}, e), Ft(i)))
-                    } else if ($t.test(o.stem)) e = (0, Et.pi)((0, Et.pi)({}, e), Ft(o.stem));
+                        }) : i && (e = (0, St.pi)((0, St.pi)({}, e), Vt(i)))
+                    } else if (Ft.test(o.stem)) e = (0, St.pi)((0, St.pi)({}, e), Vt(o.stem));
                     else {
-                        var a = Gt(o.stem);
-                        a && (e = (0, Et.pi)((0, Et.pi)({}, e), a));
-                        var s = zt(o.stem);
-                        s && (e = (0, Et.pi)((0, Et.pi)({}, e), s))
+                        var a = Wt(o.stem);
+                        a && (e = (0, St.pi)((0, St.pi)({}, e), a));
+                        var s = Kt(o.stem);
+                        s && (e = (0, St.pi)((0, St.pi)({}, e), s))
                     }
                 }
                 return e
             }
-            var Kt, Xt = {
+            var qt, Jt = {
                 "001": ["H", "h"],
                 AC: ["H", "h", "hb", "hB"],
                 AD: ["H", "hB"],
                 AE: ["h", "hB", "hb", "H"],
                 AF: ["H", "hb", "hB", "h"],
                 AG: ["h", "hb", "H", "hB"],
                 AI: ["H", "h", "hb", "hB"],
@@ -11034,115 +11187,115 @@
                 "mr-IN": ["hB", "hb", "h", "H"],
                 "pa-IN": ["hB", "hb", "h", "H"],
                 "ta-IN": ["hB", "h", "hb", "H"],
                 "te-IN": ["hB", "h", "H"],
                 "zu-ZA": ["H", "hB", "hb", "h"]
             };
 
-            function Yt(t) {
+            function Qt(t) {
                 var e = t.hourCycle;
                 if (void 0 === e && t.hourCycles && t.hourCycles.length && (e = t.hourCycles[0]), e) switch (e) {
                     case "h24":
                         return "k";
                     case "h23":
                         return "H";
                     case "h12":
                         return "h";
                     case "h11":
                         return "K";
                     default:
                         throw new Error("Invalid hourCycle")
                 }
                 var r, n = t.language;
-                return "root" !== n && (r = t.maximize().region), (Xt[r || ""] || Xt[n || ""] || Xt["".concat(n, "-001")] || Xt["001"])[0]
+                return "root" !== n && (r = t.maximize().region), (Jt[r || ""] || Jt[n || ""] || Jt["".concat(n, "-001")] || Jt["001"])[0]
             }
-            var qt = new RegExp("^".concat(Ht.source, "*")),
-                Jt = new RegExp("".concat(Ht.source, "*$"));
+            var te = new RegExp("^".concat(jt.source, "*")),
+                ee = new RegExp("".concat(jt.source, "*$"));
 
-            function Qt(t, e) {
+            function re(t, e) {
                 return {
                     start: t,
                     end: e
                 }
             }
-            var te = !!String.prototype.startsWith && "_a".startsWith("a", 1),
-                ee = !!String.fromCodePoint,
-                re = !!Object.fromEntries,
-                ne = !!String.prototype.codePointAt,
-                oe = !!String.prototype.trimStart,
-                ie = !!String.prototype.trimEnd,
-                ae = !!Number.isSafeInteger ? Number.isSafeInteger : function(t) {
+            var ne = !!String.prototype.startsWith && "_a".startsWith("a", 1),
+                oe = !!String.fromCodePoint,
+                ie = !!Object.fromEntries,
+                ae = !!String.prototype.codePointAt,
+                se = !!String.prototype.trimStart,
+                ce = !!String.prototype.trimEnd,
+                ue = !!Number.isSafeInteger ? Number.isSafeInteger : function(t) {
                     return "number" == typeof t && isFinite(t) && Math.floor(t) === t && Math.abs(t) <= 9007199254740991
                 },
-                se = !0;
+                le = !0;
             try {
-                se = "a" === (null === (Kt = ve("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu").exec("a")) || void 0 === Kt ? void 0 : Kt[0])
-            } catch (Qe) {
-                se = !1
+                le = "a" === (null === (qt = me("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu").exec("a")) || void 0 === qt ? void 0 : qt[0])
+            } catch (nr) {
+                le = !1
             }
-            var ce, ue = te ? function(t, e, r) {
+            var fe, he = ne ? function(t, e, r) {
                     return t.startsWith(e, r)
                 } : function(t, e, r) {
                     return t.slice(r, r + e.length) === e
                 },
-                le = ee ? String.fromCodePoint : function() {
+                de = oe ? String.fromCodePoint : function() {
                     for (var t = [], e = 0; e < arguments.length; e++) t[e] = arguments[e];
                     for (var r, n = "", o = t.length, i = 0; o > i;) {
                         if ((r = t[i++]) > 1114111) throw RangeError(r + " is not a valid code point");
                         n += r < 65536 ? String.fromCharCode(r) : String.fromCharCode(55296 + ((r -= 65536) >> 10), r % 1024 + 56320)
                     }
                     return n
                 },
-                fe = re ? Object.fromEntries : function(t) {
+                pe = ie ? Object.fromEntries : function(t) {
                     for (var e = {}, r = 0, n = t; r < n.length; r++) {
                         var o = n[r],
                             i = o[0],
                             a = o[1];
                         e[i] = a
                     }
                     return e
                 },
-                he = ne ? function(t, e) {
+                ve = ae ? function(t, e) {
                     return t.codePointAt(e)
                 } : function(t, e) {
                     var r = t.length;
                     if (!(e < 0 || e >= r)) {
                         var n, o = t.charCodeAt(e);
                         return o < 55296 || o > 56319 || e + 1 === r || (n = t.charCodeAt(e + 1)) < 56320 || n > 57343 ? o : n - 56320 + (o - 55296 << 10) + 65536
                     }
                 },
-                de = oe ? function(t) {
+                ge = se ? function(t) {
                     return t.trimStart()
                 } : function(t) {
-                    return t.replace(qt, "")
+                    return t.replace(te, "")
                 },
-                pe = ie ? function(t) {
+                ye = ce ? function(t) {
                     return t.trimEnd()
                 } : function(t) {
-                    return t.replace(Jt, "")
+                    return t.replace(ee, "")
                 };
 
-            function ve(t, e) {
+            function me(t, e) {
                 return new RegExp(t, e)
             }
-            if (se) {
-                var ge = ve("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
-                ce = function(t, e) {
+            if (le) {
+                var be = me("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
+                fe = function(t, e) {
                     var r;
-                    return ge.lastIndex = e, null !== (r = ge.exec(t)[1]) && void 0 !== r ? r : ""
+                    return be.lastIndex = e, null !== (r = be.exec(t)[1]) && void 0 !== r ? r : ""
                 }
-            } else ce = function(t, e) {
+            } else fe = function(t, e) {
                 for (var r = [];;) {
-                    var n = he(t, e);
-                    if (void 0 === n || be(n) || we(n)) break;
+                    var n = ve(t, e);
+                    if (void 0 === n || xe(n) || _e(n)) break;
                     r.push(n), e += n >= 65536 ? 2 : 1
                 }
-                return le.apply(void 0, r)
+                return de.apply(void 0, r)
             };
-            var ye = function() {
+            var we = function() {
                 function t(t, e) {
                     void 0 === e && (e = {}), this.message = t, this.position = {
                         offset: 0,
                         line: 1,
                         column: 1
                     }, this.ignoreTag = !!e.ignoreTag, this.locale = e.locale, this.requiresOtherClause = !!e.requiresOtherClause, this.shouldParseSkeletons = !!e.shouldParseSkeletons
                 }
@@ -11156,70 +11309,70 @@
                             if ((i = this.parseArgument(t, r)).err) return i;
                             n.push(i.val)
                         } else {
                             if (125 === o && t > 0) break;
                             if (35 !== o || "plural" !== e && "selectordinal" !== e) {
                                 if (60 === o && !this.ignoreTag && 47 === this.peek()) {
                                     if (r) break;
-                                    return this.error(vt.UNMATCHED_CLOSING_TAG, Qt(this.clonePosition(), this.clonePosition()))
+                                    return this.error(vt.UNMATCHED_CLOSING_TAG, re(this.clonePosition(), this.clonePosition()))
                                 }
-                                if (60 === o && !this.ignoreTag && me(this.peek() || 0)) {
+                                if (60 === o && !this.ignoreTag && Ee(this.peek() || 0)) {
                                     if ((i = this.parseTag(t, e)).err) return i;
                                     n.push(i.val)
                                 } else {
                                     var i;
                                     if ((i = this.parseLiteral(t, e)).err) return i;
                                     n.push(i.val)
                                 }
                             } else {
                                 var a = this.clonePosition();
                                 this.bump(), n.push({
-                                    type: xt.pound,
-                                    location: Qt(a, this.clonePosition())
+                                    type: kt.pound,
+                                    location: re(a, this.clonePosition())
                                 })
                             }
                         }
                     }
                     return {
                         val: n,
                         err: null
                     }
                 }, t.prototype.parseTag = function(t, e) {
                     var r = this.clonePosition();
                     this.bump();
                     var n = this.parseTagName();
                     if (this.bumpSpace(), this.bumpIf("/>")) return {
                         val: {
-                            type: xt.literal,
+                            type: kt.literal,
                             value: "<".concat(n, "/>"),
-                            location: Qt(r, this.clonePosition())
+                            location: re(r, this.clonePosition())
                         },
                         err: null
                     };
                     if (this.bumpIf(">")) {
                         var o = this.parseMessage(t + 1, e, !0);
                         if (o.err) return o;
                         var i = o.val,
                             a = this.clonePosition();
                         if (this.bumpIf("</")) {
-                            if (this.isEOF() || !me(this.char())) return this.error(vt.INVALID_TAG, Qt(a, this.clonePosition()));
+                            if (this.isEOF() || !Ee(this.char())) return this.error(vt.INVALID_TAG, re(a, this.clonePosition()));
                             var s = this.clonePosition();
-                            return n !== this.parseTagName() ? this.error(vt.UNMATCHED_CLOSING_TAG, Qt(s, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
+                            return n !== this.parseTagName() ? this.error(vt.UNMATCHED_CLOSING_TAG, re(s, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
                                 val: {
-                                    type: xt.tag,
+                                    type: kt.tag,
                                     value: n,
                                     children: i,
-                                    location: Qt(r, this.clonePosition())
+                                    location: re(r, this.clonePosition())
                                 },
                                 err: null
-                            } : this.error(vt.INVALID_TAG, Qt(a, this.clonePosition())))
+                            } : this.error(vt.INVALID_TAG, re(a, this.clonePosition())))
                         }
-                        return this.error(vt.UNCLOSED_TAG, Qt(r, this.clonePosition()))
+                        return this.error(vt.UNCLOSED_TAG, re(r, this.clonePosition()))
                     }
-                    return this.error(vt.INVALID_TAG, Qt(r, this.clonePosition()))
+                    return this.error(vt.INVALID_TAG, re(r, this.clonePosition()))
                 }, t.prototype.parseTagName = function() {
                     var t, e = this.offset();
                     for (this.bump(); !this.isEOF() && (45 === (t = this.char()) || 46 === t || t >= 48 && t <= 57 || 95 === t || t >= 97 && t <= 122 || t >= 65 && t <= 90 || 183 == t || t >= 192 && t <= 214 || t >= 216 && t <= 246 || t >= 248 && t <= 893 || t >= 895 && t <= 8191 || t >= 8204 && t <= 8205 || t >= 8255 && t <= 8256 || t >= 8304 && t <= 8591 || t >= 11264 && t <= 12271 || t >= 12289 && t <= 55295 || t >= 63744 && t <= 64975 || t >= 65008 && t <= 65533 || t >= 65536 && t <= 983039);) this.bump();
                     return this.message.slice(e, this.offset())
                 }, t.prototype.parseLiteral = function(t, e) {
                     for (var r = this.clonePosition(), n = "";;) {
                         var o = this.tryParseQuote(e);
@@ -11230,25 +11383,25 @@
                             else {
                                 var a = this.tryParseLeftAngleBracket();
                                 if (!a) break;
                                 n += a
                             }
                         }
                     }
-                    var s = Qt(r, this.clonePosition());
+                    var s = re(r, this.clonePosition());
                     return {
                         val: {
-                            type: xt.literal,
+                            type: kt.literal,
                             value: n,
                             location: s
                         },
                         err: null
                     }
                 }, t.prototype.tryParseLeftAngleBracket = function() {
-                    return this.isEOF() || 60 !== this.char() || !this.ignoreTag && (me(t = this.peek() || 0) || 47 === t) ? null : (this.bump(), "<");
+                    return this.isEOF() || 60 !== this.char() || !this.ignoreTag && (Ee(t = this.peek() || 0) || 47 === t) ? null : (this.bump(), "<");
                     var t
                 }, t.prototype.tryParseQuote = function(t) {
                     if (this.isEOF() || 39 !== this.char()) return null;
                     switch (this.peek()) {
                         case 39:
                             return this.bump(), this.bump(), "'";
                         case 123:
@@ -11271,79 +11424,79 @@
                                 this.bump();
                                 break
                             }
                             e.push(39), this.bump()
                         } else e.push(r);
                         this.bump()
                     }
-                    return le.apply(void 0, e)
+                    return de.apply(void 0, e)
                 }, t.prototype.tryParseUnquoted = function(t, e) {
                     if (this.isEOF()) return null;
                     var r = this.char();
-                    return 60 === r || 123 === r || 35 === r && ("plural" === e || "selectordinal" === e) || 125 === r && t > 0 ? null : (this.bump(), le(r))
+                    return 60 === r || 123 === r || 35 === r && ("plural" === e || "selectordinal" === e) || 125 === r && t > 0 ? null : (this.bump(), de(r))
                 }, t.prototype.parseArgument = function(t, e) {
                     var r = this.clonePosition();
-                    if (this.bump(), this.bumpSpace(), this.isEOF()) return this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, Qt(r, this.clonePosition()));
-                    if (125 === this.char()) return this.bump(), this.error(vt.EMPTY_ARGUMENT, Qt(r, this.clonePosition()));
+                    if (this.bump(), this.bumpSpace(), this.isEOF()) return this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, re(r, this.clonePosition()));
+                    if (125 === this.char()) return this.bump(), this.error(vt.EMPTY_ARGUMENT, re(r, this.clonePosition()));
                     var n = this.parseIdentifierIfPossible().value;
-                    if (!n) return this.error(vt.MALFORMED_ARGUMENT, Qt(r, this.clonePosition()));
-                    if (this.bumpSpace(), this.isEOF()) return this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, Qt(r, this.clonePosition()));
+                    if (!n) return this.error(vt.MALFORMED_ARGUMENT, re(r, this.clonePosition()));
+                    if (this.bumpSpace(), this.isEOF()) return this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, re(r, this.clonePosition()));
                     switch (this.char()) {
                         case 125:
                             return this.bump(), {
                                 val: {
-                                    type: xt.argument,
+                                    type: kt.argument,
                                     value: n,
-                                    location: Qt(r, this.clonePosition())
+                                    location: re(r, this.clonePosition())
                                 },
                                 err: null
                             };
                         case 44:
-                            return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, Qt(r, this.clonePosition())) : this.parseArgumentOptions(t, e, n, r);
+                            return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, re(r, this.clonePosition())) : this.parseArgumentOptions(t, e, n, r);
                         default:
-                            return this.error(vt.MALFORMED_ARGUMENT, Qt(r, this.clonePosition()))
+                            return this.error(vt.MALFORMED_ARGUMENT, re(r, this.clonePosition()))
                     }
                 }, t.prototype.parseIdentifierIfPossible = function() {
                     var t = this.clonePosition(),
                         e = this.offset(),
-                        r = ce(this.message, e),
+                        r = fe(this.message, e),
                         n = e + r.length;
                     return this.bumpTo(n), {
                         value: r,
-                        location: Qt(t, this.clonePosition())
+                        location: re(t, this.clonePosition())
                     }
                 }, t.prototype.parseArgumentOptions = function(t, e, r, n) {
                     var o, i = this.clonePosition(),
                         a = this.parseIdentifierIfPossible().value,
                         s = this.clonePosition();
                     switch (a) {
                         case "":
-                            return this.error(vt.EXPECT_ARGUMENT_TYPE, Qt(i, s));
+                            return this.error(vt.EXPECT_ARGUMENT_TYPE, re(i, s));
                         case "number":
                         case "date":
                         case "time":
                             this.bumpSpace();
                             var c = null;
                             if (this.bumpIf(",")) {
                                 this.bumpSpace();
                                 var u = this.clonePosition();
                                 if ((y = this.parseSimpleArgStyleIfPossible()).err) return y;
-                                if (0 === (d = pe(y.val)).length) return this.error(vt.EXPECT_ARGUMENT_STYLE, Qt(this.clonePosition(), this.clonePosition()));
+                                if (0 === (d = ye(y.val)).length) return this.error(vt.EXPECT_ARGUMENT_STYLE, re(this.clonePosition(), this.clonePosition()));
                                 c = {
                                     style: d,
-                                    styleLocation: Qt(u, this.clonePosition())
+                                    styleLocation: re(u, this.clonePosition())
                                 }
                             }
                             if ((m = this.tryParseArgumentClose(n)).err) return m;
-                            var l = Qt(n, this.clonePosition());
-                            if (c && ue(null == c ? void 0 : c.style, "::", 0)) {
-                                var f = de(c.style.slice(2));
+                            var l = re(n, this.clonePosition());
+                            if (c && he(null == c ? void 0 : c.style, "::", 0)) {
+                                var f = ge(c.style.slice(2));
                                 if ("number" === a) return (y = this.parseNumberSkeletonFromString(f, c.styleLocation)).err ? y : {
                                     val: {
-                                        type: xt.number,
+                                        type: kt.number,
                                         value: r,
                                         location: l,
                                         style: y.val
                                     },
                                     err: null
                                 };
                                 if (0 === f.length) return this.error(vt.EXPECT_DATE_TIME_SKELETON, l);
@@ -11351,97 +11504,97 @@
                                 this.locale && (h = function(t, e) {
                                     for (var r = "", n = 0; n < t.length; n++) {
                                         var o = t.charAt(n);
                                         if ("j" === o) {
                                             for (var i = 0; n + 1 < t.length && t.charAt(n + 1) === o;) i++, n++;
                                             var a = 1 + (1 & i),
                                                 s = i < 2 ? 1 : 3 + (i >> 1),
-                                                c = Yt(e);
+                                                c = Qt(e);
                                             for ("H" != c && "k" != c || (s = 0); s-- > 0;) r += "a";
                                             for (; a-- > 0;) r = c + r
                                         } else r += "J" === o ? "H" : o
                                     }
                                     return r
                                 }(f, this.locale));
                                 var d = {
-                                    type: _t.dateTime,
+                                    type: At.dateTime,
                                     pattern: h,
                                     location: c.styleLocation,
-                                    parsedOptions: this.shouldParseSkeletons ? Mt(h) : {}
+                                    parsedOptions: this.shouldParseSkeletons ? $t(h) : {}
                                 };
                                 return {
                                     val: {
-                                        type: "date" === a ? xt.date : xt.time,
+                                        type: "date" === a ? kt.date : kt.time,
                                         value: r,
                                         location: l,
                                         style: d
                                     },
                                     err: null
                                 }
                             }
                             return {
                                 val: {
-                                    type: "number" === a ? xt.number : "date" === a ? xt.date : xt.time,
+                                    type: "number" === a ? kt.number : "date" === a ? kt.date : kt.time,
                                     value: r,
                                     location: l,
                                     style: null !== (o = null == c ? void 0 : c.style) && void 0 !== o ? o : null
                                 }, err: null
                             };
                         case "plural":
                         case "selectordinal":
                         case "select":
                             var p = this.clonePosition();
-                            if (this.bumpSpace(), !this.bumpIf(",")) return this.error(vt.EXPECT_SELECT_ARGUMENT_OPTIONS, Qt(p, (0, Et.pi)({}, p)));
+                            if (this.bumpSpace(), !this.bumpIf(",")) return this.error(vt.EXPECT_SELECT_ARGUMENT_OPTIONS, re(p, (0, St.pi)({}, p)));
                             this.bumpSpace();
                             var v = this.parseIdentifierIfPossible(),
                                 g = 0;
                             if ("select" !== a && "offset" === v.value) {
-                                if (!this.bumpIf(":")) return this.error(vt.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, Qt(this.clonePosition(), this.clonePosition()));
+                                if (!this.bumpIf(":")) return this.error(vt.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, re(this.clonePosition(), this.clonePosition()));
                                 var y;
                                 if (this.bumpSpace(), (y = this.tryParseDecimalInteger(vt.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, vt.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE)).err) return y;
                                 this.bumpSpace(), v = this.parseIdentifierIfPossible(), g = y.val
                             }
                             var m, b = this.tryParsePluralOrSelectOptions(t, a, e, v);
                             if (b.err) return b;
                             if ((m = this.tryParseArgumentClose(n)).err) return m;
-                            var w = Qt(n, this.clonePosition());
+                            var w = re(n, this.clonePosition());
                             return "select" === a ? {
                                 val: {
-                                    type: xt.select,
+                                    type: kt.select,
                                     value: r,
-                                    options: fe(b.val),
+                                    options: pe(b.val),
                                     location: w
                                 },
                                 err: null
                             } : {
                                 val: {
-                                    type: xt.plural,
+                                    type: kt.plural,
                                     value: r,
-                                    options: fe(b.val),
+                                    options: pe(b.val),
                                     offset: g,
                                     pluralType: "plural" === a ? "cardinal" : "ordinal",
                                     location: w
                                 },
                                 err: null
                             };
                         default:
-                            return this.error(vt.INVALID_ARGUMENT_TYPE, Qt(i, s))
+                            return this.error(vt.INVALID_ARGUMENT_TYPE, re(i, s))
                     }
                 }, t.prototype.tryParseArgumentClose = function(t) {
-                    return this.isEOF() || 125 !== this.char() ? this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, Qt(t, this.clonePosition())) : (this.bump(), {
+                    return this.isEOF() || 125 !== this.char() ? this.error(vt.EXPECT_ARGUMENT_CLOSING_BRACE, re(t, this.clonePosition())) : (this.bump(), {
                         val: !0,
                         err: null
                     })
                 }, t.prototype.parseSimpleArgStyleIfPossible = function() {
                     for (var t = 0, e = this.clonePosition(); !this.isEOF();) {
                         switch (this.char()) {
                             case 39:
                                 this.bump();
                                 var r = this.clonePosition();
-                                if (!this.bumpUntil("'")) return this.error(vt.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, Qt(r, this.clonePosition()));
+                                if (!this.bumpUntil("'")) return this.error(vt.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, re(r, this.clonePosition()));
                                 this.bump();
                                 break;
                             case 123:
                                 t += 1, this.bump();
                                 break;
                             case 125:
                                 if (!(t > 0)) return {
@@ -11459,15 +11612,15 @@
                         err: null
                     }
                 }, t.prototype.parseNumberSkeletonFromString = function(t, e) {
                     var r = [];
                     try {
                         r = function(t) {
                             if (0 === t.length) throw new Error("Number skeleton cannot be empty");
-                            for (var e = [], r = 0, n = t.split(jt).filter((function(t) {
+                            for (var e = [], r = 0, n = t.split(Ut).filter((function(t) {
                                     return t.length > 0
                                 })); r < n.length; r++) {
                                 var o = n[r].split("/");
                                 if (0 === o.length) throw new Error("Invalid number skeleton");
                                 for (var i = o[0], a = o.slice(1), s = 0, c = a; s < c.length; s++)
                                     if (0 === c[s].length) throw new Error("Invalid number skeleton");
                                 e.push({
@@ -11478,58 +11631,58 @@
                             return e
                         }(t)
                     } catch (n) {
                         return this.error(vt.INVALID_NUMBER_SKELETON, e)
                     }
                     return {
                         val: {
-                            type: _t.number,
+                            type: At.number,
                             tokens: r,
                             location: e,
-                            parsedOptions: this.shouldParseSkeletons ? Wt(r) : {}
+                            parsedOptions: this.shouldParseSkeletons ? Yt(r) : {}
                         },
                         err: null
                     }
                 }, t.prototype.tryParsePluralOrSelectOptions = function(t, e, r, n) {
                     for (var o, i = !1, a = [], s = new Set, c = n.value, u = n.location;;) {
                         if (0 === c.length) {
                             var l = this.clonePosition();
                             if ("select" === e || !this.bumpIf("=")) break;
                             var f = this.tryParseDecimalInteger(vt.EXPECT_PLURAL_ARGUMENT_SELECTOR, vt.INVALID_PLURAL_ARGUMENT_SELECTOR);
                             if (f.err) return f;
-                            u = Qt(l, this.clonePosition()), c = this.message.slice(l.offset, this.offset())
+                            u = re(l, this.clonePosition()), c = this.message.slice(l.offset, this.offset())
                         }
                         if (s.has(c)) return this.error("select" === e ? vt.DUPLICATE_SELECT_ARGUMENT_SELECTOR : vt.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, u);
                         "other" === c && (i = !0), this.bumpSpace();
                         var h = this.clonePosition();
-                        if (!this.bumpIf("{")) return this.error("select" === e ? vt.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : vt.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, Qt(this.clonePosition(), this.clonePosition()));
+                        if (!this.bumpIf("{")) return this.error("select" === e ? vt.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : vt.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, re(this.clonePosition(), this.clonePosition()));
                         var d = this.parseMessage(t + 1, e, r);
                         if (d.err) return d;
                         var p = this.tryParseArgumentClose(h);
                         if (p.err) return p;
                         a.push([c, {
                             value: d.val,
-                            location: Qt(h, this.clonePosition())
+                            location: re(h, this.clonePosition())
                         }]), s.add(c), this.bumpSpace(), c = (o = this.parseIdentifierIfPossible()).value, u = o.location
                     }
-                    return 0 === a.length ? this.error("select" === e ? vt.EXPECT_SELECT_ARGUMENT_SELECTOR : vt.EXPECT_PLURAL_ARGUMENT_SELECTOR, Qt(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !i ? this.error(vt.MISSING_OTHER_CLAUSE, Qt(this.clonePosition(), this.clonePosition())) : {
+                    return 0 === a.length ? this.error("select" === e ? vt.EXPECT_SELECT_ARGUMENT_SELECTOR : vt.EXPECT_PLURAL_ARGUMENT_SELECTOR, re(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !i ? this.error(vt.MISSING_OTHER_CLAUSE, re(this.clonePosition(), this.clonePosition())) : {
                         val: a,
                         err: null
                     }
                 }, t.prototype.tryParseDecimalInteger = function(t, e) {
                     var r = 1,
                         n = this.clonePosition();
                     this.bumpIf("+") || this.bumpIf("-") && (r = -1);
                     for (var o = !1, i = 0; !this.isEOF();) {
                         var a = this.char();
                         if (!(a >= 48 && a <= 57)) break;
                         o = !0, i = 10 * i + (a - 48), this.bump()
                     }
-                    var s = Qt(n, this.clonePosition());
-                    return o ? ae(i *= r) ? {
+                    var s = re(n, this.clonePosition());
+                    return o ? ue(i *= r) ? {
                         val: i,
                         err: null
                     } : this.error(e, s) : this.error(t, s)
                 }, t.prototype.offset = function() {
                     return this.position.offset
                 }, t.prototype.isEOF = function() {
                     return this.offset() === this.message.length
@@ -11538,15 +11691,15 @@
                         offset: this.position.offset,
                         line: this.position.line,
                         column: this.position.column
                     }
                 }, t.prototype.char = function() {
                     var t = this.position.offset;
                     if (t >= this.message.length) throw Error("out of bound");
-                    var e = he(this.message, t);
+                    var e = ve(this.message, t);
                     if (void 0 === e) throw Error("Offset ".concat(t, " is at invalid UTF-16 code unit boundary"));
                     return e
                 }, t.prototype.error = function(t, e) {
                     return {
                         val: null,
                         err: {
                             kind: t,
@@ -11556,15 +11709,15 @@
                     }
                 }, t.prototype.bump = function() {
                     if (!this.isEOF()) {
                         var t = this.char();
                         10 === t ? (this.position.line += 1, this.position.column = 1, this.position.offset += 1) : (this.position.column += 1, this.position.offset += t < 65536 ? 1 : 2)
                     }
                 }, t.prototype.bumpIf = function(t) {
-                    if (ue(this.message, t, this.offset())) {
+                    if (he(this.message, t, this.offset())) {
                         for (var e = 0; e < t.length; e++) this.bump();
                         return !0
                     }
                     return !1
                 }, t.prototype.bumpUntil = function(t) {
                     var e = this.offset(),
                         r = this.message.indexOf(t, e);
@@ -11574,326 +11727,326 @@
                     for (t = Math.min(t, this.message.length);;) {
                         var e = this.offset();
                         if (e === t) break;
                         if (e > t) throw Error("targetOffset ".concat(t, " is at invalid UTF-16 code unit boundary"));
                         if (this.bump(), this.isEOF()) break
                     }
                 }, t.prototype.bumpSpace = function() {
-                    for (; !this.isEOF() && be(this.char());) this.bump()
+                    for (; !this.isEOF() && xe(this.char());) this.bump()
                 }, t.prototype.peek = function() {
                     if (this.isEOF()) return null;
                     var t = this.char(),
                         e = this.offset(),
                         r = this.message.charCodeAt(e + (t >= 65536 ? 2 : 1));
                     return null != r ? r : null
                 }, t
             }();
 
-            function me(t) {
+            function Ee(t) {
                 return t >= 97 && t <= 122 || t >= 65 && t <= 90
             }
 
-            function be(t) {
+            function xe(t) {
                 return t >= 9 && t <= 13 || 32 === t || 133 === t || t >= 8206 && t <= 8207 || 8232 === t || 8233 === t
             }
 
-            function we(t) {
+            function _e(t) {
                 return t >= 33 && t <= 35 || 36 === t || t >= 37 && t <= 39 || 40 === t || 41 === t || 42 === t || 43 === t || 44 === t || 45 === t || t >= 46 && t <= 47 || t >= 58 && t <= 59 || t >= 60 && t <= 62 || t >= 63 && t <= 64 || 91 === t || 92 === t || 93 === t || 94 === t || 96 === t || 123 === t || 124 === t || 125 === t || 126 === t || 161 === t || t >= 162 && t <= 165 || 166 === t || 167 === t || 169 === t || 171 === t || 172 === t || 174 === t || 176 === t || 177 === t || 182 === t || 187 === t || 191 === t || 215 === t || 247 === t || t >= 8208 && t <= 8213 || t >= 8214 && t <= 8215 || 8216 === t || 8217 === t || 8218 === t || t >= 8219 && t <= 8220 || 8221 === t || 8222 === t || 8223 === t || t >= 8224 && t <= 8231 || t >= 8240 && t <= 8248 || 8249 === t || 8250 === t || t >= 8251 && t <= 8254 || t >= 8257 && t <= 8259 || 8260 === t || 8261 === t || 8262 === t || t >= 8263 && t <= 8273 || 8274 === t || 8275 === t || t >= 8277 && t <= 8286 || t >= 8592 && t <= 8596 || t >= 8597 && t <= 8601 || t >= 8602 && t <= 8603 || t >= 8604 && t <= 8607 || 8608 === t || t >= 8609 && t <= 8610 || 8611 === t || t >= 8612 && t <= 8613 || 8614 === t || t >= 8615 && t <= 8621 || 8622 === t || t >= 8623 && t <= 8653 || t >= 8654 && t <= 8655 || t >= 8656 && t <= 8657 || 8658 === t || 8659 === t || 8660 === t || t >= 8661 && t <= 8691 || t >= 8692 && t <= 8959 || t >= 8960 && t <= 8967 || 8968 === t || 8969 === t || 8970 === t || 8971 === t || t >= 8972 && t <= 8991 || t >= 8992 && t <= 8993 || t >= 8994 && t <= 9e3 || 9001 === t || 9002 === t || t >= 9003 && t <= 9083 || 9084 === t || t >= 9085 && t <= 9114 || t >= 9115 && t <= 9139 || t >= 9140 && t <= 9179 || t >= 9180 && t <= 9185 || t >= 9186 && t <= 9254 || t >= 9255 && t <= 9279 || t >= 9280 && t <= 9290 || t >= 9291 && t <= 9311 || t >= 9472 && t <= 9654 || 9655 === t || t >= 9656 && t <= 9664 || 9665 === t || t >= 9666 && t <= 9719 || t >= 9720 && t <= 9727 || t >= 9728 && t <= 9838 || 9839 === t || t >= 9840 && t <= 10087 || 10088 === t || 10089 === t || 10090 === t || 10091 === t || 10092 === t || 10093 === t || 10094 === t || 10095 === t || 10096 === t || 10097 === t || 10098 === t || 10099 === t || 10100 === t || 10101 === t || t >= 10132 && t <= 10175 || t >= 10176 && t <= 10180 || 10181 === t || 10182 === t || t >= 10183 && t <= 10213 || 10214 === t || 10215 === t || 10216 === t || 10217 === t || 10218 === t || 10219 === t || 10220 === t || 10221 === t || 10222 === t || 10223 === t || t >= 10224 && t <= 10239 || t >= 10240 && t <= 10495 || t >= 10496 && t <= 10626 || 10627 === t || 10628 === t || 10629 === t || 10630 === t || 10631 === t || 10632 === t || 10633 === t || 10634 === t || 10635 === t || 10636 === t || 10637 === t || 10638 === t || 10639 === t || 10640 === t || 10641 === t || 10642 === t || 10643 === t || 10644 === t || 10645 === t || 10646 === t || 10647 === t || 10648 === t || t >= 10649 && t <= 10711 || 10712 === t || 10713 === t || 10714 === t || 10715 === t || t >= 10716 && t <= 10747 || 10748 === t || 10749 === t || t >= 10750 && t <= 11007 || t >= 11008 && t <= 11055 || t >= 11056 && t <= 11076 || t >= 11077 && t <= 11078 || t >= 11079 && t <= 11084 || t >= 11085 && t <= 11123 || t >= 11124 && t <= 11125 || t >= 11126 && t <= 11157 || 11158 === t || t >= 11159 && t <= 11263 || t >= 11776 && t <= 11777 || 11778 === t || 11779 === t || 11780 === t || 11781 === t || t >= 11782 && t <= 11784 || 11785 === t || 11786 === t || 11787 === t || 11788 === t || 11789 === t || t >= 11790 && t <= 11798 || 11799 === t || t >= 11800 && t <= 11801 || 11802 === t || 11803 === t || 11804 === t || 11805 === t || t >= 11806 && t <= 11807 || 11808 === t || 11809 === t || 11810 === t || 11811 === t || 11812 === t || 11813 === t || 11814 === t || 11815 === t || 11816 === t || 11817 === t || t >= 11818 && t <= 11822 || 11823 === t || t >= 11824 && t <= 11833 || t >= 11834 && t <= 11835 || t >= 11836 && t <= 11839 || 11840 === t || 11841 === t || 11842 === t || t >= 11843 && t <= 11855 || t >= 11856 && t <= 11857 || 11858 === t || t >= 11859 && t <= 11903 || t >= 12289 && t <= 12291 || 12296 === t || 12297 === t || 12298 === t || 12299 === t || 12300 === t || 12301 === t || 12302 === t || 12303 === t || 12304 === t || 12305 === t || t >= 12306 && t <= 12307 || 12308 === t || 12309 === t || 12310 === t || 12311 === t || 12312 === t || 12313 === t || 12314 === t || 12315 === t || 12316 === t || 12317 === t || t >= 12318 && t <= 12319 || 12320 === t || 12336 === t || 64830 === t || 64831 === t || t >= 65093 && t <= 65094
             }
 
-            function Ee(t) {
+            function Se(t) {
                 t.forEach((function(t) {
-                    if (delete t.location, Pt(t) || Rt(t))
-                        for (var e in t.options) delete t.options[e].location, Ee(t.options[e].value);
-                    else At(t) && Lt(t.style) || (Tt(t) || Ot(t)) && Nt(t.style) ? delete t.style.location : It(t) && Ee(t.children)
+                    if (delete t.location, It(t) || Lt(t))
+                        for (var e in t.options) delete t.options[e].location, Se(t.options[e].value);
+                    else Pt(t) && Mt(t.style) || (Ct(t) || Rt(t)) && Bt(t.style) ? delete t.style.location : Ht(t) && Se(t.children)
                 }))
             }
 
-            function xe(t, e) {
-                void 0 === e && (e = {}), e = (0, Et.pi)({
+            function ke(t, e) {
+                void 0 === e && (e = {}), e = (0, St.pi)({
                     shouldParseSkeletons: !0,
                     requiresOtherClause: !0
                 }, e);
-                var r = new ye(t, e).parse();
+                var r = new we(t, e).parse();
                 if (r.err) {
                     var n = SyntaxError(vt[r.err.kind]);
                     throw n.location = r.err.location, n.originalMessage = r.err.message, n
                 }
-                return (null == e ? void 0 : e.captureLocation) || Ee(r.val), r.val
+                return (null == e ? void 0 : e.captureLocation) || Se(r.val), r.val
             }
             a(88770);
 
-            function _e(t, e) {
-                var r = e && e.cache ? e.cache : Ce,
-                    n = e && e.serializer ? e.serializer : Oe;
-                return (e && e.strategy ? e.strategy : Te)(t, {
+            function Ae(t, e) {
+                var r = e && e.cache ? e.cache : Ne,
+                    n = e && e.serializer ? e.serializer : Re;
+                return (e && e.strategy ? e.strategy : Ce)(t, {
                     cache: r,
                     serializer: n
                 })
             }
 
-            function Se(t, e, r, n) {
+            function Te(t, e, r, n) {
                 var o, i = null == (o = n) || "number" == typeof o || "boolean" == typeof o ? n : r(n),
                     a = e.get(i);
                 return void 0 === a && (a = t.call(this, n), e.set(i, a)), a
             }
 
-            function ke(t, e, r) {
+            function Oe(t, e, r) {
                 var n = Array.prototype.slice.call(arguments, 3),
                     o = r(n),
                     i = e.get(o);
                 return void 0 === i && (i = t.apply(this, n), e.set(o, i)), i
             }
 
-            function Ae(t, e, r, n, o) {
+            function Pe(t, e, r, n, o) {
                 return r.bind(e, t, n, o)
             }
 
-            function Te(t, e) {
-                return Ae(t, this, 1 === t.length ? Se : ke, e.cache.create(), e.serializer)
+            function Ce(t, e) {
+                return Pe(t, this, 1 === t.length ? Te : Oe, e.cache.create(), e.serializer)
             }
-            var Oe = function() {
+            var Re = function() {
                 return JSON.stringify(arguments)
             };
 
-            function Pe() {
+            function Ie() {
                 this.cache = Object.create(null)
             }
-            Pe.prototype.get = function(t) {
+            Ie.prototype.get = function(t) {
                 return this.cache[t]
-            }, Pe.prototype.set = function(t, e) {
+            }, Ie.prototype.set = function(t, e) {
                 this.cache[t] = e
             };
-            var Re, Ce = {
+            var Le, Ne = {
                     create: function() {
-                        return new Pe
+                        return new Ie
                     }
                 },
-                Ie = {
+                He = {
                     variadic: function(t, e) {
-                        return Ae(t, this, ke, e.cache.create(), e.serializer)
+                        return Pe(t, this, Oe, e.cache.create(), e.serializer)
                     },
                     monadic: function(t, e) {
-                        return Ae(t, this, Se, e.cache.create(), e.serializer)
+                        return Pe(t, this, Te, e.cache.create(), e.serializer)
                     }
                 };
             ! function(t) {
                 t.MISSING_VALUE = "MISSING_VALUE", t.INVALID_VALUE = "INVALID_VALUE", t.MISSING_INTL_API = "MISSING_INTL_API"
-            }(Re || (Re = {}));
-            var Le, Ne = function(t) {
+            }(Le || (Le = {}));
+            var Me, Be = function(t) {
                     function e(e, r, n) {
                         var o = t.call(this, e) || this;
                         return o.code = r, o.originalMessage = n, o
                     }
-                    return (0, Et.ZT)(e, t), e.prototype.toString = function() {
+                    return (0, St.ZT)(e, t), e.prototype.toString = function() {
                         return "[formatjs Error: ".concat(this.code, "] ").concat(this.message)
                     }, e
                 }(Error),
-                He = function(t) {
+                je = function(t) {
                     function e(e, r, n, o) {
-                        return t.call(this, 'Invalid values for "'.concat(e, '": "').concat(r, '". Options are "').concat(Object.keys(n).join('", "'), '"'), Re.INVALID_VALUE, o) || this
+                        return t.call(this, 'Invalid values for "'.concat(e, '": "').concat(r, '". Options are "').concat(Object.keys(n).join('", "'), '"'), Le.INVALID_VALUE, o) || this
                     }
-                    return (0, Et.ZT)(e, t), e
-                }(Ne),
-                Be = function(t) {
+                    return (0, St.ZT)(e, t), e
+                }(Be),
+                De = function(t) {
                     function e(e, r, n) {
-                        return t.call(this, 'Value for "'.concat(e, '" must be of type ').concat(r), Re.INVALID_VALUE, n) || this
+                        return t.call(this, 'Value for "'.concat(e, '" must be of type ').concat(r), Le.INVALID_VALUE, n) || this
                     }
-                    return (0, Et.ZT)(e, t), e
-                }(Ne),
-                Me = function(t) {
+                    return (0, St.ZT)(e, t), e
+                }(Be),
+                $e = function(t) {
                     function e(e, r) {
-                        return t.call(this, 'The intl string context variable "'.concat(e, '" was not provided to the string "').concat(r, '"'), Re.MISSING_VALUE, r) || this
+                        return t.call(this, 'The intl string context variable "'.concat(e, '" was not provided to the string "').concat(r, '"'), Le.MISSING_VALUE, r) || this
                     }
-                    return (0, Et.ZT)(e, t), e
-                }(Ne);
+                    return (0, St.ZT)(e, t), e
+                }(Be);
 
-            function je(t) {
+            function Ue(t) {
                 return "function" == typeof t
             }
 
-            function De(t, e, r, n, o, i, a) {
-                if (1 === t.length && St(t[0])) return [{
-                    type: Le.literal,
+            function Ze(t, e, r, n, o, i, a) {
+                if (1 === t.length && Tt(t[0])) return [{
+                    type: Me.literal,
                     value: t[0].value
                 }];
                 for (var s = [], c = 0, u = t; c < u.length; c++) {
                     var l = u[c];
-                    if (St(l)) s.push({
-                        type: Le.literal,
+                    if (Tt(l)) s.push({
+                        type: Me.literal,
                         value: l.value
                     });
-                    else if (Ct(l)) "number" == typeof i && s.push({
-                        type: Le.literal,
+                    else if (Nt(l)) "number" == typeof i && s.push({
+                        type: Me.literal,
                         value: r.getNumberFormat(e).format(i)
                     });
                     else {
                         var f = l.value;
-                        if (!o || !(f in o)) throw new Me(f, a);
+                        if (!o || !(f in o)) throw new $e(f, a);
                         var h = o[f];
-                        if (kt(l)) h && "string" != typeof h && "number" != typeof h || (h = "string" == typeof h || "number" == typeof h ? String(h) : ""), s.push({
-                            type: "string" == typeof h ? Le.literal : Le.object,
+                        if (Ot(l)) h && "string" != typeof h && "number" != typeof h || (h = "string" == typeof h || "number" == typeof h ? String(h) : ""), s.push({
+                            type: "string" == typeof h ? Me.literal : Me.object,
                             value: h
                         });
-                        else if (Tt(l)) {
-                            var d = "string" == typeof l.style ? n.date[l.style] : Nt(l.style) ? l.style.parsedOptions : void 0;
+                        else if (Ct(l)) {
+                            var d = "string" == typeof l.style ? n.date[l.style] : Bt(l.style) ? l.style.parsedOptions : void 0;
                             s.push({
-                                type: Le.literal,
+                                type: Me.literal,
                                 value: r.getDateTimeFormat(e, d).format(h)
                             })
-                        } else if (Ot(l)) {
-                            d = "string" == typeof l.style ? n.time[l.style] : Nt(l.style) ? l.style.parsedOptions : n.time.medium;
+                        } else if (Rt(l)) {
+                            d = "string" == typeof l.style ? n.time[l.style] : Bt(l.style) ? l.style.parsedOptions : n.time.medium;
                             s.push({
-                                type: Le.literal,
+                                type: Me.literal,
                                 value: r.getDateTimeFormat(e, d).format(h)
                             })
-                        } else if (At(l)) {
-                            (d = "string" == typeof l.style ? n.number[l.style] : Lt(l.style) ? l.style.parsedOptions : void 0) && d.scale && (h *= d.scale || 1), s.push({
-                                type: Le.literal,
+                        } else if (Pt(l)) {
+                            (d = "string" == typeof l.style ? n.number[l.style] : Mt(l.style) ? l.style.parsedOptions : void 0) && d.scale && (h *= d.scale || 1), s.push({
+                                type: Me.literal,
                                 value: r.getNumberFormat(e, d).format(h)
                             })
                         } else {
-                            if (It(l)) {
+                            if (Ht(l)) {
                                 var p = l.children,
                                     v = l.value,
                                     g = o[v];
-                                if (!je(g)) throw new Be(v, "function", a);
-                                var y = g(De(p, e, r, n, o, i).map((function(t) {
+                                if (!Ue(g)) throw new De(v, "function", a);
+                                var y = g(Ze(p, e, r, n, o, i).map((function(t) {
                                     return t.value
                                 })));
                                 Array.isArray(y) || (y = [y]), s.push.apply(s, y.map((function(t) {
                                     return {
-                                        type: "string" == typeof t ? Le.literal : Le.object,
+                                        type: "string" == typeof t ? Me.literal : Me.object,
                                         value: t
                                     }
                                 })))
                             }
-                            if (Pt(l)) {
-                                if (!(m = l.options[h] || l.options.other)) throw new He(l.value, h, Object.keys(l.options), a);
-                                s.push.apply(s, De(m.value, e, r, n, o))
-                            } else if (Rt(l)) {
+                            if (It(l)) {
+                                if (!(m = l.options[h] || l.options.other)) throw new je(l.value, h, Object.keys(l.options), a);
+                                s.push.apply(s, Ze(m.value, e, r, n, o))
+                            } else if (Lt(l)) {
                                 var m;
                                 if (!(m = l.options["=".concat(h)])) {
-                                    if (!Intl.PluralRules) throw new Ne('Intl.PluralRules is not available in this environment.\nTry polyfilling it using "@formatjs/intl-pluralrules"\n', Re.MISSING_INTL_API, a);
+                                    if (!Intl.PluralRules) throw new Be('Intl.PluralRules is not available in this environment.\nTry polyfilling it using "@formatjs/intl-pluralrules"\n', Le.MISSING_INTL_API, a);
                                     var b = r.getPluralRules(e, {
                                         type: l.pluralType
                                     }).select(h - (l.offset || 0));
                                     m = l.options[b] || l.options.other
                                 }
-                                if (!m) throw new He(l.value, h, Object.keys(l.options), a);
-                                s.push.apply(s, De(m.value, e, r, n, o, h - (l.offset || 0)))
+                                if (!m) throw new je(l.value, h, Object.keys(l.options), a);
+                                s.push.apply(s, Ze(m.value, e, r, n, o, h - (l.offset || 0)))
                             } else;
                         }
                     }
                 }
                 return function(t) {
                     return t.length < 2 ? t : t.reduce((function(t, e) {
                         var r = t[t.length - 1];
-                        return r && r.type === Le.literal && e.type === Le.literal ? r.value += e.value : t.push(e), t
+                        return r && r.type === Me.literal && e.type === Me.literal ? r.value += e.value : t.push(e), t
                     }), [])
                 }(s)
             }
 
-            function $e(t, e) {
+            function Fe(t, e) {
                 return e ? Object.keys(t).reduce((function(r, n) {
                     var o, i;
-                    return r[n] = (o = t[n], (i = e[n]) ? (0, Et.pi)((0, Et.pi)((0, Et.pi)({}, o || {}), i || {}), Object.keys(o).reduce((function(t, e) {
-                        return t[e] = (0, Et.pi)((0, Et.pi)({}, o[e]), i[e] || {}), t
+                    return r[n] = (o = t[n], (i = e[n]) ? (0, St.pi)((0, St.pi)((0, St.pi)({}, o || {}), i || {}), Object.keys(o).reduce((function(t, e) {
+                        return t[e] = (0, St.pi)((0, St.pi)({}, o[e]), i[e] || {}), t
                     }), {})) : o), r
-                }), (0, Et.pi)({}, t)) : t
+                }), (0, St.pi)({}, t)) : t
             }
 
-            function Ue(t) {
+            function Ge(t) {
                 return {
                     create: function() {
                         return {
                             get: function(e) {
                                 return t[e]
                             },
                             set: function(e, r) {
                                 t[e] = r
                             }
                         }
                     }
                 }
             }! function(t) {
                 t[t.literal = 0] = "literal", t[t.object = 1] = "object"
-            }(Le || (Le = {}));
-            var Ze, Fe = function() {
+            }(Me || (Me = {}));
+            var ze, Ve = function() {
                     function t(e, r, n, o) {
                         var i, a = this;
                         if (void 0 === r && (r = t.defaultLocale), this.formatterCache = {
                                 number: {},
                                 dateTime: {},
                                 pluralRules: {}
                             }, this.format = function(t) {
                                 var e = a.formatToParts(t);
                                 if (1 === e.length) return e[0].value;
                                 var r = e.reduce((function(t, e) {
-                                    return t.length && e.type === Le.literal && "string" == typeof t[t.length - 1] ? t[t.length - 1] += e.value : t.push(e.value), t
+                                    return t.length && e.type === Me.literal && "string" == typeof t[t.length - 1] ? t[t.length - 1] += e.value : t.push(e.value), t
                                 }), []);
                                 return r.length <= 1 ? r[0] || "" : r
                             }, this.formatToParts = function(t) {
-                                return De(a.ast, a.locales, a.formatters, a.formats, t, void 0, a.message)
+                                return Ze(a.ast, a.locales, a.formatters, a.formats, t, void 0, a.message)
                             }, this.resolvedOptions = function() {
                                 var t;
                                 return {
                                     locale: (null === (t = a.resolvedLocale) || void 0 === t ? void 0 : t.toString()) || Intl.NumberFormat.supportedLocalesOf(a.locales)[0]
                                 }
                             }, this.getAst = function() {
                                 return a.ast
                             }, this.locales = r, this.resolvedLocale = t.resolveLocale(r), "string" == typeof e) {
                             if (this.message = e, !t.__parse) throw new TypeError("IntlMessageFormat.__parse must be set to process `message` of type `string`");
                             var s = o || {},
-                                c = (s.formatters, (0, Et._T)(s, ["formatters"]));
-                            this.ast = t.__parse(e, (0, Et.pi)((0, Et.pi)({}, c), {
+                                c = (s.formatters, (0, St._T)(s, ["formatters"]));
+                            this.ast = t.__parse(e, (0, St.pi)((0, St.pi)({}, c), {
                                 locale: this.resolvedLocale
                             }))
                         } else this.ast = e;
                         if (!Array.isArray(this.ast)) throw new TypeError("A message must be provided as a String or AST.");
-                        this.formats = $e(t.formats, n), this.formatters = o && o.formatters || (void 0 === (i = this.formatterCache) && (i = {
+                        this.formats = Fe(t.formats, n), this.formatters = o && o.formatters || (void 0 === (i = this.formatterCache) && (i = {
                             number: {},
                             dateTime: {},
                             pluralRules: {}
                         }), {
-                            getNumberFormat: _e((function() {
+                            getNumberFormat: Ae((function() {
                                 for (var t, e = [], r = 0; r < arguments.length; r++) e[r] = arguments[r];
-                                return new((t = Intl.NumberFormat).bind.apply(t, (0, Et.ev)([void 0], e, !1)))
+                                return new((t = Intl.NumberFormat).bind.apply(t, (0, St.ev)([void 0], e, !1)))
                             }), {
-                                cache: Ue(i.number),
-                                strategy: Ie.variadic
+                                cache: Ge(i.number),
+                                strategy: He.variadic
                             }),
-                            getDateTimeFormat: _e((function() {
+                            getDateTimeFormat: Ae((function() {
                                 for (var t, e = [], r = 0; r < arguments.length; r++) e[r] = arguments[r];
-                                return new((t = Intl.DateTimeFormat).bind.apply(t, (0, Et.ev)([void 0], e, !1)))
+                                return new((t = Intl.DateTimeFormat).bind.apply(t, (0, St.ev)([void 0], e, !1)))
                             }), {
-                                cache: Ue(i.dateTime),
-                                strategy: Ie.variadic
+                                cache: Ge(i.dateTime),
+                                strategy: He.variadic
                             }),
-                            getPluralRules: _e((function() {
+                            getPluralRules: Ae((function() {
                                 for (var t, e = [], r = 0; r < arguments.length; r++) e[r] = arguments[r];
-                                return new((t = Intl.PluralRules).bind.apply(t, (0, Et.ev)([void 0], e, !1)))
+                                return new((t = Intl.PluralRules).bind.apply(t, (0, St.ev)([void 0], e, !1)))
                             }), {
-                                cache: Ue(i.pluralRules),
-                                strategy: Ie.variadic
+                                cache: Ge(i.pluralRules),
+                                strategy: He.variadic
                             })
                         })
                     }
                     return Object.defineProperty(t, "defaultLocale", {
                         get: function() {
                             return t.memoizedDefaultLocale || (t.memoizedDefaultLocale = (new Intl.NumberFormat).resolvedOptions().locale), t.memoizedDefaultLocale
                         },
                         enumerable: !1,
                         configurable: !0
                     }), t.memoizedDefaultLocale = null, t.resolveLocale = function(t) {
                         if (void 0 !== Intl.Locale) {
                             var e = Intl.NumberFormat.supportedLocalesOf(t);
                             return e.length > 0 ? new Intl.Locale(e[0]) : new Intl.Locale("string" == typeof t ? t : t[0])
                         }
-                    }, t.__parse = xe, t.formats = {
+                    }, t.__parse = ke, t.formats = {
                         number: {
                             integer: {
                                 maximumFractionDigits: 0
                             },
                             currency: {
                                 style: "currency"
                             },
@@ -11945,91 +12098,92 @@
                                 minute: "numeric",
                                 second: "numeric",
                                 timeZoneName: "short"
                             }
                         }
                     }, t
                 }(),
-                Ge = Fe,
-                ze = JSON.parse('{"title":"LCN","group":"Gruppe","module":"Modul","segment":"Segment","id":"ID","module-id":"Modul ID","segment-id":"Segment ID","name":"Name","entity-id":"Entitäts-ID","type":"Typ","resource":"Ressource","create":"Erstellen","dismiss":"Abbrechen","domain":"Domäne","binary-sensor":"Binärsensor","climate":"Klima","cover":"Abdeckung","light":"Licht","scene":"Szene","sensor":"Sensor","switch":"Schalter","variable":"Variable","variables":"Variablen","setpoint":"Sollwert","setpoints":"Sollwerte","motor":"Motor","reverse-delay":"Umkehrverzögerung","output":"Ausgang","outputs":"Ausgänge","relay":"Relais","relays":"Relais","port":"Anschluss","port-type":"Anschlusstyp","register":"Register","threshold":"Schwellwert","thresholds":"Schwellwerte","s0input":"S0 Eingang","s0inputs":"S0 Eingänge","led":"Led","leds":"Leds","logics":"Logiken","source":"Quelle","source-type":"Quellentyp","unit-lcn-native":"LCN nativ","unit-humidity":"Luftfeuchtigkeit","unit-wind":"Wind","unit-volts":"Volt","unit-milliamperes":"Milliampere","unit-angle":"Winkel","binary-sensor-type-binsensors":"Binärsensoren","binary-sensor-type-setpoint-locks":"Sperrung Sollwerte","binary-sensor-type-keys-locks":"Sperrung Tasten","dashboard-devices-title":"LCN Konfiguration","dashboard-devices-introduction":"Willkommen auf dem LCN Konfigurations-Dashboard.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Module scannen","dashboard-devices-for-host":"Module/Gruppen für Host","dashboard-devices-add":"Modul/Gruppe erstellen","dashboard-dialog-scan-devices-title":"Suche nach Modulen...","dashboard-dialog-scan-devices-text":"Das Suchen nach Modulen kann bis zu 30 Sekunden dauern. Dieses Fenster schließt sich automatisch.","dashboard-devices-dialog-add-alert-title":"Modul oder Gruppe existiert bereits","dashboard-devices-dialog-add-alert-text":"Das Modul oder die Gruppe existiert bereits:","dashboard-devices-dialog-add-alert-hint":"Module und Gruppen dürfen nur einmal angegeben werden.","dashboard-devices-dialog-request-info-title":"Fordere Eigenschaften vom LCN Modul an","dashboard-devices-dialog-request-info-text":"Die Eigenschaften für das angegebene Modul werden angefordert. Dies kann einige Sekunden dauern.","dashboard-devices-dialog-request-info-hint":"Dieses Fenster schließt sich automatisch.","dashboard-devices-table-delete":"Lösche Eintrag","dashboard-devices-table-no-data":"Keine Geräte konfiguriert.","dashboard-devices-dialog-delete-module-title":"Modul löschen","dashboard-devices-dialog-delete-group-title":"Gruppe löschen","dashboard-devices-dialog-delete-text":"Du möchtest folgendes Gerät löschen:","dashboard-devices-dialog-delete-warning":"Mit dem Löschen des Gerätes werden alle zugehörigen Entitäten gelöscht!","dashboard-devices-dialog-create-title":"Modul / Gruppe erstellen","dashboard-devices-dialog-error-segment":"Segment ID muss im Bereich 0, 5..128 liegen.","dashboard-devices-dialog-error-module":"Modul ID muss im Bereich 5..254 liegen.","dashboard-devices-dialog-error-group":"Gruppen ID muss im Bereich 5..254 liegen.","dashboard-entities-title":"Konfiguration Entitäten","dashboard-entities-introduction":"Konfiguration der Entitäten für dieses Modul / Gruppe.","dashboard-entities-add":"Entität erstellen","dashboard-entities-dialog-add-alert-title":"LCN Ressource existiert bereits","dashboard-entities-dialog-add-alert-text":"Die angegebene LCN Ressource ist der Entität bereits zugewiesen.","dashboard-entities-dialog-add-alert-hint":"LCN Ressourcen dürfen für jede Domäne nur einmal existieren.","dashboard-entities-table-delete":"Lösche Eintrag","dashboard-entities-table-no-data":"Keine Entitäten konfiguriert.","dashboard-entities-dialog-create-title":"Entität erstellen","dashboard-entities-dialog-unit-of-measurement":"Messeinheit","dashboard-entities-dialog-climate-lockable":"Sperrbar","dashboard-entities-dialog-climate-min-temperature":"Minimale Temperatur","dashboard-entities-dialog-climate-max-temperature":"Maximale Temperatur","dashboard-entities-dialog-climate-min-temperature-error":"Ungültige minimale Temperatur","dashboard-entities-dialog-climate-max-temperature-error":"Ungültige maximale Temperatur","dashboard-entities-dialog-light-dimmable":"Dimmbar","dashboard-entities-dialog-light-transition":"Rampe","dashboard-entities-dialog-light-transition-error":"Rampe muss im Bereich 0..486 liegen.","dashboard-entities-dialog-scene-transition":"Rampe","dashboard-entities-dialog-scene-transition-error":"Rampe muss im Bereich 0..486 liegen."}'),
-                Ve = a.t(ze, 2),
-                We = JSON.parse('{"title":"LCN","group":"Group","module":"Module","segment":"Segment","id":"ID","module-id":"Module ID","segment-id":"Segment ID","name":"Name","entity-id":"Entity ID","type":"Type","resource":"Resource","create":"Create","dismiss":"Dismiss","domain":"Domain","binary-sensor":"Binary sensor","climate":"Climate","cover":"Cover","light":"Light","scene":"Scene","sensor":"Sensor","switch":"Switch","variable":"Variable","variables":"Variables","setpoint":"Setpoint","setpoints":"Setpoints","motor":"Motor","reverse-delay":"Reverse delay","output":"Output","outputs":"Outputs","relay":"Relay","relays":"Realys","port":"Port","port-type":"Port type","register":"Register","threshold":"Threshold","thresholds":"Thresholds","s0input":"S0 Input","s0inputs":"S0 Inputs","led":"Led","leds":"Leds","logic":"Logic","logics":"Logics","source":"Source","source-type":"Source type","unit-lcn-native":"LCN native","unit-humidity":"Humidity","unit-wind":"Wind","unit-volts":"Volts","unit-milliamperes":"Milliamperes","unit-angle":"Angle","binary-sensor-type-binsensors":"Binary sensors","binary-sensor-type-setpoint-locks":"Lock state setpoints","binary-sensor-type-keys-locks":"Lock state keys","dashboard-devices-title":"LCN Configuration Dashboard","dashboard-devices-introduction":"Welcome to the LCN configuration dashboard.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Scan modules","dashboard-devices-for-host":"Modules/groups for host","dashboard-devices-add":"Create module/group","dashboard-dialog-scan-devices-title":"Scanning for modules...","dashboard-dialog-scan-devices-text":"Scanning for modules might take up to 30 seconds. This dialog will close automatically.","dashboard-devices-dialog-add-alert-title":"Module or group already exists","dashboard-devices-dialog-add-alert-text":"The specified module or group already exists:","dashboard-devices-dialog-add-alert-hint":"Modules and groups have to be unique.","dashboard-devices-dialog-request-info-title":"Requesting device info from LCN","dashboard-devices-dialog-request-info-text":"The information for the specified device is beeing requested from LCN. This might take several seconds.","dashboard-devices-dialog-request-info-hint":"This dialog will close automatically.","dashboard-devices-table-delete":"Delete entry","dashboard-devices-table-no-data":"No devices configured.","dashboard-devices-dialog-delete-module-title":"Delete module","dashboard-devices-dialog-delete-group-title":"Delete group","dashboard-devices-dialog-delete-text":"You are about to delete:","dashboard-devices-dialog-delete-warning":"Removing a device will also delete all associated entities!","dashboard-devices-dialog-create-title":"Create module / group","dashboard-devices-dialog-error-segment":"Segment ID must be 0, 5..128.","dashboard-devices-dialog-error-module":"Module ID must be 5..254.","dashboard-devices-dialog-error-group":"Group ID must be 5..254.","dashboard-entities-title":"Entities configuration","dashboard-entities-introduction":"Configure entities for this module / group.","dashboard-entities-add":"Create entity","dashboard-entities-dialog-add-alert-title":"LCN resource already assigned","dashboard-entities-dialog-add-alert-text":"The specified LCN resource is already assigned to this entity.","dashboard-entities-dialog-add-alert-hint":"LCN resources may only be assigned once within a domain.","dashboard-entities-table-delete":"Delete entry","dashboard-entities-table-no-data":"No entities configured.","dashboard-entities-dialog-create-title":"Create entity","dashboard-entities-dialog-unit-of-measurement":"Unit of measurement","dashboard-entities-dialog-climate-lockable":"Lockable","dashboard-entities-dialog-climate-min-temperature":"Minimum temperature","dashboard-entities-dialog-climate-max-temperature":"Maximum temperature","dashboard-entities-dialog-climate-min-temperature-error":"Invalid minimum temperature","dashboard-entities-dialog-climate-max-temperature-error":"Invalid maximum temperature","dashboard-entities-dialog-light-dimmable":"Dimmable","dashboard-entities-dialog-light-transition":"Transition","dashboard-entities-dialog-light-transition-error":"Transition must be in 0..486.","dashboard-entities-dialog-scene-transition":"Transition","dashboard-entities-dialog-scene-transition-error":"Transition must be in 0..486."}'),
-                Ke = {
-                    de: Ve,
-                    en: a.t(We, 2)
+                We = Ve,
+                Ke = JSON.parse('{"title":"LCN","group":"Gruppe","module":"Modul","segment":"Segment","id":"ID","module-id":"Modul ID","segment-id":"Segment ID","name":"Name","entity-id":"Entitäts-ID","type":"Typ","resource":"Ressource","create":"Erstellen","dismiss":"Abbrechen","domain":"Domäne","binary-sensor":"Binärsensor","climate":"Klima","cover":"Abdeckung","light":"Licht","scene":"Szene","sensor":"Sensor","switch":"Schalter","variable":"Variable","variables":"Variablen","setpoint":"Sollwert","setpoints":"Sollwerte","motor":"Motor","reverse-delay":"Umkehrverzögerung","output":"Ausgang","outputs":"Ausgänge","relay":"Relais","relays":"Relais","port":"Anschluss","port-type":"Anschlusstyp","register":"Register","threshold":"Schwellwert","thresholds":"Schwellwerte","s0input":"S0 Eingang","s0inputs":"S0 Eingänge","led":"Led","leds":"Leds","logics":"Logiken","source":"Quelle","source-type":"Quellentyp","unit-lcn-native":"LCN nativ","unit-humidity":"Luftfeuchtigkeit","unit-wind":"Wind","unit-volts":"Volt","unit-milliamperes":"Milliampere","unit-angle":"Winkel","binary-sensor-type-binsensors":"Binärsensoren","binary-sensor-type-setpoint-locks":"Sperrung Sollwerte","binary-sensor-type-keys-locks":"Sperrung Tasten","more-help":"mehr Hilfe...","dashboard-devices-title":"LCN Konfiguration","dashboard-devices-introduction":"Willkommen auf dem LCN Konfigurations-Dashboard!","dashboard-devices-introduction-help-1":"Hier kannst du die Module und Gruppen deines LCN Systems konfigurieren.","dashboard-devices-introduction-help-2":"Um zu beginnen, selektiere deinen Host und starte eine automatische Suche nach LCN Modulen. Die gefundenen Module werden in der Liste angezeigt.","dashboard-devices-introduction-help-3":"Wird ein Modul nicht automatisch erkannt, kannst du das Modul auch manuell hinzufügen.","dashboard-devices-introduction-help-4":"Klicke auf einen Eintrag in der Liste, um die zugehörigen Entitäten anzuzeigen und zu editieren.","dashboard-devices-introduction-help-5":"Wenn du einen Eintrag löschen möchtest, klicke auf das Mülleimersymbol neben dem Eintrag.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Module scannen","dashboard-devices-for-host":"Module/Gruppen für Host","dashboard-devices-add":"Modul/Gruppe erstellen","dashboard-dialog-scan-devices-title":"Suche nach Modulen...","dashboard-dialog-scan-devices-text":"Das Suchen nach Modulen kann bis zu 30 Sekunden dauern. Dieses Fenster schließt sich automatisch.","dashboard-devices-dialog-add-alert-title":"Modul oder Gruppe existiert bereits","dashboard-devices-dialog-add-alert-text":"Das Modul oder die Gruppe existiert bereits:","dashboard-devices-dialog-add-alert-hint":"Module und Gruppen dürfen nur einmal angegeben werden.","dashboard-devices-dialog-request-info-title":"Fordere Eigenschaften vom LCN Modul an","dashboard-devices-dialog-request-info-text":"Die Eigenschaften für das angegebene Modul werden angefordert. Dies kann einige Sekunden dauern.","dashboard-devices-dialog-request-info-hint":"Dieses Fenster schließt sich automatisch.","dashboard-devices-table-delete":"Lösche Eintrag","dashboard-devices-table-no-data":"Keine Geräte konfiguriert.","dashboard-devices-dialog-delete-module-title":"Modul löschen","dashboard-devices-dialog-delete-group-title":"Gruppe löschen","dashboard-devices-dialog-delete-text":"Du möchtest folgendes Gerät löschen:","dashboard-devices-dialog-delete-warning":"Mit dem Löschen des Gerätes werden alle zugehörigen Entitäten gelöscht!","dashboard-devices-dialog-create-title":"Modul / Gruppe erstellen","dashboard-devices-dialog-error-segment":"Segment ID muss im Bereich 0, 5..128 liegen.","dashboard-devices-dialog-error-module":"Modul ID muss im Bereich 5..254 liegen.","dashboard-devices-dialog-error-group":"Gruppen ID muss im Bereich 5..254 liegen.","dashboard-entities-title":"LCN Entitäten","dashboard-entities-introduction":"Konfiguriere die Entitäten für dieses Modul / diese Gruppe.","dashboard-entities-introduction-help-1":"Füge neue Entitäten, die dieses Modul/Gruppe bereitstellt zu deiner Konfiguration hinzu.","dashboard-entities-introduction-help-2":"Klicke auf \\"Entität erstellen\\", wähle die Domäne aus und konfiguriere die Parameter entsprechend deiner LCN Installation.","dashboard-entities-introduction-help-3":"Du kannst die erstellten Entitäten nach Belieben in deinen Dashboards verwenden.","dashboard-entities-introduction-help-4":"Wenn du eine Entität löschen möchtest, klicke auf das Mülleimersymbol neben dem Eintrag.","dashboard-entities-introduction-help-5":"Möchtest du die Parameter einer Entität ändern, musst du sie zunächst löschen und danach neu erstellen.","dashboard-entities-entities-for-module":"Entities für Modul","dashboard-entities-entities-for-group":"Entities für Gruppe","dashboard-entities-add":"Entität erstellen","dashboard-entities-dialog-add-alert-title":"LCN Ressource existiert bereits","dashboard-entities-dialog-add-alert-text":"Die angegebene LCN Ressource ist der Entität bereits zugewiesen.","dashboard-entities-dialog-add-alert-hint":"LCN Ressourcen dürfen für jede Domäne nur einmal existieren.","dashboard-entities-table-delete":"Lösche Eintrag","dashboard-entities-table-no-data":"Keine Entitäten konfiguriert.","dashboard-entities-dialog-create-title":"Entität erstellen","dashboard-entities-dialog-unit-of-measurement":"Messeinheit","dashboard-entities-dialog-climate-lockable":"Sperrbar","dashboard-entities-dialog-climate-min-temperature":"Minimale Temperatur","dashboard-entities-dialog-climate-max-temperature":"Maximale Temperatur","dashboard-entities-dialog-climate-min-temperature-error":"Ungültige minimale Temperatur","dashboard-entities-dialog-climate-max-temperature-error":"Ungültige maximale Temperatur","dashboard-entities-dialog-light-dimmable":"Dimmbar","dashboard-entities-dialog-light-transition":"Rampe","dashboard-entities-dialog-light-transition-error":"Rampe muss im Bereich 0..486 liegen.","dashboard-entities-dialog-scene-transition":"Rampe","dashboard-entities-dialog-scene-transition-error":"Rampe muss im Bereich 0..486 liegen."}'),
+                Xe = a.t(Ke, 2),
+                Ye = JSON.parse('{"title":"LCN","group":"Group","module":"Module","segment":"Segment","id":"ID","module-id":"Module ID","segment-id":"Segment ID","name":"Name","entity-id":"Entity ID","type":"Type","resource":"Resource","create":"Create","dismiss":"Dismiss","domain":"Domain","binary-sensor":"Binary sensor","climate":"Climate","cover":"Cover","light":"Light","scene":"Scene","sensor":"Sensor","switch":"Switch","variable":"Variable","variables":"Variables","setpoint":"Setpoint","setpoints":"Setpoints","motor":"Motor","reverse-delay":"Reverse delay","output":"Output","outputs":"Outputs","relay":"Relay","relays":"Realys","port":"Port","port-type":"Port type","register":"Register","threshold":"Threshold","thresholds":"Thresholds","s0input":"S0 Input","s0inputs":"S0 Inputs","led":"Led","leds":"Leds","logic":"Logic","logics":"Logics","source":"Source","source-type":"Source type","unit-lcn-native":"LCN native","unit-humidity":"Humidity","unit-wind":"Wind","unit-volts":"Volts","unit-milliamperes":"Milliamperes","unit-angle":"Angle","binary-sensor-type-binsensors":"Binary sensors","binary-sensor-type-setpoint-locks":"Lock state setpoints","binary-sensor-type-keys-locks":"Lock state keys","more-help":"more help...","dashboard-devices-title":"LCN Configuration Dashboard","dashboard-devices-introduction":"Welcome to the LCN configuration dashboard!","dashboard-devices-introduction-help-1":"Here you can configure the modules and groups of your LCN system.","dashboard-devices-introduction-help-2":"To get started, select your host and start an automatic search for LCN modules. The modules found are displayed in the list.","dashboard-devices-introduction-help-3":"If a module is not recognized automatically, you can add the module manually.","dashboard-devices-introduction-help-4":"Click on an entry in the list to display and edit the associated entities.","dashboard-devices-introduction-help-5":"If you want to delete an entry, click on the trash can icon next to the entry.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Scan modules","dashboard-devices-for-host":"Modules/groups for host","dashboard-devices-add":"Create module/group","dashboard-dialog-scan-devices-title":"Scanning for modules...","dashboard-dialog-scan-devices-text":"Scanning for modules might take up to 30 seconds. This dialog will close automatically.","dashboard-devices-dialog-add-alert-title":"Module or group already exists","dashboard-devices-dialog-add-alert-text":"The specified module or group already exists:","dashboard-devices-dialog-add-alert-hint":"Modules and groups have to be unique.","dashboard-devices-dialog-request-info-title":"Requesting device info from LCN","dashboard-devices-dialog-request-info-text":"The information for the specified device is beeing requested from LCN. This might take several seconds.","dashboard-devices-dialog-request-info-hint":"This dialog will close automatically.","dashboard-devices-table-delete":"Delete entry","dashboard-devices-table-no-data":"No devices configured.","dashboard-devices-dialog-delete-module-title":"Delete module","dashboard-devices-dialog-delete-group-title":"Delete group","dashboard-devices-dialog-delete-text":"You are about to delete:","dashboard-devices-dialog-delete-warning":"Removing a device will also delete all associated entities!","dashboard-devices-dialog-create-title":"Create module / group","dashboard-devices-dialog-error-segment":"Segment ID must be 0, 5..128.","dashboard-devices-dialog-error-module":"Module ID must be 5..254.","dashboard-devices-dialog-error-group":"Group ID must be 5..254.","dashboard-entities-title":"LCN Entities","dashboard-entities-introduction":"Configure the entities for this module / group.","dashboard-entities-introduction-help-1":"Add new entities provided by this module/group to your configuration.","dashboard-entities-introduction-help-2":"Click on \\"Create entity\\", select the domain and configure the parameters according to your LCN installation.","dashboard-entities-introduction-help-3":"You can use the created entities in your dashboards as you wish.","dashboard-entities-introduction-help-4":"If you want to delete an entity, click on the trash can icon next to the entry.","dashboard-entities-introduction-help-5":"To change the parameters of an entity, you must first delete it and then create a new one.","dashboard-entities-entities-for-module":"Entities for module","dashboard-entities-entities-for-group":"Entities for group","dashboard-entities-add":"Create entity","dashboard-entities-dialog-add-alert-title":"LCN resource already assigned","dashboard-entities-dialog-add-alert-text":"The specified LCN resource is already assigned to this entity.","dashboard-entities-dialog-add-alert-hint":"LCN resources may only be assigned once within a domain.","dashboard-entities-table-delete":"Delete entry","dashboard-entities-table-no-data":"No entities configured.","dashboard-entities-dialog-create-title":"Create entity","dashboard-entities-dialog-unit-of-measurement":"Unit of measurement","dashboard-entities-dialog-climate-lockable":"Lockable","dashboard-entities-dialog-climate-min-temperature":"Minimum temperature","dashboard-entities-dialog-climate-max-temperature":"Maximum temperature","dashboard-entities-dialog-climate-min-temperature-error":"Invalid minimum temperature","dashboard-entities-dialog-climate-max-temperature-error":"Invalid maximum temperature","dashboard-entities-dialog-light-dimmable":"Dimmable","dashboard-entities-dialog-light-transition":"Transition","dashboard-entities-dialog-light-transition-error":"Transition must be in 0..486.","dashboard-entities-dialog-scene-transition":"Transition","dashboard-entities-dialog-scene-transition-error":"Transition must be in 0..486."}'),
+                qe = {
+                    de: Xe,
+                    en: a.t(Ye, 2)
                 },
-                Xe = "en",
-                Ye = {
+                Je = "en",
+                Qe = new Et("localize"),
+                tr = {
                     language: [],
                     sting: {}
                 },
-                qe = {};
-            (0, N.Z)([(0, M.Mo)("lcn-frontend")], (function(t, e) {
+                er = {};
+            (0, N.Z)([(0, B.Mo)("lcn-frontend")], (function(t, e) {
                 var r = function(e) {
                     (0, I.Z)(n, e);
                     var r = (0, L.Z)(n);
 
                     function n() {
                         var e;
-                        (0, R.Z)(this, n);
+                        (0, C.Z)(this, n);
                         for (var o = arguments.length, i = new Array(o), a = 0; a < o; a++) i[a] = arguments[a];
-                        return e = r.call.apply(r, [this].concat(i)), t((0, C.Z)(e)), e
+                        return e = r.call.apply(r, [this].concat(i)), t((0, R.Z)(e)), e
                     }
                     return (0, P.Z)(n)
                 }(e);
                 return {
                     F: r,
                     d: [{
                         kind: "field",
-                        decorators: [(0, M.Cb)({
+                        decorators: [(0, B.Cb)({
                             attribute: !1
                         })],
                         key: "hass",
                         value: void 0
                     }, {
                         kind: "field",
-                        decorators: [(0, M.Cb)({
+                        decorators: [(0, B.Cb)({
                             attribute: !1
                         })],
                         key: "lcn",
                         value: void 0
                     }, {
                         kind: "field",
-                        decorators: [(0, M.Cb)({
+                        decorators: [(0, B.Cb)({
                             attribute: !1
                         })],
                         key: "narrow",
                         value: void 0
                     }, {
                         kind: "field",
-                        decorators: [(0, M.Cb)({
+                        decorators: [(0, B.Cb)({
                             attribute: !1
                         })],
                         key: "route",
                         value: void 0
                     }, {
                         kind: "method",
                         key: "firstUpdated",
                         value: function(t) {
                             var e, n, o, i = this;
-                            ((0, H.Z)((0, B.Z)(r.prototype), "firstUpdated", this).call(this, t), this.hass) && (this.lcn || this._initLCN(), this.addEventListener("lcn-location-changed", (function(t) {
+                            ((0, H.Z)((0, M.Z)(r.prototype), "firstUpdated", this).call(this, t), this.hass) && (this.lcn || this._initLCN(), this.addEventListener("lcn-location-changed", (function(t) {
                                 return i._setRoute(t)
                             })), (0, ht.lD)(this, this.shadowRoot), "" !== this.route.path && "/" !== this.route.path || (0, ft.c)("/lcn/devices", {
                                 replace: !0
                             }), e = function(t) {
                                 i._applyTheme()
                             }, n = matchMedia("(prefers-color-scheme: dark)"), o = function(t) {
                                 return e(t.matches)
                             }, n.addListener(o), e(n.matches))
                         }
                     }, {
                         kind: "method",
                         key: "render",
                         value: function() {
-                            return this.hass ? (0, A.dy)(Ze || (Ze = (0, k.Z)(["\n      <lcn-router\n        .hass=", "\n        .lcn=", "\n        .route=", "\n        .narrow=", "\n      ></lcn-router>\n    "])), this.hass, this.lcn, this.route, this.narrow) : A.Ld
+                            return this.hass && this.lcn ? (0, A.dy)(ze || (ze = (0, k.Z)(["\n      <lcn-router\n        .hass=", "\n        .lcn=", "\n        .route=", "\n        .narrow=", "\n      ></lcn-router>\n    "])), this.hass, this.lcn, this.route, this.narrow) : A.Ld
                         }
                     }, {
                         kind: "method",
                         key: "_initLCN",
                         value: function() {
                             var t, e, r, n = this;
                             (t = this.hass, e = {
@@ -12041,35 +12195,36 @@
                                     return null === t.disabled_by
                                 }));
                                 void 0 !== e && (n.lcn = {
                                     language: n.hass.language,
                                     config_entries: t,
                                     localize: function(t, e) {
                                         return function(t, e, r) {
-                                            var n, o, i = (t || localStorage.getItem("selectedLanguage") || Xe).replace(/['"]+/g, "").replace("-", "_");
-                                            Ke[i] || (null !== (o = Ye.language) && void 0 !== o && o.includes(i) || Ye.language.push(i), i = Xe);
-                                            var a = (null === (n = Ke[i]) || void 0 === n ? void 0 : n[e]) || Ke[Xe][e];
-                                            if (!a) return console.error("Translation problem with '".concat(e, "' for '").concat(i, "'")), "";
+                                            var n, o, i = (t || localStorage.getItem("selectedLanguage") || Je).replace(/['"]+/g, "").replace("-", "_");
+                                            qe[i] || (null !== (o = tr.language) && void 0 !== o && o.includes(i) || tr.language.push(i), i = Je);
+                                            var a = (null === (n = qe[i]) || void 0 === n ? void 0 : n[e]) || qe[Je][e];
+                                            if (!a) return Qe.error("Translation problem with '".concat(e, "' for '").concat(i, "'")), "";
                                             var s = e + a,
-                                                c = qe[s];
+                                                c = er[s];
                                             if (!c) {
                                                 try {
-                                                    c = new Ge(a, t)
+                                                    c = new We(a, t)
                                                 } catch (u) {
-                                                    return console.warn("Translation problem with '".concat(e, "' for '").concat(i, "'")), ""
+                                                    return Qe.warn("Translation problem with '".concat(e, "' for '").concat(i, "'")), ""
                                                 }
-                                                qe[s] = c
+                                                er[s] = c
                                             }
                                             try {
                                                 return c.format(r)
                                             } catch (u) {
-                                                return console.warn("Translation problem with '".concat(e, "' for '").concat(i, "'")), ""
+                                                return Qe.warn("Translation problem with '".concat(e, "' for '").concat(i, "'")), ""
                                             }
                                         }(n.hass.language || "en", t, e)
                                     },
+                                    log: new Et,
                                     host: {
                                         name: e.title,
                                         id: e.entry_id
                                     },
                                     address: [0, 0, !1]
                                 })
                             }))
@@ -12096,30 +12251,30 @@
                 }
             }), function(t) {
                 (0, I.Z)(r, t);
                 var e = (0, L.Z)(r);
 
                 function r() {
                     var t;
-                    (0, R.Z)(this, r);
+                    (0, C.Z)(this, r);
                     for (var n = arguments.length, o = new Array(n), i = 0; i < n; i++) o[i] = arguments[i];
                     return (t = e.call.apply(e, [this].concat(o))).hass = void 0, t.__provideHass = [], t
                 }
                 return (0, P.Z)(r, [{
                     key: "provideHass",
                     value: function(t) {
                         this.__provideHass.push(t), t.hass = this.hass
                     }
                 }, {
                     key: "updated",
                     value: function(t) {
                         var e = this;
-                        (0, H.Z)((0, B.Z)(r.prototype), "updated", this).call(this, t), t.has("hass") && this.__provideHass.forEach((function(t) {
+                        (0, H.Z)((0, M.Z)(r.prototype), "updated", this).call(this, t), t.has("hass") && this.__provideHass.forEach((function(t) {
                             t.hass = e.hass
                         }))
                     }
                 }]), r
             }(A.oi));
-            var Je = document.createElement("style");
-            Je.innerHTML = "\nbody {\n  font-family: Roboto, sans-serif;\n  -moz-osx-font-smoothing: grayscale;\n  -webkit-font-smoothing: antialiased;\n  font-weight: 400;\n  margin: 0;\n  padding: 0;\n  height: 100vh;\n}\n@media (prefers-color-scheme: dark) {\n  body {\n    background-color: #111111;\n    color: #e1e1e1;\n  }\n}\n", document.head.appendChild(Je)
+            var rr = document.createElement("style");
+            rr.innerHTML = "\nbody {\n  font-family: Roboto, sans-serif;\n  -moz-osx-font-smoothing: grayscale;\n  -webkit-font-smoothing: antialiased;\n  font-weight: 400;\n  margin: 0;\n  padding: 0;\n  height: 100vh;\n}\n@media (prefers-color-scheme: dark) {\n  body {\n    background-color: #111111;\n    color: #e1e1e1;\n  }\n}\n", document.head.appendChild(rr)
         }()
 }();
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/f67fx1_K.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/f67fx1_K.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/f67fx1_K.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/f67fx1_K.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/gWLSf6Uq.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/gWLSf6Uq.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/gWLSf6Uq.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/gWLSf6Uq.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/kY1AJzRb.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/kY1AJzRb.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/kY1AJzRb.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/kY1AJzRb.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/nqy1LXz0.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/mNa8_BnN.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,48 @@
 "use strict";
 (self.webpackChunklcn_frontend = self.webpackChunklcn_frontend || []).push([
     [981], {
         70981: function(t, e, n) {
             n.r(e), n.d(e, {
                 LCNEntitiesPage: function() {
-                    return z
+                    return H
                 }
             });
-            var i, a, r, s, o, c = n(88962),
-                d = n(99312),
-                l = n(81043),
+            var i, a, s, r, o, d, c = n(88962),
+                l = n(99312),
+                h = n(81043),
                 u = n(33368),
-                h = n(71650),
-                f = n(82390),
+                f = n(71650),
+                b = n(82390),
                 v = n(69205),
-                b = n(70906),
-                p = n(51565),
-                k = n(34541),
-                y = n(47838),
-                g = (n(97393), n(22859), n(85472), n(46798), n(9849), n(90126), n(68144)),
+                p = n(70906),
+                k = n(51565),
+                y = n(34541),
+                g = n(47838),
+                m = (n(97393), n(22859), n(85472), n(46798), n(9849), n(90126), n(68144)),
                 Z = n(73175),
-                m = (n(70657), n(31952), n(84776), n(68336), n(37662), n(99040), n(46349), n(70320), n(85717), n(54371), n(14516)),
-                w = n(51750),
-                _ = n(9051),
-                C = "M19,4H15.5L14.5,3H9.5L8.5,4H5V6H19M6,19A2,2 0 0,0 8,21H16A2,2 0 0,0 18,19V7H6V19Z",
-                x = ((0, p.Z)([(0, Z.Mo)("lcn-entities-data-table")], (function(t, e) {
-                    var n, s = function(e) {
+                w = (n(70657), n(31952), n(84776), n(68336), n(37662), n(99040), n(46349), n(70320), n(85717), n(54371), n(14516)),
+                _ = n(51750),
+                C = n(9051),
+                z = "M19,4H15.5L14.5,3H9.5L8.5,4H5V6H19M6,19A2,2 0 0,0 8,21H16A2,2 0 0,0 18,19V7H6V19Z",
+                x = ((0, k.Z)([(0, Z.Mo)("lcn-entities-data-table")], (function(t, e) {
+                    var n, r = function(e) {
                         (0, v.Z)(i, e);
-                        var n = (0, b.Z)(i);
+                        var n = (0, p.Z)(i);
 
                         function i() {
                             var e;
-                            (0, h.Z)(this, i);
-                            for (var a = arguments.length, r = new Array(a), s = 0; s < a; s++) r[s] = arguments[s];
-                            return e = n.call.apply(n, [this].concat(r)), t((0, f.Z)(e)), e
+                            (0, f.Z)(this, i);
+                            for (var a = arguments.length, s = new Array(a), r = 0; r < a; r++) s[r] = arguments[r];
+                            return e = n.call.apply(n, [this].concat(s)), t((0, b.Z)(e)), e
                         }
                         return (0, u.Z)(i)
                     }(e);
                     return {
-                        F: s,
+                        F: r,
                         d: [{
                             kind: "field",
                             decorators: [(0, Z.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -76,41 +76,41 @@
                             value: function() {
                                 return []
                             }
                         }, {
                             kind: "field",
                             key: "_entities",
                             value: function() {
-                                return (0, m.Z)((function(t) {
+                                return (0, w.Z)((function(t) {
                                     return t.map((function(t) {
                                         return Object.assign(Object.assign({}, t), {}, {
                                             delete: t
                                         })
                                     }))
                                 }))
                             }
                         }, {
                             kind: "field",
                             key: "_columns",
                             value: function() {
                                 var t = this;
-                                return (0, m.Z)((function(e) {
+                                return (0, w.Z)((function(e) {
                                     return e ? {
                                         name: {
                                             title: t.lcn.localize("entity-id"),
                                             sortable: !0,
                                             direction: "asc",
                                             grows: !0
                                         },
                                         delete: {
                                             title: "",
                                             sortable: !1,
                                             width: "80px",
                                             template: function(e) {
-                                                return (0, g.dy)(i || (i = (0, c.Z)(["\n                  <ha-icon-button\n                    title=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), t.lcn.localize("dashboard-entities-table-delete"), C, (function(n) {
+                                                return (0, m.dy)(i || (i = (0, c.Z)(["\n                  <ha-icon-button\n                    title=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), t.lcn.localize("dashboard-entities-table-delete"), z, (function(n) {
                                                     return t._onEntityDelete(n, e)
                                                 }))
                                             }
                                         }
                                     } : {
                                         name: {
                                             title: t.lcn.localize("entity-id"),
@@ -132,45 +132,45 @@
                                             width: "25%"
                                         },
                                         delete: {
                                             title: "",
                                             sortable: !1,
                                             width: "80px",
                                             template: function(e) {
-                                                return (0, g.dy)(a || (a = (0, c.Z)(["\n                  <ha-icon-button\n                    title=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), t.lcn.localize("dashboard-entities-table-delete"), C, (function(n) {
+                                                return (0, m.dy)(a || (a = (0, c.Z)(["\n                  <ha-icon-button\n                    title=", "\n                    .path=", "\n                    @click=", "\n                  ></ha-icon-button>\n                "])), t.lcn.localize("dashboard-entities-table-delete"), z, (function(n) {
                                                     return t._onEntityDelete(n, e)
                                                 }))
                                             }
                                         }
                                     }
                                 }))
                             }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return (0, g.dy)(r || (r = (0, c.Z)(["\n      <ha-data-table\n        .hass=", "\n        .columns=", "\n        .data=", "\n        .id=", "\n        .noDataText=", "\n        .dir=", "\n        auto-height\n        clickable\n      ></ha-data-table>\n    "])), this.hass, this._columns(this.narrow), this._entities(this.entities), "unique_id", this.lcn.localize("dashboard-entities-table-no-data"), (0, w.Zu)(this.hass))
+                                return (0, m.dy)(s || (s = (0, c.Z)(["\n      <ha-data-table\n        .hass=", "\n        .columns=", "\n        .data=", "\n        .id=", "\n        .noDataText=", "\n        .dir=", "\n        auto-height\n        clickable\n      ></ha-data-table>\n    "])), this.hass, this._columns(this.narrow), this._entities(this.entities), "unique_id", this.lcn.localize("dashboard-entities-table-no-data"), (0, _.Zu)(this.hass))
                             }
                         }, {
                             kind: "method",
                             key: "_onEntityDelete",
                             value: function(t, e) {
                                 t.stopPropagation(), this._deleteEntity(e.address, e.domain, e.resource)
                             }
                         }, {
                             kind: "method",
                             key: "_deleteEntity",
-                            value: (n = (0, l.Z)((0, d.Z)().mark((function t(e, n, i) {
+                            value: (n = (0, h.Z)((0, l.Z)().mark((function t(e, n, i) {
                                 var a;
-                                return (0, d.Z)().wrap((function(t) {
+                                return (0, l.Z)().wrap((function(t) {
                                     for (;;) switch (t.prev = t.next) {
                                         case 0:
                                             return a = this.entities.find((function(t) {
                                                 return t.address[0] === e[0] && t.address[1] === e[1] && t.address[2] === e[2] && t.domain === n && t.resource === i
-                                            })), t.next = 3, (0, _.Ks)(this.hass, this.lcn.host.id, a);
+                                            })), t.next = 3, (0, C.Ks)(this.hass, this.lcn.host.id, a);
                                         case 3:
                                             this.dispatchEvent(new CustomEvent("lcn-configuration-changed", {
                                                 bubbles: !0,
                                                 composed: !0
                                             }));
                                         case 4:
                                         case "end":
@@ -178,33 +178,33 @@
                                     }
                                 }), t, this)
                             }))), function(t, e, i) {
                                 return n.apply(this, arguments)
                             })
                         }]
                     }
-                }), g.oi), n(51358), n(47084), n(5239), n(98490), n(18394)),
+                }), m.oi), n(51358), n(47084), n(5239), n(98490), n(18394)),
                 E = function() {
                     return Promise.all([n.e(597), n.e(587), n.e(812), n.e(719), n.e(925), n.e(527)]).then(n.bind(n, 86527))
                 },
-                z = (0, p.Z)([(0, Z.Mo)("lcn-entities-page")], (function(t, e) {
-                    var n, i, a, r = function(e) {
+                H = (0, k.Z)([(0, Z.Mo)("lcn-entities-page")], (function(t, e) {
+                    var n, i, a, s = function(e) {
                         (0, v.Z)(i, e);
-                        var n = (0, b.Z)(i);
+                        var n = (0, p.Z)(i);
 
                         function i() {
                             var e;
-                            (0, h.Z)(this, i);
-                            for (var a = arguments.length, r = new Array(a), s = 0; s < a; s++) r[s] = arguments[s];
-                            return e = n.call.apply(n, [this].concat(r)), t((0, f.Z)(e)), e
+                            (0, f.Z)(this, i);
+                            for (var a = arguments.length, s = new Array(a), r = 0; r < a; r++) s[r] = arguments[r];
+                            return e = n.call.apply(n, [this].concat(s)), t((0, b.Z)(e)), e
                         }
                         return (0, u.Z)(i)
                     }(e);
                     return {
-                        F: r,
+                        F: s,
                         d: [{
                             kind: "field",
                             decorators: [(0, Z.Cb)({
                                 attribute: !1
                             })],
                             key: "hass",
                             value: void 0
@@ -250,79 +250,85 @@
                             key: "_entityConfigs",
                             value: function() {
                                 return []
                             }
                         }, {
                             kind: "method",
                             key: "firstUpdated",
-                            value: (a = (0, l.Z)((0, d.Z)().mark((function t(e) {
-                                return (0, d.Z)().wrap((function(t) {
+                            value: (a = (0, h.Z)((0, l.Z)().mark((function t(e) {
+                                return (0, l.Z)().wrap((function(t) {
                                     for (;;) switch (t.prev = t.next) {
                                         case 0:
-                                            return (0, k.Z)((0, y.Z)(r.prototype), "firstUpdated", this).call(this, e), E(), t.next = 4, this._fetchEntities(this.lcn.host.id, this.lcn.address);
+                                            return (0, y.Z)((0, g.Z)(s.prototype), "firstUpdated", this).call(this, e), E(), t.next = 4, this._fetchEntities(this.lcn.host.id, this.lcn.address);
                                         case 4:
                                         case "end":
                                             return t.stop()
                                     }
                                 }), t, this)
                             }))), function(t) {
                                 return a.apply(this, arguments)
                             })
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
-                                return this._deviceConfig || 0 !== this._entityConfigs.length ? (0, g.dy)(o || (o = (0, c.Z)(["\n      <hass-tabs-subpage\n        .hass=", "\n        .narrow=", "\n        .route=", '\n        back-path="/lcn/devices"\n        .tabs=', "\n      >\n        <ha-config-section .narrow=", '>\n          <span slot="header"> ', ' </span>\n\n          <span slot="introduction"> ', ' </span>\n\n          <ha-card\n            header="Entities for ', "\n              (", ", ", ",\n              ", ")\n              ", '\n            "\n          >\n            <lcn-entities-data-table\n              .hass=', "\n              .lcn=", "\n              .entities=", "\n              .device=", "\n              .narrow=", "\n              @lcn-configuration-changed=", '\n            ></lcn-entities-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot="fab"\n          @click=', "\n          .label=", '\n          extended\n        >\n          <ha-svg-icon slot="icon" path=', "></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    "])), this.hass, this.narrow, this.route, this.tabs, this.narrow, this.lcn.localize("dashboard-entities-title"), this.lcn.localize("dashboard-entities-introduction"), this._deviceConfig.address[2] ? this.lcn.localize("group") : this.lcn.localize("module"), this.lcn.host.name, this._deviceConfig.address[0], this._deviceConfig.address[1], this._deviceConfig.name ? " - " + this._deviceConfig.name : "", this.hass, this.lcn, this._entityConfigs, this._deviceConfig, this.narrow, this._configurationChanged, this._addEntity, this.lcn.localize("dashboard-entities-add"), "M19,13H13V19H11V13H5V11H11V5H13V11H19V13Z") : (0, g.dy)(s || (s = (0, c.Z)([" <hass-loading-screen></hass-loading-screen> "])))
+                                return this._deviceConfig || 0 !== this._entityConfigs.length ? (0, m.dy)(o || (o = (0, c.Z)(["\n      <hass-tabs-subpage\n        .hass=", "\n        .narrow=", "\n        .route=", "\n        .tabs=", '\n        back-path="/lcn/devices"\n      >\n        <span slot="header"> ', " </span>\n        <ha-config-section .narrow=", '>\n          <span slot="introduction"> ', ' </span>\n\n          <ha-card\n            header="', ":\n              (", ", ", ",\n              ", ")\n              ", '\n            "\n          >\n            <lcn-entities-data-table\n              .hass=', "\n              .lcn=", "\n              .entities=", "\n              .device=", "\n              .narrow=", "\n              @lcn-configuration-changed=", '\n            ></lcn-entities-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot="fab"\n          @click=', "\n          .label=", '\n          extended\n        >\n          <ha-svg-icon slot="icon" path=', "></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    "])), this.hass, this.narrow, this.route, this.tabs, this.lcn.localize("dashboard-entities-title"), this.narrow, this.renderIntro(), this._deviceConfig.address[2] ? this.lcn.localize("dashboard-entities-entities-for-group") : this.lcn.localize("dashboard-entities-entities-for-module"), this.lcn.host.name, this._deviceConfig.address[0], this._deviceConfig.address[1], this._deviceConfig.name ? " - " + this._deviceConfig.name : "", this.hass, this.lcn, this._entityConfigs, this._deviceConfig, this.narrow, this._configurationChanged, this._addEntity, this.lcn.localize("dashboard-entities-add"), "M19,13H13V19H11V13H5V11H11V5H13V11H19V13Z") : (0, m.dy)(r || (r = (0, c.Z)([" <hass-loading-screen></hass-loading-screen> "])))
+                            }
+                        }, {
+                            kind: "method",
+                            key: "renderIntro",
+                            value: function() {
+                                return (0, m.dy)(d || (d = (0, c.Z)(["\n      <h3>", "</h3>\n      <details>\n        <summary>", "</summary>\n        <ul>\n          <li>", "</li>\n          <li>", "</li>\n          <li>", "</li>\n          <li>", "</li>\n          <li>", "</li>\n        </ul>\n      </details>\n    "])), this.lcn.localize("dashboard-entities-introduction"), this.lcn.localize("more-help"), this.lcn.localize("dashboard-entities-introduction-help-1"), this.lcn.localize("dashboard-entities-introduction-help-2"), this.lcn.localize("dashboard-entities-introduction-help-3"), this.lcn.localize("dashboard-entities-introduction-help-4"), this.lcn.localize("dashboard-entities-introduction-help-5"))
                             }
                         }, {
                             kind: "method",
                             key: "_configurationChanged",
                             value: function() {
                                 this._fetchEntities(this.lcn.host.id, this.lcn.address)
                             }
                         }, {
                             kind: "method",
                             key: "_fetchEntities",
-                            value: (i = (0, l.Z)((0, d.Z)().mark((function t(e, n) {
+                            value: (i = (0, h.Z)((0, l.Z)().mark((function t(e, n) {
                                 var i, a;
-                                return (0, d.Z)().wrap((function(t) {
+                                return (0, l.Z)().wrap((function(t) {
                                     for (;;) switch (t.prev = t.next) {
                                         case 0:
-                                            return t.next = 2, (0, _.LO)(this.hass, e);
+                                            return t.next = 2, (0, C.LO)(this.hass, e);
                                         case 2:
                                             return i = t.sent, void 0 !== (a = i.find((function(t) {
                                                 return t.address[0] === n[0] && t.address[1] === n[1] && t.address[2] === n[2]
-                                            }))) && (this._deviceConfig = a), t.next = 7, (0, _.rI)(this.hass, e, n);
+                                            }))) && (this._deviceConfig = a), t.next = 7, (0, C.rI)(this.hass, e, n);
                                         case 7:
                                             this._entityConfigs = t.sent;
                                         case 8:
                                         case "end":
                                             return t.stop()
                                     }
                                 }), t, this)
                             }))), function(t, e) {
                                 return i.apply(this, arguments)
                             })
                         }, {
                             kind: "method",
                             key: "_addEntity",
-                            value: (n = (0, l.Z)((0, d.Z)().mark((function t() {
+                            value: (n = (0, h.Z)((0, l.Z)().mark((function t() {
                                 var e = this;
-                                return (0, d.Z)().wrap((function(t) {
+                                return (0, l.Z)().wrap((function(t) {
                                     for (;;) switch (t.prev = t.next) {
                                         case 0:
                                             n = this, i = {
                                                 lcn: this.lcn,
                                                 device: this._deviceConfig,
                                                 createEntity: function() {
-                                                    var t = (0, l.Z)((0, d.Z)().mark((function t(n) {
-                                                        return (0, d.Z)().wrap((function(t) {
+                                                    var t = (0, h.Z)((0, l.Z)().mark((function t(n) {
+                                                        return (0, l.Z)().wrap((function(t) {
                                                             for (;;) switch (t.prev = t.next) {
                                                                 case 0:
-                                                                    return t.next = 2, (0, _.Ce)(e.hass, e.lcn.host.id, n);
+                                                                    return t.next = 2, (0, C.Ce)(e.hass, e.lcn.host.id, n);
                                                                 case 2:
                                                                     if (!t.sent) {
                                                                         t.next = 6;
                                                                         break
                                                                     }
                                                                     return t.next = 5, e._fetchEntities(e.lcn.host.id, e.lcn.address);
                                                                 case 5:
@@ -351,11 +357,11 @@
                                     var n, i
                                 }), t, this)
                             }))), function() {
                                 return n.apply(this, arguments)
                             })
                         }]
                     }
-                }), g.oi)
+                }), m.oi)
         }
     }
 ]);
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/riIkKI3D.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/m_bQlMKv.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,82 +1,82 @@
-/*! For license information please see riIkKI3D.js.LICENSE.txt */
+/*! For license information please see m_bQlMKv.js.LICENSE.txt */
 "use strict";
 (self.webpackChunklcn_frontend = self.webpackChunklcn_frontend || []).push([
     [244], {
-        9828: function(n, t, e) {
-            e.d(t, {
+        9828: function(n, e, t) {
+            t.d(e, {
                 i: function() {
                     return b
                 }
             });
-            var i, a, o, d = e(33368),
-                r = e(71650),
-                l = e(82390),
-                s = e(69205),
-                c = e(70906),
-                u = e(51565),
-                h = e(34541),
-                p = e(47838),
-                v = e(88962),
-                g = (e(97393), e(91989), e(87762)),
-                f = e(91632),
-                m = e(68144),
-                k = e(73175),
-                y = e(60625),
-                _ = (e(54371), ["button", "ha-list-item"]),
-                b = function(n, t) {
-                    var e;
-                    return (0, m.dy)(i || (i = (0, v.Z)(['\n  <div class="header_title">', "</div>\n  <ha-icon-button\n    .label=", "\n    .path=", '\n    dialogAction="close"\n    class="header_button"\n  ></ha-icon-button>\n'])), t, null !== (e = null == n ? void 0 : n.localize("ui.dialogs.generic.close")) && void 0 !== e ? e : "Close", "M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z")
+            var i, a, o, d = t(33368),
+                r = t(71650),
+                l = t(82390),
+                s = t(69205),
+                c = t(70906),
+                u = t(51565),
+                h = t(34541),
+                p = t(47838),
+                v = t(88962),
+                g = (t(97393), t(91989), t(87762)),
+                f = t(91632),
+                m = t(68144),
+                k = t(73175),
+                y = t(60625),
+                _ = (t(54371), ["button", "ha-list-item"]),
+                b = function(n, e) {
+                    var t;
+                    return (0, m.dy)(i || (i = (0, v.Z)(['\n  <div class="header_title">', "</div>\n  <ha-icon-button\n    .label=", "\n    .path=", '\n    dialogAction="close"\n    class="header_button"\n  ></ha-icon-button>\n'])), e, null !== (t = null == n ? void 0 : n.localize("ui.dialogs.generic.close")) && void 0 !== t ? t : "Close", "M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z")
                 };
-            (0, u.Z)([(0, k.Mo)("ha-dialog")], (function(n, t) {
-                var e = function(t) {
-                    (0, s.Z)(i, t);
-                    var e = (0, c.Z)(i);
+            (0, u.Z)([(0, k.Mo)("ha-dialog")], (function(n, e) {
+                var t = function(e) {
+                    (0, s.Z)(i, e);
+                    var t = (0, c.Z)(i);
 
                     function i() {
-                        var t;
+                        var e;
                         (0, r.Z)(this, i);
                         for (var a = arguments.length, o = new Array(a), d = 0; d < a; d++) o[d] = arguments[d];
-                        return t = e.call.apply(e, [this].concat(o)), n((0, l.Z)(t)), t
+                        return e = t.call.apply(t, [this].concat(o)), n((0, l.Z)(e)), e
                     }
                     return (0, d.Z)(i)
-                }(t);
+                }(e);
                 return {
-                    F: e,
+                    F: t,
                     d: [{
                         kind: "field",
                         key: y.gA,
                         value: void 0
                     }, {
                         kind: "method",
                         key: "scrollToPos",
-                        value: function(n, t) {
-                            var e;
-                            null === (e = this.contentElement) || void 0 === e || e.scrollTo(n, t)
+                        value: function(n, e) {
+                            var t;
+                            null === (t = this.contentElement) || void 0 === t || t.scrollTo(n, e)
                         }
                     }, {
                         kind: "method",
                         key: "renderHeading",
                         value: function() {
-                            return (0, m.dy)(a || (a = (0, v.Z)(['<slot name="heading"> ', " </slot>"])), (0, h.Z)((0, p.Z)(e.prototype), "renderHeading", this).call(this))
+                            return (0, m.dy)(a || (a = (0, v.Z)(['<slot name="heading"> ', " </slot>"])), (0, h.Z)((0, p.Z)(t.prototype), "renderHeading", this).call(this))
                         }
                     }, {
                         kind: "method",
                         key: "firstUpdated",
                         value: function() {
                             var n;
-                            (0, h.Z)((0, p.Z)(e.prototype), "firstUpdated", this).call(this), this.suppressDefaultPressSelector = [this.suppressDefaultPressSelector, _].join(", "), this._updateScrolledAttribute(), null === (n = this.contentElement) || void 0 === n || n.addEventListener("scroll", this._onScroll, {
+                            (0, h.Z)((0, p.Z)(t.prototype), "firstUpdated", this).call(this), this.suppressDefaultPressSelector = [this.suppressDefaultPressSelector, _].join(", "), this._updateScrolledAttribute(), null === (n = this.contentElement) || void 0 === n || n.addEventListener("scroll", this._onScroll, {
                                 passive: !0
                             })
                         }
                     }, {
                         kind: "method",
                         key: "disconnectedCallback",
                         value: function() {
-                            (0, h.Z)((0, p.Z)(e.prototype), "disconnectedCallback", this).call(this), this.contentElement.removeEventListener("scroll", this._onScroll)
+                            (0, h.Z)((0, p.Z)(t.prototype), "disconnectedCallback", this).call(this), this.contentElement.removeEventListener("scroll", this._onScroll)
                         }
                     }, {
                         kind: "field",
                         key: "_onScroll",
                         value: function() {
                             var n = this;
                             return function() {
@@ -96,42 +96,42 @@
                         value: function() {
                             return [f.W, (0, m.iv)(o || (o = (0, v.Z)(["\n      :host([scrolled]) ::slotted(ha-dialog-header) {\n        border-bottom: 1px solid\n          var(--mdc-dialog-scroll-divider-color, rgba(0, 0, 0, 0.12));\n      }\n      .mdc-dialog {\n        --mdc-dialog-scroll-divider-color: var(\n          --dialog-scroll-divider-color,\n          var(--divider-color)\n        );\n        z-index: var(--dialog-z-index, 8);\n        -webkit-backdrop-filter: var(--dialog-backdrop-filter, none);\n        backdrop-filter: var(--dialog-backdrop-filter, none);\n        --mdc-dialog-box-shadow: var(--dialog-box-shadow, none);\n        --mdc-typography-headline6-font-weight: 400;\n        --mdc-typography-headline6-font-size: 1.574rem;\n      }\n      .mdc-dialog__actions {\n        justify-content: var(--justify-action-buttons, flex-end);\n        padding-bottom: max(env(safe-area-inset-bottom), 24px);\n      }\n      .mdc-dialog__actions span:nth-child(1) {\n        flex: var(--secondary-action-button-flex, unset);\n      }\n      .mdc-dialog__actions span:nth-child(2) {\n        flex: var(--primary-action-button-flex, unset);\n      }\n      .mdc-dialog__container {\n        align-items: var(--vertical-align-dialog, center);\n      }\n      .mdc-dialog__title {\n        padding: 24px 24px 0 24px;\n        text-overflow: ellipsis;\n        overflow: hidden;\n      }\n      .mdc-dialog__actions {\n        padding: 12px 24px 12px 24px;\n      }\n      .mdc-dialog__title::before {\n        display: block;\n        height: 0px;\n      }\n      .mdc-dialog .mdc-dialog__content {\n        position: var(--dialog-content-position, relative);\n        padding: var(--dialog-content-padding, 24px);\n      }\n      :host([hideactions]) .mdc-dialog .mdc-dialog__content {\n        padding-bottom: max(\n          var(--dialog-content-padding, 24px),\n          env(safe-area-inset-bottom)\n        );\n      }\n      .mdc-dialog .mdc-dialog__surface {\n        position: var(--dialog-surface-position, relative);\n        top: var(--dialog-surface-top);\n        margin-top: var(--dialog-surface-margin-top);\n        min-height: var(--mdc-dialog-min-height, auto);\n        border-radius: var(--ha-dialog-border-radius, 28px);\n      }\n      :host([flexContent]) .mdc-dialog .mdc-dialog__content {\n        display: flex;\n        flex-direction: column;\n      }\n      .header_title {\n        margin-right: 32px;\n        margin-inline-end: 32px;\n        margin-inline-start: initial;\n        direction: var(--direction);\n      }\n      .header_button {\n        position: absolute;\n        right: 16px;\n        top: 14px;\n        text-decoration: none;\n        color: inherit;\n        inset-inline-start: initial;\n        inset-inline-end: 16px;\n        direction: var(--direction);\n      }\n      .dialog-actions {\n        inset-inline-start: initial !important;\n        inset-inline-end: 0px !important;\n        direction: var(--direction);\n      }\n    "])))]
                         }
                     }]
                 }
             }), g.M)
         },
-        48950: function(n, t, e) {
-            var i, a = e(88962),
-                o = e(33368),
-                d = e(71650),
-                r = e(82390),
-                l = e(69205),
-                s = e(70906),
-                c = e(51565),
-                u = (e(97393), e(8485)),
-                h = e(92038),
-                p = e(68144),
-                v = e(73175),
-                g = e(18394);
-            (0, c.Z)([(0, v.Mo)("ha-formfield")], (function(n, t) {
-                var e = function(t) {
-                    (0, l.Z)(i, t);
-                    var e = (0, s.Z)(i);
+        48950: function(n, e, t) {
+            var i, a = t(88962),
+                o = t(33368),
+                d = t(71650),
+                r = t(82390),
+                l = t(69205),
+                s = t(70906),
+                c = t(51565),
+                u = (t(97393), t(8485)),
+                h = t(92038),
+                p = t(68144),
+                v = t(73175),
+                g = t(18394);
+            (0, c.Z)([(0, v.Mo)("ha-formfield")], (function(n, e) {
+                var t = function(e) {
+                    (0, l.Z)(i, e);
+                    var t = (0, s.Z)(i);
 
                     function i() {
-                        var t;
+                        var e;
                         (0, d.Z)(this, i);
                         for (var a = arguments.length, o = new Array(a), l = 0; l < a; l++) o[l] = arguments[l];
-                        return t = e.call.apply(e, [this].concat(o)), n((0, r.Z)(t)), t
+                        return e = t.call.apply(t, [this].concat(o)), n((0, r.Z)(e)), e
                     }
                     return (0, o.Z)(i)
-                }(t);
+                }(e);
                 return {
-                    F: e,
+                    F: t,
                     d: [{
                         kind: "method",
                         key: "_labelClick",
                         value: function() {
                             var n = this.input;
                             if (n && (n.focus(), !n.disabled)) switch (n.tagName) {
                                 case "HA-CHECKBOX":
@@ -151,95 +151,95 @@
                         value: function() {
                             return [h.W, (0, p.iv)(i || (i = (0, a.Z)(["\n      :host(:not([alignEnd])) ::slotted(ha-switch) {\n        margin-right: 10px;\n        margin-inline-end: 10px;\n        margin-inline-start: inline;\n      }\n      .mdc-form-field > label {\n        direction: var(--direction);\n        margin-inline-start: 0;\n        margin-inline-end: auto;\n        padding-inline-start: 4px;\n        padding-inline-end: 0;\n      }\n    "])))]
                         }
                     }]
                 }
             }), u.a)
         },
-        19096: function(n, t, e) {
-            var i, a = e(88962),
-                o = e(33368),
-                d = e(71650),
-                r = e(82390),
-                l = e(69205),
-                s = e(70906),
-                c = e(51565),
-                u = (e(97393), e(57463)),
-                h = e(44973),
-                p = e(68144),
-                v = e(73175);
-            (0, c.Z)([(0, v.Mo)("ha-radio")], (function(n, t) {
-                var e = function(t) {
-                    (0, l.Z)(i, t);
-                    var e = (0, s.Z)(i);
+        19096: function(n, e, t) {
+            var i, a = t(88962),
+                o = t(33368),
+                d = t(71650),
+                r = t(82390),
+                l = t(69205),
+                s = t(70906),
+                c = t(51565),
+                u = (t(97393), t(57463)),
+                h = t(44973),
+                p = t(68144),
+                v = t(73175);
+            (0, c.Z)([(0, v.Mo)("ha-radio")], (function(n, e) {
+                var t = function(e) {
+                    (0, l.Z)(i, e);
+                    var t = (0, s.Z)(i);
 
                     function i() {
-                        var t;
+                        var e;
                         (0, d.Z)(this, i);
                         for (var a = arguments.length, o = new Array(a), l = 0; l < a; l++) o[l] = arguments[l];
-                        return t = e.call.apply(e, [this].concat(o)), n((0, r.Z)(t)), t
+                        return e = t.call.apply(t, [this].concat(o)), n((0, r.Z)(e)), e
                     }
                     return (0, o.Z)(i)
-                }(t);
+                }(e);
                 return {
-                    F: e,
+                    F: t,
                     d: [{
                         kind: "field",
                         static: !0,
                         key: "styles",
                         value: function() {
                             return [h.W, (0, p.iv)(i || (i = (0, a.Z)(["\n      :host {\n        --mdc-theme-secondary: var(--primary-color);\n      }\n    "])))]
                         }
                     }]
                 }
             }), u.J)
         },
-        77044: function(n, t, e) {
-            e.r(t), e.d(t, {
+        77044: function(n, e, t) {
+            t.r(e), t.d(e, {
                 CreateDeviceDialog: function() {
                     return I
                 }
             });
-            var i, a = e(88962),
-                o = e(99312),
-                d = e(81043),
-                r = e(33368),
-                l = e(71650),
-                s = e(82390),
-                c = e(69205),
-                u = e(70906),
-                h = e(51565),
-                p = e(34541),
-                v = e(47838),
-                g = (e(97393), e(46798), e(94570), e(40643), e(65660), e(71132)),
-                f = e(50856);
+            var i, a = t(88962),
+                o = t(99312),
+                d = t(81043),
+                r = t(33368),
+                l = t(71650),
+                s = t(82390),
+                c = t(69205),
+                u = t(70906),
+                h = t(51565),
+                p = t(34541),
+                v = t(47838),
+                g = (t(97393), t(46798), t(94570), t(40643), t(65660), t(71132)),
+                f = t(50856);
             (0, g.k)({
                 _template: (0, f.d)(i || (i = (0, a.Z)(["\n    <style>\n\n      :host {\n        @apply --layout-horizontal;\n        @apply --layout-center;\n        position: relative;\n        height: 64px;\n        padding: 0 16px;\n        pointer-events: none;\n        font-size: var(--app-toolbar-font-size, 20px);\n      }\n\n      :host ::slotted(*) {\n        pointer-events: auto;\n      }\n\n      :host ::slotted(paper-icon-button) {\n        /* paper-icon-button/issues/33 */\n        font-size: 0;\n      }\n\n      :host ::slotted([main-title]),\n      :host ::slotted([condensed-title]) {\n        pointer-events: none;\n        @apply --layout-flex;\n      }\n\n      :host ::slotted([bottom-item]) {\n        position: absolute;\n        right: 0;\n        bottom: 0;\n        left: 0;\n      }\n\n      :host ::slotted([top-item]) {\n        position: absolute;\n        top: 0;\n        right: 0;\n        left: 0;\n      }\n\n      :host ::slotted([spacer]) {\n        margin-left: 64px;\n      }\n    </style>\n\n    <slot></slot>\n"]))),
                 is: "app-toolbar"
             });
-            e(54371), e(19096), e(48950), e(51520);
-            var m, k, y = e(18394),
-                _ = e(68144),
-                b = e(73175),
-                x = e(9828),
-                Z = e(29950),
-                w = e(58361),
-                I = (0, h.Z)([(0, b.Mo)("lcn-create-device-dialog")], (function(n, t) {
-                    var e, i, h = function(t) {
-                        (0, c.Z)(i, t);
-                        var e = (0, u.Z)(i);
+            t(54371), t(19096), t(48950), t(51520);
+            var m, k, y = t(18394),
+                _ = t(68144),
+                b = t(73175),
+                x = t(9828),
+                Z = t(29950),
+                w = t(58361),
+                I = (0, h.Z)([(0, b.Mo)("lcn-create-device-dialog")], (function(n, e) {
+                    var t, i, h = function(e) {
+                        (0, c.Z)(i, e);
+                        var t = (0, u.Z)(i);
 
                         function i() {
-                            var t;
+                            var e;
                             (0, l.Z)(this, i);
                             for (var a = arguments.length, o = new Array(a), d = 0; d < a; d++) o[d] = arguments[d];
-                            return t = e.call.apply(e, [this].concat(o)), n((0, s.Z)(t)), t
+                            return e = t.call.apply(t, [this].concat(o)), n((0, s.Z)(e)), e
                         }
                         return (0, r.Z)(i)
-                    }(t);
+                    }(e);
                     return {
                         F: h,
                         d: [{
                             kind: "field",
                             decorators: [(0, b.Cb)({
                                 attribute: !1
                             })],
@@ -276,26 +276,27 @@
                             decorators: [(0, b.SB)()],
                             key: "_addressId",
                             value: function() {
                                 return 5
                             }
                         }, {
                             kind: "field",
+                            decorators: [(0, b.SB)()],
                             key: "_invalid",
                             value: function() {
                                 return !1
                             }
                         }, {
                             kind: "method",
                             key: "showDialog",
-                            value: (i = (0, d.Z)((0, o.Z)().mark((function n(t) {
+                            value: (i = (0, d.Z)((0, o.Z)().mark((function n(e) {
                                 return (0, o.Z)().wrap((function(n) {
                                     for (;;) switch (n.prev = n.next) {
                                         case 0:
-                                            return this._params = t, this.lcn = t.lcn, n.next = 4, this.updateComplete;
+                                            return this._params = e, this.lcn = e.lcn, n.next = 4, this.updateComplete;
                                         case 4:
                                         case "end":
                                             return n.stop()
                                     }
                                 }), n, this)
                             }))), function(n) {
                                 return i.apply(this, arguments)
@@ -306,15 +307,15 @@
                             value: function(n) {
                                 (0, p.Z)((0, v.Z)(h.prototype), "firstUpdated", this).call(this, n), (0, w.z)()
                             }
                         }, {
                             kind: "method",
                             key: "willUpdate",
                             value: function(n) {
-                                (0, p.Z)((0, v.Z)(h.prototype), "willUpdate", this).call(this, n), this._invalid = !this._validateSegmentId(this._segmentId) || !this._validateAddressId(this._addressId, this._isGroup)
+                                n.has("_invalid") && (this._invalid = !this._validateSegmentId(this._segmentId) || !this._validateAddressId(this._addressId, this._isGroup))
                             }
                         }, {
                             kind: "method",
                             key: "render",
                             value: function() {
                                 return this._params ? (0, _.dy)(m || (m = (0, a.Z)(["\n      <ha-dialog\n        open\n        scrimClickAction\n        escapeKeyAction\n        .heading=", "\n        @closed=", '\n      >\n        <div id="type">', "</div>\n\n        <ha-formfield label=", '>\n          <ha-radio\n            name="is_group"\n            value="module"\n            .checked=', "\n            @change=", "\n          ></ha-radio>\n        </ha-formfield>\n\n        <ha-formfield label=", '>\n          <ha-radio\n            name="is_group"\n            value="group"\n            .checked=', "\n            @change=", "\n          ></ha-radio>\n        </ha-formfield>\n\n        <ha-textfield\n          .label=", '\n          type="number"\n          .value=', '\n          min="0"\n          required\n          autoValidate\n          @input=', "\n          .validityTransform=", "\n          .validationMessage=", "\n        ></ha-textfield>\n\n        <ha-textfield\n          .label=", '\n          type="number"\n          .value=', '\n          min="0"\n          required\n          autoValidate\n          @input=', "\n          .validityTransform=", "\n          .validationMessage=", '\n        ></ha-textfield>\n\n        <div class="buttons">\n          <mwc-button\n            slot="secondaryAction"\n            @click=', "\n            .label=", '\n          ></mwc-button>\n\n          <mwc-button\n            slot="primaryAction"\n            @click=', "\n            .disabled=", "\n            .label=", "\n          ></mwc-button>\n        </div>\n      </ha-dialog>\n    "])), (0, x.i)(this.hass, this.lcn.localize("dashboard-devices-dialog-create-title")), this._closeDialog, this.lcn.localize("type"), this.lcn.localize("module"), !1 === this._isGroup, this._isGroupChanged, this.lcn.localize("group"), !0 === this._isGroup, this._isGroupChanged, this.lcn.localize("segment-id"), this._segmentId.toString(), this._segmentIdChanged, this._validityTransformSegmentId, this.lcn.localize("dashboard-devices-dialog-error-segment"), this.lcn.localize("id"), this._addressId.toString(), this._addressIdChanged, this._validityTransformAddressId, this._isGroup ? this.lcn.localize("dashboard-devices-dialog-error-group") : this.lcn.localize("dashboard-devices-dialog-error-module"), this._closeDialog, this.lcn.localize("dismiss"), this._create, this._invalid, this.lcn.localize("create")) : _.Ld
                             }
@@ -324,79 +325,79 @@
                             value: function(n) {
                                 this._isGroup = "group" === n.target.value
                             }
                         }, {
                             kind: "method",
                             key: "_segmentIdChanged",
                             value: function(n) {
-                                var t = n.target;
-                                this._segmentId = +t.value
+                                var e = n.target;
+                                this._segmentId = +e.value
                             }
                         }, {
                             kind: "method",
                             key: "_addressIdChanged",
                             value: function(n) {
-                                var t = n.target;
-                                this._addressId = +t.value
+                                var e = n.target;
+                                this._addressId = +e.value
                             }
                         }, {
                             kind: "method",
                             key: "_validateSegmentId",
                             value: function(n) {
                                 return 0 === n || n >= 5 && n <= 128
                             }
                         }, {
                             kind: "method",
                             key: "_validateAddressId",
-                            value: function(n, t) {
+                            value: function(n, e) {
                                 return n >= 5 && n <= 254
                             }
                         }, {
                             kind: "get",
                             key: "_validityTransformSegmentId",
                             value: function() {
                                 var n = this;
-                                return function(t) {
+                                return function(e) {
                                     return {
-                                        valid: n._validateSegmentId(+t)
+                                        valid: n._validateSegmentId(+e)
                                     }
                                 }
                             }
                         }, {
                             kind: "get",
                             key: "_validityTransformAddressId",
                             value: function() {
                                 var n = this;
-                                return function(t) {
+                                return function(e) {
                                     return {
-                                        valid: n._validateAddressId(+t, n._isGroup)
+                                        valid: n._validateAddressId(+e, n._isGroup)
                                     }
                                 }
                             }
                         }, {
                             kind: "method",
                             key: "_create",
-                            value: (e = (0, d.Z)((0, o.Z)().mark((function n() {
-                                var t;
+                            value: (t = (0, d.Z)((0, o.Z)().mark((function n() {
+                                var e;
                                 return (0, o.Z)().wrap((function(n) {
                                     for (;;) switch (n.prev = n.next) {
                                         case 0:
-                                            return t = {
+                                            return e = {
                                                 name: "",
                                                 address: [this._segmentId, this._addressId, this._isGroup]
-                                            }, n.next = 3, this._params.createDevice(t);
+                                            }, n.next = 3, this._params.createDevice(e);
                                         case 3:
                                             this._closeDialog();
                                         case 4:
                                         case "end":
                                             return n.stop()
                                     }
                                 }), n, this)
                             }))), function() {
-                                return e.apply(this, arguments)
+                                return t.apply(this, arguments)
                             })
                         }, {
                             kind: "method",
                             key: "_closeDialog",
                             value: function() {
                                 this._params = void 0, (0, y.B)(this, "dialog-closed", {
                                     dialog: this.localName
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/xK5ZNMm1.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/xK5ZNMm1.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/xK5ZNMm1.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/xK5ZNMm1.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/xK5ZNMm1.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/xK5ZNMm1.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ye57YhXr.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ye57YhXr.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_es5/ye57YhXr.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_es5/ye57YhXr.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/AuN1Wwjr.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/AuN1Wwjr.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/AuN1Wwjr.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/AuN1Wwjr.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/CHsIPDL8.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/CHsIPDL8.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/CHsIPDL8.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/CHsIPDL8.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/CHsIPDL8.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/CHsIPDL8.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/HyurOyWN.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/HyurOyWN.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/JAAifVse.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/JAAifVse.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/JAAifVse.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/JAAifVse.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/PHB24J1t.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/PHB24J1t.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/PHB24J1t.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/PHB24J1t.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/R9L2-V1R.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/gwnfZ3wa.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
-export const id = 540;
-export const ids = [540];
+export const id = 770;
+export const ids = [770];
 export const modules = {
     2136: (e, t, a) => {
         a.d(t, {
             i: () => i
         });
         const o = ((e, t, a = !0, o = !0) => {
                 let i, r = 0;
@@ -181,15 +181,15 @@
         var o = a(309),
             i = a(4541),
             r = a(7838),
             n = a(8095),
             s = a(2477),
             d = a(4243),
             l = a(8144),
-            c = a(2138);
+            h = a(2138);
         (0, o.Z)([(0, d.Mo)("ha-fab")], (function(e, t) {
             class a extends t {
                 constructor(...t) {
                     super(...t), e(this)
                 }
             }
             return {
@@ -207,15 +207,15 @@
                     value() {
                         return [s.W, l.iv`
       :host .mdc-fab--extended .mdc-fab__icon {
         margin-inline-start: -8px;
         margin-inline-end: 12px;
         direction: var(--direction);
       }
-    `, "rtl" === c.E.document.dir ? l.iv`
+    `, "rtl" === h.E.document.dir ? l.iv`
           :host .mdc-fab--extended .mdc-fab__icon {
             direction: rtl;
           }
         ` : l.iv``]
                     }
                 }]
             }
@@ -225,16 +225,16 @@
         var o = a(309),
             i = a(4541),
             r = a(7838),
             n = (a(7763), a(8144)),
             s = a(4243),
             d = a(3448),
             l = a(4516);
-        var c = a(2136),
-            h = a(1750),
+        var h = a(2136),
+            c = a(1750),
             p = (a(3358), a(3957), a(7662), a(8734)),
             u = a(153);
         (0, o.Z)([(0, s.Mo)("ha-tab")], (function(e, t) {
             return {
                 F: class extends t {
                     constructor(...t) {
                         super(...t), e(this)
@@ -509,15 +509,15 @@
                 }, {
                     kind: "field",
                     decorators: [(0, s.SB)()],
                     key: "_activeTab",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, c.i)(".content")],
+                    decorators: [(0, h.i)(".content")],
                     key: "_savedScrollPos",
                     value: void 0
                 }, {
                     kind: "field",
                     key: "_getTabs",
                     value() {
                         return (0, l.Z)(((e, t, a, o, i, r, s) => {
@@ -551,15 +551,15 @@
                     }
                 }, {
                     kind: "method",
                     key: "willUpdate",
                     value: function(e) {
                         if (e.has("route") && (this._activeTab = this.tabs.find((e => `${this.route.prefix}${this.route.path}`.includes(e.path)))), e.has("hass")) {
                             const t = e.get("hass");
-                            t && t.language === this.hass.language || (this.rtl = (0, h.HE)(this.hass))
+                            t && t.language === this.hass.language || (this.rtl = (0, c.HE)(this.hass))
                         }(0, i.Z)((0, r.Z)(a.prototype), "willUpdate", this).call(this, e)
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
                         var e, t;
@@ -920,64 +920,10 @@
         flex-direction: column;
       }
     `
                     }
                 }]
             }
         }), i.oi)
-    },
-    9051: (e, t, a) => {
-        a.d(t, {
-            Ce: () => s,
-            Ks: () => d,
-            LO: () => i,
-            S6: () => l,
-            V5: () => o,
-            Vy: () => n,
-            n1: () => c,
-            rI: () => r
-        });
-        const o = e => e.callWS({
-                type: "lcn/hosts"
-            }),
-            i = (e, t) => e.callWS({
-                type: "lcn/devices",
-                host_id: t
-            }),
-            r = (e, t, a) => e.callWS({
-                type: "lcn/entities",
-                host_id: t,
-                address: a
-            }),
-            n = (e, t) => e.callWS({
-                type: "lcn/devices/scan",
-                host_id: t
-            }),
-            s = (e, t, a) => e.callWS({
-                type: "lcn/entities/add",
-                host_id: t,
-                address: a.address,
-                name: a.name,
-                domain: a.domain,
-                domain_data: a.domain_data
-            }),
-            d = (e, t, a) => e.callWS({
-                type: "lcn/entities/delete",
-                host_id: t,
-                address: a.address,
-                domain: a.domain,
-                resource: a.resource
-            }),
-            l = (e, t, a) => e.callWS({
-                type: "lcn/devices/add",
-                host_id: t,
-                address: a.address,
-                name: a.name
-            }),
-            c = (e, t, a) => e.callWS({
-                type: "lcn/devices/delete",
-                host_id: t,
-                address: a.address
-            })
     }
 };
-//# sourceMappingURL=R9L2-V1R.js.map
+//# sourceMappingURL=gwnfZ3wa.js.map
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/R9L2-V1R.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/gwnfZ3wa.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'gwnfZ3wa.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "R9L2-V1R.js",
+    "file": "gwnfZ3wa.js",
     "mappings": ";;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsEA;AAIA;;AAKA;;;;;;ACxDA;;;;AAKA;;;;ACEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAiFA;AChCA;;AAEA;AACA;AACA;AACA;;AAIA;;AAGA;AACA;;;AAIA;;AAmCA;;AAGA;AACA;AACA;;AAEA;AAGA;;AAEA;;;AAGA;;AAGA;AACA;;;AAGA;AAEA;AACA;AAEA;AAEA;AACA;;AAEA;;;;;;AAOA;AACA;;;;AAIA;;;AAIA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA4JA;;ACjVA;;;;AAOA;;;;;;AAWA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA4FA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-card.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-fab.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-tab.ts",
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/SaPEbRz1.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/SaPEbRz1.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/SaPEbRz1.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/SaPEbRz1.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/SaPEbRz1.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/SaPEbRz1.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/X5sZzGl8.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/X5sZzGl8.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/X5sZzGl8.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/X5sZzGl8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/X5sZzGl8.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/X5sZzGl8.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/ZRpJZyXB.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ZRpJZyXB.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/ZRpJZyXB.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ZRpJZyXB.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/ZRpJZyXB.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ZRpJZyXB.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bZayZmh0.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/Ntga-_EF.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -4,58 +4,58 @@
     981: (t, e, i) => {
         i.r(e), i.d(e, {
             LCNEntitiesPage: () => f
         });
         var s = i(309),
             a = i(4541),
             n = i(7838),
-            d = i(8144),
-            o = i(4243),
+            o = i(8144),
+            d = i(4243),
             l = (i(657), i(1952), i(4776), i(8336), i(7662), i(9040), i(4371), i(4516)),
             r = i(1750),
             c = i(9051);
         const h = "M19,4H15.5L14.5,3H9.5L8.5,4H5V6H19M6,19A2,2 0 0,0 8,21H16A2,2 0 0,0 18,19V7H6V19Z";
-        (0, s.Z)([(0, o.Mo)("lcn-entities-data-table")], (function(t, e) {
+        (0, s.Z)([(0, d.Mo)("lcn-entities-data-table")], (function(t, e) {
             return {
                 F: class extends e {
                     constructor(...e) {
                         super(...e), t(this)
                     }
                 },
                 d: [{
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "hass",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "lcn",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "narrow",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "device",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "entities",
                     value() {
                         return []
                     }
                 }, {
@@ -78,15 +78,15 @@
                                 direction: "asc",
                                 grows: !0
                             },
                             delete: {
                                 title: "",
                                 sortable: !1,
                                 width: "80px",
-                                template: t => d.dy`
+                                template: t => o.dy`
                   <ha-icon-button
                     title=${this.lcn.localize("dashboard-entities-table-delete")}
                     .path=${h}
                     @click=${e=>this._onEntityDelete(e,t)}
                   ></ha-icon-button>
                 `
                             }
@@ -110,29 +110,29 @@
                                 grows: !1,
                                 width: "25%"
                             },
                             delete: {
                                 title: "",
                                 sortable: !1,
                                 width: "80px",
-                                template: t => d.dy`
+                                template: t => o.dy`
                   <ha-icon-button
                     title=${this.lcn.localize("dashboard-entities-table-delete")}
                     .path=${h}
                     @click=${e=>this._onEntityDelete(e,t)}
                   ></ha-icon-button>
                 `
                             }
                         }))
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
-                        return d.dy`
+                        return o.dy`
       <ha-data-table
         .hass=${this.hass}
         .columns=${this._columns(this.narrow)}
         .data=${this._entities(this.entities)}
         .id=${"unique_id"}
         .noDataText=${this.lcn.localize("dashboard-entities-table-no-data")}
         .dir=${(0,r.Zu)(this.hass)}
@@ -155,100 +155,99 @@
                         await (0, c.Ks)(this.hass, this.lcn.host.id, s), this.dispatchEvent(new CustomEvent("lcn-configuration-changed", {
                             bubbles: !0,
                             composed: !0
                         }))
                     }
                 }]
             }
-        }), d.oi);
+        }), o.oi);
         var u = i(8394);
         const b = () => Promise.all([i.e(597), i.e(321), i.e(812), i.e(719), i.e(527)]).then(i.bind(i, 6527));
-        let f = (0, s.Z)([(0, o.Mo)("lcn-entities-page")], (function(t, e) {
+        let f = (0, s.Z)([(0, d.Mo)("lcn-entities-page")], (function(t, e) {
             class i extends e {
                 constructor(...e) {
                     super(...e), t(this)
                 }
             }
             return {
                 F: i,
                 d: [{
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "hass",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "lcn",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "narrow",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         attribute: !1
                     })],
                     key: "route",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.Cb)({
+                    decorators: [(0, d.Cb)({
                         type: Array,
                         reflect: !1
                     })],
                     key: "tabs",
                     value() {
                         return []
                     }
                 }, {
                     kind: "field",
-                    decorators: [(0, o.SB)()],
+                    decorators: [(0, d.SB)()],
                     key: "_deviceConfig",
                     value: void 0
                 }, {
                     kind: "field",
-                    decorators: [(0, o.SB)()],
+                    decorators: [(0, d.SB)()],
                     key: "_entityConfigs",
                     value() {
                         return []
                     }
                 }, {
                     kind: "method",
                     key: "firstUpdated",
                     value: async function(t) {
                         (0, a.Z)((0, n.Z)(i.prototype), "firstUpdated", this).call(this, t), b(), await this._fetchEntities(this.lcn.host.id, this.lcn.address)
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
-                        return this._deviceConfig || 0 !== this._entityConfigs.length ? d.dy`
+                        return this._deviceConfig || 0 !== this._entityConfigs.length ? o.dy`
       <hass-tabs-subpage
         .hass=${this.hass}
         .narrow=${this.narrow}
         .route=${this.route}
-        back-path="/lcn/devices"
         .tabs=${this.tabs}
+        back-path="/lcn/devices"
       >
+        <span slot="header"> ${this.lcn.localize("dashboard-entities-title")} </span>
         <ha-config-section .narrow=${this.narrow}>
-          <span slot="header"> ${this.lcn.localize("dashboard-entities-title")} </span>
-
-          <span slot="introduction"> ${this.lcn.localize("dashboard-entities-introduction")} </span>
+          <span slot="introduction"> ${this.renderIntro()} </span>
 
           <ha-card
-            header="Entities for ${this._deviceConfig.address[2]?this.lcn.localize("group"):this.lcn.localize("module")}
+            header="${this._deviceConfig.address[2]?this.lcn.localize("dashboard-entities-entities-for-group"):this.lcn.localize("dashboard-entities-entities-for-module")}:
               (${this.lcn.host.name}, ${this._deviceConfig.address[0]},
               ${this._deviceConfig.address[1]})
               ${this._deviceConfig.name?" - "+this._deviceConfig.name:""}
             "
           >
             <lcn-entities-data-table
               .hass=${this.hass}
@@ -265,15 +264,33 @@
           @click=${this._addEntity}
           .label=${this.lcn.localize("dashboard-entities-add")}
           extended
         >
           <ha-svg-icon slot="icon" path=${"M19,13H13V19H11V13H5V11H11V5H13V11H19V13Z"}></ha-svg-icon>
         </ha-fab>
       </hass-tabs-subpage>
-    ` : d.dy` <hass-loading-screen></hass-loading-screen> `
+    ` : o.dy` <hass-loading-screen></hass-loading-screen> `
+                    }
+                }, {
+                    kind: "method",
+                    key: "renderIntro",
+                    value: function() {
+                        return o.dy`
+      <h3>${this.lcn.localize("dashboard-entities-introduction")}</h3>
+      <details>
+        <summary>${this.lcn.localize("more-help")}</summary>
+        <ul>
+          <li>${this.lcn.localize("dashboard-entities-introduction-help-1")}</li>
+          <li>${this.lcn.localize("dashboard-entities-introduction-help-2")}</li>
+          <li>${this.lcn.localize("dashboard-entities-introduction-help-3")}</li>
+          <li>${this.lcn.localize("dashboard-entities-introduction-help-4")}</li>
+          <li>${this.lcn.localize("dashboard-entities-introduction-help-5")}</li>
+        </ul>
+      </details>
+    `
                     }
                 }, {
                     kind: "method",
                     key: "_configurationChanged",
                     value: function() {
                         this._fetchEntities(this.lcn.host.id, this.lcn.address)
                     }
@@ -297,11 +314,11 @@
                             dialogTag: "lcn-create-entity-dialog",
                             dialogImport: b,
                             dialogParams: e
                         })
                     }
                 }]
             }
-        }), d.oi)
+        }), o.oi)
     }
 };
-//# sourceMappingURL=bZayZmh0.js.map
+//# sourceMappingURL=Ntga-_EF.js.map
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bZayZmh0.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/Ntga-_EF.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238094%*

 * *Differences: {"'file'": "'Ntga-_EF.js'",*

 * * "'mappings'": "';;AAuDA;AACA;AAJA;;AAUA;;AA6BA;AACA;AAJA;;AAWA;;AAKA;AACA;AACA;AACA;AACA;AACA;;;;AAKA;;AC3DA;AACA;AACA;AACA;;;AAGA;AACA;AACA;;;AAGA;AAGA;AACA;AACA;;;;AAIA;AACA;AACA;AACA;AACA;AACA;;;;;;AAMA;AACA;;;AAtFA;;;AAkDA;AA+CA;;AAEA;;AAEA;AACA;AACA;AACA;AACA;;;AAIA'",*

 * * "'sourcesContent'": "{insert: [(1, 'import { html, LitElement, TemplateResult } from "*

 * *                     '"lit";\\nimport { customElement, property, state } from '*

 * *                     '"lit/decorators";\ […]*

```diff
@@ -1,15 +1,15 @@
 {
-    "file": "bZayZmh0.js",
-    "mappings": ";;AAuDA;AACA;AAJA;;AAUA;;AA6BA;AACA;AAJA;;AAWA;;AAKA;AACA;AACA;AACA;AACA;AACA;;;;AAKA;;AC3DA;AACA;AACA;;AAEA;;AAEA;AACA;;AAEA;;;AAGA;AAGA;AACA;AACA;;;;AAIA;AACA;AACA;AACA;AACA;AACA;;;;;;AAMA;AACA;;;AAvFA;;;AAkDA",
+    "file": "Ntga-_EF.js",
+    "mappings": ";;AAuDA;AACA;AAJA;;AAUA;;AA6BA;AACA;AAJA;;AAWA;;AAKA;AACA;AACA;AACA;AACA;AACA;;;;AAKA;;AC3DA;AACA;AACA;AACA;;;AAGA;AACA;AACA;;;AAGA;AAGA;AACA;AACA;;;;AAIA;AACA;AACA;AACA;AACA;AACA;;;;;;AAMA;AACA;;;AAtFA;;;AAkDA;AA+CA;;AAEA;;AAEA;AACA;AACA;AACA;AACA;;;AAIA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://lcn-frontend/./src/lcn-entities-data-table.ts",
         "webpack://lcn-frontend/./src/lcn-entities-page.ts"
     ],
     "sourcesContent": [
         "import \"@ha/components/ha-icon-button\";\nimport { html, LitElement } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\nimport memoizeOne from \"memoize-one\";\nimport { mdiDelete } from \"@mdi/js\";\nimport { computeRTLDirection } from \"@ha/common/util/compute_rtl\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport { LCN, LcnEntityConfig, deleteEntity, LcnDeviceConfig, LcnAddress } from \"types/lcn\";\nimport {\n  DataTableColumnContainer,\n  DataTableRowData,\n} from \"@ha/components/data-table/ha-data-table\";\n\nexport type EntityRowData = LcnEntityConfig & {\n  delete: LcnEntityConfig;\n};\n\n@customElement(\"lcn-entities-data-table\")\nexport class LCNEntitiesDataTable extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public narrow!: boolean;\n\n  @property({ attribute: false }) public device!: LcnDeviceConfig;\n\n  @property({ attribute: false }) public entities: LcnEntityConfig[] = [];\n\n  private _entities = memoizeOne((entities: LcnEntityConfig[]) => {\n    const entityRowData: EntityRowData[] = entities.map((entity) => ({\n      ...entity,\n      delete: entity,\n    }));\n    return entityRowData;\n  });\n\n  private _columns = memoizeOne(\n    (narrow: boolean): DataTableColumnContainer =>\n      narrow\n        ? {\n            name: {\n              title: this.lcn.localize(\"entity-id\"),\n              sortable: true,\n              direction: \"asc\",\n              grows: true,\n            },\n            delete: {\n              title: \"\",\n              sortable: false,\n              width: \"80px\",\n              template: (entity: LcnEntityConfig) => {\n                const handler = (ev) => this._onEntityDelete(ev, entity);\n                return html`\n                  <ha-icon-button\n                    title=${this.lcn.localize(\"dashboard-entities-table-delete\")}\n                    .path=${mdiDelete}\n                    @click=${handler}\n                  ></ha-icon-button>\n                `;\n              },\n            },\n          }\n        : {\n            name: {\n              title: this.lcn.localize(\"entity-id\"),\n              sortable: true,\n              direction: \"asc\",\n              grows: true,\n              width: \"35%\",\n            },\n            domain: {\n              title: this.lcn.localize(\"domain\"),\n              sortable: true,\n              grows: false,\n              width: \"25%\",\n            },\n            resource: {\n              title: this.lcn.localize(\"resource\"),\n              sortable: true,\n              grows: false,\n              width: \"25%\",\n            },\n            delete: {\n              title: \"\",\n              sortable: false,\n              width: \"80px\",\n              template: (entity: LcnEntityConfig) => {\n                const handler = (ev) => this._onEntityDelete(ev, entity);\n                return html`\n                  <ha-icon-button\n                    title=${this.lcn.localize(\"dashboard-entities-table-delete\")}\n                    .path=${mdiDelete}\n                    @click=${handler}\n                  ></ha-icon-button>\n                `;\n              },\n            },\n          },\n  );\n\n  protected render() {\n    return html`\n      <ha-data-table\n        .hass=${this.hass}\n        .columns=${this._columns(this.narrow)}\n        .data=${this._entities(this.entities) as DataTableRowData[]}\n        .id=${\"unique_id\"}\n        .noDataText=${this.lcn.localize(\"dashboard-entities-table-no-data\")}\n        .dir=${computeRTLDirection(this.hass)}\n        auto-height\n        clickable\n      ></ha-data-table>\n    `;\n  }\n\n  private _onEntityDelete(ev, entity: LcnEntityConfig) {\n    ev.stopPropagation();\n    this._deleteEntity(entity.address, entity.domain, entity.resource);\n  }\n\n  private async _deleteEntity(address: LcnAddress, domain: string, resource: string) {\n    const entity_to_delete = this.entities.find(\n      (entity) =>\n        entity.address[0] === address[0] &&\n        entity.address[1] === address[1] &&\n        entity.address[2] === address[2] &&\n        entity.domain === domain &&\n        entity.resource === resource,\n    )!;\n\n    await deleteEntity(this.hass, this.lcn.host.id, entity_to_delete);\n\n    this.dispatchEvent(\n      new CustomEvent(\"lcn-configuration-changed\", {\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-entities-data-table\": LCNEntitiesDataTable;\n  }\n}\n",
-        "import { html, LitElement, TemplateResult } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport { mdiPlus } from \"@mdi/js\";\nimport type { HomeAssistant, Route } from \"@ha/types\";\nimport \"@ha/layouts/hass-tabs-subpage\";\nimport type { PageNavigation } from \"@ha/layouts/hass-tabs-subpage\";\nimport \"@ha/panels/config/ha-config-section\";\nimport \"@ha/layouts/hass-loading-screen\";\nimport \"@ha/components/ha-card\";\nimport \"@ha/components/ha-svg-icon\";\nimport \"@ha/components/ha-fab\";\nimport \"./lcn-entities-data-table\";\nimport {\n  LCN,\n  fetchEntities,\n  fetchDevices,\n  addEntity,\n  LcnDeviceConfig,\n  LcnEntityConfig,\n  LcnAddress,\n} from \"types/lcn\";\nimport {\n  loadLCNCreateEntityDialog,\n  showLCNCreateEntityDialog,\n} from \"./dialogs/show-dialog-create-entity\";\n\n@customElement(\"lcn-entities-page\")\nexport class LCNEntitiesPage extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public narrow!: boolean;\n\n  @property({ attribute: false }) public route!: Route;\n\n  @property({ type: Array, reflect: false }) public tabs: PageNavigation[] = [];\n\n  @state() private _deviceConfig!: LcnDeviceConfig;\n\n  @state() private _entityConfigs: LcnEntityConfig[] = [];\n\n  protected async firstUpdated(changedProperties) {\n    super.firstUpdated(changedProperties);\n    loadLCNCreateEntityDialog();\n\n    await this._fetchEntities(this.lcn.host.id, this.lcn.address);\n  }\n\n  protected render(): TemplateResult {\n    if (!this._deviceConfig && this._entityConfigs.length === 0) {\n      return html` <hass-loading-screen></hass-loading-screen> `;\n    }\n    return html`\n      <hass-tabs-subpage\n        .hass=${this.hass}\n        .narrow=${this.narrow}\n        .route=${this.route}\n        back-path=\"/lcn/devices\"\n        .tabs=${this.tabs}\n      >\n        <ha-config-section .narrow=${this.narrow}>\n          <span slot=\"header\"> ${this.lcn.localize(\"dashboard-entities-title\")} </span>\n\n          <span slot=\"introduction\"> ${this.lcn.localize(\"dashboard-entities-introduction\")} </span>\n\n          <ha-card\n            header=\"Entities for ${this._deviceConfig.address[2]\n              ? this.lcn.localize(\"group\")\n              : this.lcn.localize(\"module\")}\n              (${this.lcn.host.name}, ${this._deviceConfig.address[0]},\n              ${this._deviceConfig.address[1]})\n              ${this._deviceConfig.name ? \" - \" + this._deviceConfig.name : \"\"}\n            \"\n          >\n            <lcn-entities-data-table\n              .hass=${this.hass}\n              .lcn=${this.lcn}\n              .entities=${this._entityConfigs}\n              .device=${this._deviceConfig}\n              .narrow=${this.narrow}\n              @lcn-configuration-changed=${this._configurationChanged}\n            ></lcn-entities-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot=\"fab\"\n          @click=${this._addEntity}\n          .label=${this.lcn.localize(\"dashboard-entities-add\")}\n          extended\n        >\n          <ha-svg-icon slot=\"icon\" path=${mdiPlus}></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    `;\n  }\n\n  private _configurationChanged() {\n    this._fetchEntities(this.lcn.host.id, this.lcn.address);\n  }\n\n  private async _fetchEntities(host: string, address: LcnAddress) {\n    const deviceConfigs = await fetchDevices(this.hass!, host);\n    const deviceConfig = deviceConfigs.find(\n      (el) =>\n        el.address[0] === address[0] &&\n        el.address[1] === address[1] &&\n        el.address[2] === address[2],\n    );\n    if (deviceConfig !== undefined) {\n      this._deviceConfig = deviceConfig;\n    }\n    this._entityConfigs = await fetchEntities(this.hass!, host, address);\n  }\n\n  private async _addEntity() {\n    showLCNCreateEntityDialog(this, {\n      lcn: this.lcn,\n      device: <LcnDeviceConfig>this._deviceConfig,\n      createEntity: async (entityParams) => {\n        if (await addEntity(this.hass, this.lcn.host.id, entityParams)) {\n          await this._fetchEntities(this.lcn.host.id, this.lcn.address);\n          return true;\n        }\n        return false;\n      },\n    });\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-entities-page\": LCNEntitiesPage;\n  }\n}\n"
+        "import { html, LitElement, TemplateResult } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport { mdiPlus } from \"@mdi/js\";\nimport type { HomeAssistant, Route } from \"@ha/types\";\nimport \"@ha/layouts/hass-tabs-subpage\";\nimport type { PageNavigation } from \"@ha/layouts/hass-tabs-subpage\";\nimport \"@ha/panels/config/ha-config-section\";\nimport \"@ha/layouts/hass-loading-screen\";\nimport \"@ha/components/ha-card\";\nimport \"@ha/components/ha-svg-icon\";\nimport \"@ha/components/ha-fab\";\nimport \"./lcn-entities-data-table\";\nimport {\n  LCN,\n  fetchEntities,\n  fetchDevices,\n  addEntity,\n  LcnDeviceConfig,\n  LcnEntityConfig,\n  LcnAddress,\n} from \"types/lcn\";\nimport {\n  loadLCNCreateEntityDialog,\n  showLCNCreateEntityDialog,\n} from \"./dialogs/show-dialog-create-entity\";\n\n@customElement(\"lcn-entities-page\")\nexport class LCNEntitiesPage extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public narrow!: boolean;\n\n  @property({ attribute: false }) public route!: Route;\n\n  @property({ type: Array, reflect: false }) public tabs: PageNavigation[] = [];\n\n  @state() private _deviceConfig!: LcnDeviceConfig;\n\n  @state() private _entityConfigs: LcnEntityConfig[] = [];\n\n  protected async firstUpdated(changedProperties) {\n    super.firstUpdated(changedProperties);\n    loadLCNCreateEntityDialog();\n\n    await this._fetchEntities(this.lcn.host.id, this.lcn.address);\n  }\n\n  protected render(): TemplateResult {\n    if (!this._deviceConfig && this._entityConfigs.length === 0) {\n      return html` <hass-loading-screen></hass-loading-screen> `;\n    }\n    return html`\n      <hass-tabs-subpage\n        .hass=${this.hass}\n        .narrow=${this.narrow}\n        .route=${this.route}\n        .tabs=${this.tabs}\n        back-path=\"/lcn/devices\"\n      >\n        <span slot=\"header\"> ${this.lcn.localize(\"dashboard-entities-title\")} </span>\n        <ha-config-section .narrow=${this.narrow}>\n          <span slot=\"introduction\"> ${this.renderIntro()} </span>\n\n          <ha-card\n            header=\"${this._deviceConfig.address[2]\n              ? this.lcn.localize(\"dashboard-entities-entities-for-group\")\n              : this.lcn.localize(\"dashboard-entities-entities-for-module\")}:\n              (${this.lcn.host.name}, ${this._deviceConfig.address[0]},\n              ${this._deviceConfig.address[1]})\n              ${this._deviceConfig.name ? \" - \" + this._deviceConfig.name : \"\"}\n            \"\n          >\n            <lcn-entities-data-table\n              .hass=${this.hass}\n              .lcn=${this.lcn}\n              .entities=${this._entityConfigs}\n              .device=${this._deviceConfig}\n              .narrow=${this.narrow}\n              @lcn-configuration-changed=${this._configurationChanged}\n            ></lcn-entities-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot=\"fab\"\n          @click=${this._addEntity}\n          .label=${this.lcn.localize(\"dashboard-entities-add\")}\n          extended\n        >\n          <ha-svg-icon slot=\"icon\" path=${mdiPlus}></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    `;\n  }\n\n  private renderIntro(): TemplateResult {\n    return html`\n      <h3>${this.lcn.localize(\"dashboard-entities-introduction\")}</h3>\n      <details>\n        <summary>${this.lcn.localize(\"more-help\")}</summary>\n        <ul>\n          <li>${this.lcn.localize(\"dashboard-entities-introduction-help-1\")}</li>\n          <li>${this.lcn.localize(\"dashboard-entities-introduction-help-2\")}</li>\n          <li>${this.lcn.localize(\"dashboard-entities-introduction-help-3\")}</li>\n          <li>${this.lcn.localize(\"dashboard-entities-introduction-help-4\")}</li>\n          <li>${this.lcn.localize(\"dashboard-entities-introduction-help-5\")}</li>\n        </ul>\n      </details>\n    `;\n  }\n\n  private _configurationChanged() {\n    this._fetchEntities(this.lcn.host.id, this.lcn.address);\n  }\n\n  private async _fetchEntities(host: string, address: LcnAddress) {\n    const deviceConfigs = await fetchDevices(this.hass!, host);\n    const deviceConfig = deviceConfigs.find(\n      (el) =>\n        el.address[0] === address[0] &&\n        el.address[1] === address[1] &&\n        el.address[2] === address[2],\n    );\n    if (deviceConfig !== undefined) {\n      this._deviceConfig = deviceConfig;\n    }\n    this._entityConfigs = await fetchEntities(this.hass!, host, address);\n  }\n\n  private async _addEntity() {\n    showLCNCreateEntityDialog(this, {\n      lcn: this.lcn,\n      device: <LcnDeviceConfig>this._deviceConfig,\n      createEntity: async (entityParams) => {\n        if (await addEntity(this.hass, this.lcn.host.id, entityParams)) {\n          await this._fetchEntities(this.lcn.host.id, this.lcn.address);\n          return true;\n        }\n        return false;\n      },\n    });\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-entities-page\": LCNEntitiesPage;\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/bc9cfM__.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/bc9cfM__.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/eOHcBlX_.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ovjKXg0y.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1080,17 +1080,17 @@
                             name: this.lcn.localize("binary-sensor-type-keys-locks"),
                             value: this._keys,
                             id: "key-locks"
                         }]
                     }
                 }, {
                     kind: "method",
-                    key: "firstUpdated",
-                    value: async function(e) {
-                        (0, c.Z)((0, u.Z)(i.prototype), "firstUpdated", this).call(this, e), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0]
+                    key: "connectedCallback",
+                    value: function() {
+                        (0, c.Z)((0, u.Z)(i.prototype), "connectedCallback", this).call(this), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0]
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
                         return this._sourceType || this._source ? l.dy`
       <div class="sources">
@@ -1322,17 +1322,17 @@
                     kind: "get",
                     key: "_setpoints",
                     value: function() {
                         return this._is2012 ? this._varSetpoints.concat(this._variablesNew) : this._varSetpoints
                     }
                 }, {
                     kind: "method",
-                    key: "firstUpdated",
-                    value: async function(e) {
-                        (0, c.Z)((0, u.Z)(i.prototype), "firstUpdated", this).call(this, e), this._source = this._sources[0], this._setpoint = this._setpoints[0], this._unit = this._varUnits[0]
+                    key: "connectedCallback",
+                    value: function() {
+                        (0, c.Z)((0, u.Z)(i.prototype), "connectedCallback", this).call(this), this._source = this._sources[0], this._setpoint = this._setpoints[0], this._unit = this._varUnits[0]
                     }
                 }, {
                     kind: "method",
                     key: "willUpdate",
                     value: function(e) {
                         (0, c.Z)((0, u.Z)(i.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateMinTemp(this.domainData.min_temp) || !this._validateMaxTemp(this.domainData.max_temp)
                     }
@@ -1598,17 +1598,17 @@
                         }, {
                             name: "1200ms",
                             value: "RT1200"
                         }]
                     }
                 }, {
                     kind: "method",
-                    key: "firstUpdated",
-                    value: async function(e) {
-                        (0, c.Z)((0, u.Z)(i.prototype), "firstUpdated", this).call(this, e), this._motor = this._motors[0], this._reverseDelay = this._reverseDelays[0]
+                    key: "connectedCallback",
+                    value: function() {
+                        (0, c.Z)((0, u.Z)(i.prototype), "connectedCallback", this).call(this), this._motor = this._motors[0], this._reverseDelay = this._reverseDelays[0]
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
                         return this._motor || this._reverseDelay ? l.dy`
       <ha-select
@@ -1784,17 +1784,17 @@
                             name: this.lcn.localize("relay"),
                             value: this._relayPorts,
                             id: "relay"
                         }]
                     }
                 }, {
                     kind: "method",
-                    key: "firstUpdated",
-                    value: async function(e) {
-                        (0, c.Z)((0, u.Z)(i.prototype), "firstUpdated", this).call(this, e), this._portType = this._portTypes[0], this._port = this._portType.value[0]
+                    key: "connectedCallback",
+                    value: function() {
+                        (0, c.Z)((0, u.Z)(i.prototype), "connectedCallback", this).call(this), this._portType = this._portTypes[0], this._port = this._portType.value[0]
                     }
                 }, {
                     kind: "method",
                     key: "willUpdate",
                     value: function(e) {
                         (0, c.Z)((0, u.Z)(i.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateTransition(this.domainData.transition)
                     }
@@ -2116,17 +2116,17 @@
                         }, {
                             name: e + " 8",
                             value: "RELAY8"
                         }]
                     }
                 }, {
                     kind: "method",
-                    key: "firstUpdated",
-                    value: async function(e) {
-                        (0, c.Z)((0, u.Z)(i.prototype), "firstUpdated", this).call(this, e), this._register = this._registers[0], this._scene = this._scenes[0]
+                    key: "connectedCallback",
+                    value: function() {
+                        (0, c.Z)((0, u.Z)(i.prototype), "connectedCallback", this).call(this), this._register = this._registers[0], this._scene = this._scenes[0]
                     }
                 }, {
                     kind: "method",
                     key: "willUpdate",
                     value: function(e) {
                         (0, c.Z)((0, u.Z)(i.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateTransition(this.domainData.transition)
                     }
@@ -2641,17 +2641,17 @@
                         }, {
                             name: this.lcn.localize("unit-angle") + " (°)",
                             value: "DEGREE"
                         }]
                     }
                 }, {
                     kind: "method",
-                    key: "firstUpdated",
-                    value: async function(e) {
-                        (0, c.Z)((0, u.Z)(i.prototype), "firstUpdated", this).call(this, e), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0], this._unit = this._varUnits[0]
+                    key: "connectedCallback",
+                    value: function() {
+                        (0, c.Z)((0, u.Z)(i.prototype), "connectedCallback", this).call(this), this._sourceType = this._sourceTypes[0], this._source = this._sourceType.value[0], this._unit = this._varUnits[0]
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
                         return this._sourceType || this._source ? l.dy`
       <div class="sources">
@@ -2841,17 +2841,17 @@
                             name: this.lcn.localize("relay"),
                             value: this._relayPorts,
                             id: "relay"
                         }]
                     }
                 }, {
                     kind: "method",
-                    key: "firstUpdated",
-                    value: async function(e) {
-                        (0, c.Z)((0, u.Z)(i.prototype), "firstUpdated", this).call(this, e), this._portType = this._portTypes[0], this._port = this._portType.value[0]
+                    key: "connectedCallback",
+                    value: function() {
+                        (0, c.Z)((0, u.Z)(i.prototype), "connectedCallback", this).call(this), this._portType = this._portTypes[0], this._port = this._portType.value[0]
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
                         return this._portType || this._port ? l.dy`
       <div id="port-type">${this.lcn.localize("port-type")}</div>
@@ -3177,8 +3177,8 @@
       `]
                     }
                 }]
             }
         }), l.oi)
     }
 };
-//# sourceMappingURL=eOHcBlX_.js.map
+//# sourceMappingURL=ovjKXg0y.js.map
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/eOHcBlX_.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/ovjKXg0y.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8136645962732919%*

 * *Differences: {"'file'": "'ovjKXg0y.js'",*

 * * "'mappings'": "';;;;AAcA;ACCA;;AAEA;AAhBA;;;;AAqBA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA+HA;;;;;;;;;;;;;ACtGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACkCA;;;;ACnEA;ACIA;AACA;;AAGA;AArBA;AAuBA;AAGA;;AAIA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsFA;;;;;;;;;;;;;;;;;;;;ACxEA;;ACyBA;AACA;;AAEA;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;; […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "eOHcBlX_.js",
-    "mappings": ";;;;AAcA;ACCA;;AAEA;AAhBA;;;;AAqBA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA+HA;;;;;;;;;;;;;ACtGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACkCA;;;;ACnEA;ACIA;AACA;;AAGA;AArBA;AAuBA;AAGA;;AAIA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsFA;;;;;;;;;;;;;;;;;;;;ACxEA;;ACyBA;AACA;;AAEA;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAyHA;;;;;;;;;;AAWA;;;;AChFA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;AA7BA;;;;;;;;;;AAqEA;;;;AChEA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;;AAEA;AACA;;;;;;AAMA;;AAEA;;;AAGA;AACA;AACA;;;;;AAOA;;AAEA;;;AAGA;AACA;AACA;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;;AA/EA;;;;;;;;;;;;;;;;;AAwKA;;;AClOA;AACA;;AAEA;AACA;;AAEA;;;AAKA;;;AAIA;AACA;;AAEA;AACA;;AAEA;AAEA;;;AAIA;AAhCA;;;;;AAkEA;ACnBA;;AAEA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;AACA;;;;;;AAMA;AACA;;AAEA;AACA;;AAEA;;;AAKA;AApCA;;AA6CA;;;AAGA;AACA;;;;;;AAMA;;AAEA;;;;;AAKA;AACA;AACA;;AAQA;;;;;;;;;;;;;;;AA0DA;;;;AC3GA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;;;;;AAOA;AACA;AAEA;AACA;;;;;;AAOA;AACA;AAEA;AACA;;;;;;AAOA;;AAEA;;;;;AAKA;AACA;AACA;AACA;;AAlEA;;;;;;;;;;;;;;AAwIA;;;;AClDA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;;AAQA;AACA;;AAEA;AACA;;AAEA;;AA3CA;;;;;;;;;;AA0FA;ACjNA;;AAEA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;AACA;;;;;;AAMA;AACA;;AAEA;AACA;;AAEA;;AA/BA;;;;;;;;AAmEA;;;;;ACzEA;AAIA;;;;AAIA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;;AAEA;;AAEA;;;AAGA;;;;;AAKA;AACA;;;;AAIA;AACA;AACA;;;;AAjDA;;AAgEA;AACA;AAEA;;AAGA;AACA;AACA;AACA;AAEA;;AAGA;AACA;AAEA;;AAGA;AACA;AACA;AAEA;;AAGA;AACA;AACA;AAEA;;AAGA;AACA;AACA;AAEA;;AAGA;AACA;AAEA;;;;;;;;;;;;;;;AAuEA",
+    "file": "ovjKXg0y.js",
+    "mappings": ";;;;AAcA;ACCA;;AAEA;AAhBA;;;;AAqBA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA+HA;;;;;;;;;;;;;ACtGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACkCA;;;;ACnEA;ACIA;AACA;;AAGA;AArBA;AAuBA;AAGA;;AAIA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsFA;;;;;;;;;;;;;;;;;;;;ACxEA;;ACyBA;AACA;;AAEA;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAyHA;;;;;;;;;;AAWA;;;;AChFA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;AA7BA;;;;;;;;;;AAqEA;;;;ACjEA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;;AAEA;AACA;;;;;;AAMA;;AAEA;;;AAGA;AACA;AACA;;;;;AAOA;;AAEA;;;AAGA;AACA;AACA;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;;AA/EA;;;;;;;;;;;;;;;;;AAwKA;;;ACjOA;AACA;;AAEA;AACA;;AAEA;;;AAKA;;;AAIA;AACA;;AAEA;AACA;;AAEA;AAEA;;;AAIA;AAhCA;;;;;AAkEA;ACnBA;;AAEA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;AACA;;;;;;AAMA;AACA;;AAEA;AACA;;AAEA;;;AAKA;AApCA;;AA6CA;;;AAGA;AACA;;;;;;AAMA;;AAEA;;;;;AAKA;AACA;AACA;;AAQA;;;;;;;;;;;;;;;AA0DA;;;;AC5GA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;;;;;AAOA;AACA;AAEA;AACA;;;;;;AAOA;AACA;AAEA;AACA;;;;;;AAOA;;AAEA;;;;;AAKA;AACA;AACA;AACA;;AAlEA;;;;;;;;;;;;;;AAwIA;;;;AClDA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;;AAQA;AACA;;AAEA;AACA;;AAEA;;AA3CA;;;;;;;;;;AA0FA;AChNA;;AAEA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;AACA;;;;;;AAMA;AACA;;AAEA;AACA;;AAEA;;AA/BA;;;;;;;;AAmEA;;;;;ACzEA;AAIA;;;;AAIA;AACA;;AAEA;AACA;;AAEA;AAEA;;;;;;AAOA;;AAEA;;AAEA;;;AAGA;;;;;AAKA;AACA;;;;AAIA;AACA;AACA;;;;AAjDA;;AAgEA;AACA;AAEA;;AAGA;AACA;AACA;AACA;AAEA;;AAGA;AACA;AAEA;;AAGA;AACA;AACA;AAEA;;AAGA;AACA;AACA;AAEA;;AAGA;AACA;AACA;AAEA;;AAGA;AACA;AAEA;;;;;;;;;;;;;;;AAuEA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-checkbox.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-dialog.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-formfield.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-list-item.ts",
@@ -26,18 +26,18 @@
         "import { DialogBase } from \"@material/mwc-dialog/mwc-dialog-base\";\nimport { styles } from \"@material/mwc-dialog/mwc-dialog.css\";\nimport { mdiClose } from \"@mdi/js\";\nimport { css, html, TemplateResult } from \"lit\";\nimport { customElement } from \"lit/decorators\";\nimport { FOCUS_TARGET } from \"../dialogs/make-dialog-manager\";\nimport type { HomeAssistant } from \"../types\";\nimport \"./ha-icon-button\";\n\nconst SUPPRESS_DEFAULT_PRESS_SELECTOR = [\"button\", \"ha-list-item\"];\n\nexport const createCloseHeading = (\n  hass: HomeAssistant | undefined,\n  title: string | TemplateResult\n) => html`\n  <div class=\"header_title\">${title}</div>\n  <ha-icon-button\n    .label=${hass?.localize(\"ui.dialogs.generic.close\") ?? \"Close\"}\n    .path=${mdiClose}\n    dialogAction=\"close\"\n    class=\"header_button\"\n  ></ha-icon-button>\n`;\n\n@customElement(\"ha-dialog\")\nexport class HaDialog extends DialogBase {\n  protected readonly [FOCUS_TARGET];\n\n  public scrollToPos(x: number, y: number) {\n    this.contentElement?.scrollTo(x, y);\n  }\n\n  protected renderHeading() {\n    return html`<slot name=\"heading\"> ${super.renderHeading()} </slot>`;\n  }\n\n  protected firstUpdated(): void {\n    super.firstUpdated();\n    this.suppressDefaultPressSelector = [\n      this.suppressDefaultPressSelector,\n      SUPPRESS_DEFAULT_PRESS_SELECTOR,\n    ].join(\", \");\n    this._updateScrolledAttribute();\n    this.contentElement?.addEventListener(\"scroll\", this._onScroll, {\n      passive: true,\n    });\n  }\n\n  disconnectedCallback(): void {\n    super.disconnectedCallback();\n    this.contentElement.removeEventListener(\"scroll\", this._onScroll);\n  }\n\n  private _onScroll = () => {\n    this._updateScrolledAttribute();\n  };\n\n  private _updateScrolledAttribute() {\n    if (!this.contentElement) return;\n    this.toggleAttribute(\"scrolled\", this.contentElement.scrollTop !== 0);\n  }\n\n  static override styles = [\n    styles,\n    css`\n      :host([scrolled]) ::slotted(ha-dialog-header) {\n        border-bottom: 1px solid\n          var(--mdc-dialog-scroll-divider-color, rgba(0, 0, 0, 0.12));\n      }\n      .mdc-dialog {\n        --mdc-dialog-scroll-divider-color: var(\n          --dialog-scroll-divider-color,\n          var(--divider-color)\n        );\n        z-index: var(--dialog-z-index, 8);\n        -webkit-backdrop-filter: var(--dialog-backdrop-filter, none);\n        backdrop-filter: var(--dialog-backdrop-filter, none);\n        --mdc-dialog-box-shadow: var(--dialog-box-shadow, none);\n        --mdc-typography-headline6-font-weight: 400;\n        --mdc-typography-headline6-font-size: 1.574rem;\n      }\n      .mdc-dialog__actions {\n        justify-content: var(--justify-action-buttons, flex-end);\n        padding-bottom: max(env(safe-area-inset-bottom), 24px);\n      }\n      .mdc-dialog__actions span:nth-child(1) {\n        flex: var(--secondary-action-button-flex, unset);\n      }\n      .mdc-dialog__actions span:nth-child(2) {\n        flex: var(--primary-action-button-flex, unset);\n      }\n      .mdc-dialog__container {\n        align-items: var(--vertical-align-dialog, center);\n      }\n      .mdc-dialog__title {\n        padding: 24px 24px 0 24px;\n        text-overflow: ellipsis;\n        overflow: hidden;\n      }\n      .mdc-dialog__actions {\n        padding: 12px 24px 12px 24px;\n      }\n      .mdc-dialog__title::before {\n        display: block;\n        height: 0px;\n      }\n      .mdc-dialog .mdc-dialog__content {\n        position: var(--dialog-content-position, relative);\n        padding: var(--dialog-content-padding, 24px);\n      }\n      :host([hideactions]) .mdc-dialog .mdc-dialog__content {\n        padding-bottom: max(\n          var(--dialog-content-padding, 24px),\n          env(safe-area-inset-bottom)\n        );\n      }\n      .mdc-dialog .mdc-dialog__surface {\n        position: var(--dialog-surface-position, relative);\n        top: var(--dialog-surface-top);\n        margin-top: var(--dialog-surface-margin-top);\n        min-height: var(--mdc-dialog-min-height, auto);\n        border-radius: var(--ha-dialog-border-radius, 28px);\n      }\n      :host([flexContent]) .mdc-dialog .mdc-dialog__content {\n        display: flex;\n        flex-direction: column;\n      }\n      .header_title {\n        margin-right: 32px;\n        margin-inline-end: 32px;\n        margin-inline-start: initial;\n        direction: var(--direction);\n      }\n      .header_button {\n        position: absolute;\n        right: 16px;\n        top: 14px;\n        text-decoration: none;\n        color: inherit;\n        inset-inline-start: initial;\n        inset-inline-end: 16px;\n        direction: var(--direction);\n      }\n      .dialog-actions {\n        inset-inline-start: initial !important;\n        inset-inline-end: 0px !important;\n        direction: var(--direction);\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-dialog\": HaDialog;\n  }\n}\n",
         "import { FormfieldBase } from \"@material/mwc-formfield/mwc-formfield-base\";\nimport { styles } from \"@material/mwc-formfield/mwc-formfield.css\";\nimport { css } from \"lit\";\nimport { customElement } from \"lit/decorators\";\nimport { fireEvent } from \"../common/dom/fire_event\";\n\n@customElement(\"ha-formfield\")\nexport class HaFormfield extends FormfieldBase {\n  protected _labelClick() {\n    const input = this.input as HTMLInputElement | undefined;\n    if (!input) return;\n\n    input.focus();\n    if (input.disabled) {\n      return;\n    }\n    switch (input.tagName) {\n      case \"HA-CHECKBOX\":\n        input.checked = !input.checked;\n        fireEvent(input, \"change\");\n        break;\n      case \"HA-RADIO\":\n        input.checked = true;\n        fireEvent(input, \"change\");\n        break;\n      default:\n        input.click();\n        break;\n    }\n  }\n\n  static override styles = [\n    styles,\n    css`\n      :host(:not([alignEnd])) ::slotted(ha-switch) {\n        margin-right: 10px;\n        margin-inline-end: 10px;\n        margin-inline-start: inline;\n      }\n      .mdc-form-field > label {\n        direction: var(--direction);\n        margin-inline-start: 0;\n        margin-inline-end: auto;\n        padding-inline-start: 4px;\n        padding-inline-end: 0;\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-formfield\": HaFormfield;\n  }\n}\n",
         "import { ListItemBase } from \"@material/mwc-list/mwc-list-item-base\";\nimport { styles } from \"@material/mwc-list/mwc-list-item.css\";\nimport { css, CSSResultGroup } from \"lit\";\nimport { customElement } from \"lit/decorators\";\n\n@customElement(\"ha-list-item\")\nexport class HaListItem extends ListItemBase {\n  protected renderRipple() {\n    if (this.noninteractive) {\n      return \"\";\n    }\n    return super.renderRipple();\n  }\n\n  static get styles(): CSSResultGroup {\n    return [\n      styles,\n      css`\n        :host {\n          padding-left: var(\n            --mdc-list-side-padding-left,\n            var(--mdc-list-side-padding, 20px)\n          );\n          padding-right: var(\n            --mdc-list-side-padding-right,\n            var(--mdc-list-side-padding, 20px)\n          );\n        }\n        :host([graphic=\"avatar\"]:not([twoLine])),\n        :host([graphic=\"icon\"]:not([twoLine])) {\n          height: 48px;\n        }\n        span.material-icons:first-of-type {\n          margin-inline-start: 0px !important;\n          margin-inline-end: var(\n            --mdc-list-item-graphic-margin,\n            16px\n          ) !important;\n          direction: var(--direction);\n        }\n        span.material-icons:last-of-type {\n          margin-inline-start: auto !important;\n          margin-inline-end: 0px !important;\n          direction: var(--direction);\n        }\n        .mdc-deprecated-list-item__meta {\n          display: var(--mdc-list-item-meta-display);\n          align-items: center;\n        }\n        :host([multiline-secondary]) {\n          height: auto;\n        }\n        :host([multiline-secondary]) .mdc-deprecated-list-item__text {\n          padding: 8px 0;\n        }\n        :host([multiline-secondary]) .mdc-deprecated-list-item__secondary-text {\n          text-overflow: initial;\n          white-space: normal;\n          overflow: auto;\n          display: inline-block;\n          margin-top: 10px;\n        }\n        :host([multiline-secondary]) .mdc-deprecated-list-item__primary-text {\n          margin-top: 10px;\n        }\n        :host([multiline-secondary])\n          .mdc-deprecated-list-item__secondary-text::before {\n          display: none;\n        }\n        :host([multiline-secondary])\n          .mdc-deprecated-list-item__primary-text::before {\n          display: none;\n        }\n        :host([disabled]) {\n          color: var(--disabled-text-color);\n        }\n        :host([noninteractive]) {\n          pointer-events: unset;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-list-item\": HaListItem;\n  }\n}\n",
         "import { RadioBase } from \"@material/mwc-radio/mwc-radio-base\";\nimport { styles } from \"@material/mwc-radio/mwc-radio.css\";\nimport { css } from \"lit\";\nimport { customElement } from \"lit/decorators\";\n\n@customElement(\"ha-radio\")\nexport class HaRadio extends RadioBase {\n  static override styles = [\n    styles,\n    css`\n      :host {\n        --mdc-theme-secondary: var(--primary-color);\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-radio\": HaRadio;\n  }\n}\n",
         "import { SelectBase } from \"@material/mwc-select/mwc-select-base\";\nimport { styles } from \"@material/mwc-select/mwc-select.css\";\nimport { mdiClose } from \"@mdi/js\";\nimport { css, html, nothing } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\nimport { debounce } from \"../common/util/debounce\";\nimport { nextRender } from \"../common/util/render-status\";\nimport \"./ha-icon-button\";\n\n@customElement(\"ha-select\")\nexport class HaSelect extends SelectBase {\n  // @ts-ignore\n  @property({ type: Boolean }) public icon?: boolean;\n\n  @property({ type: Boolean, reflect: true }) public clearable?: boolean;\n\n  protected override render() {\n    return html`\n      ${super.render()}\n      ${this.clearable && !this.required && !this.disabled && this.value\n        ? html`<ha-icon-button\n            label=\"clear\"\n            @click=${this._clearValue}\n            .path=${mdiClose}\n          ></ha-icon-button>`\n        : nothing}\n    `;\n  }\n\n  protected override renderLeadingIcon() {\n    if (!this.icon) {\n      return nothing;\n    }\n\n    return html`<span class=\"mdc-select__icon\"\n      ><slot name=\"icon\"></slot\n    ></span>`;\n  }\n\n  connectedCallback() {\n    super.connectedCallback();\n    window.addEventListener(\"translations-updated\", this._translationsUpdated);\n  }\n\n  disconnectedCallback() {\n    super.disconnectedCallback();\n    window.removeEventListener(\n      \"translations-updated\",\n      this._translationsUpdated\n    );\n  }\n\n  private _clearValue(): void {\n    if (this.disabled || !this.value) {\n      return;\n    }\n    this.valueSetDirectly = true;\n    this.select(-1);\n    this.mdcFoundation.handleChange();\n  }\n\n  private _translationsUpdated = debounce(async () => {\n    await nextRender();\n    this.layoutOptions();\n  }, 500);\n\n  static override styles = [\n    styles,\n    css`\n      :host([clearable]) {\n        position: relative;\n      }\n      .mdc-select:not(.mdc-select--disabled) .mdc-select__icon {\n        color: var(--secondary-text-color);\n      }\n      .mdc-select__anchor {\n        width: var(--ha-select-min-width, 200px);\n      }\n      .mdc-select--filled .mdc-select__anchor {\n        height: var(--ha-select-height, 56px);\n      }\n      .mdc-select--filled .mdc-floating-label {\n        inset-inline-start: 12px;\n        inset-inline-end: initial;\n        direction: var(--direction);\n      }\n      .mdc-select--filled.mdc-select--with-leading-icon .mdc-floating-label {\n        inset-inline-start: 48px;\n        inset-inline-end: initial;\n        direction: var(--direction);\n      }\n      .mdc-select .mdc-select__anchor {\n        padding-inline-start: 12px;\n        padding-inline-end: 0px;\n        direction: var(--direction);\n      }\n      .mdc-select__anchor .mdc-floating-label--float-above {\n        transform-origin: var(--float-start);\n      }\n      .mdc-select__selected-text-container {\n        padding-inline-end: var(--select-selected-text-padding-end, 0px);\n      }\n      :host([clearable]) .mdc-select__selected-text-container {\n        padding-inline-end: var(--select-selected-text-padding-end, 12px);\n      }\n      ha-icon-button {\n        position: absolute;\n        top: 10px;\n        right: 28px;\n        --mdc-icon-button-size: 36px;\n        --mdc-icon-size: 20px;\n        color: var(--secondary-text-color);\n        inset-inline-start: initial;\n        inset-inline-end: 28px;\n        direction: var(--direction);\n      }\n    `,\n  ];\n}\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-select\": HaSelect;\n  }\n}\n",
         "import { SwitchBase } from \"@material/mwc-switch/deprecated/mwc-switch-base\";\nimport { styles } from \"@material/mwc-switch/deprecated/mwc-switch.css\";\nimport { css } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\nimport { forwardHaptic } from \"../data/haptics\";\n\n@customElement(\"ha-switch\")\nexport class HaSwitch extends SwitchBase {\n  // Generate a haptic vibration.\n  // Only set to true if the new value of the switch is applied right away when toggling.\n  // Do not add haptic when a user is required to press save.\n  @property({ type: Boolean }) public haptic = false;\n\n  protected firstUpdated() {\n    super.firstUpdated();\n    this.addEventListener(\"change\", () => {\n      if (this.haptic) {\n        forwardHaptic(\"light\");\n      }\n    });\n  }\n\n  static override styles = [\n    styles,\n    css`\n      :host {\n        --mdc-theme-secondary: var(--switch-checked-color);\n      }\n      .mdc-switch.mdc-switch--checked .mdc-switch__thumb {\n        background-color: var(--switch-checked-button-color);\n        border-color: var(--switch-checked-button-color);\n      }\n      .mdc-switch.mdc-switch--checked .mdc-switch__track {\n        background-color: var(--switch-checked-track-color);\n        border-color: var(--switch-checked-track-color);\n      }\n      .mdc-switch:not(.mdc-switch--checked) .mdc-switch__thumb {\n        background-color: var(--switch-unchecked-button-color);\n        border-color: var(--switch-unchecked-button-color);\n      }\n      .mdc-switch:not(.mdc-switch--checked) .mdc-switch__track {\n        background-color: var(--switch-unchecked-track-color);\n        border-color: var(--switch-unchecked-track-color);\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-switch\": HaSwitch;\n  }\n}\n",
         "import { TextFieldBase } from \"@material/mwc-textfield/mwc-textfield-base\";\nimport { styles } from \"@material/mwc-textfield/mwc-textfield.css\";\nimport { TemplateResult, html, PropertyValues, css } from \"lit\";\nimport { customElement, property, query } from \"lit/decorators\";\nimport { mainWindow } from \"../common/dom/get_main_window\";\n\n@customElement(\"ha-textfield\")\nexport class HaTextField extends TextFieldBase {\n  @property({ type: Boolean }) public invalid?: boolean;\n\n  @property({ attribute: \"error-message\" }) public errorMessage?: string;\n\n  // @ts-ignore\n  @property({ type: Boolean }) public icon?: boolean;\n\n  // @ts-ignore\n  @property({ type: Boolean }) public iconTrailing?: boolean;\n\n  @property() public autocomplete?: string;\n\n  @property() public autocorrect?: string;\n\n  @property({ attribute: \"input-spellcheck\" })\n  public inputSpellcheck?: string;\n\n  @query(\"input\") public formElement!: HTMLInputElement;\n\n  override updated(changedProperties: PropertyValues) {\n    super.updated(changedProperties);\n    if (\n      (changedProperties.has(\"invalid\") &&\n        (this.invalid || changedProperties.get(\"invalid\") !== undefined)) ||\n      changedProperties.has(\"errorMessage\")\n    ) {\n      this.setCustomValidity(\n        this.invalid ? this.errorMessage || \"Invalid\" : \"\"\n      );\n      this.reportValidity();\n    }\n    if (changedProperties.has(\"autocomplete\")) {\n      if (this.autocomplete) {\n        this.formElement.setAttribute(\"autocomplete\", this.autocomplete);\n      } else {\n        this.formElement.removeAttribute(\"autocomplete\");\n      }\n    }\n    if (changedProperties.has(\"autocorrect\")) {\n      if (this.autocorrect) {\n        this.formElement.setAttribute(\"autocorrect\", this.autocorrect);\n      } else {\n        this.formElement.removeAttribute(\"autocorrect\");\n      }\n    }\n    if (changedProperties.has(\"inputSpellcheck\")) {\n      if (this.inputSpellcheck) {\n        this.formElement.setAttribute(\"spellcheck\", this.inputSpellcheck);\n      } else {\n        this.formElement.removeAttribute(\"spellcheck\");\n      }\n    }\n  }\n\n  protected override renderIcon(\n    _icon: string,\n    isTrailingIcon = false\n  ): TemplateResult {\n    const type = isTrailingIcon ? \"trailing\" : \"leading\";\n\n    return html`\n      <span\n        class=\"mdc-text-field__icon mdc-text-field__icon--${type}\"\n        tabindex=${isTrailingIcon ? 1 : -1}\n      >\n        <slot name=\"${type}Icon\"></slot>\n      </span>\n    `;\n  }\n\n  static override styles = [\n    styles,\n    css`\n      .mdc-text-field__input {\n        width: var(--ha-textfield-input-width, 100%);\n      }\n      .mdc-text-field:not(.mdc-text-field--with-leading-icon) {\n        padding: var(--text-field-padding, 0px 16px);\n      }\n      .mdc-text-field__affix--suffix {\n        padding-left: var(--text-field-suffix-padding-left, 12px);\n        padding-right: var(--text-field-suffix-padding-right, 0px);\n        padding-inline-start: var(--text-field-suffix-padding-left, 12px);\n        padding-inline-end: var(--text-field-suffix-padding-right, 0px);\n        direction: var(--direction);\n      }\n      .mdc-text-field--with-leading-icon {\n        padding-inline-start: var(--text-field-suffix-padding-left, 0px);\n        padding-inline-end: var(--text-field-suffix-padding-right, 16px);\n        direction: var(--direction);\n      }\n\n      .mdc-text-field--with-leading-icon.mdc-text-field--with-trailing-icon {\n        padding-left: var(--text-field-suffix-padding-left, 0px);\n        padding-right: var(--text-field-suffix-padding-right, 0px);\n        padding-inline-start: var(--text-field-suffix-padding-left, 0px);\n        padding-inline-end: var(--text-field-suffix-padding-right, 0px);\n      }\n      .mdc-text-field:not(.mdc-text-field--disabled)\n        .mdc-text-field__affix--suffix {\n        color: var(--secondary-text-color);\n      }\n\n      .mdc-text-field__icon {\n        color: var(--secondary-text-color);\n      }\n\n      .mdc-text-field__icon--leading {\n        margin-inline-start: 16px;\n        margin-inline-end: 8px;\n        direction: var(--direction);\n      }\n\n      .mdc-text-field__icon--trailing {\n        padding: var(--textfield-icon-trailing-padding, 12px);\n      }\n\n      .mdc-floating-label:not(.mdc-floating-label--float-above) {\n        text-overflow: ellipsis;\n        width: inherit;\n        padding-right: 30px;\n        padding-inline-end: 30px;\n        padding-inline-start: initial;\n        box-sizing: border-box;\n        direction: var(--direction);\n      }\n\n      input {\n        text-align: var(--text-field-text-align, start);\n      }\n\n      /* Edge, hide reveal password icon */\n      ::-ms-reveal {\n        display: none;\n      }\n\n      /* Chrome, Safari, Edge, Opera */\n      :host([no-spinner]) input::-webkit-outer-spin-button,\n      :host([no-spinner]) input::-webkit-inner-spin-button {\n        -webkit-appearance: none;\n        margin: 0;\n      }\n\n      /* Firefox */\n      :host([no-spinner]) input[type=\"number\"] {\n        -moz-appearance: textfield;\n      }\n\n      .mdc-text-field__ripple {\n        overflow: hidden;\n      }\n\n      .mdc-text-field {\n        overflow: var(--text-field-overflow);\n      }\n\n      .mdc-floating-label {\n        inset-inline-start: 16px !important;\n        inset-inline-end: initial !important;\n        transform-origin: var(--float-start);\n        direction: var(--direction);\n        text-align: var(--float-start);\n      }\n\n      .mdc-text-field--with-leading-icon.mdc-text-field--filled\n        .mdc-floating-label {\n        max-width: calc(\n          100% - 48px - var(--text-field-suffix-padding-left, 0px)\n        );\n        inset-inline-start: calc(\n          48px + var(--text-field-suffix-padding-left, 0px)\n        ) !important;\n        inset-inline-end: initial !important;\n        direction: var(--direction);\n      }\n\n      .mdc-text-field__input[type=\"number\"] {\n        direction: var(--direction);\n      }\n      .mdc-text-field__affix--prefix {\n        padding-right: var(--text-field-prefix-padding-right, 2px);\n      }\n\n      .mdc-text-field:not(.mdc-text-field--disabled)\n        .mdc-text-field__affix--prefix {\n        color: var(--mdc-text-field-label-ink-color);\n      }\n    `,\n    // safari workaround - must be explicit\n    mainWindow.document.dir === \"rtl\"\n      ? css`\n          .mdc-text-field__affix--suffix,\n          .mdc-text-field--with-leading-icon,\n          .mdc-text-field__icon--leading,\n          .mdc-floating-label,\n          .mdc-text-field--with-leading-icon.mdc-text-field--filled\n            .mdc-floating-label,\n          .mdc-text-field__input[type=\"number\"] {\n            direction: rtl;\n          }\n        `\n      : css``,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-textfield\": HaTextField;\n  }\n}\n",
-        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, CSSResult, PropertyValues, nothing } from \"lit\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, BinarySensorConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-binary-sensor-element\")\nexport class LCNConfigBinarySensorElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: BinarySensorConfig = {\n    source: \"BINSENSOR1\",\n  };\n\n  @state() private _sourceType!: ConfigItemCollection;\n\n  @state() private _source!: ConfigItem;\n\n  @query(\"#source-select\") private _sourceSelect!: HaSelect;\n\n  private get _binsensorPorts(): ConfigItem[] {\n    const binary_sensor: string = this.lcn.localize(\"binary-sensor\");\n    return [\n      { name: binary_sensor + \" 1\", value: \"BINSENSOR1\" },\n      { name: binary_sensor + \" 2\", value: \"BINSENSOR2\" },\n      { name: binary_sensor + \" 3\", value: \"BINSENSOR3\" },\n      { name: binary_sensor + \" 4\", value: \"BINSENSOR4\" },\n      { name: binary_sensor + \" 5\", value: \"BINSENSOR5\" },\n      { name: binary_sensor + \" 6\", value: \"BINSENSOR6\" },\n      { name: binary_sensor + \" 7\", value: \"BINSENSOR7\" },\n      { name: binary_sensor + \" 8\", value: \"BINSENSOR8\" },\n    ];\n  }\n\n  private get _setpoints(): ConfigItem[] {\n    const setpoint: string = this.lcn.localize(\"setpoint\");\n    return [\n      { name: setpoint + \" 1\", value: \"R1VARSETPOINT\" },\n      { name: setpoint + \" 2\", value: \"R2VARSETPOINT\" },\n    ];\n  }\n\n  private _keys: ConfigItem[] = [\n    { name: \"A1\", value: \"A1\" },\n    { name: \"A2\", value: \"A2\" },\n    { name: \"A3\", value: \"A3\" },\n    { name: \"A4\", value: \"A4\" },\n    { name: \"A5\", value: \"A5\" },\n    { name: \"A6\", value: \"A6\" },\n    { name: \"A7\", value: \"A7\" },\n    { name: \"A8\", value: \"A8\" },\n    { name: \"B1\", value: \"B1\" },\n    { name: \"B2\", value: \"B2\" },\n    { name: \"B3\", value: \"B3\" },\n    { name: \"B4\", value: \"B4\" },\n    { name: \"B5\", value: \"B5\" },\n    { name: \"B6\", value: \"B6\" },\n    { name: \"B7\", value: \"B7\" },\n    { name: \"B8\", value: \"B8\" },\n    { name: \"C1\", value: \"C1\" },\n    { name: \"C2\", value: \"C2\" },\n    { name: \"C3\", value: \"C3\" },\n    { name: \"C4\", value: \"C4\" },\n    { name: \"C5\", value: \"C5\" },\n    { name: \"C6\", value: \"C6\" },\n    { name: \"C7\", value: \"C7\" },\n    { name: \"C8\", value: \"C8\" },\n    { name: \"D1\", value: \"D1\" },\n    { name: \"D2\", value: \"D2\" },\n    { name: \"D3\", value: \"D3\" },\n    { name: \"D4\", value: \"D4\" },\n    { name: \"D5\", value: \"D5\" },\n    { name: \"D6\", value: \"D6\" },\n    { name: \"D7\", value: \"D7\" },\n    { name: \"D8\", value: \"D8\" },\n  ];\n\n  private get _sourceTypes(): ConfigItemCollection[] {\n    return [\n      {\n        name: this.lcn.localize(\"binary-sensor-type-binsensors\"),\n        value: this._binsensorPorts,\n        id: \"binsensors\",\n      },\n      {\n        name: this.lcn.localize(\"binary-sensor-type-setpoint-locks\"),\n        value: this._setpoints,\n        id: \"setpoint-locks\",\n      },\n      {\n        name: this.lcn.localize(\"binary-sensor-type-keys-locks\"),\n        value: this._keys,\n        id: \"key-locks\",\n      },\n    ];\n  }\n\n  protected async firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n    this._sourceType = this._sourceTypes[0];\n    this._source = this._sourceType.value[0];\n  }\n\n  protected render() {\n    if (!(this._sourceType || this._source)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"sources\">\n        <ha-select\n          id=\"source-type-select\"\n          .label=${this.lcn.localize(\"source-type\")}\n          .value=${this._sourceType.id}\n          fixedMenuPosition\n          @selected=${this._sourceTypeChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceTypes.map(\n            (sourceType) => html`\n              <ha-list-item .value=${sourceType.id}> ${sourceType.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"source-select\"\n          .label=${this.lcn.localize(\"source\")}\n          .value=${this._source.value}\n          fixedMenuPosition\n          @selected=${this._sourceChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceType.value.map(\n            (source) => html`\n              <ha-list-item .value=${source.value}> ${source.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n      </div>\n    `;\n  }\n\n  private _sourceTypeChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._sourceType = this._sourceTypes.find((sourceType) => sourceType.id === target.value)!;\n    this._source = this._sourceType.value[0];\n    this._sourceSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _sourceChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._source = this._sourceType.value.find((source) => source.value === target.value)!;\n    this.domainData.source = this._source.value;\n  }\n\n  static get styles(): CSSResult[] {\n    return [\n      haStyleDialog,\n      css`\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-binary-sensor-element\": LCNConfigBinarySensorElement;\n  }\n}\n",
-        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@ha/components/ha-textfield\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport \"@ha/components/ha-switch\";\nimport type { HaSwitch } from \"@ha/components/ha-switch\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport { LCN, ClimateConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\n@customElement(\"lcn-config-climate-element\")\nexport class LCNConfigClimateElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ type: Number }) public softwareSerial: number = -1;\n\n  @property({ attribute: false }) public domainData: ClimateConfig = {\n    source: \"VAR1\",\n    setpoint: \"R1VARSETPOINT\",\n    max_temp: 35,\n    min_temp: 7,\n    lockable: false,\n    unit_of_measurement: \"\u00b0C\",\n  };\n\n  @state() private _source!: ConfigItem;\n\n  @state() private _setpoint!: ConfigItem;\n\n  @state() private _unit!: ConfigItem;\n\n  private _invalid = false;\n\n  private get _is2012() {\n    return this.softwareSerial >= 0x160000;\n  }\n\n  private get _variablesNew(): ConfigItem[] {\n    const variable: string = this.lcn.localize(\"variable\");\n    return [\n      { name: variable + \" 1\", value: \"VAR1\" },\n      { name: variable + \" 2\", value: \"VAR2\" },\n      { name: variable + \" 3\", value: \"VAR3\" },\n      { name: variable + \" 4\", value: \"VAR4\" },\n      { name: variable + \" 5\", value: \"VAR5\" },\n      { name: variable + \" 6\", value: \"VAR6\" },\n      { name: variable + \" 7\", value: \"VAR7\" },\n      { name: variable + \" 8\", value: \"VAR8\" },\n      { name: variable + \" 9\", value: \"VAR9\" },\n      { name: variable + \" 10\", value: \"VAR10\" },\n      { name: variable + \" 11\", value: \"VAR11\" },\n      { name: variable + \" 12\", value: \"VAR12\" },\n    ];\n  }\n\n  private _variablesOld: ConfigItem[] = [\n    { name: \"TVar\", value: \"TVAR\" },\n    { name: \"R1Var\", value: \"R1VAR\" },\n    { name: \"R2Var\", value: \"R2VAR\" },\n  ];\n\n  private get _varSetpoints(): ConfigItem[] {\n    const setpoint: string = this.lcn.localize(\"setpoint\");\n    return [\n      { name: setpoint + \" 1\", value: \"R1VARSETPOINT\" },\n      { name: setpoint + \" 2\", value: \"R2VARSETPOINT\" },\n    ];\n  }\n\n  private _varUnits: ConfigItem[] = [\n    { name: \"Celsius\", value: \"\u00b0C\" },\n    { name: \"Fahrenheit\", value: \"\u00b0F\" },\n  ];\n\n  private get _sources(): ConfigItem[] {\n    return this._is2012 ? this._variablesNew : this._variablesOld;\n  }\n\n  private get _setpoints(): ConfigItem[] {\n    return this._is2012 ? this._varSetpoints.concat(this._variablesNew) : this._varSetpoints;\n  }\n\n  protected async firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n\n    this._source = this._sources[0];\n    this._setpoint = this._setpoints[0];\n    this._unit = this._varUnits[0];\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    super.willUpdate(changedProperties);\n    this._invalid =\n      !this._validateMinTemp(this.domainData.min_temp) ||\n      !this._validateMaxTemp(this.domainData.max_temp);\n  }\n\n  protected update(changedProperties: PropertyValues) {\n    super.update(changedProperties);\n    this.dispatchEvent(\n      new CustomEvent(\"validity-changed\", {\n        detail: this._invalid,\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n\n  protected render() {\n    if (!(this._source || this._setpoint || this._unit)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"sources\">\n        <ha-select\n          id=\"source-select\"\n          .label=${this.lcn.localize(\"source\")}\n          .value=${this._source.value}\n          fixedMenuPosition\n          @selected=${this._sourceChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sources.map(\n            (source) => html`\n              <ha-list-item .value=${source.value}> ${source.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"setpoint-select\"\n          .label=${this.lcn.localize(\"setpoint\")}\n          .value=${this._setpoint.value}\n          fixedMenuPosition\n          @selected=${this._setpointChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._setpoints.map(\n            (setpoint) => html`\n              <ha-list-item .value=${setpoint.value}> ${setpoint.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n      </div>\n\n      <div class=\"lockable\">\n        <label>${this.lcn.localize(\"dashboard-entities-dialog-climate-lockable\")}:</label>\n        <ha-switch\n          .checked=${this.domainData.lockable}\n          @change=${this._lockableChanged}\n        ></ha-switch>\n      </div>\n\n      <ha-textfield\n        id=\"min-textfield\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-climate-min-temperature\")}\n        type=\"number\"\n        .value=${this.domainData.min_temp.toString()}\n        required\n        autoValidate\n        @input=${this._minTempChanged}\n        .validityTransform=${this._validityTransformMinTemp}\n        .validationMessage=${this.lcn.localize(\n          \"dashboard-entities-dialog-climate-min-temperature-error\",\n        )}\n      ></ha-textfield>\n\n      <ha-textfield\n        id=\"max-textfield\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-climate-max-temperature\")}\n        type=\"number\"\n        .value=${this.domainData.max_temp.toString()}\n        required\n        autoValidate\n        @input=${this._maxTempChanged}\n        .validityTransform=${this._validityTransformMaxTemp}\n        .validationMessage=${this.lcn.localize(\n          \"dashboard-entities-dialog-climate-max-temperature-error\",\n        )}\n      ></ha-textfield>\n\n      <ha-select\n        id=\"unit-select\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-unit-of-measurement\")}\n        .value=${this._unit.value}\n        fixedMenuPosition\n        @selected=${this._unitChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._varUnits.map(\n          (unit) => html` <ha-list-item .value=${unit.value}> ${unit.name} </ha-list-item> `,\n        )}\n      </ha-select>\n    `;\n  }\n\n  private _sourceChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._source = this._sources.find((source) => source.value === target.value)!;\n    this.domainData.source = this._source.value;\n  }\n\n  private _setpointChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._setpoint = this._setpoints.find((setpoint) => setpoint.value === target.value)!;\n    this.domainData.setpoint = this._setpoint.value;\n  }\n\n  private _minTempChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.min_temp = +target.value;\n    const maxTextfield: HaTextField = this.shadowRoot!.querySelector(\"#max-textfield\")!;\n    maxTextfield.reportValidity();\n    this.requestUpdate();\n  }\n\n  private _maxTempChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.max_temp = +target.value;\n    const minTextfield: HaTextField = this.shadowRoot!.querySelector(\"#min-textfield\")!;\n    minTextfield.reportValidity();\n    this.requestUpdate();\n  }\n\n  private _lockableChanged(ev: ValueChangedEvent<string>): void {\n    this.domainData.lockable = (ev.target as HaSwitch).checked;\n  }\n\n  private _unitChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._unit = this._varUnits.find((unit) => unit.value === target.value)!;\n    this.domainData.unit_of_measurement = this._unit.value;\n  }\n\n  private _validateMaxTemp(max_temp: number): boolean {\n    return max_temp > this.domainData.min_temp;\n  }\n\n  private _validateMinTemp(min_temp: number): boolean {\n    return min_temp < this.domainData.max_temp;\n  }\n\n  private get _validityTransformMaxTemp() {\n    return (value: string) => ({ valid: this._validateMaxTemp(+value) });\n  }\n\n  private get _validityTransformMinTemp() {\n    return (value: string) => ({ valid: this._validateMinTemp(+value) });\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .lockable {\n          margin-top: 10px;\n        }\n        ha-switch {\n          margin-left: 25px;\n        }\n      `,\n    ];\n  }\n}\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-climate-element\": LCNConfigClimateElement;\n  }\n}\n",
-        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@polymer/paper-dropdown-menu/paper-dropdown-menu\";\nimport \"@polymer/paper-item/paper-item\";\nimport \"@polymer/paper-listbox/paper-listbox\";\nimport { css, html, LitElement, CSSResult, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, CoverConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\n@customElement(\"lcn-config-cover-element\")\nexport class LCNConfigCoverElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: CoverConfig = {\n    motor: \"MOTOR1\",\n    reverse_time: \"RT1200\",\n  };\n\n  @state() private _motor!: ConfigItem;\n\n  @state() private _reverseDelay!: ConfigItem;\n\n  private get _motors(): ConfigItem[] {\n    const motor: string = this.lcn.localize(\"motor\");\n    return [\n      { name: motor + \" 1\", value: \"MOTOR1\" },\n      { name: motor + \" 2\", value: \"MOTOR2\" },\n      { name: motor + \" 3\", value: \"MOTOR3\" },\n      { name: motor + \" 4\", value: \"MOTOR4\" },\n      { name: this.lcn.localize(\"outputs\"), value: \"OUTPUTS\" },\n    ];\n  }\n\n  private _reverseDelays: ConfigItem[] = [\n    { name: \"70ms\", value: \"RT70\" },\n    { name: \"600ms\", value: \"RT600\" },\n    { name: \"1200ms\", value: \"RT1200\" },\n  ];\n\n  protected async firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n    this._motor = this._motors[0];\n    this._reverseDelay = this._reverseDelays[0];\n  }\n\n  protected render() {\n    if (!(this._motor || this._reverseDelay)) {\n      return nothing;\n    }\n    return html`\n      <ha-select\n        id=\"motor-select\"\n        .label=${this.lcn.localize(\"motor\")}\n        .value=${this._motor.value}\n        fixedMenuPosition\n        @selected=${this._motorChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._motors.map(\n          (motor) => html` <ha-list-item .value=${motor.value}> ${motor.name} </ha-list-item> `,\n        )}\n      </ha-select>\n\n      ${this._motor.value === \"OUTPUTS\"\n        ? html`\n            <ha-select\n              id=\"reverse-delay-select\"\n              .label=${this.lcn.localize(\"reverse-delay\")}\n              .value=${this._reverseDelay.value}\n              fixedMenuPosition\n              @selected=${this._reverseDelayChanged}\n              @closed=${stopPropagation}\n            >\n              ${this._reverseDelays.map(\n                (reverseDelay) => html`\n                  <ha-list-item .value=${reverseDelay.value}> ${reverseDelay.name} </ha-list-item>\n                `,\n              )}\n            </ha-select>\n          `\n        : nothing}\n    `;\n  }\n\n  private _motorChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._motor = this._motors.find((motor) => motor.value === target.value)!;\n    this._reverseDelay = this._reverseDelays[0];\n    this.domainData.motor = this._motor.value;\n  }\n\n  private _reverseDelayChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._reverseDelay = this._reverseDelays.find(\n      (reverseDelay) => reverseDelay.value === target.value,\n    )!;\n    this.domainData.reverse_time = this._reverseDelay.value;\n  }\n\n  static get styles(): CSSResult[] {\n    return [\n      haStyleDialog,\n      css`\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-cover-element\": LCNConfigCoverElement;\n  }\n}\n",
-        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@ha/components/ha-radio\";\nimport \"@ha/components/ha-formfield\";\nimport \"@ha/components/ha-textfield\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HaRadio } from \"@ha/components/ha-radio\";\nimport type { HaSwitch } from \"@ha/components/ha-switch\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, LightConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-light-element\")\nexport class LCNConfigLightElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: LightConfig = {\n    output: \"OUTPUT1\",\n    dimmable: false,\n    transition: 0,\n  };\n\n  @state() private _portType!: ConfigItemCollection;\n\n  @state() private _port!: ConfigItem;\n\n  @query(\"#port-select\") private _portSelect;\n\n  private _invalid = false;\n\n  private get _outputPorts(): ConfigItem[] {\n    const output: string = this.lcn.localize(\"output\");\n    return [\n      { name: output + \" 1\", value: \"OUTPUT1\" },\n      { name: output + \" 2\", value: \"OUTPUT2\" },\n      { name: output + \" 3\", value: \"OUTPUT3\" },\n      { name: output + \" 4\", value: \"OUTPUT4\" },\n    ];\n  }\n\n  private get _relayPorts(): ConfigItem[] {\n    const relay: string = this.lcn.localize(\"relay\");\n    return [\n      { name: relay + \" 1\", value: \"RELAY1\" },\n      { name: relay + \" 2\", value: \"RELAY2\" },\n      { name: relay + \" 3\", value: \"RELAY3\" },\n      { name: relay + \" 4\", value: \"RELAY4\" },\n      { name: relay + \" 5\", value: \"RELAY5\" },\n      { name: relay + \" 6\", value: \"RELAY6\" },\n      { name: relay + \" 7\", value: \"RELAY7\" },\n      { name: relay + \" 8\", value: \"RELAY8\" },\n    ];\n  }\n\n  private get _portTypes(): ConfigItemCollection[] {\n    return [\n      { name: this.lcn.localize(\"output\"), value: this._outputPorts, id: \"output\" },\n      { name: this.lcn.localize(\"relay\"), value: this._relayPorts, id: \"relay\" },\n    ];\n  }\n\n  protected async firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n    this._portType = this._portTypes[0];\n    this._port = this._portType.value[0];\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    super.willUpdate(changedProperties);\n    this._invalid = !this._validateTransition(this.domainData.transition);\n  }\n\n  protected update(changedProperties: PropertyValues) {\n    super.update(changedProperties);\n    this.dispatchEvent(\n      new CustomEvent(\"validity-changed\", {\n        detail: this._invalid,\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n\n  protected render() {\n    if (!(this._portType || this._port)) {\n      return nothing;\n    }\n    return html`\n      <div id=\"port-type\">${this.lcn.localize(\"port-type\")}</div>\n\n      <ha-formfield label=${this.lcn.localize(\"output\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"output\"\n          .checked=${this._portType.id === \"output\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-formfield label=${this.lcn.localize(\"relay\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"relay\"\n          .checked=${this._portType.id === \"relay\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-select\n        id=\"port-select\"\n        .label=${this.lcn.localize(\"port\")}\n        .value=${this._port.value}\n        fixedMenuPosition\n        @selected=${this._portChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._portType.value.map(\n          (port) => html` <ha-list-item .value=${port.value}> ${port.name} </ha-list-item> `,\n        )}\n      </ha-select>\n\n      ${this.renderOutputFeatures()}\n    `;\n  }\n\n  private renderOutputFeatures() {\n    switch (this._portType.id) {\n      case \"output\":\n        return html`\n          <div id=\"dimmable\">\n            <label>${this.lcn.localize(\"dashboard-entities-dialog-light-dimmable\")}:</label>\n\n            <ha-switch\n              .checked=${this.domainData.dimmable}\n              @change=${this._dimmableChanged}\n            ></ha-switch>\n          </div>\n\n          <ha-textfield\n            id=\"transition\"\n            .label=${this.lcn.localize(\"dashboard-entities-dialog-light-transition\")}\n            type=\"number\"\n            .value=${this.domainData.transition.toString()}\n            min=\"0\"\n            max=\"486\"\n            required\n            autoValidate\n            @input=${this._transitionChanged}\n            .validityTransform=${this._validityTransformTransition}\n            .validationMessage=${this.lcn.localize(\n              \"dashboard-entities-dialog-light-transition-error\",\n            )}\n          ></ha-textfield>\n        `;\n      case \"relay\":\n        return nothing;\n      default:\n        return nothing;\n    }\n  }\n\n  private _portTypeChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaRadio;\n\n    this._portType = this._portTypes.find((portType) => portType.id === target.value)!;\n    this._port = this._portType.value[0];\n    this._portSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _portChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._port = this._portType.value.find((portType) => portType.value === target.value)!;\n    this.domainData.output = this._port.value;\n  }\n\n  private _dimmableChanged(ev: ValueChangedEvent<boolean>): void {\n    this.domainData.dimmable = (ev.target as HaSwitch).checked;\n  }\n\n  private _transitionChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.transition = +target.value;\n    this.requestUpdate();\n  }\n\n  private _validateTransition(transition: number): boolean {\n    return transition >= 0 && transition <= 486;\n  }\n\n  private get _validityTransformTransition() {\n    return (value: string) => ({ valid: this._validateTransition(+value) });\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        #dimmable {\n          margin-top: 16px;\n        }\n        #transition {\n          margin-top: 16px;\n        }\n      `,\n    ];\n  }\n}\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-light-element\": LCNConfigLightElement;\n  }\n}\n",
-        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@ha/components/ha-textfield\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport \"@ha/components/ha-checkbox\";\nimport \"@ha/components/ha-formfield\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, SceneConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\n@customElement(\"lcn-config-scene-element\")\nexport class LCNConfigSceneElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: SceneConfig = {\n    register: 0,\n    scene: 0,\n    outputs: [],\n    transition: 0,\n  };\n\n  @state() private _register!: ConfigItem;\n\n  @state() private _scene!: ConfigItem;\n\n  private _invalid = false;\n\n  private get _registers(): ConfigItem[] {\n    const register: string = this.lcn.localize(\"register\");\n    return [\n      { name: register + \" 0\", value: \"0\" },\n      { name: register + \" 1\", value: \"1\" },\n      { name: register + \" 2\", value: \"2\" },\n      { name: register + \" 3\", value: \"3\" },\n      { name: register + \" 4\", value: \"4\" },\n      { name: register + \" 5\", value: \"5\" },\n      { name: register + \" 6\", value: \"6\" },\n      { name: register + \" 7\", value: \"7\" },\n      { name: register + \" 8\", value: \"8\" },\n      { name: register + \" 9\", value: \"9\" },\n    ];\n  }\n\n  private get _scenes(): ConfigItem[] {\n    const scene: string = this.lcn.localize(\"scene\");\n    return [\n      { name: scene + \" 1\", value: \"0\" },\n      { name: scene + \" 2\", value: \"1\" },\n      { name: scene + \" 3\", value: \"2\" },\n      { name: scene + \" 4\", value: \"3\" },\n      { name: scene + \" 5\", value: \"4\" },\n      { name: scene + \" 6\", value: \"5\" },\n      { name: scene + \" 7\", value: \"6\" },\n      { name: scene + \" 8\", value: \"7\" },\n      { name: scene + \" 9\", value: \"8\" },\n      { name: scene + \" 10\", value: \"9\" },\n    ];\n  }\n\n  private get _outputPorts(): ConfigItem[] {\n    const output: string = this.lcn.localize(\"output\");\n    return [\n      { name: output + \" 1\", value: \"OUTPUT1\" },\n      { name: output + \" 2\", value: \"OUTPUT2\" },\n      { name: output + \" 3\", value: \"OUTPUT3\" },\n      { name: output + \" 4\", value: \"OUTPUT4\" },\n    ];\n  }\n\n  private get _relayPorts(): ConfigItem[] {\n    const relay: string = this.lcn.localize(\"relay\");\n    return [\n      { name: relay + \" 1\", value: \"RELAY1\" },\n      { name: relay + \" 2\", value: \"RELAY2\" },\n      { name: relay + \" 3\", value: \"RELAY3\" },\n      { name: relay + \" 4\", value: \"RELAY4\" },\n      { name: relay + \" 5\", value: \"RELAY5\" },\n      { name: relay + \" 6\", value: \"RELAY6\" },\n      { name: relay + \" 7\", value: \"RELAY7\" },\n      { name: relay + \" 8\", value: \"RELAY8\" },\n    ];\n  }\n\n  protected async firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n\n    this._register = this._registers[0];\n    this._scene = this._scenes[0];\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    super.willUpdate(changedProperties);\n    this._invalid = !this._validateTransition(this.domainData.transition);\n  }\n\n  protected update(changedProperties: PropertyValues) {\n    super.update(changedProperties);\n    this.dispatchEvent(\n      new CustomEvent(\"validity-changed\", {\n        detail: this._invalid,\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n\n  protected render() {\n    if (!(this._register || this._scene)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"registers\">\n        <ha-select\n          id=\"register-select\"\n          .label=${this.lcn.localize(\"register\")}\n          .value=${this._register.value}\n          fixedMenuPosition\n          @selected=${this._registerChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._registers.map(\n            (register) => html`\n              <ha-list-item .value=${register.value}> ${register.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"scene-select\"\n          .label=${this.lcn.localize(\"scene\")}\n          .value=${this._scene.value}\n          fixedMenuPosition\n          @selected=${this._sceneChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._scenes.map(\n            (scene) => html` <ha-list-item .value=${scene.value}> ${scene.name} </ha-list-item> `,\n          )}\n        </ha-select>\n      </div>\n\n      <div class=\"ports\">\n        <label>${this.lcn.localize(\"outputs\")}:</label><br />\n        ${this._outputPorts.map(\n          (port) => html`\n            <ha-formfield label=${port.name}>\n              <ha-checkbox .value=${port.value} @change=${this._portCheckedChanged}></ha-checkbox>\n            </ha-formfield>\n          `,\n        )}\n      </div>\n\n      <div class=\"ports\">\n        <label>${this.lcn.localize(\"relays\")}:</label><br />\n        ${this._relayPorts.map(\n          (port) => html`\n            <ha-formfield label=${port.name}>\n              <ha-checkbox .value=${port.value} @change=${this._portCheckedChanged}></ha-checkbox>\n            </ha-formfield>\n          `,\n        )}\n      </div>\n\n      <ha-textfield\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-scene-transition\")}\n        type=\"number\"\n        .value=${this.domainData.transition.toString()}\n        min=\"0\"\n        max=\"486\"\n        required\n        autoValidate\n        @input=${this._transitionChanged}\n        .validityTransform=${this._validityTransformTransition}\n        .disabled=${this._transitionDisabled}\n        .validationMessage=${this.lcn.localize(\"dashboard-entities-dialog-scene-transition-error\")}\n      ></ha-textfield>\n    `;\n  }\n\n  private _registerChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._register = this._registers.find((register) => register.value === target.value)!;\n    this.domainData.register = +this._register.value;\n  }\n\n  private _sceneChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._scene = this._scenes.find((scene) => scene.value === target.value)!;\n    this.domainData.scene = +this._scene.value;\n  }\n\n  private _portCheckedChanged(ev: ValueChangedEvent<string> | any): void {\n    if (ev.target.checked) {\n      this.domainData.outputs.push(ev.target.value);\n    } else {\n      this.domainData.outputs = this.domainData.outputs.filter((port) => ev.target.value !== port);\n    }\n    this.requestUpdate();\n  }\n\n  private _transitionChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.transition = +target.value;\n    this.requestUpdate();\n  }\n\n  private _validateTransition(transition: number): boolean {\n    return transition >= 0 && transition <= 486;\n  }\n\n  private get _validityTransformTransition() {\n    return (value: string) => ({ valid: this._validateTransition(+value) });\n  }\n\n  private get _transitionDisabled(): boolean {\n    const outputPortValues = this._outputPorts.map((port) => port.value);\n    return (\n      this.domainData.outputs.filter((output) => outputPortValues.includes(output)).length === 0\n    );\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        .registers {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .ports {\n          margin-top: 10px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-scene-element\": LCNConfigSceneElement;\n  }\n}\n",
-        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport type { LCN, SensorConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-sensor-element\")\nexport class LCNConfigSensorElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ type: Number }) public softwareSerial: number = -1;\n\n  @property({ attribute: false }) public domainData: SensorConfig = {\n    source: \"VAR1\",\n    unit_of_measurement: \"NATIVE\",\n  };\n\n  @state() private _sourceType!: ConfigItemCollection;\n\n  @state() private _source!: ConfigItem;\n\n  @state() private _unit!: ConfigItem;\n\n  @query(\"#source-select\") private _sourceSelect!: HaSelect;\n\n  private get _is2013() {\n    return this.softwareSerial >= 0x170206;\n  }\n\n  private _variablesOld: ConfigItem[] = [\n    { name: \"TVar\", value: \"TVAR\" },\n    { name: \"R1Var\", value: \"R1VAR\" },\n    { name: \"R2Var\", value: \"R2VAR\" },\n  ];\n\n  private get _variablesNew(): ConfigItem[] {\n    const variable: string = this.lcn.localize(\"variable\");\n    return [\n      { name: variable + \" 1\", value: \"VAR1\" },\n      { name: variable + \" 2\", value: \"VAR2\" },\n      { name: variable + \" 3\", value: \"VAR3\" },\n      { name: variable + \" 4\", value: \"VAR4\" },\n      { name: variable + \" 5\", value: \"VAR5\" },\n      { name: variable + \" 6\", value: \"VAR6\" },\n      { name: variable + \" 7\", value: \"VAR7\" },\n      { name: variable + \" 8\", value: \"VAR8\" },\n      { name: variable + \" 9\", value: \"VAR9\" },\n      { name: variable + \" 10\", value: \"VAR10\" },\n      { name: variable + \" 11\", value: \"VAR11\" },\n      { name: variable + \" 12\", value: \"VAR12\" },\n    ];\n  }\n\n  private get _setpoints(): ConfigItem[] {\n    const setpoint: string = this.lcn.localize(\"setpoint\");\n    return [\n      { name: setpoint + \" 1\", value: \"R1VARSETPOINT\" },\n      { name: setpoint + \" 2\", value: \"R2VARSETPOINT\" },\n    ];\n  }\n\n  private get _thresholdsOld(): ConfigItem[] {\n    const threshold: string = this.lcn.localize(\"threshold\");\n    return [\n      { name: threshold + \" 1\", value: \"THRS1\" },\n      { name: threshold + \" 2\", value: \"THRS2\" },\n      { name: threshold + \" 3\", value: \"THRS3\" },\n      { name: threshold + \" 4\", value: \"THRS4\" },\n      { name: threshold + \" 5\", value: \"THRS5\" },\n    ];\n  }\n\n  private get _thresholdsNew(): ConfigItem[] {\n    const threshold: string = this.lcn.localize(\"threshold\");\n    return [\n      { name: threshold + \" 1-1\", value: \"THRS1\" },\n      { name: threshold + \" 1-2\", value: \"THRS2\" },\n      { name: threshold + \" 1-3\", value: \"THRS3\" },\n      { name: threshold + \" 1-4\", value: \"THRS4\" },\n      { name: threshold + \" 2-1\", value: \"THRS2_1\" },\n      { name: threshold + \" 2-2\", value: \"THRS2_2\" },\n      { name: threshold + \" 2-3\", value: \"THRS2_3\" },\n      { name: threshold + \" 2-4\", value: \"THRS2_4\" },\n      { name: threshold + \" 3-1\", value: \"THRS3_1\" },\n      { name: threshold + \" 3-2\", value: \"THRS3_2\" },\n      { name: threshold + \" 3-3\", value: \"THRS3_3\" },\n      { name: threshold + \" 3-4\", value: \"THRS3_4\" },\n      { name: threshold + \" 4-1\", value: \"THRS4_1\" },\n      { name: threshold + \" 4-2\", value: \"THRS4_2\" },\n      { name: threshold + \" 4-3\", value: \"THRS4_3\" },\n      { name: threshold + \" 4-4\", value: \"THRS4_4\" },\n    ];\n  }\n\n  private get _s0Inputs(): ConfigItem[] {\n    const s0input: string = this.lcn.localize(\"s0input\");\n    return [\n      { name: s0input + \" 1\", value: \"S0INPUT1\" },\n      { name: s0input + \" 2\", value: \"S0INPUT2\" },\n      { name: s0input + \" 3\", value: \"S0INPUT3\" },\n      { name: s0input + \" 4\", value: \"S0INPUT4\" },\n    ];\n  }\n\n  private get _ledPorts(): ConfigItem[] {\n    const led: string = this.lcn.localize(\"led\");\n    return [\n      { name: led + \" 1\", value: \"LED1\" },\n      { name: led + \" 2\", value: \"LED2\" },\n      { name: led + \" 3\", value: \"LED3\" },\n      { name: led + \" 4\", value: \"LED4\" },\n      { name: led + \" 5\", value: \"LED5\" },\n      { name: led + \" 6\", value: \"LED6\" },\n      { name: led + \" 7\", value: \"LED7\" },\n      { name: led + \" 8\", value: \"LED8\" },\n      { name: led + \" 9\", value: \"LED9\" },\n      { name: led + \" 10\", value: \"LED10\" },\n      { name: led + \" 11\", value: \"LED11\" },\n      { name: led + \" 12\", value: \"LED12\" },\n    ];\n  }\n\n  private get _logicOpPorts(): ConfigItem[] {\n    const logic: string = this.lcn.localize(\"logic\");\n    return [\n      { name: logic + \" 1\", value: \"LOGICOP1\" },\n      { name: logic + \" 2\", value: \"LOGICOP2\" },\n      { name: logic + \" 3\", value: \"LOGICOP3\" },\n      { name: logic + \" 4\", value: \"LOGICOP4\" },\n    ];\n  }\n\n  private get _sourceTypes(): ConfigItemCollection[] {\n    return [\n      {\n        name: this.lcn.localize(\"variables\"),\n        value: this._is2013 ? this._variablesNew : this._variablesOld,\n        id: \"variables\",\n      },\n      {\n        name: this.lcn.localize(\"setpoints\"),\n        value: this._setpoints,\n        id: \"setpoints\",\n      },\n      {\n        name: this.lcn.localize(\"thresholds\"),\n        value: this._is2013 ? this._thresholdsNew : this._thresholdsOld,\n        id: \"thresholds\",\n      },\n      { name: this.lcn.localize(\"s0inputs\"), value: this._s0Inputs, id: \"s0inputs\" },\n      { name: this.lcn.localize(\"leds\"), value: this._ledPorts, id: \"ledports\" },\n      { name: this.lcn.localize(\"logics\"), value: this._logicOpPorts, id: \"logicopports\" },\n    ];\n  }\n\n  private get _varUnits(): ConfigItem[] {\n    return [\n      { name: this.lcn.localize(\"unit-lcn-native\"), value: \"NATIVE\" },\n      { name: \"Celsius\", value: \"\u00b0C\" },\n      { name: \"Fahrenheit\", value: \"\u00b0F\" },\n      { name: \"Kelvin\", value: \"K\" },\n      { name: \"Lux\", value: \"LUX_T\" },\n      { name: \"Lux (I-Port)\", value: \"LUX_I\" },\n      { name: this.lcn.localize(\"unit-humidity\") + \" (%)\", value: \"PERCENT\" },\n      { name: \"CO2 (\u2030)\", value: \"PPM\" },\n      { name: this.lcn.localize(\"unit-wind\") + \" (m/s)\", value: \"METERPERSECOND\" },\n      { name: this.lcn.localize(\"unit-volts\"), value: \"VOLT\" },\n      { name: this.lcn.localize(\"unit-milliamperes\"), value: \"AMPERE\" },\n      { name: this.lcn.localize(\"unit-angle\") + \" (\u00b0)\", value: \"DEGREE\" },\n    ];\n  }\n\n  protected async firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n\n    this._sourceType = this._sourceTypes[0];\n    this._source = this._sourceType.value[0];\n    this._unit = this._varUnits[0];\n  }\n\n  protected render() {\n    if (!(this._sourceType || this._source)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"sources\">\n        <ha-select\n          id=\"source-type-select\"\n          .label=${this.lcn.localize(\"source-type\")}\n          .value=${this._sourceType.id}\n          fixedMenuPosition\n          @selected=${this._sourceTypeChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceTypes.map(\n            (sourceType) => html`\n              <ha-list-item .value=${sourceType.id}> ${sourceType.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"source-select\"\n          .label=${this.lcn.localize(\"source\")}\n          .value=${this._source.value}\n          fixedMenuPosition\n          @selected=${this._sourceChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceType.value.map(\n            (source) => html`\n              <ha-list-item .value=${source.value}> ${source.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n      </div>\n\n      <ha-select\n        id=\"unit-select\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-unit-of-measurement\")}\n        .value=${this._unit.value}\n        fixedMenuPosition\n        @selected=${this._unitChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._varUnits.map(\n          (unit) => html` <ha-list-item .value=${unit.value}> ${unit.name} </ha-list-item> `,\n        )}\n      </ha-select>\n    `;\n  }\n\n  private _sourceTypeChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._sourceType = this._sourceTypes.find((sourceType) => sourceType.id === target.value)!;\n    this._source = this._sourceType.value[0];\n    this._sourceSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _sourceChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._source = this._sourceType.value.find((source) => source.value === target.value)!;\n    this.domainData.source = this._source.value;\n  }\n\n  private _unitChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._unit = this._varUnits.find((unit) => unit.value === target.value)!;\n    this.domainData.unit_of_measurement = this._unit.value;\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-sensor-element\": LCNConfigSensorElement;\n  }\n}\n",
-        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, SwitchConfig } from \"types/lcn\";\nimport \"@ha/components/ha-radio\";\nimport \"@ha/components/ha-formfield\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport type { HaRadio } from \"@ha/components/ha-radio\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-switch-element\")\nexport class LCNConfigSwitchElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: SwitchConfig = { output: \"OUTPUT1\" };\n\n  @state() private _portType!: ConfigItemCollection;\n\n  @state() private _port!: ConfigItem;\n\n  @query(\"#port-select\") private _portSelect;\n\n  private get _outputPorts(): ConfigItem[] {\n    const output: string = this.lcn.localize(\"output\");\n    return [\n      { name: output + \" 1\", value: \"OUTPUT1\" },\n      { name: output + \" 2\", value: \"OUTPUT2\" },\n      { name: output + \" 3\", value: \"OUTPUT3\" },\n      { name: output + \" 4\", value: \"OUTPUT4\" },\n    ];\n  }\n\n  private get _relayPorts(): ConfigItem[] {\n    const relay: string = this.lcn.localize(\"relay\");\n    return [\n      { name: relay + \" 1\", value: \"RELAY1\" },\n      { name: relay + \" 2\", value: \"RELAY2\" },\n      { name: relay + \" 3\", value: \"RELAY3\" },\n      { name: relay + \" 4\", value: \"RELAY4\" },\n      { name: relay + \" 5\", value: \"RELAY5\" },\n      { name: relay + \" 6\", value: \"RELAY6\" },\n      { name: relay + \" 7\", value: \"RELAY7\" },\n      { name: relay + \" 8\", value: \"RELAY8\" },\n    ];\n  }\n\n  private get _portTypes(): ConfigItemCollection[] {\n    return [\n      { name: this.lcn.localize(\"output\"), value: this._outputPorts, id: \"output\" },\n      { name: this.lcn.localize(\"relay\"), value: this._relayPorts, id: \"relay\" },\n    ];\n  }\n\n  protected async firstUpdated(changedProperties: PropertyValues) {\n    super.firstUpdated(changedProperties);\n    this._portType = this._portTypes[0];\n    this._port = this._portType.value[0];\n  }\n\n  protected render() {\n    if (!(this._portType || this._port)) {\n      return nothing;\n    }\n    return html`\n      <div id=\"port-type\">${this.lcn.localize(\"port-type\")}</div>\n\n      <ha-formfield label=${this.lcn.localize(\"output\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"output\"\n          .checked=${this._portType.id === \"output\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-formfield label=${this.lcn.localize(\"relay\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"relay\"\n          .checked=${this._portType.id === \"relay\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-select\n        id=\"port-select\"\n        .label=${this.lcn.localize(\"port\")}\n        .value=${this._port.value}\n        fixedMenuPosition\n        @selected=${this._portChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._portType.value.map(\n          (port) => html` <ha-list-item .value=${port.value}> ${port.name} </ha-list-item> `,\n        )}\n      </ha-select>\n    `;\n  }\n\n  private _portTypeChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaRadio;\n\n    this._portType = this._portTypes.find((portType) => portType.id === target.value)!;\n    this._port = this._portType.value[0];\n    this._portSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _portChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._port = this._portType.value.find((portType) => portType.value === target.value)!;\n    this.domainData.output = this._port.value;\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-switch-element\": LCNConfigSwitchElement;\n  }\n}\n",
+        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, CSSResult, nothing } from \"lit\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, BinarySensorConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-binary-sensor-element\")\nexport class LCNConfigBinarySensorElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: BinarySensorConfig = {\n    source: \"BINSENSOR1\",\n  };\n\n  @state() private _sourceType!: ConfigItemCollection;\n\n  @state() private _source!: ConfigItem;\n\n  @query(\"#source-select\") private _sourceSelect!: HaSelect;\n\n  private get _binsensorPorts(): ConfigItem[] {\n    const binary_sensor: string = this.lcn.localize(\"binary-sensor\");\n    return [\n      { name: binary_sensor + \" 1\", value: \"BINSENSOR1\" },\n      { name: binary_sensor + \" 2\", value: \"BINSENSOR2\" },\n      { name: binary_sensor + \" 3\", value: \"BINSENSOR3\" },\n      { name: binary_sensor + \" 4\", value: \"BINSENSOR4\" },\n      { name: binary_sensor + \" 5\", value: \"BINSENSOR5\" },\n      { name: binary_sensor + \" 6\", value: \"BINSENSOR6\" },\n      { name: binary_sensor + \" 7\", value: \"BINSENSOR7\" },\n      { name: binary_sensor + \" 8\", value: \"BINSENSOR8\" },\n    ];\n  }\n\n  private get _setpoints(): ConfigItem[] {\n    const setpoint: string = this.lcn.localize(\"setpoint\");\n    return [\n      { name: setpoint + \" 1\", value: \"R1VARSETPOINT\" },\n      { name: setpoint + \" 2\", value: \"R2VARSETPOINT\" },\n    ];\n  }\n\n  private _keys: ConfigItem[] = [\n    { name: \"A1\", value: \"A1\" },\n    { name: \"A2\", value: \"A2\" },\n    { name: \"A3\", value: \"A3\" },\n    { name: \"A4\", value: \"A4\" },\n    { name: \"A5\", value: \"A5\" },\n    { name: \"A6\", value: \"A6\" },\n    { name: \"A7\", value: \"A7\" },\n    { name: \"A8\", value: \"A8\" },\n    { name: \"B1\", value: \"B1\" },\n    { name: \"B2\", value: \"B2\" },\n    { name: \"B3\", value: \"B3\" },\n    { name: \"B4\", value: \"B4\" },\n    { name: \"B5\", value: \"B5\" },\n    { name: \"B6\", value: \"B6\" },\n    { name: \"B7\", value: \"B7\" },\n    { name: \"B8\", value: \"B8\" },\n    { name: \"C1\", value: \"C1\" },\n    { name: \"C2\", value: \"C2\" },\n    { name: \"C3\", value: \"C3\" },\n    { name: \"C4\", value: \"C4\" },\n    { name: \"C5\", value: \"C5\" },\n    { name: \"C6\", value: \"C6\" },\n    { name: \"C7\", value: \"C7\" },\n    { name: \"C8\", value: \"C8\" },\n    { name: \"D1\", value: \"D1\" },\n    { name: \"D2\", value: \"D2\" },\n    { name: \"D3\", value: \"D3\" },\n    { name: \"D4\", value: \"D4\" },\n    { name: \"D5\", value: \"D5\" },\n    { name: \"D6\", value: \"D6\" },\n    { name: \"D7\", value: \"D7\" },\n    { name: \"D8\", value: \"D8\" },\n  ];\n\n  private get _sourceTypes(): ConfigItemCollection[] {\n    return [\n      {\n        name: this.lcn.localize(\"binary-sensor-type-binsensors\"),\n        value: this._binsensorPorts,\n        id: \"binsensors\",\n      },\n      {\n        name: this.lcn.localize(\"binary-sensor-type-setpoint-locks\"),\n        value: this._setpoints,\n        id: \"setpoint-locks\",\n      },\n      {\n        name: this.lcn.localize(\"binary-sensor-type-keys-locks\"),\n        value: this._keys,\n        id: \"key-locks\",\n      },\n    ];\n  }\n\n  public connectedCallback(): void {\n    super.connectedCallback();\n    this._sourceType = this._sourceTypes[0];\n    this._source = this._sourceType.value[0];\n  }\n\n  protected render() {\n    if (!(this._sourceType || this._source)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"sources\">\n        <ha-select\n          id=\"source-type-select\"\n          .label=${this.lcn.localize(\"source-type\")}\n          .value=${this._sourceType.id}\n          fixedMenuPosition\n          @selected=${this._sourceTypeChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceTypes.map(\n            (sourceType) => html`\n              <ha-list-item .value=${sourceType.id}> ${sourceType.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"source-select\"\n          .label=${this.lcn.localize(\"source\")}\n          .value=${this._source.value}\n          fixedMenuPosition\n          @selected=${this._sourceChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceType.value.map(\n            (source) => html`\n              <ha-list-item .value=${source.value}> ${source.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n      </div>\n    `;\n  }\n\n  private _sourceTypeChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._sourceType = this._sourceTypes.find((sourceType) => sourceType.id === target.value)!;\n    this._source = this._sourceType.value[0];\n    this._sourceSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _sourceChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._source = this._sourceType.value.find((source) => source.value === target.value)!;\n    this.domainData.source = this._source.value;\n  }\n\n  static get styles(): CSSResult[] {\n    return [\n      haStyleDialog,\n      css`\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-binary-sensor-element\": LCNConfigBinarySensorElement;\n  }\n}\n",
+        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@ha/components/ha-textfield\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport \"@ha/components/ha-switch\";\nimport type { HaSwitch } from \"@ha/components/ha-switch\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport { LCN, ClimateConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\n@customElement(\"lcn-config-climate-element\")\nexport class LCNConfigClimateElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ type: Number }) public softwareSerial: number = -1;\n\n  @property({ attribute: false }) public domainData: ClimateConfig = {\n    source: \"VAR1\",\n    setpoint: \"R1VARSETPOINT\",\n    max_temp: 35,\n    min_temp: 7,\n    lockable: false,\n    unit_of_measurement: \"\u00b0C\",\n  };\n\n  @state() private _source!: ConfigItem;\n\n  @state() private _setpoint!: ConfigItem;\n\n  @state() private _unit!: ConfigItem;\n\n  private _invalid = false;\n\n  private get _is2012() {\n    return this.softwareSerial >= 0x160000;\n  }\n\n  private get _variablesNew(): ConfigItem[] {\n    const variable: string = this.lcn.localize(\"variable\");\n    return [\n      { name: variable + \" 1\", value: \"VAR1\" },\n      { name: variable + \" 2\", value: \"VAR2\" },\n      { name: variable + \" 3\", value: \"VAR3\" },\n      { name: variable + \" 4\", value: \"VAR4\" },\n      { name: variable + \" 5\", value: \"VAR5\" },\n      { name: variable + \" 6\", value: \"VAR6\" },\n      { name: variable + \" 7\", value: \"VAR7\" },\n      { name: variable + \" 8\", value: \"VAR8\" },\n      { name: variable + \" 9\", value: \"VAR9\" },\n      { name: variable + \" 10\", value: \"VAR10\" },\n      { name: variable + \" 11\", value: \"VAR11\" },\n      { name: variable + \" 12\", value: \"VAR12\" },\n    ];\n  }\n\n  private _variablesOld: ConfigItem[] = [\n    { name: \"TVar\", value: \"TVAR\" },\n    { name: \"R1Var\", value: \"R1VAR\" },\n    { name: \"R2Var\", value: \"R2VAR\" },\n  ];\n\n  private get _varSetpoints(): ConfigItem[] {\n    const setpoint: string = this.lcn.localize(\"setpoint\");\n    return [\n      { name: setpoint + \" 1\", value: \"R1VARSETPOINT\" },\n      { name: setpoint + \" 2\", value: \"R2VARSETPOINT\" },\n    ];\n  }\n\n  private _varUnits: ConfigItem[] = [\n    { name: \"Celsius\", value: \"\u00b0C\" },\n    { name: \"Fahrenheit\", value: \"\u00b0F\" },\n  ];\n\n  private get _sources(): ConfigItem[] {\n    return this._is2012 ? this._variablesNew : this._variablesOld;\n  }\n\n  private get _setpoints(): ConfigItem[] {\n    return this._is2012 ? this._varSetpoints.concat(this._variablesNew) : this._varSetpoints;\n  }\n\n  public connectedCallback(): void {\n    super.connectedCallback();\n    this._source = this._sources[0];\n    this._setpoint = this._setpoints[0];\n    this._unit = this._varUnits[0];\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    super.willUpdate(changedProperties);\n    this._invalid =\n      !this._validateMinTemp(this.domainData.min_temp) ||\n      !this._validateMaxTemp(this.domainData.max_temp);\n  }\n\n  protected update(changedProperties: PropertyValues) {\n    super.update(changedProperties);\n    this.dispatchEvent(\n      new CustomEvent(\"validity-changed\", {\n        detail: this._invalid,\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n\n  protected render() {\n    if (!(this._source || this._setpoint || this._unit)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"sources\">\n        <ha-select\n          id=\"source-select\"\n          .label=${this.lcn.localize(\"source\")}\n          .value=${this._source.value}\n          fixedMenuPosition\n          @selected=${this._sourceChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sources.map(\n            (source) => html`\n              <ha-list-item .value=${source.value}> ${source.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"setpoint-select\"\n          .label=${this.lcn.localize(\"setpoint\")}\n          .value=${this._setpoint.value}\n          fixedMenuPosition\n          @selected=${this._setpointChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._setpoints.map(\n            (setpoint) => html`\n              <ha-list-item .value=${setpoint.value}> ${setpoint.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n      </div>\n\n      <div class=\"lockable\">\n        <label>${this.lcn.localize(\"dashboard-entities-dialog-climate-lockable\")}:</label>\n        <ha-switch\n          .checked=${this.domainData.lockable}\n          @change=${this._lockableChanged}\n        ></ha-switch>\n      </div>\n\n      <ha-textfield\n        id=\"min-textfield\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-climate-min-temperature\")}\n        type=\"number\"\n        .value=${this.domainData.min_temp.toString()}\n        required\n        autoValidate\n        @input=${this._minTempChanged}\n        .validityTransform=${this._validityTransformMinTemp}\n        .validationMessage=${this.lcn.localize(\n          \"dashboard-entities-dialog-climate-min-temperature-error\",\n        )}\n      ></ha-textfield>\n\n      <ha-textfield\n        id=\"max-textfield\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-climate-max-temperature\")}\n        type=\"number\"\n        .value=${this.domainData.max_temp.toString()}\n        required\n        autoValidate\n        @input=${this._maxTempChanged}\n        .validityTransform=${this._validityTransformMaxTemp}\n        .validationMessage=${this.lcn.localize(\n          \"dashboard-entities-dialog-climate-max-temperature-error\",\n        )}\n      ></ha-textfield>\n\n      <ha-select\n        id=\"unit-select\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-unit-of-measurement\")}\n        .value=${this._unit.value}\n        fixedMenuPosition\n        @selected=${this._unitChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._varUnits.map(\n          (unit) => html` <ha-list-item .value=${unit.value}> ${unit.name} </ha-list-item> `,\n        )}\n      </ha-select>\n    `;\n  }\n\n  private _sourceChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._source = this._sources.find((source) => source.value === target.value)!;\n    this.domainData.source = this._source.value;\n  }\n\n  private _setpointChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._setpoint = this._setpoints.find((setpoint) => setpoint.value === target.value)!;\n    this.domainData.setpoint = this._setpoint.value;\n  }\n\n  private _minTempChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.min_temp = +target.value;\n    const maxTextfield: HaTextField = this.shadowRoot!.querySelector(\"#max-textfield\")!;\n    maxTextfield.reportValidity();\n    this.requestUpdate();\n  }\n\n  private _maxTempChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.max_temp = +target.value;\n    const minTextfield: HaTextField = this.shadowRoot!.querySelector(\"#min-textfield\")!;\n    minTextfield.reportValidity();\n    this.requestUpdate();\n  }\n\n  private _lockableChanged(ev: ValueChangedEvent<string>): void {\n    this.domainData.lockable = (ev.target as HaSwitch).checked;\n  }\n\n  private _unitChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._unit = this._varUnits.find((unit) => unit.value === target.value)!;\n    this.domainData.unit_of_measurement = this._unit.value;\n  }\n\n  private _validateMaxTemp(max_temp: number): boolean {\n    return max_temp > this.domainData.min_temp;\n  }\n\n  private _validateMinTemp(min_temp: number): boolean {\n    return min_temp < this.domainData.max_temp;\n  }\n\n  private get _validityTransformMaxTemp() {\n    return (value: string) => ({ valid: this._validateMaxTemp(+value) });\n  }\n\n  private get _validityTransformMinTemp() {\n    return (value: string) => ({ valid: this._validateMinTemp(+value) });\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .lockable {\n          margin-top: 10px;\n        }\n        ha-switch {\n          margin-left: 25px;\n        }\n      `,\n    ];\n  }\n}\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-climate-element\": LCNConfigClimateElement;\n  }\n}\n",
+        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@polymer/paper-dropdown-menu/paper-dropdown-menu\";\nimport \"@polymer/paper-item/paper-item\";\nimport \"@polymer/paper-listbox/paper-listbox\";\nimport { css, html, LitElement, CSSResult, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, CoverConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\n@customElement(\"lcn-config-cover-element\")\nexport class LCNConfigCoverElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: CoverConfig = {\n    motor: \"MOTOR1\",\n    reverse_time: \"RT1200\",\n  };\n\n  @state() private _motor!: ConfigItem;\n\n  @state() private _reverseDelay!: ConfigItem;\n\n  private get _motors(): ConfigItem[] {\n    const motor: string = this.lcn.localize(\"motor\");\n    return [\n      { name: motor + \" 1\", value: \"MOTOR1\" },\n      { name: motor + \" 2\", value: \"MOTOR2\" },\n      { name: motor + \" 3\", value: \"MOTOR3\" },\n      { name: motor + \" 4\", value: \"MOTOR4\" },\n      { name: this.lcn.localize(\"outputs\"), value: \"OUTPUTS\" },\n    ];\n  }\n\n  private _reverseDelays: ConfigItem[] = [\n    { name: \"70ms\", value: \"RT70\" },\n    { name: \"600ms\", value: \"RT600\" },\n    { name: \"1200ms\", value: \"RT1200\" },\n  ];\n\n  public connectedCallback(): void {\n    super.connectedCallback();\n    this._motor = this._motors[0];\n    this._reverseDelay = this._reverseDelays[0];\n  }\n\n  protected render() {\n    if (!(this._motor || this._reverseDelay)) {\n      return nothing;\n    }\n    return html`\n      <ha-select\n        id=\"motor-select\"\n        .label=${this.lcn.localize(\"motor\")}\n        .value=${this._motor.value}\n        fixedMenuPosition\n        @selected=${this._motorChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._motors.map(\n          (motor) => html` <ha-list-item .value=${motor.value}> ${motor.name} </ha-list-item> `,\n        )}\n      </ha-select>\n\n      ${this._motor.value === \"OUTPUTS\"\n        ? html`\n            <ha-select\n              id=\"reverse-delay-select\"\n              .label=${this.lcn.localize(\"reverse-delay\")}\n              .value=${this._reverseDelay.value}\n              fixedMenuPosition\n              @selected=${this._reverseDelayChanged}\n              @closed=${stopPropagation}\n            >\n              ${this._reverseDelays.map(\n                (reverseDelay) => html`\n                  <ha-list-item .value=${reverseDelay.value}> ${reverseDelay.name} </ha-list-item>\n                `,\n              )}\n            </ha-select>\n          `\n        : nothing}\n    `;\n  }\n\n  private _motorChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._motor = this._motors.find((motor) => motor.value === target.value)!;\n    this._reverseDelay = this._reverseDelays[0];\n    this.domainData.motor = this._motor.value;\n  }\n\n  private _reverseDelayChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._reverseDelay = this._reverseDelays.find(\n      (reverseDelay) => reverseDelay.value === target.value,\n    )!;\n    this.domainData.reverse_time = this._reverseDelay.value;\n  }\n\n  static get styles(): CSSResult[] {\n    return [\n      haStyleDialog,\n      css`\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-cover-element\": LCNConfigCoverElement;\n  }\n}\n",
+        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@ha/components/ha-radio\";\nimport \"@ha/components/ha-formfield\";\nimport \"@ha/components/ha-textfield\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HaRadio } from \"@ha/components/ha-radio\";\nimport type { HaSwitch } from \"@ha/components/ha-switch\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, LightConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-light-element\")\nexport class LCNConfigLightElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: LightConfig = {\n    output: \"OUTPUT1\",\n    dimmable: false,\n    transition: 0,\n  };\n\n  @state() private _portType!: ConfigItemCollection;\n\n  @state() private _port!: ConfigItem;\n\n  @query(\"#port-select\") private _portSelect;\n\n  private _invalid = false;\n\n  private get _outputPorts(): ConfigItem[] {\n    const output: string = this.lcn.localize(\"output\");\n    return [\n      { name: output + \" 1\", value: \"OUTPUT1\" },\n      { name: output + \" 2\", value: \"OUTPUT2\" },\n      { name: output + \" 3\", value: \"OUTPUT3\" },\n      { name: output + \" 4\", value: \"OUTPUT4\" },\n    ];\n  }\n\n  private get _relayPorts(): ConfigItem[] {\n    const relay: string = this.lcn.localize(\"relay\");\n    return [\n      { name: relay + \" 1\", value: \"RELAY1\" },\n      { name: relay + \" 2\", value: \"RELAY2\" },\n      { name: relay + \" 3\", value: \"RELAY3\" },\n      { name: relay + \" 4\", value: \"RELAY4\" },\n      { name: relay + \" 5\", value: \"RELAY5\" },\n      { name: relay + \" 6\", value: \"RELAY6\" },\n      { name: relay + \" 7\", value: \"RELAY7\" },\n      { name: relay + \" 8\", value: \"RELAY8\" },\n    ];\n  }\n\n  private get _portTypes(): ConfigItemCollection[] {\n    return [\n      { name: this.lcn.localize(\"output\"), value: this._outputPorts, id: \"output\" },\n      { name: this.lcn.localize(\"relay\"), value: this._relayPorts, id: \"relay\" },\n    ];\n  }\n\n  public connectedCallback(): void {\n    super.connectedCallback();\n    this._portType = this._portTypes[0];\n    this._port = this._portType.value[0];\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    super.willUpdate(changedProperties);\n    this._invalid = !this._validateTransition(this.domainData.transition);\n  }\n\n  protected update(changedProperties: PropertyValues) {\n    super.update(changedProperties);\n    this.dispatchEvent(\n      new CustomEvent(\"validity-changed\", {\n        detail: this._invalid,\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n\n  protected render() {\n    if (!(this._portType || this._port)) {\n      return nothing;\n    }\n    return html`\n      <div id=\"port-type\">${this.lcn.localize(\"port-type\")}</div>\n\n      <ha-formfield label=${this.lcn.localize(\"output\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"output\"\n          .checked=${this._portType.id === \"output\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-formfield label=${this.lcn.localize(\"relay\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"relay\"\n          .checked=${this._portType.id === \"relay\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-select\n        id=\"port-select\"\n        .label=${this.lcn.localize(\"port\")}\n        .value=${this._port.value}\n        fixedMenuPosition\n        @selected=${this._portChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._portType.value.map(\n          (port) => html` <ha-list-item .value=${port.value}> ${port.name} </ha-list-item> `,\n        )}\n      </ha-select>\n\n      ${this.renderOutputFeatures()}\n    `;\n  }\n\n  private renderOutputFeatures() {\n    switch (this._portType.id) {\n      case \"output\":\n        return html`\n          <div id=\"dimmable\">\n            <label>${this.lcn.localize(\"dashboard-entities-dialog-light-dimmable\")}:</label>\n\n            <ha-switch\n              .checked=${this.domainData.dimmable}\n              @change=${this._dimmableChanged}\n            ></ha-switch>\n          </div>\n\n          <ha-textfield\n            id=\"transition\"\n            .label=${this.lcn.localize(\"dashboard-entities-dialog-light-transition\")}\n            type=\"number\"\n            .value=${this.domainData.transition.toString()}\n            min=\"0\"\n            max=\"486\"\n            required\n            autoValidate\n            @input=${this._transitionChanged}\n            .validityTransform=${this._validityTransformTransition}\n            .validationMessage=${this.lcn.localize(\n              \"dashboard-entities-dialog-light-transition-error\",\n            )}\n          ></ha-textfield>\n        `;\n      case \"relay\":\n        return nothing;\n      default:\n        return nothing;\n    }\n  }\n\n  private _portTypeChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaRadio;\n\n    this._portType = this._portTypes.find((portType) => portType.id === target.value)!;\n    this._port = this._portType.value[0];\n    this._portSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _portChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._port = this._portType.value.find((portType) => portType.value === target.value)!;\n    this.domainData.output = this._port.value;\n  }\n\n  private _dimmableChanged(ev: ValueChangedEvent<boolean>): void {\n    this.domainData.dimmable = (ev.target as HaSwitch).checked;\n  }\n\n  private _transitionChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.transition = +target.value;\n    this.requestUpdate();\n  }\n\n  private _validateTransition(transition: number): boolean {\n    return transition >= 0 && transition <= 486;\n  }\n\n  private get _validityTransformTransition() {\n    return (value: string) => ({ valid: this._validateTransition(+value) });\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        #dimmable {\n          margin-top: 16px;\n        }\n        #transition {\n          margin-top: 16px;\n        }\n      `,\n    ];\n  }\n}\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-light-element\": LCNConfigLightElement;\n  }\n}\n",
+        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport \"@ha/components/ha-textfield\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport \"@ha/components/ha-checkbox\";\nimport \"@ha/components/ha-formfield\";\nimport { css, html, LitElement, CSSResultGroup, PropertyValues, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, SceneConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\n@customElement(\"lcn-config-scene-element\")\nexport class LCNConfigSceneElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: SceneConfig = {\n    register: 0,\n    scene: 0,\n    outputs: [],\n    transition: 0,\n  };\n\n  @state() private _register!: ConfigItem;\n\n  @state() private _scene!: ConfigItem;\n\n  private _invalid = false;\n\n  private get _registers(): ConfigItem[] {\n    const register: string = this.lcn.localize(\"register\");\n    return [\n      { name: register + \" 0\", value: \"0\" },\n      { name: register + \" 1\", value: \"1\" },\n      { name: register + \" 2\", value: \"2\" },\n      { name: register + \" 3\", value: \"3\" },\n      { name: register + \" 4\", value: \"4\" },\n      { name: register + \" 5\", value: \"5\" },\n      { name: register + \" 6\", value: \"6\" },\n      { name: register + \" 7\", value: \"7\" },\n      { name: register + \" 8\", value: \"8\" },\n      { name: register + \" 9\", value: \"9\" },\n    ];\n  }\n\n  private get _scenes(): ConfigItem[] {\n    const scene: string = this.lcn.localize(\"scene\");\n    return [\n      { name: scene + \" 1\", value: \"0\" },\n      { name: scene + \" 2\", value: \"1\" },\n      { name: scene + \" 3\", value: \"2\" },\n      { name: scene + \" 4\", value: \"3\" },\n      { name: scene + \" 5\", value: \"4\" },\n      { name: scene + \" 6\", value: \"5\" },\n      { name: scene + \" 7\", value: \"6\" },\n      { name: scene + \" 8\", value: \"7\" },\n      { name: scene + \" 9\", value: \"8\" },\n      { name: scene + \" 10\", value: \"9\" },\n    ];\n  }\n\n  private get _outputPorts(): ConfigItem[] {\n    const output: string = this.lcn.localize(\"output\");\n    return [\n      { name: output + \" 1\", value: \"OUTPUT1\" },\n      { name: output + \" 2\", value: \"OUTPUT2\" },\n      { name: output + \" 3\", value: \"OUTPUT3\" },\n      { name: output + \" 4\", value: \"OUTPUT4\" },\n    ];\n  }\n\n  private get _relayPorts(): ConfigItem[] {\n    const relay: string = this.lcn.localize(\"relay\");\n    return [\n      { name: relay + \" 1\", value: \"RELAY1\" },\n      { name: relay + \" 2\", value: \"RELAY2\" },\n      { name: relay + \" 3\", value: \"RELAY3\" },\n      { name: relay + \" 4\", value: \"RELAY4\" },\n      { name: relay + \" 5\", value: \"RELAY5\" },\n      { name: relay + \" 6\", value: \"RELAY6\" },\n      { name: relay + \" 7\", value: \"RELAY7\" },\n      { name: relay + \" 8\", value: \"RELAY8\" },\n    ];\n  }\n\n  public connectedCallback(): void {\n    super.connectedCallback();\n    this._register = this._registers[0];\n    this._scene = this._scenes[0];\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    super.willUpdate(changedProperties);\n    this._invalid = !this._validateTransition(this.domainData.transition);\n  }\n\n  protected update(changedProperties: PropertyValues) {\n    super.update(changedProperties);\n    this.dispatchEvent(\n      new CustomEvent(\"validity-changed\", {\n        detail: this._invalid,\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n\n  protected render() {\n    if (!(this._register || this._scene)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"registers\">\n        <ha-select\n          id=\"register-select\"\n          .label=${this.lcn.localize(\"register\")}\n          .value=${this._register.value}\n          fixedMenuPosition\n          @selected=${this._registerChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._registers.map(\n            (register) => html`\n              <ha-list-item .value=${register.value}> ${register.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"scene-select\"\n          .label=${this.lcn.localize(\"scene\")}\n          .value=${this._scene.value}\n          fixedMenuPosition\n          @selected=${this._sceneChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._scenes.map(\n            (scene) => html` <ha-list-item .value=${scene.value}> ${scene.name} </ha-list-item> `,\n          )}\n        </ha-select>\n      </div>\n\n      <div class=\"ports\">\n        <label>${this.lcn.localize(\"outputs\")}:</label><br />\n        ${this._outputPorts.map(\n          (port) => html`\n            <ha-formfield label=${port.name}>\n              <ha-checkbox .value=${port.value} @change=${this._portCheckedChanged}></ha-checkbox>\n            </ha-formfield>\n          `,\n        )}\n      </div>\n\n      <div class=\"ports\">\n        <label>${this.lcn.localize(\"relays\")}:</label><br />\n        ${this._relayPorts.map(\n          (port) => html`\n            <ha-formfield label=${port.name}>\n              <ha-checkbox .value=${port.value} @change=${this._portCheckedChanged}></ha-checkbox>\n            </ha-formfield>\n          `,\n        )}\n      </div>\n\n      <ha-textfield\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-scene-transition\")}\n        type=\"number\"\n        .value=${this.domainData.transition.toString()}\n        min=\"0\"\n        max=\"486\"\n        required\n        autoValidate\n        @input=${this._transitionChanged}\n        .validityTransform=${this._validityTransformTransition}\n        .disabled=${this._transitionDisabled}\n        .validationMessage=${this.lcn.localize(\"dashboard-entities-dialog-scene-transition-error\")}\n      ></ha-textfield>\n    `;\n  }\n\n  private _registerChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._register = this._registers.find((register) => register.value === target.value)!;\n    this.domainData.register = +this._register.value;\n  }\n\n  private _sceneChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._scene = this._scenes.find((scene) => scene.value === target.value)!;\n    this.domainData.scene = +this._scene.value;\n  }\n\n  private _portCheckedChanged(ev: ValueChangedEvent<string> | any): void {\n    if (ev.target.checked) {\n      this.domainData.outputs.push(ev.target.value);\n    } else {\n      this.domainData.outputs = this.domainData.outputs.filter((port) => ev.target.value !== port);\n    }\n    this.requestUpdate();\n  }\n\n  private _transitionChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this.domainData.transition = +target.value;\n    this.requestUpdate();\n  }\n\n  private _validateTransition(transition: number): boolean {\n    return transition >= 0 && transition <= 486;\n  }\n\n  private get _validityTransformTransition() {\n    return (value: string) => ({ valid: this._validateTransition(+value) });\n  }\n\n  private get _transitionDisabled(): boolean {\n    const outputPortValues = this._outputPorts.map((port) => port.value);\n    return (\n      this.domainData.outputs.filter((output) => outputPortValues.includes(output)).length === 0\n    );\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        .registers {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .ports {\n          margin-top: 10px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-scene-element\": LCNConfigSceneElement;\n  }\n}\n",
+        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, CSSResultGroup, nothing } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport type { LCN, SensorConfig } from \"types/lcn\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-sensor-element\")\nexport class LCNConfigSensorElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ type: Number }) public softwareSerial: number = -1;\n\n  @property({ attribute: false }) public domainData: SensorConfig = {\n    source: \"VAR1\",\n    unit_of_measurement: \"NATIVE\",\n  };\n\n  @state() private _sourceType!: ConfigItemCollection;\n\n  @state() private _source!: ConfigItem;\n\n  @state() private _unit!: ConfigItem;\n\n  @query(\"#source-select\") private _sourceSelect!: HaSelect;\n\n  private get _is2013() {\n    return this.softwareSerial >= 0x170206;\n  }\n\n  private _variablesOld: ConfigItem[] = [\n    { name: \"TVar\", value: \"TVAR\" },\n    { name: \"R1Var\", value: \"R1VAR\" },\n    { name: \"R2Var\", value: \"R2VAR\" },\n  ];\n\n  private get _variablesNew(): ConfigItem[] {\n    const variable: string = this.lcn.localize(\"variable\");\n    return [\n      { name: variable + \" 1\", value: \"VAR1\" },\n      { name: variable + \" 2\", value: \"VAR2\" },\n      { name: variable + \" 3\", value: \"VAR3\" },\n      { name: variable + \" 4\", value: \"VAR4\" },\n      { name: variable + \" 5\", value: \"VAR5\" },\n      { name: variable + \" 6\", value: \"VAR6\" },\n      { name: variable + \" 7\", value: \"VAR7\" },\n      { name: variable + \" 8\", value: \"VAR8\" },\n      { name: variable + \" 9\", value: \"VAR9\" },\n      { name: variable + \" 10\", value: \"VAR10\" },\n      { name: variable + \" 11\", value: \"VAR11\" },\n      { name: variable + \" 12\", value: \"VAR12\" },\n    ];\n  }\n\n  private get _setpoints(): ConfigItem[] {\n    const setpoint: string = this.lcn.localize(\"setpoint\");\n    return [\n      { name: setpoint + \" 1\", value: \"R1VARSETPOINT\" },\n      { name: setpoint + \" 2\", value: \"R2VARSETPOINT\" },\n    ];\n  }\n\n  private get _thresholdsOld(): ConfigItem[] {\n    const threshold: string = this.lcn.localize(\"threshold\");\n    return [\n      { name: threshold + \" 1\", value: \"THRS1\" },\n      { name: threshold + \" 2\", value: \"THRS2\" },\n      { name: threshold + \" 3\", value: \"THRS3\" },\n      { name: threshold + \" 4\", value: \"THRS4\" },\n      { name: threshold + \" 5\", value: \"THRS5\" },\n    ];\n  }\n\n  private get _thresholdsNew(): ConfigItem[] {\n    const threshold: string = this.lcn.localize(\"threshold\");\n    return [\n      { name: threshold + \" 1-1\", value: \"THRS1\" },\n      { name: threshold + \" 1-2\", value: \"THRS2\" },\n      { name: threshold + \" 1-3\", value: \"THRS3\" },\n      { name: threshold + \" 1-4\", value: \"THRS4\" },\n      { name: threshold + \" 2-1\", value: \"THRS2_1\" },\n      { name: threshold + \" 2-2\", value: \"THRS2_2\" },\n      { name: threshold + \" 2-3\", value: \"THRS2_3\" },\n      { name: threshold + \" 2-4\", value: \"THRS2_4\" },\n      { name: threshold + \" 3-1\", value: \"THRS3_1\" },\n      { name: threshold + \" 3-2\", value: \"THRS3_2\" },\n      { name: threshold + \" 3-3\", value: \"THRS3_3\" },\n      { name: threshold + \" 3-4\", value: \"THRS3_4\" },\n      { name: threshold + \" 4-1\", value: \"THRS4_1\" },\n      { name: threshold + \" 4-2\", value: \"THRS4_2\" },\n      { name: threshold + \" 4-3\", value: \"THRS4_3\" },\n      { name: threshold + \" 4-4\", value: \"THRS4_4\" },\n    ];\n  }\n\n  private get _s0Inputs(): ConfigItem[] {\n    const s0input: string = this.lcn.localize(\"s0input\");\n    return [\n      { name: s0input + \" 1\", value: \"S0INPUT1\" },\n      { name: s0input + \" 2\", value: \"S0INPUT2\" },\n      { name: s0input + \" 3\", value: \"S0INPUT3\" },\n      { name: s0input + \" 4\", value: \"S0INPUT4\" },\n    ];\n  }\n\n  private get _ledPorts(): ConfigItem[] {\n    const led: string = this.lcn.localize(\"led\");\n    return [\n      { name: led + \" 1\", value: \"LED1\" },\n      { name: led + \" 2\", value: \"LED2\" },\n      { name: led + \" 3\", value: \"LED3\" },\n      { name: led + \" 4\", value: \"LED4\" },\n      { name: led + \" 5\", value: \"LED5\" },\n      { name: led + \" 6\", value: \"LED6\" },\n      { name: led + \" 7\", value: \"LED7\" },\n      { name: led + \" 8\", value: \"LED8\" },\n      { name: led + \" 9\", value: \"LED9\" },\n      { name: led + \" 10\", value: \"LED10\" },\n      { name: led + \" 11\", value: \"LED11\" },\n      { name: led + \" 12\", value: \"LED12\" },\n    ];\n  }\n\n  private get _logicOpPorts(): ConfigItem[] {\n    const logic: string = this.lcn.localize(\"logic\");\n    return [\n      { name: logic + \" 1\", value: \"LOGICOP1\" },\n      { name: logic + \" 2\", value: \"LOGICOP2\" },\n      { name: logic + \" 3\", value: \"LOGICOP3\" },\n      { name: logic + \" 4\", value: \"LOGICOP4\" },\n    ];\n  }\n\n  private get _sourceTypes(): ConfigItemCollection[] {\n    return [\n      {\n        name: this.lcn.localize(\"variables\"),\n        value: this._is2013 ? this._variablesNew : this._variablesOld,\n        id: \"variables\",\n      },\n      {\n        name: this.lcn.localize(\"setpoints\"),\n        value: this._setpoints,\n        id: \"setpoints\",\n      },\n      {\n        name: this.lcn.localize(\"thresholds\"),\n        value: this._is2013 ? this._thresholdsNew : this._thresholdsOld,\n        id: \"thresholds\",\n      },\n      { name: this.lcn.localize(\"s0inputs\"), value: this._s0Inputs, id: \"s0inputs\" },\n      { name: this.lcn.localize(\"leds\"), value: this._ledPorts, id: \"ledports\" },\n      { name: this.lcn.localize(\"logics\"), value: this._logicOpPorts, id: \"logicopports\" },\n    ];\n  }\n\n  private get _varUnits(): ConfigItem[] {\n    return [\n      { name: this.lcn.localize(\"unit-lcn-native\"), value: \"NATIVE\" },\n      { name: \"Celsius\", value: \"\u00b0C\" },\n      { name: \"Fahrenheit\", value: \"\u00b0F\" },\n      { name: \"Kelvin\", value: \"K\" },\n      { name: \"Lux\", value: \"LUX_T\" },\n      { name: \"Lux (I-Port)\", value: \"LUX_I\" },\n      { name: this.lcn.localize(\"unit-humidity\") + \" (%)\", value: \"PERCENT\" },\n      { name: \"CO2 (\u2030)\", value: \"PPM\" },\n      { name: this.lcn.localize(\"unit-wind\") + \" (m/s)\", value: \"METERPERSECOND\" },\n      { name: this.lcn.localize(\"unit-volts\"), value: \"VOLT\" },\n      { name: this.lcn.localize(\"unit-milliamperes\"), value: \"AMPERE\" },\n      { name: this.lcn.localize(\"unit-angle\") + \" (\u00b0)\", value: \"DEGREE\" },\n    ];\n  }\n\n  public connectedCallback(): void {\n    super.connectedCallback();\n    this._sourceType = this._sourceTypes[0];\n    this._source = this._sourceType.value[0];\n    this._unit = this._varUnits[0];\n  }\n\n  protected render() {\n    if (!(this._sourceType || this._source)) {\n      return nothing;\n    }\n    return html`\n      <div class=\"sources\">\n        <ha-select\n          id=\"source-type-select\"\n          .label=${this.lcn.localize(\"source-type\")}\n          .value=${this._sourceType.id}\n          fixedMenuPosition\n          @selected=${this._sourceTypeChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceTypes.map(\n            (sourceType) => html`\n              <ha-list-item .value=${sourceType.id}> ${sourceType.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-select\n          id=\"source-select\"\n          .label=${this.lcn.localize(\"source\")}\n          .value=${this._source.value}\n          fixedMenuPosition\n          @selected=${this._sourceChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._sourceType.value.map(\n            (source) => html`\n              <ha-list-item .value=${source.value}> ${source.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n      </div>\n\n      <ha-select\n        id=\"unit-select\"\n        .label=${this.lcn.localize(\"dashboard-entities-dialog-unit-of-measurement\")}\n        .value=${this._unit.value}\n        fixedMenuPosition\n        @selected=${this._unitChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._varUnits.map(\n          (unit) => html` <ha-list-item .value=${unit.value}> ${unit.name} </ha-list-item> `,\n        )}\n      </ha-select>\n    `;\n  }\n\n  private _sourceTypeChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._sourceType = this._sourceTypes.find((sourceType) => sourceType.id === target.value)!;\n    this._source = this._sourceType.value[0];\n    this._sourceSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _sourceChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._source = this._sourceType.value.find((source) => source.value === target.value)!;\n    this.domainData.source = this._source.value;\n  }\n\n  private _unitChanged(ev: CustomEvent): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._unit = this._varUnits.find((unit) => unit.value === target.value)!;\n    this.domainData.unit_of_measurement = this._unit.value;\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        .sources {\n          display: grid;\n          grid-template-columns: 1fr 1fr;\n          column-gap: 4px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-sensor-element\": LCNConfigSensorElement;\n  }\n}\n",
+        "import \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, CSSResultGroup, nothing } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { LCN, SwitchConfig } from \"types/lcn\";\nimport \"@ha/components/ha-radio\";\nimport \"@ha/components/ha-formfield\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport type { HaRadio } from \"@ha/components/ha-radio\";\n\ninterface ConfigItem {\n  name: string;\n  value: string;\n}\n\ninterface ConfigItemCollection {\n  name: string;\n  value: ConfigItem[];\n  id: string;\n}\n\n@customElement(\"lcn-config-switch-element\")\nexport class LCNConfigSwitchElement extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public domainData: SwitchConfig = { output: \"OUTPUT1\" };\n\n  @state() private _portType!: ConfigItemCollection;\n\n  @state() private _port!: ConfigItem;\n\n  @query(\"#port-select\") private _portSelect;\n\n  private get _outputPorts(): ConfigItem[] {\n    const output: string = this.lcn.localize(\"output\");\n    return [\n      { name: output + \" 1\", value: \"OUTPUT1\" },\n      { name: output + \" 2\", value: \"OUTPUT2\" },\n      { name: output + \" 3\", value: \"OUTPUT3\" },\n      { name: output + \" 4\", value: \"OUTPUT4\" },\n    ];\n  }\n\n  private get _relayPorts(): ConfigItem[] {\n    const relay: string = this.lcn.localize(\"relay\");\n    return [\n      { name: relay + \" 1\", value: \"RELAY1\" },\n      { name: relay + \" 2\", value: \"RELAY2\" },\n      { name: relay + \" 3\", value: \"RELAY3\" },\n      { name: relay + \" 4\", value: \"RELAY4\" },\n      { name: relay + \" 5\", value: \"RELAY5\" },\n      { name: relay + \" 6\", value: \"RELAY6\" },\n      { name: relay + \" 7\", value: \"RELAY7\" },\n      { name: relay + \" 8\", value: \"RELAY8\" },\n    ];\n  }\n\n  private get _portTypes(): ConfigItemCollection[] {\n    return [\n      { name: this.lcn.localize(\"output\"), value: this._outputPorts, id: \"output\" },\n      { name: this.lcn.localize(\"relay\"), value: this._relayPorts, id: \"relay\" },\n    ];\n  }\n\n  public connectedCallback(): void {\n    super.connectedCallback();\n    this._portType = this._portTypes[0];\n    this._port = this._portType.value[0];\n  }\n\n  protected render() {\n    if (!(this._portType || this._port)) {\n      return nothing;\n    }\n    return html`\n      <div id=\"port-type\">${this.lcn.localize(\"port-type\")}</div>\n\n      <ha-formfield label=${this.lcn.localize(\"output\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"output\"\n          .checked=${this._portType.id === \"output\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-formfield label=${this.lcn.localize(\"relay\")}>\n        <ha-radio\n          name=\"port\"\n          value=\"relay\"\n          .checked=${this._portType.id === \"relay\"}\n          @change=${this._portTypeChanged}\n        ></ha-radio>\n      </ha-formfield>\n\n      <ha-select\n        id=\"port-select\"\n        .label=${this.lcn.localize(\"port\")}\n        .value=${this._port.value}\n        fixedMenuPosition\n        @selected=${this._portChanged}\n        @closed=${stopPropagation}\n      >\n        ${this._portType.value.map(\n          (port) => html` <ha-list-item .value=${port.value}> ${port.name} </ha-list-item> `,\n        )}\n      </ha-select>\n    `;\n  }\n\n  private _portTypeChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaRadio;\n\n    this._portType = this._portTypes.find((portType) => portType.id === target.value)!;\n    this._port = this._portType.value[0];\n    this._portSelect.select(-1); // need to change index, so ha-select gets updated\n  }\n\n  private _portChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaSelect;\n    if (target.index === -1) return;\n\n    this._port = this._portType.value.find((portType) => portType.value === target.value)!;\n    this.domainData.output = this._port.value;\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyleDialog,\n      css`\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-select {\n          display: block;\n          margin-bottom: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-switch-element\": LCNConfigSwitchElement;\n  }\n}\n",
         "import \"@ha/components/ha-icon-button\";\nimport \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport { fireEvent } from \"@ha/common/dom/fire_event\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, CSSResultGroup, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport { createCloseHeading } from \"@ha/components/ha-dialog\";\nimport { stopPropagation } from \"@ha/common/dom/stop_propagation\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { HomeAssistant } from \"@ha/types\";\nimport type { LCN, LcnEntityConfig } from \"types/lcn\";\nimport \"./lcn-config-binary-sensor\";\nimport \"./lcn-config-climate\";\nimport \"./lcn-config-cover\";\nimport \"./lcn-config-light\";\nimport \"./lcn-config-scene\";\nimport \"./lcn-config-sensor\";\nimport \"./lcn-config-switch\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport { showAlertDialog } from \"@ha/dialogs/generic/show-dialog-box\";\nimport type { LcnEntityDialogParams } from \"./show-dialog-create-entity\";\n\ninterface DomainItem {\n  name: string;\n  domain: string;\n}\n\n@customElement(\"lcn-create-entity-dialog\")\nexport class CreateEntityDialog extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @state() private _params?: LcnEntityDialogParams;\n\n  @state() private _name: string = \"\";\n\n  @state() public domain: string = \"binary_sensor\";\n\n  @state() private _invalid: boolean = true;\n\n  private get _domains(): DomainItem[] {\n    return [\n      { name: this.lcn.localize(\"binary-sensor\"), domain: \"binary_sensor\" },\n      { name: this.lcn.localize(\"climate\"), domain: \"climate\" },\n      { name: this.lcn.localize(\"cover\"), domain: \"cover\" },\n      { name: this.lcn.localize(\"light\"), domain: \"light\" },\n      { name: this.lcn.localize(\"scene\"), domain: \"scene\" },\n      { name: this.lcn.localize(\"sensor\"), domain: \"sensor\" },\n      { name: this.lcn.localize(\"switch\"), domain: \"switch\" },\n    ];\n  }\n\n  public async showDialog(params: LcnEntityDialogParams): Promise<void> {\n    this._params = params;\n    this.lcn = params.lcn;\n    this._name = \"\";\n    this._invalid = true;\n    await this.updateComplete;\n  }\n\n  protected render() {\n    if (!this._params) {\n      return nothing;\n    }\n    return html`\n      <ha-dialog\n        open\n        scrimClickAction\n        escapeKeyAction\n        .heading=${createCloseHeading(\n          this.hass,\n          this.lcn.localize(\"dashboard-entities-dialog-create-title\"),\n        ) as unknown as string}\n        @closed=${this._closeDialog}\n      >\n        <ha-select\n          id=\"domain-select\"\n          .label=${this.lcn.localize(\"domain\")}\n          .value=${this.domain}\n          fixedMenuPosition\n          @selected=${this._domainChanged}\n          @closed=${stopPropagation}\n        >\n          ${this._domains.map(\n            (domain) => html`\n              <ha-list-item .value=${domain.domain}> ${domain.name} </ha-list-item>\n            `,\n          )}\n        </ha-select>\n\n        <ha-textfield\n          id=\"name-input\"\n          label=${this.lcn.localize(\"entity-id\")}\n          type=\"string\"\n          prefix=${this.domain + \".\"}\n          maxLength=\"20\"\n          @input=${this._nameChanged}\n        ></ha-textfield>\n\n        ${this.renderDomain(this.domain)}\n\n        <div class=\"buttons\">\n          <mwc-button\n            slot=\"secondaryAction\"\n            @click=${this._closeDialog}\n            .label=${this.lcn.localize(\"dismiss\")}\n          ></mwc-button>\n          <mwc-button\n            slot=\"primaryAction\"\n            .disabled=${this._invalid}\n            @click=${this._create}\n            .label=${this.lcn.localize(\"create\")}\n          ></mwc-button>\n        </div>\n      </ha-dialog>\n    `;\n  }\n\n  private renderDomain(domain: string) {\n    if (!this._params) {\n      return nothing;\n    }\n    switch (domain) {\n      case \"binary_sensor\":\n        return html`<lcn-config-binary-sensor-element\n          id=\"domain\"\n          .hass=${this.hass}\n          .lcn=${this.lcn}\n        ></lcn-config-binary-sensor-element>`;\n      case \"climate\":\n        return html`<lcn-config-climate-element\n          id=\"domain\"\n          .hass=${this.hass}\n          .lcn=${this.lcn}\n          .softwareSerial=${this._params.device.software_serial!}\n          @validity-changed=${this._validityChanged}\n        ></lcn-config-climate-element>`;\n      case \"cover\":\n        return html`<lcn-config-cover-element\n          id=\"domain\"\n          .hass=${this.hass}\n          .lcn=${this.lcn}\n        ></lcn-config-cover-element>`;\n      case \"light\":\n        return html`<lcn-config-light-element\n          id=\"domain\"\n          .hass=${this.hass}\n          .lcn=${this.lcn}\n          @validity-changed=${this._validityChanged}\n        ></lcn-config-light-element>`;\n      case \"scene\":\n        return html`<lcn-config-scene-element\n          id=\"domain\"\n          .hass=${this.hass}\n          .lcn=${this.lcn}\n          @validity-changed=${this._validityChanged}\n        ></lcn-config-scene-element>`;\n      case \"sensor\":\n        return html`<lcn-config-sensor-element\n          id=\"domain\"\n          .hass=${this.hass}\n          .lcn=${this.lcn}\n          .softwareSerial=${this._params.device.software_serial!}\n        ></lcn-config-sensor-element>`;\n      case \"switch\":\n        return html`<lcn-config-switch-element\n          id=\"domain\"\n          .hass=${this.hass}\n          .lcn=${this.lcn}\n        ></lcn-config-switch-element>`;\n      default:\n        return nothing;\n    }\n  }\n\n  private _nameChanged(ev: CustomEvent): void {\n    const target = ev.target as HaTextField;\n    this._name = target.value;\n    this._validityChanged(\n      new CustomEvent(\"validity-changed\", {\n        detail: !this._name,\n      }),\n    );\n  }\n\n  private _validityChanged(ev: CustomEvent): void {\n    this._invalid = ev.detail;\n  }\n\n  private async _create(): Promise<void> {\n    const domainElement = this.shadowRoot?.querySelector<any>(\"#domain\");\n\n    const values: Partial<LcnEntityConfig> = {\n      name: this._name ? this._name : this.domain,\n      address: this._params!.device.address,\n      domain: this.domain,\n      domain_data: domainElement.domainData,\n    };\n\n    if (!(await this._params!.createEntity(values))) {\n      await showAlertDialog(this, {\n        title: this.lcn.localize(\"dashboard-entities-dialog-add-alert-title\"),\n        text: `${this.lcn.localize(\"dashboard-entities-dialog-add-alert-text\")}\n              ${this.lcn.localize(\"dashboard-entities-dialog-add-alert-hint\")}`,\n      });\n      return;\n    }\n\n    this._closeDialog();\n  }\n\n  private _closeDialog(): void {\n    this._params = undefined;\n    fireEvent(this, \"dialog-closed\", { dialog: this.localName });\n  }\n\n  private _domainChanged(ev: CustomEvent) {\n    const target = ev.target as HaSelect;\n    this.domain = target.value;\n  }\n\n  static get styles(): CSSResultGroup {\n    return [\n      haStyleDialog,\n      css`\n        ha-dialog {\n          --mdc-dialog-max-width: 500px;\n          --dialog-z-index: 10;\n        }\n        ha-select,\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .buttons {\n          display: flex;\n          justify-content: space-between;\n          padding: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-create-entity-dialog\": CreateEntityDialog;\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see entrypoint-UP5lFvdJ.js.LICENSE.txt */
+/*! For license information please see entrypoint-Wn7tXtT_.js.LICENSE.txt */
 var e, t, r = {
         8394: (e, t, r) => {
             r.d(t, {
                 B: () => o
             });
             const o = (e, t, r, o) => {
                 o = o || {}, r = null == r ? {} : r;
@@ -159,14 +159,68 @@
                     }, n
                 }
                 return o.clear = function() {
                     r = null
                 }, o
             }
         },
+        9051: (e, t, r) => {
+            r.d(t, {
+                Ce: () => s,
+                Ks: () => l,
+                LO: () => i,
+                S6: () => c,
+                V5: () => o,
+                Vy: () => a,
+                n1: () => h,
+                rI: () => n
+            });
+            const o = e => e.callWS({
+                    type: "lcn/hosts"
+                }),
+                i = (e, t) => e.callWS({
+                    type: "lcn/devices",
+                    host_id: t
+                }),
+                n = (e, t, r) => e.callWS({
+                    type: "lcn/entities",
+                    host_id: t,
+                    address: r
+                }),
+                a = (e, t) => e.callWS({
+                    type: "lcn/devices/scan",
+                    host_id: t
+                }),
+                s = (e, t, r) => e.callWS({
+                    type: "lcn/entities/add",
+                    host_id: t,
+                    address: r.address,
+                    name: r.name,
+                    domain: r.domain,
+                    domain_data: r.domain_data
+                }),
+                l = (e, t, r) => e.callWS({
+                    type: "lcn/entities/delete",
+                    host_id: t,
+                    address: r.address,
+                    domain: r.domain,
+                    resource: r.resource
+                }),
+                c = (e, t, r) => e.callWS({
+                    type: "lcn/devices/add",
+                    host_id: t,
+                    address: r.address,
+                    name: r.name
+                }),
+                h = (e, t, r) => e.callWS({
+                    type: "lcn/devices/delete",
+                    host_id: t,
+                    address: r.address
+                })
+        },
         309: (e, t, r) => {
             function o(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var r = 0, o = new Array(t); r < t; r++) o[r] = e[r];
                 return o
             }
 
@@ -527,18 +581,18 @@
                 return (t, r) => void 0 !== r ? i(e, t, r) : o(e, t)
             }
         },
         5304: (e, t, r) => {
             var o;
             r.d(t, {
                 Jb: () => H,
-                Ld: () => P,
+                Ld: () => C,
                 YP: () => T,
                 _$LH: () => j,
-                dy: () => k,
+                dy: () => S,
                 sY: () => V
             });
             const i = window,
                 n = i.trustedTypes,
                 a = n ? n.createPolicy("lit-html", {
                     createHTML: e => e
                 }) : void 0,
@@ -555,91 +609,91 @@
                 g = /<(?:(!--|\/[^a-zA-Z])|(\/?[a-zA-Z][^>\s]*)|(\/?$))/g,
                 v = /-->/g,
                 y = />/g,
                 E = RegExp(`>|${b}(?:([^\\s"'>=/]+)(${b}*=${b}*(?:[^ \t\n\f\r"'\`<>=]|("|')|))|$)`, "g"),
                 _ = /'/g,
                 w = /"/g,
                 A = /^(?:script|style|textarea|title)$/i,
-                S = e => (t, ...r) => ({
+                k = e => (t, ...r) => ({
                     _$litType$: e,
                     strings: t,
                     values: r
                 }),
-                k = S(1),
-                T = S(2),
+                S = k(1),
+                T = k(2),
                 H = Symbol.for("lit-noChange"),
-                P = Symbol.for("lit-nothing"),
-                C = new WeakMap,
-                B = d.createTreeWalker(d, 129, null, !1);
+                C = Symbol.for("lit-nothing"),
+                P = new WeakMap,
+                x = d.createTreeWalker(d, 129, null, !1);
 
-            function x(e, t) {
+            function B(e, t) {
                 if (!Array.isArray(e) || !e.hasOwnProperty("raw")) throw Error("invalid template strings array");
                 return void 0 !== a ? a.createHTML(t) : t
             }
-            const R = (e, t) => {
+            const L = (e, t) => {
                 const r = e.length - 1,
                     o = [];
                 let i, n = 2 === t ? "<svg>" : "",
                     a = g;
                 for (let c = 0; c < r; c++) {
                     const t = e[c];
                     let r, d, u = -1,
                         p = 0;
                     for (; p < t.length && (a.lastIndex = p, d = a.exec(t), null !== d);) p = a.lastIndex, a === g ? "!--" === d[1] ? a = v : void 0 !== d[1] ? a = y : void 0 !== d[2] ? (A.test(d[2]) && (i = RegExp("</" + d[2], "g")), a = E) : void 0 !== d[3] && (a = E) : a === E ? ">" === d[0] ? (a = null != i ? i : g, u = -1) : void 0 === d[1] ? u = -2 : (u = a.lastIndex - d[2].length, r = d[1], a = void 0 === d[3] ? E : '"' === d[3] ? w : _) : a === w || a === _ ? a = E : a === v || a === y ? a = g : (a = E, i = void 0);
                     const f = a === E && e[c + 1].startsWith("/>") ? " " : "";
                     n += a === g ? t + h : u >= 0 ? (o.push(r), t.slice(0, u) + s + t.slice(u) + l + f) : t + l + (-2 === u ? (o.push(void 0), c) : f)
                 }
-                return [x(e, n + (e[r] || "<?>") + (2 === t ? "</svg>" : "")), o]
+                return [B(e, n + (e[r] || "<?>") + (2 === t ? "</svg>" : "")), o]
             };
-            class L {
+            class R {
                 constructor({
                     strings: e,
                     _$litType$: t
                 }, r) {
                     let o;
                     this.parts = [];
                     let i = 0,
                         a = 0;
                     const h = e.length - 1,
                         d = this.parts,
-                        [p, f] = R(e, t);
-                    if (this.el = L.createElement(p, r), B.currentNode = this.el.content, 2 === t) {
+                        [p, f] = L(e, t);
+                    if (this.el = R.createElement(p, r), x.currentNode = this.el.content, 2 === t) {
                         const e = this.el.content,
                             t = e.firstChild;
                         t.remove(), e.append(...t.childNodes)
                     }
-                    for (; null !== (o = B.nextNode()) && d.length < h;) {
+                    for (; null !== (o = x.nextNode()) && d.length < h;) {
                         if (1 === o.nodeType) {
                             if (o.hasAttributes()) {
                                 const e = [];
                                 for (const t of o.getAttributeNames())
                                     if (t.endsWith(s) || t.startsWith(l)) {
                                         const r = f[a++];
                                         if (e.push(t), void 0 !== r) {
                                             const e = o.getAttribute(r.toLowerCase() + s).split(l),
                                                 t = /([.?@])?(.*)/.exec(r);
                                             d.push({
                                                 type: 1,
                                                 index: i,
                                                 name: t[2],
                                                 strings: e,
-                                                ctor: "." === t[1] ? M : "?" === t[1] ? D : "@" === t[1] ? G : I
+                                                ctor: "." === t[1] ? M : "?" === t[1] ? U : "@" === t[1] ? G : O
                                             })
                                         } else d.push({
                                             type: 6,
                                             index: i
                                         })
                                     } for (const t of e) o.removeAttribute(t)
                             }
                             if (A.test(o.tagName)) {
                                 const e = o.textContent.split(l),
                                     t = e.length - 1;
                                 if (t > 0) {
                                     o.textContent = n ? n.emptyScript : "";
-                                    for (let r = 0; r < t; r++) o.append(e[r], u()), B.nextNode(), d.push({
+                                    for (let r = 0; r < t; r++) o.append(e[r], u()), x.nextNode(), d.push({
                                         type: 2,
                                         index: ++i
                                     });
                                     o.append(e[t], u())
                                 }
                             }
                         } else if (8 === o.nodeType)
@@ -683,37 +737,37 @@
                     var t;
                     const {
                         el: {
                             content: r
                         },
                         parts: o
                     } = this._$AD, i = (null !== (t = null == e ? void 0 : e.creationScope) && void 0 !== t ? t : d).importNode(r, !0);
-                    B.currentNode = i;
-                    let n = B.nextNode(),
+                    x.currentNode = i;
+                    let n = x.nextNode(),
                         a = 0,
                         s = 0,
                         l = o[0];
                     for (; void 0 !== l;) {
                         if (a === l.index) {
                             let t;
-                            2 === l.type ? t = new O(n, n.nextSibling, this, e) : 1 === l.type ? t = new l.ctor(n, l.name, l.strings, this, e) : 6 === l.type && (t = new F(n, this, e)), this._$AV.push(t), l = o[++s]
+                            2 === l.type ? t = new I(n, n.nextSibling, this, e) : 1 === l.type ? t = new l.ctor(n, l.name, l.strings, this, e) : 6 === l.type && (t = new F(n, this, e)), this._$AV.push(t), l = o[++s]
                         }
-                        a !== (null == l ? void 0 : l.index) && (n = B.nextNode(), a++)
+                        a !== (null == l ? void 0 : l.index) && (n = x.nextNode(), a++)
                     }
-                    return B.currentNode = d, i
+                    return x.currentNode = d, i
                 }
                 v(e) {
                     let t = 0;
                     for (const r of this._$AV) void 0 !== r && (void 0 !== r.strings ? (r._$AI(e, r, t), t += r.strings.length - 2) : r._$AI(e[t])), t++
                 }
             }
-            class O {
+            class I {
                 constructor(e, t, r, o) {
                     var i;
-                    this.type = 2, this._$AH = P, this._$AN = void 0, this._$AA = e, this._$AB = t, this._$AM = r, this.options = o, this._$Cp = null === (i = null == o ? void 0 : o.isConnected) || void 0 === i || i
+                    this.type = 2, this._$AH = C, this._$AN = void 0, this._$AA = e, this._$AB = t, this._$AM = r, this.options = o, this._$Cp = null === (i = null == o ? void 0 : o.isConnected) || void 0 === i || i
                 }
                 get _$AU() {
                     var e, t;
                     return null !== (t = null === (e = this._$AM) || void 0 === e ? void 0 : e._$AU) && void 0 !== t ? t : this._$Cp
                 }
                 get parentNode() {
                     let e = this._$AA.parentNode;
@@ -723,113 +777,113 @@
                 get startNode() {
                     return this._$AA
                 }
                 get endNode() {
                     return this._$AB
                 }
                 _$AI(e, t = this) {
-                    e = N(this, e, t), p(e) ? e === P || null == e || "" === e ? (this._$AH !== P && this._$AR(), this._$AH = P) : e !== this._$AH && e !== H && this._(e) : void 0 !== e._$litType$ ? this.g(e) : void 0 !== e.nodeType ? this.$(e) : m(e) ? this.T(e) : this._(e)
+                    e = N(this, e, t), p(e) ? e === C || null == e || "" === e ? (this._$AH !== C && this._$AR(), this._$AH = C) : e !== this._$AH && e !== H && this._(e) : void 0 !== e._$litType$ ? this.g(e) : void 0 !== e.nodeType ? this.$(e) : m(e) ? this.T(e) : this._(e)
                 }
                 k(e) {
                     return this._$AA.parentNode.insertBefore(e, this._$AB)
                 }
                 $(e) {
                     this._$AH !== e && (this._$AR(), this._$AH = this.k(e))
                 }
                 _(e) {
-                    this._$AH !== P && p(this._$AH) ? this._$AA.nextSibling.data = e : this.$(d.createTextNode(e)), this._$AH = e
+                    this._$AH !== C && p(this._$AH) ? this._$AA.nextSibling.data = e : this.$(d.createTextNode(e)), this._$AH = e
                 }
                 g(e) {
                     var t;
                     const {
                         values: r,
                         _$litType$: o
-                    } = e, i = "number" == typeof o ? this._$AC(e) : (void 0 === o.el && (o.el = L.createElement(x(o.h, o.h[0]), this.options)), o);
+                    } = e, i = "number" == typeof o ? this._$AC(e) : (void 0 === o.el && (o.el = R.createElement(B(o.h, o.h[0]), this.options)), o);
                     if ((null === (t = this._$AH) || void 0 === t ? void 0 : t._$AD) === i) this._$AH.v(r);
                     else {
                         const e = new $(i, this),
                             t = e.u(this.options);
                         e.v(r), this.$(t), this._$AH = e
                     }
                 }
                 _$AC(e) {
-                    let t = C.get(e.strings);
-                    return void 0 === t && C.set(e.strings, t = new L(e)), t
+                    let t = P.get(e.strings);
+                    return void 0 === t && P.set(e.strings, t = new R(e)), t
                 }
                 T(e) {
                     f(this._$AH) || (this._$AH = [], this._$AR());
                     const t = this._$AH;
                     let r, o = 0;
-                    for (const i of e) o === t.length ? t.push(r = new O(this.k(u()), this.k(u()), this, this.options)) : r = t[o], r._$AI(i), o++;
+                    for (const i of e) o === t.length ? t.push(r = new I(this.k(u()), this.k(u()), this, this.options)) : r = t[o], r._$AI(i), o++;
                     o < t.length && (this._$AR(r && r._$AB.nextSibling, o), t.length = o)
                 }
                 _$AR(e = this._$AA.nextSibling, t) {
                     var r;
                     for (null === (r = this._$AP) || void 0 === r || r.call(this, !1, !0, t); e && e !== this._$AB;) {
                         const t = e.nextSibling;
                         e.remove(), e = t
                     }
                 }
                 setConnected(e) {
                     var t;
                     void 0 === this._$AM && (this._$Cp = e, null === (t = this._$AP) || void 0 === t || t.call(this, e))
                 }
             }
-            class I {
+            class O {
                 constructor(e, t, r, o, i) {
-                    this.type = 1, this._$AH = P, this._$AN = void 0, this.element = e, this.name = t, this._$AM = o, this.options = i, r.length > 2 || "" !== r[0] || "" !== r[1] ? (this._$AH = Array(r.length - 1).fill(new String), this.strings = r) : this._$AH = P
+                    this.type = 1, this._$AH = C, this._$AN = void 0, this.element = e, this.name = t, this._$AM = o, this.options = i, r.length > 2 || "" !== r[0] || "" !== r[1] ? (this._$AH = Array(r.length - 1).fill(new String), this.strings = r) : this._$AH = C
                 }
                 get tagName() {
                     return this.element.tagName
                 }
                 get _$AU() {
                     return this._$AM._$AU
                 }
                 _$AI(e, t = this, r, o) {
                     const i = this.strings;
                     let n = !1;
                     if (void 0 === i) e = N(this, e, t, 0), n = !p(e) || e !== this._$AH && e !== H, n && (this._$AH = e);
                     else {
                         const o = e;
                         let a, s;
-                        for (e = i[0], a = 0; a < i.length - 1; a++) s = N(this, o[r + a], t, a), s === H && (s = this._$AH[a]), n || (n = !p(s) || s !== this._$AH[a]), s === P ? e = P : e !== P && (e += (null != s ? s : "") + i[a + 1]), this._$AH[a] = s
+                        for (e = i[0], a = 0; a < i.length - 1; a++) s = N(this, o[r + a], t, a), s === H && (s = this._$AH[a]), n || (n = !p(s) || s !== this._$AH[a]), s === C ? e = C : e !== C && (e += (null != s ? s : "") + i[a + 1]), this._$AH[a] = s
                     }
                     n && !o && this.j(e)
                 }
                 j(e) {
-                    e === P ? this.element.removeAttribute(this.name) : this.element.setAttribute(this.name, null != e ? e : "")
+                    e === C ? this.element.removeAttribute(this.name) : this.element.setAttribute(this.name, null != e ? e : "")
                 }
             }
-            class M extends I {
+            class M extends O {
                 constructor() {
                     super(...arguments), this.type = 3
                 }
                 j(e) {
-                    this.element[this.name] = e === P ? void 0 : e
+                    this.element[this.name] = e === C ? void 0 : e
                 }
             }
-            const U = n ? n.emptyScript : "";
-            class D extends I {
+            const D = n ? n.emptyScript : "";
+            class U extends O {
                 constructor() {
                     super(...arguments), this.type = 4
                 }
                 j(e) {
-                    e && e !== P ? this.element.setAttribute(this.name, U) : this.element.removeAttribute(this.name)
+                    e && e !== C ? this.element.setAttribute(this.name, D) : this.element.removeAttribute(this.name)
                 }
             }
-            class G extends I {
+            class G extends O {
                 constructor(e, t, r, o, i) {
                     super(e, t, r, o, i), this.type = 5
                 }
                 _$AI(e, t = this) {
                     var r;
-                    if ((e = null !== (r = N(this, e, t, 0)) && void 0 !== r ? r : P) === H) return;
+                    if ((e = null !== (r = N(this, e, t, 0)) && void 0 !== r ? r : C) === H) return;
                     const o = this._$AH,
-                        i = e === P && o !== P || e.capture !== o.capture || e.once !== o.once || e.passive !== o.passive,
-                        n = e !== P && (o === P || i);
+                        i = e === C && o !== C || e.capture !== o.capture || e.once !== o.once || e.passive !== o.passive,
+                        n = e !== C && (o === C || i);
                     i && this.element.removeEventListener(this.name, this, o), n && this.element.addEventListener(this.name, this, e), this._$AH = e
                 }
                 handleEvent(e) {
                     var t, r;
                     "function" == typeof this._$AH ? this._$AH.call(null !== (r = null === (t = this.options) || void 0 === t ? void 0 : t.host) && void 0 !== r ? r : this.element, e) : this._$AH.handleEvent(e)
                 }
             }
@@ -845,34 +899,34 @@
                 }
             }
             const j = {
                     O: s,
                     P: l,
                     A: c,
                     C: 1,
-                    M: R,
+                    M: L,
                     L: $,
                     R: m,
                     D: N,
-                    I: O,
-                    V: I,
-                    H: D,
+                    I: I,
+                    V: O,
+                    H: U,
                     N: G,
                     U: M,
                     F: F
                 },
                 z = i.litHtmlPolyfillSupport;
-            null == z || z(L, O), (null !== (o = i.litHtmlVersions) && void 0 !== o ? o : i.litHtmlVersions = []).push("2.8.0");
+            null == z || z(R, I), (null !== (o = i.litHtmlVersions) && void 0 !== o ? o : i.litHtmlVersions = []).push("2.8.0");
             const V = (e, t, r) => {
                 var o, i;
                 const n = null !== (o = null == r ? void 0 : r.renderBefore) && void 0 !== o ? o : t;
                 let a = n._$litPart$;
                 if (void 0 === a) {
                     const e = null !== (i = null == r ? void 0 : r.renderBefore) && void 0 !== i ? i : null;
-                    n._$litPart$ = a = new O(t.insertBefore(u(), e), e, void 0, null != r ? r : {})
+                    n._$litPart$ = a = new I(t.insertBefore(u(), e), e, void 0, null != r ? r : {})
                 }
                 return a._$AI(e), a
             }
         },
         4243: (e, t, r) => {
             r.d(t, {
                 Mo: () => o,
@@ -1013,15 +1067,15 @@
                         configurable: !0
                     })
                 })
             }
         },
         8144: (e, t, r) => {
             r.d(t, {
-                oi: () => S,
+                oi: () => k,
                 fl: () => E,
                 iv: () => c,
                 dy: () => A.dy,
                 Jb: () => A.Jb,
                 Ld: () => A.Ld,
                 YP: () => A.YP,
                 $m: () => l
@@ -1297,15 +1351,15 @@
             }
             E[y] = !0, E.elementProperties = new Map, E.elementStyles = [], E.shadowRootOptions = {
                 mode: "open"
             }, null == m || m({
                 ReactiveElement: E
             }), (null !== (d = u.reactiveElementVersions) && void 0 !== d ? d : u.reactiveElementVersions = []).push("1.6.3");
             var _, w, A = r(5304);
-            class S extends E {
+            class k extends E {
                 constructor() {
                     super(...arguments), this.renderOptions = {
                         host: this
                     }, this._$Do = void 0
                 }
                 createRenderRoot() {
                     var e, t;
@@ -1324,20 +1378,20 @@
                     var e;
                     super.disconnectedCallback(), null === (e = this._$Do) || void 0 === e || e.setConnected(!1)
                 }
                 render() {
                     return A.Jb
                 }
             }
-            S.finalized = !0, S._$litElement$ = !0, null === (_ = globalThis.litElementHydrateSupport) || void 0 === _ || _.call(globalThis, {
-                LitElement: S
+            k.finalized = !0, k._$litElement$ = !0, null === (_ = globalThis.litElementHydrateSupport) || void 0 === _ || _.call(globalThis, {
+                LitElement: k
             });
-            const k = globalThis.litElementPolyfillSupport;
-            null == k || k({
-                LitElement: S
+            const S = globalThis.litElementPolyfillSupport;
+            null == S || S({
+                LitElement: k
             });
             (null !== (w = globalThis.litElementVersions) && void 0 !== w ? w : globalThis.litElementVersions = []).push("3.3.3")
         },
         3204: (e, t, r) => {
             r.d(t, {
                 XA: () => l,
                 ZT: () => i,
@@ -1443,35 +1497,35 @@
     return a.default = () => r, i.d(n, a), n
 }, i.d = (e, t) => {
     for (var r in t) i.o(t, r) && !i.o(e, r) && Object.defineProperty(e, r, {
         enumerable: !0,
         get: t[r]
     })
 }, i.f = {}, i.e = e => Promise.all(Object.keys(i.f).reduce(((t, r) => (i.f[r](e, t), t)), [])), i.u = e => ({
-    15: "yvD5aARM",
+    15: "9yFFShGq",
     210: "yw4J-5vt",
-    244: "oUOHqENt",
+    244: "9VkUPPxQ",
     321: "HyurOyWN",
     338: "sBNRM32J",
     430: "SaPEbRz1",
     442: "X5sZzGl8",
     447: "PHB24J1t",
     456: "JAAifVse",
-    527: "eOHcBlX_",
+    527: "ovjKXg0y",
     537: "fP3U9roj",
-    540: "R9L2-V1R",
     597: "fYLWqtat",
     650: "hzhoTwCw",
     719: "bc9cfM__",
+    770: "gwnfZ3wa",
     776: "mUrtGIle",
     812: "CHsIPDL8",
     879: "oyUFw0ts",
     886: "AuN1Wwjr",
     942: "ZRpJZyXB",
-    981: "bZayZmh0"
+    981: "Ntga-_EF"
 } [e] + ".js"), i.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), i.r = e => {
     "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
         value: "Module"
     }), Object.defineProperty(e, "__esModule", {
         value: !0
     })
 }, i.p = "/lcn_static/frontend_latest/", (() => {
@@ -1797,25 +1851,25 @@
             let i = (t + 16) / 116,
                 n = isNaN(r) ? i : i + r / 500,
                 a = isNaN(o) ? i : i - o / 200;
             i = 1 * E(i), n = p * E(n), a = f * E(a);
             return [y(3.2404542 * n - 1.5371385 * i - .4985314 * a), y(-.969266 * n + 1.8760108 * i + .041556 * a), y(.0556434 * n - .2040259 * i + 1.0572252 * a)]
         },
         A = (e, t = 1) => [e[0] - 18 * t, e[1], e[2]],
-        S = e => {
+        k = e => {
             const t = [0, 0, 0];
             for (let r = 0; r < e.length; r++) {
                 const o = e[r] / 255;
                 t[r] = o <= .03928 ? o / 12.92 : ((o + .055) / 1.055) ** 2.4
             }
             return .2126 * t[0] + .7152 * t[1] + .0722 * t[2]
         },
-        k = (e, t) => {
-            const r = S(e),
-                o = S(t);
+        S = (e, t) => {
+            const r = k(e),
+                o = k(t);
             return r > o ? (r + .05) / (o + .05) : (o + .05) / (r + .05)
         };
     let T = {};
     const H = (e, t, r, o, i) => {
             var n, a;
             const l = r || (i ? t.theme : void 0),
                 h = void 0 !== (null == o ? void 0 : o.dark) ? o.dark : t.darkMode;
@@ -1843,20 +1897,20 @@
                     const e = d(t),
                         r = _(e);
                     f["primary-color"] = t;
                     const o = w(((e, t = 1) => A(e, -t))(r));
                     f["light-primary-color"] = u(o), f["dark-primary-color"] = (e => {
                         const t = w(e);
                         return u(t)
-                    })(A(r)), f["text-primary-color"] = k(e, [33, 33, 33]) < 6 ? "#fff" : "#212121", f["text-light-primary-color"] = k(o, [33, 33, 33]) < 6 ? "#fff" : "#212121", f["state-icon-color"] = f["dark-primary-color"]
+                    })(A(r)), f["text-primary-color"] = S(e, [33, 33, 33]) < 6 ? "#fff" : "#212121", f["text-light-primary-color"] = S(o, [33, 33, 33]) < 6 ? "#fff" : "#212121", f["state-icon-color"] = f["dark-primary-color"]
                 }
                 if (r) {
                     p = `${p}__accent_${r}`, f["accent-color"] = r;
                     const e = d(r);
-                    f["text-accent-color"] = k(e, [33, 33, 33]) < 6 ? "#fff" : "#212121"
+                    f["text-accent-color"] = S(e, [33, 33, 33]) < 6 ? "#fff" : "#212121"
                 }
                 if ((null === (m = e.__themes) || void 0 === m ? void 0 : m.cacheKey) === p) return
             }
             if (l && "default" !== l && t.themes[l]) {
                 const {
                     modes: e,
                     ...r
@@ -1869,28 +1923,28 @@
                     ...e.dark
                 } : {
                     ...f,
                     ...e.light
                 })
             }
             if (!(null !== (n = e.__themes) && void 0 !== n && n.keys || Object.keys(f).length)) return;
-            const b = Object.keys(f).length && p ? T[p] || P(p, f) : void 0,
+            const b = Object.keys(f).length && p ? T[p] || C(p, f) : void 0,
                 g = {
                     ...null === (a = e.__themes) || void 0 === a ? void 0 : a.keys,
                     ...null == b ? void 0 : b.styles
                 };
             if (e.__themes = {
                     cacheKey: p,
                     keys: null == b ? void 0 : b.keys
                 }, e.updateStyles) e.updateStyles(g);
             else if (window.ShadyCSS) window.ShadyCSS.styleSubtree(e, g);
             else
                 for (const s in g) null === s ? e.style.removeProperty(s) : e.style.setProperty(s, g[s])
         },
-        P = (e, t) => {
+        C = (e, t) => {
             if (!t || !Object.keys(t).length) return;
             const r = {
                     ...l,
                     ...t
                 },
                 o = {},
                 i = {};
@@ -1911,17 +1965,17 @@
                 styles: o,
                 keys: i
             }, {
                 styles: o,
                 keys: i
             }
         };
-    var C = i(8480),
-        B = i(625);
-    const x = e.iv`
+    var P = i(8480),
+        x = i(625);
+    const B = e.iv`
   /*
     Home Assistant default styles.
 
     In Polymer 2.0, default styles should to be set on the html selector.
     (Setting all default styles only on body breaks shadyCSS polyfill.)
     See: https://github.com/home-assistant/home-assistant-polymer/pull/901
   */
@@ -2339,17 +2393,17 @@
     --direction: ltr;
     --float-start: left;
     --float-end: right;
 
     ${(0,e.$m)(Object.entries(l).map((([e,t])=>`--${e}: ${t};`)).join(""))}
   }
 `.toString(),
-        R = document.createElement("style");
-    R.textContent = [x, t].join(""), document.head.append(R);
-    var L = i(4516);
+        L = document.createElement("style");
+    L.textContent = [B, t].join(""), document.head.append(L);
+    var R = i(4516);
     let N = (0, r.Z)(null, (function(e, t) {
         class r extends t {
             constructor(...t) {
                 super(...t), e(this)
             }
         }
         return {
@@ -2385,15 +2439,15 @@
                 value() {
                     return !1
                 }
             }, {
                 kind: "field",
                 key: "_computeTail",
                 value() {
-                    return (0, L.Z)((e => {
+                    return (0, R.Z)((e => {
                         const t = e.path.indexOf("/", 1);
                         return -1 === t ? {
                             prefix: e.prefix + e.path,
                             path: ""
                         } : {
                             prefix: e.prefix + e.path.substr(0, t),
                             path: e.path.substr(t)
@@ -2414,15 +2468,15 @@
                     const t = this.routerOptions || {
                         routes: {}
                     };
                     if (t && t.initialLoad && !this._initialLoadDone) return;
                     if (!e.has("route")) return void(this.lastChild && !this._currentLoadProm && this.updatePageEl(this.lastChild, e));
                     const i = this.route,
                         a = t.defaultPage;
-                    i && "" === i.path && void 0 !== a && (0, C.c)(`${i.prefix}/${a}`, {
+                    i && "" === i.path && void 0 !== a && (0, P.c)(`${i.prefix}/${a}`, {
                         replace: !0
                     });
                     let s = i ? ((e, t) => {
                             if ("" === e) return t;
                             const r = e.indexOf("/", 1);
                             return -1 === r ? e.substr(1) : e.substr(1, r - 1)
                         })(i.path, a || "") : "not_found",
@@ -2430,15 +2484,15 @@
                     for (;
                         "string" == typeof l;) s = l, l = t.routes[s];
                     if (t.beforeRender) {
                         const e = t.beforeRender(s);
                         if (void 0 !== e) {
                             for (s = e, l = t.routes[s];
                                 "string" == typeof l;) s = l, l = t.routes[s];
-                            i && (0, C.c)(`${i.prefix}/${e}${location.search}`, {
+                            i && (0, P.c)(`${i.prefix}/${e}${location.search}`, {
                                 replace: !0
                             })
                         }
                     }
                     if (this._currentPage === s) return void(this.lastChild && this.updatePageEl(this.lastChild, e));
                     if (!l) return this._currentPage = "", void(this.lastChild && this.removeChild(this.lastChild));
                     this._currentPage = s;
@@ -2518,14 +2572,36 @@
                     this.lastChild && this.removeChild(this.lastChild);
                     const o = this._cache[t] || this.createElement(r.tag);
                     this.updatePageEl(o), this.appendChild(o), (e.cacheAll || r.cache) && (this._cache[t] = o)
                 }
             }]
         }
     }), e.fl);
+    class $ {
+        constructor(e) {
+            this.prefix = void 0, this.prefix = e ? `[lcn.${e}]` : "[lcn]"
+        }
+        info(...e) {
+            console.info(this.prefix, ...e)
+        }
+        log(...e) {
+            console.log(this.prefix, ...e)
+        }
+        debug(...e) {
+            console.debug(this.prefix, ...e)
+        }
+        warn(...e) {
+            console.warn(this.prefix, ...e)
+        }
+        error(...e) {
+            console.error(this.prefix, ...e)
+        }
+    }
+    var I = i(9051);
+    const O = new $("router");
     (0, r.Z)([(0, a.Mo)("lcn-router")], (function(e, t) {
         return {
             F: class extends t {
                 constructor(...t) {
                     super(...t), e(this)
                 }
             },
@@ -2549,105 +2625,117 @@
                     attribute: !1
                 })],
                 key: "route",
                 value: void 0
             }, {
                 kind: "field",
                 decorators: [(0, a.Cb)({
-                    attribute: !1
+                    type: Boolean
                 })],
                 key: "narrow",
                 value: void 0
             }, {
                 kind: "field",
+                decorators: [(0, a.SB)()],
+                key: "hosts",
+                value: void 0
+            }, {
+                kind: "field",
                 key: "routerOptions",
                 value() {
                     return {
                         defaultPage: "devices",
                         showLoading: !0,
                         routes: {
                             devices: {
                                 tag: "lcn-config-dashboard",
-                                load: () => (console.log("Importing lcn-config-dashboard"), Promise.all([i.e(210), i.e(321), i.e(430), i.e(650), i.e(776), i.e(540), i.e(15)]).then(i.bind(i, 9015)))
+                                load: () => (O.debug("Importing lcn-config-dashboard"), Promise.all([i.e(210), i.e(321), i.e(430), i.e(650), i.e(776), i.e(770), i.e(15)]).then(i.bind(i, 9015)))
                             },
                             entities: {
                                 tag: "lcn-entities-page",
-                                load: () => (console.log("Importing lcn-entities-page"), Promise.all([i.e(210), i.e(430), i.e(776), i.e(540), i.e(981)]).then(i.bind(i, 981)))
+                                load: () => (O.debug("Importing lcn-entities-page"), Promise.all([i.e(210), i.e(430), i.e(776), i.e(770), i.e(981)]).then(i.bind(i, 981)))
                             }
-                        }
+                        },
+                        initialLoad: () => this._fetchHosts()
                     }
                 }
             }, {
                 kind: "method",
                 key: "updatePageEl",
                 value: function(e) {
-                    e.hass = this.hass, e.lcn = this.lcn, e.route = this.routeTail, e.narrow = this.narrow, console.log(`Current Page: ${this._currentPage} Route: ${this.route.path}`)
+                    e.hass = this.hass, e.lcn = this.lcn, e.route = this.routeTail, e.narrow = this.narrow, "devices" === this._currentPage && (e.hosts = this.hosts), O.debug(`Current Page: ${this._currentPage} Route: ${this.route.path}`)
+                }
+            }, {
+                kind: "method",
+                key: "_fetchHosts",
+                value: async function() {
+                    this.hosts = await (0, I.V5)(this.hass)
                 }
             }]
         }
     }), N);
-    var $, O, I, M = i(3204);
-
-    function U(e) {
-        return e.type === O.literal
-    }
-
-    function D(e) {
-        return e.type === O.argument
-    }
-
-    function G(e) {
-        return e.type === O.number
-    }
+    var M, D, U, G = i(3204);
 
     function F(e) {
-        return e.type === O.date
+        return e.type === D.literal
     }
 
     function j(e) {
-        return e.type === O.time
+        return e.type === D.argument
     }
 
     function z(e) {
-        return e.type === O.select
+        return e.type === D.number
     }
 
     function V(e) {
-        return e.type === O.plural
+        return e.type === D.date
+    }
+
+    function K(e) {
+        return e.type === D.time
     }
 
     function Z(e) {
-        return e.type === O.pound
+        return e.type === D.select
     }
 
-    function K(e) {
-        return e.type === O.tag
+    function W(e) {
+        return e.type === D.plural
     }
 
     function X(e) {
-        return !(!e || "object" != typeof e || e.type !== I.number)
+        return e.type === D.pound
     }
 
-    function W(e) {
-        return !(!e || "object" != typeof e || e.type !== I.dateTime)
+    function Y(e) {
+        return e.type === D.tag
+    }
+
+    function q(e) {
+        return !(!e || "object" != typeof e || e.type !== U.number)
+    }
+
+    function J(e) {
+        return !(!e || "object" != typeof e || e.type !== U.dateTime)
     }! function(e) {
         e[e.EXPECT_ARGUMENT_CLOSING_BRACE = 1] = "EXPECT_ARGUMENT_CLOSING_BRACE", e[e.EMPTY_ARGUMENT = 2] = "EMPTY_ARGUMENT", e[e.MALFORMED_ARGUMENT = 3] = "MALFORMED_ARGUMENT", e[e.EXPECT_ARGUMENT_TYPE = 4] = "EXPECT_ARGUMENT_TYPE", e[e.INVALID_ARGUMENT_TYPE = 5] = "INVALID_ARGUMENT_TYPE", e[e.EXPECT_ARGUMENT_STYLE = 6] = "EXPECT_ARGUMENT_STYLE", e[e.INVALID_NUMBER_SKELETON = 7] = "INVALID_NUMBER_SKELETON", e[e.INVALID_DATE_TIME_SKELETON = 8] = "INVALID_DATE_TIME_SKELETON", e[e.EXPECT_NUMBER_SKELETON = 9] = "EXPECT_NUMBER_SKELETON", e[e.EXPECT_DATE_TIME_SKELETON = 10] = "EXPECT_DATE_TIME_SKELETON", e[e.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE = 11] = "UNCLOSED_QUOTE_IN_ARGUMENT_STYLE", e[e.EXPECT_SELECT_ARGUMENT_OPTIONS = 12] = "EXPECT_SELECT_ARGUMENT_OPTIONS", e[e.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE = 13] = "EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE", e[e.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE = 14] = "INVALID_PLURAL_ARGUMENT_OFFSET_VALUE", e[e.EXPECT_SELECT_ARGUMENT_SELECTOR = 15] = "EXPECT_SELECT_ARGUMENT_SELECTOR", e[e.EXPECT_PLURAL_ARGUMENT_SELECTOR = 16] = "EXPECT_PLURAL_ARGUMENT_SELECTOR", e[e.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT = 17] = "EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT", e[e.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT = 18] = "EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT", e[e.INVALID_PLURAL_ARGUMENT_SELECTOR = 19] = "INVALID_PLURAL_ARGUMENT_SELECTOR", e[e.DUPLICATE_PLURAL_ARGUMENT_SELECTOR = 20] = "DUPLICATE_PLURAL_ARGUMENT_SELECTOR", e[e.DUPLICATE_SELECT_ARGUMENT_SELECTOR = 21] = "DUPLICATE_SELECT_ARGUMENT_SELECTOR", e[e.MISSING_OTHER_CLAUSE = 22] = "MISSING_OTHER_CLAUSE", e[e.INVALID_TAG = 23] = "INVALID_TAG", e[e.INVALID_TAG_NAME = 25] = "INVALID_TAG_NAME", e[e.UNMATCHED_CLOSING_TAG = 26] = "UNMATCHED_CLOSING_TAG", e[e.UNCLOSED_TAG = 27] = "UNCLOSED_TAG"
-    }($ || ($ = {})),
+    }(M || (M = {})),
     function(e) {
         e[e.literal = 0] = "literal", e[e.argument = 1] = "argument", e[e.number = 2] = "number", e[e.date = 3] = "date", e[e.time = 4] = "time", e[e.select = 5] = "select", e[e.plural = 6] = "plural", e[e.pound = 7] = "pound", e[e.tag = 8] = "tag"
-    }(O || (O = {})),
+    }(D || (D = {})),
     function(e) {
         e[e.number = 0] = "number", e[e.dateTime = 1] = "dateTime"
-    }(I || (I = {}));
-    var Y = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
-        q = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
+    }(U || (U = {}));
+    var Q = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
+        ee = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
 
-    function J(e) {
+    function te(e) {
         var t = {};
-        return e.replace(q, (function(e) {
+        return e.replace(ee, (function(e) {
             var r = e.length;
             switch (e[0]) {
                 case "G":
                     t.era = 4 === r ? "long" : 5 === r ? "narrow" : "short";
                     break;
                 case "y":
                     t.year = 2 === r ? "2-digit" : "numeric";
@@ -2726,28 +2814,28 @@
                 case "X":
                 case "x":
                     throw new RangeError("`Z/O/v/V/X/x` (timeZone) patterns are not supported, use `z` instead")
             }
             return ""
         })), t
     }
-    var Q = /[\t-\r \x85\u200E\u200F\u2028\u2029]/i;
-    var ee = /^\.(?:(0+)(\*)?|(#+)|(0+)(#+))$/g,
-        te = /^(@+)?(\+|#+)?[rs]?$/g,
-        re = /(\*)(0+)|(#+)(0+)|(0+)/g,
-        oe = /^(0+)$/;
+    var re = /[\t-\r \x85\u200E\u200F\u2028\u2029]/i;
+    var oe = /^\.(?:(0+)(\*)?|(#+)|(0+)(#+))$/g,
+        ie = /^(@+)?(\+|#+)?[rs]?$/g,
+        ne = /(\*)(0+)|(#+)(0+)|(0+)/g,
+        ae = /^(0+)$/;
 
-    function ie(e) {
+    function se(e) {
         var t = {};
-        return "r" === e[e.length - 1] ? t.roundingPriority = "morePrecision" : "s" === e[e.length - 1] && (t.roundingPriority = "lessPrecision"), e.replace(te, (function(e, r, o) {
+        return "r" === e[e.length - 1] ? t.roundingPriority = "morePrecision" : "s" === e[e.length - 1] && (t.roundingPriority = "lessPrecision"), e.replace(ie, (function(e, r, o) {
             return "string" != typeof o ? (t.minimumSignificantDigits = r.length, t.maximumSignificantDigits = r.length) : "+" === o ? t.minimumSignificantDigits = r.length : "#" === r[0] ? t.maximumSignificantDigits = r.length : (t.minimumSignificantDigits = r.length, t.maximumSignificantDigits = r.length + ("string" == typeof o ? o.length : 0)), ""
         })), t
     }
 
-    function ne(e) {
+    function le(e) {
         switch (e) {
             case "sign-auto":
                 return {
                     signDisplay: "auto"
                 };
             case "sign-accounting":
             case "()":
@@ -2778,34 +2866,34 @@
             case "+_":
                 return {
                     signDisplay: "never"
                 }
         }
     }
 
-    function ae(e) {
+    function ce(e) {
         var t;
         if ("E" === e[0] && "E" === e[1] ? (t = {
                 notation: "engineering"
             }, e = e.slice(2)) : "E" === e[0] && (t = {
                 notation: "scientific"
             }, e = e.slice(1)), t) {
             var r = e.slice(0, 2);
-            if ("+!" === r ? (t.signDisplay = "always", e = e.slice(2)) : "+?" === r && (t.signDisplay = "exceptZero", e = e.slice(2)), !oe.test(e)) throw new Error("Malformed concise eng/scientific notation");
+            if ("+!" === r ? (t.signDisplay = "always", e = e.slice(2)) : "+?" === r && (t.signDisplay = "exceptZero", e = e.slice(2)), !ae.test(e)) throw new Error("Malformed concise eng/scientific notation");
             t.minimumIntegerDigits = e.length
         }
         return t
     }
 
-    function se(e) {
-        var t = ne(e);
+    function he(e) {
+        var t = le(e);
         return t || {}
     }
 
-    function le(e) {
+    function de(e) {
         for (var t = {}, r = 0, o = e; r < o.length; r++) {
             var i = o[r];
             switch (i.stem) {
                 case "percent":
                 case "%":
                     t.style = "percent";
                     continue;
@@ -2832,25 +2920,25 @@
                     t.notation = "compact", t.compactDisplay = "short";
                     continue;
                 case "compact-long":
                 case "KK":
                     t.notation = "compact", t.compactDisplay = "long";
                     continue;
                 case "scientific":
-                    t = (0, M.pi)((0, M.pi)((0, M.pi)({}, t), {
+                    t = (0, G.pi)((0, G.pi)((0, G.pi)({}, t), {
                         notation: "scientific"
                     }), i.options.reduce((function(e, t) {
-                        return (0, M.pi)((0, M.pi)({}, e), se(t))
+                        return (0, G.pi)((0, G.pi)({}, e), he(t))
                     }), {}));
                     continue;
                 case "engineering":
-                    t = (0, M.pi)((0, M.pi)((0, M.pi)({}, t), {
+                    t = (0, G.pi)((0, G.pi)((0, G.pi)({}, t), {
                         notation: "engineering"
                     }), i.options.reduce((function(e, t) {
-                        return (0, M.pi)((0, M.pi)({}, e), se(t))
+                        return (0, G.pi)((0, G.pi)({}, e), he(t))
                     }), {}));
                     continue;
                 case "notation-simple":
                     t.notation = "standard";
                     continue;
                 case "unit-width-narrow":
                     t.currencyDisplay = "narrowSymbol", t.unitDisplay = "narrow";
@@ -2865,45 +2953,45 @@
                     t.currencyDisplay = "symbol";
                     continue;
                 case "scale":
                     t.scale = parseFloat(i.options[0]);
                     continue;
                 case "integer-width":
                     if (i.options.length > 1) throw new RangeError("integer-width stems only accept a single optional option");
-                    i.options[0].replace(re, (function(e, r, o, i, n, a) {
+                    i.options[0].replace(ne, (function(e, r, o, i, n, a) {
                         if (r) t.minimumIntegerDigits = o.length;
                         else {
                             if (i && n) throw new Error("We currently do not support maximum integer digits");
                             if (a) throw new Error("We currently do not support exact integer digits")
                         }
                         return ""
                     }));
                     continue
             }
-            if (oe.test(i.stem)) t.minimumIntegerDigits = i.stem.length;
-            else if (ee.test(i.stem)) {
+            if (ae.test(i.stem)) t.minimumIntegerDigits = i.stem.length;
+            else if (oe.test(i.stem)) {
                 if (i.options.length > 1) throw new RangeError("Fraction-precision stems only accept a single optional option");
-                i.stem.replace(ee, (function(e, r, o, i, n, a) {
+                i.stem.replace(oe, (function(e, r, o, i, n, a) {
                     return "*" === o ? t.minimumFractionDigits = r.length : i && "#" === i[0] ? t.maximumFractionDigits = i.length : n && a ? (t.minimumFractionDigits = n.length, t.maximumFractionDigits = n.length + a.length) : (t.minimumFractionDigits = r.length, t.maximumFractionDigits = r.length), ""
                 }));
                 var n = i.options[0];
-                "w" === n ? t = (0, M.pi)((0, M.pi)({}, t), {
+                "w" === n ? t = (0, G.pi)((0, G.pi)({}, t), {
                     trailingZeroDisplay: "stripIfInteger"
-                }) : n && (t = (0, M.pi)((0, M.pi)({}, t), ie(n)))
-            } else if (te.test(i.stem)) t = (0, M.pi)((0, M.pi)({}, t), ie(i.stem));
+                }) : n && (t = (0, G.pi)((0, G.pi)({}, t), se(n)))
+            } else if (ie.test(i.stem)) t = (0, G.pi)((0, G.pi)({}, t), se(i.stem));
             else {
-                var a = ne(i.stem);
-                a && (t = (0, M.pi)((0, M.pi)({}, t), a));
-                var s = ae(i.stem);
-                s && (t = (0, M.pi)((0, M.pi)({}, t), s))
+                var a = le(i.stem);
+                a && (t = (0, G.pi)((0, G.pi)({}, t), a));
+                var s = ce(i.stem);
+                s && (t = (0, G.pi)((0, G.pi)({}, t), s))
             }
         }
         return t
     }
-    var ce, he = {
+    var ue, pe = {
         "001": ["H", "h"],
         AC: ["H", "h", "hb", "hB"],
         AD: ["H", "hB"],
         AE: ["h", "hB", "hb", "H"],
         AF: ["H", "hb", "hB", "h"],
         AG: ["h", "hb", "H", "hB"],
         AI: ["H", "h", "hb", "hB"],
@@ -3171,115 +3259,115 @@
         "mr-IN": ["hB", "hb", "h", "H"],
         "pa-IN": ["hB", "hb", "h", "H"],
         "ta-IN": ["hB", "h", "hb", "H"],
         "te-IN": ["hB", "h", "H"],
         "zu-ZA": ["H", "hB", "hb", "h"]
     };
 
-    function de(e) {
+    function fe(e) {
         var t = e.hourCycle;
         if (void 0 === t && e.hourCycles && e.hourCycles.length && (t = e.hourCycles[0]), t) switch (t) {
             case "h24":
                 return "k";
             case "h23":
                 return "H";
             case "h12":
                 return "h";
             case "h11":
                 return "K";
             default:
                 throw new Error("Invalid hourCycle")
         }
         var r, o = e.language;
-        return "root" !== o && (r = e.maximize().region), (he[r || ""] || he[o || ""] || he["".concat(o, "-001")] || he["001"])[0]
+        return "root" !== o && (r = e.maximize().region), (pe[r || ""] || pe[o || ""] || pe["".concat(o, "-001")] || pe["001"])[0]
     }
-    var ue = new RegExp("^".concat(Y.source, "*")),
-        pe = new RegExp("".concat(Y.source, "*$"));
+    var me = new RegExp("^".concat(Q.source, "*")),
+        be = new RegExp("".concat(Q.source, "*$"));
 
-    function fe(e, t) {
+    function ge(e, t) {
         return {
             start: e,
             end: t
         }
     }
-    var me = !!String.prototype.startsWith && "_a".startsWith("a", 1),
-        be = !!String.fromCodePoint,
-        ge = !!Object.fromEntries,
-        ve = !!String.prototype.codePointAt,
-        ye = !!String.prototype.trimStart,
-        Ee = !!String.prototype.trimEnd,
-        _e = !!Number.isSafeInteger ? Number.isSafeInteger : function(e) {
+    var ve = !!String.prototype.startsWith && "_a".startsWith("a", 1),
+        ye = !!String.fromCodePoint,
+        Ee = !!Object.fromEntries,
+        _e = !!String.prototype.codePointAt,
+        we = !!String.prototype.trimStart,
+        Ae = !!String.prototype.trimEnd,
+        ke = !!Number.isSafeInteger ? Number.isSafeInteger : function(e) {
             return "number" == typeof e && isFinite(e) && Math.floor(e) === e && Math.abs(e) <= 9007199254740991
         },
-        we = !0;
+        Se = !0;
     try {
-        we = "a" === (null === (ce = Be("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu").exec("a")) || void 0 === ce ? void 0 : ce[0])
-    } catch (ft) {
-        we = !1
+        Se = "a" === (null === (ue = Re("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu").exec("a")) || void 0 === ue ? void 0 : ue[0])
+    } catch (vt) {
+        Se = !1
     }
-    var Ae, Se = me ? function(e, t, r) {
+    var Te, He = ve ? function(e, t, r) {
             return e.startsWith(t, r)
         } : function(e, t, r) {
             return e.slice(r, r + t.length) === t
         },
-        ke = be ? String.fromCodePoint : function() {
+        Ce = ye ? String.fromCodePoint : function() {
             for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
             for (var r, o = "", i = e.length, n = 0; i > n;) {
                 if ((r = e[n++]) > 1114111) throw RangeError(r + " is not a valid code point");
                 o += r < 65536 ? String.fromCharCode(r) : String.fromCharCode(55296 + ((r -= 65536) >> 10), r % 1024 + 56320)
             }
             return o
         },
-        Te = ge ? Object.fromEntries : function(e) {
+        Pe = Ee ? Object.fromEntries : function(e) {
             for (var t = {}, r = 0, o = e; r < o.length; r++) {
                 var i = o[r],
                     n = i[0],
                     a = i[1];
                 t[n] = a
             }
             return t
         },
-        He = ve ? function(e, t) {
+        xe = _e ? function(e, t) {
             return e.codePointAt(t)
         } : function(e, t) {
             var r = e.length;
             if (!(t < 0 || t >= r)) {
                 var o, i = e.charCodeAt(t);
                 return i < 55296 || i > 56319 || t + 1 === r || (o = e.charCodeAt(t + 1)) < 56320 || o > 57343 ? i : o - 56320 + (i - 55296 << 10) + 65536
             }
         },
-        Pe = ye ? function(e) {
+        Be = we ? function(e) {
             return e.trimStart()
         } : function(e) {
-            return e.replace(ue, "")
+            return e.replace(me, "")
         },
-        Ce = Ee ? function(e) {
+        Le = Ae ? function(e) {
             return e.trimEnd()
         } : function(e) {
-            return e.replace(pe, "")
+            return e.replace(be, "")
         };
 
-    function Be(e, t) {
+    function Re(e, t) {
         return new RegExp(e, t)
     }
-    if (we) {
-        var xe = Be("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
-        Ae = function(e, t) {
+    if (Se) {
+        var Ne = Re("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
+        Te = function(e, t) {
             var r;
-            return xe.lastIndex = t, null !== (r = xe.exec(e)[1]) && void 0 !== r ? r : ""
+            return Ne.lastIndex = t, null !== (r = Ne.exec(e)[1]) && void 0 !== r ? r : ""
         }
-    } else Ae = function(e, t) {
+    } else Te = function(e, t) {
         for (var r = [];;) {
-            var o = He(e, t);
-            if (void 0 === o || Ne(o) || $e(o)) break;
+            var o = xe(e, t);
+            if (void 0 === o || Oe(o) || Me(o)) break;
             r.push(o), t += o >= 65536 ? 2 : 1
         }
-        return ke.apply(void 0, r)
+        return Ce.apply(void 0, r)
     };
-    var Re = function() {
+    var $e = function() {
         function e(e, t) {
             void 0 === t && (t = {}), this.message = e, this.position = {
                 offset: 0,
                 line: 1,
                 column: 1
             }, this.ignoreTag = !!t.ignoreTag, this.locale = t.locale, this.requiresOtherClause = !!t.requiresOtherClause, this.shouldParseSkeletons = !!t.shouldParseSkeletons
         }
@@ -3293,70 +3381,70 @@
                     if ((n = this.parseArgument(e, r)).err) return n;
                     o.push(n.val)
                 } else {
                     if (125 === i && e > 0) break;
                     if (35 !== i || "plural" !== t && "selectordinal" !== t) {
                         if (60 === i && !this.ignoreTag && 47 === this.peek()) {
                             if (r) break;
-                            return this.error($.UNMATCHED_CLOSING_TAG, fe(this.clonePosition(), this.clonePosition()))
+                            return this.error(M.UNMATCHED_CLOSING_TAG, ge(this.clonePosition(), this.clonePosition()))
                         }
-                        if (60 === i && !this.ignoreTag && Le(this.peek() || 0)) {
+                        if (60 === i && !this.ignoreTag && Ie(this.peek() || 0)) {
                             if ((n = this.parseTag(e, t)).err) return n;
                             o.push(n.val)
                         } else {
                             var n;
                             if ((n = this.parseLiteral(e, t)).err) return n;
                             o.push(n.val)
                         }
                     } else {
                         var a = this.clonePosition();
                         this.bump(), o.push({
-                            type: O.pound,
-                            location: fe(a, this.clonePosition())
+                            type: D.pound,
+                            location: ge(a, this.clonePosition())
                         })
                     }
                 }
             }
             return {
                 val: o,
                 err: null
             }
         }, e.prototype.parseTag = function(e, t) {
             var r = this.clonePosition();
             this.bump();
             var o = this.parseTagName();
             if (this.bumpSpace(), this.bumpIf("/>")) return {
                 val: {
-                    type: O.literal,
+                    type: D.literal,
                     value: "<".concat(o, "/>"),
-                    location: fe(r, this.clonePosition())
+                    location: ge(r, this.clonePosition())
                 },
                 err: null
             };
             if (this.bumpIf(">")) {
                 var i = this.parseMessage(e + 1, t, !0);
                 if (i.err) return i;
                 var n = i.val,
                     a = this.clonePosition();
                 if (this.bumpIf("</")) {
-                    if (this.isEOF() || !Le(this.char())) return this.error($.INVALID_TAG, fe(a, this.clonePosition()));
+                    if (this.isEOF() || !Ie(this.char())) return this.error(M.INVALID_TAG, ge(a, this.clonePosition()));
                     var s = this.clonePosition();
-                    return o !== this.parseTagName() ? this.error($.UNMATCHED_CLOSING_TAG, fe(s, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
+                    return o !== this.parseTagName() ? this.error(M.UNMATCHED_CLOSING_TAG, ge(s, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
                         val: {
-                            type: O.tag,
+                            type: D.tag,
                             value: o,
                             children: n,
-                            location: fe(r, this.clonePosition())
+                            location: ge(r, this.clonePosition())
                         },
                         err: null
-                    } : this.error($.INVALID_TAG, fe(a, this.clonePosition())))
+                    } : this.error(M.INVALID_TAG, ge(a, this.clonePosition())))
                 }
-                return this.error($.UNCLOSED_TAG, fe(r, this.clonePosition()))
+                return this.error(M.UNCLOSED_TAG, ge(r, this.clonePosition()))
             }
-            return this.error($.INVALID_TAG, fe(r, this.clonePosition()))
+            return this.error(M.INVALID_TAG, ge(r, this.clonePosition()))
         }, e.prototype.parseTagName = function() {
             var e, t = this.offset();
             for (this.bump(); !this.isEOF() && (45 === (e = this.char()) || 46 === e || e >= 48 && e <= 57 || 95 === e || e >= 97 && e <= 122 || e >= 65 && e <= 90 || 183 == e || e >= 192 && e <= 214 || e >= 216 && e <= 246 || e >= 248 && e <= 893 || e >= 895 && e <= 8191 || e >= 8204 && e <= 8205 || e >= 8255 && e <= 8256 || e >= 8304 && e <= 8591 || e >= 11264 && e <= 12271 || e >= 12289 && e <= 55295 || e >= 63744 && e <= 64975 || e >= 65008 && e <= 65533 || e >= 65536 && e <= 983039);) this.bump();
             return this.message.slice(t, this.offset())
         }, e.prototype.parseLiteral = function(e, t) {
             for (var r = this.clonePosition(), o = "";;) {
                 var i = this.tryParseQuote(t);
@@ -3367,25 +3455,25 @@
                     else {
                         var a = this.tryParseLeftAngleBracket();
                         if (!a) break;
                         o += a
                     }
                 }
             }
-            var s = fe(r, this.clonePosition());
+            var s = ge(r, this.clonePosition());
             return {
                 val: {
-                    type: O.literal,
+                    type: D.literal,
                     value: o,
                     location: s
                 },
                 err: null
             }
         }, e.prototype.tryParseLeftAngleBracket = function() {
-            return this.isEOF() || 60 !== this.char() || !this.ignoreTag && (Le(e = this.peek() || 0) || 47 === e) ? null : (this.bump(), "<");
+            return this.isEOF() || 60 !== this.char() || !this.ignoreTag && (Ie(e = this.peek() || 0) || 47 === e) ? null : (this.bump(), "<");
             var e
         }, e.prototype.tryParseQuote = function(e) {
             if (this.isEOF() || 39 !== this.char()) return null;
             switch (this.peek()) {
                 case 39:
                     return this.bump(), this.bump(), "'";
                 case 123:
@@ -3408,177 +3496,177 @@
                         this.bump();
                         break
                     }
                     t.push(39), this.bump()
                 } else t.push(r);
                 this.bump()
             }
-            return ke.apply(void 0, t)
+            return Ce.apply(void 0, t)
         }, e.prototype.tryParseUnquoted = function(e, t) {
             if (this.isEOF()) return null;
             var r = this.char();
-            return 60 === r || 123 === r || 35 === r && ("plural" === t || "selectordinal" === t) || 125 === r && e > 0 ? null : (this.bump(), ke(r))
+            return 60 === r || 123 === r || 35 === r && ("plural" === t || "selectordinal" === t) || 125 === r && e > 0 ? null : (this.bump(), Ce(r))
         }, e.prototype.parseArgument = function(e, t) {
             var r = this.clonePosition();
-            if (this.bump(), this.bumpSpace(), this.isEOF()) return this.error($.EXPECT_ARGUMENT_CLOSING_BRACE, fe(r, this.clonePosition()));
-            if (125 === this.char()) return this.bump(), this.error($.EMPTY_ARGUMENT, fe(r, this.clonePosition()));
+            if (this.bump(), this.bumpSpace(), this.isEOF()) return this.error(M.EXPECT_ARGUMENT_CLOSING_BRACE, ge(r, this.clonePosition()));
+            if (125 === this.char()) return this.bump(), this.error(M.EMPTY_ARGUMENT, ge(r, this.clonePosition()));
             var o = this.parseIdentifierIfPossible().value;
-            if (!o) return this.error($.MALFORMED_ARGUMENT, fe(r, this.clonePosition()));
-            if (this.bumpSpace(), this.isEOF()) return this.error($.EXPECT_ARGUMENT_CLOSING_BRACE, fe(r, this.clonePosition()));
+            if (!o) return this.error(M.MALFORMED_ARGUMENT, ge(r, this.clonePosition()));
+            if (this.bumpSpace(), this.isEOF()) return this.error(M.EXPECT_ARGUMENT_CLOSING_BRACE, ge(r, this.clonePosition()));
             switch (this.char()) {
                 case 125:
                     return this.bump(), {
                         val: {
-                            type: O.argument,
+                            type: D.argument,
                             value: o,
-                            location: fe(r, this.clonePosition())
+                            location: ge(r, this.clonePosition())
                         },
                         err: null
                     };
                 case 44:
-                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error($.EXPECT_ARGUMENT_CLOSING_BRACE, fe(r, this.clonePosition())) : this.parseArgumentOptions(e, t, o, r);
+                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(M.EXPECT_ARGUMENT_CLOSING_BRACE, ge(r, this.clonePosition())) : this.parseArgumentOptions(e, t, o, r);
                 default:
-                    return this.error($.MALFORMED_ARGUMENT, fe(r, this.clonePosition()))
+                    return this.error(M.MALFORMED_ARGUMENT, ge(r, this.clonePosition()))
             }
         }, e.prototype.parseIdentifierIfPossible = function() {
             var e = this.clonePosition(),
                 t = this.offset(),
-                r = Ae(this.message, t),
+                r = Te(this.message, t),
                 o = t + r.length;
             return this.bumpTo(o), {
                 value: r,
-                location: fe(e, this.clonePosition())
+                location: ge(e, this.clonePosition())
             }
         }, e.prototype.parseArgumentOptions = function(e, t, r, o) {
             var i, n = this.clonePosition(),
                 a = this.parseIdentifierIfPossible().value,
                 s = this.clonePosition();
             switch (a) {
                 case "":
-                    return this.error($.EXPECT_ARGUMENT_TYPE, fe(n, s));
+                    return this.error(M.EXPECT_ARGUMENT_TYPE, ge(n, s));
                 case "number":
                 case "date":
                 case "time":
                     this.bumpSpace();
                     var l = null;
                     if (this.bumpIf(",")) {
                         this.bumpSpace();
                         var c = this.clonePosition();
                         if ((g = this.parseSimpleArgStyleIfPossible()).err) return g;
-                        if (0 === (p = Ce(g.val)).length) return this.error($.EXPECT_ARGUMENT_STYLE, fe(this.clonePosition(), this.clonePosition()));
+                        if (0 === (p = Le(g.val)).length) return this.error(M.EXPECT_ARGUMENT_STYLE, ge(this.clonePosition(), this.clonePosition()));
                         l = {
                             style: p,
-                            styleLocation: fe(c, this.clonePosition())
+                            styleLocation: ge(c, this.clonePosition())
                         }
                     }
                     if ((v = this.tryParseArgumentClose(o)).err) return v;
-                    var h = fe(o, this.clonePosition());
-                    if (l && Se(null == l ? void 0 : l.style, "::", 0)) {
-                        var d = Pe(l.style.slice(2));
+                    var h = ge(o, this.clonePosition());
+                    if (l && He(null == l ? void 0 : l.style, "::", 0)) {
+                        var d = Be(l.style.slice(2));
                         if ("number" === a) return (g = this.parseNumberSkeletonFromString(d, l.styleLocation)).err ? g : {
                             val: {
-                                type: O.number,
+                                type: D.number,
                                 value: r,
                                 location: h,
                                 style: g.val
                             },
                             err: null
                         };
-                        if (0 === d.length) return this.error($.EXPECT_DATE_TIME_SKELETON, h);
+                        if (0 === d.length) return this.error(M.EXPECT_DATE_TIME_SKELETON, h);
                         var u = d;
                         this.locale && (u = function(e, t) {
                             for (var r = "", o = 0; o < e.length; o++) {
                                 var i = e.charAt(o);
                                 if ("j" === i) {
                                     for (var n = 0; o + 1 < e.length && e.charAt(o + 1) === i;) n++, o++;
                                     var a = 1 + (1 & n),
                                         s = n < 2 ? 1 : 3 + (n >> 1),
-                                        l = de(t);
+                                        l = fe(t);
                                     for ("H" != l && "k" != l || (s = 0); s-- > 0;) r += "a";
                                     for (; a-- > 0;) r = l + r
                                 } else r += "J" === i ? "H" : i
                             }
                             return r
                         }(d, this.locale));
                         var p = {
-                            type: I.dateTime,
+                            type: U.dateTime,
                             pattern: u,
                             location: l.styleLocation,
-                            parsedOptions: this.shouldParseSkeletons ? J(u) : {}
+                            parsedOptions: this.shouldParseSkeletons ? te(u) : {}
                         };
                         return {
                             val: {
-                                type: "date" === a ? O.date : O.time,
+                                type: "date" === a ? D.date : D.time,
                                 value: r,
                                 location: h,
                                 style: p
                             },
                             err: null
                         }
                     }
                     return {
                         val: {
-                            type: "number" === a ? O.number : "date" === a ? O.date : O.time,
+                            type: "number" === a ? D.number : "date" === a ? D.date : D.time,
                             value: r,
                             location: h,
                             style: null !== (i = null == l ? void 0 : l.style) && void 0 !== i ? i : null
                         }, err: null
                     };
                 case "plural":
                 case "selectordinal":
                 case "select":
                     var f = this.clonePosition();
-                    if (this.bumpSpace(), !this.bumpIf(",")) return this.error($.EXPECT_SELECT_ARGUMENT_OPTIONS, fe(f, (0, M.pi)({}, f)));
+                    if (this.bumpSpace(), !this.bumpIf(",")) return this.error(M.EXPECT_SELECT_ARGUMENT_OPTIONS, ge(f, (0, G.pi)({}, f)));
                     this.bumpSpace();
                     var m = this.parseIdentifierIfPossible(),
                         b = 0;
                     if ("select" !== a && "offset" === m.value) {
-                        if (!this.bumpIf(":")) return this.error($.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, fe(this.clonePosition(), this.clonePosition()));
+                        if (!this.bumpIf(":")) return this.error(M.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, ge(this.clonePosition(), this.clonePosition()));
                         var g;
-                        if (this.bumpSpace(), (g = this.tryParseDecimalInteger($.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, $.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE)).err) return g;
+                        if (this.bumpSpace(), (g = this.tryParseDecimalInteger(M.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, M.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE)).err) return g;
                         this.bumpSpace(), m = this.parseIdentifierIfPossible(), b = g.val
                     }
                     var v, y = this.tryParsePluralOrSelectOptions(e, a, t, m);
                     if (y.err) return y;
                     if ((v = this.tryParseArgumentClose(o)).err) return v;
-                    var E = fe(o, this.clonePosition());
+                    var E = ge(o, this.clonePosition());
                     return "select" === a ? {
                         val: {
-                            type: O.select,
+                            type: D.select,
                             value: r,
-                            options: Te(y.val),
+                            options: Pe(y.val),
                             location: E
                         },
                         err: null
                     } : {
                         val: {
-                            type: O.plural,
+                            type: D.plural,
                             value: r,
-                            options: Te(y.val),
+                            options: Pe(y.val),
                             offset: b,
                             pluralType: "plural" === a ? "cardinal" : "ordinal",
                             location: E
                         },
                         err: null
                     };
                 default:
-                    return this.error($.INVALID_ARGUMENT_TYPE, fe(n, s))
+                    return this.error(M.INVALID_ARGUMENT_TYPE, ge(n, s))
             }
         }, e.prototype.tryParseArgumentClose = function(e) {
-            return this.isEOF() || 125 !== this.char() ? this.error($.EXPECT_ARGUMENT_CLOSING_BRACE, fe(e, this.clonePosition())) : (this.bump(), {
+            return this.isEOF() || 125 !== this.char() ? this.error(M.EXPECT_ARGUMENT_CLOSING_BRACE, ge(e, this.clonePosition())) : (this.bump(), {
                 val: !0,
                 err: null
             })
         }, e.prototype.parseSimpleArgStyleIfPossible = function() {
             for (var e = 0, t = this.clonePosition(); !this.isEOF();) {
                 switch (this.char()) {
                     case 39:
                         this.bump();
                         var r = this.clonePosition();
-                        if (!this.bumpUntil("'")) return this.error($.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, fe(r, this.clonePosition()));
+                        if (!this.bumpUntil("'")) return this.error(M.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, ge(r, this.clonePosition()));
                         this.bump();
                         break;
                     case 123:
                         e += 1, this.bump();
                         break;
                     case 125:
                         if (!(e > 0)) return {
@@ -3596,77 +3684,77 @@
                 err: null
             }
         }, e.prototype.parseNumberSkeletonFromString = function(e, t) {
             var r = [];
             try {
                 r = function(e) {
                     if (0 === e.length) throw new Error("Number skeleton cannot be empty");
-                    for (var t = [], r = 0, o = e.split(Q).filter((function(e) {
+                    for (var t = [], r = 0, o = e.split(re).filter((function(e) {
                             return e.length > 0
                         })); r < o.length; r++) {
                         var i = o[r].split("/");
                         if (0 === i.length) throw new Error("Invalid number skeleton");
                         for (var n = i[0], a = i.slice(1), s = 0, l = a; s < l.length; s++)
                             if (0 === l[s].length) throw new Error("Invalid number skeleton");
                         t.push({
                             stem: n,
                             options: a
                         })
                     }
                     return t
                 }(e)
             } catch (o) {
-                return this.error($.INVALID_NUMBER_SKELETON, t)
+                return this.error(M.INVALID_NUMBER_SKELETON, t)
             }
             return {
                 val: {
-                    type: I.number,
+                    type: U.number,
                     tokens: r,
                     location: t,
-                    parsedOptions: this.shouldParseSkeletons ? le(r) : {}
+                    parsedOptions: this.shouldParseSkeletons ? de(r) : {}
                 },
                 err: null
             }
         }, e.prototype.tryParsePluralOrSelectOptions = function(e, t, r, o) {
             for (var i, n = !1, a = [], s = new Set, l = o.value, c = o.location;;) {
                 if (0 === l.length) {
                     var h = this.clonePosition();
                     if ("select" === t || !this.bumpIf("=")) break;
-                    var d = this.tryParseDecimalInteger($.EXPECT_PLURAL_ARGUMENT_SELECTOR, $.INVALID_PLURAL_ARGUMENT_SELECTOR);
+                    var d = this.tryParseDecimalInteger(M.EXPECT_PLURAL_ARGUMENT_SELECTOR, M.INVALID_PLURAL_ARGUMENT_SELECTOR);
                     if (d.err) return d;
-                    c = fe(h, this.clonePosition()), l = this.message.slice(h.offset, this.offset())
+                    c = ge(h, this.clonePosition()), l = this.message.slice(h.offset, this.offset())
                 }
-                if (s.has(l)) return this.error("select" === t ? $.DUPLICATE_SELECT_ARGUMENT_SELECTOR : $.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, c);
+                if (s.has(l)) return this.error("select" === t ? M.DUPLICATE_SELECT_ARGUMENT_SELECTOR : M.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, c);
                 "other" === l && (n = !0), this.bumpSpace();
                 var u = this.clonePosition();
-                if (!this.bumpIf("{")) return this.error("select" === t ? $.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : $.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, fe(this.clonePosition(), this.clonePosition()));
+                if (!this.bumpIf("{")) return this.error("select" === t ? M.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : M.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, ge(this.clonePosition(), this.clonePosition()));
                 var p = this.parseMessage(e + 1, t, r);
                 if (p.err) return p;
                 var f = this.tryParseArgumentClose(u);
                 if (f.err) return f;
                 a.push([l, {
                     value: p.val,
-                    location: fe(u, this.clonePosition())
+                    location: ge(u, this.clonePosition())
                 }]), s.add(l), this.bumpSpace(), l = (i = this.parseIdentifierIfPossible()).value, c = i.location
             }
-            return 0 === a.length ? this.error("select" === t ? $.EXPECT_SELECT_ARGUMENT_SELECTOR : $.EXPECT_PLURAL_ARGUMENT_SELECTOR, fe(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !n ? this.error($.MISSING_OTHER_CLAUSE, fe(this.clonePosition(), this.clonePosition())) : {
+            return 0 === a.length ? this.error("select" === t ? M.EXPECT_SELECT_ARGUMENT_SELECTOR : M.EXPECT_PLURAL_ARGUMENT_SELECTOR, ge(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !n ? this.error(M.MISSING_OTHER_CLAUSE, ge(this.clonePosition(), this.clonePosition())) : {
                 val: a,
                 err: null
             }
         }, e.prototype.tryParseDecimalInteger = function(e, t) {
             var r = 1,
                 o = this.clonePosition();
             this.bumpIf("+") || this.bumpIf("-") && (r = -1);
             for (var i = !1, n = 0; !this.isEOF();) {
                 var a = this.char();
                 if (!(a >= 48 && a <= 57)) break;
                 i = !0, n = 10 * n + (a - 48), this.bump()
             }
-            var s = fe(o, this.clonePosition());
-            return i ? _e(n *= r) ? {
+            var s = ge(o, this.clonePosition());
+            return i ? ke(n *= r) ? {
                 val: n,
                 err: null
             } : this.error(t, s) : this.error(e, s)
         }, e.prototype.offset = function() {
             return this.position.offset
         }, e.prototype.isEOF = function() {
             return this.offset() === this.message.length
@@ -3675,15 +3763,15 @@
                 offset: this.position.offset,
                 line: this.position.line,
                 column: this.position.column
             }
         }, e.prototype.char = function() {
             var e = this.position.offset;
             if (e >= this.message.length) throw Error("out of bound");
-            var t = He(this.message, e);
+            var t = xe(this.message, e);
             if (void 0 === t) throw Error("Offset ".concat(e, " is at invalid UTF-16 code unit boundary"));
             return t
         }, e.prototype.error = function(e, t) {
             return {
                 val: null,
                 err: {
                     kind: e,
@@ -3693,15 +3781,15 @@
             }
         }, e.prototype.bump = function() {
             if (!this.isEOF()) {
                 var e = this.char();
                 10 === e ? (this.position.line += 1, this.position.column = 1, this.position.offset += 1) : (this.position.column += 1, this.position.offset += e < 65536 ? 1 : 2)
             }
         }, e.prototype.bumpIf = function(e) {
-            if (Se(this.message, e, this.offset())) {
+            if (He(this.message, e, this.offset())) {
                 for (var t = 0; t < e.length; t++) this.bump();
                 return !0
             }
             return !1
         }, e.prototype.bumpUntil = function(e) {
             var t = this.offset(),
                 r = this.message.indexOf(e, t);
@@ -3711,325 +3799,325 @@
             for (e = Math.min(e, this.message.length);;) {
                 var t = this.offset();
                 if (t === e) break;
                 if (t > e) throw Error("targetOffset ".concat(e, " is at invalid UTF-16 code unit boundary"));
                 if (this.bump(), this.isEOF()) break
             }
         }, e.prototype.bumpSpace = function() {
-            for (; !this.isEOF() && Ne(this.char());) this.bump()
+            for (; !this.isEOF() && Oe(this.char());) this.bump()
         }, e.prototype.peek = function() {
             if (this.isEOF()) return null;
             var e = this.char(),
                 t = this.offset(),
                 r = this.message.charCodeAt(t + (e >= 65536 ? 2 : 1));
             return null != r ? r : null
         }, e
     }();
 
-    function Le(e) {
+    function Ie(e) {
         return e >= 97 && e <= 122 || e >= 65 && e <= 90
     }
 
-    function Ne(e) {
+    function Oe(e) {
         return e >= 9 && e <= 13 || 32 === e || 133 === e || e >= 8206 && e <= 8207 || 8232 === e || 8233 === e
     }
 
-    function $e(e) {
+    function Me(e) {
         return e >= 33 && e <= 35 || 36 === e || e >= 37 && e <= 39 || 40 === e || 41 === e || 42 === e || 43 === e || 44 === e || 45 === e || e >= 46 && e <= 47 || e >= 58 && e <= 59 || e >= 60 && e <= 62 || e >= 63 && e <= 64 || 91 === e || 92 === e || 93 === e || 94 === e || 96 === e || 123 === e || 124 === e || 125 === e || 126 === e || 161 === e || e >= 162 && e <= 165 || 166 === e || 167 === e || 169 === e || 171 === e || 172 === e || 174 === e || 176 === e || 177 === e || 182 === e || 187 === e || 191 === e || 215 === e || 247 === e || e >= 8208 && e <= 8213 || e >= 8214 && e <= 8215 || 8216 === e || 8217 === e || 8218 === e || e >= 8219 && e <= 8220 || 8221 === e || 8222 === e || 8223 === e || e >= 8224 && e <= 8231 || e >= 8240 && e <= 8248 || 8249 === e || 8250 === e || e >= 8251 && e <= 8254 || e >= 8257 && e <= 8259 || 8260 === e || 8261 === e || 8262 === e || e >= 8263 && e <= 8273 || 8274 === e || 8275 === e || e >= 8277 && e <= 8286 || e >= 8592 && e <= 8596 || e >= 8597 && e <= 8601 || e >= 8602 && e <= 8603 || e >= 8604 && e <= 8607 || 8608 === e || e >= 8609 && e <= 8610 || 8611 === e || e >= 8612 && e <= 8613 || 8614 === e || e >= 8615 && e <= 8621 || 8622 === e || e >= 8623 && e <= 8653 || e >= 8654 && e <= 8655 || e >= 8656 && e <= 8657 || 8658 === e || 8659 === e || 8660 === e || e >= 8661 && e <= 8691 || e >= 8692 && e <= 8959 || e >= 8960 && e <= 8967 || 8968 === e || 8969 === e || 8970 === e || 8971 === e || e >= 8972 && e <= 8991 || e >= 8992 && e <= 8993 || e >= 8994 && e <= 9e3 || 9001 === e || 9002 === e || e >= 9003 && e <= 9083 || 9084 === e || e >= 9085 && e <= 9114 || e >= 9115 && e <= 9139 || e >= 9140 && e <= 9179 || e >= 9180 && e <= 9185 || e >= 9186 && e <= 9254 || e >= 9255 && e <= 9279 || e >= 9280 && e <= 9290 || e >= 9291 && e <= 9311 || e >= 9472 && e <= 9654 || 9655 === e || e >= 9656 && e <= 9664 || 9665 === e || e >= 9666 && e <= 9719 || e >= 9720 && e <= 9727 || e >= 9728 && e <= 9838 || 9839 === e || e >= 9840 && e <= 10087 || 10088 === e || 10089 === e || 10090 === e || 10091 === e || 10092 === e || 10093 === e || 10094 === e || 10095 === e || 10096 === e || 10097 === e || 10098 === e || 10099 === e || 10100 === e || 10101 === e || e >= 10132 && e <= 10175 || e >= 10176 && e <= 10180 || 10181 === e || 10182 === e || e >= 10183 && e <= 10213 || 10214 === e || 10215 === e || 10216 === e || 10217 === e || 10218 === e || 10219 === e || 10220 === e || 10221 === e || 10222 === e || 10223 === e || e >= 10224 && e <= 10239 || e >= 10240 && e <= 10495 || e >= 10496 && e <= 10626 || 10627 === e || 10628 === e || 10629 === e || 10630 === e || 10631 === e || 10632 === e || 10633 === e || 10634 === e || 10635 === e || 10636 === e || 10637 === e || 10638 === e || 10639 === e || 10640 === e || 10641 === e || 10642 === e || 10643 === e || 10644 === e || 10645 === e || 10646 === e || 10647 === e || 10648 === e || e >= 10649 && e <= 10711 || 10712 === e || 10713 === e || 10714 === e || 10715 === e || e >= 10716 && e <= 10747 || 10748 === e || 10749 === e || e >= 10750 && e <= 11007 || e >= 11008 && e <= 11055 || e >= 11056 && e <= 11076 || e >= 11077 && e <= 11078 || e >= 11079 && e <= 11084 || e >= 11085 && e <= 11123 || e >= 11124 && e <= 11125 || e >= 11126 && e <= 11157 || 11158 === e || e >= 11159 && e <= 11263 || e >= 11776 && e <= 11777 || 11778 === e || 11779 === e || 11780 === e || 11781 === e || e >= 11782 && e <= 11784 || 11785 === e || 11786 === e || 11787 === e || 11788 === e || 11789 === e || e >= 11790 && e <= 11798 || 11799 === e || e >= 11800 && e <= 11801 || 11802 === e || 11803 === e || 11804 === e || 11805 === e || e >= 11806 && e <= 11807 || 11808 === e || 11809 === e || 11810 === e || 11811 === e || 11812 === e || 11813 === e || 11814 === e || 11815 === e || 11816 === e || 11817 === e || e >= 11818 && e <= 11822 || 11823 === e || e >= 11824 && e <= 11833 || e >= 11834 && e <= 11835 || e >= 11836 && e <= 11839 || 11840 === e || 11841 === e || 11842 === e || e >= 11843 && e <= 11855 || e >= 11856 && e <= 11857 || 11858 === e || e >= 11859 && e <= 11903 || e >= 12289 && e <= 12291 || 12296 === e || 12297 === e || 12298 === e || 12299 === e || 12300 === e || 12301 === e || 12302 === e || 12303 === e || 12304 === e || 12305 === e || e >= 12306 && e <= 12307 || 12308 === e || 12309 === e || 12310 === e || 12311 === e || 12312 === e || 12313 === e || 12314 === e || 12315 === e || 12316 === e || 12317 === e || e >= 12318 && e <= 12319 || 12320 === e || 12336 === e || 64830 === e || 64831 === e || e >= 65093 && e <= 65094
     }
 
-    function Oe(e) {
+    function De(e) {
         e.forEach((function(e) {
-            if (delete e.location, z(e) || V(e))
-                for (var t in e.options) delete e.options[t].location, Oe(e.options[t].value);
-            else G(e) && X(e.style) || (F(e) || j(e)) && W(e.style) ? delete e.style.location : K(e) && Oe(e.children)
+            if (delete e.location, Z(e) || W(e))
+                for (var t in e.options) delete e.options[t].location, De(e.options[t].value);
+            else z(e) && q(e.style) || (V(e) || K(e)) && J(e.style) ? delete e.style.location : Y(e) && De(e.children)
         }))
     }
 
-    function Ie(e, t) {
-        void 0 === t && (t = {}), t = (0, M.pi)({
+    function Ue(e, t) {
+        void 0 === t && (t = {}), t = (0, G.pi)({
             shouldParseSkeletons: !0,
             requiresOtherClause: !0
         }, t);
-        var r = new Re(e, t).parse();
+        var r = new $e(e, t).parse();
         if (r.err) {
-            var o = SyntaxError($[r.err.kind]);
+            var o = SyntaxError(M[r.err.kind]);
             throw o.location = r.err.location, o.originalMessage = r.err.message, o
         }
-        return (null == t ? void 0 : t.captureLocation) || Oe(r.val), r.val
+        return (null == t ? void 0 : t.captureLocation) || De(r.val), r.val
     }
 
-    function Me(e, t) {
-        var r = t && t.cache ? t.cache : Ze,
-            o = t && t.serializer ? t.serializer : je;
-        return (t && t.strategy ? t.strategy : Fe)(e, {
+    function Ge(e, t) {
+        var r = t && t.cache ? t.cache : Xe,
+            o = t && t.serializer ? t.serializer : Ke;
+        return (t && t.strategy ? t.strategy : Ve)(e, {
             cache: r,
             serializer: o
         })
     }
 
-    function Ue(e, t, r, o) {
+    function Fe(e, t, r, o) {
         var i, n = null == (i = o) || "number" == typeof i || "boolean" == typeof i ? o : r(o),
             a = t.get(n);
         return void 0 === a && (a = e.call(this, o), t.set(n, a)), a
     }
 
-    function De(e, t, r) {
+    function je(e, t, r) {
         var o = Array.prototype.slice.call(arguments, 3),
             i = r(o),
             n = t.get(i);
         return void 0 === n && (n = e.apply(this, o), t.set(i, n)), n
     }
 
-    function Ge(e, t, r, o, i) {
+    function ze(e, t, r, o, i) {
         return r.bind(t, e, o, i)
     }
 
-    function Fe(e, t) {
-        return Ge(e, this, 1 === e.length ? Ue : De, t.cache.create(), t.serializer)
+    function Ve(e, t) {
+        return ze(e, this, 1 === e.length ? Fe : je, t.cache.create(), t.serializer)
     }
-    var je = function() {
+    var Ke = function() {
         return JSON.stringify(arguments)
     };
 
-    function ze() {
+    function Ze() {
         this.cache = Object.create(null)
     }
-    ze.prototype.get = function(e) {
+    Ze.prototype.get = function(e) {
         return this.cache[e]
-    }, ze.prototype.set = function(e, t) {
+    }, Ze.prototype.set = function(e, t) {
         this.cache[e] = t
     };
-    var Ve, Ze = {
+    var We, Xe = {
             create: function() {
-                return new ze
+                return new Ze
             }
         },
-        Ke = {
+        Ye = {
             variadic: function(e, t) {
-                return Ge(e, this, De, t.cache.create(), t.serializer)
+                return ze(e, this, je, t.cache.create(), t.serializer)
             },
             monadic: function(e, t) {
-                return Ge(e, this, Ue, t.cache.create(), t.serializer)
+                return ze(e, this, Fe, t.cache.create(), t.serializer)
             }
         };
     ! function(e) {
         e.MISSING_VALUE = "MISSING_VALUE", e.INVALID_VALUE = "INVALID_VALUE", e.MISSING_INTL_API = "MISSING_INTL_API"
-    }(Ve || (Ve = {}));
-    var Xe, We = function(e) {
+    }(We || (We = {}));
+    var qe, Je = function(e) {
             function t(t, r, o) {
                 var i = e.call(this, t) || this;
                 return i.code = r, i.originalMessage = o, i
             }
-            return (0, M.ZT)(t, e), t.prototype.toString = function() {
+            return (0, G.ZT)(t, e), t.prototype.toString = function() {
                 return "[formatjs Error: ".concat(this.code, "] ").concat(this.message)
             }, t
         }(Error),
-        Ye = function(e) {
+        Qe = function(e) {
             function t(t, r, o, i) {
-                return e.call(this, 'Invalid values for "'.concat(t, '": "').concat(r, '". Options are "').concat(Object.keys(o).join('", "'), '"'), Ve.INVALID_VALUE, i) || this
+                return e.call(this, 'Invalid values for "'.concat(t, '": "').concat(r, '". Options are "').concat(Object.keys(o).join('", "'), '"'), We.INVALID_VALUE, i) || this
             }
-            return (0, M.ZT)(t, e), t
-        }(We),
-        qe = function(e) {
+            return (0, G.ZT)(t, e), t
+        }(Je),
+        et = function(e) {
             function t(t, r, o) {
-                return e.call(this, 'Value for "'.concat(t, '" must be of type ').concat(r), Ve.INVALID_VALUE, o) || this
+                return e.call(this, 'Value for "'.concat(t, '" must be of type ').concat(r), We.INVALID_VALUE, o) || this
             }
-            return (0, M.ZT)(t, e), t
-        }(We),
-        Je = function(e) {
+            return (0, G.ZT)(t, e), t
+        }(Je),
+        tt = function(e) {
             function t(t, r) {
-                return e.call(this, 'The intl string context variable "'.concat(t, '" was not provided to the string "').concat(r, '"'), Ve.MISSING_VALUE, r) || this
+                return e.call(this, 'The intl string context variable "'.concat(t, '" was not provided to the string "').concat(r, '"'), We.MISSING_VALUE, r) || this
             }
-            return (0, M.ZT)(t, e), t
-        }(We);
+            return (0, G.ZT)(t, e), t
+        }(Je);
 
-    function Qe(e) {
+    function rt(e) {
         return "function" == typeof e
     }
 
-    function et(e, t, r, o, i, n, a) {
-        if (1 === e.length && U(e[0])) return [{
-            type: Xe.literal,
+    function ot(e, t, r, o, i, n, a) {
+        if (1 === e.length && F(e[0])) return [{
+            type: qe.literal,
             value: e[0].value
         }];
         for (var s = [], l = 0, c = e; l < c.length; l++) {
             var h = c[l];
-            if (U(h)) s.push({
-                type: Xe.literal,
+            if (F(h)) s.push({
+                type: qe.literal,
                 value: h.value
             });
-            else if (Z(h)) "number" == typeof n && s.push({
-                type: Xe.literal,
+            else if (X(h)) "number" == typeof n && s.push({
+                type: qe.literal,
                 value: r.getNumberFormat(t).format(n)
             });
             else {
                 var d = h.value;
-                if (!i || !(d in i)) throw new Je(d, a);
+                if (!i || !(d in i)) throw new tt(d, a);
                 var u = i[d];
-                if (D(h)) u && "string" != typeof u && "number" != typeof u || (u = "string" == typeof u || "number" == typeof u ? String(u) : ""), s.push({
-                    type: "string" == typeof u ? Xe.literal : Xe.object,
+                if (j(h)) u && "string" != typeof u && "number" != typeof u || (u = "string" == typeof u || "number" == typeof u ? String(u) : ""), s.push({
+                    type: "string" == typeof u ? qe.literal : qe.object,
                     value: u
                 });
-                else if (F(h)) {
-                    var p = "string" == typeof h.style ? o.date[h.style] : W(h.style) ? h.style.parsedOptions : void 0;
+                else if (V(h)) {
+                    var p = "string" == typeof h.style ? o.date[h.style] : J(h.style) ? h.style.parsedOptions : void 0;
                     s.push({
-                        type: Xe.literal,
+                        type: qe.literal,
                         value: r.getDateTimeFormat(t, p).format(u)
                     })
-                } else if (j(h)) {
-                    p = "string" == typeof h.style ? o.time[h.style] : W(h.style) ? h.style.parsedOptions : o.time.medium;
+                } else if (K(h)) {
+                    p = "string" == typeof h.style ? o.time[h.style] : J(h.style) ? h.style.parsedOptions : o.time.medium;
                     s.push({
-                        type: Xe.literal,
+                        type: qe.literal,
                         value: r.getDateTimeFormat(t, p).format(u)
                     })
-                } else if (G(h)) {
-                    (p = "string" == typeof h.style ? o.number[h.style] : X(h.style) ? h.style.parsedOptions : void 0) && p.scale && (u *= p.scale || 1), s.push({
-                        type: Xe.literal,
+                } else if (z(h)) {
+                    (p = "string" == typeof h.style ? o.number[h.style] : q(h.style) ? h.style.parsedOptions : void 0) && p.scale && (u *= p.scale || 1), s.push({
+                        type: qe.literal,
                         value: r.getNumberFormat(t, p).format(u)
                     })
                 } else {
-                    if (K(h)) {
+                    if (Y(h)) {
                         var f = h.children,
                             m = h.value,
                             b = i[m];
-                        if (!Qe(b)) throw new qe(m, "function", a);
-                        var g = b(et(f, t, r, o, i, n).map((function(e) {
+                        if (!rt(b)) throw new et(m, "function", a);
+                        var g = b(ot(f, t, r, o, i, n).map((function(e) {
                             return e.value
                         })));
                         Array.isArray(g) || (g = [g]), s.push.apply(s, g.map((function(e) {
                             return {
-                                type: "string" == typeof e ? Xe.literal : Xe.object,
+                                type: "string" == typeof e ? qe.literal : qe.object,
                                 value: e
                             }
                         })))
                     }
-                    if (z(h)) {
-                        if (!(v = h.options[u] || h.options.other)) throw new Ye(h.value, u, Object.keys(h.options), a);
-                        s.push.apply(s, et(v.value, t, r, o, i))
-                    } else if (V(h)) {
+                    if (Z(h)) {
+                        if (!(v = h.options[u] || h.options.other)) throw new Qe(h.value, u, Object.keys(h.options), a);
+                        s.push.apply(s, ot(v.value, t, r, o, i))
+                    } else if (W(h)) {
                         var v;
                         if (!(v = h.options["=".concat(u)])) {
-                            if (!Intl.PluralRules) throw new We('Intl.PluralRules is not available in this environment.\nTry polyfilling it using "@formatjs/intl-pluralrules"\n', Ve.MISSING_INTL_API, a);
+                            if (!Intl.PluralRules) throw new Je('Intl.PluralRules is not available in this environment.\nTry polyfilling it using "@formatjs/intl-pluralrules"\n', We.MISSING_INTL_API, a);
                             var y = r.getPluralRules(t, {
                                 type: h.pluralType
                             }).select(u - (h.offset || 0));
                             v = h.options[y] || h.options.other
                         }
-                        if (!v) throw new Ye(h.value, u, Object.keys(h.options), a);
-                        s.push.apply(s, et(v.value, t, r, o, i, u - (h.offset || 0)))
+                        if (!v) throw new Qe(h.value, u, Object.keys(h.options), a);
+                        s.push.apply(s, ot(v.value, t, r, o, i, u - (h.offset || 0)))
                     } else;
                 }
             }
         }
         return function(e) {
             return e.length < 2 ? e : e.reduce((function(e, t) {
                 var r = e[e.length - 1];
-                return r && r.type === Xe.literal && t.type === Xe.literal ? r.value += t.value : e.push(t), e
+                return r && r.type === qe.literal && t.type === qe.literal ? r.value += t.value : e.push(t), e
             }), [])
         }(s)
     }
 
-    function tt(e, t) {
+    function it(e, t) {
         return t ? Object.keys(e).reduce((function(r, o) {
             var i, n;
-            return r[o] = (i = e[o], (n = t[o]) ? (0, M.pi)((0, M.pi)((0, M.pi)({}, i || {}), n || {}), Object.keys(i).reduce((function(e, t) {
-                return e[t] = (0, M.pi)((0, M.pi)({}, i[t]), n[t] || {}), e
+            return r[o] = (i = e[o], (n = t[o]) ? (0, G.pi)((0, G.pi)((0, G.pi)({}, i || {}), n || {}), Object.keys(i).reduce((function(e, t) {
+                return e[t] = (0, G.pi)((0, G.pi)({}, i[t]), n[t] || {}), e
             }), {})) : i), r
-        }), (0, M.pi)({}, e)) : e
+        }), (0, G.pi)({}, e)) : e
     }
 
-    function rt(e) {
+    function nt(e) {
         return {
             create: function() {
                 return {
                     get: function(t) {
                         return e[t]
                     },
                     set: function(t, r) {
                         e[t] = r
                     }
                 }
             }
         }
     }! function(e) {
         e[e.literal = 0] = "literal", e[e.object = 1] = "object"
-    }(Xe || (Xe = {}));
-    var ot = function() {
+    }(qe || (qe = {}));
+    var at = function() {
         function e(t, r, o, i) {
             var n, a = this;
             if (void 0 === r && (r = e.defaultLocale), this.formatterCache = {
                     number: {},
                     dateTime: {},
                     pluralRules: {}
                 }, this.format = function(e) {
                     var t = a.formatToParts(e);
                     if (1 === t.length) return t[0].value;
                     var r = t.reduce((function(e, t) {
-                        return e.length && t.type === Xe.literal && "string" == typeof e[e.length - 1] ? e[e.length - 1] += t.value : e.push(t.value), e
+                        return e.length && t.type === qe.literal && "string" == typeof e[e.length - 1] ? e[e.length - 1] += t.value : e.push(t.value), e
                     }), []);
                     return r.length <= 1 ? r[0] || "" : r
                 }, this.formatToParts = function(e) {
-                    return et(a.ast, a.locales, a.formatters, a.formats, e, void 0, a.message)
+                    return ot(a.ast, a.locales, a.formatters, a.formats, e, void 0, a.message)
                 }, this.resolvedOptions = function() {
                     var e;
                     return {
                         locale: (null === (e = a.resolvedLocale) || void 0 === e ? void 0 : e.toString()) || Intl.NumberFormat.supportedLocalesOf(a.locales)[0]
                     }
                 }, this.getAst = function() {
                     return a.ast
                 }, this.locales = r, this.resolvedLocale = e.resolveLocale(r), "string" == typeof t) {
                 if (this.message = t, !e.__parse) throw new TypeError("IntlMessageFormat.__parse must be set to process `message` of type `string`");
                 var s = i || {},
-                    l = (s.formatters, (0, M._T)(s, ["formatters"]));
-                this.ast = e.__parse(t, (0, M.pi)((0, M.pi)({}, l), {
+                    l = (s.formatters, (0, G._T)(s, ["formatters"]));
+                this.ast = e.__parse(t, (0, G.pi)((0, G.pi)({}, l), {
                     locale: this.resolvedLocale
                 }))
             } else this.ast = t;
             if (!Array.isArray(this.ast)) throw new TypeError("A message must be provided as a String or AST.");
-            this.formats = tt(e.formats, o), this.formatters = i && i.formatters || (void 0 === (n = this.formatterCache) && (n = {
+            this.formats = it(e.formats, o), this.formatters = i && i.formatters || (void 0 === (n = this.formatterCache) && (n = {
                 number: {},
                 dateTime: {},
                 pluralRules: {}
             }), {
-                getNumberFormat: Me((function() {
+                getNumberFormat: Ge((function() {
                     for (var e, t = [], r = 0; r < arguments.length; r++) t[r] = arguments[r];
-                    return new((e = Intl.NumberFormat).bind.apply(e, (0, M.ev)([void 0], t, !1)))
+                    return new((e = Intl.NumberFormat).bind.apply(e, (0, G.ev)([void 0], t, !1)))
                 }), {
-                    cache: rt(n.number),
-                    strategy: Ke.variadic
+                    cache: nt(n.number),
+                    strategy: Ye.variadic
                 }),
-                getDateTimeFormat: Me((function() {
+                getDateTimeFormat: Ge((function() {
                     for (var e, t = [], r = 0; r < arguments.length; r++) t[r] = arguments[r];
-                    return new((e = Intl.DateTimeFormat).bind.apply(e, (0, M.ev)([void 0], t, !1)))
+                    return new((e = Intl.DateTimeFormat).bind.apply(e, (0, G.ev)([void 0], t, !1)))
                 }), {
-                    cache: rt(n.dateTime),
-                    strategy: Ke.variadic
+                    cache: nt(n.dateTime),
+                    strategy: Ye.variadic
                 }),
-                getPluralRules: Me((function() {
+                getPluralRules: Ge((function() {
                     for (var e, t = [], r = 0; r < arguments.length; r++) t[r] = arguments[r];
-                    return new((e = Intl.PluralRules).bind.apply(e, (0, M.ev)([void 0], t, !1)))
+                    return new((e = Intl.PluralRules).bind.apply(e, (0, G.ev)([void 0], t, !1)))
                 }), {
-                    cache: rt(n.pluralRules),
-                    strategy: Ke.variadic
+                    cache: nt(n.pluralRules),
+                    strategy: Ye.variadic
                 })
             })
         }
         return Object.defineProperty(e, "defaultLocale", {
             get: function() {
                 return e.memoizedDefaultLocale || (e.memoizedDefaultLocale = (new Intl.NumberFormat).resolvedOptions().locale), e.memoizedDefaultLocale
             },
             enumerable: !1,
             configurable: !0
         }), e.memoizedDefaultLocale = null, e.resolveLocale = function(e) {
             if (void 0 !== Intl.Locale) {
                 var t = Intl.NumberFormat.supportedLocalesOf(e);
                 return t.length > 0 ? new Intl.Locale(t[0]) : new Intl.Locale("string" == typeof e ? e : e[0])
             }
-        }, e.__parse = Ie, e.formats = {
+        }, e.__parse = Ue, e.formats = {
             number: {
                 integer: {
                     maximumFractionDigits: 0
                 },
                 currency: {
                     style: "currency"
                 },
@@ -4081,28 +4169,29 @@
                     minute: "numeric",
                     second: "numeric",
                     timeZoneName: "short"
                 }
             }
         }, e
     }();
-    const it = ot,
-        nt = JSON.parse('{"title":"LCN","group":"Gruppe","module":"Modul","segment":"Segment","id":"ID","module-id":"Modul ID","segment-id":"Segment ID","name":"Name","entity-id":"Entitäts-ID","type":"Typ","resource":"Ressource","create":"Erstellen","dismiss":"Abbrechen","domain":"Domäne","binary-sensor":"Binärsensor","climate":"Klima","cover":"Abdeckung","light":"Licht","scene":"Szene","sensor":"Sensor","switch":"Schalter","variable":"Variable","variables":"Variablen","setpoint":"Sollwert","setpoints":"Sollwerte","motor":"Motor","reverse-delay":"Umkehrverzögerung","output":"Ausgang","outputs":"Ausgänge","relay":"Relais","relays":"Relais","port":"Anschluss","port-type":"Anschlusstyp","register":"Register","threshold":"Schwellwert","thresholds":"Schwellwerte","s0input":"S0 Eingang","s0inputs":"S0 Eingänge","led":"Led","leds":"Leds","logics":"Logiken","source":"Quelle","source-type":"Quellentyp","unit-lcn-native":"LCN nativ","unit-humidity":"Luftfeuchtigkeit","unit-wind":"Wind","unit-volts":"Volt","unit-milliamperes":"Milliampere","unit-angle":"Winkel","binary-sensor-type-binsensors":"Binärsensoren","binary-sensor-type-setpoint-locks":"Sperrung Sollwerte","binary-sensor-type-keys-locks":"Sperrung Tasten","dashboard-devices-title":"LCN Konfiguration","dashboard-devices-introduction":"Willkommen auf dem LCN Konfigurations-Dashboard.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Module scannen","dashboard-devices-for-host":"Module/Gruppen für Host","dashboard-devices-add":"Modul/Gruppe erstellen","dashboard-dialog-scan-devices-title":"Suche nach Modulen...","dashboard-dialog-scan-devices-text":"Das Suchen nach Modulen kann bis zu 30 Sekunden dauern. Dieses Fenster schließt sich automatisch.","dashboard-devices-dialog-add-alert-title":"Modul oder Gruppe existiert bereits","dashboard-devices-dialog-add-alert-text":"Das Modul oder die Gruppe existiert bereits:","dashboard-devices-dialog-add-alert-hint":"Module und Gruppen dürfen nur einmal angegeben werden.","dashboard-devices-dialog-request-info-title":"Fordere Eigenschaften vom LCN Modul an","dashboard-devices-dialog-request-info-text":"Die Eigenschaften für das angegebene Modul werden angefordert. Dies kann einige Sekunden dauern.","dashboard-devices-dialog-request-info-hint":"Dieses Fenster schließt sich automatisch.","dashboard-devices-table-delete":"Lösche Eintrag","dashboard-devices-table-no-data":"Keine Geräte konfiguriert.","dashboard-devices-dialog-delete-module-title":"Modul löschen","dashboard-devices-dialog-delete-group-title":"Gruppe löschen","dashboard-devices-dialog-delete-text":"Du möchtest folgendes Gerät löschen:","dashboard-devices-dialog-delete-warning":"Mit dem Löschen des Gerätes werden alle zugehörigen Entitäten gelöscht!","dashboard-devices-dialog-create-title":"Modul / Gruppe erstellen","dashboard-devices-dialog-error-segment":"Segment ID muss im Bereich 0, 5..128 liegen.","dashboard-devices-dialog-error-module":"Modul ID muss im Bereich 5..254 liegen.","dashboard-devices-dialog-error-group":"Gruppen ID muss im Bereich 5..254 liegen.","dashboard-entities-title":"Konfiguration Entitäten","dashboard-entities-introduction":"Konfiguration der Entitäten für dieses Modul / Gruppe.","dashboard-entities-add":"Entität erstellen","dashboard-entities-dialog-add-alert-title":"LCN Ressource existiert bereits","dashboard-entities-dialog-add-alert-text":"Die angegebene LCN Ressource ist der Entität bereits zugewiesen.","dashboard-entities-dialog-add-alert-hint":"LCN Ressourcen dürfen für jede Domäne nur einmal existieren.","dashboard-entities-table-delete":"Lösche Eintrag","dashboard-entities-table-no-data":"Keine Entitäten konfiguriert.","dashboard-entities-dialog-create-title":"Entität erstellen","dashboard-entities-dialog-unit-of-measurement":"Messeinheit","dashboard-entities-dialog-climate-lockable":"Sperrbar","dashboard-entities-dialog-climate-min-temperature":"Minimale Temperatur","dashboard-entities-dialog-climate-max-temperature":"Maximale Temperatur","dashboard-entities-dialog-climate-min-temperature-error":"Ungültige minimale Temperatur","dashboard-entities-dialog-climate-max-temperature-error":"Ungültige maximale Temperatur","dashboard-entities-dialog-light-dimmable":"Dimmbar","dashboard-entities-dialog-light-transition":"Rampe","dashboard-entities-dialog-light-transition-error":"Rampe muss im Bereich 0..486 liegen.","dashboard-entities-dialog-scene-transition":"Rampe","dashboard-entities-dialog-scene-transition-error":"Rampe muss im Bereich 0..486 liegen."}');
-    var at = i.t(nt, 2);
-    const st = JSON.parse('{"title":"LCN","group":"Group","module":"Module","segment":"Segment","id":"ID","module-id":"Module ID","segment-id":"Segment ID","name":"Name","entity-id":"Entity ID","type":"Type","resource":"Resource","create":"Create","dismiss":"Dismiss","domain":"Domain","binary-sensor":"Binary sensor","climate":"Climate","cover":"Cover","light":"Light","scene":"Scene","sensor":"Sensor","switch":"Switch","variable":"Variable","variables":"Variables","setpoint":"Setpoint","setpoints":"Setpoints","motor":"Motor","reverse-delay":"Reverse delay","output":"Output","outputs":"Outputs","relay":"Relay","relays":"Realys","port":"Port","port-type":"Port type","register":"Register","threshold":"Threshold","thresholds":"Thresholds","s0input":"S0 Input","s0inputs":"S0 Inputs","led":"Led","leds":"Leds","logic":"Logic","logics":"Logics","source":"Source","source-type":"Source type","unit-lcn-native":"LCN native","unit-humidity":"Humidity","unit-wind":"Wind","unit-volts":"Volts","unit-milliamperes":"Milliamperes","unit-angle":"Angle","binary-sensor-type-binsensors":"Binary sensors","binary-sensor-type-setpoint-locks":"Lock state setpoints","binary-sensor-type-keys-locks":"Lock state keys","dashboard-devices-title":"LCN Configuration Dashboard","dashboard-devices-introduction":"Welcome to the LCN configuration dashboard.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Scan modules","dashboard-devices-for-host":"Modules/groups for host","dashboard-devices-add":"Create module/group","dashboard-dialog-scan-devices-title":"Scanning for modules...","dashboard-dialog-scan-devices-text":"Scanning for modules might take up to 30 seconds. This dialog will close automatically.","dashboard-devices-dialog-add-alert-title":"Module or group already exists","dashboard-devices-dialog-add-alert-text":"The specified module or group already exists:","dashboard-devices-dialog-add-alert-hint":"Modules and groups have to be unique.","dashboard-devices-dialog-request-info-title":"Requesting device info from LCN","dashboard-devices-dialog-request-info-text":"The information for the specified device is beeing requested from LCN. This might take several seconds.","dashboard-devices-dialog-request-info-hint":"This dialog will close automatically.","dashboard-devices-table-delete":"Delete entry","dashboard-devices-table-no-data":"No devices configured.","dashboard-devices-dialog-delete-module-title":"Delete module","dashboard-devices-dialog-delete-group-title":"Delete group","dashboard-devices-dialog-delete-text":"You are about to delete:","dashboard-devices-dialog-delete-warning":"Removing a device will also delete all associated entities!","dashboard-devices-dialog-create-title":"Create module / group","dashboard-devices-dialog-error-segment":"Segment ID must be 0, 5..128.","dashboard-devices-dialog-error-module":"Module ID must be 5..254.","dashboard-devices-dialog-error-group":"Group ID must be 5..254.","dashboard-entities-title":"Entities configuration","dashboard-entities-introduction":"Configure entities for this module / group.","dashboard-entities-add":"Create entity","dashboard-entities-dialog-add-alert-title":"LCN resource already assigned","dashboard-entities-dialog-add-alert-text":"The specified LCN resource is already assigned to this entity.","dashboard-entities-dialog-add-alert-hint":"LCN resources may only be assigned once within a domain.","dashboard-entities-table-delete":"Delete entry","dashboard-entities-table-no-data":"No entities configured.","dashboard-entities-dialog-create-title":"Create entity","dashboard-entities-dialog-unit-of-measurement":"Unit of measurement","dashboard-entities-dialog-climate-lockable":"Lockable","dashboard-entities-dialog-climate-min-temperature":"Minimum temperature","dashboard-entities-dialog-climate-max-temperature":"Maximum temperature","dashboard-entities-dialog-climate-min-temperature-error":"Invalid minimum temperature","dashboard-entities-dialog-climate-max-temperature-error":"Invalid maximum temperature","dashboard-entities-dialog-light-dimmable":"Dimmable","dashboard-entities-dialog-light-transition":"Transition","dashboard-entities-dialog-light-transition-error":"Transition must be in 0..486.","dashboard-entities-dialog-scene-transition":"Transition","dashboard-entities-dialog-scene-transition-error":"Transition must be in 0..486."}');
-    const lt = {
-            de: at,
-            en: i.t(st, 2)
+    const st = at,
+        lt = JSON.parse('{"title":"LCN","group":"Gruppe","module":"Modul","segment":"Segment","id":"ID","module-id":"Modul ID","segment-id":"Segment ID","name":"Name","entity-id":"Entitäts-ID","type":"Typ","resource":"Ressource","create":"Erstellen","dismiss":"Abbrechen","domain":"Domäne","binary-sensor":"Binärsensor","climate":"Klima","cover":"Abdeckung","light":"Licht","scene":"Szene","sensor":"Sensor","switch":"Schalter","variable":"Variable","variables":"Variablen","setpoint":"Sollwert","setpoints":"Sollwerte","motor":"Motor","reverse-delay":"Umkehrverzögerung","output":"Ausgang","outputs":"Ausgänge","relay":"Relais","relays":"Relais","port":"Anschluss","port-type":"Anschlusstyp","register":"Register","threshold":"Schwellwert","thresholds":"Schwellwerte","s0input":"S0 Eingang","s0inputs":"S0 Eingänge","led":"Led","leds":"Leds","logics":"Logiken","source":"Quelle","source-type":"Quellentyp","unit-lcn-native":"LCN nativ","unit-humidity":"Luftfeuchtigkeit","unit-wind":"Wind","unit-volts":"Volt","unit-milliamperes":"Milliampere","unit-angle":"Winkel","binary-sensor-type-binsensors":"Binärsensoren","binary-sensor-type-setpoint-locks":"Sperrung Sollwerte","binary-sensor-type-keys-locks":"Sperrung Tasten","more-help":"mehr Hilfe...","dashboard-devices-title":"LCN Konfiguration","dashboard-devices-introduction":"Willkommen auf dem LCN Konfigurations-Dashboard!","dashboard-devices-introduction-help-1":"Hier kannst du die Module und Gruppen deines LCN Systems konfigurieren.","dashboard-devices-introduction-help-2":"Um zu beginnen, selektiere deinen Host und starte eine automatische Suche nach LCN Modulen. Die gefundenen Module werden in der Liste angezeigt.","dashboard-devices-introduction-help-3":"Wird ein Modul nicht automatisch erkannt, kannst du das Modul auch manuell hinzufügen.","dashboard-devices-introduction-help-4":"Klicke auf einen Eintrag in der Liste, um die zugehörigen Entitäten anzuzeigen und zu editieren.","dashboard-devices-introduction-help-5":"Wenn du einen Eintrag löschen möchtest, klicke auf das Mülleimersymbol neben dem Eintrag.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Module scannen","dashboard-devices-for-host":"Module/Gruppen für Host","dashboard-devices-add":"Modul/Gruppe erstellen","dashboard-dialog-scan-devices-title":"Suche nach Modulen...","dashboard-dialog-scan-devices-text":"Das Suchen nach Modulen kann bis zu 30 Sekunden dauern. Dieses Fenster schließt sich automatisch.","dashboard-devices-dialog-add-alert-title":"Modul oder Gruppe existiert bereits","dashboard-devices-dialog-add-alert-text":"Das Modul oder die Gruppe existiert bereits:","dashboard-devices-dialog-add-alert-hint":"Module und Gruppen dürfen nur einmal angegeben werden.","dashboard-devices-dialog-request-info-title":"Fordere Eigenschaften vom LCN Modul an","dashboard-devices-dialog-request-info-text":"Die Eigenschaften für das angegebene Modul werden angefordert. Dies kann einige Sekunden dauern.","dashboard-devices-dialog-request-info-hint":"Dieses Fenster schließt sich automatisch.","dashboard-devices-table-delete":"Lösche Eintrag","dashboard-devices-table-no-data":"Keine Geräte konfiguriert.","dashboard-devices-dialog-delete-module-title":"Modul löschen","dashboard-devices-dialog-delete-group-title":"Gruppe löschen","dashboard-devices-dialog-delete-text":"Du möchtest folgendes Gerät löschen:","dashboard-devices-dialog-delete-warning":"Mit dem Löschen des Gerätes werden alle zugehörigen Entitäten gelöscht!","dashboard-devices-dialog-create-title":"Modul / Gruppe erstellen","dashboard-devices-dialog-error-segment":"Segment ID muss im Bereich 0, 5..128 liegen.","dashboard-devices-dialog-error-module":"Modul ID muss im Bereich 5..254 liegen.","dashboard-devices-dialog-error-group":"Gruppen ID muss im Bereich 5..254 liegen.","dashboard-entities-title":"LCN Entitäten","dashboard-entities-introduction":"Konfiguriere die Entitäten für dieses Modul / diese Gruppe.","dashboard-entities-introduction-help-1":"Füge neue Entitäten, die dieses Modul/Gruppe bereitstellt zu deiner Konfiguration hinzu.","dashboard-entities-introduction-help-2":"Klicke auf \\"Entität erstellen\\", wähle die Domäne aus und konfiguriere die Parameter entsprechend deiner LCN Installation.","dashboard-entities-introduction-help-3":"Du kannst die erstellten Entitäten nach Belieben in deinen Dashboards verwenden.","dashboard-entities-introduction-help-4":"Wenn du eine Entität löschen möchtest, klicke auf das Mülleimersymbol neben dem Eintrag.","dashboard-entities-introduction-help-5":"Möchtest du die Parameter einer Entität ändern, musst du sie zunächst löschen und danach neu erstellen.","dashboard-entities-entities-for-module":"Entities für Modul","dashboard-entities-entities-for-group":"Entities für Gruppe","dashboard-entities-add":"Entität erstellen","dashboard-entities-dialog-add-alert-title":"LCN Ressource existiert bereits","dashboard-entities-dialog-add-alert-text":"Die angegebene LCN Ressource ist der Entität bereits zugewiesen.","dashboard-entities-dialog-add-alert-hint":"LCN Ressourcen dürfen für jede Domäne nur einmal existieren.","dashboard-entities-table-delete":"Lösche Eintrag","dashboard-entities-table-no-data":"Keine Entitäten konfiguriert.","dashboard-entities-dialog-create-title":"Entität erstellen","dashboard-entities-dialog-unit-of-measurement":"Messeinheit","dashboard-entities-dialog-climate-lockable":"Sperrbar","dashboard-entities-dialog-climate-min-temperature":"Minimale Temperatur","dashboard-entities-dialog-climate-max-temperature":"Maximale Temperatur","dashboard-entities-dialog-climate-min-temperature-error":"Ungültige minimale Temperatur","dashboard-entities-dialog-climate-max-temperature-error":"Ungültige maximale Temperatur","dashboard-entities-dialog-light-dimmable":"Dimmbar","dashboard-entities-dialog-light-transition":"Rampe","dashboard-entities-dialog-light-transition-error":"Rampe muss im Bereich 0..486 liegen.","dashboard-entities-dialog-scene-transition":"Rampe","dashboard-entities-dialog-scene-transition-error":"Rampe muss im Bereich 0..486 liegen."}');
+    var ct = i.t(lt, 2);
+    const ht = JSON.parse('{"title":"LCN","group":"Group","module":"Module","segment":"Segment","id":"ID","module-id":"Module ID","segment-id":"Segment ID","name":"Name","entity-id":"Entity ID","type":"Type","resource":"Resource","create":"Create","dismiss":"Dismiss","domain":"Domain","binary-sensor":"Binary sensor","climate":"Climate","cover":"Cover","light":"Light","scene":"Scene","sensor":"Sensor","switch":"Switch","variable":"Variable","variables":"Variables","setpoint":"Setpoint","setpoints":"Setpoints","motor":"Motor","reverse-delay":"Reverse delay","output":"Output","outputs":"Outputs","relay":"Relay","relays":"Realys","port":"Port","port-type":"Port type","register":"Register","threshold":"Threshold","thresholds":"Thresholds","s0input":"S0 Input","s0inputs":"S0 Inputs","led":"Led","leds":"Leds","logic":"Logic","logics":"Logics","source":"Source","source-type":"Source type","unit-lcn-native":"LCN native","unit-humidity":"Humidity","unit-wind":"Wind","unit-volts":"Volts","unit-milliamperes":"Milliamperes","unit-angle":"Angle","binary-sensor-type-binsensors":"Binary sensors","binary-sensor-type-setpoint-locks":"Lock state setpoints","binary-sensor-type-keys-locks":"Lock state keys","more-help":"more help...","dashboard-devices-title":"LCN Configuration Dashboard","dashboard-devices-introduction":"Welcome to the LCN configuration dashboard!","dashboard-devices-introduction-help-1":"Here you can configure the modules and groups of your LCN system.","dashboard-devices-introduction-help-2":"To get started, select your host and start an automatic search for LCN modules. The modules found are displayed in the list.","dashboard-devices-introduction-help-3":"If a module is not recognized automatically, you can add the module manually.","dashboard-devices-introduction-help-4":"Click on an entry in the list to display and edit the associated entities.","dashboard-devices-introduction-help-5":"If you want to delete an entry, click on the trash can icon next to the entry.","dashboard-devices-hosts":"Hosts","dashboard-devices-scan":"Scan modules","dashboard-devices-for-host":"Modules/groups for host","dashboard-devices-add":"Create module/group","dashboard-dialog-scan-devices-title":"Scanning for modules...","dashboard-dialog-scan-devices-text":"Scanning for modules might take up to 30 seconds. This dialog will close automatically.","dashboard-devices-dialog-add-alert-title":"Module or group already exists","dashboard-devices-dialog-add-alert-text":"The specified module or group already exists:","dashboard-devices-dialog-add-alert-hint":"Modules and groups have to be unique.","dashboard-devices-dialog-request-info-title":"Requesting device info from LCN","dashboard-devices-dialog-request-info-text":"The information for the specified device is beeing requested from LCN. This might take several seconds.","dashboard-devices-dialog-request-info-hint":"This dialog will close automatically.","dashboard-devices-table-delete":"Delete entry","dashboard-devices-table-no-data":"No devices configured.","dashboard-devices-dialog-delete-module-title":"Delete module","dashboard-devices-dialog-delete-group-title":"Delete group","dashboard-devices-dialog-delete-text":"You are about to delete:","dashboard-devices-dialog-delete-warning":"Removing a device will also delete all associated entities!","dashboard-devices-dialog-create-title":"Create module / group","dashboard-devices-dialog-error-segment":"Segment ID must be 0, 5..128.","dashboard-devices-dialog-error-module":"Module ID must be 5..254.","dashboard-devices-dialog-error-group":"Group ID must be 5..254.","dashboard-entities-title":"LCN Entities","dashboard-entities-introduction":"Configure the entities for this module / group.","dashboard-entities-introduction-help-1":"Add new entities provided by this module/group to your configuration.","dashboard-entities-introduction-help-2":"Click on \\"Create entity\\", select the domain and configure the parameters according to your LCN installation.","dashboard-entities-introduction-help-3":"You can use the created entities in your dashboards as you wish.","dashboard-entities-introduction-help-4":"If you want to delete an entity, click on the trash can icon next to the entry.","dashboard-entities-introduction-help-5":"To change the parameters of an entity, you must first delete it and then create a new one.","dashboard-entities-entities-for-module":"Entities for module","dashboard-entities-entities-for-group":"Entities for group","dashboard-entities-add":"Create entity","dashboard-entities-dialog-add-alert-title":"LCN resource already assigned","dashboard-entities-dialog-add-alert-text":"The specified LCN resource is already assigned to this entity.","dashboard-entities-dialog-add-alert-hint":"LCN resources may only be assigned once within a domain.","dashboard-entities-table-delete":"Delete entry","dashboard-entities-table-no-data":"No entities configured.","dashboard-entities-dialog-create-title":"Create entity","dashboard-entities-dialog-unit-of-measurement":"Unit of measurement","dashboard-entities-dialog-climate-lockable":"Lockable","dashboard-entities-dialog-climate-min-temperature":"Minimum temperature","dashboard-entities-dialog-climate-max-temperature":"Maximum temperature","dashboard-entities-dialog-climate-min-temperature-error":"Invalid minimum temperature","dashboard-entities-dialog-climate-max-temperature-error":"Invalid maximum temperature","dashboard-entities-dialog-light-dimmable":"Dimmable","dashboard-entities-dialog-light-transition":"Transition","dashboard-entities-dialog-light-transition-error":"Transition must be in 0..486.","dashboard-entities-dialog-scene-transition":"Transition","dashboard-entities-dialog-scene-transition-error":"Transition must be in 0..486."}');
+    const dt = {
+            de: ct,
+            en: i.t(ht, 2)
         },
-        ct = "en",
-        ht = {
+        ut = "en",
+        pt = new $("localize"),
+        ft = {
             language: [],
             sting: {}
         },
-        dt = {};
+        mt = {};
     (0, r.Z)([(0, a.Mo)("lcn-frontend")], (function(t, r) {
         class i extends r {
             constructor(...e) {
                 super(...e), t(this)
             }
         }
         return {
@@ -4135,29 +4224,29 @@
                 })],
                 key: "route",
                 value: void 0
             }, {
                 kind: "method",
                 key: "firstUpdated",
                 value: function(e) {
-                    (0, o.Z)((0, n.Z)(i.prototype), "firstUpdated", this).call(this, e), this.hass && (this.lcn || this._initLCN(), this.addEventListener("lcn-location-changed", (e => this._setRoute(e))), (0, B.lD)(this, this.shadowRoot), "" !== this.route.path && "/" !== this.route.path || (0, C.c)("/lcn/devices", {
+                    (0, o.Z)((0, n.Z)(i.prototype), "firstUpdated", this).call(this, e), this.hass && (this.lcn || this._initLCN(), this.addEventListener("lcn-location-changed", (e => this._setRoute(e))), (0, x.lD)(this, this.shadowRoot), "" !== this.route.path && "/" !== this.route.path || (0, P.c)("/lcn/devices", {
                         replace: !0
                     }), ((e, t) => {
                         const r = matchMedia(e),
                             o = e => t(e.matches);
                         r.addListener(o), t(r.matches)
                     })("(prefers-color-scheme: dark)", (e => {
                         this._applyTheme()
                     })))
                 }
             }, {
                 kind: "method",
                 key: "render",
                 value: function() {
-                    return this.hass ? e.dy`
+                    return this.hass && this.lcn ? e.dy`
       <lcn-router
         .hass=${this.hass}
         .lcn=${this.lcn}
         .route=${this.route}
         .narrow=${this.narrow}
       ></lcn-router>
     ` : e.Ld
@@ -4177,49 +4266,50 @@
                     }).then((e => {
                         const t = e.find((e => null === e.disabled_by));
                         void 0 !== t && (this.lcn = {
                             language: this.hass.language,
                             config_entries: e,
                             localize: (e, t) => function(e, t, r) {
                                 var o;
-                                let i = (e || localStorage.getItem("selectedLanguage") || ct).replace(/['"]+/g, "").replace("-", "_");
+                                let i = (e || localStorage.getItem("selectedLanguage") || ut).replace(/['"]+/g, "").replace("-", "_");
                                 var n;
-                                lt[i] || (null !== (n = ht.language) && void 0 !== n && n.includes(i) || ht.language.push(i), i = ct);
-                                const a = (null === (o = lt[i]) || void 0 === o ? void 0 : o[t]) || lt[ct][t];
-                                if (!a) return console.error(`Translation problem with '${t}' for '${i}'`), "";
+                                dt[i] || (null !== (n = ft.language) && void 0 !== n && n.includes(i) || ft.language.push(i), i = ut);
+                                const a = (null === (o = dt[i]) || void 0 === o ? void 0 : o[t]) || dt[ut][t];
+                                if (!a) return pt.error(`Translation problem with '${t}' for '${i}'`), "";
                                 const s = t + a;
-                                let l = dt[s];
+                                let l = mt[s];
                                 if (!l) {
                                     try {
-                                        l = new it(a, e)
+                                        l = new st(a, e)
                                     } catch (c) {
-                                        return console.warn(`Translation problem with '${t}' for '${i}'`), ""
+                                        return pt.warn(`Translation problem with '${t}' for '${i}'`), ""
                                     }
-                                    dt[s] = l
+                                    mt[s] = l
                                 }
                                 try {
                                     return l.format(r)
                                 } catch (c) {
-                                    return console.warn(`Translation problem with '${t}' for '${i}'`), ""
+                                    return pt.warn(`Translation problem with '${t}' for '${i}'`), ""
                                 }
                             }(this.hass.language || "en", e, t),
+                            log: new $,
                             host: {
                                 name: t.title,
                                 id: t.entry_id
                             },
                             address: [0, 0, !1]
                         })
                     }))
                 }
             }, {
                 kind: "method",
                 key: "_setRoute",
                 value: function(e) {
                     var t;
-                    null !== (t = e.detail) && void 0 !== t && t.route && (this.route = e.detail.route, (0, C.c)(this.route.path, {
+                    null !== (t = e.detail) && void 0 !== t && t.route && (this.route = e.detail.route, (0, P.c)(this.route.path, {
                         replace: !0
                     }), this.requestUpdate())
                 }
             }, {
                 kind: "method",
                 key: "_applyTheme",
                 value: function() {
@@ -4227,25 +4317,25 @@
                     H(this.parentElement, this.hass.themes, (null === (e = this.hass.selectedTheme) || void 0 === e ? void 0 : e.theme) || (this.hass.themes.darkMode && this.hass.themes.default_dark_theme ? this.hass.themes.default_dark_theme : this.hass.themes.default_theme), {
                         ...this.hass.selectedTheme,
                         dark: this.hass.themes.darkMode
                     }), this.parentElement.style.backgroundColor = "var(--primary-background-color)", this.parentElement.style.color = "var(--primary-text-color)"
                 }
             }]
         }
-    }), (ut = e.oi, class extends ut {
+    }), (bt = e.oi, class extends bt {
         constructor(...e) {
             super(...e), this.hass = void 0, this.__provideHass = []
         }
         provideHass(e) {
             this.__provideHass.push(e), e.hass = this.hass
         }
         updated(e) {
             super.updated(e), e.has("hass") && this.__provideHass.forEach((e => {
                 e.hass = this.hass
             }))
         }
     }));
-    var ut;
-    const pt = document.createElement("style");
-    pt.innerHTML = "\nbody {\n  font-family: Roboto, sans-serif;\n  -moz-osx-font-smoothing: grayscale;\n  -webkit-font-smoothing: antialiased;\n  font-weight: 400;\n  margin: 0;\n  padding: 0;\n  height: 100vh;\n}\n@media (prefers-color-scheme: dark) {\n  body {\n    background-color: #111111;\n    color: #e1e1e1;\n  }\n}\n", document.head.appendChild(pt)
+    var bt;
+    const gt = document.createElement("style");
+    gt.innerHTML = "\nbody {\n  font-family: Roboto, sans-serif;\n  -moz-osx-font-smoothing: grayscale;\n  -webkit-font-smoothing: antialiased;\n  font-weight: 400;\n  margin: 0;\n  padding: 0;\n  height: 100vh;\n}\n@media (prefers-color-scheme: dark) {\n  body {\n    background-color: #111111;\n    color: #e1e1e1;\n  }\n}\n", document.head.appendChild(gt)
 })();
-//# sourceMappingURL=entrypoint-UP5lFvdJ.js.map
+//# sourceMappingURL=entrypoint-Wn7tXtT_.js.map
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8214285714285714%*

 * *Differences: {"'file'": "'entrypoint-Wn7tXtT_.js'",*

 * * "'mappings'": "';;;;;;;AAQA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;AAKA;;;;;;;;;;;;;;;;;;;;AC/FA;;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;; […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "file": "entrypoint-UP5lFvdJ.js",
-    "mappings": ";;;;;;;AAQA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;AAKA;;;;;;;;;;;;;;;;;;;;AC/FA;;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAgZA;;AAMA;;AChYA;AACA;AACA;AACA;;AAPA",
+    "file": "entrypoint-Wn7tXtT_.js",
+    "mappings": ";;;;;;;AAQA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;;;;;;AAUA;;;;;AAKA;;;;;;;;;;;;;;;;;;;;AC/FA;;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAgZA;;AAMA;;AC/XA;AACA;AACA;AACA;;AAPA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://lcn-frontend/./homeassistant-frontend/src/resources/roboto.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/resources/ha-style.ts",
         "webpack://lcn-frontend/./src/main.ts"
     ],
     "sourcesContent": [
         "import { css, unsafeCSS } from \"lit\";\n\nexport const fontStyles = css`\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Thin\"),\n      local(\"Roboto-Thin\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-Thin.woff2)\n        format(\"woff2\");\n    font-weight: 100;\n    font-style: normal;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Thin Italic\"),\n      local(\"Roboto-ThinItalic\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-ThinItalic.woff2)\n        format(\"woff2\");\n    font-weight: 100;\n    font-style: italic;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Light\"),\n      local(\"Roboto-Light\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-Light.woff2)\n        format(\"woff2\");\n    font-weight: 300;\n    font-style: normal;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Light Italic\"),\n      local(\"Roboto-LightItalic\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-LightItalic.woff2)\n        format(\"woff2\");\n    font-weight: 300;\n    font-style: italic;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Regular\"),\n      local(\"Roboto-Regular\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-Regular.woff2)\n        format(\"woff2\");\n    font-weight: 400;\n    font-style: normal;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Italic\"),\n      local(\"Roboto-Italic\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-RegularItalic.woff2)\n        format(\"woff2\");\n    font-weight: 400;\n    font-style: italic;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Medium\"),\n      local(\"Roboto-Medium\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-Medium.woff2)\n        format(\"woff2\");\n    font-weight: 500;\n    font-style: normal;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Medium Italic\"),\n      local(\"Roboto-MediumItalic\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-MediumItalic.woff2)\n        format(\"woff2\");\n    font-weight: 500;\n    font-style: italic;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Bold\"),\n      local(\"Roboto-Bold\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-Bold.woff2)\n        format(\"woff2\");\n    font-weight: 700;\n    font-style: normal;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Bold Italic\"),\n      local(\"Roboto-BoldItalic\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-BoldItalic.woff2)\n        format(\"woff2\");\n    font-weight: 700;\n    font-style: italic;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Black\"),\n      local(\"Roboto-Black\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-Black.woff2)\n        format(\"woff2\");\n    font-weight: 900;\n    font-style: normal;\n  }\n  @font-face {\n    font-family: \"Roboto\";\n    src:\n      local(\"Roboto Black Italic\"),\n      local(\"Roboto-BlackItalic\"),\n      url(${unsafeCSS(__STATIC_PATH__)}fonts/roboto/Roboto-BlackItalic.woff2)\n        format(\"woff2\");\n    font-weight: 900;\n    font-style: italic;\n  }\n`.toString();\n",
         "import { css, unsafeCSS } from \"lit\";\nimport { fontStyles } from \"./roboto\";\nimport {\n  DEFAULT_ACCENT_COLOR,\n  DEFAULT_PRIMARY_COLOR,\n  derivedStyles,\n} from \"./styles-data\";\n\nconst mainStyles = css`\n  /*\n    Home Assistant default styles.\n\n    In Polymer 2.0, default styles should to be set on the html selector.\n    (Setting all default styles only on body breaks shadyCSS polyfill.)\n    See: https://github.com/home-assistant/home-assistant-polymer/pull/901\n  */\n  html {\n    font-size: 14px;\n    height: 100vh;\n\n    /* text */\n    --primary-text-color: #212121;\n    --secondary-text-color: #727272;\n    --text-primary-color: #ffffff;\n    --text-light-primary-color: #212121;\n    --disabled-text-color: #bdbdbd;\n\n    /* main interface colors */\n    --primary-color: ${unsafeCSS(DEFAULT_PRIMARY_COLOR)};\n    --dark-primary-color: #0288d1;\n    --light-primary-color: #b3e5fc;\n    --accent-color: ${unsafeCSS(DEFAULT_ACCENT_COLOR)};\n    --divider-color: rgba(0, 0, 0, 0.12);\n    --outline-color: rgba(0, 0, 0, 0.12);\n\n    --scrollbar-thumb-color: rgb(194, 194, 194);\n\n    --error-color: #db4437;\n    --warning-color: #ffa600;\n    --success-color: #43a047;\n    --info-color: #039be5;\n\n    /* backgrounds */\n    --card-background-color: #ffffff;\n    --primary-background-color: #fafafa;\n    --secondary-background-color: #e5e5e5; /* behind the cards on state */\n    --clear-background-color: #ffffff;\n\n    /* for header */\n    --header-height: 56px;\n\n    /* for label-badge */\n    --label-badge-red: var(--error-color);\n    --label-badge-blue: var(--info-color);\n    --label-badge-green: var(--success-color);\n    --label-badge-yellow: var(--warning-color);\n    --label-badge-grey: #9e9e9e;\n\n    /* states icon */\n    --state-icon-color: #44739e;\n    /* an error state is anything that would be considered an error */\n    /* --state-icon-error-color: #db4437; derived from error-color */\n\n    /* energy */\n    --energy-grid-consumption-color: #488fc2;\n    --energy-grid-return-color: #8353d1;\n    --energy-solar-color: #ff9800;\n    --energy-non-fossil-color: #0f9d58;\n    --energy-battery-out-color: #4db6ac;\n    --energy-battery-in-color: #f06292;\n    --energy-gas-color: #8e021b;\n    --energy-water-color: #00bcd4;\n\n    /* opacity for dark text on a light background */\n    --dark-divider-opacity: 0.12;\n    --dark-disabled-opacity: 0.38; /* or hint text or icon */\n    --dark-secondary-opacity: 0.54;\n    --dark-primary-opacity: 0.87;\n\n    /* opacity for light text on a dark background */\n    --light-divider-opacity: 0.12;\n    --light-disabled-opacity: 0.3; /* or hint text or icon */\n    --light-secondary-opacity: 0.7;\n    --light-primary-opacity: 1;\n\n    /* rgb */\n    --rgb-primary-color: 3, 169, 244;\n    --rgb-accent-color: 255, 152, 0;\n    --rgb-primary-text-color: 33, 33, 33;\n    --rgb-secondary-text-color: 114, 114, 114;\n    --rgb-text-primary-color: 255, 255, 255;\n    --rgb-card-background-color: 255, 255, 255;\n\n    /* color */\n    --disabled-color: #bdbdbd;\n    --red-color: #f44336;\n    --pink-color: #e91e63;\n    --purple-color: #926bc7;\n    --deep-purple-color: #6e41ab;\n    --indigo-color: #3f51b5;\n    --blue-color: #2196f3;\n    --light-blue-color: #03a9f4;\n    --cyan-color: #00bcd4;\n    --teal-color: #009688;\n    --green-color: #4caf50;\n    --light-green-color: #8bc34a;\n    --lime-color: #cddc39;\n    --yellow-color: #ffeb3b;\n    --amber-color: #ffc107;\n    --orange-color: #ff9800;\n    --deep-orange-color: #ff6f22;\n    --brown-color: #795548;\n    --light-grey-color: #bdbdbd;\n    --grey-color: #9e9e9e;\n    --dark-grey-color: #606060;\n    --blue-grey-color: #607d8b;\n    --black-color: #000000;\n    --white-color: #ffffff;\n\n    /* state color */\n    --state-active-color: var(--amber-color);\n    --state-inactive-color: var(--grey-color);\n    --state-unavailable-color: var(--disabled-color);\n\n    /* state domain colors */\n    --state-alarm_control_panel-armed_away-color: var(--green-color);\n    --state-alarm_control_panel-armed_custom_bypass-color: var(--green-color);\n    --state-alarm_control_panel-armed_home-color: var(--green-color);\n    --state-alarm_control_panel-armed_night-color: var(--green-color);\n    --state-alarm_control_panel-armed_vacation-color: var(--green-color);\n    --state-alarm_control_panel-arming-color: var(--orange-color);\n    --state-alarm_control_panel-disarming-color: var(--orange-color);\n    --state-alarm_control_panel-pending-color: var(--orange-color);\n    --state-alarm_control_panel-triggered-color: var(--red-color);\n    --state-alert-off-color: var(--orange-color);\n    --state-alert-on-color: var(--red-color);\n    --state-binary_sensor-active-color: var(--amber-color);\n    --state-binary_sensor-battery-on-color: var(--red-color);\n    --state-binary_sensor-carbon_monoxide-on-color: var(--red-color);\n    --state-binary_sensor-gas-on-color: var(--red-color);\n    --state-binary_sensor-heat-on-color: var(--red-color);\n    --state-binary_sensor-lock-on-color: var(--red-color);\n    --state-binary_sensor-moisture-on-color: var(--red-color);\n    --state-binary_sensor-problem-on-color: var(--red-color);\n    --state-binary_sensor-safety-on-color: var(--red-color);\n    --state-binary_sensor-smoke-on-color: var(--red-color);\n    --state-binary_sensor-sound-on-color: var(--red-color);\n    --state-binary_sensor-tamper-on-color: var(--red-color);\n    --state-climate-auto-color: var(--green-color);\n    --state-climate-cool-color: var(--blue-color);\n    --state-climate-dry-color: var(--orange-color);\n    --state-climate-fan_only-color: var(--cyan-color);\n    --state-climate-heat-color: var(--deep-orange-color);\n    --state-climate-heat-cool-color: var(--amber-color);\n    --state-cover-active-color: var(--purple-color);\n    --state-device_tracker-active-color: var(--blue-color);\n    --state-device_tracker-home-color: var(--green-color);\n    --state-fan-active-color: var(--cyan-color);\n    --state-humidifier-on-color: var(--blue-color);\n    --state-lawn_mower-error-color: var(--red-color);\n    --state-lawn_mower-mowing-color: var(--teal-color);\n    --state-light-active-color: var(--amber-color);\n    --state-lock-jammed-color: var(--red-color);\n    --state-lock-locked-color: var(--green-color);\n    --state-lock-pending-color: var(--orange-color);\n    --state-lock-unlocked-color: var(--red-color);\n    --state-media_player-active-color: var(--light-blue-color);\n    --state-person-active-color: var(--blue-color);\n    --state-person-home-color: var(--green-color);\n    --state-plant-active-color: var(--red-color);\n    --state-siren-active-color: var(--red-color);\n    --state-sun-above_horizon-color: var(--amber-color);\n    --state-sun-below_horizon-color: var(--indigo-color);\n    --state-switch-active-color: var(--amber-color);\n    --state-update-active-color: var(--orange-color);\n    --state-vacuum-active-color: var(--teal-color);\n    --state-sensor-battery-high-color: var(--green-color);\n    --state-sensor-battery-low-color: var(--red-color);\n    --state-sensor-battery-medium-color: var(--orange-color);\n    --state-water_heater-eco-color: var(--green-color);\n    --state-water_heater-electric-color: var(--orange-color);\n    --state-water_heater-gas-color: var(--orange-color);\n    --state-water_heater-heat_pump-color: var(--orange-color);\n    --state-water_heater-high_demand-color: var(--deep-orange-color);\n    --state-water_heater-performance-color: var(--deep-orange-color);\n\n    /* history colors */\n    --history-unavailable-color: transparent;\n    --history-unknown-color: var(--dark-grey-color);\n\n    /* input components */\n    --input-idle-line-color: rgba(0, 0, 0, 0.42);\n    --input-hover-line-color: rgba(0, 0, 0, 0.87);\n    --input-disabled-line-color: rgba(0, 0, 0, 0.06);\n    --input-outlined-idle-border-color: rgba(0, 0, 0, 0.38);\n    --input-outlined-hover-border-color: rgba(0, 0, 0, 0.87);\n    --input-outlined-disabled-border-color: rgba(0, 0, 0, 0.06);\n    --input-fill-color: rgb(245, 245, 245);\n    --input-disabled-fill-color: rgb(250, 250, 250);\n    --input-ink-color: rgba(0, 0, 0, 0.87);\n    --input-label-ink-color: rgba(0, 0, 0, 0.6);\n    --input-disabled-ink-color: rgba(0, 0, 0, 0.37);\n    --input-dropdown-icon-color: rgba(0, 0, 0, 0.54);\n\n    /* Vaadin typography */\n    --material-h6-font-size: 1.25rem;\n    --material-small-font-size: 0.875rem;\n    --material-caption-font-size: 0.75rem;\n    --material-button-font-size: 0.875rem;\n\n    /* Paper shadow */\n    --shadow-transition: {\n      transition: box-shadow 0.28s cubic-bezier(0.4, 0, 0.2, 1);\n    };\n\n    --shadow-none: {\n      box-shadow: none;\n    };\n\n    /* from http://codepen.io/shyndman/pen/c5394ddf2e8b2a5c9185904b57421cdb */\n\n    --shadow-elevation-2dp: {\n      box-shadow:\n        0 2px 2px 0 rgba(0, 0, 0, 0.14),\n        0 1px 5px 0 rgba(0, 0, 0, 0.12),\n        0 3px 1px -2px rgba(0, 0, 0, 0.2);\n    };\n\n    --shadow-elevation-3dp: {\n      box-shadow:\n        0 3px 4px 0 rgba(0, 0, 0, 0.14),\n        0 1px 8px 0 rgba(0, 0, 0, 0.12),\n        0 3px 3px -2px rgba(0, 0, 0, 0.4);\n    };\n\n    --shadow-elevation-4dp: {\n      box-shadow:\n        0 4px 5px 0 rgba(0, 0, 0, 0.14),\n        0 1px 10px 0 rgba(0, 0, 0, 0.12),\n        0 2px 4px -1px rgba(0, 0, 0, 0.4);\n    };\n\n    --shadow-elevation-6dp: {\n      box-shadow:\n        0 6px 10px 0 rgba(0, 0, 0, 0.14),\n        0 1px 18px 0 rgba(0, 0, 0, 0.12),\n        0 3px 5px -1px rgba(0, 0, 0, 0.4);\n    };\n\n    --shadow-elevation-8dp: {\n      box-shadow:\n        0 8px 10px 1px rgba(0, 0, 0, 0.14),\n        0 3px 14px 2px rgba(0, 0, 0, 0.12),\n        0 5px 5px -3px rgba(0, 0, 0, 0.4);\n    };\n\n    --shadow-elevation-12dp: {\n      box-shadow:\n        0 12px 16px 1px rgba(0, 0, 0, 0.14),\n        0 4px 22px 3px rgba(0, 0, 0, 0.12),\n        0 6px 7px -4px rgba(0, 0, 0, 0.4);\n    };\n\n    --shadow-elevation-16dp: {\n      box-shadow:\n        0 16px 24px 2px rgba(0, 0, 0, 0.14),\n        0 6px 30px 5px rgba(0, 0, 0, 0.12),\n        0 8px 10px -5px rgba(0, 0, 0, 0.4);\n    };\n\n    --shadow-elevation-24dp: {\n      box-shadow:\n        0 24px 38px 3px rgba(0, 0, 0, 0.14),\n        0 9px 46px 8px rgba(0, 0, 0, 0.12),\n        0 11px 15px -7px rgba(0, 0, 0, 0.4);\n    };\n\n    /* Paper typography Styles */\n    --paper-font-common-base: {\n      font-family: \"Roboto\", \"Noto\", sans-serif;\n      -webkit-font-smoothing: antialiased;\n    };\n\n    --paper-font-common-code: {\n      font-family: \"Roboto Mono\", \"Consolas\", \"Menlo\", monospace;\n      -webkit-font-smoothing: antialiased;\n    };\n\n    --paper-font-common-expensive-kerning: {\n      text-rendering: optimizeLegibility;\n    };\n\n    --paper-font-common-nowrap: {\n      white-space: nowrap;\n      overflow: hidden;\n      text-overflow: ellipsis;\n    };\n\n    /* Material Font Styles */\n\n    --paper-font-display4: {\n      @apply --paper-font-common-base;\n      @apply --paper-font-common-nowrap;\n\n      font-size: 112px;\n      font-weight: 300;\n      letter-spacing: -0.044em;\n      line-height: 120px;\n    };\n\n    --paper-font-display3: {\n      @apply --paper-font-common-base;\n      @apply --paper-font-common-nowrap;\n\n      font-size: 56px;\n      font-weight: 400;\n      letter-spacing: -0.026em;\n      line-height: 60px;\n    };\n\n    --paper-font-display2: {\n      @apply --paper-font-common-base;\n\n      font-size: 45px;\n      font-weight: 400;\n      letter-spacing: -0.018em;\n      line-height: 48px;\n    };\n\n    --paper-font-display1: {\n      @apply --paper-font-common-base;\n\n      font-size: 34px;\n      font-weight: 400;\n      letter-spacing: -0.01em;\n      line-height: 40px;\n    };\n\n    --paper-font-headline: {\n      @apply --paper-font-common-base;\n\n      font-size: 24px;\n      font-weight: 400;\n      letter-spacing: -0.012em;\n      line-height: 32px;\n    };\n\n    --paper-font-title: {\n      @apply --paper-font-common-base;\n      @apply --paper-font-common-nowrap;\n\n      font-size: 20px;\n      font-weight: 500;\n      line-height: 28px;\n    };\n\n    --paper-font-subhead: {\n      @apply --paper-font-common-base;\n\n      font-size: 16px;\n      font-weight: 400;\n      line-height: 24px;\n    };\n\n    --paper-font-body2: {\n      @apply --paper-font-common-base;\n\n      font-size: 14px;\n      font-weight: 500;\n      line-height: 24px;\n    };\n\n    --paper-font-body1: {\n      @apply --paper-font-common-base;\n\n      font-size: 14px;\n      font-weight: 400;\n      line-height: 20px;\n    };\n\n    --paper-font-caption: {\n      @apply --paper-font-common-base;\n      @apply --paper-font-common-nowrap;\n\n      font-size: 12px;\n      font-weight: 400;\n      letter-spacing: 0.011em;\n      line-height: 20px;\n    };\n\n    --paper-font-menu: {\n      @apply --paper-font-common-base;\n      @apply --paper-font-common-nowrap;\n\n      font-size: 13px;\n      font-weight: 500;\n      line-height: 24px;\n    };\n\n    --paper-font-button: {\n      @apply --paper-font-common-base;\n      @apply --paper-font-common-nowrap;\n\n      font-size: 14px;\n      font-weight: 500;\n      letter-spacing: 0.018em;\n      line-height: 24px;\n      text-transform: uppercase;\n    };\n\n    --paper-font-code2: {\n      @apply --paper-font-common-code;\n\n      font-size: 14px;\n      font-weight: 700;\n      line-height: 20px;\n    };\n\n    --paper-font-code1: {\n      @apply --paper-font-common-code;\n\n      font-size: 14px;\n      font-weight: 500;\n      line-height: 20px;\n    };\n\n    direction: ltr;\n    --direction: ltr;\n    --float-start: left;\n    --float-end: right;\n\n    ${unsafeCSS(\n      Object.entries(derivedStyles)\n        .map(([key, value]) => `--${key}: ${value};`)\n        .join(\"\")\n    )}\n  }\n`.toString();\n\nconst styleElement = document.createElement(\"style\");\nstyleElement.textContent = [mainStyles, fontStyles].join(\"\");\ndocument.head.append(styleElement);\n",
-        "import { LitElement, html, nothing } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\n\nimport { applyThemesOnElement } from \"@ha/common/dom/apply_themes_on_element\";\nimport { listenMediaQuery } from \"@ha/common/dom/media_query\";\nimport { navigate } from \"@ha/common/navigate\";\nimport { makeDialogManager } from \"@ha/dialogs/make-dialog-manager\";\nimport \"@ha/resources/ha-style\";\nimport { getConfigEntries } from \"@ha/data/config_entries\";\nimport type { HomeAssistant, Route } from \"@ha/types\";\n\nimport \"./lcn-router\";\nimport { ProvideHassLitMixin } from \"@ha/mixins/provide-hass-lit-mixin\";\nimport { localize } from \"./localize/localize\";\nimport { LCN, LcnHost, LcnAddress } from \"./types/lcn\";\nimport { LocationChangedEvent } from \"./types/navigation\";\n\n@customElement(\"lcn-frontend\")\nclass LcnFrontend extends ProvideHassLitMixin(LitElement) {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public narrow!: boolean;\n\n  @property({ attribute: false }) public route!: Route;\n\n  protected firstUpdated(changedProps) {\n    super.firstUpdated(changedProps);\n    if (!this.hass) {\n      return;\n    }\n    if (!this.lcn) {\n      this._initLCN();\n    }\n    this.addEventListener(\"lcn-location-changed\", (e) => this._setRoute(e as LocationChangedEvent));\n\n    makeDialogManager(this, this.shadowRoot!);\n    if (this.route.path === \"\" || this.route.path === \"/\") {\n      navigate(\"/lcn/devices\", { replace: true });\n    }\n\n    listenMediaQuery(\"(prefers-color-scheme: dark)\", (_matches) => {\n      this._applyTheme();\n    });\n  }\n\n  protected render() {\n    if (!this.hass) {\n      return nothing;\n    }\n    return html`\n      <lcn-router\n        .hass=${this.hass}\n        .lcn=${this.lcn}\n        .route=${this.route}\n        .narrow=${this.narrow}\n      ></lcn-router>\n    `;\n  }\n\n  protected _initLCN() {\n    getConfigEntries(this.hass, { domain: \"lcn\" }).then((configEntries) => {\n      const configEntry = configEntries.find((el) => el.disabled_by === null);\n\n      if (configEntry === undefined) return;\n\n      this.lcn = {\n        language: this.hass.language,\n        config_entries: configEntries,\n        localize: (string, replace) => localize(this.hass.language || \"en\", string, replace),\n        host: <LcnHost>{\n          name: configEntry.title,\n          id: configEntry.entry_id,\n        },\n        address: <LcnAddress>[0, 0, false],\n      };\n    });\n  }\n\n  private _setRoute(ev: LocationChangedEvent): void {\n    if (!ev.detail?.route) {\n      return;\n    }\n    this.route = ev.detail.route;\n    navigate(this.route.path, { replace: true });\n    this.requestUpdate();\n  }\n\n  private _applyTheme() {\n    applyThemesOnElement(\n      this.parentElement,\n      this.hass.themes,\n      this.hass.selectedTheme?.theme ||\n        (this.hass.themes.darkMode && this.hass.themes.default_dark_theme\n          ? this.hass.themes.default_dark_theme!\n          : this.hass.themes.default_theme),\n      {\n        ...this.hass.selectedTheme,\n        dark: this.hass.themes.darkMode,\n      },\n    );\n    this.parentElement!.style.backgroundColor = \"var(--primary-background-color)\";\n    this.parentElement!.style.color = \"var(--primary-text-color)\";\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-frontend\": LcnFrontend;\n  }\n}\n"
+        "import { LitElement, html, nothing } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\n\nimport { applyThemesOnElement } from \"@ha/common/dom/apply_themes_on_element\";\nimport { listenMediaQuery } from \"@ha/common/dom/media_query\";\nimport { navigate } from \"@ha/common/navigate\";\nimport { makeDialogManager } from \"@ha/dialogs/make-dialog-manager\";\nimport \"@ha/resources/ha-style\";\nimport { getConfigEntries } from \"@ha/data/config_entries\";\nimport type { HomeAssistant, Route } from \"@ha/types\";\n\nimport \"./lcn-router\";\nimport { ProvideHassLitMixin } from \"@ha/mixins/provide-hass-lit-mixin\";\nimport { LCNLogger } from \"./lcn-logger\";\nimport { localize } from \"./localize/localize\";\nimport type { LCN, LcnHost, LcnAddress } from \"./types/lcn\";\nimport { LocationChangedEvent } from \"./types/navigation\";\n\n@customElement(\"lcn-frontend\")\nclass LcnFrontend extends ProvideHassLitMixin(LitElement) {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public narrow!: boolean;\n\n  @property({ attribute: false }) public route!: Route;\n\n  protected firstUpdated(changedProps) {\n    super.firstUpdated(changedProps);\n    if (!this.hass) {\n      return;\n    }\n    if (!this.lcn) {\n      this._initLCN();\n    }\n    this.addEventListener(\"lcn-location-changed\", (e) => this._setRoute(e as LocationChangedEvent));\n\n    makeDialogManager(this, this.shadowRoot!);\n    if (this.route.path === \"\" || this.route.path === \"/\") {\n      navigate(\"/lcn/devices\", { replace: true });\n    }\n\n    listenMediaQuery(\"(prefers-color-scheme: dark)\", (_matches) => {\n      this._applyTheme();\n    });\n  }\n\n  protected render() {\n    if (!this.hass || !this.lcn) {\n      return nothing;\n    }\n    return html`\n      <lcn-router\n        .hass=${this.hass}\n        .lcn=${this.lcn}\n        .route=${this.route}\n        .narrow=${this.narrow}\n      ></lcn-router>\n    `;\n  }\n\n  protected _initLCN() {\n    getConfigEntries(this.hass, { domain: \"lcn\" }).then((configEntries) => {\n      const configEntry = configEntries.find((el) => el.disabled_by === null);\n\n      if (configEntry === undefined) return;\n\n      this.lcn = {\n        language: this.hass.language,\n        config_entries: configEntries,\n        localize: (string, replace) => localize(this.hass.language || \"en\", string, replace),\n        log: new LCNLogger(),\n        host: <LcnHost>{\n          name: configEntry.title,\n          id: configEntry.entry_id,\n        },\n        address: <LcnAddress>[0, 0, false],\n      };\n    });\n  }\n\n  private _setRoute(ev: LocationChangedEvent): void {\n    if (!ev.detail?.route) {\n      return;\n    }\n    this.route = ev.detail.route;\n    navigate(this.route.path, { replace: true });\n    this.requestUpdate();\n  }\n\n  private _applyTheme() {\n    applyThemesOnElement(\n      this.parentElement,\n      this.hass.themes,\n      this.hass.selectedTheme?.theme ||\n        (this.hass.themes.darkMode && this.hass.themes.default_dark_theme\n          ? this.hass.themes.default_dark_theme!\n          : this.hass.themes.default_theme),\n      {\n        ...this.hass.selectedTheme,\n        dark: this.hass.themes.darkMode,\n      },\n    );\n    this.parentElement!.style.backgroundColor = \"var(--primary-background-color)\";\n    this.parentElement!.style.color = \"var(--primary-text-color)\";\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-frontend\": LcnFrontend;\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fP3U9roj.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fP3U9roj.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fP3U9roj.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fP3U9roj.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fP3U9roj.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fP3U9roj.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/fYLWqtat.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/fYLWqtat.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/hzhoTwCw.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/hzhoTwCw.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/hzhoTwCw.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/hzhoTwCw.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/hzhoTwCw.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/hzhoTwCw.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/mUrtGIle.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/mUrtGIle.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/mUrtGIle.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/mUrtGIle.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/mUrtGIle.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/mUrtGIle.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oUOHqENt.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9VkUPPxQ.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see oUOHqENt.js.LICENSE.txt */
+/*! For license information please see 9VkUPPxQ.js.LICENSE.txt */
 export const id = 244;
 export const ids = [244];
 export const modules = {
     9828: (e, t, i) => {
         i.d(t, {
             i: () => u
         });
@@ -373,14 +373,15 @@
                     decorators: [(0, c.SB)()],
                     key: "_addressId",
                     value() {
                         return 5
                     }
                 }, {
                     kind: "field",
+                    decorators: [(0, c.SB)()],
                     key: "_invalid",
                     value() {
                         return !1
                     }
                 }, {
                     kind: "method",
                     key: "showDialog",
@@ -393,15 +394,15 @@
                     value: function(e) {
                         (0, a.Z)((0, d.Z)(i.prototype), "firstUpdated", this).call(this, e), (0, p.z)()
                     }
                 }, {
                     kind: "method",
                     key: "willUpdate",
                     value: function(e) {
-                        (0, a.Z)((0, d.Z)(i.prototype), "willUpdate", this).call(this, e), this._invalid = !this._validateSegmentId(this._segmentId) || !this._validateAddressId(this._addressId, this._isGroup)
+                        e.has("_invalid") && (this._invalid = !this._validateSegmentId(this._segmentId) || !this._validateAddressId(this._addressId, this._isGroup))
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
                         return this._params ? r.dy`
       <ha-dialog
@@ -559,8 +560,8 @@
       `]
                     }
                 }]
             }
         }), r.oi)
     }
 };
-//# sourceMappingURL=oUOHqENt.js.map
+//# sourceMappingURL=9VkUPPxQ.js.map
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oUOHqENt.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9VkUPPxQ.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'file'": "'9VkUPPxQ.js'",*

 * * "'mappings'": "';;AAeA;;AAEA;AAhBA;;;;AAqBA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA+HA;;;;;;;;;;;;;ACtGA;;;;ACjCA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACoGA;;;;;ACrDA;AAIA;;AAEA;;AAEA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;AACA;;;;;AAKA;;AAEA;;;;AAIA;AACA;AACA;;;;AAIA;;AAEA;;;;AAIA;AACA;AACA;;;;;;AAQA;AACA;;;;;AAKA;AACA;AACA;;;;AAtEA;;;;;;;;;;;;;AAiJA'",*

 * * "'sourcesContent'": "{insert: [(4, 'import "*

 * *                     '"@polymer/ap […]*

```diff
@@ -1,21 +1,21 @@
 {
-    "file": "oUOHqENt.js",
-    "mappings": ";;AAeA;;AAEA;AAhBA;;;;AAqBA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA+HA;;;;;;;;;;;;;ACtGA;;;;ACjCA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACoGA;;;;;ACtDA;AAIA;;AAEA;;AAEA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;AACA;;;;;AAKA;;AAEA;;;;AAIA;AACA;AACA;;;;AAIA;;AAEA;;;;AAIA;AACA;AACA;;;;;;AAQA;AACA;;;;;AAKA;AACA;AACA;;;;AAtEA;;;;;;;;;;;;;AAiJA",
+    "file": "9VkUPPxQ.js",
+    "mappings": ";;AAeA;;AAEA;AAhBA;;;;AAqBA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA+HA;;;;;;;;;;;;;ACtGA;;;;ACjCA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACoGA;;;;;ACrDA;AAIA;;AAEA;;AAEA;;;;AAIA;AACA;;;;AAIA;;;;AAIA;AACA;;;;;AAKA;;AAEA;;;;AAIA;AACA;AACA;;;;AAIA;;AAEA;;;;AAIA;AACA;AACA;;;;;;AAQA;AACA;;;;;AAKA;AACA;AACA;;;;AAtEA;;;;;;;;;;;;;AAiJA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-dialog.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-formfield.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-radio.ts",
         "webpack://lcn-frontend/./node_modules/@polymer/app-layout/app-toolbar/app-toolbar.js",
         "webpack://lcn-frontend/./src/dialogs/lcn-create-device-dialog.ts"
     ],
     "sourcesContent": [
         "import { DialogBase } from \"@material/mwc-dialog/mwc-dialog-base\";\nimport { styles } from \"@material/mwc-dialog/mwc-dialog.css\";\nimport { mdiClose } from \"@mdi/js\";\nimport { css, html, TemplateResult } from \"lit\";\nimport { customElement } from \"lit/decorators\";\nimport { FOCUS_TARGET } from \"../dialogs/make-dialog-manager\";\nimport type { HomeAssistant } from \"../types\";\nimport \"./ha-icon-button\";\n\nconst SUPPRESS_DEFAULT_PRESS_SELECTOR = [\"button\", \"ha-list-item\"];\n\nexport const createCloseHeading = (\n  hass: HomeAssistant | undefined,\n  title: string | TemplateResult\n) => html`\n  <div class=\"header_title\">${title}</div>\n  <ha-icon-button\n    .label=${hass?.localize(\"ui.dialogs.generic.close\") ?? \"Close\"}\n    .path=${mdiClose}\n    dialogAction=\"close\"\n    class=\"header_button\"\n  ></ha-icon-button>\n`;\n\n@customElement(\"ha-dialog\")\nexport class HaDialog extends DialogBase {\n  protected readonly [FOCUS_TARGET];\n\n  public scrollToPos(x: number, y: number) {\n    this.contentElement?.scrollTo(x, y);\n  }\n\n  protected renderHeading() {\n    return html`<slot name=\"heading\"> ${super.renderHeading()} </slot>`;\n  }\n\n  protected firstUpdated(): void {\n    super.firstUpdated();\n    this.suppressDefaultPressSelector = [\n      this.suppressDefaultPressSelector,\n      SUPPRESS_DEFAULT_PRESS_SELECTOR,\n    ].join(\", \");\n    this._updateScrolledAttribute();\n    this.contentElement?.addEventListener(\"scroll\", this._onScroll, {\n      passive: true,\n    });\n  }\n\n  disconnectedCallback(): void {\n    super.disconnectedCallback();\n    this.contentElement.removeEventListener(\"scroll\", this._onScroll);\n  }\n\n  private _onScroll = () => {\n    this._updateScrolledAttribute();\n  };\n\n  private _updateScrolledAttribute() {\n    if (!this.contentElement) return;\n    this.toggleAttribute(\"scrolled\", this.contentElement.scrollTop !== 0);\n  }\n\n  static override styles = [\n    styles,\n    css`\n      :host([scrolled]) ::slotted(ha-dialog-header) {\n        border-bottom: 1px solid\n          var(--mdc-dialog-scroll-divider-color, rgba(0, 0, 0, 0.12));\n      }\n      .mdc-dialog {\n        --mdc-dialog-scroll-divider-color: var(\n          --dialog-scroll-divider-color,\n          var(--divider-color)\n        );\n        z-index: var(--dialog-z-index, 8);\n        -webkit-backdrop-filter: var(--dialog-backdrop-filter, none);\n        backdrop-filter: var(--dialog-backdrop-filter, none);\n        --mdc-dialog-box-shadow: var(--dialog-box-shadow, none);\n        --mdc-typography-headline6-font-weight: 400;\n        --mdc-typography-headline6-font-size: 1.574rem;\n      }\n      .mdc-dialog__actions {\n        justify-content: var(--justify-action-buttons, flex-end);\n        padding-bottom: max(env(safe-area-inset-bottom), 24px);\n      }\n      .mdc-dialog__actions span:nth-child(1) {\n        flex: var(--secondary-action-button-flex, unset);\n      }\n      .mdc-dialog__actions span:nth-child(2) {\n        flex: var(--primary-action-button-flex, unset);\n      }\n      .mdc-dialog__container {\n        align-items: var(--vertical-align-dialog, center);\n      }\n      .mdc-dialog__title {\n        padding: 24px 24px 0 24px;\n        text-overflow: ellipsis;\n        overflow: hidden;\n      }\n      .mdc-dialog__actions {\n        padding: 12px 24px 12px 24px;\n      }\n      .mdc-dialog__title::before {\n        display: block;\n        height: 0px;\n      }\n      .mdc-dialog .mdc-dialog__content {\n        position: var(--dialog-content-position, relative);\n        padding: var(--dialog-content-padding, 24px);\n      }\n      :host([hideactions]) .mdc-dialog .mdc-dialog__content {\n        padding-bottom: max(\n          var(--dialog-content-padding, 24px),\n          env(safe-area-inset-bottom)\n        );\n      }\n      .mdc-dialog .mdc-dialog__surface {\n        position: var(--dialog-surface-position, relative);\n        top: var(--dialog-surface-top);\n        margin-top: var(--dialog-surface-margin-top);\n        min-height: var(--mdc-dialog-min-height, auto);\n        border-radius: var(--ha-dialog-border-radius, 28px);\n      }\n      :host([flexContent]) .mdc-dialog .mdc-dialog__content {\n        display: flex;\n        flex-direction: column;\n      }\n      .header_title {\n        margin-right: 32px;\n        margin-inline-end: 32px;\n        margin-inline-start: initial;\n        direction: var(--direction);\n      }\n      .header_button {\n        position: absolute;\n        right: 16px;\n        top: 14px;\n        text-decoration: none;\n        color: inherit;\n        inset-inline-start: initial;\n        inset-inline-end: 16px;\n        direction: var(--direction);\n      }\n      .dialog-actions {\n        inset-inline-start: initial !important;\n        inset-inline-end: 0px !important;\n        direction: var(--direction);\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-dialog\": HaDialog;\n  }\n}\n",
         "import { FormfieldBase } from \"@material/mwc-formfield/mwc-formfield-base\";\nimport { styles } from \"@material/mwc-formfield/mwc-formfield.css\";\nimport { css } from \"lit\";\nimport { customElement } from \"lit/decorators\";\nimport { fireEvent } from \"../common/dom/fire_event\";\n\n@customElement(\"ha-formfield\")\nexport class HaFormfield extends FormfieldBase {\n  protected _labelClick() {\n    const input = this.input as HTMLInputElement | undefined;\n    if (!input) return;\n\n    input.focus();\n    if (input.disabled) {\n      return;\n    }\n    switch (input.tagName) {\n      case \"HA-CHECKBOX\":\n        input.checked = !input.checked;\n        fireEvent(input, \"change\");\n        break;\n      case \"HA-RADIO\":\n        input.checked = true;\n        fireEvent(input, \"change\");\n        break;\n      default:\n        input.click();\n        break;\n    }\n  }\n\n  static override styles = [\n    styles,\n    css`\n      :host(:not([alignEnd])) ::slotted(ha-switch) {\n        margin-right: 10px;\n        margin-inline-end: 10px;\n        margin-inline-start: inline;\n      }\n      .mdc-form-field > label {\n        direction: var(--direction);\n        margin-inline-start: 0;\n        margin-inline-end: auto;\n        padding-inline-start: 4px;\n        padding-inline-end: 0;\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-formfield\": HaFormfield;\n  }\n}\n",
         "import { RadioBase } from \"@material/mwc-radio/mwc-radio-base\";\nimport { styles } from \"@material/mwc-radio/mwc-radio.css\";\nimport { css } from \"lit\";\nimport { customElement } from \"lit/decorators\";\n\n@customElement(\"ha-radio\")\nexport class HaRadio extends RadioBase {\n  static override styles = [\n    styles,\n    css`\n      :host {\n        --mdc-theme-secondary: var(--primary-color);\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-radio\": HaRadio;\n  }\n}\n",
         "/**\n@license\nCopyright (c) 2015 The Polymer Project Authors. All rights reserved.\nThis code may only be used under the BSD style license found at\nhttp://polymer.github.io/LICENSE.txt The complete set of authors may be found at\nhttp://polymer.github.io/AUTHORS.txt The complete set of contributors may be\nfound at http://polymer.github.io/CONTRIBUTORS.txt Code distributed by Google as\npart of the polymer project is also subject to an additional IP rights grant\nfound at http://polymer.github.io/PATENTS.txt\n*/\nimport '@polymer/polymer/polymer-legacy.js';\n\nimport '@polymer/iron-flex-layout/iron-flex-layout.js';\nimport {Polymer} from '@polymer/polymer/lib/legacy/polymer-fn.js';\nimport {html} from '@polymer/polymer/lib/utils/html-tag.js';\n\n/**\napp-toolbar is a horizontal toolbar containing items that can be used for\nlabel, navigation, search and actions.\n\n### Example\n\nAdd a title to the toolbar.\n\n```html\n<app-toolbar>\n  <div main-title>App name</div>\n</app-toolbar>\n```\n\nAdd a button to the left and right side of the toolbar.\n\n```html\n<app-toolbar>\n  <paper-icon-button icon=\"menu\"></paper-icon-button>\n  <div main-title>App name</div>\n  <paper-icon-button icon=\"search\"></paper-icon-button>\n</app-toolbar>\n```\n\nYou can use the attributes `top-item` or `bottom-item` to completely fit an\nelement to the top or bottom of the toolbar respectively.\n\n### Content attributes\n\nAttribute            | Description\n---------------------|---------------------------------------------------------\n`main-title`         | The main title element.\n`condensed-title`    | The title element if used inside a condensed app-header.\n`spacer`             | Adds a left margin of `64px`.\n`bottom-item`        | Sticks the element to the bottom of the toolbar.\n`top-item`           | Sticks the element to the top of the toolbar.\n\n### Styling\n\nCustom property              | Description                  | Default\n-----------------------------|------------------------------|-----------------------\n`--app-toolbar-font-size`    | Toolbar font size            | 20px\n\n@element app-toolbar\n@demo app-toolbar/demo/index.html\n*/\nPolymer({\n  /** @override */\n  _template: html`\n    <style>\n\n      :host {\n        @apply --layout-horizontal;\n        @apply --layout-center;\n        position: relative;\n        height: 64px;\n        padding: 0 16px;\n        pointer-events: none;\n        font-size: var(--app-toolbar-font-size, 20px);\n      }\n\n      :host ::slotted(*) {\n        pointer-events: auto;\n      }\n\n      :host ::slotted(paper-icon-button) {\n        /* paper-icon-button/issues/33 */\n        font-size: 0;\n      }\n\n      :host ::slotted([main-title]),\n      :host ::slotted([condensed-title]) {\n        pointer-events: none;\n        @apply --layout-flex;\n      }\n\n      :host ::slotted([bottom-item]) {\n        position: absolute;\n        right: 0;\n        bottom: 0;\n        left: 0;\n      }\n\n      :host ::slotted([top-item]) {\n        position: absolute;\n        top: 0;\n        right: 0;\n        left: 0;\n      }\n\n      :host ::slotted([spacer]) {\n        margin-left: 64px;\n      }\n    </style>\n\n    <slot></slot>\n`,\n\n  is: 'app-toolbar'\n});\n",
-        "import \"@polymer/app-layout/app-toolbar/app-toolbar\";\nimport \"@ha/components/ha-icon-button\";\nimport \"@ha/components/ha-radio\";\nimport \"@ha/components/ha-formfield\";\nimport \"@ha/components/ha-textfield\";\nimport { fireEvent } from \"@ha/common/dom/fire_event\";\nimport { css, html, LitElement, PropertyValues, CSSResultGroup, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport { createCloseHeading } from \"@ha/components/ha-dialog\";\nimport type { HaRadio } from \"@ha/components/ha-radio\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport type { LCN, LcnDeviceConfig } from \"types/lcn\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport { loadProgressDialog } from \"./show-dialog-progress\";\nimport type { LcnDeviceDialogParams } from \"./show-dialog-create-device\";\n\n@customElement(\"lcn-create-device-dialog\")\nexport class CreateDeviceDialog extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @state() private _params?: LcnDeviceDialogParams;\n\n  @state() private _isGroup: boolean = false;\n\n  @state() private _segmentId: number = 0;\n\n  @state() private _addressId: number = 5;\n\n  private _invalid = false;\n\n  public async showDialog(params: LcnDeviceDialogParams): Promise<void> {\n    this._params = params;\n    this.lcn = params.lcn;\n    await this.updateComplete;\n  }\n\n  protected firstUpdated(changedProperties: PropertyValues): void {\n    super.firstUpdated(changedProperties);\n    loadProgressDialog();\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    super.willUpdate(changedProperties);\n    this._invalid =\n      !this._validateSegmentId(this._segmentId) ||\n      !this._validateAddressId(this._addressId, this._isGroup);\n  }\n\n  protected render() {\n    if (!this._params) {\n      return nothing;\n    }\n    return html`\n      <ha-dialog\n        open\n        scrimClickAction\n        escapeKeyAction\n        .heading=${createCloseHeading(\n          this.hass,\n          this.lcn.localize(\"dashboard-devices-dialog-create-title\"),\n        ) as unknown as string}\n        @closed=${this._closeDialog}\n      >\n        <div id=\"type\">${this.lcn.localize(\"type\")}</div>\n\n        <ha-formfield label=${this.lcn.localize(\"module\")}>\n          <ha-radio\n            name=\"is_group\"\n            value=\"module\"\n            .checked=${this._isGroup === false}\n            @change=${this._isGroupChanged}\n          ></ha-radio>\n        </ha-formfield>\n\n        <ha-formfield label=${this.lcn.localize(\"group\")}>\n          <ha-radio\n            name=\"is_group\"\n            value=\"group\"\n            .checked=${this._isGroup === true}\n            @change=${this._isGroupChanged}\n          ></ha-radio>\n        </ha-formfield>\n\n        <ha-textfield\n          .label=${this.lcn.localize(\"segment-id\")}\n          type=\"number\"\n          .value=${this._segmentId.toString()}\n          min=\"0\"\n          required\n          autoValidate\n          @input=${this._segmentIdChanged}\n          .validityTransform=${this._validityTransformSegmentId}\n          .validationMessage=${this.lcn.localize(\"dashboard-devices-dialog-error-segment\")}\n        ></ha-textfield>\n\n        <ha-textfield\n          .label=${this.lcn.localize(\"id\")}\n          type=\"number\"\n          .value=${this._addressId.toString()}\n          min=\"0\"\n          required\n          autoValidate\n          @input=${this._addressIdChanged}\n          .validityTransform=${this._validityTransformAddressId}\n          .validationMessage=${this._isGroup\n            ? this.lcn.localize(\"dashboard-devices-dialog-error-group\")\n            : this.lcn.localize(\"dashboard-devices-dialog-error-module\")}\n        ></ha-textfield>\n\n        <div class=\"buttons\">\n          <mwc-button\n            slot=\"secondaryAction\"\n            @click=${this._closeDialog}\n            .label=${this.lcn.localize(\"dismiss\")}\n          ></mwc-button>\n\n          <mwc-button\n            slot=\"primaryAction\"\n            @click=${this._create}\n            .disabled=${this._invalid}\n            .label=${this.lcn.localize(\"create\")}\n          ></mwc-button>\n        </div>\n      </ha-dialog>\n    `;\n  }\n\n  private _isGroupChanged(ev: ValueChangedEvent<string>): void {\n    this._isGroup = (ev.target as HaRadio).value === \"group\";\n  }\n\n  private _segmentIdChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this._segmentId = +target.value;\n  }\n\n  private _addressIdChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this._addressId = +target.value;\n  }\n\n  private _validateSegmentId(segment_id: number): boolean {\n    // segement_id: 0, 5-128\n    return segment_id === 0 || (segment_id >= 5 && segment_id <= 128);\n  }\n\n  private _validateAddressId(address_id: number, is_group: boolean): boolean {\n    // module_id: 5-254\n    // group_id: 5-254\n    if (is_group) {\n      return address_id >= 5 && address_id <= 254;\n    }\n    return address_id >= 5 && address_id <= 254;\n  }\n\n  private get _validityTransformSegmentId() {\n    return (value: string) => ({ valid: this._validateSegmentId(+value) });\n  }\n\n  private get _validityTransformAddressId() {\n    return (value: string) => ({ valid: this._validateAddressId(+value, this._isGroup) });\n  }\n\n  private async _create(): Promise<void> {\n    const values: Partial<LcnDeviceConfig> = {\n      name: \"\",\n      address: [this._segmentId, this._addressId, this._isGroup],\n    };\n    await this._params!.createDevice(values);\n    this._closeDialog();\n  }\n\n  private _closeDialog(): void {\n    this._params = undefined;\n    fireEvent(this, \"dialog-closed\", { dialog: this.localName });\n  }\n\n  static get styles(): CSSResultGroup {\n    return [\n      haStyleDialog,\n      css`\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .buttons {\n          display: flex;\n          justify-content: space-between;\n          padding: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-create-device-dialog\": CreateDeviceDialog;\n  }\n}\n"
+        "import \"@polymer/app-layout/app-toolbar/app-toolbar\";\nimport \"@ha/components/ha-icon-button\";\nimport \"@ha/components/ha-radio\";\nimport \"@ha/components/ha-formfield\";\nimport \"@ha/components/ha-textfield\";\nimport { fireEvent } from \"@ha/common/dom/fire_event\";\nimport { css, html, LitElement, PropertyValues, CSSResultGroup, nothing } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport { createCloseHeading } from \"@ha/components/ha-dialog\";\nimport type { HaRadio } from \"@ha/components/ha-radio\";\nimport { haStyleDialog } from \"@ha/resources/styles\";\nimport type { HomeAssistant, ValueChangedEvent } from \"@ha/types\";\nimport type { LCN, LcnDeviceConfig } from \"types/lcn\";\nimport type { HaTextField } from \"@ha/components/ha-textfield\";\nimport { loadProgressDialog } from \"./show-dialog-progress\";\nimport type { LcnDeviceDialogParams } from \"./show-dialog-create-device\";\n\n@customElement(\"lcn-create-device-dialog\")\nexport class CreateDeviceDialog extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @state() private _params?: LcnDeviceDialogParams;\n\n  @state() private _isGroup: boolean = false;\n\n  @state() private _segmentId: number = 0;\n\n  @state() private _addressId: number = 5;\n\n  @state() private _invalid: boolean = false;\n\n  public async showDialog(params: LcnDeviceDialogParams): Promise<void> {\n    this._params = params;\n    this.lcn = params.lcn;\n    await this.updateComplete;\n  }\n\n  protected firstUpdated(changedProperties: PropertyValues): void {\n    super.firstUpdated(changedProperties);\n    loadProgressDialog();\n  }\n\n  public willUpdate(changedProperties: PropertyValues) {\n    if (changedProperties.has(\"_invalid\")) {\n      this._invalid =\n        !this._validateSegmentId(this._segmentId) ||\n        !this._validateAddressId(this._addressId, this._isGroup);\n    }\n  }\n\n  protected render() {\n    if (!this._params) {\n      return nothing;\n    }\n    return html`\n      <ha-dialog\n        open\n        scrimClickAction\n        escapeKeyAction\n        .heading=${createCloseHeading(\n          this.hass,\n          this.lcn.localize(\"dashboard-devices-dialog-create-title\"),\n        ) as unknown as string}\n        @closed=${this._closeDialog}\n      >\n        <div id=\"type\">${this.lcn.localize(\"type\")}</div>\n\n        <ha-formfield label=${this.lcn.localize(\"module\")}>\n          <ha-radio\n            name=\"is_group\"\n            value=\"module\"\n            .checked=${this._isGroup === false}\n            @change=${this._isGroupChanged}\n          ></ha-radio>\n        </ha-formfield>\n\n        <ha-formfield label=${this.lcn.localize(\"group\")}>\n          <ha-radio\n            name=\"is_group\"\n            value=\"group\"\n            .checked=${this._isGroup === true}\n            @change=${this._isGroupChanged}\n          ></ha-radio>\n        </ha-formfield>\n\n        <ha-textfield\n          .label=${this.lcn.localize(\"segment-id\")}\n          type=\"number\"\n          .value=${this._segmentId.toString()}\n          min=\"0\"\n          required\n          autoValidate\n          @input=${this._segmentIdChanged}\n          .validityTransform=${this._validityTransformSegmentId}\n          .validationMessage=${this.lcn.localize(\"dashboard-devices-dialog-error-segment\")}\n        ></ha-textfield>\n\n        <ha-textfield\n          .label=${this.lcn.localize(\"id\")}\n          type=\"number\"\n          .value=${this._addressId.toString()}\n          min=\"0\"\n          required\n          autoValidate\n          @input=${this._addressIdChanged}\n          .validityTransform=${this._validityTransformAddressId}\n          .validationMessage=${this._isGroup\n            ? this.lcn.localize(\"dashboard-devices-dialog-error-group\")\n            : this.lcn.localize(\"dashboard-devices-dialog-error-module\")}\n        ></ha-textfield>\n\n        <div class=\"buttons\">\n          <mwc-button\n            slot=\"secondaryAction\"\n            @click=${this._closeDialog}\n            .label=${this.lcn.localize(\"dismiss\")}\n          ></mwc-button>\n\n          <mwc-button\n            slot=\"primaryAction\"\n            @click=${this._create}\n            .disabled=${this._invalid}\n            .label=${this.lcn.localize(\"create\")}\n          ></mwc-button>\n        </div>\n      </ha-dialog>\n    `;\n  }\n\n  private _isGroupChanged(ev: ValueChangedEvent<string>): void {\n    this._isGroup = (ev.target as HaRadio).value === \"group\";\n  }\n\n  private _segmentIdChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this._segmentId = +target.value;\n  }\n\n  private _addressIdChanged(ev: ValueChangedEvent<string>): void {\n    const target = ev.target as HaTextField;\n    this._addressId = +target.value;\n  }\n\n  private _validateSegmentId(segment_id: number): boolean {\n    // segement_id: 0, 5-128\n    return segment_id === 0 || (segment_id >= 5 && segment_id <= 128);\n  }\n\n  private _validateAddressId(address_id: number, is_group: boolean): boolean {\n    // module_id: 5-254\n    // group_id: 5-254\n    if (is_group) {\n      return address_id >= 5 && address_id <= 254;\n    }\n    return address_id >= 5 && address_id <= 254;\n  }\n\n  private get _validityTransformSegmentId() {\n    return (value: string) => ({ valid: this._validateSegmentId(+value) });\n  }\n\n  private get _validityTransformAddressId() {\n    return (value: string) => ({ valid: this._validateAddressId(+value, this._isGroup) });\n  }\n\n  private async _create(): Promise<void> {\n    const values: Partial<LcnDeviceConfig> = {\n      name: \"\",\n      address: [this._segmentId, this._addressId, this._isGroup],\n    };\n    await this._params!.createDevice(values);\n    this._closeDialog();\n  }\n\n  private _closeDialog(): void {\n    this._params = undefined;\n    fireEvent(this, \"dialog-closed\", { dialog: this.localName });\n  }\n\n  static get styles(): CSSResultGroup {\n    return [\n      haStyleDialog,\n      css`\n        #port-type {\n          margin-top: 16px;\n        }\n        ha-textfield {\n          display: block;\n          margin-bottom: 8px;\n        }\n        .buttons {\n          display: flex;\n          justify-content: space-between;\n          padding: 8px;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-create-device-dialog\": CreateDeviceDialog;\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oyUFw0ts.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/oyUFw0ts.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oyUFw0ts.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/oyUFw0ts.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/oyUFw0ts.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/oyUFw0ts.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/sBNRM32J.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/sBNRM32J.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/sBNRM32J.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/sBNRM32J.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/sBNRM32J.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/sBNRM32J.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yvD5aARM.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9yFFShGq.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -560,16 +560,16 @@
             c = i(4243),
             r = i(1285),
             s = (i(657), i(1952), i(4776), i(8336), i(7662), i(9051)),
             h = i(8394);
         const u = () => Promise.all([i.e(597), i.e(812), i.e(244)]).then(i.bind(i, 7044));
         var m = i(8361),
             b = i(4516),
-            _ = i(1750),
-            f = i(3239),
+            f = i(1750),
+            _ = i(3239),
             p = i(3448),
             v = i(153),
             g = i(6538),
             k = i(2136),
             x = i(2218),
             y = i(2537);
         const w = async () => {
@@ -721,15 +721,15 @@
     `
                     }
                 }]
             }
         }), n.oi);
         var $ = i(3217);
         let C;
-        const L = () => (C || (C = (0, $.Ud)(new Worker(new URL(i.p + i.u(456), i.b), {
+        const z = () => (C || (C = (0, $.Ud)(new Worker(new URL(i.p + i.u(456), i.b), {
             type: "module"
         }))), C);
         (0, a.Z)([(0, c.Mo)("ha-data-table")], (function(e, t) {
             class i extends t {
                 constructor(...t) {
                     super(...t), e(this)
                 }
@@ -958,15 +958,15 @@
                     value: function(e) {
                         if ((0, l.Z)((0, d.Z)(i.prototype), "willUpdate", this).call(this, e), this.hasUpdated || w(), e.has("columns")) {
                             this._filterable = Object.values(this.columns).some((e => e.filterable));
                             for (const t in this.columns)
                                 if (this.columns[t].direction) {
                                     this._sortDirection = this.columns[t].direction, this._sortColumn = t;
                                     break
-                                } const e = (0, f.Z)(this.columns);
+                                } const e = (0, _.Z)(this.columns);
                             Object.values(e).forEach((e => {
                                 delete e.title, delete e.template
                             })), this._sortColumns = e
                         }
                         e.has("filter") && this._debounceSearch(this.filter), e.has("data") && (this._checkableRowsCount = this.data.filter((e => !1 !== e.selectable)).length), (e.has("data") || e.has("columns") || e.has("_filter") || e.has("_sortColumn") || e.has("_sortDirection")) && this._sortFilterData()
                     }
                 }, {
@@ -1117,15 +1117,15 @@
                     key: "_sortFilterData",
                     value: async function() {
                         const e = (new Date).getTime();
                         this.curRequest++;
                         const t = this.curRequest;
                         let i = this.data;
                         this._filter && (i = await this._memFilterData(this.data, this._sortColumns, this._filter));
-                        const a = this._sortColumn ? ((e, t, i, a, l) => L().sortData(e, t, i, a, l))(i, this._sortColumns[this._sortColumn], this._sortDirection, this._sortColumn, this.hass.locale.language) : i,
+                        const a = this._sortColumn ? ((e, t, i, a, l) => z().sortData(e, t, i, a, l))(i, this._sortColumns[this._sortColumn], this._sortDirection, this._sortColumn, this.hass.locale.language) : i,
                             [l] = await Promise.all([a, y.y]),
                             d = (new Date).getTime() - e;
                         if (d < 100 && await new Promise((e => {
                                 setTimeout(e, 100 - d)
                             })), this.curRequest === t) {
                             if (this.appendRow || this.hasFab) {
                                 const e = [...l];
@@ -1139,15 +1139,15 @@
                             this._filteredData = l
                         }
                     }
                 }, {
                     kind: "field",
                     key: "_memFilterData",
                     value() {
-                        return (0, b.Z)(((e, t, i) => ((e, t, i) => L().filterData(e, t, i))(e, t, i)))
+                        return (0, b.Z)(((e, t, i) => ((e, t, i) => z().filterData(e, t, i))(e, t, i)))
                     }
                 }, {
                     kind: "method",
                     key: "_handleHeaderClick",
                     value: function(e) {
                         const t = e.currentTarget.columnId;
                         this.columns[t].sortable && (this._sortDirection && this._sortColumn === t ? "asc" === this._sortDirection ? this._sortDirection = "desc" : this._sortDirection = null : this._sortDirection = "asc", this._sortColumn = null === this._sortDirection ? void 0 : t, (0, h.B)(this, "sorting-changed", {
@@ -1628,15 +1628,15 @@
           overscroll-behavior: contain;
         }
       `]
                     }
                 }]
             }
         }), n.oi);
-        var z = i(8480);
+        var L = i(8480);
         const D = "M19,4H15.5L14.5,3H9.5L8.5,4H5V6H19M6,19A2,2 0 0,0 8,21H16A2,2 0 0,0 18,19V7H6V19Z";
         (0, a.Z)([(0, c.Mo)("lcn-devices-data-table")], (function(e, t) {
             class i extends t {
                 constructor(...t) {
                     super(...t), e(this)
                 }
             }
@@ -1767,15 +1767,15 @@
                         return n.dy`
       <ha-data-table
         .hass=${this.hass}
         .columns=${this._columns(this.narrow)}
         .data=${this._devices(this.devices)}
         .id=${"address"}
         .noDataText=${this.lcn.localize("dashboard-devices-table-no-data")}
-        .dir=${(0,_.Zu)(this.hass)}
+        .dir=${(0,f.Zu)(this.hass)}
         auto-height
         clickable
         @row-click=${this._rowClicked}
       ></ha-data-table>
     `
                     }
                 }, {
@@ -1799,15 +1799,15 @@
                             composed: !0
                         }))
                     }
                 }, {
                     kind: "method",
                     key: "_openDevice",
                     value: function() {
-                        (0, z.c)("/lcn/entities")
+                        (0, L.c)("/lcn/entities")
                     }
                 }, {
                     kind: "method",
                     key: "_deleteDevice",
                     value: async function(e) {
                         const t = this.devices.find((t => t.address[0] === e[0] && t.address[1] === e[1] && t.address[2] === e[2]));
                         await (0, r.g7)(this, {
@@ -1859,74 +1859,68 @@
                         attribute: !1
                     })],
                     key: "route",
                     value: void 0
                 }, {
                     kind: "field",
                     decorators: [(0, c.Cb)({
+                        attribute: !1
+                    })],
+                    key: "hosts",
+                    value: void 0
+                }, {
+                    kind: "field",
+                    decorators: [(0, c.Cb)({
                         type: Array,
                         reflect: !1
                     })],
                     key: "tabs",
                     value() {
                         return []
                     }
                 }, {
                     kind: "field",
                     decorators: [(0, c.SB)()],
-                    key: "_hosts",
-                    value() {
-                        return []
-                    }
-                }, {
-                    kind: "field",
-                    decorators: [(0, c.SB)()],
                     key: "_deviceConfigs",
                     value() {
                         return []
                     }
                 }, {
-                    kind: "field",
-                    decorators: [(0, c.IO)("#host-select")],
-                    key: "_hostsSelect",
-                    value: void 0
-                }, {
                     kind: "method",
                     key: "firstUpdated",
                     value: async function(e) {
-                        (0, l.Z)((0, d.Z)(i.prototype), "firstUpdated", this).call(this, e), await this._fetchHosts(), (0, m.z)(), u(), this._hostsSelect.value = this.lcn.host.id, this.addEventListener("lcn-config-changed", (async () => {
+                        (0, l.Z)((0, d.Z)(i.prototype), "firstUpdated", this).call(this, e), (0, m.z)(), u(), this.addEventListener("lcn-config-changed", (async () => {
                             this._fetchDevices(this.lcn.host)
                         }))
                     }
                 }, {
                     kind: "method",
                     key: "render",
                     value: function() {
-                        return this.hass && this.lcn ? n.dy`
+                        return this.hass && this.lcn && this.hosts ? n.dy`
       <hass-tabs-subpage
         .hass=${this.hass}
         .narrow=${this.narrow}
-        back-path="/lcn"
         .route=${this.route}
         .tabs=${this.tabs}
+        main-page
       >
+        <span slot="header"> ${this.lcn.localize("dashboard-devices-title")} </span>
         <ha-config-section .narrow=${this.narrow}>
-          <span slot="header"> ${this.lcn.localize("dashboard-devices-title")} </span>
-
-          <span slot="introduction"> ${this.lcn.localize("dashboard-devices-introduction")} </span>
+          <span slot="introduction"> ${this.renderIntro()} </span>
 
           <div id="box">
             <ha-select
               id="host-select"
               .label=${this.lcn.localize("dashboard-devices-hosts")}
               .value=${this.lcn.host.id}
               fixedMenuPosition
               @selected=${this._hostChanged}
             >
-              ${this._hosts.map((e=>n.dy` <ha-list-item .value=${e.id}> ${e.name} </ha-list-item> `))}
+              ${this.hosts.map((e=>n.dy` <ha-list-item .value=${e.id}> ${e.name} </ha-list-item> `))}
             </ha-select>
 
             <mwc-button id="scan_devices" raised @click=${this._scanDevices}>
               ${this.lcn.localize("dashboard-devices-scan")}
             </mwc-button>
           </div>
 
@@ -1950,25 +1944,37 @@
           <ha-svg-icon slot="icon" .path=${"M19,13H13V19H11V13H5V11H11V5H13V11H19V13Z"}></ha-svg-icon>
         </ha-fab>
       </hass-tabs-subpage>
     ` : n.dy` <hass-loading-screen></hass-loading-screen> `
                     }
                 }, {
                     kind: "method",
-                    key: "_hostChanged",
-                    value: function(e) {
-                        const t = e.target,
-                            i = this._hosts.find((e => e.id === t.value));
-                        this.lcn.host = i, this._fetchDevices(this.lcn.host)
+                    key: "renderIntro",
+                    value: function() {
+                        return n.dy`
+      <h2>${this.lcn.localize("dashboard-devices-introduction")}</h2>
+      ${this.lcn.localize("dashboard-devices-introduction-help-1")} <br />
+      <details>
+        <summary>${this.lcn.localize("more-help")}</summary>
+        <ul>
+          <li>${this.lcn.localize("dashboard-devices-introduction-help-2")}</li>
+          <li>${this.lcn.localize("dashboard-devices-introduction-help-3")}</li>
+          <li>${this.lcn.localize("dashboard-devices-introduction-help-4")}</li>
+          <li>${this.lcn.localize("dashboard-devices-introduction-help-5")}</li>
+        </ul>
+      </details>
+    `
                     }
                 }, {
                     kind: "method",
-                    key: "_fetchHosts",
-                    value: async function() {
-                        this._hosts = await (0, s.V5)(this.hass)
+                    key: "_hostChanged",
+                    value: async function(e) {
+                        const t = e.target,
+                            i = this.hosts.find((e => e.id === t.value));
+                        this.lcn.host = i, await this._fetchDevices(this.lcn.host)
                     }
                 }, {
                     kind: "method",
                     key: "_fetchDevices",
                     value: async function(e) {
                         this._deviceConfigs = await (0, s.LO)(this.hass, e.id)
                     }
@@ -2034,15 +2040,18 @@
           display: inline-block;
         }
         #scan-devices {
           display: inline-block;
           margin-top: 20px;
           justify-content: center;
         }
+        summary:hover {
+          text-decoration: underline;
+        }
       `]
                     }
                 }]
             }
         }), n.oi)
     }
 };
-//# sourceMappingURL=yvD5aARM.js.map
+//# sourceMappingURL=9yFFShGq.js.map
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yvD5aARM.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/9yFFShGq.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8412698412698413%*

 * *Differences: {"'file'": "'9yFFShGq.js'",*

 * * "'mappings'": "';;;;AAcA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACmEA;AC/DA;AACA;;AAGA;AArBA;AAuBA;AAGA;;AAIA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsFA;;AC/CA;AACA;;AAEA;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAyHA;;;;;;;;;;AAWA;;AC9KA;AACA;AACA;;AAEA;AACA;;;;;;;;;;AAUA;;AAGA;AACA;;;;;;;;AASA;;;;;;;;;;;;;;;;;;;;;AAqCA;;AC2IA;AACA;;;AAIA;AACA;AACA;AACA;;;AAGA;;;AAIA;; […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "yvD5aARM.js",
-    "mappings": ";;;;AAcA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACmEA;AC/DA;AACA;;AAGA;AArBA;AAuBA;AAGA;;AAIA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsFA;;AC/CA;AACA;;AAEA;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAyHA;;;;;;;;;;AAWA;;AC9KA;AACA;AACA;;AAEA;AACA;;;;;;;;;;AAUA;;AAGA;AACA;;;;;;;;AASA;;;;;;;;;;;;;;;;;;;;;AAqCA;;AC2IA;AACA;;;AAIA;AACA;AACA;AACA;;;AAGA;;;AAIA;;AAIA;AACA;;;AAOA;;;;;;;AAQA;AACA;AAEA;;;;AAKA;AAEA;;AAmBA;AACA;AACA;;AAOA;AAOA;AACA;;AAEA;;AAGA;;AAIA;AAEA;;AAEA;;AAGA;;;;AAeA;AACA;AACA;AACA;;AAlBA;;;;AAKA;;;;;;;AAmBA;;AAiBA;;AAEA;AACA;AACA;AAMA;AAGA;;AAEA;;;;;;;AAQA;AACA;AACA;AACA;;;;AAIA;AAEA;;AAMA;AACA;AAWA;;AAOA;;;;AAnEA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA0nBA;;ACv6BA;AACA;AAJA;;AAUA;;AAmCA;AACA;AAJA;;AAWA;;AAUA;AACA;AACA;AACA;AACA;AACA;;;AAGA;;AAGA;AA0CA;AACA;AAGA;AACA;;AAEA;;ACjHA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;;;;;AAKA;AACA;;AAEA;;AAEA;;;AAKA;AACA;;;;;AAKA;;;AAGA;AACA;AACA;AACA;;;;;;AAMA;AACA;;;AA3GA;;;AA4DA;AA4FA;;AAEA;AAIA;AAKA;AACA;AACA;;AAEA;;;;;;;;;;;;;;AA2BA",
+    "file": "9yFFShGq.js",
+    "mappings": ";;;;AAcA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACmEA;AC/DA;AACA;;AAGA;AArBA;AAuBA;AAGA;;AAIA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAsFA;;AC/CA;AACA;;AAEA;;AAGA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAyHA;;;;;;;;;;AAWA;;AC9KA;AACA;AACA;;AAEA;AACA;;;;;;;;;;AAUA;;AAGA;AACA;;;;;;;;AASA;;;;;;;;;;;;;;;;;;;;;AAqCA;;AC2IA;AACA;;;AAIA;AACA;AACA;AACA;;;AAGA;;;AAIA;;AAIA;AACA;;;AAOA;;;;;;;AAQA;AACA;AAEA;;;;AAKA;AAEA;;AAmBA;AACA;AACA;;AAOA;AAOA;AACA;;AAEA;;AAGA;;AAIA;AAEA;;AAEA;;AAGA;;;;AAeA;AACA;AACA;AACA;;AAlBA;;;;AAKA;;;;;;;AAmBA;;AAiBA;;AAEA;AACA;AACA;AAMA;AAGA;;AAEA;;;;;;;AAQA;AACA;AACA;AACA;;;;AAIA;AAEA;;AAMA;AACA;AAWA;;AAOA;;;;AAnEA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AA0nBA;;ACv6BA;AACA;AAJA;;AAUA;;AAmCA;AACA;AAJA;;AAWA;;AAUA;AACA;AACA;AACA;AACA;AACA;;;AAGA;;AAGA;AA0CA;AACA;AAGA;AACA;;AAEA;;AC9HA;AACA;AACA;AACA;;;AAGA;AACA;AACA;;;;;AAKA;AACA;;AAEA;;AAEA;;;AAKA;AACA;;;;;AAKA;;;AAGA;AACA;AACA;AACA;;;;;;AAMA;AACA;;;AA7FA;;;AA+CA;AAyDA;AACA;;AAEA;;AAEA;AACA;AACA;AACA;;;AAIA;AAkCA;;AAEA;AAIA;AAKA;AACA;AACA;;AAEA;;;;;;;;;;;;;;;;;AA8BA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-checkbox.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-list-item.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-select.ts",
         "webpack://lcn-frontend/./homeassistant-frontend/src/components/ha-textfield.ts",
@@ -17,11 +17,11 @@
         "import { CheckboxBase } from \"@material/mwc-checkbox/mwc-checkbox-base\";\nimport { styles } from \"@material/mwc-checkbox/mwc-checkbox.css\";\nimport { css } from \"lit\";\nimport { customElement } from \"lit/decorators\";\n\n@customElement(\"ha-checkbox\")\nexport class HaCheckbox extends CheckboxBase {\n  static override styles = [\n    styles,\n    css`\n      :host {\n        --mdc-theme-secondary: var(--primary-color);\n      }\n    `,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-checkbox\": HaCheckbox;\n  }\n}\n",
         "import { ListItemBase } from \"@material/mwc-list/mwc-list-item-base\";\nimport { styles } from \"@material/mwc-list/mwc-list-item.css\";\nimport { css, CSSResultGroup } from \"lit\";\nimport { customElement } from \"lit/decorators\";\n\n@customElement(\"ha-list-item\")\nexport class HaListItem extends ListItemBase {\n  protected renderRipple() {\n    if (this.noninteractive) {\n      return \"\";\n    }\n    return super.renderRipple();\n  }\n\n  static get styles(): CSSResultGroup {\n    return [\n      styles,\n      css`\n        :host {\n          padding-left: var(\n            --mdc-list-side-padding-left,\n            var(--mdc-list-side-padding, 20px)\n          );\n          padding-right: var(\n            --mdc-list-side-padding-right,\n            var(--mdc-list-side-padding, 20px)\n          );\n        }\n        :host([graphic=\"avatar\"]:not([twoLine])),\n        :host([graphic=\"icon\"]:not([twoLine])) {\n          height: 48px;\n        }\n        span.material-icons:first-of-type {\n          margin-inline-start: 0px !important;\n          margin-inline-end: var(\n            --mdc-list-item-graphic-margin,\n            16px\n          ) !important;\n          direction: var(--direction);\n        }\n        span.material-icons:last-of-type {\n          margin-inline-start: auto !important;\n          margin-inline-end: 0px !important;\n          direction: var(--direction);\n        }\n        .mdc-deprecated-list-item__meta {\n          display: var(--mdc-list-item-meta-display);\n          align-items: center;\n        }\n        :host([multiline-secondary]) {\n          height: auto;\n        }\n        :host([multiline-secondary]) .mdc-deprecated-list-item__text {\n          padding: 8px 0;\n        }\n        :host([multiline-secondary]) .mdc-deprecated-list-item__secondary-text {\n          text-overflow: initial;\n          white-space: normal;\n          overflow: auto;\n          display: inline-block;\n          margin-top: 10px;\n        }\n        :host([multiline-secondary]) .mdc-deprecated-list-item__primary-text {\n          margin-top: 10px;\n        }\n        :host([multiline-secondary])\n          .mdc-deprecated-list-item__secondary-text::before {\n          display: none;\n        }\n        :host([multiline-secondary])\n          .mdc-deprecated-list-item__primary-text::before {\n          display: none;\n        }\n        :host([disabled]) {\n          color: var(--disabled-text-color);\n        }\n        :host([noninteractive]) {\n          pointer-events: unset;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-list-item\": HaListItem;\n  }\n}\n",
         "import { SelectBase } from \"@material/mwc-select/mwc-select-base\";\nimport { styles } from \"@material/mwc-select/mwc-select.css\";\nimport { mdiClose } from \"@mdi/js\";\nimport { css, html, nothing } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\nimport { debounce } from \"../common/util/debounce\";\nimport { nextRender } from \"../common/util/render-status\";\nimport \"./ha-icon-button\";\n\n@customElement(\"ha-select\")\nexport class HaSelect extends SelectBase {\n  // @ts-ignore\n  @property({ type: Boolean }) public icon?: boolean;\n\n  @property({ type: Boolean, reflect: true }) public clearable?: boolean;\n\n  protected override render() {\n    return html`\n      ${super.render()}\n      ${this.clearable && !this.required && !this.disabled && this.value\n        ? html`<ha-icon-button\n            label=\"clear\"\n            @click=${this._clearValue}\n            .path=${mdiClose}\n          ></ha-icon-button>`\n        : nothing}\n    `;\n  }\n\n  protected override renderLeadingIcon() {\n    if (!this.icon) {\n      return nothing;\n    }\n\n    return html`<span class=\"mdc-select__icon\"\n      ><slot name=\"icon\"></slot\n    ></span>`;\n  }\n\n  connectedCallback() {\n    super.connectedCallback();\n    window.addEventListener(\"translations-updated\", this._translationsUpdated);\n  }\n\n  disconnectedCallback() {\n    super.disconnectedCallback();\n    window.removeEventListener(\n      \"translations-updated\",\n      this._translationsUpdated\n    );\n  }\n\n  private _clearValue(): void {\n    if (this.disabled || !this.value) {\n      return;\n    }\n    this.valueSetDirectly = true;\n    this.select(-1);\n    this.mdcFoundation.handleChange();\n  }\n\n  private _translationsUpdated = debounce(async () => {\n    await nextRender();\n    this.layoutOptions();\n  }, 500);\n\n  static override styles = [\n    styles,\n    css`\n      :host([clearable]) {\n        position: relative;\n      }\n      .mdc-select:not(.mdc-select--disabled) .mdc-select__icon {\n        color: var(--secondary-text-color);\n      }\n      .mdc-select__anchor {\n        width: var(--ha-select-min-width, 200px);\n      }\n      .mdc-select--filled .mdc-select__anchor {\n        height: var(--ha-select-height, 56px);\n      }\n      .mdc-select--filled .mdc-floating-label {\n        inset-inline-start: 12px;\n        inset-inline-end: initial;\n        direction: var(--direction);\n      }\n      .mdc-select--filled.mdc-select--with-leading-icon .mdc-floating-label {\n        inset-inline-start: 48px;\n        inset-inline-end: initial;\n        direction: var(--direction);\n      }\n      .mdc-select .mdc-select__anchor {\n        padding-inline-start: 12px;\n        padding-inline-end: 0px;\n        direction: var(--direction);\n      }\n      .mdc-select__anchor .mdc-floating-label--float-above {\n        transform-origin: var(--float-start);\n      }\n      .mdc-select__selected-text-container {\n        padding-inline-end: var(--select-selected-text-padding-end, 0px);\n      }\n      :host([clearable]) .mdc-select__selected-text-container {\n        padding-inline-end: var(--select-selected-text-padding-end, 12px);\n      }\n      ha-icon-button {\n        position: absolute;\n        top: 10px;\n        right: 28px;\n        --mdc-icon-button-size: 36px;\n        --mdc-icon-size: 20px;\n        color: var(--secondary-text-color);\n        inset-inline-start: initial;\n        inset-inline-end: 28px;\n        direction: var(--direction);\n      }\n    `,\n  ];\n}\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-select\": HaSelect;\n  }\n}\n",
         "import { TextFieldBase } from \"@material/mwc-textfield/mwc-textfield-base\";\nimport { styles } from \"@material/mwc-textfield/mwc-textfield.css\";\nimport { TemplateResult, html, PropertyValues, css } from \"lit\";\nimport { customElement, property, query } from \"lit/decorators\";\nimport { mainWindow } from \"../common/dom/get_main_window\";\n\n@customElement(\"ha-textfield\")\nexport class HaTextField extends TextFieldBase {\n  @property({ type: Boolean }) public invalid?: boolean;\n\n  @property({ attribute: \"error-message\" }) public errorMessage?: string;\n\n  // @ts-ignore\n  @property({ type: Boolean }) public icon?: boolean;\n\n  // @ts-ignore\n  @property({ type: Boolean }) public iconTrailing?: boolean;\n\n  @property() public autocomplete?: string;\n\n  @property() public autocorrect?: string;\n\n  @property({ attribute: \"input-spellcheck\" })\n  public inputSpellcheck?: string;\n\n  @query(\"input\") public formElement!: HTMLInputElement;\n\n  override updated(changedProperties: PropertyValues) {\n    super.updated(changedProperties);\n    if (\n      (changedProperties.has(\"invalid\") &&\n        (this.invalid || changedProperties.get(\"invalid\") !== undefined)) ||\n      changedProperties.has(\"errorMessage\")\n    ) {\n      this.setCustomValidity(\n        this.invalid ? this.errorMessage || \"Invalid\" : \"\"\n      );\n      this.reportValidity();\n    }\n    if (changedProperties.has(\"autocomplete\")) {\n      if (this.autocomplete) {\n        this.formElement.setAttribute(\"autocomplete\", this.autocomplete);\n      } else {\n        this.formElement.removeAttribute(\"autocomplete\");\n      }\n    }\n    if (changedProperties.has(\"autocorrect\")) {\n      if (this.autocorrect) {\n        this.formElement.setAttribute(\"autocorrect\", this.autocorrect);\n      } else {\n        this.formElement.removeAttribute(\"autocorrect\");\n      }\n    }\n    if (changedProperties.has(\"inputSpellcheck\")) {\n      if (this.inputSpellcheck) {\n        this.formElement.setAttribute(\"spellcheck\", this.inputSpellcheck);\n      } else {\n        this.formElement.removeAttribute(\"spellcheck\");\n      }\n    }\n  }\n\n  protected override renderIcon(\n    _icon: string,\n    isTrailingIcon = false\n  ): TemplateResult {\n    const type = isTrailingIcon ? \"trailing\" : \"leading\";\n\n    return html`\n      <span\n        class=\"mdc-text-field__icon mdc-text-field__icon--${type}\"\n        tabindex=${isTrailingIcon ? 1 : -1}\n      >\n        <slot name=\"${type}Icon\"></slot>\n      </span>\n    `;\n  }\n\n  static override styles = [\n    styles,\n    css`\n      .mdc-text-field__input {\n        width: var(--ha-textfield-input-width, 100%);\n      }\n      .mdc-text-field:not(.mdc-text-field--with-leading-icon) {\n        padding: var(--text-field-padding, 0px 16px);\n      }\n      .mdc-text-field__affix--suffix {\n        padding-left: var(--text-field-suffix-padding-left, 12px);\n        padding-right: var(--text-field-suffix-padding-right, 0px);\n        padding-inline-start: var(--text-field-suffix-padding-left, 12px);\n        padding-inline-end: var(--text-field-suffix-padding-right, 0px);\n        direction: var(--direction);\n      }\n      .mdc-text-field--with-leading-icon {\n        padding-inline-start: var(--text-field-suffix-padding-left, 0px);\n        padding-inline-end: var(--text-field-suffix-padding-right, 16px);\n        direction: var(--direction);\n      }\n\n      .mdc-text-field--with-leading-icon.mdc-text-field--with-trailing-icon {\n        padding-left: var(--text-field-suffix-padding-left, 0px);\n        padding-right: var(--text-field-suffix-padding-right, 0px);\n        padding-inline-start: var(--text-field-suffix-padding-left, 0px);\n        padding-inline-end: var(--text-field-suffix-padding-right, 0px);\n      }\n      .mdc-text-field:not(.mdc-text-field--disabled)\n        .mdc-text-field__affix--suffix {\n        color: var(--secondary-text-color);\n      }\n\n      .mdc-text-field__icon {\n        color: var(--secondary-text-color);\n      }\n\n      .mdc-text-field__icon--leading {\n        margin-inline-start: 16px;\n        margin-inline-end: 8px;\n        direction: var(--direction);\n      }\n\n      .mdc-text-field__icon--trailing {\n        padding: var(--textfield-icon-trailing-padding, 12px);\n      }\n\n      .mdc-floating-label:not(.mdc-floating-label--float-above) {\n        text-overflow: ellipsis;\n        width: inherit;\n        padding-right: 30px;\n        padding-inline-end: 30px;\n        padding-inline-start: initial;\n        box-sizing: border-box;\n        direction: var(--direction);\n      }\n\n      input {\n        text-align: var(--text-field-text-align, start);\n      }\n\n      /* Edge, hide reveal password icon */\n      ::-ms-reveal {\n        display: none;\n      }\n\n      /* Chrome, Safari, Edge, Opera */\n      :host([no-spinner]) input::-webkit-outer-spin-button,\n      :host([no-spinner]) input::-webkit-inner-spin-button {\n        -webkit-appearance: none;\n        margin: 0;\n      }\n\n      /* Firefox */\n      :host([no-spinner]) input[type=\"number\"] {\n        -moz-appearance: textfield;\n      }\n\n      .mdc-text-field__ripple {\n        overflow: hidden;\n      }\n\n      .mdc-text-field {\n        overflow: var(--text-field-overflow);\n      }\n\n      .mdc-floating-label {\n        inset-inline-start: 16px !important;\n        inset-inline-end: initial !important;\n        transform-origin: var(--float-start);\n        direction: var(--direction);\n        text-align: var(--float-start);\n      }\n\n      .mdc-text-field--with-leading-icon.mdc-text-field--filled\n        .mdc-floating-label {\n        max-width: calc(\n          100% - 48px - var(--text-field-suffix-padding-left, 0px)\n        );\n        inset-inline-start: calc(\n          48px + var(--text-field-suffix-padding-left, 0px)\n        ) !important;\n        inset-inline-end: initial !important;\n        direction: var(--direction);\n      }\n\n      .mdc-text-field__input[type=\"number\"] {\n        direction: var(--direction);\n      }\n      .mdc-text-field__affix--prefix {\n        padding-right: var(--text-field-prefix-padding-right, 2px);\n      }\n\n      .mdc-text-field:not(.mdc-text-field--disabled)\n        .mdc-text-field__affix--prefix {\n        color: var(--mdc-text-field-label-ink-color);\n      }\n    `,\n    // safari workaround - must be explicit\n    mainWindow.document.dir === \"rtl\"\n      ? css`\n          .mdc-text-field__affix--suffix,\n          .mdc-text-field--with-leading-icon,\n          .mdc-text-field__icon--leading,\n          .mdc-floating-label,\n          .mdc-text-field--with-leading-icon.mdc-text-field--filled\n            .mdc-floating-label,\n          .mdc-text-field__input[type=\"number\"] {\n            direction: rtl;\n          }\n        `\n      : css``,\n  ];\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-textfield\": HaTextField;\n  }\n}\n",
         "import { mdiClose, mdiMagnify } from \"@mdi/js\";\nimport { css, CSSResultGroup, html, LitElement, TemplateResult } from \"lit\";\nimport { customElement, property, query } from \"lit/decorators\";\nimport \"./ha-icon-button\";\nimport \"./ha-svg-icon\";\nimport \"./ha-textfield\";\nimport type { HaTextField } from \"./ha-textfield\";\nimport { HomeAssistant } from \"../types\";\nimport { fireEvent } from \"../common/dom/fire_event\";\n\n@customElement(\"search-input\")\nclass SearchInput extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property() public filter?: string;\n\n  @property({ type: Boolean })\n  public suffix = false;\n\n  @property({ type: Boolean })\n  public autofocus = false;\n\n  @property({ type: String })\n  public label?: string;\n\n  public focus() {\n    this._input?.focus();\n  }\n\n  @query(\"ha-textfield\", true) private _input!: HaTextField;\n\n  protected render(): TemplateResult {\n    return html`\n      <ha-textfield\n        .autofocus=${this.autofocus}\n        .label=${this.label || this.hass.localize(\"ui.common.search\")}\n        .value=${this.filter || \"\"}\n        icon\n        .iconTrailing=${this.filter || this.suffix}\n        @input=${this._filterInputChanged}\n      >\n        <slot name=\"prefix\" slot=\"leadingIcon\">\n          <ha-svg-icon\n            tabindex=\"-1\"\n            class=\"prefix\"\n            .path=${mdiMagnify}\n          ></ha-svg-icon>\n        </slot>\n        <div class=\"trailing\" slot=\"trailingIcon\">\n          ${this.filter &&\n          html`\n            <ha-icon-button\n              @click=${this._clearSearch}\n              .label=${this.hass.localize(\"ui.common.clear\")}\n              .path=${mdiClose}\n              class=\"clear-button\"\n            ></ha-icon-button>\n          `}\n          <slot name=\"suffix\"></slot>\n        </div>\n      </ha-textfield>\n    `;\n  }\n\n  private async _filterChanged(value: string) {\n    fireEvent(this, \"value-changed\", { value: String(value) });\n  }\n\n  private async _filterInputChanged(e) {\n    this._filterChanged(e.target.value);\n  }\n\n  private async _clearSearch() {\n    this._filterChanged(\"\");\n  }\n\n  static get styles(): CSSResultGroup {\n    return css`\n      :host {\n        display: inline-flex;\n      }\n      ha-svg-icon,\n      ha-icon-button {\n        color: var(--primary-text-color);\n      }\n      ha-svg-icon {\n        outline: none;\n      }\n      .clear-button {\n        --mdc-icon-size: 20px;\n      }\n      ha-textfield {\n        display: inherit;\n      }\n      .trailing {\n        display: flex;\n        align-items: center;\n      }\n    `;\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"search-input\": SearchInput;\n  }\n}\n",
         "import { mdiArrowDown, mdiArrowUp } from \"@mdi/js\";\nimport deepClone from \"deep-clone-simple\";\nimport {\n  css,\n  CSSResultGroup,\n  html,\n  LitElement,\n  nothing,\n  PropertyValues,\n  TemplateResult,\n} from \"lit\";\nimport {\n  customElement,\n  eventOptions,\n  property,\n  query,\n  state,\n} from \"lit/decorators\";\nimport { classMap } from \"lit/directives/class-map\";\nimport { ifDefined } from \"lit/directives/if-defined\";\nimport { styleMap } from \"lit/directives/style-map\";\nimport memoizeOne from \"memoize-one\";\nimport { restoreScroll } from \"../../common/decorators/restore-scroll\";\nimport { fireEvent } from \"../../common/dom/fire_event\";\nimport { debounce } from \"../../common/util/debounce\";\nimport { nextRender } from \"../../common/util/render-status\";\nimport { haStyleScrollbar } from \"../../resources/styles\";\nimport { loadVirtualizer } from \"../../resources/virtualizer\";\nimport { HomeAssistant } from \"../../types\";\nimport \"../ha-checkbox\";\nimport type { HaCheckbox } from \"../ha-checkbox\";\nimport \"../ha-svg-icon\";\nimport \"../search-input\";\nimport { filterData, sortData } from \"./sort-filter\";\n\ndeclare global {\n  // for fire event\n  interface HASSDomEvents {\n    \"selection-changed\": SelectionChangedEvent;\n    \"row-click\": RowClickedEvent;\n    \"sorting-changed\": SortingChangedEvent;\n  }\n}\n\nexport interface RowClickedEvent {\n  id: string;\n}\n\nexport interface SelectionChangedEvent {\n  value: string[];\n}\n\nexport interface SortingChangedEvent {\n  column: string;\n  direction: SortingDirection;\n}\n\nexport type SortingDirection = \"desc\" | \"asc\" | null;\n\nexport interface DataTableColumnContainer<T = any> {\n  [key: string]: DataTableColumnData<T>;\n}\n\nexport interface DataTableSortColumnData {\n  sortable?: boolean;\n  filterable?: boolean;\n  filterKey?: string;\n  valueColumn?: string;\n  direction?: SortingDirection;\n}\n\nexport interface DataTableColumnData<T = any> extends DataTableSortColumnData {\n  main?: boolean;\n  title: TemplateResult | string;\n  label?: TemplateResult | string;\n  type?: \"numeric\" | \"icon\" | \"icon-button\" | \"overflow-menu\" | \"flex\";\n  template?: (row: T) => TemplateResult | string | typeof nothing;\n  width?: string;\n  maxWidth?: string;\n  grows?: boolean;\n  forceLTR?: boolean;\n  hidden?: boolean;\n}\n\nexport type ClonedDataTableColumnData = Omit<DataTableColumnData, \"title\"> & {\n  title?: TemplateResult | string;\n};\n\nexport interface DataTableRowData {\n  [key: string]: any;\n  selectable?: boolean;\n}\n\nexport interface SortableColumnContainer {\n  [key: string]: ClonedDataTableColumnData;\n}\n\n@customElement(\"ha-data-table\")\nexport class HaDataTable extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ type: Object }) public columns: DataTableColumnContainer = {};\n\n  @property({ type: Array }) public data: DataTableRowData[] = [];\n\n  @property({ type: Boolean }) public selectable = false;\n\n  @property({ type: Boolean }) public clickable = false;\n\n  @property({ type: Boolean }) public hasFab = false;\n\n  /**\n   * Add an extra row at the bottom of the data table\n   * @type {TemplateResult}\n   */\n  @property({ attribute: false }) public appendRow?;\n\n  @property({ type: Boolean, attribute: \"auto-height\" })\n  public autoHeight = false;\n\n  @property({ type: String }) public id = \"id\";\n\n  @property({ type: String }) public noDataText?: string;\n\n  @property({ type: String }) public searchLabel?: string;\n\n  @property({ type: Boolean, attribute: \"no-label-float\" })\n  public noLabelFloat? = false;\n\n  @property({ type: String }) public filter = \"\";\n\n  @state() private _filterable = false;\n\n  @state() private _filter = \"\";\n\n  @state() private _sortColumn?: string;\n\n  @state() private _sortDirection: SortingDirection = null;\n\n  @state() private _filteredData: DataTableRowData[] = [];\n\n  @state() private _headerHeight = 0;\n\n  @query(\"slot[name='header']\") private _header!: HTMLSlotElement;\n\n  @state() private _items: DataTableRowData[] = [];\n\n  private _checkableRowsCount?: number;\n\n  private _checkedRows: string[] = [];\n\n  private _sortColumns: SortableColumnContainer = {};\n\n  private curRequest = 0;\n\n  // @ts-ignore\n  @restoreScroll(\".scroller\") private _savedScrollPos?: number;\n\n  private _debounceSearch = debounce(\n    (value: string) => {\n      this._filter = value;\n    },\n    100,\n    false\n  );\n\n  public clearSelection(): void {\n    this._checkedRows = [];\n    this._checkedRowsChanged();\n  }\n\n  public connectedCallback() {\n    super.connectedCallback();\n    if (this._items.length) {\n      // Force update of location of rows\n      this._items = [...this._items];\n    }\n  }\n\n  protected firstUpdated() {\n    this.updateComplete.then(() => this._calcTableHeight());\n  }\n\n  public willUpdate(properties: PropertyValues) {\n    super.willUpdate(properties);\n\n    if (!this.hasUpdated) {\n      loadVirtualizer();\n    }\n\n    if (properties.has(\"columns\")) {\n      this._filterable = Object.values(this.columns).some(\n        (column) => column.filterable\n      );\n\n      for (const columnId in this.columns) {\n        if (this.columns[columnId].direction) {\n          this._sortDirection = this.columns[columnId].direction!;\n          this._sortColumn = columnId;\n          break;\n        }\n      }\n\n      const clonedColumns: DataTableColumnContainer = deepClone(this.columns);\n      Object.values(clonedColumns).forEach(\n        (column: ClonedDataTableColumnData) => {\n          delete column.title;\n          delete column.template;\n        }\n      );\n\n      this._sortColumns = clonedColumns;\n    }\n\n    if (properties.has(\"filter\")) {\n      this._debounceSearch(this.filter);\n    }\n\n    if (properties.has(\"data\")) {\n      this._checkableRowsCount = this.data.filter(\n        (row) => row.selectable !== false\n      ).length;\n    }\n\n    if (\n      properties.has(\"data\") ||\n      properties.has(\"columns\") ||\n      properties.has(\"_filter\") ||\n      properties.has(\"_sortColumn\") ||\n      properties.has(\"_sortDirection\")\n    ) {\n      this._sortFilterData();\n    }\n  }\n\n  protected render() {\n    return html`\n      <div class=\"mdc-data-table\">\n        <slot name=\"header\" @slotchange=${this._calcTableHeight}>\n          ${this._filterable\n            ? html`\n                <div class=\"table-header\">\n                  <search-input\n                    .hass=${this.hass}\n                    @value-changed=${this._handleSearchChange}\n                    .label=${this.searchLabel}\n                    .noLabelFloat=${this.noLabelFloat}\n                  ></search-input>\n                </div>\n              `\n            : \"\"}\n        </slot>\n        <div\n          class=\"mdc-data-table__table ${classMap({\n            \"auto-height\": this.autoHeight,\n          })}\"\n          role=\"table\"\n          aria-rowcount=${this._filteredData.length + 1}\n          style=${styleMap({\n            height: this.autoHeight\n              ? `${(this._filteredData.length || 1) * 53 + 53}px`\n              : `calc(100% - ${this._headerHeight}px)`,\n          })}\n        >\n          <div class=\"mdc-data-table__header-row\" role=\"row\" aria-rowindex=\"1\">\n            ${this.selectable\n              ? html`\n                  <div\n                    class=\"mdc-data-table__header-cell mdc-data-table__header-cell--checkbox\"\n                    role=\"columnheader\"\n                  >\n                    <ha-checkbox\n                      class=\"mdc-data-table__row-checkbox\"\n                      @change=${this._handleHeaderRowCheckboxClick}\n                      .indeterminate=${this._checkedRows.length &&\n                      this._checkedRows.length !== this._checkableRowsCount}\n                      .checked=${this._checkedRows.length &&\n                      this._checkedRows.length === this._checkableRowsCount}\n                    >\n                    </ha-checkbox>\n                  </div>\n                `\n              : \"\"}\n            ${Object.entries(this.columns).map(([key, column]) => {\n              if (column.hidden) {\n                return \"\";\n              }\n              const sorted = key === this._sortColumn;\n              const classes = {\n                \"mdc-data-table__header-cell--numeric\":\n                  column.type === \"numeric\",\n                \"mdc-data-table__header-cell--icon\": column.type === \"icon\",\n                \"mdc-data-table__header-cell--icon-button\":\n                  column.type === \"icon-button\",\n                \"mdc-data-table__header-cell--overflow-menu\":\n                  column.type === \"overflow-menu\",\n                sortable: Boolean(column.sortable),\n                \"not-sorted\": Boolean(column.sortable && !sorted),\n                grows: Boolean(column.grows),\n              };\n              return html`\n                <div\n                  aria-label=${column.label}\n                  class=\"mdc-data-table__header-cell ${classMap(classes)}\"\n                  style=${column.width\n                    ? styleMap({\n                        [column.grows ? \"minWidth\" : \"width\"]: column.width,\n                        maxWidth: column.maxWidth || \"\",\n                      })\n                    : \"\"}\n                  role=\"columnheader\"\n                  aria-sort=${ifDefined(\n                    sorted\n                      ? this._sortDirection === \"desc\"\n                        ? \"descending\"\n                        : \"ascending\"\n                      : undefined\n                  )}\n                  @click=${this._handleHeaderClick}\n                  .columnId=${key}\n                >\n                  ${column.sortable\n                    ? html`\n                        <ha-svg-icon\n                          .path=${sorted && this._sortDirection === \"desc\"\n                            ? mdiArrowDown\n                            : mdiArrowUp}\n                        ></ha-svg-icon>\n                      `\n                    : \"\"}\n                  <span>${column.title}</span>\n                </div>\n              `;\n            })}\n          </div>\n          ${!this._filteredData.length\n            ? html`\n                <div class=\"mdc-data-table__content\">\n                  <div class=\"mdc-data-table__row\" role=\"row\">\n                    <div class=\"mdc-data-table__cell grows center\" role=\"cell\">\n                      ${this.noDataText ||\n                      this.hass.localize(\"ui.components.data-table.no-data\")}\n                    </div>\n                  </div>\n                </div>\n              `\n            : html`\n                <lit-virtualizer\n                  scroller\n                  class=\"mdc-data-table__content scroller ha-scrollbar\"\n                  @scroll=${this._saveScrollPos}\n                  .items=${this._items}\n                  .keyFunction=${this._keyFunction}\n                  .renderItem=${this._renderRow}\n                ></lit-virtualizer>\n              `}\n        </div>\n      </div>\n    `;\n  }\n\n  private _keyFunction = (row: DataTableRowData) => row[this.id] || row;\n\n  private _renderRow = (row: DataTableRowData, index: number) => {\n    // not sure how this happens...\n    if (!row) {\n      return nothing;\n    }\n    if (row.append) {\n      return html`<div class=\"mdc-data-table__row\">${row.content}</div>`;\n    }\n    if (row.empty) {\n      return html`<div class=\"mdc-data-table__row\"></div>`;\n    }\n    return html`\n      <div\n        aria-rowindex=${index + 2}\n        role=\"row\"\n        .rowId=${row[this.id]}\n        @click=${this._handleRowClick}\n        class=\"mdc-data-table__row ${classMap({\n          \"mdc-data-table__row--selected\": this._checkedRows.includes(\n            String(row[this.id])\n          ),\n          clickable: this.clickable,\n        })}\"\n        aria-selected=${ifDefined(\n          this._checkedRows.includes(String(row[this.id])) ? true : undefined\n        )}\n        .selectable=${row.selectable !== false}\n      >\n        ${this.selectable\n          ? html`\n              <div\n                class=\"mdc-data-table__cell mdc-data-table__cell--checkbox\"\n                role=\"cell\"\n              >\n                <ha-checkbox\n                  class=\"mdc-data-table__row-checkbox\"\n                  @change=${this._handleRowCheckboxClick}\n                  .rowId=${row[this.id]}\n                  .disabled=${row.selectable === false}\n                  .checked=${this._checkedRows.includes(String(row[this.id]))}\n                >\n                </ha-checkbox>\n              </div>\n            `\n          : \"\"}\n        ${Object.entries(this.columns).map(([key, column]) => {\n          if (column.hidden) {\n            return \"\";\n          }\n          return html`\n            <div\n              role=${column.main ? \"rowheader\" : \"cell\"}\n              class=\"mdc-data-table__cell ${classMap({\n                \"mdc-data-table__cell--flex\": column.type === \"flex\",\n                \"mdc-data-table__cell--numeric\": column.type === \"numeric\",\n                \"mdc-data-table__cell--icon\": column.type === \"icon\",\n                \"mdc-data-table__cell--icon-button\":\n                  column.type === \"icon-button\",\n                \"mdc-data-table__cell--overflow-menu\":\n                  column.type === \"overflow-menu\",\n                grows: Boolean(column.grows),\n                forceLTR: Boolean(column.forceLTR),\n              })}\"\n              style=${column.width\n                ? styleMap({\n                    [column.grows ? \"minWidth\" : \"width\"]: column.width,\n                    maxWidth: column.maxWidth ? column.maxWidth : \"\",\n                  })\n                : \"\"}\n            >\n              ${column.template ? column.template(row) : row[key]}\n            </div>\n          `;\n        })}\n      </div>\n    `;\n  };\n\n  private async _sortFilterData() {\n    const startTime = new Date().getTime();\n    this.curRequest++;\n    const curRequest = this.curRequest;\n\n    let filteredData = this.data;\n    if (this._filter) {\n      filteredData = await this._memFilterData(\n        this.data,\n        this._sortColumns,\n        this._filter\n      );\n    }\n\n    const prom = this._sortColumn\n      ? sortData(\n          filteredData,\n          this._sortColumns[this._sortColumn],\n          this._sortDirection,\n          this._sortColumn,\n          this.hass.locale.language\n        )\n      : filteredData;\n\n    const [data] = await Promise.all([prom, nextRender]);\n\n    const curTime = new Date().getTime();\n    const elapsed = curTime - startTime;\n\n    if (elapsed < 100) {\n      await new Promise((resolve) => {\n        setTimeout(resolve, 100 - elapsed);\n      });\n    }\n    if (this.curRequest !== curRequest) {\n      return;\n    }\n\n    if (this.appendRow || this.hasFab) {\n      const items = [...data];\n\n      if (this.appendRow) {\n        items.push({ append: true, content: this.appendRow });\n      }\n\n      if (this.hasFab) {\n        items.push({ empty: true });\n      }\n      this._items = items;\n    } else {\n      this._items = data;\n    }\n    this._filteredData = data;\n  }\n\n  private _memFilterData = memoizeOne(\n    (\n      data: DataTableRowData[],\n      columns: SortableColumnContainer,\n      filter: string\n    ): Promise<DataTableRowData[]> => filterData(data, columns, filter)\n  );\n\n  private _handleHeaderClick(ev: Event) {\n    const columnId = (ev.currentTarget as any).columnId;\n    if (!this.columns[columnId].sortable) {\n      return;\n    }\n    if (!this._sortDirection || this._sortColumn !== columnId) {\n      this._sortDirection = \"asc\";\n    } else if (this._sortDirection === \"asc\") {\n      this._sortDirection = \"desc\";\n    } else {\n      this._sortDirection = null;\n    }\n\n    this._sortColumn = this._sortDirection === null ? undefined : columnId;\n\n    fireEvent(this, \"sorting-changed\", {\n      column: columnId,\n      direction: this._sortDirection,\n    });\n  }\n\n  private _handleHeaderRowCheckboxClick(ev: Event) {\n    const checkbox = ev.target as HaCheckbox;\n    if (checkbox.checked) {\n      this._checkedRows = this._filteredData\n        .filter((data) => data.selectable !== false)\n        .map((data) => data[this.id]);\n      this._checkedRowsChanged();\n    } else {\n      this._checkedRows = [];\n      this._checkedRowsChanged();\n    }\n  }\n\n  private _handleRowCheckboxClick = (ev: Event) => {\n    const checkbox = ev.currentTarget as HaCheckbox;\n    const rowId = (checkbox as any).rowId;\n\n    if (checkbox.checked) {\n      if (this._checkedRows.includes(rowId)) {\n        return;\n      }\n      this._checkedRows = [...this._checkedRows, rowId];\n    } else {\n      this._checkedRows = this._checkedRows.filter((row) => row !== rowId);\n    }\n    this._checkedRowsChanged();\n  };\n\n  private _handleRowClick = (ev: Event) => {\n    const target = ev.target as HTMLElement;\n    if ([\"HA-CHECKBOX\", \"MWC-BUTTON\"].includes(target.tagName)) {\n      return;\n    }\n    const rowId = (ev.currentTarget as any).rowId;\n    fireEvent(this, \"row-click\", { id: rowId }, { bubbles: false });\n  };\n\n  private _checkedRowsChanged() {\n    // force scroller to update, change it's items\n    if (this._items.length) {\n      this._items = [...this._items];\n    }\n    fireEvent(this, \"selection-changed\", {\n      value: this._checkedRows,\n    });\n  }\n\n  private _handleSearchChange(ev: CustomEvent): void {\n    if (this.filter) {\n      return;\n    }\n    this._debounceSearch(ev.detail.value);\n  }\n\n  private async _calcTableHeight() {\n    if (this.autoHeight) {\n      return;\n    }\n    await this.updateComplete;\n    this._headerHeight = this._header.clientHeight;\n  }\n\n  @eventOptions({ passive: true })\n  private _saveScrollPos(e: Event) {\n    this._savedScrollPos = (e.target as HTMLDivElement).scrollTop;\n  }\n\n  static get styles(): CSSResultGroup {\n    return [\n      haStyleScrollbar,\n      css`\n        /* default mdc styles, colors changed, without checkbox styles */\n        :host {\n          height: 100%;\n        }\n        .mdc-data-table__content {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.25rem;\n          font-weight: 400;\n          letter-spacing: 0.0178571429em;\n          text-decoration: inherit;\n          text-transform: inherit;\n        }\n\n        .mdc-data-table {\n          background-color: var(--data-table-background-color);\n          border-radius: 4px;\n          border-width: 1px;\n          border-style: solid;\n          border-color: var(--divider-color);\n          display: inline-flex;\n          flex-direction: column;\n          box-sizing: border-box;\n          overflow: hidden;\n        }\n\n        .mdc-data-table__row--selected {\n          background-color: rgba(var(--rgb-primary-color), 0.04);\n        }\n\n        .mdc-data-table__row {\n          display: flex;\n          width: 100%;\n          height: 52px;\n        }\n\n        .mdc-data-table__row ~ .mdc-data-table__row {\n          border-top: 1px solid var(--divider-color);\n        }\n\n        .mdc-data-table__row.clickable:not(\n            .mdc-data-table__row--selected\n          ):hover {\n          background-color: rgba(var(--rgb-primary-text-color), 0.04);\n        }\n\n        .mdc-data-table__header-cell {\n          color: var(--primary-text-color);\n        }\n\n        .mdc-data-table__cell {\n          color: var(--primary-text-color);\n        }\n\n        .mdc-data-table__header-row {\n          height: 56px;\n          display: flex;\n          width: 100%;\n          border-bottom: 1px solid var(--divider-color);\n          overflow-x: auto;\n        }\n\n        .mdc-data-table__header-row::-webkit-scrollbar {\n          display: none;\n        }\n\n        .mdc-data-table__cell,\n        .mdc-data-table__header-cell {\n          padding-right: 16px;\n          padding-left: 16px;\n          align-self: center;\n          overflow: hidden;\n          text-overflow: ellipsis;\n          flex-shrink: 0;\n          box-sizing: border-box;\n        }\n\n        .mdc-data-table__cell.mdc-data-table__cell--flex {\n          display: flex;\n          overflow: initial;\n        }\n\n        .mdc-data-table__cell.mdc-data-table__cell--icon {\n          overflow: initial;\n        }\n\n        .mdc-data-table__header-cell--checkbox,\n        .mdc-data-table__cell--checkbox {\n          /* @noflip */\n          padding-left: 16px;\n          /* @noflip */\n          padding-right: 0;\n          width: 60px;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell--checkbox,\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--checkbox {\n          /* @noflip */\n          padding-left: 0;\n          /* @noflip */\n          padding-right: 16px;\n        }\n\n        .mdc-data-table__table {\n          height: 100%;\n          width: 100%;\n          border: 0;\n          white-space: nowrap;\n        }\n\n        .mdc-data-table__cell {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.25rem;\n          font-weight: 400;\n          letter-spacing: 0.0178571429em;\n          text-decoration: inherit;\n          text-transform: inherit;\n        }\n\n        .mdc-data-table__cell a {\n          color: inherit;\n          text-decoration: none;\n        }\n\n        .mdc-data-table__cell--numeric {\n          text-align: right;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--numeric {\n          /* @noflip */\n          text-align: left;\n        }\n\n        .mdc-data-table__cell--icon {\n          color: var(--secondary-text-color);\n          text-align: center;\n        }\n\n        .mdc-data-table__header-cell--icon,\n        .mdc-data-table__cell--icon {\n          width: 54px;\n        }\n\n        .mdc-data-table__cell--icon img {\n          width: 24px;\n          height: 24px;\n        }\n\n        .mdc-data-table__header-cell.mdc-data-table__header-cell--icon {\n          text-align: center;\n        }\n\n        .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:hover,\n        .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:not(\n            .not-sorted\n          ) {\n          text-align: left;\n        }\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:hover,\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell.sortable.mdc-data-table__header-cell--icon:not(\n            .not-sorted\n          ) {\n          text-align: right;\n        }\n\n        .mdc-data-table__cell--icon:first-child ha-icon,\n        .mdc-data-table__cell--icon:first-child img,\n        .mdc-data-table__cell--icon:first-child ha-state-icon,\n        .mdc-data-table__cell--icon:first-child ha-svg-icon {\n          margin-left: 8px;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--icon:first-child ha-icon,\n        :host([dir=\"rtl\"])\n          .mdc-data-table__cell--icon:first-child\n          ha-state-icon,\n        :host([dir=\"rtl\"])\n          .mdc-data-table__cell--icon:first-child\n          ha-svg-icon\n          :host([dir=\"rtl\"])\n          .mdc-data-table__cell--icon:first-child\n          img {\n          margin-left: auto;\n          margin-right: 8px;\n        }\n\n        .mdc-data-table__cell--icon:first-child state-badge {\n          margin-right: -8px;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--icon:first-child state-badge {\n          margin-right: auto;\n          margin-left: -8px;\n        }\n\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__header-cell--overflow-menu,\n        .mdc-data-table__header-cell--icon-button,\n        .mdc-data-table__cell--icon-button {\n          padding: 8px;\n        }\n\n        .mdc-data-table__header-cell--icon-button,\n        .mdc-data-table__cell--icon-button {\n          width: 56px;\n        }\n\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__cell--icon-button {\n          color: var(--secondary-text-color);\n          text-overflow: clip;\n        }\n\n        .mdc-data-table__header-cell--icon-button:first-child,\n        .mdc-data-table__cell--icon-button:first-child,\n        .mdc-data-table__header-cell--icon-button:last-child,\n        .mdc-data-table__cell--icon-button:last-child {\n          width: 64px;\n        }\n\n        .mdc-data-table__cell--overflow-menu:first-child,\n        .mdc-data-table__header-cell--overflow-menu:first-child,\n        .mdc-data-table__header-cell--icon-button:first-child,\n        .mdc-data-table__cell--icon-button:first-child {\n          padding-left: 16px;\n        }\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell--overflow-menu:first-child,\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--overflow-menu:first-child,\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell--overflow-menu:first-child,\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--overflow-menu:first-child {\n          padding-left: 8px;\n          padding-right: 16px;\n        }\n\n        .mdc-data-table__cell--overflow-menu:last-child,\n        .mdc-data-table__header-cell--overflow-menu:last-child,\n        .mdc-data-table__header-cell--icon-button:last-child,\n        .mdc-data-table__cell--icon-button:last-child {\n          padding-right: 16px;\n        }\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell--overflow-menu:last-child,\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--overflow-menu:last-child,\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell--icon-button:last-child,\n        :host([dir=\"rtl\"]) .mdc-data-table__cell--icon-button:last-child {\n          padding-right: 8px;\n          padding-left: 16px;\n        }\n        .mdc-data-table__cell--overflow-menu,\n        .mdc-data-table__header-cell--overflow-menu {\n          overflow: initial;\n        }\n        .mdc-data-table__cell--icon-button a {\n          color: var(--secondary-text-color);\n        }\n\n        .mdc-data-table__header-cell {\n          font-family: Roboto, sans-serif;\n          -moz-osx-font-smoothing: grayscale;\n          -webkit-font-smoothing: antialiased;\n          font-size: 0.875rem;\n          line-height: 1.375rem;\n          font-weight: 500;\n          letter-spacing: 0.0071428571em;\n          text-decoration: inherit;\n          text-transform: inherit;\n          text-align: left;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell {\n          /* @noflip */\n          text-align: right;\n        }\n\n        .mdc-data-table__header-cell--numeric {\n          text-align: right;\n        }\n        .mdc-data-table__header-cell--numeric.sortable:hover,\n        .mdc-data-table__header-cell--numeric.sortable:not(.not-sorted) {\n          text-align: left;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell--numeric {\n          /* @noflip */\n          text-align: left;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell--numeric.sortable:hover,\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell--numeric.sortable:not(.not-sorted) {\n          text-align: right;\n        }\n\n        /* custom from here */\n\n        :host {\n          display: block;\n        }\n\n        .mdc-data-table {\n          display: block;\n          border-width: var(--data-table-border-width, 1px);\n          height: 100%;\n        }\n        .mdc-data-table__header-cell {\n          overflow: hidden;\n          position: relative;\n        }\n        .mdc-data-table__header-cell span {\n          position: relative;\n          left: 0px;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell span {\n          left: auto;\n          right: 0px;\n        }\n\n        .mdc-data-table__header-cell.sortable {\n          cursor: pointer;\n        }\n        .mdc-data-table__header-cell > * {\n          transition: left 0.2s ease;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell > * {\n          transition: right 0.2s ease;\n        }\n        .mdc-data-table__header-cell ha-svg-icon {\n          top: -3px;\n          position: absolute;\n        }\n        .mdc-data-table__header-cell.not-sorted ha-svg-icon {\n          left: -20px;\n        }\n        :host([dir=\"rtl\"]) .mdc-data-table__header-cell.not-sorted ha-svg-icon {\n          right: -20px;\n        }\n        .mdc-data-table__header-cell.sortable:not(.not-sorted) span,\n        .mdc-data-table__header-cell.sortable.not-sorted:hover span {\n          left: 24px;\n        }\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell.sortable:not(.not-sorted)\n          span,\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell.sortable.not-sorted:hover\n          span {\n          left: auto;\n          right: 24px;\n        }\n        .mdc-data-table__header-cell.sortable:not(.not-sorted) ha-svg-icon,\n        .mdc-data-table__header-cell.sortable:hover.not-sorted ha-svg-icon {\n          left: 12px;\n        }\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell.sortable:not(.not-sorted)\n          ha-svg-icon,\n        :host([dir=\"rtl\"])\n          .mdc-data-table__header-cell.sortable:hover.not-sorted\n          ha-svg-icon {\n          left: auto;\n          right: 12px;\n        }\n        .table-header {\n          border-bottom: 1px solid var(--divider-color);\n        }\n        search-input {\n          display: block;\n          flex: 1;\n        }\n        slot[name=\"header\"] {\n          display: block;\n        }\n        .center {\n          text-align: center;\n        }\n        .secondary {\n          color: var(--secondary-text-color);\n        }\n        .scroller {\n          height: calc(100% - 57px);\n          overflow: overlay !important;\n        }\n\n        .mdc-data-table__table.auto-height .scroller {\n          overflow-y: hidden !important;\n        }\n        .grows {\n          flex-grow: 1;\n          flex-shrink: 1;\n        }\n        .forceLTR {\n          direction: ltr;\n        }\n        .clickable {\n          cursor: pointer;\n        }\n        lit-virtualizer {\n          contain: size layout !important;\n          overscroll-behavior: contain;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"ha-data-table\": HaDataTable;\n  }\n}\n",
         "import { LitElement, html, TemplateResult } from \"lit\";\nimport { customElement, property } from \"lit/decorators\";\nimport memoizeOne from \"memoize-one\";\nimport { mdiDelete } from \"@mdi/js\";\nimport { computeRTLDirection } from \"@ha/common/util/compute_rtl\";\nimport \"@ha/components/data-table/ha-data-table\";\nimport type {\n  DataTableColumnContainer,\n  DataTableRowData,\n} from \"@ha/components/data-table/ha-data-table\";\nimport type { HomeAssistant, Route } from \"@ha/types\";\nimport { showConfirmationDialog } from \"@ha/dialogs/generic/show-dialog-box\";\nimport { navigate } from \"@ha/common/navigate\";\nimport { LCN, LcnDeviceConfig, deleteDevice, LcnAddress } from \"types/lcn\";\nimport \"@ha/components/ha-icon-button\";\nimport { loadLCNCreateDeviceDialog } from \"./dialogs/show-dialog-create-device\";\n\nexport type DeviceRowData = LcnDeviceConfig & {\n  segment_id: number;\n  address_id: number;\n  type: string;\n  delete: LcnDeviceConfig;\n};\n\n@customElement(\"lcn-devices-data-table\")\nexport class LCNDevicesDataTable extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ attribute: false }) public narrow!: boolean;\n\n  @property({ attribute: false }) public route!: Route;\n\n  @property({ attribute: false }) public devices: LcnDeviceConfig[] = [];\n\n  private _devices = memoizeOne((devices: LcnDeviceConfig[]) => {\n    const deviceRowData: DeviceRowData[] = devices.map((device) => ({\n      ...device,\n      segment_id: device.address[0],\n      address_id: device.address[1],\n      type: device.address[2] ? this.lcn.localize(\"group\") : this.lcn.localize(\"module\"),\n      delete: device,\n    }));\n    return deviceRowData;\n  });\n\n  private _columns = memoizeOne(\n    (narrow: boolean): DataTableColumnContainer =>\n      narrow\n        ? {\n            name: {\n              title: this.lcn.localize(\"name\"),\n              sortable: true,\n              direction: \"asc\",\n              grows: true,\n            },\n            delete: {\n              title: \"\",\n              sortable: false,\n              width: \"80px\",\n              template: (device: LcnDeviceConfig) => {\n                const handler = (ev) => this._onDeviceDelete(ev, device);\n                return html`\n                  <ha-icon-button\n                    .label=${this.lcn.localize(\"dashboard-devices-table-delete\")}\n                    .path=${mdiDelete}\n                    @click=${handler}\n                  ></ha-icon-button>\n                `;\n              },\n            },\n          }\n        : {\n            name: {\n              title: this.lcn.localize(\"name\"),\n              sortable: true,\n              direction: \"asc\",\n              grows: true,\n              width: \"40%\",\n            },\n            segment_id: {\n              title: this.lcn.localize(\"segment\"),\n              sortable: true,\n              grows: false,\n              width: \"15%\",\n            },\n            address_id: {\n              title: this.lcn.localize(\"id\"),\n              sortable: true,\n              grows: false,\n              width: \"15%\",\n            },\n            type: {\n              title: this.lcn.localize(\"type\"),\n              sortable: true,\n              grows: false,\n              width: \"15%\",\n            },\n            delete: {\n              title: \"\",\n              sortable: false,\n              width: \"80px\",\n              template: (device: LcnDeviceConfig) => {\n                const handler = (ev) => this._onDeviceDelete(ev, device);\n                return html`\n                  <ha-icon-button\n                    .label=${this.lcn.localize(\"dashboard-devices-table-delete\")}\n                    .path=${mdiDelete}\n                    @click=${handler}\n                  ></ha-icon-button>\n                `;\n              },\n            },\n          },\n  );\n\n  protected firstUpdated(changedProperties) {\n    super.firstUpdated(changedProperties);\n    loadLCNCreateDeviceDialog();\n  }\n\n  protected render(): TemplateResult {\n    return html`\n      <ha-data-table\n        .hass=${this.hass}\n        .columns=${this._columns(this.narrow)}\n        .data=${this._devices(this.devices) as DataTableRowData[]}\n        .id=${\"address\"}\n        .noDataText=${this.lcn.localize(\"dashboard-devices-table-no-data\")}\n        .dir=${computeRTLDirection(this.hass)}\n        auto-height\n        clickable\n        @row-click=${this._rowClicked}\n      ></ha-data-table>\n    `;\n  }\n\n  private _rowClicked(ev: CustomEvent) {\n    this.lcn.address = ev.detail.id;\n    this._openDevice();\n  }\n\n  private _onDeviceDelete(ev, device: LcnDeviceConfig) {\n    ev.stopPropagation();\n    this._deleteDevice(device.address);\n  }\n\n  private _dispatchConfigurationChangedEvent() {\n    this.dispatchEvent(\n      new CustomEvent(\"lcn-config-changed\", {\n        bubbles: true,\n        composed: true,\n      }),\n    );\n  }\n\n  private _openDevice() {\n    navigate(\"/lcn/entities\");\n  }\n\n  private async _deleteDevice(address: LcnAddress) {\n    const device_to_delete = this.devices.find(\n      (device) =>\n        device.address[0] === address[0] &&\n        device.address[1] === address[1] &&\n        device.address[2] === address[2],\n    )!;\n\n    if (\n      !(await showConfirmationDialog(this, {\n        title: `\n          ${\n            device_to_delete.address[2]\n              ? this.lcn.localize(\"dashboard-devices-dialog-delete-group-title\")\n              : this.lcn.localize(\"dashboard-devices-dialog-delete-module-title\")\n          }`,\n        text: html`${this.lcn.localize(\"dashboard-devices-dialog-delete-text\")}\n          ${device_to_delete.name ? `'${device_to_delete.name}'` : \"\"}\n          (${device_to_delete.address[2]\n            ? this.lcn.localize(\"group\")\n            : this.lcn.localize(\"module\")}:\n          ${this.lcn.localize(\"segment\")} ${device_to_delete.address[0]}, ${this.lcn.localize(\"id\")}\n          ${device_to_delete.address[1]})\n          <br />\n          ${this.lcn.localize(\"dashboard-devices-dialog-delete-warning\")}`,\n      }))\n    ) {\n      return;\n    }\n\n    await deleteDevice(this.hass, this.lcn.host.id, device_to_delete);\n    this._dispatchConfigurationChangedEvent();\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-devices-data-table\": LCNDevicesDataTable;\n  }\n}\n",
-        "import { haStyle } from \"@ha/resources/styles\";\nimport \"@material/mwc-button\";\nimport \"@polymer/paper-dropdown-menu/paper-dropdown-menu\";\nimport \"@ha/components/ha-fab\";\nimport \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, PropertyValues, TemplateResult, CSSResultGroup } from \"lit\";\nimport { customElement, property, query, state } from \"lit/decorators\";\nimport { mdiPlus } from \"@mdi/js\";\nimport type { HomeAssistant, Route } from \"@ha/types\";\nimport { showAlertDialog } from \"@ha/dialogs/generic/show-dialog-box\";\nimport \"@ha/layouts/hass-tabs-subpage\";\nimport type { PageNavigation } from \"@ha/layouts/hass-tabs-subpage\";\nimport \"@ha/panels/config/ha-config-section\";\nimport \"@ha/layouts/hass-loading-screen\";\nimport \"@ha/components/ha-card\";\nimport \"@ha/components/ha-svg-icon\";\nimport {\n  LCN,\n  fetchHosts,\n  fetchDevices,\n  scanDevices,\n  addDevice,\n  LcnHost,\n  LcnDeviceConfig,\n} from \"types/lcn\";\nimport { ProgressDialog } from \"./dialogs/progress-dialog\";\nimport {\n  loadLCNCreateDeviceDialog,\n  showLCNCreateDeviceDialog,\n} from \"./dialogs/show-dialog-create-device\";\nimport { loadProgressDialog, showProgressDialog } from \"./dialogs/show-dialog-progress\";\nimport \"./lcn-devices-data-table\";\n\n@customElement(\"lcn-config-dashboard\")\nexport class LCNConfigDashboard extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ type: Boolean }) public narrow!: boolean;\n\n  @property({ attribute: false }) public route!: Route;\n\n  @property({ type: Array, reflect: false }) public tabs: PageNavigation[] = [];\n\n  @state() private _hosts: LcnHost[] = [];\n\n  @state() private _deviceConfigs: LcnDeviceConfig[] = [];\n\n  @query(\"#host-select\") private _hostsSelect!: HaSelect;\n\n  protected async firstUpdated(changedProperties: PropertyValues): Promise<void> {\n    super.firstUpdated(changedProperties);\n    await this._fetchHosts();\n    loadProgressDialog();\n    loadLCNCreateDeviceDialog();\n\n    this._hostsSelect.value = this.lcn.host.id; // invokes this._fetchDevices()\n\n    this.addEventListener(\"lcn-config-changed\", async () => {\n      this._fetchDevices(this.lcn.host);\n    });\n  }\n\n  protected render(): TemplateResult {\n    if (!(this.hass && this.lcn)) {\n      return html` <hass-loading-screen></hass-loading-screen> `;\n    }\n    return html`\n      <hass-tabs-subpage\n        .hass=${this.hass}\n        .narrow=${this.narrow}\n        back-path=\"/lcn\"\n        .route=${this.route}\n        .tabs=${this.tabs}\n      >\n        <ha-config-section .narrow=${this.narrow}>\n          <span slot=\"header\"> ${this.lcn.localize(\"dashboard-devices-title\")} </span>\n\n          <span slot=\"introduction\"> ${this.lcn.localize(\"dashboard-devices-introduction\")} </span>\n\n          <div id=\"box\">\n            <ha-select\n              id=\"host-select\"\n              .label=${this.lcn.localize(\"dashboard-devices-hosts\")}\n              .value=${this.lcn.host.id}\n              fixedMenuPosition\n              @selected=${this._hostChanged}\n            >\n              ${this._hosts.map(\n                (host) => html` <ha-list-item .value=${host.id}> ${host.name} </ha-list-item> `,\n              )}\n            </ha-select>\n\n            <mwc-button id=\"scan_devices\" raised @click=${this._scanDevices}>\n              ${this.lcn.localize(\"dashboard-devices-scan\")}\n            </mwc-button>\n          </div>\n\n          <ha-card\n            header=\"${this.lcn.localize(\"dashboard-devices-for-host\")}: ${this.lcn.host.name}\"\n          >\n            <lcn-devices-data-table\n              .hass=${this.hass}\n              .lcn=${this.lcn}\n              .devices=${this._deviceConfigs}\n              .narrow=${this.narrow}\n            ></lcn-devices-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot=\"fab\"\n          @click=${this._addDevice}\n          .label=${this.lcn.localize(\"dashboard-devices-add\")}\n          extended\n        >\n          <ha-svg-icon slot=\"icon\" .path=${mdiPlus}></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    `;\n  }\n\n  private _hostChanged(ev: CustomEvent) {\n    const target = ev.target as HaSelect;\n    const host: LcnHost = this._hosts.find((el) => el.id === target.value)!;\n    this.lcn.host = host;\n    this._fetchDevices(this.lcn.host);\n  }\n\n  private async _fetchHosts() {\n    this._hosts = await fetchHosts(this.hass!);\n  }\n\n  private async _fetchDevices(host: LcnHost) {\n    this._deviceConfigs = await fetchDevices(this.hass!, host.id);\n  }\n\n  private async _scanDevices() {\n    const dialog: () => ProgressDialog | undefined = showProgressDialog(this, {\n      title: this.lcn.localize(\"dashboard-dialog-scan-devices-title\"),\n      text: this.lcn.localize(\"dashboard-dialog-scan-devices-text\"),\n    });\n\n    this._deviceConfigs = await scanDevices(this.hass!, this.lcn.host.id);\n    await dialog()!.closeDialog();\n  }\n\n  private _addDevice() {\n    showLCNCreateDeviceDialog(this, {\n      lcn: this.lcn,\n      createDevice: (deviceParams) => this._createDevice(deviceParams),\n    });\n  }\n\n  private async _createDevice(deviceParams: Partial<LcnDeviceConfig>) {\n    const dialog: () => ProgressDialog | undefined = showProgressDialog(this, {\n      title: this.lcn.localize(\"dashboard-devices-dialog-request-info-title\"),\n      text: html`\n        ${this.lcn.localize(\"dashboard-devices-dialog-request-info-text\")}\n        <br />\n        ${this.lcn.localize(\"dashboard-devices-dialog-request-info-hint\")}\n      `,\n    });\n\n    if (!(await addDevice(this.hass, this.lcn.host.id, deviceParams))) {\n      dialog()!.closeDialog();\n      await showAlertDialog(this, {\n        title: this.lcn.localize(\"dashboard-devices-dialog-add-alert-title\"),\n        text: html`${this.lcn.localize(\"dashboard-devices-dialog-add-alert-text\")}\n          (${deviceParams.address![2] ? this.lcn.localize(\"group\") : this.lcn.localize(\"module\")}:\n          ${this.lcn.localize(\"segment\")} ${deviceParams.address![0]}, ${this.lcn.localize(\"id\")}\n          ${deviceParams.address![1]})\n          <br />\n          ${this.lcn.localize(\"dashboard-devices-dialog-add-alert-hint\")}`,\n      });\n      return;\n    }\n    dialog()!.closeDialog();\n    this._fetchDevices(this.lcn.host);\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyle,\n      css`\n        #box {\n          display: flex;\n          justify-content: space-between;\n        }\n        #host-select {\n          width: 40%;\n          display: inline-block;\n        }\n        #scan-devices {\n          display: inline-block;\n          margin-top: 20px;\n          justify-content: center;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-dashboard\": LCNConfigDashboard;\n  }\n}\n"
+        "import { haStyle } from \"@ha/resources/styles\";\nimport \"@material/mwc-button\";\nimport \"@polymer/paper-dropdown-menu/paper-dropdown-menu\";\nimport \"@ha/components/ha-fab\";\nimport \"@ha/components/ha-list-item\";\nimport \"@ha/components/ha-select\";\nimport type { HaSelect } from \"@ha/components/ha-select\";\nimport { css, html, LitElement, PropertyValues, TemplateResult, CSSResultGroup } from \"lit\";\nimport { customElement, property, state } from \"lit/decorators\";\nimport { mdiPlus } from \"@mdi/js\";\nimport type { HomeAssistant, Route } from \"@ha/types\";\nimport { showAlertDialog } from \"@ha/dialogs/generic/show-dialog-box\";\nimport \"@ha/layouts/hass-tabs-subpage\";\nimport type { PageNavigation } from \"@ha/layouts/hass-tabs-subpage\";\nimport \"@ha/panels/config/ha-config-section\";\nimport \"@ha/layouts/hass-loading-screen\";\nimport \"@ha/components/ha-card\";\nimport \"@ha/components/ha-svg-icon\";\nimport { LCN, fetchDevices, scanDevices, addDevice, LcnHost, LcnDeviceConfig } from \"types/lcn\";\nimport { ProgressDialog } from \"./dialogs/progress-dialog\";\nimport {\n  loadLCNCreateDeviceDialog,\n  showLCNCreateDeviceDialog,\n} from \"./dialogs/show-dialog-create-device\";\nimport { loadProgressDialog, showProgressDialog } from \"./dialogs/show-dialog-progress\";\nimport \"./lcn-devices-data-table\";\n\n@customElement(\"lcn-config-dashboard\")\nexport class LCNConfigDashboard extends LitElement {\n  @property({ attribute: false }) public hass!: HomeAssistant;\n\n  @property({ attribute: false }) public lcn!: LCN;\n\n  @property({ type: Boolean }) public narrow!: boolean;\n\n  @property({ attribute: false }) public route!: Route;\n\n  @property({ attribute: false }) public hosts!: LcnHost[];\n\n  @property({ type: Array, reflect: false }) public tabs: PageNavigation[] = [];\n\n  @state() private _deviceConfigs: LcnDeviceConfig[] = [];\n\n  protected async firstUpdated(changedProperties: PropertyValues): Promise<void> {\n    super.firstUpdated(changedProperties);\n    loadProgressDialog();\n    loadLCNCreateDeviceDialog();\n\n    this.addEventListener(\"lcn-config-changed\", async () => {\n      this._fetchDevices(this.lcn.host);\n    });\n  }\n\n  protected render(): TemplateResult {\n    if (!(this.hass && this.lcn && this.hosts)) {\n      return html` <hass-loading-screen></hass-loading-screen> `;\n    }\n    return html`\n      <hass-tabs-subpage\n        .hass=${this.hass}\n        .narrow=${this.narrow}\n        .route=${this.route}\n        .tabs=${this.tabs}\n        main-page\n      >\n        <span slot=\"header\"> ${this.lcn.localize(\"dashboard-devices-title\")} </span>\n        <ha-config-section .narrow=${this.narrow}>\n          <span slot=\"introduction\"> ${this.renderIntro()} </span>\n\n          <div id=\"box\">\n            <ha-select\n              id=\"host-select\"\n              .label=${this.lcn.localize(\"dashboard-devices-hosts\")}\n              .value=${this.lcn.host.id}\n              fixedMenuPosition\n              @selected=${this._hostChanged}\n            >\n              ${this.hosts.map(\n                (host) => html` <ha-list-item .value=${host.id}> ${host.name} </ha-list-item> `,\n              )}\n            </ha-select>\n\n            <mwc-button id=\"scan_devices\" raised @click=${this._scanDevices}>\n              ${this.lcn.localize(\"dashboard-devices-scan\")}\n            </mwc-button>\n          </div>\n\n          <ha-card\n            header=\"${this.lcn.localize(\"dashboard-devices-for-host\")}: ${this.lcn.host.name}\"\n          >\n            <lcn-devices-data-table\n              .hass=${this.hass}\n              .lcn=${this.lcn}\n              .devices=${this._deviceConfigs}\n              .narrow=${this.narrow}\n            ></lcn-devices-data-table>\n          </ha-card>\n        </ha-config-section>\n        <ha-fab\n          slot=\"fab\"\n          @click=${this._addDevice}\n          .label=${this.lcn.localize(\"dashboard-devices-add\")}\n          extended\n        >\n          <ha-svg-icon slot=\"icon\" .path=${mdiPlus}></ha-svg-icon>\n        </ha-fab>\n      </hass-tabs-subpage>\n    `;\n  }\n\n  private renderIntro(): TemplateResult {\n    return html`\n      <h2>${this.lcn.localize(\"dashboard-devices-introduction\")}</h2>\n      ${this.lcn.localize(\"dashboard-devices-introduction-help-1\")} <br />\n      <details>\n        <summary>${this.lcn.localize(\"more-help\")}</summary>\n        <ul>\n          <li>${this.lcn.localize(\"dashboard-devices-introduction-help-2\")}</li>\n          <li>${this.lcn.localize(\"dashboard-devices-introduction-help-3\")}</li>\n          <li>${this.lcn.localize(\"dashboard-devices-introduction-help-4\")}</li>\n          <li>${this.lcn.localize(\"dashboard-devices-introduction-help-5\")}</li>\n        </ul>\n      </details>\n    `;\n  }\n\n  private async _hostChanged(ev: CustomEvent) {\n    const target = ev.target as HaSelect;\n    const host: LcnHost = this.hosts.find((el) => el.id === target.value)!;\n    this.lcn.host = host;\n    await this._fetchDevices(this.lcn.host);\n  }\n\n  private async _fetchDevices(host: LcnHost) {\n    this._deviceConfigs = await fetchDevices(this.hass!, host.id);\n  }\n\n  private async _scanDevices() {\n    const dialog: () => ProgressDialog | undefined = showProgressDialog(this, {\n      title: this.lcn.localize(\"dashboard-dialog-scan-devices-title\"),\n      text: this.lcn.localize(\"dashboard-dialog-scan-devices-text\"),\n    });\n\n    this._deviceConfigs = await scanDevices(this.hass!, this.lcn.host.id);\n    await dialog()!.closeDialog();\n  }\n\n  private _addDevice() {\n    showLCNCreateDeviceDialog(this, {\n      lcn: this.lcn,\n      createDevice: (deviceParams) => this._createDevice(deviceParams),\n    });\n  }\n\n  private async _createDevice(deviceParams: Partial<LcnDeviceConfig>) {\n    const dialog: () => ProgressDialog | undefined = showProgressDialog(this, {\n      title: this.lcn.localize(\"dashboard-devices-dialog-request-info-title\"),\n      text: html`\n        ${this.lcn.localize(\"dashboard-devices-dialog-request-info-text\")}\n        <br />\n        ${this.lcn.localize(\"dashboard-devices-dialog-request-info-hint\")}\n      `,\n    });\n\n    if (!(await addDevice(this.hass, this.lcn.host.id, deviceParams))) {\n      dialog()!.closeDialog();\n      await showAlertDialog(this, {\n        title: this.lcn.localize(\"dashboard-devices-dialog-add-alert-title\"),\n        text: html`${this.lcn.localize(\"dashboard-devices-dialog-add-alert-text\")}\n          (${deviceParams.address![2] ? this.lcn.localize(\"group\") : this.lcn.localize(\"module\")}:\n          ${this.lcn.localize(\"segment\")} ${deviceParams.address![0]}, ${this.lcn.localize(\"id\")}\n          ${deviceParams.address![1]})\n          <br />\n          ${this.lcn.localize(\"dashboard-devices-dialog-add-alert-hint\")}`,\n      });\n      return;\n    }\n    dialog()!.closeDialog();\n    this._fetchDevices(this.lcn.host);\n  }\n\n  static get styles(): CSSResultGroup[] {\n    return [\n      haStyle,\n      css`\n        #box {\n          display: flex;\n          justify-content: space-between;\n        }\n        #host-select {\n          width: 40%;\n          display: inline-block;\n        }\n        #scan-devices {\n          display: inline-block;\n          margin-top: 20px;\n          justify-content: center;\n        }\n        summary:hover {\n          text-decoration: underline;\n        }\n      `,\n    ];\n  }\n}\n\ndeclare global {\n  interface HTMLElementTagNameMap {\n    \"lcn-config-dashboard\": LCNConfigDashboard;\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js.LICENSE.txt` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js.gz` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js.gz`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend/frontend_latest/yw4J-5vt.js.map` & `lcn_frontend-0.1.2/lcn_frontend/frontend_latest/yw4J-5vt.js.map`

 * *Files identical despite different names*

### Comparing `lcn_frontend-0.1.1/lcn_frontend.egg-info/SOURCES.txt` & `lcn_frontend-0.1.2/lcn_frontend.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
 setup.cfg
 lcn_frontend/__init__.py
 lcn_frontend/constants.py
-lcn_frontend/entrypoint-UP5lFvdJ.js
-lcn_frontend/entrypoint-UP5lFvdJ.js.gz
+lcn_frontend/entrypoint-Wn7tXtT_.js
+lcn_frontend/entrypoint-Wn7tXtT_.js.gz
 lcn_frontend/py.typed
 lcn_frontend.egg-info/PKG-INFO
 lcn_frontend.egg-info/SOURCES.txt
 lcn_frontend.egg-info/dependency_links.txt
 lcn_frontend.egg-info/not-zip-safe
 lcn_frontend.egg-info/top_level.txt
-lcn_frontend/frontend_es5/-Bo5aSaU.js
-lcn_frontend/frontend_es5/-Bo5aSaU.js.gz
+lcn_frontend/frontend_es5/1JtEbuPe.js
+lcn_frontend/frontend_es5/1JtEbuPe.js.gz
 lcn_frontend/frontend_es5/52ZGgRTb.js
 lcn_frontend/frontend_es5/52ZGgRTb.js.LICENSE.txt
 lcn_frontend/frontend_es5/52ZGgRTb.js.gz
 lcn_frontend/frontend_es5/6vdISARd.js
 lcn_frontend/frontend_es5/6vdISARd.js.gz
+lcn_frontend/frontend_es5/79rx9Er-.js
+lcn_frontend/frontend_es5/79rx9Er-.js.gz
 lcn_frontend/frontend_es5/8uDhd8eQ.js
 lcn_frontend/frontend_es5/8uDhd8eQ.js.gz
 lcn_frontend/frontend_es5/9niMDe6j.js
 lcn_frontend/frontend_es5/9niMDe6j.js.LICENSE.txt
 lcn_frontend/frontend_es5/9niMDe6j.js.gz
 lcn_frontend/frontend_es5/DVZuMQTQ.js
 lcn_frontend/frontend_es5/DVZuMQTQ.js.LICENSE.txt
 lcn_frontend/frontend_es5/DVZuMQTQ.js.gz
-lcn_frontend/frontend_es5/NATIZehR.js
-lcn_frontend/frontend_es5/NATIZehR.js.gz
+lcn_frontend/frontend_es5/J71QpLgx.js
+lcn_frontend/frontend_es5/J71QpLgx.js.gz
 lcn_frontend/frontend_es5/Niahov52.js
 lcn_frontend/frontend_es5/Niahov52.js.LICENSE.txt
 lcn_frontend/frontend_es5/Niahov52.js.gz
 lcn_frontend/frontend_es5/NmyD-jM4.js
 lcn_frontend/frontend_es5/NmyD-jM4.js.LICENSE.txt
 lcn_frontend/frontend_es5/NmyD-jM4.js.gz
 lcn_frontend/frontend_es5/PJOjJOeb.js
@@ -42,43 +44,48 @@
 lcn_frontend/frontend_es5/PJOjJOeb.js.gz
 lcn_frontend/frontend_es5/RIGgWZMd.js
 lcn_frontend/frontend_es5/RIGgWZMd.js.LICENSE.txt
 lcn_frontend/frontend_es5/RIGgWZMd.js.gz
 lcn_frontend/frontend_es5/RaxGx9Oy.js
 lcn_frontend/frontend_es5/RaxGx9Oy.js.LICENSE.txt
 lcn_frontend/frontend_es5/RaxGx9Oy.js.gz
-lcn_frontend/frontend_es5/RlIVWY_9.js
-lcn_frontend/frontend_es5/RlIVWY_9.js.gz
 lcn_frontend/frontend_es5/VCTfVQ_Y.js
 lcn_frontend/frontend_es5/VCTfVQ_Y.js.gz
 lcn_frontend/frontend_es5/VYXPimMw.js
 lcn_frontend/frontend_es5/VYXPimMw.js.gz
 lcn_frontend/frontend_es5/ZshdvKRY.js
 lcn_frontend/frontend_es5/ZshdvKRY.js.gz
-lcn_frontend/frontend_es5/entrypoint-IIGRb-2R.js
-lcn_frontend/frontend_es5/entrypoint-IIGRb-2R.js.LICENSE.txt
-lcn_frontend/frontend_es5/entrypoint-IIGRb-2R.js.gz
+lcn_frontend/frontend_es5/entrypoint-YtbOLj1f.js
+lcn_frontend/frontend_es5/entrypoint-YtbOLj1f.js.LICENSE.txt
+lcn_frontend/frontend_es5/entrypoint-YtbOLj1f.js.gz
 lcn_frontend/frontend_es5/f67fx1_K.js
 lcn_frontend/frontend_es5/f67fx1_K.js.gz
 lcn_frontend/frontend_es5/gWLSf6Uq.js
 lcn_frontend/frontend_es5/gWLSf6Uq.js.gz
 lcn_frontend/frontend_es5/kY1AJzRb.js
 lcn_frontend/frontend_es5/kY1AJzRb.js.gz
+lcn_frontend/frontend_es5/mNa8_BnN.js
+lcn_frontend/frontend_es5/mNa8_BnN.js.gz
+lcn_frontend/frontend_es5/m_bQlMKv.js
+lcn_frontend/frontend_es5/m_bQlMKv.js.LICENSE.txt
+lcn_frontend/frontend_es5/m_bQlMKv.js.gz
 lcn_frontend/frontend_es5/manifest.json
-lcn_frontend/frontend_es5/nqy1LXz0.js
-lcn_frontend/frontend_es5/nqy1LXz0.js.gz
-lcn_frontend/frontend_es5/riIkKI3D.js
-lcn_frontend/frontend_es5/riIkKI3D.js.LICENSE.txt
-lcn_frontend/frontend_es5/riIkKI3D.js.gz
 lcn_frontend/frontend_es5/xK5ZNMm1.js
 lcn_frontend/frontend_es5/xK5ZNMm1.js.LICENSE.txt
 lcn_frontend/frontend_es5/xK5ZNMm1.js.gz
 lcn_frontend/frontend_es5/ye57YhXr.js
 lcn_frontend/frontend_es5/ye57YhXr.js.LICENSE.txt
 lcn_frontend/frontend_es5/ye57YhXr.js.gz
+lcn_frontend/frontend_latest/9VkUPPxQ.js
+lcn_frontend/frontend_latest/9VkUPPxQ.js.LICENSE.txt
+lcn_frontend/frontend_latest/9VkUPPxQ.js.gz
+lcn_frontend/frontend_latest/9VkUPPxQ.js.map
+lcn_frontend/frontend_latest/9yFFShGq.js
+lcn_frontend/frontend_latest/9yFFShGq.js.gz
+lcn_frontend/frontend_latest/9yFFShGq.js.map
 lcn_frontend/frontend_latest/AuN1Wwjr.js
 lcn_frontend/frontend_latest/AuN1Wwjr.js.LICENSE.txt
 lcn_frontend/frontend_latest/AuN1Wwjr.js.gz
 lcn_frontend/frontend_latest/CHsIPDL8.js
 lcn_frontend/frontend_latest/CHsIPDL8.js.LICENSE.txt
 lcn_frontend/frontend_latest/CHsIPDL8.js.gz
 lcn_frontend/frontend_latest/CHsIPDL8.js.map
@@ -86,72 +93,65 @@
 lcn_frontend/frontend_latest/HyurOyWN.js.LICENSE.txt
 lcn_frontend/frontend_latest/HyurOyWN.js.gz
 lcn_frontend/frontend_latest/HyurOyWN.js.map
 lcn_frontend/frontend_latest/JAAifVse.js
 lcn_frontend/frontend_latest/JAAifVse.js.LICENSE.txt
 lcn_frontend/frontend_latest/JAAifVse.js.gz
 lcn_frontend/frontend_latest/JAAifVse.js.map
+lcn_frontend/frontend_latest/Ntga-_EF.js
+lcn_frontend/frontend_latest/Ntga-_EF.js.gz
+lcn_frontend/frontend_latest/Ntga-_EF.js.map
 lcn_frontend/frontend_latest/PHB24J1t.js
 lcn_frontend/frontend_latest/PHB24J1t.js.LICENSE.txt
 lcn_frontend/frontend_latest/PHB24J1t.js.gz
-lcn_frontend/frontend_latest/R9L2-V1R.js
-lcn_frontend/frontend_latest/R9L2-V1R.js.gz
-lcn_frontend/frontend_latest/R9L2-V1R.js.map
 lcn_frontend/frontend_latest/SaPEbRz1.js
 lcn_frontend/frontend_latest/SaPEbRz1.js.LICENSE.txt
 lcn_frontend/frontend_latest/SaPEbRz1.js.gz
 lcn_frontend/frontend_latest/SaPEbRz1.js.map
 lcn_frontend/frontend_latest/X5sZzGl8.js
 lcn_frontend/frontend_latest/X5sZzGl8.js.LICENSE.txt
 lcn_frontend/frontend_latest/X5sZzGl8.js.gz
 lcn_frontend/frontend_latest/ZRpJZyXB.js
 lcn_frontend/frontend_latest/ZRpJZyXB.js.gz
 lcn_frontend/frontend_latest/ZRpJZyXB.js.map
-lcn_frontend/frontend_latest/bZayZmh0.js
-lcn_frontend/frontend_latest/bZayZmh0.js.gz
-lcn_frontend/frontend_latest/bZayZmh0.js.map
 lcn_frontend/frontend_latest/bc9cfM__.js
 lcn_frontend/frontend_latest/bc9cfM__.js.LICENSE.txt
 lcn_frontend/frontend_latest/bc9cfM__.js.gz
 lcn_frontend/frontend_latest/bc9cfM__.js.map
-lcn_frontend/frontend_latest/eOHcBlX_.js
-lcn_frontend/frontend_latest/eOHcBlX_.js.gz
-lcn_frontend/frontend_latest/eOHcBlX_.js.map
-lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js
-lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js.LICENSE.txt
-lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js.gz
-lcn_frontend/frontend_latest/entrypoint-UP5lFvdJ.js.map
+lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js
+lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js.LICENSE.txt
+lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js.gz
+lcn_frontend/frontend_latest/entrypoint-Wn7tXtT_.js.map
 lcn_frontend/frontend_latest/fP3U9roj.js
 lcn_frontend/frontend_latest/fP3U9roj.js.LICENSE.txt
 lcn_frontend/frontend_latest/fP3U9roj.js.gz
 lcn_frontend/frontend_latest/fP3U9roj.js.map
 lcn_frontend/frontend_latest/fYLWqtat.js
 lcn_frontend/frontend_latest/fYLWqtat.js.LICENSE.txt
 lcn_frontend/frontend_latest/fYLWqtat.js.gz
 lcn_frontend/frontend_latest/fYLWqtat.js.map
+lcn_frontend/frontend_latest/gwnfZ3wa.js
+lcn_frontend/frontend_latest/gwnfZ3wa.js.gz
+lcn_frontend/frontend_latest/gwnfZ3wa.js.map
 lcn_frontend/frontend_latest/hzhoTwCw.js
 lcn_frontend/frontend_latest/hzhoTwCw.js.LICENSE.txt
 lcn_frontend/frontend_latest/hzhoTwCw.js.gz
 lcn_frontend/frontend_latest/hzhoTwCw.js.map
 lcn_frontend/frontend_latest/mUrtGIle.js
 lcn_frontend/frontend_latest/mUrtGIle.js.gz
 lcn_frontend/frontend_latest/mUrtGIle.js.map
 lcn_frontend/frontend_latest/manifest.json
-lcn_frontend/frontend_latest/oUOHqENt.js
-lcn_frontend/frontend_latest/oUOHqENt.js.LICENSE.txt
-lcn_frontend/frontend_latest/oUOHqENt.js.gz
-lcn_frontend/frontend_latest/oUOHqENt.js.map
+lcn_frontend/frontend_latest/ovjKXg0y.js
+lcn_frontend/frontend_latest/ovjKXg0y.js.gz
+lcn_frontend/frontend_latest/ovjKXg0y.js.map
 lcn_frontend/frontend_latest/oyUFw0ts.js
 lcn_frontend/frontend_latest/oyUFw0ts.js.LICENSE.txt
 lcn_frontend/frontend_latest/oyUFw0ts.js.gz
 lcn_frontend/frontend_latest/oyUFw0ts.js.map
 lcn_frontend/frontend_latest/sBNRM32J.js
 lcn_frontend/frontend_latest/sBNRM32J.js.LICENSE.txt
 lcn_frontend/frontend_latest/sBNRM32J.js.gz
 lcn_frontend/frontend_latest/sBNRM32J.js.map
-lcn_frontend/frontend_latest/yvD5aARM.js
-lcn_frontend/frontend_latest/yvD5aARM.js.gz
-lcn_frontend/frontend_latest/yvD5aARM.js.map
 lcn_frontend/frontend_latest/yw4J-5vt.js
 lcn_frontend/frontend_latest/yw4J-5vt.js.LICENSE.txt
 lcn_frontend/frontend_latest/yw4J-5vt.js.gz
 lcn_frontend/frontend_latest/yw4J-5vt.js.map
```

### Comparing `lcn_frontend-0.1.1/pyproject.toml` & `lcn_frontend-0.1.2/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/pyaudisam-1.0.2.tar.gz` & `tmp/pyaudisam-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaudisam-1.0.2.tar", last modified: Wed Feb 21 13:17:39 2024, max compression
+gzip compressed data, was "pyaudisam-1.1.0.tar", last modified: Wed May 15 18:45:01 2024, max compression
```

## Comparing `pyaudisam-1.0.2.tar` & `pyaudisam-1.1.0.tar`

### file list

```diff
@@ -1,211 +1,231 @@
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.677223 pyaudisam-1.0.2/
--rw-rw-rw-   0        0        0    35149 2021-10-03 09:00:39.000000 pyaudisam-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2546 2023-05-21 19:51:31.000000 pyaudisam-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8377 2024-02-21 13:17:39.676224 pyaudisam-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7177 2024-02-21 11:00:28.000000 pyaudisam-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.323007 pyaudisam-1.0.2/docs/
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.353516 pyaudisam-1.0.2/docs/how-it-works/
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.427521 pyaudisam-1.0.2/docs/how-it-works/common/
--rw-rw-rw-   0        0        0      475 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-angle-up.svg
--rw-rw-rw-   0        0        0      522 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-left-hover.svg
--rw-rw-rw-   0        0        0      522 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-left.svg
--rw-rw-rw-   0        0        0      527 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-right-hover.svg
--rw-rw-rw-   0        0        0      527 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-right.svg
--rw-rw-rw-   0        0        0      525 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-up-hover.svg
--rw-rw-rw-   0        0        0      525 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-up.svg
--rw-rw-rw-   0        0        0      673 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-feather-alt.svg
--rw-rw-rw-   0        0        0      866 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-file-excel-hover.svg
--rw-rw-rw-   0        0        0      866 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/fa-file-excel.svg
--rw-rw-rw-   0        0        0     5281 2023-04-16 16:55:43.000000 pyaudisam-1.0.2/docs/how-it-works/common/report.css
--rw-rw-rw-   0        0        0    18513 2023-08-10 17:17:22.000000 pyaudisam-1.0.2/docs/how-it-works/how-it-works-en.md
--rw-rw-rw-   0        0        0    20013 2023-08-10 17:16:58.000000 pyaudisam-1.0.2/docs/how-it-works/how-it-works-fr.md
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.482030 pyaudisam-1.0.2/docs/how-it-works/optanlys/
--rw-rw-rw-   0        0        0   387006 2023-05-08 12:19:10.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report-partview.ExAicMQua-r925m8q3d12.jpg
--rw-rw-rw-   0        0        0   100947 2023-05-23 18:49:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.ExAicMQua-r925m8q3d12.html
--rw-rw-rw-   0        0        0   431912 2023-04-30 14:23:33.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.xlsx
--rw-rw-rw-   0        0        0   196363 2023-04-30 13:55:20.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat.230430-153402.log
--rw-rw-rw-   0        0        0    35769 2023-04-30 14:27:16.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat.230430-162324.log
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.554547 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/
--rw-rw-rw-   0        0        0      862 2023-05-01 18:57:23.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/cmd.txt
--rw-rw-rw-   0        0        0    12865 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/data.txt
--rw-rw-rw-   0        0        0    43733 2023-04-30 14:24:04.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/detprob1.png
--rw-rw-rw-   0        0        0    44166 2023-04-30 14:24:05.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/disthist.png
--rw-rw-rw-   0        0        0    66444 2023-05-01 19:04:24.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/index.html
--rw-rw-rw-   0        0        0     3418 2023-05-01 18:57:34.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/log.txt
--rw-rw-rw-   0        0        0    19974 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/output.txt
--rw-rw-rw-   0        0        0    33720 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/plots.txt
--rw-rw-rw-   0        0        0    44116 2023-04-30 14:24:05.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/probdens1.png
--rw-rw-rw-   0        0        0    34280 2023-04-30 14:24:04.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/qqplot.png
--rw-rw-rw-   0        0        0     2769 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/stats.txt
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.627585 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/
--rw-rw-rw-   0        0        0      892 2023-05-01 18:56:59.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/cmd.txt
--rw-rw-rw-   0        0        0    12865 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/data.txt
--rw-rw-rw-   0        0        0    43600 2023-04-30 14:24:01.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/detprob1.png
--rw-rw-rw-   0        0        0    44166 2023-04-30 14:24:02.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/disthist.png
--rw-rw-rw-   0        0        0    63551 2023-05-01 19:04:46.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/index.html
--rw-rw-rw-   0        0        0     3418 2023-05-01 18:57:07.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/log.txt
--rw-rw-rw-   0        0        0    17139 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/output.txt
--rw-rw-rw-   0        0        0    32372 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/plots.txt
--rw-rw-rw-   0        0        0    47130 2023-04-30 14:24:01.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/probdens1.png
--rw-rw-rw-   0        0        0    34486 2023-04-30 14:24:01.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/qqplot.png
--rw-rw-rw-   0        0        0     2769 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/stats.txt
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.699142 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/
--rw-rw-rw-   0        0        0      833 2023-05-01 18:55:47.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/cmd.txt
--rw-rw-rw-   0        0        0    12865 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/data.txt
--rw-rw-rw-   0        0        0    44906 2023-04-30 14:24:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/detprob1.png
--rw-rw-rw-   0        0        0    44166 2023-04-30 14:24:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/disthist.png
--rw-rw-rw-   0        0        0    65003 2023-05-01 19:05:49.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/index.html
--rw-rw-rw-   0        0        0     3418 2023-05-01 18:56:09.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/log.txt
--rw-rw-rw-   0        0        0    18242 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/output.txt
--rw-rw-rw-   0        0        0    31308 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/plots.txt
--rw-rw-rw-   0        0        0    48239 2023-04-30 14:24:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/probdens1.png
--rw-rw-rw-   0        0        0    34267 2023-04-30 14:24:02.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/qqplot.png
--rw-rw-rw-   0        0        0     2769 2023-04-30 13:55:03.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/stats.txt
--rw-rw-rw-   0        0        0    19306 2023-05-22 19:44:36.000000 pyaudisam-1.0.2/docs/how-it-works/optanlys/acdc-2019-nat-ds-params.py
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.748656 pyaudisam-1.0.2/docs/how-it-works/preanlys/
--rw-rw-rw-   0        0        0   231698 2023-05-08 12:17:55.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report-partview.jpg
--rw-rw-rw-   0        0        0    12984 2023-05-23 18:50:04.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.html
--rw-rw-rw-   0        0        0    21757 2023-05-01 16:50:23.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.xlsx
--rw-rw-rw-   0        0        0     9144 2023-04-16 16:03:15.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat.230416-180310.log
--rw-rw-rw-   0        0        0    13245 2023-04-16 16:55:52.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat.230416-185538.log
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.823701 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/
--rw-rw-rw-   0        0        0      805 2023-05-01 18:58:07.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/cmd.txt
--rw-rw-rw-   0        0        0     2475 2023-04-16 16:55:40.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/data.txt
--rw-rw-rw-   0        0        0    44290 2023-04-16 16:55:47.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob1.png
--rw-rw-rw-   0        0        0    44964 2023-04-16 16:55:48.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob2.png
--rw-rw-rw-   0        0        0    45850 2023-04-16 16:55:49.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob3.png
--rw-rw-rw-   0        0        0    41578 2023-04-16 16:55:50.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/disthist.png
--rw-rw-rw-   0        0        0    69061 2023-05-01 17:11:09.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/index.html
--rw-rw-rw-   0        0        0     3573 2023-05-01 18:58:14.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/log.txt
--rw-rw-rw-   0        0        0    37243 2023-04-16 16:55:40.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/output.txt
--rw-rw-rw-   0        0        0    50116 2023-04-16 16:55:40.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/plots.txt
--rw-rw-rw-   0        0        0    46974 2023-04-16 16:55:48.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens1.png
--rw-rw-rw-   0        0        0    45282 2023-04-16 16:55:49.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens2.png
--rw-rw-rw-   0        0        0    44681 2023-04-16 16:55:50.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens3.png
--rw-rw-rw-   0        0        0    34997 2023-04-16 16:55:47.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/qqplot.png
--rw-rw-rw-   0        0        0     2963 2023-04-16 16:55:40.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/stats.txt
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.900239 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/
--rw-rw-rw-   0        0        0      804 2023-05-01 18:58:25.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/cmd.txt
--rw-rw-rw-   0        0        0    12865 2023-04-16 16:55:41.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/data.txt
--rw-rw-rw-   0        0        0    44906 2023-04-16 16:55:47.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob1.png
--rw-rw-rw-   0        0        0    43261 2023-04-16 16:55:48.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob2.png
--rw-rw-rw-   0        0        0    44019 2023-04-16 16:55:49.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob3.png
--rw-rw-rw-   0        0        0    44166 2023-04-16 16:55:51.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/disthist.png
--rw-rw-rw-   0        0        0    74210 2023-05-01 17:09:51.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/index.html
--rw-rw-rw-   0        0        0     3494 2023-05-01 18:58:30.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/log.txt
--rw-rw-rw-   0        0        0    42287 2023-04-16 16:55:41.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/output.txt
--rw-rw-rw-   0        0        0    68276 2023-04-16 16:55:41.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/plots.txt
--rw-rw-rw-   0        0        0    48239 2023-04-16 16:55:48.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens1.png
--rw-rw-rw-   0        0        0    44532 2023-04-16 16:55:49.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens2.png
--rw-rw-rw-   0        0        0    45563 2023-04-16 16:55:50.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens3.png
--rw-rw-rw-   0        0        0    34267 2023-04-16 16:55:47.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/qqplot.png
--rw-rw-rw-   0        0        0     2963 2023-04-16 16:55:41.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/stats.txt
--rw-rw-rw-   0        0        0    19306 2023-05-22 19:44:36.000000 pyaudisam-1.0.2/docs/how-it-works/preanlys/acdc-2019-nat-ds-params.py
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:38.968752 pyaudisam-1.0.2/docs/howto-acdc19-nat/
--rw-rw-rw-   0        0        0   328909 2023-04-12 10:00:56.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-108-points-300m-circles.kml
--rw-rw-rw-   0        0        0    75485 2023-04-12 20:57:51.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-Nat-ObsIndivDist.xlsx
--rw-rw-rw-   0        0        0    12243 2023-05-20 16:40:50.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-OptAnalysesToDo.xlsx
--rw-rw-rw-   0        0        0     6890 2023-04-12 19:03:05.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-Samples.xlsx
--rw-rw-rw-   0        0        0    19318 2024-02-21 11:40:22.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/acdc-2019-nat-ds-params.py
--rw-rw-rw-   0        0        0    72210 2024-02-21 13:09:36.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/acdc-2019-nat-ds-run.ipynb
--rw-rw-rw-   0        0        0    38137 2024-02-21 10:40:43.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/howto.md
--rw-rw-rw-   0        0        0     3235 2023-05-03 09:51:38.000000 pyaudisam-1.0.2/docs/howto-acdc19-nat/ipython_notebook_toc.js
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.093381 pyaudisam-1.0.2/pyaudisam/
--rw-rw-rw-   0        0        0     2728 2024-02-21 11:02:19.000000 pyaudisam-1.0.2/pyaudisam/__init__.py
--rw-rw-rw-   0        0        0    54951 2023-11-02 11:33:21.000000 pyaudisam-1.0.2/pyaudisam/__main__.py
--rw-rw-rw-   0        0        0   152935 2023-11-03 11:10:27.000000 pyaudisam-1.0.2/pyaudisam/analyser.py
--rw-rw-rw-   0        0        0    19380 2023-11-02 11:01:39.000000 pyaudisam-1.0.2/pyaudisam/analysis.py
--rw-rw-rw-   0        0        0    79553 2024-02-19 18:33:08.000000 pyaudisam-1.0.2/pyaudisam/data.py
--rw-rw-rw-   0        0        0    44086 2023-11-02 11:01:09.000000 pyaudisam-1.0.2/pyaudisam/engine.py
--rw-rw-rw-   0        0        0     7652 2023-11-02 11:13:04.000000 pyaudisam-1.0.2/pyaudisam/executor.py
--rw-rw-rw-   0        0        0     7881 2023-05-12 13:54:38.000000 pyaudisam-1.0.2/pyaudisam/log.py
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.198899 pyaudisam-1.0.2/pyaudisam/mcds/
--rw-rw-rw-   0        0        0     9851 2023-08-27 19:22:15.000000 pyaudisam-1.0.2/pyaudisam/mcds/anlys.htpl
--rw-rw-rw-   0        0        0     9093 2023-11-26 18:21:29.000000 pyaudisam-1.0.2/pyaudisam/mcds/fulltop.htpl
--rw-rw-rw-   0        0        0     6044 2023-11-26 18:21:29.000000 pyaudisam-1.0.2/pyaudisam/mcds/pretop.htpl
--rw-rw-rw-   0        0        0      686 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/mcds/stat-mod-notes.txt
--rw-rw-rw-   0        0        0     1988 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/mcds/stat-mod-specs.txt
--rw-rw-rw-   0        0        0     7965 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/mcds/stat-mod-trans.txt
--rw-rw-rw-   0        0        0      834 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/mcds/stat-row-specs.txt
--rw-rw-rw-   0        0        0     6418 2023-08-27 19:22:06.000000 pyaudisam-1.0.2/pyaudisam/mcds/top.htpl
--rw-rw-rw-   0        0        0    34064 2023-05-14 17:51:10.000000 pyaudisam-1.0.2/pyaudisam/optanalyser.py
--rw-rw-rw-   0        0        0    39014 2023-11-02 14:17:30.000000 pyaudisam-1.0.2/pyaudisam/optimisation.py
--rw-rw-rw-   0        0        0    74788 2023-11-02 11:38:22.000000 pyaudisam-1.0.2/pyaudisam/optimiser.py
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.222903 pyaudisam-1.0.2/pyaudisam/report/
--rw-rw-rw-   0        0        0      475 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-angle-up.svg
--rw-rw-rw-   0        0        0      522 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-arrow-left-hover.svg
--rw-rw-rw-   0        0        0      522 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-arrow-left.svg
--rw-rw-rw-   0        0        0      527 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-arrow-right-hover.svg
--rw-rw-rw-   0        0        0      527 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-arrow-right.svg
--rw-rw-rw-   0        0        0      525 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-arrow-up-hover.svg
--rw-rw-rw-   0        0        0      525 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-arrow-up.svg
--rw-rw-rw-   0        0        0      673 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-feather-alt.svg
--rw-rw-rw-   0        0        0      866 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-file-excel-hover.svg
--rw-rw-rw-   0        0        0      866 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/fa-file-excel.svg
--rw-rw-rw-   0        0        0     5281 2022-01-22 16:29:08.000000 pyaudisam-1.0.2/pyaudisam/report/report.css
--rw-rw-rw-   0        0        0   127439 2023-12-21 20:15:04.000000 pyaudisam-1.0.2/pyaudisam/report.py
--rw-rw-rw-   0        0        0     2124 2023-05-12 13:54:38.000000 pyaudisam-1.0.2/pyaudisam/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.675224 pyaudisam-1.0.2/pyaudisam.egg-info/
--rw-rw-rw-   0        0        0     8377 2024-02-21 13:17:38.000000 pyaudisam-1.0.2/pyaudisam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10450 2024-02-21 13:17:38.000000 pyaudisam-1.0.2/pyaudisam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-21 13:17:38.000000 pyaudisam-1.0.2/pyaudisam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2024-02-21 13:17:38.000000 pyaudisam-1.0.2/pyaudisam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-21 13:17:38.000000 pyaudisam-1.0.2/pyaudisam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      157 2024-02-21 10:58:20.000000 pyaudisam-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       77 2024-02-21 13:17:39.678224 pyaudisam-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2751 2023-05-25 18:54:26.000000 pyaudisam-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.362633 pyaudisam-1.0.2/tests/
--rw-rw-rw-   0        0        0     1102 2024-02-20 14:13:45.000000 pyaudisam-1.0.2/tests/conftest.py
--rw-rw-rw-   0        0        0   149073 2021-11-20 09:47:55.000000 pyaudisam-1.0.2/tests/devarchives1.ipynb
--rw-rw-rw-   0        0        0   205550 2023-04-16 10:02:37.000000 pyaudisam-1.0.2/tests/devarchives2.ipynb
--rw-rw-rw-   0        0        0     3048 2021-10-03 10:04:40.000000 pyaudisam-1.0.2/tests/ipython_notebook_toc.js
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.581697 pyaudisam-1.0.2/tests/refin/
--rw-rw-rw-   0        0        0    57477 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt
--rw-rw-rw-   0        0        0    57750 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods
--rw-rw-rw-   0        0        0    13349 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx
--rw-rw-rw-   0        0        0    11922 2021-12-28 09:03:01.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitSpecsEchants.ods
--rw-rw-rw-   0        0        0    18211 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx
--rw-rw-rw-   0        0        0    66148 2021-11-20 20:11:41.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-UnitestOptResultats.ods
--rw-rw-rw-   0        0        0     5686 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dec-dist.txt
--rw-rw-rw-   0        0        0     5686 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dotdec-dist.txt
--rw-rw-rw-   0        0        0     6771 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-6dec-dist.txt
--rw-rw-rw-   0        0        0     6340 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0    39311 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods
--rw-rw-rw-   0        0        0    29263 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.ods
--rw-rw-rw-   0        0        0    16242 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xlsx
--rw-rw-rw-   0        0        0     2493 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ANTTRI-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0     4881 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-COLPAL-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0   190595 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-DonneesBrutesPourAutoDS.xlsx
--rw-rw-rw-   0        0        0     3170 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-EMBCIR-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0     2620 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-EMBCIT-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0     6105 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-LUSMEG-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0     2313 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-MILCAL-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0     4165 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-PHYCOL-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0    11401 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-SYLATR-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0     9638 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-1dec-dist.txt
--rw-rw-rw-   0        0        0    11753 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-6dec-dist.txt
--rw-rw-rw-   0        0        0    11227 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-ttdec-dist.txt
--rw-rw-rw-   0        0        0     7440 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-5mn-1dec-dist.txt
--rw-rw-rw-   0        0        0    51263 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refin/TURMER-10mn-1dec-hnorm-cos.odt
-drwxrwxrwx   0        0        0        0 2024-02-21 13:17:39.674223 pyaudisam-1.0.2/tests/refout/
--rw-rw-rw-   0        0        0     7566 2024-02-19 21:32:47.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist-sampleDataSet.xlsx
--rw-rw-rw-   0        0        0     7566 2024-02-19 21:32:47.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist-sampleDataSet_sep.xlsx
--rw-rw-rw-   0        0        0    58058 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Naturalist-ExtraitOptResultats.ods
--rw-rw-rw-   0        0        0    25032 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Naturalist-ExtraitPreResultats.ods
--rw-rw-rw-   0        0        0    48727 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Naturalist-ExtraitResultats.ods
--rw-rw-rw-   0        0        0    24594 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-distance-73.xlsx
--rw-rw-rw-   0        0        0    19410 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-postcomp.ods
--rw-rw-rw-   0        0        0     6120 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-5-cols.txt
--rw-rw-rw-   0        0        0      273 2024-02-19 11:12:12.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-clusters.txt
--rw-rw-rw-   0        0        0     6120 2024-02-19 11:12:07.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-noextra.txt
--rw-rw-rw-   0        0        0    13142 2024-02-19 11:12:08.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-withextra.txt
--rw-rw-rw-   0        0        0    13142 2021-09-26 19:14:02.000000 pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.txt
--rw-rw-rw-   0        0        0    17786 2022-01-22 14:52:05.000000 pyaudisam-1.0.2/tests/sensitivity.ipynb
--rw-rw-rw-   0        0        0    69580 2024-02-21 09:54:40.000000 pyaudisam-1.0.2/tests/unint_analyser_results_test.py
--rw-rw-rw-   0        0        0    42980 2024-02-20 18:45:04.000000 pyaudisam-1.0.2/tests/unint_data_test.py
--rw-rw-rw-   0        0        0    25894 2024-02-20 18:38:28.000000 pyaudisam-1.0.2/tests/unint_engine_test.py
--rw-rw-rw-   0        0        0   288062 2024-02-19 22:10:15.000000 pyaudisam-1.0.2/tests/unintests.ipynb
--rw-rw-rw-   0        0        0     2601 2024-02-20 14:25:34.000000 pyaudisam-1.0.2/tests/unintval_utils.py
--rw-rw-rw-   0        0        0   129281 2021-11-20 18:31:15.000000 pyaudisam-1.0.2/tests/valarchives.ipynb
--rw-rw-rw-   0        0        0    22094 2023-05-12 13:54:38.000000 pyaudisam-1.0.2/tests/valtests-ds-params.py
--rw-rw-rw-   0        0        0   124830 2023-11-02 16:19:55.000000 pyaudisam-1.0.2/tests/valtests.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:01.031925 pyaudisam-1.1.0/
+-rw-rw-rw-   0        0        0       21 2024-02-25 09:46:42.000000 pyaudisam-1.1.0/.coveragerc
+-rw-rw-rw-   0        0        0    35149 2021-10-03 09:00:39.000000 pyaudisam-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2679 2024-05-15 18:44:13.000000 pyaudisam-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10425 2024-05-15 18:45:01.031925 pyaudisam-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9083 2024-05-14 17:54:48.000000 pyaudisam-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.132820 pyaudisam-1.1.0/docs/
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.148481 pyaudisam-1.1.0/docs/how-it-works/
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.226979 pyaudisam-1.1.0/docs/how-it-works/common/
+-rw-rw-rw-   0        0        0      475 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-angle-up.svg
+-rw-rw-rw-   0        0        0      522 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-left-hover.svg
+-rw-rw-rw-   0        0        0      522 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-left.svg
+-rw-rw-rw-   0        0        0      527 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-right-hover.svg
+-rw-rw-rw-   0        0        0      527 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-right.svg
+-rw-rw-rw-   0        0        0      525 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-up-hover.svg
+-rw-rw-rw-   0        0        0      525 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-up.svg
+-rw-rw-rw-   0        0        0      673 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-feather-alt.svg
+-rw-rw-rw-   0        0        0      866 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-file-excel-hover.svg
+-rw-rw-rw-   0        0        0      866 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/fa-file-excel.svg
+-rw-rw-rw-   0        0        0     5281 2023-04-16 16:55:43.000000 pyaudisam-1.1.0/docs/how-it-works/common/report.css
+-rw-rw-rw-   0        0        0    18514 2024-04-01 12:17:34.000000 pyaudisam-1.1.0/docs/how-it-works/how-it-works-en.md
+-rw-rw-rw-   0        0        0    20014 2024-04-01 12:17:34.000000 pyaudisam-1.1.0/docs/how-it-works/how-it-works-fr.md
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.305529 pyaudisam-1.1.0/docs/how-it-works/optanlys/
+-rw-rw-rw-   0        0        0   387006 2023-05-08 12:19:10.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report-partview.ExAicMQua-r925m8q3d12.jpg
+-rw-rw-rw-   0        0        0   100947 2023-05-23 18:49:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.ExAicMQua-r925m8q3d12.html
+-rw-rw-rw-   0        0        0   431912 2023-04-30 14:23:33.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.xlsx
+-rw-rw-rw-   0        0        0   196363 2023-04-30 13:55:20.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat.230430-153402.log
+-rw-rw-rw-   0        0        0    35769 2023-04-30 14:27:16.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat.230430-162324.log
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.383670 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/
+-rw-rw-rw-   0        0        0      862 2023-05-01 18:57:23.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/cmd.txt
+-rw-rw-rw-   0        0        0    12865 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/data.txt
+-rw-rw-rw-   0        0        0    43733 2023-04-30 14:24:04.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/detprob1.png
+-rw-rw-rw-   0        0        0    44166 2023-04-30 14:24:05.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/disthist.png
+-rw-rw-rw-   0        0        0    66444 2023-05-01 19:04:24.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/index.html
+-rw-rw-rw-   0        0        0     3418 2023-05-01 18:57:34.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/log.txt
+-rw-rw-rw-   0        0        0    19974 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/output.txt
+-rw-rw-rw-   0        0        0    33720 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/plots.txt
+-rw-rw-rw-   0        0        0    44116 2023-04-30 14:24:05.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/probdens1.png
+-rw-rw-rw-   0        0        0    34280 2023-04-30 14:24:04.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/qqplot.png
+-rw-rw-rw-   0        0        0     2769 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/stats.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.477824 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/
+-rw-rw-rw-   0        0        0      892 2023-05-01 18:56:59.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/cmd.txt
+-rw-rw-rw-   0        0        0    12865 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/data.txt
+-rw-rw-rw-   0        0        0    43600 2023-04-30 14:24:01.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/detprob1.png
+-rw-rw-rw-   0        0        0    44166 2023-04-30 14:24:02.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/disthist.png
+-rw-rw-rw-   0        0        0    63551 2023-05-01 19:04:46.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/index.html
+-rw-rw-rw-   0        0        0     3418 2023-05-01 18:57:07.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/log.txt
+-rw-rw-rw-   0        0        0    17139 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/output.txt
+-rw-rw-rw-   0        0        0    32372 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/plots.txt
+-rw-rw-rw-   0        0        0    47130 2023-04-30 14:24:01.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/probdens1.png
+-rw-rw-rw-   0        0        0    34486 2023-04-30 14:24:01.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/qqplot.png
+-rw-rw-rw-   0        0        0     2769 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/stats.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.571991 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/
+-rw-rw-rw-   0        0        0      833 2023-05-01 18:55:47.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/cmd.txt
+-rw-rw-rw-   0        0        0    12865 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/data.txt
+-rw-rw-rw-   0        0        0    44906 2023-04-30 14:24:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/detprob1.png
+-rw-rw-rw-   0        0        0    44166 2023-04-30 14:24:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/disthist.png
+-rw-rw-rw-   0        0        0    65003 2023-05-01 19:05:49.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/index.html
+-rw-rw-rw-   0        0        0     3418 2023-05-01 18:56:09.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/log.txt
+-rw-rw-rw-   0        0        0    18242 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/output.txt
+-rw-rw-rw-   0        0        0    31308 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/plots.txt
+-rw-rw-rw-   0        0        0    48239 2023-04-30 14:24:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/probdens1.png
+-rw-rw-rw-   0        0        0    34267 2023-04-30 14:24:02.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/qqplot.png
+-rw-rw-rw-   0        0        0     2769 2023-04-30 13:55:03.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/stats.txt
+-rw-rw-rw-   0        0        0    19306 2023-05-22 19:44:36.000000 pyaudisam-1.1.0/docs/how-it-works/optanlys/acdc-2019-nat-ds-params.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.619272 pyaudisam-1.1.0/docs/how-it-works/preanlys/
+-rw-rw-rw-   0        0        0   231698 2023-05-08 12:17:55.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report-partview.jpg
+-rw-rw-rw-   0        0        0    12984 2023-05-23 18:50:04.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.html
+-rw-rw-rw-   0        0        0    21757 2023-05-01 16:50:23.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.xlsx
+-rw-rw-rw-   0        0        0     9144 2023-04-16 16:03:15.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat.230416-180310.log
+-rw-rw-rw-   0        0        0    13245 2023-04-16 16:55:52.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat.230416-185538.log
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.713490 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/
+-rw-rw-rw-   0        0        0      805 2023-05-01 18:58:07.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/cmd.txt
+-rw-rw-rw-   0        0        0     2475 2023-04-16 16:55:40.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/data.txt
+-rw-rw-rw-   0        0        0    44290 2023-04-16 16:55:47.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob1.png
+-rw-rw-rw-   0        0        0    44964 2023-04-16 16:55:48.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob2.png
+-rw-rw-rw-   0        0        0    45850 2023-04-16 16:55:49.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob3.png
+-rw-rw-rw-   0        0        0    41578 2023-04-16 16:55:50.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/disthist.png
+-rw-rw-rw-   0        0        0    69061 2023-05-01 17:11:09.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/index.html
+-rw-rw-rw-   0        0        0     3573 2023-05-01 18:58:14.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/log.txt
+-rw-rw-rw-   0        0        0    37243 2023-04-16 16:55:40.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/output.txt
+-rw-rw-rw-   0        0        0    50116 2023-04-16 16:55:40.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/plots.txt
+-rw-rw-rw-   0        0        0    46974 2023-04-16 16:55:48.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens1.png
+-rw-rw-rw-   0        0        0    45282 2023-04-16 16:55:49.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens2.png
+-rw-rw-rw-   0        0        0    44681 2023-04-16 16:55:50.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens3.png
+-rw-rw-rw-   0        0        0    34997 2023-04-16 16:55:47.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/qqplot.png
+-rw-rw-rw-   0        0        0     2963 2023-04-16 16:55:40.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/stats.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.807664 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/
+-rw-rw-rw-   0        0        0      804 2023-05-01 18:58:25.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/cmd.txt
+-rw-rw-rw-   0        0        0    12865 2023-04-16 16:55:41.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/data.txt
+-rw-rw-rw-   0        0        0    44906 2023-04-16 16:55:47.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob1.png
+-rw-rw-rw-   0        0        0    43261 2023-04-16 16:55:48.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob2.png
+-rw-rw-rw-   0        0        0    44019 2023-04-16 16:55:49.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob3.png
+-rw-rw-rw-   0        0        0    44166 2023-04-16 16:55:51.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/disthist.png
+-rw-rw-rw-   0        0        0    74210 2023-05-01 17:09:51.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/index.html
+-rw-rw-rw-   0        0        0     3494 2023-05-01 18:58:30.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/log.txt
+-rw-rw-rw-   0        0        0    42287 2023-04-16 16:55:41.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/output.txt
+-rw-rw-rw-   0        0        0    68276 2023-04-16 16:55:41.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/plots.txt
+-rw-rw-rw-   0        0        0    48239 2023-04-16 16:55:48.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens1.png
+-rw-rw-rw-   0        0        0    44532 2023-04-16 16:55:49.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens2.png
+-rw-rw-rw-   0        0        0    45563 2023-04-16 16:55:50.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens3.png
+-rw-rw-rw-   0        0        0    34267 2023-04-16 16:55:47.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/qqplot.png
+-rw-rw-rw-   0        0        0     2963 2023-04-16 16:55:41.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/stats.txt
+-rw-rw-rw-   0        0        0    19306 2023-05-22 19:44:36.000000 pyaudisam-1.1.0/docs/how-it-works/preanlys/acdc-2019-nat-ds-params.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:44:59.901853 pyaudisam-1.1.0/docs/howto-acdc19-nat/
+-rw-rw-rw-   0        0        0   328909 2023-04-12 10:00:56.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-108-points-300m-circles.kml
+-rw-rw-rw-   0        0        0    75485 2023-04-12 20:57:51.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-Nat-ObsIndivDist.xlsx
+-rw-rw-rw-   0        0        0    12243 2023-05-20 16:40:50.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-OptAnalysesToDo.xlsx
+-rw-rw-rw-   0        0        0     6890 2023-04-12 19:03:05.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-Samples.xlsx
+-rw-rw-rw-   0        0        0    19318 2024-03-09 13:42:28.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/acdc-2019-nat-ds-params.py
+-rw-rw-rw-   0        0        0    72210 2024-02-24 20:45:31.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/acdc-2019-nat-ds-run.ipynb
+-rw-rw-rw-   0        0        0    38886 2024-04-01 12:15:09.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/howto.md
+-rw-rw-rw-   0        0        0     3235 2023-05-03 09:51:38.000000 pyaudisam-1.1.0/docs/howto-acdc19-nat/ipython_notebook_toc.js
+-rw-rw-rw-   0        0        0     2275 2024-05-14 19:07:25.000000 pyaudisam-1.1.0/docs/release-notes.md
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:00.058598 pyaudisam-1.1.0/pyaudisam/
+-rw-rw-rw-   0        0        0     2778 2024-04-21 14:38:53.000000 pyaudisam-1.1.0/pyaudisam/__init__.py
+-rw-rw-rw-   0        0        0     1058 2024-03-10 19:01:06.000000 pyaudisam-1.1.0/pyaudisam/__main__.py
+-rw-rw-rw-   0        0        0   159773 2024-05-04 16:23:45.000000 pyaudisam-1.1.0/pyaudisam/analyser.py
+-rw-rw-rw-   0        0        0    19242 2024-04-21 14:30:34.000000 pyaudisam-1.1.0/pyaudisam/analysis.py
+-rw-rw-rw-   0        0        0    81193 2024-05-08 16:24:05.000000 pyaudisam-1.1.0/pyaudisam/data.py
+-rw-rw-rw-   0        0        0    48495 2024-04-21 14:27:52.000000 pyaudisam-1.1.0/pyaudisam/engine.py
+-rw-rw-rw-   0        0        0     7636 2024-04-21 14:27:52.000000 pyaudisam-1.1.0/pyaudisam/executor.py
+-rw-rw-rw-   0        0        0     7881 2023-05-12 13:54:38.000000 pyaudisam-1.1.0/pyaudisam/log.py
+-rw-rw-rw-   0        0        0    68493 2024-05-08 12:45:37.000000 pyaudisam-1.1.0/pyaudisam/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:00.215453 pyaudisam-1.1.0/pyaudisam/mcds/
+-rw-rw-rw-   0        0        0     9859 2024-04-07 16:51:48.000000 pyaudisam-1.1.0/pyaudisam/mcds/anlys.htpl
+-rw-rw-rw-   0        0        0     9101 2024-04-07 16:51:22.000000 pyaudisam-1.1.0/pyaudisam/mcds/fulltop.htpl
+-rw-rw-rw-   0        0        0     6038 2024-04-07 16:58:11.000000 pyaudisam-1.1.0/pyaudisam/mcds/pretop.htpl
+-rw-rw-rw-   0        0        0      686 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/mcds/stat-mod-notes.txt
+-rw-rw-rw-   0        0        0     1988 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/mcds/stat-mod-specs.old.txt
+-rw-rw-rw-   0        0        0     2422 2024-04-01 13:24:15.000000 pyaudisam-1.1.0/pyaudisam/mcds/stat-mod-specs.txt
+-rw-rw-rw-   0        0        0     8957 2024-04-01 13:13:05.000000 pyaudisam-1.1.0/pyaudisam/mcds/stat-mod-trans.txt
+-rw-rw-rw-   0        0        0      834 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/mcds/stat-row-specs.txt
+-rw-rw-rw-   0        0        0     6426 2024-04-07 16:55:19.000000 pyaudisam-1.1.0/pyaudisam/mcds/top.htpl
+-rw-rw-rw-   0        0        0    34495 2024-03-09 21:15:13.000000 pyaudisam-1.1.0/pyaudisam/optanalyser.py
+-rw-rw-rw-   0        0        0    39140 2024-04-21 14:36:27.000000 pyaudisam-1.1.0/pyaudisam/optimisation.py
+-rw-rw-rw-   0        0        0    74772 2024-04-21 14:27:52.000000 pyaudisam-1.1.0/pyaudisam/optimiser.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:00.231090 pyaudisam-1.1.0/pyaudisam/report/
+-rw-rw-rw-   0        0        0      475 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-angle-up.svg
+-rw-rw-rw-   0        0        0      522 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-arrow-left-hover.svg
+-rw-rw-rw-   0        0        0      522 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-arrow-left.svg
+-rw-rw-rw-   0        0        0      527 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-arrow-right-hover.svg
+-rw-rw-rw-   0        0        0      527 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-arrow-right.svg
+-rw-rw-rw-   0        0        0      525 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-arrow-up-hover.svg
+-rw-rw-rw-   0        0        0      525 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-arrow-up.svg
+-rw-rw-rw-   0        0        0      673 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-feather-alt.svg
+-rw-rw-rw-   0        0        0      866 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-file-excel-hover.svg
+-rw-rw-rw-   0        0        0      866 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/fa-file-excel.svg
+-rw-rw-rw-   0        0        0     5281 2022-01-22 16:29:08.000000 pyaudisam-1.1.0/pyaudisam/report/report.css
+-rw-rw-rw-   0        0        0   127312 2024-05-05 14:38:24.000000 pyaudisam-1.1.0/pyaudisam/report.py
+-rw-rw-rw-   0        0        0     2124 2023-05-12 13:54:38.000000 pyaudisam-1.1.0/pyaudisam/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:01.031925 pyaudisam-1.1.0/pyaudisam.egg-info/
+-rw-rw-rw-   0        0        0    10425 2024-05-15 18:44:59.000000 pyaudisam-1.1.0/pyaudisam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11143 2024-05-15 18:44:59.000000 pyaudisam-1.1.0/pyaudisam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:44:59.000000 pyaudisam-1.1.0/pyaudisam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2024-05-15 18:44:59.000000 pyaudisam-1.1.0/pyaudisam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 18:44:59.000000 pyaudisam-1.1.0/pyaudisam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       96 2024-05-09 09:37:52.000000 pyaudisam-1.1.0/pytest.ini
+-rw-rw-rw-   0        0        0      157 2024-02-21 10:58:20.000000 pyaudisam-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       77 2024-05-15 18:45:01.047581 pyaudisam-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3157 2024-02-23 14:45:21.000000 pyaudisam-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:00.513908 pyaudisam-1.1.0/tests/
+-rw-rw-rw-   0        0        0     2975 2024-05-13 19:04:23.000000 pyaudisam-1.1.0/tests/conftest.py
+-rw-rw-rw-   0        0        0   149074 2024-03-19 19:45:23.000000 pyaudisam-1.1.0/tests/devarchives1.ipynb
+-rw-rw-rw-   0        0        0   200169 2024-03-19 19:45:44.000000 pyaudisam-1.1.0/tests/devarchives2.ipynb
+-rw-rw-rw-   0        0        0     3048 2021-10-03 10:04:40.000000 pyaudisam-1.1.0/tests/ipython_notebook_toc.js
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:00.780662 pyaudisam-1.1.0/tests/refin/
+-rw-rw-rw-   0        0        0    57477 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt
+-rw-rw-rw-   0        0        0    57750 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods
+-rw-rw-rw-   0        0        0    14366 2024-05-08 13:55:44.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.ods
+-rw-rw-rw-   0        0        0    11922 2021-12-28 09:03:01.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-SpecsEchants.ods
+-rw-rw-rw-   0        0        0    14103 2024-05-08 13:28:52.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-SpecsOptAnalyses.ods
+-rw-rw-rw-   0        0        0    66148 2021-11-20 20:11:41.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-UnitestOptResultats.ods
+-rw-rw-rw-   0        0        0     5686 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dec-dist.txt
+-rw-rw-rw-   0        0        0     5686 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dotdec-dist.txt
+-rw-rw-rw-   0        0        0     6771 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-6dec-dist.txt
+-rw-rw-rw-   0        0        0     6340 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0    39311 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods
+-rw-rw-rw-   0        0        0    29263 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.ods
+-rw-rw-rw-   0        0        0    16242 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xlsx
+-rw-rw-rw-   0        0        0     2493 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ANTTRI-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0     4881 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-COLPAL-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0   190595 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-DonneesBrutesPourAutoDS.xlsx
+-rw-rw-rw-   0        0        0     3170 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-EMBCIR-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0     2620 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-EMBCIT-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0     6105 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-LUSMEG-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0     2313 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-MILCAL-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0     4165 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-PHYCOL-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0    11401 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-SYLATR-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0     9638 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-1dec-dist.txt
+-rw-rw-rw-   0        0        0    11753 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-6dec-dist.txt
+-rw-rw-rw-   0        0        0    11227 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-ttdec-dist.txt
+-rw-rw-rw-   0        0        0     7440 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-5mn-1dec-dist.txt
+-rw-rw-rw-   0        0        0    51263 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refin/TURMER-10mn-1dec-hnorm-cos.odt
+drwxrwxrwx   0        0        0        0 2024-05-15 18:45:01.031925 pyaudisam-1.1.0/tests/refout/
+-rw-rw-rw-   0        0        0  2038208 2024-05-12 14:32:56.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-OptRapport.ExAicMQua-r900m6q3d15.html
+-rw-rw-rw-   0        0        0   299548 2024-05-09 16:33:23.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-OptRapport.ods
+-rw-rw-rw-   0        0        0   140352 2024-05-08 17:00:04.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-OptResultats.ods
+-rw-rw-rw-   0        0        0    32712 2024-04-07 19:24:40.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-PreRapport.html
+-rw-rw-rw-   0        0        0    32531 2024-04-27 16:55:07.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-PreRapport.ods
+-rw-rw-rw-   0        0        0    12662 2024-04-20 15:00:26.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-PreResultats.ods
+-rw-rw-rw-   0        0        0  1015383 2024-04-27 16:44:59.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-Rapport.html
+-rw-rw-rw-   0        0        0    83055 2024-04-27 16:50:29.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-Rapport.ods
+-rw-rw-rw-   0        0        0    65534 2024-04-27 16:49:57.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Naturalist-extrait-Resultats.ods
+-rw-rw-rw-   0        0        0    24594 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-distance-73.xlsx
+-rw-rw-rw-   0        0        0    19410 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-postcomp.ods
+-rw-rw-rw-   0        0        0     6120 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-5-cols.txt
+-rw-rw-rw-   0        0        0      273 2024-02-19 11:12:12.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-clusters.txt
+-rw-rw-rw-   0        0        0     6120 2024-02-19 11:12:07.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-noextra.txt
+-rw-rw-rw-   0        0        0    13142 2024-02-19 11:12:08.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-withextra.txt
+-rw-rw-rw-   0        0        0    13142 2021-09-26 19:14:02.000000 pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.txt
+-rw-rw-rw-   0        0        0     8204 2024-04-01 16:19:39.000000 pyaudisam-1.1.0/tests/refout/mcds-stat-specs.ods
+-rw-rw-rw-   0        0        0       41 2024-02-22 08:59:31.000000 pyaudisam-1.1.0/tests/requirements.txt
+-rw-rw-rw-   0        0        0    17786 2022-01-22 14:52:05.000000 pyaudisam-1.1.0/tests/sensitivity.ipynb
+-rw-rw-rw-   0        0        0    23779 2024-05-09 10:02:41.000000 pyaudisam-1.1.0/tests/test_unint_analysis_results.py
+-rw-rw-rw-   0        0        0    41948 2024-05-08 17:26:06.000000 pyaudisam-1.1.0/tests/test_unint_data.py
+-rw-rw-rw-   0        0        0    28868 2024-05-08 17:26:24.000000 pyaudisam-1.1.0/tests/test_unint_engine.py
+-rw-rw-rw-   0        0        0    14647 2024-05-08 17:27:00.000000 pyaudisam-1.1.0/tests/test_unint_mcds_analyser.py
+-rw-rw-rw-   0        0        0    13502 2024-05-08 17:27:00.000000 pyaudisam-1.1.0/tests/test_unint_mcds_analysis.py
+-rw-rw-rw-   0        0        0    54265 2024-05-09 09:56:24.000000 pyaudisam-1.1.0/tests/test_unint_mcds_analysis_results.py
+-rw-rw-rw-   0        0        0    20953 2024-05-13 17:54:32.000000 pyaudisam-1.1.0/tests/test_unint_mcds_optanalysis_results.py
+-rw-rw-rw-   0        0        0    45977 2024-05-14 06:17:49.000000 pyaudisam-1.1.0/tests/test_unint_mcds_optimiser.py
+-rw-rw-rw-   0        0        0     3619 2024-05-13 19:30:27.000000 pyaudisam-1.1.0/tests/test_unint_utils_logger.py
+-rw-rw-rw-   0        0        0    39639 2024-05-14 06:26:08.000000 pyaudisam-1.1.0/tests/test_val_mcds_analyser.py
+-rw-rw-rw-   0        0        0    73278 2024-05-12 18:50:17.000000 pyaudisam-1.1.0/tests/test_val_mcds_optanalyser.py
+-rw-rw-rw-   0        0        0    44414 2024-05-12 14:09:06.000000 pyaudisam-1.1.0/tests/test_val_mcds_preanalyser.py
+-rw-rw-rw-   0        0        0   293960 2024-03-19 19:43:56.000000 pyaudisam-1.1.0/tests/unintests.ipynb
+-rw-rw-rw-   0        0        0     9519 2024-05-10 13:12:58.000000 pyaudisam-1.1.0/tests/unintval_utils.py
+-rw-rw-rw-   0        0        0   129288 2024-03-19 19:44:39.000000 pyaudisam-1.1.0/tests/valarchives.ipynb
+-rw-rw-rw-   0        0        0    21346 2024-05-12 14:27:33.000000 pyaudisam-1.1.0/tests/valtests-ds-params.py
+-rw-rw-rw-   0        0        0   154501 2024-05-14 10:38:58.000000 pyaudisam-1.1.0/tests/valtests.ipynb
```

### Comparing `pyaudisam-1.0.2/LICENSE.txt` & `pyaudisam-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/MANIFEST.in` & `pyaudisam-1.1.0/MANIFEST.in`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 include README.md
 include LICENSE.txt
 include requirements.txt
-
+include .coveragerc
+include pytest.ini
 include pyaudisam/mcds/*.htpl
 include pyaudisam/mcds/*.txt
 include pyaudisam/report/*.css
 include pyaudisam/report/*.svg
 
+include tests/requirements.txt
 include tests/*.py
 include tests/*.ipynb
 include tests/*.js
 
 include tests/refin/*.txt
 include tests/refin/*.xlsx
 include tests/refin/*.ods
 include tests/refin/*.odt
 
 include tests/refout/*.txt
 include tests/refout/*.xlsx
 include tests/refout/*.ods
+include tests/refout/*.html
 prune tests/refout/dist-order-sens-min
 
+include docs/release-notes.md
+
 include docs/howto-acdc19-nat/*.md
 include docs/howto-acdc19-nat/*.xlsx
 exclude docs/howto-acdc19-nat/*.autogen.xlsx
 include docs/howto-acdc19-nat/*.py
 include docs/howto-acdc19-nat/*.ipynb
 include docs/howto-acdc19-nat/*.js
 include docs/howto-acdc19-nat/*.kml
```

### Comparing `pyaudisam-1.0.2/PKG-INFO` & `pyaudisam-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,151 +1,158 @@
-Metadata-Version: 2.1
-Name: pyaudisam
-Version: 1.0.2
-Summary: Distance Sampling automation through python and Distance sofware
-Home-page: https://github.com/denmedius/pyaudisam
-Author: denmedius
-Author-email: fefeqe22.vucuqu82@murena.io
-License: GPLv3+
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Environment :: Win32 (MS Windows)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy<1.25,>=1.16
-Requires-Dist: pandas<1.3,>=0.25
-Requires-Dist: openpyxl<3.2,>=3
-Requires-Dist: xlrd~=2.0
-Requires-Dist: matplotlib<3.8,>=3.1
-Requires-Dist: jinja2<3.2,>=2.10
-Requires-Dist: zoopt==0.4.0
-Requires-Dist: packaging
-
-# Python module for AUtomated DIstance SAMpling analyses
-
-This module interfaces **distance sampling** analysis engines from [Distance software](https://distancesampling.org/), and possibly others in the future ; thus, it has been designed in order to make it easier :
-* to run (in parallel) numerous [Distance Sampling](https://en.wikipedia.org/wiki/Distance_sampling) analyses with many (many) parameter variants on many field observation samples
-  (possibly using some optimisation techniques for automated computation of right and left distance truncations),
-* to select the best analysis variant results through a mostly automated process, based on customisable statistical
-  quality indicators,
-* to produce partly customisable reports in spreadsheet (numerical results only) and HTML formats
-  (more complete, with full-featured plots like in Distance, and more).
-
-As for now, only the Windows MCDS.exe V6 engine and Point Transect analyses are supported, and so, it runs only under Windows.
-
-## Requirements
-
-The module itself was actually tested extensively with:
-* python 3.8 only
-* pandas 0.25 to 1.2.5
-* openpyxl 3.0 to 3.1.2
-* matplotlib 3.1 to 3.7
-* jinja2 2.10 to 3.1
-* zoopt 0.4.0
-* xlrd 2.0 (only for .xls format support)
-
-You will get no support outside of this (but porting to python 3.12 is planned for 2024).
-
-As for testing:
-* pytest, pytest-cov
-* plotly (sometimes)
-* xlrd >= 2 (only for old .xls format support)
-
-## Installation
-
-You can install **pyaudisam** from [PyPI](https://pypi.org/project/pyaudisam/) in your current python environment (conda or venv, whatever):
-
-`$ pip install pyaudisam`
-
-TODO: Publish also on [Conda Forge](https://conda-forge.org/), probably following [this recipe](https://jacobtomlinson.dev/posts/2020/publishing-open-source-python-packages-on-github-pypi-and-conda-forge/#conda-forge).  
-
-Or from a downloaded source package:
-
-`$ pip install pyaudisam-1.0.2.tar.gz`
-
-Or from a downloaded wheel package:
-
-`$ pip install pyaudisam-1.0.2-py3-none-any.whl`
-
-Or even directly from GitHub:
-
-* `$ pip install git+https://github.com/pypa/sampleproject.git@1.0.2`
-* `$ pip install git+https://github.com/pypa/sampleproject.git@main`
-
-## Usage
-
-As a **python package**, pyaudisam can be used through its python API.
-
-But there's also a **command-line interface**: try and run it with the -h/--help option.
-
-`python -m pyaudisam --help`
-
-Whichever method, the best way to go is to read the concrete quick-start guide : see [Documentation](#documentation) below.
-
-## Documentation
-
-* a short ["how it works" guide](https://github.com/denmedius/pyaudisam/blob/main/docs/how-it-works/how-it-works-en.md) to understand the basics (also in [French](https://github.com/denmedius/pyaudisam/blob/main/docs/how-it-works/how-it-works-fr.md)),
-* a concrete ["quick-start" guide](https://github.com/denmedius/pyaudisam/blob/main/docs/howto-acdc19-nat/howto.md) with a real life use case and relevant field data to play with,
-* another similar but shorter concrete ["quick-start guide" (in French)](http://jpmeuret.free.fr/ds/acdc19/materiau-public.zip) (command-line only) with the full field data set of the "ACDC 2019" birding study.
-
-Note: You can also get a detailled idea of how to use pyaudisam python API by playing with the fully functional [jupyter](https://jupyter.org/) notebook [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) (see below [Running tests](#running-tests) for how to obtain and run it).
-
-TODO:
-* complete the quick start guides above by other small and focused articles to explain some mandatory details:
-  - how to build a sample or analysis specification workbook (see a short draft in [analyser.py:273](https://github.com/denmedius/pyaudisam/blob/main/pyaudisam/analyser.py)),
-  - ...
-* write a technical documentation of the whole module,
-* write a guide for building the module API documentation ([sphinx](https://www.sphinx-doc.org/) should work out of the box as [reStructured text](https://en.wikipedia.org/wiki/ReStructuredText) has been used in docstrings),
-
-## Running tests
-
-You first need to clone the [source tree](https://github.com/denmedius/pyaudisam) or download and install a [source package](https://pypi.org/project/pyaudisam/#files): once done, look in the _tests_ sub-folder, everything's inside :
-* some tests are fully automated : after installing pytest, simply run it:
-
-  `pytest`
-
-* for code corevage during tests, after installing pytest-cov, simply run:
-
-  `pytest --cov`
-
-* some other tests not: they are implemented as [jupyter notebooks](https://jupyter.org/) (see [tests/unintests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/unintests.ipynb) and [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) that you must run step by step, as long as no one has fully automated them :-).
-
-## Building
-
-To build pyaudisam [PyPI](https://pypi.org/project/pyaudisam/) source and binary packages, you first need to clone the [source tree](https://github.com/denmedius/pyaudisam) or download and extract a [source package](https://pypi.org/project/pyaudisam/#files): once done, it's as simple as:
-
-`python -m build`
-
-Note: Don't care about warnings about pyaudisam.mcds and pyaudisam.report being recognised as importable,
- but being absent from setuptools' packages configuration ... these folders simply contain
- pyaudisam config. and data files, no python code at all.
-
-## Contributing
-
-Merge requests are very welcome !
-
-And if you are lacking ideas, here are some good ones below ;-)
-
-### To do list
-
-* finish tests automation (move and complete[tests/unintests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/unintests.ipynb) and [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) notebooks code to pytest scripts, after checking the state of this work in progress in tests/\*\_test.py scripts),
-* make pyaudisam work under Linux / Mac OS (all python: OK, but calling MCDS.exe):
-  - or: through some kind of external client-server interface to MCDS.exe (that runs only under Windows),
-  - or: by porting MCDS to Linux (closed Fortran source, but old, so might be obtained through a polite request to [this Distance Sampling forum](https://groups.google.com/g/distance-sampling) ; BUT, needs an IMSL license, which is horribly expensive).
-  - or: by rewriting MCDS from scratch, or by porting the [MRDS Distance package](https://distancesampling.org/) to Python,
-  - or: by rewriting MCDS using the [MRDS Distance package](https://distancesampling.org/), meaning some kind of interface to R,
-* build a GUI for pyaudisam command-line (with some kind of "project" concept, and parameter set template, and ...),
-* add support for line transects (only point transects for the moment),
-* add support for the co-variates feature of MCDS,
-* ...
-
-### Some hints
-
-Some formal things that I don't plan to change (let's concentrate on substantive content) :-)
-* this code is not blacked or isorted or fully conform to pep8 (but it's clean, commented, and it works),
-* the identifier naming scheme used is old-fashioned: camel case everywhere.
+# PYthon module for AUtomated DIstance SAMpling analyses
+
+This module interfaces **distance sampling** analysis engines from [Distance software](https://distancesampling.org/), and possibly others in the future ; thus, it has been designed in order to make it easier :
+* to run (in parallel) numerous [Distance Sampling](https://en.wikipedia.org/wiki/Distance_sampling) analyses with many (many) parameter variants on many field observation samples
+  (possibly using some optimisation techniques for automated computation of right and left distance truncations),
+* to select the best analysis variant results through a mostly automated process, based on customisable statistical
+  quality indicators,
+* to produce partly customisable reports in spreadsheet (numerical results only) and HTML formats
+  (more complete, with full-featured plots like in Distance, and more).
+
+As for now, only the Windows MCDS.exe 6.x (Distance 6 to 7.3) and 7.4 (Distance 7.4 and 7.5 at least) engine and Point Transect analyses are supported, and so, it runs only under Windows.
+
+## Requirements
+
+The module itself was actually tested extensively with:
+* python 3.8 only
+* pandas 0.25 to 1.2.5
+* openpyxl 3.0 to 3.1.2
+* matplotlib 3.1 to 3.7
+* jinja2 2.10 to 3.1
+* zoopt 0.4.0
+* xlrd 2.0 (only for .xls format support)
+
+You will get no support outside of this (but porting to python 3.12 & pandas 2.x is planned for 2024 or 2025).
+
+As for testing:
+* pytest, pytest-cov
+* plotly (sometimes)
+
+## Installation
+
+You can install **pyaudisam** from [PyPI](https://pypi.org/project/pyaudisam/) in your current python environment (conda or venv, whatever):
+
+`pip install pyaudisam`
+
+Or from a downloaded source package:
+
+`pip install pyaudisam-1.1.0.tar.gz`
+
+Or from a downloaded wheel package:
+
+`pip install pyaudisam-1.1.0-py3-none-any.whl`
+
+Or even directly from GitHub:
+
+* `pip install git+https://github.com/pypa/sampleproject.git@1.1.0`
+* `pip install git+https://github.com/pypa/sampleproject.git@main`
+
+## Usage
+
+As a **python package**, pyaudisam can be used through its python API.
+
+But there's also a **command-line interface**: try and run it with the -h/--help option.
+
+`python -m pyaudisam --help`
+
+Whichever method, the best way to go is to read the concrete quick-start guide : see [Documentation](#documentation) below
+(but be aware that you'll need to install an external Distance Sampling engine, like MCDS, to run analyses with paudisam).
+
+## Documentation
+
+* a short ["how it works" guide](https://github.com/denmedius/pyaudisam/blob/main/docs/how-it-works/how-it-works-en.md) to understand the basics (also in [French](https://github.com/denmedius/pyaudisam/blob/main/docs/how-it-works/how-it-works-fr.md)),
+* a concrete ["quick-start" guide](https://github.com/denmedius/pyaudisam/blob/main/docs/howto-acdc19-nat/howto.md) with a real life use case and relevant field data to play with,
+* another similar but shorter concrete ["quick-start guide" (in French)](http://jpmeuret.free.fr/ds/acdc19/materiau-public.zip) (command-line only) with the full field data set of the "ACDC 2019" birding study.
+
+Note: You can also get a detailed idea of how to use pyaudisam python API by playing with the fully functional [jupyter](https://jupyter.org/) notebook [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) (see below [Running tests](#running-tests) for how to obtain and run it).
+
+## Testing
+
+You first need to clone the [source tree](https://github.com/denmedius/pyaudisam) or download and install a [source package](https://pypi.org/project/pyaudisam/#files): once done, look in the _tests_ sub-folder, everything's inside.
+
+Then, you need to install test dependencies:
+
+`pip install pyaudisam[test]`
+
+Some tests are fully automated, simply run:
+
+`pytest`
+
+For code coverage during tests, simply run:
+
+`pytest --cov`
+
+Or even, if you want an HTML report with annotated code coverage:
+
+`pytest --cov --cov-report html`
+
+Note: Some other tests are not yet automated: they are implemented as [jupyter notebooks](https://jupyter.org/) (see [tests/unintests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/unintests.ipynb) and [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) that you must run step by step, as long as no one has fully automated them :-).
+
+## Building
+
+To build pyaudisam [PyPI](https://pypi.org/project/pyaudisam/) source and binary packages, you need:
+* a source tree (clone the [source tree](https://github.com/denmedius/pyaudisam) or download and extract a [source package](https://pypi.org/project/pyaudisam/#files)),
+* a python environment where pyaudisam works,
+* the `build` module (to install through pip as an example).
+
+Then, it's as simple as:
+
+`python -m build`
+
+You'll get 2 files in the `dist` folder (ex. for version 1.1.0) :
+* the wheel package: `pyaudisam-1.1.0-py3-none-any.whl`
+* the source package: `pyaudisam-1.1.0.tar.gz`
+
+## Contributing
+
+Merge requests are very welcome !
+
+And if you are lacking ideas, here are some good ones below ;-)
+
+### To do list
+
+* documentation:
+  * complete the quick start guides above by other small and focused articles to explain some mandatory details:
+    * how to build a sample or analysis specification workbook (see a short draft in [analyser.py:273](https://github.com/denmedius/pyaudisam/blob/main/pyaudisam/analyser.py)),
+    * ...
+  * write a technical documentation of the whole module and sub-modules,
+  * write a guide for building the module API documentation ([sphinx](https://www.sphinx-doc.org/) should work out of the box as [reStructured text](https://en.wikipedia.org/wiki/ReStructuredText) has been used in docstrings),
+* code quality and tests:
+  * add more tests for improving code coverage (thanks to HTML coverage report),
+  * configure and run pylint, and follow its useful advices, 
+  * main: split \_Application.\_run in feature sub-functions for clarity,
+* features:
+  * add support for line transects (only point transects for the moment),
+  * add support for the co-variates feature of MCDS,
+  * integrate the notebook prototype of "final reports" (workbook, HTML, and OpenDoc text formats) to automate most of the work of producing a publication-grade "full results appendix" for a Distance Sampling study (based on the auto-filtered report, but with semi-automated diagnosis at sample and analysis level in order to help in the final choice for each sample),
+  * add more features for selecting sample data before running analyses (to avoid the need of creating multiple data sets, run multiple analysis sessions, and then re-aggregate results and reports manually): exclude some specific transects, pre-truncate data above some fixed distance, ...
+* packaging:
+  * publish also pyaudisam on [Conda Forge](https://conda-forge.org/), probably following [this recipe](https://jacobtomlinson.dev/posts/2020/publishing-open-source-python-packages-on-github-pypi-and-conda-forge/#conda-forge),
+* platform support:
+  * add support for newer Python versions (probably 3.12 now) and updated pandas (2+) and zoopt dependencies,
+  * make pyaudisam work under Linux / macOS (all python: OK, but ... calling MCDS.exe, that runs exclusively under Windows):
+    * or: through some kind of external client-server interface to MCDS.exe (that runs only under Windows),
+    * or: by porting MCDS to Linux (closed Fortran source, but old, so might be obtained through a polite request to [this Distance Sampling forum](https://groups.google.com/g/distance-sampling) ;
+      BUT, you'll need an IMSL license, which is horribly expensive).
+    * or: by rewriting MCDS from scratch, or by porting the [MRDS Distance package](https://distancesampling.org/) to Python,
+    * or: by rewriting MCDS using the [MRDS Distance package](https://distancesampling.org/), meaning some kind of interface to R,
+* user interface:
+  * build a GUI for pyaudisam command-line (with some kind of "project" concept, and parameter set template, and ...),
+* ...
+
+### Known issues
+
+* AnalysisResultsSet.toOpenDoc sometimes produces broken header rows (the 3-row multi-index header is not rendered as it is on the right side),
+* The new undocumented MCDS 7.4 result column names are not translated correctly (switched fr and en translations) (minor, as not used actually for the moment),
+* The "Details" table header is not translated in auto-filtered reports (whereas the "Synthesis" one is),
+* Too many decimals rendered for the Max/Min dist figures in HTML reports when the distance unit is "meter",
+* The colorisation of HTML and workbook auto-filtered reports is of no use as it is now (need for a full rework).
+
+### Release notes
+
+You can [read them here](https://github.com/denmedius/pyaudisam/blob/main/docs/release-notes.md) :-)
+
+### Some hints
+
+Some formal things that I don't plan to change (let's concentrate on substantive content) :-)
+* this code is not blacked or isorted or fully conform to pep8 (but it's clean, commented, and it works),
+* the identifier naming scheme used is old-fashioned: camel case everywhere.
```

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-left-hover.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-left-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-left.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-left.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-right-hover.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-right-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-right.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-right.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-up-hover.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-up-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-arrow-up.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-feather-alt.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-feather-alt.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-file-excel-hover.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-file-excel-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/fa-file-excel.svg` & `pyaudisam-1.1.0/docs/how-it-works/common/fa-file-excel.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/common/report.css` & `pyaudisam-1.1.0/docs/how-it-works/common/report.css`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/how-it-works-en.md` & `pyaudisam-1.1.0/docs/how-it-works/how-it-works-en.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 In the second mode, known as "**analysis mode**",
 * as input, it is provided with
     - the set of **individualised data** (the same as for the "pre-analysis" mode: the data of the selected samples will be extracted automatically),
     - the **list of samples to be analysed**: as in the "pre-analysis" mode, but a priori a subset, the pre-analyses being made to filter the non-exploitable samples,
     - the **combinations of analysis parameters to be covered for each sample**; this time, it is different from the pre-analysis mode: it is necessary to specify what one wants to do: model x fit series x left truncation distance x right truncation distance x number of distance slices to be considered for the modelling (N.B. for these last 3 parameters, an "automatic" mode makes it possible not to have to specify the values, and to let the software seek them itself by numerical optimisation of the statistical quality of the results of the DS analysis), 
 * The software then automatically carries out the following main steps:
     - for the "automatic truncation" parameter combinations, **automatic determination of the left and right truncation distances** by an optimisation technique (launch of numerous analyses by varying the said truncations within limits set by the number of ignored data, considered as "outliers", ... and retaining only the best set of truncations (left and/or right) according to a "combined quality" indicator / criterion based on the indicators produced by MCDS and the analysis parameters (see below for a first overview, and chapter II for all the details);
-    - **execution of the individual analyses** corresponding to each of the parameter combinations (with truncations now all fixed) for each sample: as for manual analyses via the Distance 7 software, its MCDS V6 calculation "engine" is used, in "Conventional Distance Sampling" mode (no co-variable); the results thus produced feed a table in which each line corresponds to an analysis, i.e. to one of the parameter combinations for each sample; these results are those produced directly by MCDS V6, and completed by the "combined quality" indicator specific to pyaudisam
+    - **execution of the individual analyses** corresponding to each of the parameter combinations (with truncations now all fixed) for each sample: as for manual analyses via the Distance 7 software, its MCDS 6 or 7 calculation "engine" is used, in "Conventional Distance Sampling" mode (no co-variable); the results thus produced feed a table in which each line corresponds to an analysis, i.e. to one of the parameter combinations for each sample; these results are those produced directly by MCDS, and completed by the "combined quality" indicator specific to pyaudisam
     - **automatic sorting and filtering of results** according to their "**combined quality**": for each sample, following a sequence of steps similar to what a human analyst would do "manually" when looking for the "best" analysis result among those corresponding to multiple parameter combinations,
     	+ only retain analyses with non-identical results, to within one epsilon (for raw statistical criteria at the output of MCDS, calculated densities and detection probabilities, as well as their confidence intervals)
         + only retain analyses with no errors reported by MCDS (but analyses with warnings retained),
         + for analyses with strictly identical truncations, keep only the N with the best AIC (configurable N),
         + for analyses with close truncations, keep only the one (only 1) with the best Chi2, the best KS with identical Chi2, the best DCv with identical Chi2 and KS (Chi2 and KS tests = Kolmogorov-Smirnov, DCv = 95% variability of the estimated density),
         + only retain analyses that are "truncated in distance" to less than X% (i.e. for which the truncations in distance to the left and/or to the right have not eliminated more than X% of the total number of birds contacted) (configurable X),
         + keep only the remaining analyses with the best "combined quality" criteria, provided they exceed the minimum value Y (configurable),
```

### Comparing `pyaudisam-1.0.2/docs/how-it-works/how-it-works-fr.md` & `pyaudisam-1.1.0/docs/how-it-works/how-it-works-fr.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Dans le second mode dit "d'**analyse**",
 * en entrée, on lui fournit
     - l'ensemble des données individualisées (le même que pour le mode "pré-analyse" : les données des échantillons choisis en seront extraites automatiquement),
     - la liste des échantillons à analyser : comme dans le mode "pré-analyse", mais à priori un sous-ensemble, les pré-analyses étant faites pour filtrer les échantillons non exploitables,
     - les combinaisons de paramètres d'analyse à couvrir pour chaque échantillon ; cette fois, c'est différent du mode pré-analyse : il faut spécifier ce que l'on veut faire : modèle x série d'ajustement x troncature en distance à gauche x troncature en distance à droite x nombre de tranches de distance à considérer pour la modélisation (N.B. pour ces 3 derniers paramètres, un mode "automatique" permet de ne pas avoir à spécifier les valeurs, et de laisser le logiciel les chercher lui-même par optimisation numérique de la qualité statistique des résultats de l'analyse DS), 
 * le logiciel enchaîne ensuite automatiquement les grandes étapes suivantes :
     - pour les combinaisons de paramètres "à troncatures automatiques", détermination automatique des distances de troncatures à gauche et à droite par une technique d'optimisation (lancement de nombreuses analyses en faisant varier les dites troncatures dans des limites paramétrées par le nombre de données ignorées, considérées comme des "outliers", ... et en ne retenant que le meilleur jeu de troncatures (à gauche et/ou à droite) selon un indicateur / critère de "qualité combinée" à partir des indicateurs produits par MCDS et des paramètres d'analyses (voir ci-dessous pour un 1er survol, et chapitre II pour tous les détails) ;
-    - exécution des analyses individuelles correspondant à chacune des combinaisons de paramètres (à troncatures maintenant toutes fixées) pour chaque échantillon : comme lors d'analyses manuelles via le logiciel Distance 7, c'est son "moteur" de calcul MCDS V6 qui est utilisé, en mode "Conventional Distance Sampling" (pas de co-variable) ; les résultats ainsi produits alimentent ainsi une table dont chaque ligne correspond à une analyse, c'est à dire à l'une des combinaisons de paramètres pour chaque échantillon ; ces résultats sont ceux produits directement par MCDS V6, et complétés par l'indicateur de "qualité combinée" spécifique à pyaudisam
+    - exécution des analyses individuelles correspondant à chacune des combinaisons de paramètres (à troncatures maintenant toutes fixées) pour chaque échantillon : comme lors d'analyses manuelles via le logiciel Distance 7, c'est son "moteur" de calcul MCDS 6 ou 7 qui est utilisé, en mode "Conventional Distance Sampling" (pas de co-variable) ; les résultats ainsi produits alimentent ainsi une table dont chaque ligne correspond à une analyse, c'est à dire à l'une des combinaisons de paramètres pour chaque échantillon ; ces résultats sont ceux produits directement par MCDS, et complétés par l'indicateur de "qualité combinée" spécifique à pyaudisam
     - tri et filtrage automatique des résultats selon leur "qualité combinée" : pour chaque échantillon, suivant une suite d'étapes proche de ce que ferait "manuellement" un analyste humain cherchant le "meilleur résultat" d'analyse parmi ceux correspondant à de multiples combinaisons de paramètres,
         + ne conserver que les analyses à résultats non "identiques", à un epsilon près (pour les critères statistiques bruts en sortie de MCDS, les densités et probabilité de détection calculées, ainsi que leurs intervalles de confiance)
         + ne conserver que les analyses sans erreur rapportée par MCDS (analyses à "warnings" conservées),
         + pour les analyses à troncatures strictement identiques, ne conserver que les N ayant les meilleurs AIC (N paramétrable),
         + pour les analyses à troncatures proches, ne conserver que celle (1 seule) ayant le meilleur Khi2, le meilleur KS à Khi2 identique, le meilleur DCv à Khi2 et KS identiques (tests du Khi2 et de KS =  Kolmogorov-Smirnov, DCv = variabilité à 95% de la densité estimée),
         + ne conserver que les analyses "tronquées en distance" à moins de X % (i.e. pour lesquelles les troncatures en distance à gauche et/ou à droite n'ont pas éliminé plus de X % des oiseaux contactés au total) (X paramétrable),
         + ne conserver que les analyses restantes ayant les meilleurs critères de "qualité combinée", pourvu qu'ils dépassent la valeur minimale Y (paramétrable),
```

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report-partview.ExAicMQua-r925m8q3d12.jpg` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report-partview.ExAicMQua-r925m8q3d12.jpg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.ExAicMQua-r925m8q3d12.html` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.ExAicMQua-r925m8q3d12.html`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.xlsx` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat-optanalyses-report.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat.230430-153402.log` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat.230430-153402.log`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/ACDC2019-Nat.230430-162324.log` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/ACDC2019-Nat.230430-162324.log`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/cmd.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/cmd.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/data.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/data.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/detprob1.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/detprob1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/disthist.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/disthist.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/index.html` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/index.html`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/log.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/log.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/output.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/output.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/plots.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/plots.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/probdens1.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/probdens1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/qqplot.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/qqplot.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/stats.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ma-7ak3cu9l/stats.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/cmd.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/cmd.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/data.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/data.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/detprob1.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/detprob1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/disthist.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/disthist.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/index.html` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/index.html`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/log.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/log.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/output.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/output.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/plots.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/plots.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/probdens1.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/probdens1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/qqplot.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/qqplot.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/stats.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-la-ra-ma-90vq_6nr/stats.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/cmd.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/cmd.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/data.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/data.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/detprob1.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/detprob1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/disthist.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/disthist.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/index.html` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/index.html`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/log.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/log.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/output.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/output.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/plots.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/plots.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/probdens1.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/probdens1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/qqplot.png` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/qqplot.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/stats.txt` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/SylvAtri-ab-10mn-m-haz-pol-ma-w3hq64b3/stats.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/optanlys/acdc-2019-nat-ds-params.py` & `pyaudisam-1.1.0/docs/how-it-works/optanlys/acdc-2019-nat-ds-params.py`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report-partview.jpg` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report-partview.jpg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.html` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.html`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.xlsx` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat-preanalyses-report.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat.230416-180310.log` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat.230416-180310.log`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/ACDC2019-Nat.230416-185538.log` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/ACDC2019-Nat.230416-185538.log`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/cmd.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/cmd.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/data.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/data.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob1.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob2.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob2.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob3.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/detprob3.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/disthist.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/disthist.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/index.html` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/index.html`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/log.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/log.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/output.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/output.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/plots.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/plots.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens1.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens2.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens2.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens3.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/probdens3.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/qqplot.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/qqplot.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/stats.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/PrunModu-ab-10mn-m-uni-cos-f3smf1_a/stats.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/cmd.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/cmd.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/data.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/data.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob1.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob2.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob2.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob3.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/detprob3.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/disthist.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/disthist.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/index.html` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/index.html`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/log.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/log.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/output.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/output.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/plots.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/plots.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens1.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens1.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens2.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens2.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens3.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/probdens3.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/qqplot.png` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/qqplot.png`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/stats.txt` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/SylvAtri-ab-10mn-m-haz-cos-fx8uk14r/stats.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/how-it-works/preanlys/acdc-2019-nat-ds-params.py` & `pyaudisam-1.1.0/docs/how-it-works/preanlys/acdc-2019-nat-ds-params.py`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-108-points-300m-circles.kml` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-108-points-300m-circles.kml`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-Nat-ObsIndivDist.xlsx` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-Nat-ObsIndivDist.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-OptAnalysesToDo.xlsx` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-OptAnalysesToDo.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/ACDC2019-Samples.xlsx` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/ACDC2019-Samples.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/acdc-2019-nat-ds-params.py` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/acdc-2019-nat-ds-params.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 # d. Analyses to run : auto-extraction from opt-analyses spec. file ...
 #    (by simply removing 'auto' truncation parameters)
 analysisSpecFile = dataDir / f'{studyName}-AnalysesToDo.autogen.xlsx'
 
 _ddfAnlysSpecs = pd.read_excel(dataDir / f'{studyName}-OptAnalysesToDo.xlsx', sheet_name=None)
 with pd.ExcelWriter(analysisSpecFile) as xlWrtr:
     for sn in _ddfAnlysSpecs:
-        if sn != 'TroncaturesAuto_impl':
+        if sn != 'AutoTruncations_impl':
             _ddfAnlysSpecs[sn].to_excel(xlWrtr, sheet_name=sn, index=False)
 
 # e. Parameters for computations run and follow-up
 runAnalysisMethod = 'subprocess.run'
 runAnalysisTimeOut = 300
 logAnalysisData = False
 logAnalysisProgressEvery = 5
```

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/acdc-2019-nat-ds-run.ipynb` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/acdc-2019-nat-ds-run.ipynb`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/howto.md` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/howto.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,20 @@
 
     `python -m pyaudisam -h`
 
 Note: As an alternative to installing pyaudisam in your python environment (through conda or pip) after activating it, you can also apply the commands of the following chapters (just as they are, no change) after first:
 1. extracting a source package of pyaudisam 1.0.0 or newer after downloading it from [pypi.org](https://pypi.org/project/pyaudisam/),
 2. set the PYTHONPATH env. variable to the absolute path of the root folder of the extracted tree (example: /c/my/dev/pyaudisam-1.0.0 for ... the 1.0.0 release).
 
+Note: pyaudisam will auto-detect MCDS.exe, the executable of the Distance Sampling engine (the only one supported as for now), if it was installed through the Distance software ; alternatively, you can put a copy of this (standalone) executable:
+* in one of the folders specified through the 'MCDS_PATH' environment variable (individual paths separated by ';', left one are tried first),
+* in a 'Distance 7' (or 'Distance 6') sub-folder of the current folder of your terminal or notebook, 
+* in a 'Distance 7' (or 'Distance 6') sub-folder of the C:/PortableApps folder ;
+* then, if no MCDS.exe found in the above folders (first ones searched first), pyaudisam with search in standard installation folders for Distance 7 or 6.
+
 
 ## B. pyaudisam as a command line tool
 
 ### 1. Background and tips
 
 For running any pyaudisam processing on the "ACDC 2019 Nat" dataset, you'll always use a **command line starting by**:
 
@@ -313,15 +319,15 @@
 
 #### d. Full (rather than "filtered") reports
 
 This is generally not what you want, as you trust pyaudisam filtering system and don't want to examine all the analyses yourself one by one :-).
 
 But in case you really want to get exhaustive **reports**, showing the resuls **of all the analyses** run, without any filtering (beware of the total number !), you can go with the "**full**" Excel and HTML report types:
 
-`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./optanlys -o -f html:full,excel:full -u`
+`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./optanlys/YYMMDD-HHMMSS -f html:full,excel:full -u`
 
 The produced Excel report workbook: `ACDC2019-Nat-optanalyses-report.xlsx` is actually just the same as the "filtered" one (see above), except that it **does not contain any "filtered" sheet** ; which means that it not actually usefull, as it is really a subset of the filtered report. Note that here, due to some specific settings in `acdc-2019-ds-params.py`, especially about row sorting, the results are not in the same order (sorted by increasing left and right truncation distance, and then only by decreasing Qual Bal 3 indicator) ; but you can change the settings !
 
 Warning: If you generate the "full" Excel report (`-f excel:full`) after generating the "filtered" one (only `-f excel`), the first one will be overwritten by the second one, as they share the same name `ACDC2019-Nat-optanalyses-report.xlsx` (but not a big deal, as `-f excel:full` is probably useless).
 
 Notes: When filters are available in `-p acdc-2019-nat-ds-params.py`, using `excel:full` as a report specifier prevents the "filtered" sheets (1 for each filter) to be generated ; with simply `excel`, you'll get both types of report in the same workbook: the filtered one (1 sheet for each filter) + the full one (`synthesis` and `details` sheets).
 
@@ -350,29 +356,29 @@
 
 To **generate** both HTML and Excel **filtered reports** (the HTML one only for the `MFTA-ExAicMQua-r950m8q3d10` filter), from the results of the analyses just run:
 
 1. retrieve the `./anlys/<date>-<hour>` folder where the analysis results were just written: easy, copy it from the console log ; let's say it's `YYMMDD-HHMMSS`.
 
 2. generate the (filtered) reports (as always, run first without `-u` to check what's going on):
 
-`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./anlys/YYMMDD-HHMMSS -f excel,html:r950 -u`
+`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./anlys/YYMMDD-HHMMSS -r excel,html:r950 -u`
 
 
 #### c. Run and report in 1 command
 
 You can also run and report analyses the same way in one command only:
 
-`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./anlys -a -f excel,html:r950 -u`
+`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./anlys -a -r excel,html:r950 -u`
 
 
 #### d. Full (rather than "filtered") report
 
 This is generally not what you want (see above), but in case you want it, you can go with the "**full**" report types:
 
-`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./anlys -o -f html:full,excel:full -u`
+`python -m pyaudisam -p acdc-2019-nat-ds-params.py -w ./anlys/YYMMDD-HHMMSS -r excel:full,html:full -u`
 
 
 ### 5. Export sample data files ready for manual analyses through Distance
 
 In some cases, you might have doubts about some analysis results produced and reported above, or some needed / not needed combination of analysis parameters to try, or ... etc.
 
 Then you might need to fall back to the Distance software to run things manually for a few analyses / samples.
```

### Comparing `pyaudisam-1.0.2/docs/howto-acdc19-nat/ipython_notebook_toc.js` & `pyaudisam-1.1.0/docs/howto-acdc19-nat/ipython_notebook_toc.js`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/__init__.py` & `pyaudisam-1.1.0/pyaudisam/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 
 # Module version
-__version__ = '1.0.2'
+__version__ = '1.1.0'
 
 import os
 import sys
 import platform
 
 
 # Infos about run-time (Python version, dependency library versions, ... + also updated by submodules)
@@ -49,12 +49,12 @@
 
 from .optimiser import DSParamsOptimiser, MCDSTruncationOptimiser, MCDSZerothOrderTruncationOptimiser
 
 from .optanalyser import MCDSTruncationOptanalyser, MCDSTruncOptanalysisResultsSet
 
 from .report import MCDSResultsPreReport, MCDSResultsFullReport, MCDSResultsFilterSortReport
 
-from .utils import loadPythonData
+from .main import main
 
 # Sort and update runtime last bits
 runtime.update(pyaudisam=f'{__version__}')
-runtime.update({'DS engine': runtime.pop('DS engine')})
+runtime.update({'MCDS engine': MCDSEngine.ExeFilePathName.as_posix(), 'MCDS engine version': MCDSEngine.ExeVersion})
```

### Comparing `pyaudisam-1.0.2/pyaudisam/__main__.py` & `pyaudisam-1.1.0/tests/test_val_mcds_preanalyser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,966 +1,893 @@
 # coding: utf-8
-
 # PyAuDiSam: Automation of Distance Sampling analyses with Distance software (http://distancesampling.org/)
-
 # Copyright (C) 2021 Jean-Philippe Meuret
 
 # This program is free software: you can redistribute it and/or modify it under the terms
 # of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 
-# Package main script, for when pyaudisam is invoked through "python -m"
-import re
-import sys
-import atexit
-import tempfile
+# Automated validation tests for "analyser" submodule: MCDSPreAnalyser class,
+# and "reports" submodule: MCDSResultsPreReport class and bases (adapted from valtest.ipynb notebook)
+
+# To run : simply run "pytest" and see ./tmp/val.pnr.{datetime}.log for detailed test log
+
+import time
 import pathlib as pl
-import argparse
+import shutil
 
+import numpy as np
 import pandas as pd
 
-from . import log, runtime
-from .utils import loadPythonData
-from .analyser import MCDSAnalyser, MCDSPreAnalyser, FilterSortSchemeIdManager
-from .optanalyser import MCDSTruncationOptanalyser
-from .report import MCDSResultsPreReport, MCDSResultsFullReport, MCDSResultsFilterSortReport
-
-
-class Logger:
-
-    """Local logger, taking care of output log file at exit time"""
-
-    DefLogNamePrefix = 'pyaudisam-main'
-
-    def __init__(self, runTimestamp, level=log.INFO):
-
-        self.runTimestamp = runTimestamp
-        self.openOpr = 'Checking'
-        self.dOprStart = dict()
-
-        # Log to sys.stdout, and also to a temporary log file (unique folder).
-        self.runLogFileName = f'{self.DefLogNamePrefix}.{runTimestamp}.log'
-        self.runLogFileName = pl.Path(tempfile.mkdtemp(prefix='pyaudisam')) / self.runLogFileName
-        log.configure(handlers=[sys.stdout, self.runLogFileName], reset=True,
-                      loggers=[dict(name='matplotlib', level=log.WARNING),
-                               dict(name='ads', level=log.INFO2),
-                               dict(name='ads.eng', level=log.INFO),
-                               dict(name='ads.exr', level=log.INFO),
-                               # dict(name='ads.dat', level=log.DEBUG),
-                               # dict(name='ads.rep', level=log.DEBUG),
-                               dict(name='ads.anr', level=log.INFO1),
-                               dict(name='main', level=level)])
-
-        # Fallback final log file path-name as long as it is not specified : current folder, generic (timestamped) name.
-        self.finalLogFileName = pl.Path('.') / self.runLogFileName.name
-
-        # Set up an atexit handler to move and rename the session log file in a user-friendly place if possible.
-        atexit.register(self.giveBackLogFile)
-
-        # Add logging methods to this logger
-        self.logger = log.logger(name='main')
-        for meth in dir(self.logger):
-            if any(meth.startswith(prefix) for prefix in ['critical', 'error', 'warning', 'info', 'debug']):
-                setattr(self, meth, getattr(self.logger, meth))
+import pytest
 
-        # Done.
-        self.info1(f'Logging session to temporary ' + self.runLogFileName.as_posix())
-        self.info('Current folder: ' + pl.Path().absolute().as_posix())
-        self.info('Command line: {} {}'.format(pl.Path(sys.argv[0]).as_posix(), ' '.join(sys.argv[1:])))
+import pyaudisam as ads
 
-    def setFinalLogPrefix(self, prefix=None):
+import unintval_utils as uivu
 
-        self.finalLogFileName = None if prefix is None else pl.Path(prefix + f'.{self.runTimestamp}.log')
 
-    def giveBackLogFile(self):
+# Setup local logger.
+logger = uivu.setupLogger('val.pnr', level=ads.DEBUG)
+
+# Some constants
+RS = ads.MCDSPreAnalysisResultsSet
+KResLogCols = [
+    ('header (head)', 'NumEchant', 'Value'),
+    ('header (head)', 'NumAnlys', 'Value'),
+    ('header (tail)', 'AbrevAnlys', 'Value'),
+    RS.CLNTotObs,
+    RS.CLMinObsDist, RS.CLMaxObsDist,
+    RS.CLNObs,
+    RS.CLRunStatus,
+    RS.CLCmbQuaBal3,
+    RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+]
+
+
+@pytest.mark.valtests
+@pytest.mark.parametrize("sampleSpecMode", ['implicit', 'explicit'])
+class TestMcdsPreAnalyser:
+
+    # Set to False to skip final cleanup (useful for debugging)
+    KFinalCleanup = True
+
+    # Class and test function initializers / finalizers ###########################
+    @pytest.fixture(autouse=True, scope='class')
+    def _inifinalizeClass(self):
+
+        KWhat2Test = 'pre-analyser'
+
+        uivu.logBegin(what=KWhat2Test)
+
+        # Set up a clear ground before starting
+        uivu.setupWorkDir('val-panlr', cleanup=self.KFinalCleanup)
+
+        # The code before yield is run before the first test function in this class
+        yield
+        # The code after yield is run after the last test function in this class
+
+        # Let the ground clear after passing there
+        if self.KFinalCleanup:
+            uivu.cleanupWorkDir()
+
+        uivu.logEnd(what=KWhat2Test)
+
+    @pytest.fixture(autouse=True, scope='function')
+    def _inifinalizeFunction(self):
+
+        # The code before yield is run before every test function
+        yield
+        # The code after yield is run after every test function
+
+    # Test functions #############################################################
+
+    # II. Run and report pre-analyses
+    @pytest.fixture()
+    def inputDataSet_fxt(self):
+
+        logger.info(f'Preparing individual. sightings ...')
+
+        # ## 1. Individuals data set
+        dfObsIndiv = ads.DataSet(uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-ObsIndiv.ods',
+                                 sheet='DonnéesIndiv').dfData
+
+        logger.info(f'Invidual. sightings: n={len(dfObsIndiv)} =>\n'
+                    + dfObsIndiv.to_string(min_rows=30, max_rows=30))
+        indObsDesc = {col: dfObsIndiv[col].unique()
+                      for col in ['Observateur', 'Point', 'Passage', 'Adulte', 'Durée', 'Espèce']}
+        logger.info(f'... {indObsDesc}')
+
+        # ## 2. Actual transects
+        # (can't deduce them from data, some points are missing because of data selection)
+        dfTransects = ads.DataSet(uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-ObsIndiv.ods',
+                                  sheet='Inventaires').dfData
+
+        logger.info(f'Invidual. sightings: n={len(dfObsIndiv)} =>\n' + dfTransects.to_string(min_rows=30, max_rows=30))
+
+        logger.info(f'Done preparing individual. sightings.\n')
+
+        return dfObsIndiv, dfTransects
+
+    @staticmethod
+    def sampleSpecMode(implicit):
+        return 'im' if implicit else 'ex'
+
+    @pytest.fixture()
+    def preAnalyser_fxt(self, sampleSpecMode, inputDataSet_fxt):
+
+        logger.info(f'Preparing pre-analyser ...')
+
+        # ## 0. Data description
+        transectPlaceCols = ['Point']
+        passIdCol = 'Passage'
+        effortCol = 'Effort'
+
+        sampleDecCols = [effortCol, 'Distance']
+
+        sampleNumCol = 'NumEchant'
+        sampleSelCols = ['Espèce', passIdCol, 'Adulte', 'Durée']
+
+        sampleAbbrevCol = 'AbrevEchant'
+
+        speciesAbbrevCol = 'AbrevEsp'
+
+        dSurveyArea = dict(Zone='ACDC', Surface='2400')
+
+        # ## 1. Individuals data set
+        # ## 2. Actual transects
+        # See parameters
+
+        # ## 4A. Really run pre-analyses
+        # ### a. MCDSPreAnalyser object
+        areSpecsImplicit = sampleSpecMode == 'implicit'
+        dfObsIndiv, dfTransects = inputDataSet_fxt
+        preAnlysr = \
+            ads.MCDSPreAnalyser(dfObsIndiv, dfTransects=dfTransects, dSurveyArea=dSurveyArea,
+                                transectPlaceCols=transectPlaceCols, passIdCol=passIdCol, effortCol=effortCol,
+                                sampleSelCols=sampleSelCols, sampleDecCols=sampleDecCols,
+                                sampleSpecCustCols=[speciesAbbrevCol],
+                                abbrevCol=sampleAbbrevCol, abbrevBuilder=uivu.sampleAbbrev, sampleIndCol=sampleNumCol,
+                                distanceUnit='Meter', areaUnit='Hectare',
+                                surveyType='Point', distanceType='Radial', clustering=False,
+                                resultsHeadCols=dict(before=[sampleNumCol], sample=sampleSelCols,
+                                                     after=([] if areSpecsImplicit else [speciesAbbrevCol])
+                                                           + [sampleAbbrevCol]),
+                                workDir=uivu.pWorkDir, logProgressEvery=5)
+
+        assert preAnlysr.specs == dict(Zone='ACDC',
+                                       Surface='2400',
+                                       distanceUnit='Meter',
+                                       areaUnit='Hectare',
+                                       runMethod='subprocess.run',
+                                       runTimeOut=300,
+                                       surveyType='Point',
+                                       distanceType='Radial',
+                                       clustering=False,
+                                       defEstimKeyFn='UNIFORM',
+                                       defEstimAdjustFn='POLY',
+                                       defEstimCriterion='AIC',
+                                       defCVInterval=95,
+                                       defMinDist=None,
+                                       defMaxDist=None,
+                                       defFitDistCuts=None,
+                                       defDiscrDistCuts=None)
+
+        logger.info(f'Pre-analyser specs:\n{preAnlysr.specs}')
+
+        logger.info(f'Done preparing pre-analyser.\n')
+
+        logger.info(f'Preparing {sampleSpecMode} sample specs ...')
+
+        # a. Implicit variants
+        varEspeces = ['Sylvia atricapilla', 'Turdus merula', 'Luscinia megarhynchos']  # 1 species variant per species
+        varPassages = ['b', 'a+b']  # Pass b or a+b => 2 variants
+        varAdultes = ['m']  # Males only => 1 variant
+        varDurees = ['5mn', '10mn']  # first 5mn, and then all 10mn => 2 variants
+
+        dImplSampleSpecs = {'Espèce': varEspeces, 'Passage': varPassages, 'Adulte': varAdultes, 'Durée': varDurees}
+        implSampleSpecs = dict(_impl=dImplSampleSpecs)
+
+        logger.info(f'Implicit sample specs: {implSampleSpecs}')
+
+        # b. Explicit variants
+        dfExplSampleSpecs = None
+        if not areSpecsImplicit:
+            dfExplSampleSpecs = ads.Analyser.explicitVariantSpecs(implSampleSpecs)
+            # Just the same, but less generic.
+            # dfExplSampleSpecs = ads.Analyser.explicitPartialVariantSpecs(dImplSampleSpecs)
+
+            # Added neutral pass-through column (from sample specs to results)
+            speciesAbbrevCol = 'AbrevEsp'
+            dfExplSampleSpecs[speciesAbbrevCol] = \
+                dfExplSampleSpecs['Espèce'].apply(lambda s: ''.join(m[:4] for m in s.split()))
+
+            logger.info(f'Explicit sample specs:\n{dfExplSampleSpecs.to_string()}')
+
+        # c. Check pre-analyses specs
+        dfExplSampleSpecs, userParamSpecCols, intParamSpecCols, unmUserParamSpecCols, verdict, reasons = \
+            preAnlysr.explicitParamSpecs(dfExplParamSpecs=dfExplSampleSpecs if not areSpecsImplicit else None,
+                                         implParamSpecs=implSampleSpecs if areSpecsImplicit else None,
+                                         dropDupes=True, check=True)
+
+        logger.info('Sample spec. explicitations:')
+        logger.info(f'* verdict: {verdict}')
+        logger.info(f'* reasons: {reasons}')
+        logger.info(f'* userParamSpecCols: n={len(userParamSpecCols)} => {userParamSpecCols}')
+        logger.info(f'* intParamSpecCols: n={len(intParamSpecCols)} => {intParamSpecCols}')
+        logger.info(f'* unmUserParamSpecCols: n={len(unmUserParamSpecCols)} => {unmUserParamSpecCols}')
+
+        logger.info(f'Explicitated sample specs: n={len(dfExplSampleSpecs)} =>\n'
+                    + dfExplSampleSpecs.to_string(min_rows=30, max_rows=30))
+
+        assert len(dfExplSampleSpecs) == 12
+        assert userParamSpecCols == []  # No analysis params here (auto. generated by PreAnalyser)
+        assert intParamSpecCols == []  # Idem
+        assert unmUserParamSpecCols == []
+        assert verdict
+        assert not reasons
 
-        if any(arg in sys.argv for arg in ['-h', '--help']):
-            self.finalLogFileName = None  # No need for a log file here !
+        # Done.
+        logger.info(f'Done preparing {sampleSpecMode} sample specs.\n')
 
-        if self.finalLogFileName is not None:
-            self.info1(f'Giving back session log to {self.finalLogFileName}')
+        return (preAnlysr, implSampleSpecs) if areSpecsImplicit else (preAnlysr, dfExplSampleSpecs)
 
-        # Release the log file
-        log.configure(handlers=[sys.stdout], reset=True, loggers=[dict(name='main', level=log.INFO)])
+    @pytest.fixture()
+    def expectedSampleStats_fxt(self):
 
-        # Actually move and rename the log file if it is needed, or delete it if not.
-        if self.finalLogFileName is not None:
-            self.finalLogFileName.parent.mkdir(parents=True, exist_ok=True)
-            self.runLogFileName.rename(self.finalLogFileName)
+        return pd.DataFrame(columns=('NumEchant', 'Distance Min', 'Distance Max', 'NTot Obs'),
+                            data=[(0, 13.7, 488.2, 137),
+                                  (1, 8.4, 488.2, 207),
+                                  (2, 10.8, 488.2, 261),
+                                  (3, 1.2, 511.4, 388),
+                                  (4, 2.9, 714.1, 131),
+                                  (5, 2.9, 786.0, 220),
+                                  (6, 2.9, 714.1, 231),
+                                  (7, 2.9, 786.0, 400),
+                                  (8, 32.7, 1005.4, 57),
+                                  (9, 32.7, 1005.4, 84),
+                                  (10, 14.4, 1005.4, 107),
+                                  (11, 14.4, 1005.4, 156)]).set_index('NumEchant')
+
+    def testComputeSampleStats(self, sampleSpecMode, preAnalyser_fxt, expectedSampleStats_fxt):
+
+        if sampleSpecMode != 'implicit':
+            msg = 'testComputeSampleStats(explicit): skipped, as not relevant'
+            logger.info(msg)
+            pytest.skip(msg)  # Raises an exception => function execution stops here.
+
+        preAnlysr, sampleSpecs = preAnalyser_fxt
+        dfSampleStats = preAnlysr.computeSampleStats(implSampleSpecs=sampleSpecs, sampleDistCol='Distance')
+        logger.info(f'Sample stats: n={len(dfSampleStats)} =>\n{dfSampleStats.to_string(min_rows=30, max_rows=30)}')
+
+        dfSampleStats['Distance Min'] = dfSampleStats['Distance Min'].round(1)
+        dfSampleStats['Distance Max'] = dfSampleStats['Distance Max'].round(1)
+        dfSampleStats.set_index('NumEchant', inplace=True)
+        dfSampleStats = dfSampleStats[['Distance Min', 'Distance Max', 'NTot Obs']]
+
+        dfExptdStats = expectedSampleStats_fxt
+        assert dfSampleStats.compare(dfExptdStats).empty
+
+        logger.info(f'PASS testComputeSampleStats: computeSampleStats')
+
+    # Only minimalistic checks done here, as already more deeply tested in test_unint_engine.py
+    @staticmethod
+    def checkExportedDsInputData(exportDir, sampleSpecs, sampleSpecMode):
+
+        areSpecsImplicit = sampleSpecMode == 'implicit'
+
+        # ii. Check list of generated files
+        expdGenFileNames = []
+        if areSpecsImplicit:
+            for esp in sampleSpecs['_impl']['Espèce']:
+                for pas in sampleSpecs['_impl']['Passage']:
+                    for ad in sampleSpecs['_impl']['Adulte']:
+                        for dur in sampleSpecs['_impl']['Durée']:
+                            sampAbbrv = uivu.sampleAbbrev(pd.Series({'Espèce': esp, 'Passage': pas,
+                                                                     'Adulte': ad, 'Durée': dur}))
+                            expdGenFileNames.append(f'{sampAbbrv}-dist.txt')
         else:
-            self.runLogFileName.unlink()
+            for _, sSampSpec in sampleSpecs.iterrows():
+                sampAbbrv = uivu.sampleAbbrev(sSampSpec[['Espèce', 'Passage', 'Adulte', 'Durée']])
+                expdGenFileNames.append(f'{sampAbbrv}-dist.txt')
+        assert all(fpn.name in expdGenFileNames for fpn in exportDir.glob('*-dist.txt'))
+
+        # iii. Check first generated file
+        sampAbbrv = uivu.sampleAbbrev(pd.Series({'Espèce': 'Luscinia megarynchos', 'Passage': 'a+b',
+                                                 'Adulte': 'm', 'Durée': '10mn'}))
+        fpnSamp = exportDir / f'{sampAbbrv}-dist.txt'
+        dfSampDist = pd.read_csv(fpnSamp, sep='\t', decimal=',')
+        logger.info(f'{fpnSamp.as_posix()}:\n{dfSampDist.to_string(min_rows=30, max_rows=30)}')
+
+        assert len(dfSampDist) == 182
+        assert dfSampDist.columns.tolist() == ['Region*Label', 'Region*Area', 'Point transect*Label',
+                                               'Point transect*Survey effort', 'Observation*Radial distance']
+        assert dfSampDist['Point transect*Label'].nunique() == 96
+        assert all(dfSampDist['Region*Label'].unique() == ['ACDC'])
+        assert all(dfSampDist['Region*Area'].unique() == [2400])
+        assert dfSampDist['Point transect*Survey effort'].sum() == 362
+        assert dfSampDist['Observation*Radial distance'].isnull().sum() == 26
+
+        # iv. Cleanup all generated files
+        for fpnSamp in exportDir.glob('*-dist.txt'):
+            fpnSamp.unlink()
+
+    # ### c. Generate input files for manual analyses with Distance GUI (not needed for pre-analyses)
+    #        through pyaudisam API
+    def testExportDsInputData(self, sampleSpecMode, preAnalyser_fxt):
+
+        # i. Export distance files
+        logger.info(f'Exporting Distance files ({sampleSpecMode} sample specs) ...')
+
+        areSpecsImplicit = sampleSpecMode == 'implicit'
+        preAnlysr, sampleSpecs = preAnalyser_fxt
+        preAnlysr.exportDSInputData(implSampleSpecs=sampleSpecs if areSpecsImplicit else None,
+                                    dfExplSampleSpecs=sampleSpecs if not areSpecsImplicit else None,
+                                    format='Distance')
+
+        # ii. Check exported files
+        self.checkExportedDsInputData(preAnlysr.workDir, sampleSpecs, sampleSpecMode)
+
+        logger.info(f'PASS testExportDsInputData: exportDsInputData({sampleSpecMode} sample specs)')
+
+    # ### c. Generate input files for manual analyses with Distance GUI (not needed for pre-analyses),
+    #        through pyaudisam command line interface (implicit mode only, see valtests-ds-params.py)
+    def testExportDsInputDataCli(self, sampleSpecMode, preAnalyser_fxt):
+
+        if sampleSpecMode != 'implicit':
+            msg = 'testExportDsInputDataCli(explicit): skipped, as not relevant'
+            logger.info(msg)
+            pytest.skip(msg)  # Raises an exception => function execution stops here.
+
+        # i. Export distance files
+        logger.info(f'Exporting Distance files (command line mode) ...')
+
+        testPath = pl.Path(__file__).parent
+        preAnlysr, sampleSpecs = preAnalyser_fxt
+        workPath = preAnlysr.workDir
+
+        # a. Export files "through the commande line"
+        argv = f'-p {testPath.as_posix()}/valtests-ds-params.py -w {workPath.as_posix()} -n --distexport -u'.split()
+        rc = ads.main(argv, standaloneLogConfig=False)
+        logger.info(f'CLI run: rc={rc}')
+
+        # ii. Check exported files
+        self.checkExportedDsInputData(workPath, sampleSpecs, sampleSpecMode)
+
+        logger.info(f'PASS testExportDsInputDataCli: exportDsInputData(command line mode)')
+
+    @staticmethod
+    def loadResults(preAnlysr, filePath, postComputed=False):
+
+        logger.info(f'Loading pre-results from {filePath.as_posix()} ...')
+
+        rsRes = preAnlysr.setupResults()
+        rsRes.fromFile(filePath, postComputed=postComputed)
+
+        assert isinstance(rsRes, ads.MCDSPreAnalysisResultsSet)
+
+        return rsRes
+
+    @pytest.fixture()
+    def refResults_fxt(self, sampleSpecMode, preAnalyser_fxt):
+
+        logger.info(f'Preparing reference pre-results ({sampleSpecMode} mode) ...')
+
+        # Prevent re-postComputation as this ref. file is old, with now missing computed cols
+        preAnlysr, _ = preAnalyser_fxt
+        rsRef = self.loadResults(preAnlysr, uivu.pRefOutDir / 'ACDC2019-Naturalist-extrait-PreResultats.ods',
+                                 postComputed=True)
+
+        logger.info(f'Reference results: n={len(rsRef)} =>\n'
+                    + rsRef.dfTransData(columns=KResLogCols, lang='en').to_string(min_rows=99, max_rows=99))
+
+        return rsRef
+
+    @staticmethod
+    def compareResults(rsRef, rsAct):
+        """Prerequisite: Reference results generated with either MCDS 7.4 or 6.2"""
+
+        logger.info('Comparing reference to actual pre-results ...')
+
+        # 1. Actual pre-analysis results: "all-results" sheet
+        # 1a. Comparison index = analysis "Id": sample Id columns and analysis indexes.
+        indexPreCols = [col for col in rsAct.miCustomCols.to_list() if '(sample)' in col[0]] \
+                       + [('parameters', 'estimator key function', 'Value'),
+                          ('parameters', 'estimator adjustment series', 'Value')]
+
+        # 1b. Comparison columns: ignore ...
+        #   - sample Id columns and analysis indexes (used as comparison index = analysis "Id")
+        #   - 'run output' chapter results (start time, elapsed time, run folder ... always different)
+        #   - text columns (not supported by ResultsSet.compare).
+        subsetPreCols = [col for col in rsAct.dfData.columns.to_list()
+                         if col in rsRef.columns
+                         and col not in indexPreCols + [col for col in rsAct.miCustomCols.to_list()
+                                                        if '(sample)' not in col[0]]
+                         + [('parameters', 'estimator selection criterion', 'Value'),
+                            ('parameters', 'CV interval', 'Value'),
+                            ('run output', 'start time', 'Value'),
+                            ('run output', 'elapsed time', 'Value'),
+                            ('run output', 'run folder', 'Value'),
+                            ('detection probability', 'key function type', 'Value'),
+                            ('detection probability', 'adjustment series type', 'Value'),
+                            ('detection probability', 'Delta AIC', 'Value'),
+                            ('density/abundance', 'density of animals', 'Delta Cv')]]
+
+        # 1c. Compare
+        dfDiff = rsRef.compare(rsAct, indexCols=indexPreCols, subsetCols=subsetPreCols,
+                               noneIsNan=True, dropCloser=13, dropNans=True)
+
+        logger.info(f'Diff. to reference (relative): n={len(dfDiff)} =>\n'
+                    + dfDiff.to_string(min_rows=30, max_rows=30))
+        if not dfDiff.empty:
+            dfDiff.to_excel(uivu.pWorkDir / 'res-comp-13.xlsx')
+
+        assert dfDiff.empty, 'Oh oh ... some unexpected differences !'
+
+        # 1d. To be perfectly honest ... there may be some 10**-14/-16 glitches (due to worksheet I/O ?) ... or not.
+        dfComp = rsRef.compare(rsAct, indexCols=indexPreCols, subsetCols=subsetPreCols,
+                               noneIsNan=True, dropNans=True)
+        dfComp = dfComp[(dfComp != np.inf).all(axis='columns')]
+
+        logger.info(f'Diff. to reference (absolute): n={len(dfComp)} =>\n'
+                    + dfComp.to_string(min_rows=30, max_rows=30))
+
+        # 2. Specs: Samples
+        dfRefSampSpecs = rsRef.specs['samples']
+        logger.info(f'Ref sample specs: n={len(dfRefSampSpecs)} =>\n'
+                    + dfRefSampSpecs.to_string(min_rows=30, max_rows=30))
+        # Remove neutral pass-through column (from sample specs to results)
+        # from actual sample specs if there (not present in ref.)
+        dfActSampSpecs = rsAct.specs['samples'].drop(columns=['AbrevEsp'], errors='ignore')
+        logger.info(f'Actual sample specs: n={len(dfActSampSpecs)} =>\n'
+                    + dfActSampSpecs.to_string(min_rows=30, max_rows=30))
+        assert dfRefSampSpecs.compare(dfActSampSpecs).empty
+
+        # 3. Specs: Models
+        dfRefModSpecs = rsRef.specs['models']
+        logger.info(f'Ref. model specs: n={len(dfRefModSpecs)} =>\n'
+                    + dfRefModSpecs.to_string(min_rows=30, max_rows=30))
+        dfActModSpecs = rsAct.specs['models']
+        logger.info(f'Actual model specs: n={len(dfActModSpecs)} =>\n'
+                    + dfActModSpecs.to_string(min_rows=30, max_rows=30))
+        assert dfRefModSpecs.compare(dfActModSpecs).empty
+
+        # 4. Specs: Analyser
+        dfRefAnrSpecs = rsRef.specs['analyser']
+        logger.info(f'Ref. analyser specs: n={len(dfRefAnrSpecs)} =>\n'
+                    + dfRefAnrSpecs.to_string(min_rows=30, max_rows=30))
+        dfActAnrSpecs = rsAct.specs['analyser']
+        logger.info(f'Actual analyser specs: n={len(dfActAnrSpecs)} =>\n'
+                    + dfActAnrSpecs.to_string(min_rows=30, max_rows=30))
+        assert dfRefAnrSpecs.compare(dfActAnrSpecs).empty
+
+        # 5. Specs: Run-time : whatever ref, expect a specific up-to-date list of item names, but nothing more
+        sRefRunSpecs = rsRef.specs['runtime']
+        logger.info(f'Ref. runtime specs: n={len(sRefRunSpecs)} =>\n' + sRefRunSpecs.to_string())
+        sActRunSpecs = rsAct.specs['runtime']
+        logger.info(f'Actual runtime specs: n={len(sActRunSpecs)} =>\n' + sActRunSpecs.to_string())
+        assert set(sActRunSpecs.index) \
+               == {'os', 'processor', 'python', 'numpy', 'pandas', 'zoopt', 'matplotlib',
+                   'jinja2', 'pyaudisam', 'MCDS engine', 'MCDS engine version'}
+
+        logger.info('Done comparing reference to actual pre-results.')
+
+    # ### d. Run pre-analyses through pyaudisam API
+    # Performance figures:
+    # Ruindows 10 laptop with PCI-e SSD, "optimal performances" power scheme, Python 3.8 :
+    # * 4-HT-core i5-8350U:
+    #   * 2021 (precise date ?): 50s to ~1mn10s elapsed for 12 samples, 6-12 threads (N=?)
+    # * 6-core i7-10750H (HT off):
+    #   * 2022-01-17, 2023-11-02: 39-40s elapsed for 12 samples, 6-12 threads (N=5)
+    # Ruindows 11 laptop with PCI-e SSD, "high performances" power scheme, Python 3.8 :
+    # * 6-HT-core i7-10850H (HT on):
+    #   * 2024-03-02: 40s elapsed for 12 samples, 6 threads (N=1)
+    #   * 2024-03-02: 39s elapsed for 12 samples, 12 threads (N=1)
+    def testRun(self, sampleSpecMode, preAnalyser_fxt, refResults_fxt):
+
+        postCleanup = True  # Debug only: Set to False to prevent cleaning at the end
+
+        # i. Cleanup test folder (Note: avoid any Ruindows shell or explorer inside this folder !)
+        preAnlysr, sampleSpecs = preAnalyser_fxt
+        if preAnlysr.workDir.exists():
+            shutil.rmtree(preAnlysr.workDir)
+
+        # ii. Run and measure performance
+        threads = 6
+        logger.info(f'Running pre-analyses: {sampleSpecMode} sample specs, {threads} parallel threads ...')
+
+        # Model fall-down strategy
+        # Note: For real bird study analyses, you'll probably avoid NEXPON key function
+        #       (a model with no shoulder: g'(0) << 1).
+        #       And also HERMITE adjustment series (overkill fitting).
+        modelStrategy = [dict(keyFn=kf, adjSr=js, estCrit='AIC', cvInt=95)
+                         for js in ['COSINE', 'POLY', 'HERMITE']
+                         for kf in ['HNORMAL', 'HAZARD', 'UNIFORM', 'NEXPON']]
+
+        # BE CAREFUL: time.process_time() uses relative time for comparison only of codes among the same environment
+        # NOT A REAL TIME reference
+        areSpecsImplicit = sampleSpecMode == 'implicit'
+
+        start = time.perf_counter()
+        preAnlysr, sampleSpecs = preAnalyser_fxt
+        rsAct = preAnlysr.run(implSampleSpecs=sampleSpecs if areSpecsImplicit else None,
+                              dfExplSampleSpecs=sampleSpecs if not areSpecsImplicit else None,
+                              dModelStrategy=modelStrategy, threads=threads)
+        end = time.perf_counter()
+
+        logger.info(f'Elapsed time={end - start:.2f}s')
+        logger.info(f'Actual results: n={len(rsAct)} =>\n'
+                    + rsAct.dfTransData(columns=KResLogCols, lang='en').to_string(min_rows=99, max_rows=99))
+
+        # Export results
+        rsAct.toOpenDoc(preAnlysr.workDir / f'valtests-preanalyses-results-{sampleSpecMode}api.ods')
+        # rsAct.toExcel(preAnlysr.workDir / f'valtests-preanalyses-results-{sampleSpecMode}api-fr.xlsx', lang='fr')
+
+        # ### e. Check results: Compare to reference
+        # i. Check presence of neutral and pass-through column in explicit spec. mode
+        #    (it should have effectively passed through :-)
+        speciesAbbrevCol = 'AbrevEsp'
+        logger.debug('dfTransData(en).columns: ' + str(rsAct.dfTransData('en').columns))
+        assert areSpecsImplicit or speciesAbbrevCol in rsAct.dfTransData('en').columns
+
+        # ii. Compare to reference results
+        rsRef = refResults_fxt
+        self.compareResults(rsRef, rsAct)
+
+        # f. Minimal check of pre-analysis folders
+        logger.info('Checking pre-analysis folders (minimal) ...')
+        uivu.checkAnalysisFolders(rsAct.dfTransData('en').RunFolder, expectedCount=12, anlysKind='pre-analysis')
+
+        # g. Cleanup analyser (analysis folders, not workbook results files)
+        if postCleanup:
+            preAnlysr.cleanup()
+        else:
+            logger.warning('NOT cleaning up the pre-analyser: this is not the normal testing scheme !')
 
-        # Remove initial parent folder, now empty (was specially created for).
-        self.runLogFileName.parent.rmdir()
+        # h. Done.
+        logger.info(f'PASS testRun: run({sampleSpecMode} sample specs), cleanup')
 
-    def setRealRun(self, realRun=True):
+    # Run pre-analyses through pyaudisam command line interface
+    # (implicit mode only, see valtests-ds-params.py)
+    def testRunCli(self, sampleSpecMode, preAnalyser_fxt, refResults_fxt):
+
+        if sampleSpecMode != 'implicit':
+            msg = 'testRunCli(explicit): skipped, as not relevant'
+            logger.info(msg)
+            pytest.skip(msg)  # Raises an exception => function execution stops here.
+
+        # a. Cleanup test folder (Note: avoid any Ruindows shell or explorer inside this folder !)
+        preAnlysr, _ = preAnalyser_fxt
+        shutil.rmtree(preAnlysr.workDir)
+
+        # b. Run "through the commande line"
+        argv = f'-p {uivu.pTestDir.as_posix()}/valtests-ds-params.py -w {preAnlysr.workDir.as_posix()}' \
+               ' -n --preanalyses -u'.split()
+        rc = ads.main(argv, standaloneLogConfig=False)
+        logger.info(f'CLI run: rc={rc}')
+
+        # c. Load pre-results
+        rsAct = self.loadResults(preAnlysr, preAnlysr.workDir / 'valtests-preanalyses-results.xlsx')
+        logger.info(f'Actual results: n={len(rsAct)} =>\n'
+                    + rsAct.dfTransData(columns=KResLogCols, lang='en').to_string(min_rows=99, max_rows=99))
+
+        # d. Compare to reference.
+        rsRef = refResults_fxt
+        self.compareResults(rsRef, rsAct)
+
+        # e. Minimal check of pre-analysis folders
+        uivu.checkAnalysisFolders(rsAct.dfTransData('en').RunFolder, expectedCount=12, anlysKind='pre-analysis')
+
+        # f. Don't clean up work folder / analysis folders : needed for report generations below
+
+        # g. Done.
+        logger.info(f'PASS testRunCli: main, run (command line mode)')
+
+    @pytest.fixture()
+    def excelRefReport_fxt(self):
+
+        return pd.read_excel(uivu.pRefOutDir / 'ACDC2019-Naturalist-extrait-PreRapport.ods',
+                             sheet_name=None, index_col=0)
+
+    @staticmethod
+    def compareExcelReports(ddfRefReport, ddfActReport):
+        """Prerequisite: Reference report generated with either MCDS 7.4 or 6.2"""
+
+        logger.info('Comparing reference to actual workbook reports ...')
+
+        # Compare "Synthesis" sheet
+        dfRef = ddfRefReport['Synthesis'].drop(columns=['RunFolder']).set_index('NumEchant')
+        dfAct = ddfActReport['Synthesis'].drop(columns=['RunFolder']).set_index('NumEchant')
+        assert dfRef.compare(dfAct).empty
+
+        # Compare "Details" sheet : not that simple ...
+        # * 11 more "No Doc" columns with MCDS 7.4 (the ref) compared to MCDS 6.2,
+        # * very small differences in "Qua" indicators between MCDS 7.4 compared to MCDS 6.2
+        dfRef = ddfRefReport['Details'].drop(columns=['StartTime', 'ElapsedTime', 'RunFolder'])
+        dfAct = ddfActReport['Details'].drop(columns=['StartTime', 'ElapsedTime', 'RunFolder'])
+        # a. Compare all the string columns and a few "no precision issue" more.
+        idCols = ['NumEchant', 'Espèce', 'Passage', 'Adulte', 'Durée', 'AbrevEchant']
+        simpleCompCols = idCols
+        simpleCompCols += ['NTot Obs', 'Mod Key Fn', 'Mod Adj Ser', 'Mod Chc Crit', 'Conf Interv', 'Key Fn', 'Adj Ser']
+        assert dfRef[simpleCompCols].set_index('NumEchant').compare(dfAct[simpleCompCols].set_index('NumEchant')).empty
+
+        # b. Compare other (all numerical) columns with a small margin (1e-14 relative diff)
+        otherCompCols = [col for col in dfRef if col not in simpleCompCols]
+        if len(dfAct.columns) != len(dfRef.columns):  # Not the same version of MCDS as for the ref. report
+            spe74CompCols = [col for col in otherCompCols if col.startswith('SansDoc #')]  # 7.4-specifics
+            assert len(spe74CompCols) == 11
+            otherCompCols = [col for col in otherCompCols if col not in spe74CompCols]  # Remove 7.4-specifics
+
+        logger.info(f'* {otherCompCols=}')
+        dfDiff = ads.DataSet.compareDataFrames(dfLeft=dfRef, dfRight=dfAct,
+                                               subsetCols=otherCompCols, indexCols=idCols,
+                                               noneIsNan=True, dropCloserCols=True,
+                                               dropCloser=14, dropNans=True)
+        logger.info(f'* diff. to reference (relative): n={len(dfDiff)} =>\n'
+                    + dfDiff.to_string(min_rows=30, max_rows=30))
+        if not dfDiff.empty:
+            dfDiff.reset_index().to_excel(uivu.pWorkDir / 'rep-comp-14.xlsx')
+
+        # Compare "Samples" sheet
+        dfRef = ddfRefReport['Samples'].set_index('NumEchant', drop=True)
+        dfAct = ddfActReport['Samples'].set_index('NumEchant', drop=True)
+        assert dfRef.compare(dfAct).empty
+
+        # Compare "Models" sheet
+        dfRef = ddfRefReport['Models']
+        dfAct = ddfActReport['Models']
+        assert dfRef.compare(dfAct).empty
+
+        # Compare "Analyser" sheet
+        dfRef = ddfRefReport['Analyser']
+        dfAct = ddfActReport['Analyser']
+        assert dfRef.compare(dfAct).empty
+
+        # Compare "Computing platform" sheet
+        # (whatever ref, expect a specific up-to-date list of item names, but nothing more ;
+        #  values may vary, 'cause they are mostly software versions: it's OK)
+        dfAct = ddfActReport['Computing platform']
+        assert set(dfAct.index) \
+               == {'os', 'processor', 'python', 'numpy', 'pandas', 'zoopt', 'matplotlib',
+                   'jinja2', 'pyaudisam', 'MCDS engine', 'MCDS engine version'}
+
+        logger.info('Done comparing reference to actual workbook reports.')
+
+    @pytest.fixture()
+    def htmlRefReportLines_fxt(self):
+
+        with open(uivu.pRefOutDir / 'ACDC2019-Naturalist-extrait-PreRapport.html') as file:
+            repLines = file.readlines()
+
+        return repLines
+
+    @staticmethod
+    def compareHtmlReports(refReportLines, actReportLines):
+        """Prerequisite: Reference report generated with either MCDS 7.4 or 6.2"""
+
+        logger.info('Preprocessing HTML pre-reports for comparison ...')
+
+        # Pre-process actual report lines
+        remRefLines = remActLines = 0
+
+        # * list unique analysis folders (keeping the original order) in both reports
+        KREAnlysDir = r'="./([a-zA-Z0-9-_]+)/'
+        refAnlysDirs = uivu.listUniqueStrings(KREAnlysDir, refReportLines)
+        actAnlysDirs = uivu.listUniqueStrings(KREAnlysDir, actReportLines)
+        logger.info(f'* found {len(refAnlysDirs)}/{len(actAnlysDirs)} ref./act. pre-analysis folder')
+        assert len(refAnlysDirs) == len(actAnlysDirs)
+
+        # * replace each analysis folder in the actual report by the corresponding ref. report one
+        repAnlysDirLines = uivu.replaceStrings(froms=actAnlysDirs, tos=refAnlysDirs, lines=actReportLines)
+        logger.info(f'* replaced analysis folder by ref. one in {repAnlysDirLines} act. lines')
+
+        # * remove specific lines in both reports:
+        #   - header meta "DateTime"
+        KREDateTime = r'[0-9]{2}/[0-9]{2}/[0-9]{4} [0-9]{2}:[0-9]{2}:[0-9]{2}'
+        KREMetaDateTime = rf'<meta name="datetime" content="{KREDateTime}"/>'
+        remRefLines += uivu.removeLines(KREMetaDateTime, refReportLines)
+        remActLines += uivu.removeLines(KREMetaDateTime, actReportLines)
+
+        #   - footer "Generated on <date+time>"  => not needed, 'cause in final ignored blocks (see below)
+        # KREGenDateTime = rf'Generated on {KREDateTime}'
+        # remRefLines += uivu.removeLines(KREGenDateTime, refReportLines)
+        # remActLines += uivu.removeLines(KREGenDateTime, actReportLines)
+
+        logger.info(f'* removed {remRefLines} ref. and {remActLines} act. lines')
+
+        # Build the list of unified diff blocks
+        blocks = uivu.unifiedDiff(refReportLines, actReportLines, logger=logger, subject='HTML pre-reports')
+
+        # Filter diff blocks to check (ignore some that are expected to change without any issue:
+        # * header meta "datetime" generation date,
+        # * computation platform table, with component versions,
+        # * generation date, credits to components with versions, sources)
+        blocks_to_check = []
+        for block in blocks:
+            if block.startLines.expected >= 552 - remRefLines:  # <h3>Computing platform</h3><table ...<tbody>
+                logger.info(f'Ignoring block @ -{block.startLines.expected} +{block.startLines.real} @')
+                continue
+            blocks_to_check.append(block)
+
+        # Check filtered blocks : should not be any left !
+        assert len(blocks_to_check) == 0
+
+        logger.info('HTML pre-reports comparison: success !')
+
+    # ## 7. Generate HTML and Excel pre-analyses reports through pyaudisam API
+    def testReports(self, sampleSpecMode, preAnalyser_fxt, excelRefReport_fxt, htmlRefReportLines_fxt):
+
+        if sampleSpecMode != 'implicit':
+            msg = 'testReports(explicit): skipped, as not relevant'
+            logger.info(msg)
+            pytest.skip(msg)  # Raises an exception => function execution stops here.
+
+        build = True  # Debug only: Set to False to avoid rebuilding the reports, and only check them
+        postCleanup = True  # Debug only: Set to False to prevent cleaning at the end
+
+        # Pre-requisites : uncleaned pre-analyser work dir (we need the results file and analysis folders).
+        preAnlysr, _ = preAnalyser_fxt
+        if build:
+            logger.info('Checking analyser results presence ...')
+            preAnlysrResFilePath = preAnlysr.workDir / 'valtests-preanalyses-results.xlsx'
+            assert preAnlysr.workDir.exists() and preAnlysrResFilePath.is_file()
+            anlysFolders = [path for path in preAnlysr.workDir.iterdir() if path.is_dir()]
+            assert len(anlysFolders) == 12
+            logger.info('Done checking analyser results presence: OK.')
+
+            # a. Load pre-results
+            # (the last generated one, through implicit or explicit sample specs:
+            #  never mind, they are the same as checked above)
+            rsAct = self.loadResults(preAnlysr, preAnlysrResFilePath)
+            logger.info(f'Actual results: n={len(rsAct)} =>\n' + rsAct.dfData.to_string(min_rows=30, max_rows=30))
+
+            # # b. Generate Excel and HTML reports
+            # b.i. Super-synthesis sub-report : Selected analysis results columns for the 3 textual columns of the table
+            sampleRepCols = [
+                ('header (head)', 'NumEchant', 'Value'),
+                ('header (sample)', 'Espèce', 'Value'),
+                ('header (sample)', 'Passage', 'Value'),
+                ('header (sample)', 'Adulte', 'Value'),
+                ('header (sample)', 'Durée', 'Value'),
+                RS.CLNTotObs, RS.CLMinObsDist, RS.CLMaxObsDist,
+            ]
+
+            paramRepCols = [
+                RS.CLParEstKeyFn, RS.CLParEstAdjSer,
+                # RS.CLParEstSelCrit, RS.CLParEstCVInt
+            ]
+
+            resultRepCols = [
+                RS.CLRunStatus,
+                RS.CLNObs, RS.CLEffort,
+                RS.CLAic, RS.CLChi2, RS.CLKS, RS.CLDCv,
+
+                RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3,
+
+                RS.CLPDetec,
+                RS.CLEswEdr,
+                RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+                RS.CLNumber, RS.CLNumberMin, RS.CLNumberMax,
+            ]
+
+            # b.ii. Synthesis sub-report : Selected analysis results columns for the
+            synthRepCols = [
+                ('header (head)', 'NumEchant', 'Value'),
+                ('header (sample)', 'Espèce', 'Value'),
+                ('header (sample)', 'Passage', 'Value'),
+                ('header (sample)', 'Adulte', 'Value'),
+                ('header (sample)', 'Durée', 'Value'),
+                RS.CLParEstKeyFn,
+                RS.CLParEstAdjSer,
+
+                RS.CLNTotObs, RS.CLNObs, RS.CLNTotPars, RS.CLEffort, RS.CLDeltaAic,
+                RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw, RS.CLDCv,
+
+                RS.CLSightRate,
+                RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3,
+                RS.CLCmbQuaChi2, RS.CLCmbQuaKS, RS.CLCmbQuaDCv,
+
+                RS.CLPDetec, RS.CLPDetecMin, RS.CLPDetecMax,
+                RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+                RS.CLNumber, RS.CLNumberMin, RS.CLNumberMax,
+            ]
+
+            # b.iii. Sorting columns for all the sub-reports
+            sortRepCols = [('header (head)', 'NumEchant', 'Value')]
+            sortRepAscend = True
+
+            # b.iv. Report object
+            report = ads.MCDSResultsPreReport(resultsSet=rsAct,
+                                              title='PyAuDiSam Validation: Pre-analyses',
+                                              subTitle='Pre-analysis results report',
+                                              anlysSubTitle='Pre-analysis results details',
+                                              description='Easy and parallel run through MCDSPreAnalyser',
+                                              keywords='pyaudisam, validation, pre-analysis',
+                                              lang='en', superSynthPlotsHeight=288,
+                                              # plotImgSize=(640, 400), plotLineWidth=1, plotDotWidth=4,
+                                              # plotFontSizes=dict(title=11, axes=10, ticks=9, legend=10),
+                                              sampleCols=sampleRepCols, paramCols=paramRepCols,
+                                              resultCols=resultRepCols, synthCols=synthRepCols,
+                                              sortCols=sortRepCols, sortAscend=sortRepAscend,
+                                              tgtFolder=preAnlysr.workDir,
+                                              tgtPrefix='valtests-preanalyses-report-api')
+
+            # b.iv. Excel report
+            xlsxRep = report.toExcel()
+            logger.info('Excel pre-report: ' + pl.Path(xlsxRep).resolve().as_posix())
+
+            # b.v. HTML report
+            htmlRep = report.toHtml()
+            logger.info('HTML pre-report: ' + pl.Path(htmlRep).resolve().as_posix())
 
-        if realRun:
-            self.openOpr = 'Running'
-            self.info('This is a real run: requested operation will be actually run !')
         else:
-            self.openOpr = 'Checking'
-            self.warning('Not a real run, only checking requested operations ...')
+            logger.warning('NOT building the reports: this is not the normal testing scheme !')
+            xlsxRep = preAnlysr.workDir / 'valtests-preanalyses-report.xlsx'
+            htmlRep = preAnlysr.workDir / 'valtests-preanalyses-report.html'
+
+        # c. Load generated Excel report and compare it to reference one
+        ddfRefRep = excelRefReport_fxt
 
-    def openOperation(self, oprText):
+        ddfActRep = pd.read_excel(xlsxRep, sheet_name=None, index_col=0)
 
-        self.info(f'{self.openOpr} {oprText} ...')
-        self.dOprStart[oprText] = pd.Timestamp.now()
+        self.compareExcelReports(ddfRefRep, ddfActRep)
 
-    def closeOperation(self, oprText):
-
-        elapsed = str(pd.Timestamp.now() - self.dOprStart[oprText]).replace('0 days ', '')
-        self.info(f'Done {self.openOpr.lower()} {oprText} ({elapsed}).')
-        del self.dOprStart[oprText]
-
-
-def decodeReportArg(repArg, repName='report'):
-
-    """Decode report argument value
-
-    Mini-language examples: none ; excel ; excel,html ; html:full ; excel,html:mqua-r925,html:mqua-r950
-
-    :returns: dict(format: list(type)) with format in {'none', 'excel', 'html'}, 'none' excluding any other,
-              and list(type) empty for 'none', empty or ['full'] for 'excel' format,
-              and containing at least 1 of {full, <filter-sort method regex search string>*} for 'html' format.
-    """
-
-    # Separate format[:type] items
-    repItems = [item.lower() for item in repArg.split(',')]
-
-    # List types for each format
-    repSpecs = dict()
-    for repItem in repItems:
-        fmt, typ = repItem.split(':') + ([None] if ':' not in repItem else [])
-        if fmt not in repSpecs:
-            repSpecs[fmt] = list()
-        if typ not in repSpecs[fmt] and typ is not None:
-            repSpecs[fmt].append(typ)
-
-    # 'none' format kept iff alone
-    repSpecs = {fmt: typs for fmt, typs in repSpecs.items() if fmt != 'none' or len(repSpecs) == 1}
-    if 'none' in repSpecs:
-        repSpecs.clear()
-
-    # Check formats
-    unsupRepFmts = [fmt for fmt in repSpecs if fmt not in ['none', 'html', 'excel']]
-    if unsupRepFmts:
-        logger.error('Unsupported {} format(s) {}'.format(repName, ', '.join(unsupRepFmts)))
-        sys.exit(2)
-
-    logger.debug1(f'{repName}: {repSpecs}')
-
-    return repSpecs
-
-
-# 0. Configure logging.
-runTimestamp = pd.Timestamp.now().strftime('%y%m%d-%H%M%S')  # Date+time of the run (for log file, ... etc).
-
-logger = Logger(runTimestamp, level=log.DEBUG2 if '-v' in sys.argv or '--verbose' in sys.argv else log.INFO1)
-
-logger.info('Computation platform:')
-for k, v in runtime.items():
-    logger.info(f'* {k}: {v}')
-
-# 1. Parse, check and post-process command line args.
-argser = argparse.ArgumentParser(prog='pyaudisam',  # usage='python -m pyaudisam',
-                                 description='Prepare or run (and / or generate reports for) many distance'
-                                             ' sampling (pre-)analyses using a DS engine from Distance software',
-                                 epilog='Exit codes:'
-                                        ' 0 if OK,'
-                                        ' 2 if any command line argument issue,'
-                                        ' 1 if any other (unexpected) issue.')
-
-argser.add_argument('-u', '--run', dest='realRun', action='store_true', default=False,
-                    help='Actually run specified operation (not only run diagnosis of)'
-                         ' => as long as -u/--run is not there, you can try any option,'
-                         ' it wont start or write anything (or maybe slightly when -v, but anyway)'
-                         ' ... feel free, you are safe :-)')
-argser.add_argument('-v', '--verbose', dest='verbose', action='store_true', default=False,
-                    help='Display more infos about the work to be done and export sample / (opt-)analysis'
-                         ' spec. files when relevant in the current directory ;')
-argser.add_argument('-p', '--params', dest='paramFile', type=str, required=True,
-                    help='Path-name of python file (.py assumed if no extension / suffix given) specifying'
-                         ' export / (opt)analysis / report parameters')
-argser.add_argument('-s', '--speparams', dest='speParams', type=str, default='',
-                    help='Comma-separated key=value items specifying "special" parameters'
-                         'defined before the parameter file is loaded, just as overridable built-in variables'
-                         r' (syntax and limitations: string-only values, with no space or ,;\'"$&! inside'
-                         ' => use it only for few and simple args like switches and simple names')
-argser.add_argument('-w', '--workdir', dest='workDir', type=str, default='.',
-                    help='Work folder = where to store DS analyses sub-folders and output files'
-                         ' (Note: a timestamp sub-folder YYMMDD-HHMMSS is auto-appended, if not already such)')
-argser.add_argument('-n', '--notimestamp', dest='noTimestamp', action='store_true', default=False,
-                    help='Inhibit auto-timestamped work sub-folder creation (under work folder)')
-argser.add_argument('-x', '--distexport', dest='distExport', action='store_true', default=False,
-                    help='Export one Distance input file for each specified sample of the survey data'
-                         ' (Note: a sample spec. file and a survey data file must be also specified, through -p)')
-argser.add_argument('-e', '--preanalyses', dest='preAnalyses', action='store_true', default=False,
-                    help='Run pre-analyses for the specified samples of the survey data'
-                         ' (Note: a sample spec. file and a survey data file must be also specified, through -p)')
-argser.add_argument('-a', '--analyses', dest='analyses', action='store_true', default=False,
-                    help='Run analyses for the specified samples of the survey data'
-                         ' (Note: an analysis spec. file and a survey data file must be also specified, through -p)')
-argser.add_argument('-o', '--optanalyses', dest='optAnalyses', action='store_true', default=False,
-                    help='Run opt-analyses for the specified samples of the survey data'
-                         ' (Note: an opt-analysis spec. file and a survey data file must be also specified,'
-                         ' through -p)')
-argser.add_argument('-c', '--recoveropts', dest='recoverOpts', action='store_true', default=False,
-                    help='Restart optimisations at the point they were when interrupted (for any reason), from the'
-                         ' last usable recovery file found in the work folder (use in conjonction with -w & -n)'
-                         ' (Note: if no usable recovery file found, the restart will fail: no automatic restart from'
-                         ' scratch ; remove -c to do so)')
-argser.add_argument('-t', '--prereports', dest='preReports', type=str, default='none',
-                    help='Which reports to generate from pre-analyses results, through comma-separated keywords'
-                         ' among {excel, html, none} (case does not matter, none ignored if not alone)')
-argser.add_argument('-r', '--reports', dest='reports', type=str, default='none',
-                    help='Which reports to generate from analyses results, through comma-separated format:type'
-                         ' case-insensitive items with format among {excel, html, none}, "none" ignored if not alone ;'
-                         ' type among {full, <empty>} for excel format (use full to prevent default filter-sort report'
-                         " when filter-sort methods are available in the '-p' / '--params' parameters),"
-                         ' and among {full, <filter-sort method regex search string>*} (at least one of) for html ;'
-                         ' note: available filter-sort methods are automatically listed when auto-filtering parameters'
-                         ' are specified, so run command without -u first !'
-                         ' examples: none ; excel ; excel:full,html:full ; html:mqua92,html:full,excel,html:mqua950')
-argser.add_argument('-f', '--optreports', dest='optReports', type=str, default='none',
-                    help='Which reports to generate from opt-analyses results (same mini-language as for -r)')
-argser.add_argument('-l', '--logprefix', dest='logPrefix', type=str, default=None,
-                    help='Target log file path-name prefix (will be postfixed by .<YYMMDD-HHMMSS timestamp>.log)'
-                         f" (Default: <work folder>/{logger.DefLogNamePrefix} if -u/--run, else 'none' ;"
-                         "if special value 'none', no log saved)")
-argser.add_argument('-m', '--threads', dest='threads', type=int, default=0,
-                    help='Number of parallel threads to use for (pre/opt-)analyses / report generation'
-                         ' (default: 0 => auto-determined actual number of parallel threads from CPU specs ;'
-                         ' 1 for no parallelism ; for any other choice, first check your actual CPU specs)')
-argser.add_argument('-g', '--engine', dest='engineType', type=str, default='MCDS',
-                    choices=['MCDS'],
-                    help='The Distance engine to use, among MCDS, ... and no other for the moment'
-                         ' (insensitive to case)')
-
-args = argser.parse_args()
-logger.debug(f'Arguments: {args}')
-
-logger.setRealRun(args.realRun)
-
-if args.threads == 1:
-    args.threads = None  # No need for asynchronism: enforce sequential run.
-
-args.preReports = decodeReportArg(args.preReports, repName='pre-analysis report')
-args.reports = decodeReportArg(args.reports, repName='analysis report')
-args.optReports = decodeReportArg(args.optReports, repName='opt-analysis report')
-
-logger.info1('Arguments:')
-for k, v in vars(args).items():
-    logger.info1(f'* {k}: {v}')
-
-# 2. Load parameter python file, passing "special" parameters if any.
-speParamItems = args.speParams.split(',') if args.speParams else list()
-if any(item.count('=') != 1 for item in speParamItems):
-    logger.error(f'Syntax error in pre-parameters: "{args.speParams}"'
-                 ' (should be "name1=value1,name2=value2,...")')
-    sys.exit(2)
-
-speParams = dict([item.split('=') for item in speParamItems])
-paramFile, pars = loadPythonData(path=args.paramFile, **speParams)
-if not pars:
-    logger.error(f'Failed to load parameter file {paramFile.as_posix()}')
-    sys.exit(2)
-logger.debug1('Parameters: ' + ', '.join(vars(pars)))
-
-paramFiles = [paramFile.as_posix()]
-if 'paramFiles' in vars(pars):
-    paramFiles += pars.paramFiles
-
-# 3. More checks on args and parameters.
-# a. Check filter and sort report args
-if 'filsorReportSchemes' in vars(pars):
-    filsorSchemeIdMgr = FilterSortSchemeIdManager()
-    filsorReportSchemes = {filsorSchemeIdMgr.schemeId(sch): sch for sch in pars.filsorReportSchemes}
-    logger.info('Available filter & sort report schemes: ' + ', '.join(filsorReportSchemes.keys()))
-
-if 'html' in args.reports and not args.reports['html']:
-    logger.error('HTML analysis report: MUST specify type / filter & sort method')
-    sys.exit(2)
-
-if 'html' in args.reports and ('full' not in args.reports['html'] or len(args.reports['html']) > 1):
-
-    filsorMatches = {reSchId: [schId for schId in filsorReportSchemes if re.search(reSchId, schId, flags=re.I)]
-                     for reSchId in args.reports['html'] if reSchId != 'full'}
-    if any(len(matches) != 1 for matches in filsorMatches.values()) \
-       or len(filsorMatches) != len(set(match for matches in filsorMatches.values() for match in matches)):
-        logger.error('HTML analysis report: Bad or ambiguous filter & sort method specification(s) {}'
-                     .format(' ; '.join('{} => [{}]'.format(reSchId, ', '.join(matchSchemes))
-                                        for reSchId, matchSchemes in filsorMatches.items())))
-        sys.exit(2)
-
-    filsorAnlysReportSchemes = {schId: schValue for schId, schValue in filsorReportSchemes.items()
-                                if schId in set(match for matches in filsorMatches.values() for match in matches)}
-    if not filsorAnlysReportSchemes:
-        logger.error('HTML analysis report: No filter & sort method specified')
-        sys.exit(2)
-
-if 'html' in args.optReports and not args.optReports['html']:
-    logger.error('HTML opt-analysis report: MUST specify type / filter & sort method')
-    sys.exit(2)
-
-if 'html' in args.optReports and ('full' not in args.optReports['html'] or len(args.optReports['html']) > 1):
-
-    filsorMatches = {reSchId: [schId for schId in filsorReportSchemes if re.search(reSchId, schId, flags=re.I)]
-                     for reSchId in args.optReports['html'] if reSchId != 'full'}
-    if any(len(matches) != 1 for matches in filsorMatches.values()) \
-       or len(filsorMatches) != len(set(match for matches in filsorMatches.values() for match in matches)):
-        logger.error('HTML opt-analysis report: Bad or ambiguous filter & sort method specification(s) {}'
-                     .format(' ; '.join('{} => [{}]'.format(reSchId, ', '.join(matchSchemes))
-                                        for reSchId, matchSchemes in filsorMatches.items())))
-        sys.exit(2)
-
-    filsorOptAnlysReportSchemes = {schId: schValue for schId, schValue in filsorReportSchemes.items()
-                                   if schId in set(match for matches in filsorMatches.values() for match in matches)}
-    if not filsorOptAnlysReportSchemes:
-        logger.error('HTML opt-analysis report: No filter & sort method specified')
-        sys.exit(2)
-
-# 4. Output folder for results, reports ... etc.
-#    (post-fixed with the run timestamp, if not already specified)
-workDir = args.workDir if 'workDir' in vars(args) else pars.workDir if 'workDir' in vars(pars) else '.'
-workDir = pl.Path(workDir)
-if not (args.noTimestamp or re.match('.*[0-9]{6}-[0-9]{4,6}$', workDir.name)):
-    workDir = workDir / runTimestamp
-logger.info(f'Work folder: {workDir.as_posix()}')
-
-# 5. Now we can set up the final session log file path-name prefix !
-if args.logPrefix is None:
-    if args.realRun:  # Default
-        args.logPrefix = workDir.as_posix() + f'/{pars.studyName}{pars.subStudyName}'
-elif args.logPrefix.lower() == 'none':
-    args.logPrefix = None
-logger.setFinalLogPrefix(args.logPrefix)
-
-# 6. Really something to do ?
-emptyRun = not any([args.distExport, args.preAnalyses, args.preReports,
-                    args.analyses, args.reports, args.optAnalyses, args.optReports])
-if emptyRun:
-    logger.warning('No operation specified: nothing to do actually !')
-
-if args.realRun and not workDir.parent.exists():
-    workDir.parent.mkdir()  # pyaudisam create sub-dirs, but not parent
-
-# 7. Load input data if needed:
-# a. Survey data
-# * individualised data with distance from observer to observed "object",
-# * point transect definition
-if not emptyRun:
-
-    surveyDataFile = pars.surveyDataFile if 'surveyDataFile' in vars(pars) else None
-    if surveyDataFile:
-        surveyDataFile = pl.Path(surveyDataFile)
-        if surveyDataFile.exists():
-            indivDistSheet = pars.indivDistDataSheet if 'indivDistDataSheet' in vars(pars) else 0
-            transectSheet = pars.transectsDataSheet if 'transectsDataSheet' in vars(pars) else 1
-            logger.info1(f'Loading survey data and transects infos from file {surveyDataFile.as_posix()} ...')
-            with pd.ExcelFile(surveyDataFile) as xlInFile:
-                dfMonoCatObs = pd.read_excel(xlInFile, sheet_name=indivDistSheet)
-                dfTransects = pd.read_excel(xlInFile, sheet_name=transectSheet)
-            logger.info1(f'... found {len(dfMonoCatObs)} mono-category sightings and {len(dfTransects)} transects')
+        # c. Load generated HTML report and compare it to reference one
+        htmlRefRepLines = htmlRefReportLines_fxt
+
+        with open(htmlRep) as file:
+            htmlActRepLines = file.readlines()
+
+        self.compareHtmlReports(htmlRefRepLines, htmlActRepLines)
+
+        # e. Cleanup generated report (well ... partially at least)
+        #    for clearing next function's ground
+        if postCleanup:
+            pl.Path(xlsxRep).unlink()
+            pl.Path(htmlRep).unlink()
         else:
-            logger.error(f'Could not find survey data file {surveyDataFile.as_posix()}')
-            sys.exit(2)
-    else:
-        logger.error('No survey data file specified, can\'t export Distance file or run any type of analysis')
-        sys.exit(2)
-
-# 7.b. Sample specs
-if args.distExport or args.preAnalyses:
-
-    sampleSpecFile = pars.sampleSpecFile if 'sampleSpecFile' in vars(pars) else None
-    if sampleSpecFile:
-        sampleSpecFile = pl.Path(sampleSpecFile)
-        if not sampleSpecFile.exists():
-            logger.error(f'Could not find sample spec. file {sampleSpecFile.as_posix()}')
-            sys.exit(2)
-    else:
-        logger.error('No sample spec. file specified, can\'t export Distance file or run pre-analyses')
-        sys.exit(2)
-
-# 8. Export input files for Distance software, for manual analyses (if specified to).
-sampExplSpecFilePath = workDir / f'{pars.studyName}{pars.subStudyName}-samples-explispecs.xlsx'
-if sampExplSpecFilePath.exists():
-    logger.info('Found sample explicit specs file ' + sampExplSpecFilePath.as_posix())
-
-if args.distExport:
-
-    oprText = 'export of input data files for Distance'
-    logger.openOperation(oprText)
-
-    # a. Create PreAnalyser object.
-    preAnlysr = MCDSPreAnalyser(dfMonoCatObs, dfTransects=dfTransects, dSurveyArea=pars.studyAreaSpecs,
-                                effortConstVal=pars.passEffort, effortCol=pars.effortCol,
-                                transectPlaceCols=pars.transectPlaceCols, passIdCol=pars.passIdCol,
-                                sampleSelCols=pars.sampleSelCols,
-                                sampleDecCols=[pars.effortCol, pars.distanceCol],
-                                sampleIndCol=pars.sampleIndCol, sampleSpecCustCols=pars.sampleSpecCustCols,
-                                abbrevCol=pars.sampleAbbrevCol, abbrevBuilder=pars.sampleAbbrev,
-                                distanceUnit=pars.distanceUnit, areaUnit=pars.areaUnit,
-                                surveyType=pars.surveyType, distanceType=pars.distanceType,
-                                clustering=pars.clustering,
-                                workDir=workDir)
-
-    # b. Check sample specs.
-    dfExplSampleSpecs, userParamSpecCols, intParamSpecCols, unmUserParamSpecCols, verdict, reasons = \
-        preAnlysr.explicitParamSpecs(implParamSpecs=sampleSpecFile, dropDupes=True, check=True)
-
-    assert userParamSpecCols == []  # No analysis params here (auto. generated by PreAnalyser)
-    assert intParamSpecCols == []  # Idem
-    assert verdict
-    assert not reasons
-
-    logger.info2(f'Explicit sample specs:\n{dfExplSampleSpecs.to_string()}')
-    logger.info1(f'From sample specs, {len(dfExplSampleSpecs)} samples to export')
-    if args.verbose and not args.realRun:
-        while not sampExplSpecFilePath.parent.exists():
-            sampExplSpecFilePath = sampExplSpecFilePath.parent.parent / sampExplSpecFilePath.name
-        dfExplSampleSpecs.to_excel(sampExplSpecFilePath, index=False)
-
-    # b. Export 1 Distance input data file for each specified sample.
-    if args.realRun:
-        preAnlysr.exportDSInputData(implSampleSpecs=sampleSpecFile, format='Distance')
-        dfExplSampleSpecs.to_excel(sampExplSpecFilePath, index=False)
-    preAnlysr.shutdown()  # Not really needed, actually.
-
-    logger.closeOperation(oprText)
-
-# 9. Run pre-analyses (if specified to).
-PreAnalyser = MCDSPreAnalyser
-resultsWord = 'resultats' if pars.studyLang == 'fr' else 'results'
-preAnlysResFilePath = workDir / f'{pars.studyName}{pars.subStudyName}-preanalyses-{resultsWord}.xlsx'
-if preAnlysResFilePath.exists():
-    logger.info('Found pre-analyses results file ' + preAnlysResFilePath.as_posix())
-
-if args.preAnalyses:
-
-    oprText = 'pre-analyses'
-    logger.openOperation(oprText)
-
-    # a. Create PreAnalyser object.
-    preAnlysr = PreAnalyser(dfMonoCatObs, dfTransects=dfTransects, dSurveyArea=pars.studyAreaSpecs,
-                            effortConstVal=pars.passEffort, effortCol=pars.effortCol,
-                            transectPlaceCols=pars.transectPlaceCols, passIdCol=pars.passIdCol,
-                            sampleSelCols=pars.sampleSelCols,
-                            sampleDecCols=[pars.effortCol, pars.distanceCol],
-                            sampleIndCol=pars.sampleIndCol, sampleSpecCustCols=pars.sampleSpecCustCols,
-                            abbrevCol=pars.sampleAbbrevCol, abbrevBuilder=pars.sampleAbbrev,
-                            distanceUnit=pars.distanceUnit, areaUnit=pars.areaUnit,
-                            surveyType=pars.surveyType, distanceType=pars.distanceType,
-                            clustering=pars.clustering,
-                            resultsHeadCols=pars.preResultsHeadCols,
-                            workDir=workDir,
-                            runMethod=pars.runPreAnalysisMethod, runTimeOut=pars.runPreAnalysisTimeOut,
-                            logData=pars.logPreAnalysisData, logProgressEvery=pars.logPreAnalysisProgressEvery)
-
-    # b. Check sample specs.
-    dfExplSampleSpecs, userParamSpecCols, intParamSpecCols, unmUserParamSpecCols, verdict, reasons = \
-        preAnlysr.explicitParamSpecs(implParamSpecs=sampleSpecFile, dropDupes=True, check=True)
-
-    assert userParamSpecCols == []  # No analysis params here (auto. generated by PreAnalyser)
-    assert verdict
-    assert not reasons
-
-    logger.info2(f'Explicit sample specs:\n{dfExplSampleSpecs.to_string()}')
-    logger.info2(f'Pre-analysis model fallback strategy:\n{pd.DataFrame(pars.modelPreStrategy).to_string()}')
-    logger.info1(f'From sample specs, {len(dfExplSampleSpecs)} samples to pre-analyse')
-    if args.verbose and not args.realRun:
-        while not sampExplSpecFilePath.parent.exists():
-            sampExplSpecFilePath = sampExplSpecFilePath.parent.parent / sampExplSpecFilePath.name
-        dfExplSampleSpecs.to_excel(sampExplSpecFilePath, index=False)
-
-    if any(col not in dfExplSampleSpecs.columns for col in pars.sampleSpecCustCols):
-        logger.error('Missing custom (pass-through) column(s) in sample specs: {}'
-                     .format(', '.join(col for col in pars.sampleSpecCustCols
-                                       if col not in dfExplSampleSpecs.columns)))
-        sys.exit(2)
-
-    # c. Run pre-analyses.
-    if args.realRun:
-        preResults = preAnlysr.run(implSampleSpecs=sampleSpecFile, dModelStrategy=pars.modelPreStrategy,
-                                   threads=args.threads)
-        dfExplSampleSpecs.to_excel(sampExplSpecFilePath, index=False)
-    preAnlysr.shutdown()
-
-    # d. Save results to disk.
-    # if 'dfSampleStats' in dir(): # Qq specs supplémentaires
-    #    preResults.updateSpecs(sampleStats=dfSampleStats)
-    if args.realRun:
-        preResults.toExcel(preAnlysResFilePath)
-
-    logger.closeOperation(oprText)
-
-# 10. Generate pre-analysis reports (if specified to).
-PreReport = MCDSResultsPreReport
-reportWord = 'rapport' if pars.studyLang == 'fr' else 'report'
-if args.preReports:
-
-    # a. Load pre-analyses results if not just computed
-    if not args.preAnalyses:
-
-        if not preAnlysResFilePath.exists():
-            logger.error('Cannot generate pre-analysis reports:'
-                         f' results file not found {preAnlysResFilePath.as_posix()}')
-            sys.exit(2)
-
-        logger.info(f'Loading pre-analysis results from {preAnlysResFilePath.as_posix()}')
-
-        preAnlysr = PreAnalyser(dfMonoCatObs, dfTransects=dfTransects, dSurveyArea=pars.studyAreaSpecs,
-                                effortConstVal=pars.passEffort, effortCol=pars.effortCol,
-                                transectPlaceCols=pars.transectPlaceCols, passIdCol=pars.passIdCol,
-                                sampleSelCols=pars.sampleSelCols,
-                                sampleDecCols=[pars.effortCol, pars.distanceCol],
-                                sampleIndCol=pars.sampleIndCol, sampleSpecCustCols=pars.sampleSpecCustCols,
-                                abbrevCol=pars.sampleAbbrevCol, abbrevBuilder=pars.sampleAbbrev,
-                                distanceUnit=pars.distanceUnit, areaUnit=pars.areaUnit,
-                                surveyType=pars.surveyType, distanceType=pars.distanceType,
-                                clustering=pars.clustering,
-                                resultsHeadCols=pars.preResultsHeadCols)
-
-        preResults = preAnlysr.setupResults()
-        preAnlysr.shutdown()  # Not really needed, actually.
-
-        preResults.fromFile(preAnlysResFilePath)
-
-    # b. Check report generation parameters
-    assert isinstance(pars.preReportSortAscend, bool) or len(pars.preReportSortCols) == len(pars.preReportSortAscend)
-
-    # c. Generate specified reports
-    oprText = 'generation of {} pre-analysis report(s)'.format(','.join(args.preReports))
-    logger.openOperation(oprText)
-
-    preRepPrfx = f'{pars.studyName}{pars.subStudyName}-preanalyses-{reportWord}'
-    preReport = PreReport(resultsSet=preResults, lang=pars.studyLang,
-                          title=pars.preReportStudyTitle, subTitle=pars.preReportStudySubTitle,
-                          anlysSubTitle=pars.preReportAnlysSubTitle, description=pars.preReportStudyDescr,
-                          keywords=pars.preReportStudyKeywords, pySources=paramFiles,
-                          sampleCols=pars.preReportSampleCols, paramCols=pars.preReportParamCols,
-                          resultCols=pars.preReportResultCols, synthCols=pars.preReportSynthCols,
-                          sortCols=pars.preReportSortCols, sortAscend=pars.preReportSortAscend,
-                          tgtFolder=workDir, tgtPrefix=preRepPrfx,
-                          **pars.preReportPlotParams)
-
-    if 'excel' in args.preReports:
-        logger.info1('* Excel pre-analysis report to be generated')
-        if args.realRun:
-            preReport.toExcel(rebuild=pars.preReportRebuild)
-
-    if 'html' in args.preReports:
-        logger.info1('* HTML pre-analysis report to be generated')
-        if args.realRun:
-            preReport.toHtml(rebuild=pars.preReportRebuild,
-                             generators=1 if args.threads is None else args.threads)
-
-    logger.closeOperation(oprText)
-
-# 11. Run analyses (if specified to).
-Analyser = MCDSAnalyser
-anlysExplSpecFilePath = workDir / f'{pars.studyName}{pars.subStudyName}-analyses-explispecs.xlsx'
-if anlysExplSpecFilePath.exists():
-    logger.info('Found analyses explicit spec. file ' + anlysExplSpecFilePath.as_posix())
-anlysResFilePath = workDir / f'{pars.studyName}{pars.subStudyName}-analyses-{resultsWord}.xlsx'
-if anlysResFilePath.exists():
-    logger.info('Found analyses results file ' + anlysResFilePath.as_posix())
-
-if args.analyses:
-
-    # Check analysis spec. file
-    analysisSpecFile = pars.analysisSpecFile if 'analysisSpecFile' in vars(pars) else None
-    if analysisSpecFile:
-        analysisSpecFile = pl.Path(analysisSpecFile)
-        if not analysisSpecFile.exists():
-            logger.error(f'Could not find analysis spec. file {analysisSpecFile.as_posix()}')
-            sys.exit(2)
-    else:
-        logger.error('No analysis spec. file specified, can\'t run analyses')
-        sys.exit(2)
-
-    oprText = 'analyses'
-    logger.openOperation(oprText)
-
-    # a. Create Analyser object.
-    anlysr = Analyser(dfMonoCatObs, dfTransects=dfTransects, dSurveyArea=pars.studyAreaSpecs,
-                      effortConstVal=pars.passEffort, effortCol=pars.effortCol,
-                      transectPlaceCols=pars.transectPlaceCols, passIdCol=pars.passIdCol,
-                      sampleSelCols=pars.sampleSelCols, sampleDecCols=[pars.effortCol, pars.distanceCol],
-                      anlysSpecCustCols=pars.analysisSpecCustCols,
-                      abbrevCol=pars.analysisAbbrevCol, abbrevBuilder=pars.analysisAbbrev,
-                      anlysIndCol=pars.analysisIndCol, sampleIndCol=pars.sampleIndCol,
-                      distanceUnit=pars.distanceUnit, areaUnit=pars.areaUnit,
-                      surveyType=pars.surveyType, distanceType=pars.distanceType,
-                      clustering=pars.clustering,
-                      resultsHeadCols=pars.resultsHeadCols,
-                      ldTruncIntrvSpecs=pars.ldTruncIntrvSpecs, truncIntrvEpsilon=pars.truncIntrvEpsilon,
-                      workDir=workDir, runMethod=pars.runAnalysisMethod, runTimeOut=pars.runAnalysisTimeOut,
-                      logData=pars.logAnalysisData, logProgressEvery=pars.logAnalysisProgressEvery,
-                      defEstimKeyFn=pars.defEstimKeyFn, defEstimAdjustFn=pars.defEstimAdjustFn,
-                      defEstimCriterion=pars.defEstimCriterion, defCVInterval=pars.defCVInterval,
-                      defMinDist=pars.defMinDist, defMaxDist=pars.defMaxDist,
-                      defFitDistCuts=pars.defFitDistCuts, defDiscrDistCuts=pars.defDiscrDistCuts)
-
-    # b. Check analysis specs.
-    dfExplAnlysSpecs, userParamSpecCols, intParamSpecCols, unmUserParamSpecCols, verdict, reasons = \
-        anlysr.explicitParamSpecs(implParamSpecs=analysisSpecFile, dropDupes=True, check=True)
-
-    assert userParamSpecCols == pars.analysisParamCols
-    assert verdict
-    assert not reasons
-
-    logger.info2(f'Explicit analysis specs:\n{dfExplAnlysSpecs.to_string()}')
-    logger.info1(f'From analysis specs, {len(dfExplAnlysSpecs)} analyses to run')
-    if args.verbose and not args.realRun:
-        while not anlysExplSpecFilePath.parent.exists():
-            anlysExplSpecFilePath = anlysExplSpecFilePath.parent.parent / anlysExplSpecFilePath.name
-        dfExplAnlysSpecs.to_excel(anlysExplSpecFilePath, index=False)
-
-    if any(col not in dfExplAnlysSpecs.columns for col in pars.analysisSpecCustCols):
-        logger.error('Missing custom (pass-through) column(s) in analysis specs: {}'
-                     .format(', '.join(col for col in pars.analysisSpecCustCols
-                                       if col not in dfExplAnlysSpecs.columns)))
-        sys.exit(2)
-
-    # c. Run analyses.
-    if args.realRun:
-        results = anlysr.run(implParamSpecs=analysisSpecFile, threads=args.threads)
-        dfExplAnlysSpecs.to_excel(anlysExplSpecFilePath, index=False)
-    anlysr.shutdown()
-
-    # d. Save results to disk.
-    if args.realRun:
-        results.toExcel(anlysResFilePath)
-
-    logger.closeOperation(oprText)
-
-# 12. Generate analysis reports (if specified to).
-FullReport = MCDSResultsFullReport
-FilSorReport = MCDSResultsFilterSortReport
-
-if args.reports:
-
-    # a. Load analysis results if not just computed
-    if not args.analyses:
-
-        if not anlysResFilePath.exists():
-            logger.error(f'Cannot generate analysis reports: results file not found {anlysResFilePath.as_posix()}')
-            sys.exit(2)
-
-        logger.info(f'Loading analysis results from {anlysResFilePath.as_posix()}')
-
-        anlysr = Analyser(dfMonoCatObs, dfTransects=dfTransects, dSurveyArea=pars.studyAreaSpecs,
-                          effortConstVal=pars.passEffort, effortCol=pars.effortCol,
-                          transectPlaceCols=pars.transectPlaceCols, passIdCol=pars.passIdCol,
-                          sampleSelCols=pars.sampleSelCols, sampleDecCols=[pars.effortCol, pars.distanceCol],
-                          anlysSpecCustCols=pars.analysisSpecCustCols,
-                          abbrevCol=pars.analysisAbbrevCol, abbrevBuilder=pars.analysisAbbrev,
-                          anlysIndCol=pars.analysisIndCol, sampleIndCol=pars.sampleIndCol,
-                          distanceUnit=pars.distanceUnit, areaUnit=pars.areaUnit,
-                          surveyType=pars.surveyType, distanceType=pars.distanceType,
-                          clustering=pars.clustering,
-                          resultsHeadCols=pars.resultsHeadCols)
-
-        results = anlysr.setupResults()
-        anlysr.shutdown()  # Not really needed, actually.
-
-        results.fromFile(anlysResFilePath)
-
-    # b. Generate specified reports
-    oprText = 'generation of {} analysis report(s)'.format(','.join(args.reports))
-    logger.openOperation(oprText)
-
-    repPrfx = f'{pars.studyName}{pars.subStudyName}-analyses-{reportWord}'
-
-    # * Auto-filtered reports.
-    if ('excel' in args.reports and 'full' not in args.reports['excel'] and 'filsorReportSchemes' in dir()) \
-       or ('html' in args.reports and 'full' not in args.reports['html'] and 'filsorAnlysReportSchemes' in dir()):
-
-        assert isinstance(pars.filsorReportSortAscend, bool) \
-               or len(pars.filsorReportSortCols) == len(pars.filsorReportSortAscend)
-
-        filsorReport = FilSorReport(resultsSet=results, lang=pars.studyLang,
-                                    title=pars.anlysFilsorReportStudyTitle,
-                                    subTitle=pars.anlysFilsorReportStudySubTitle,
-                                    anlysSubTitle=pars.anlysFilsorReportAnlysSubTitle,
-                                    description=pars.anlysFilsorReportStudyDescr,
-                                    keywords=pars.anlysFilsorReportStudyKeywords, pySources=paramFiles,
-                                    sampleCols=pars.filsorReportSampleCols, paramCols=pars.filsorReportParamCols,
-                                    resultCols=pars.filsorReportResultCols, synthCols=pars.filsorReportSynthCols,
-                                    sortCols=pars.filsorReportSortCols, sortAscend=pars.filsorReportSortAscend,
-                                    filSorSchemes=pars.filsorReportSchemes,
-                                    tgtFolder=workDir, tgtPrefix=repPrfx,
-                                    **pars.filsorReportPlotParams)
-
-        if 'excel' in args.reports and 'full' not in args.reports['excel'] and 'filsorReportSchemes' in dir():
-            logger.info1('* Auto-filtered Excel analysis report to be generated: all schemes')
-            if args.realRun:
-                filsorReport.toExcel(rebuild=pars.filsorReportRebuild)
-
-        if 'html' in args.reports and 'full' not in args.reports['html'] and 'filsorAnlysReportSchemes' in dir():
-            logger.info1('* Auto-filtered HTML analysis report(s) to be generated: {}'
-                         .format(', '.join(filsorAnlysReportSchemes.keys())))
-            if args.realRun:
-                for scheme in filsorAnlysReportSchemes.values():
-                    filsorReport.toHtml(filSorScheme=scheme, rebuild=pars.filsorReportRebuild)
-
-    # * Full reports.
-    if ('excel' in args.reports and ('full' in args.reports['excel'] or 'filsorReportSchemes' not in dir())) \
-       or ('html' in args.reports and 'full' in args.reports['html']):
-
-        assert isinstance(pars.fullReportSortAscend, bool) \
-               or len(pars.fullReportSortCols) == len(pars.fullReportSortAscend)
-
-        fullReport = FullReport(resultsSet=results, lang=pars.studyLang,
-                                title=pars.anlysFullReportStudyTitle,
-                                subTitle=pars.anlysFullReportStudySubTitle,
-                                anlysSubTitle=pars.anlysFullReportAnlysSubTitle,
-                                description=pars.anlysFullReportStudyDescr,
-                                keywords=pars.anlysFullReportStudyKeywords, pySources=paramFiles,
-                                sampleCols=pars.fullReportSampleCols, paramCols=pars.fullReportParamCols,
-                                resultCols=pars.fullReportResultCols, synthCols=pars.fullReportSynthCols,
-                                sortCols=pars.fullReportSortCols, sortAscend=pars.fullReportSortAscend,
-                                tgtFolder=workDir, tgtPrefix=repPrfx,
-                                **pars.fullReportPlotParams)
-
-        if 'excel' in args.reports and ('full' in args.reports['excel'] or 'filsorReportSchemes' not in dir()):
-            logger.info1('* Full Excel analysis report to be generated')
-            if args.realRun:
-                fullReport.toExcel(rebuild=pars.fullReportRebuild)
-
-        if 'html' in args.reports and 'full' in args.reports['html']:
-            logger.info1('* Full HTML analysis report to be generated')
-            if args.realRun:
-                fullReport.toHtml(rebuild=pars.fullReportRebuild,
-                                  generators=1 if args.threads is None else args.threads)
-
-    # if not any(rep in dir() for rep in ['fullReport', 'filsorReport']):  # This doesn't work ... !!??
-    if not any(['fullReport' in dir(), 'filsorReport' in dir()]):
-        logger.error('Neither full nor filter & sort analysis report to be generated (whatever format)')
-        sys.exit(2)
-
-    logger.closeOperation(oprText)
-
-# 13. Run opt-analyses (if specified to).
-OptAnalyser = MCDSTruncationOptanalyser
-optAnlysExplSpecFilePath = workDir / f'{pars.studyName}{pars.subStudyName}-optanalyses-explispecs.xlsx'
-if optAnlysExplSpecFilePath.exists():
-    logger.info('Found opt-analyses explicit spec. file ' + optAnlysExplSpecFilePath.as_posix())
-optAnlysResFilePath = workDir / f'{pars.studyName}{pars.subStudyName}-optanalyses-{resultsWord}.xlsx'
-if optAnlysResFilePath.exists():
-    logger.info('Found opt-analyses results file ' + optAnlysResFilePath.as_posix())
-if args.optAnalyses:
-
-    # Check analysis spec. file
-    optAnalysisSpecFile = pars.optAnalysisSpecFile if 'optAnalysisSpecFile' in vars(pars) else None
-    if optAnalysisSpecFile:
-        optAnalysisSpecFile = pl.Path(optAnalysisSpecFile)
-        if not optAnalysisSpecFile.exists():
-            logger.error(f'Could not find opt-analysis spec. file {optAnalysisSpecFile.as_posix()}')
-            sys.exit(2)
-    else:
-        logger.error('No opt-analysis spec. file specified, can\'t run opt-analyses')
-        sys.exit(2)
-
-    oprText = 'opt-analyses'
-    logger.openOperation(oprText)
-
-    # a. Create OptAnalyser object.
-    optAnlysr = OptAnalyser(dfMonoCatObs, dfTransects=dfTransects, dSurveyArea=pars.studyAreaSpecs,
-                            effortConstVal=pars.passEffort, effortCol=pars.effortCol,
-                            transectPlaceCols=pars.transectPlaceCols, passIdCol=pars.passIdCol,
-                            sampleSelCols=pars.sampleSelCols, sampleDecCols=[pars.effortCol, pars.distanceCol],
-                            sampleDistCol=pars.distanceCol, anlysSpecCustCols=pars.optAnalysisSpecCustCols,
-                            abbrevCol=pars.analysisAbbrevCol, abbrevBuilder=pars.analysisAbbrev,
-                            anlysIndCol=pars.analysisIndCol, sampleIndCol=pars.sampleIndCol,
-                            distanceUnit=pars.distanceUnit, areaUnit=pars.areaUnit,
-                            surveyType=pars.surveyType, distanceType=pars.distanceType,
-                            clustering=pars.clustering,
-                            resultsHeadCols=pars.optResultsHeadCols,
-                            ldTruncIntrvSpecs=pars.ldTruncIntrvSpecs, truncIntrvEpsilon=pars.truncIntrvEpsilon,
-                            workDir=workDir, logData=pars.logOptAnalysisData,
-                            runMethod=pars.runOptAnalysisMethod, runTimeOut=pars.runOptAnalysisTimeOut,
-                            logAnlysProgressEvery=pars.logOptAnalysisProgressEvery,
-                            logOptimProgressEvery=pars.logOptimisationProgressEvery,
-                            backupOptimEvery=pars.backupOptimisationsEvery,
-                            defEstimKeyFn=pars.defEstimKeyFn, defEstimAdjustFn=pars.defEstimAdjustFn,
-                            defEstimCriterion=pars.defEstimCriterion, defCVInterval=pars.defCVInterval,
-                            defExpr2Optimise=pars.defExpr2Optimise, defMinimiseExpr=pars.defMinimiseExpr,
-                            defOutliersMethod=pars.defOutliersMethod,
-                            defOutliersQuantCutPct=pars.defOutliersQuantCutPct,
-                            defFitDistCutsFctr=pars.defFitDistCutsFctr,
-                            defDiscrDistCutsFctr=pars.defDiscrDistCutsFctr,
-                            defSubmitTimes=pars.defSubmitTimes, defSubmitOnlyBest=pars.defSubmitOnlyBest,
-                            dDefSubmitOtherParams=pars.dDefSubmitOtherParams,
-                            dDefOptimCoreParams=dict(core=pars.defCoreEngine, maxIters=pars.defCoreMaxIters,
-                                                     termExprValue=pars.defCoreTermExprValue,
-                                                     algorithm=pars.defCoreAlgorithm,
-                                                     maxRetries=pars.defCoreMaxRetries))
-
-    # b. Check opt-analysis specs.
-    dfExplOptAnlysSpecs, userParamSpecCols, intParamSpecCols, unmUserParamSpecCols, verdict, reasons = \
-        optAnlysr.explicitParamSpecs(implParamSpecs=optAnalysisSpecFile, dropDupes=True, check=True)
-
-    assert userParamSpecCols == pars.optAnalysisParamCols
-    assert verdict
-    assert not reasons
-
-    logger.info2(f'Explicit opt-analysis specs:\n{dfExplOptAnlysSpecs.to_string()}')
-    optUserParamSpecCols = optAnlysr.zoptr4Specs.optimisationParamSpecUserNames(userParamSpecCols, intParamSpecCols)
-    sbAnlysNeedOpt = dfExplOptAnlysSpecs[optUserParamSpecCols].apply(optAnlysr.analysisNeedsOptimisationFirst,
-                                                                     axis='columns')
-    logger.info1('From opt-analysis specs, {} / {} opt-analyses to run with truncation optimisation first ...'
-                 .format(sbAnlysNeedOpt.sum(), len(dfExplOptAnlysSpecs)))
-    logger.info1('... implying possibly up to {} auto-analyses in the background if only full "auto" specs'
-                 .format(sbAnlysNeedOpt.sum() * pars.defCoreMaxIters * pars.defSubmitTimes))
-    if args.verbose and not args.realRun:
-        while not optAnlysExplSpecFilePath.parent.exists():
-            optAnlysExplSpecFilePath = optAnlysExplSpecFilePath.parent.parent / optAnlysExplSpecFilePath.name
-        dfExplOptAnlysSpecs.to_excel(optAnlysExplSpecFilePath, index=False)
-
-    if any(col not in dfExplOptAnlysSpecs.columns for col in pars.optAnalysisSpecCustCols):
-        logger.error('Missing custom (pass-through) column(s) in opt-analysis specs: {}'
-                     .format(', '.join(col for col in pars.optAnalysisSpecCustCols
-                                       if col not in dfExplOptAnlysSpecs.columns)))
-        sys.exit(2)
-
-    # c. Check if recovery possible (not 100% reliable), if specified
-    if args.recoverOpts:
-        if not list(workDir.glob('optr-resbak-*.pickle.xz')):
-            logger.error('No optimisation backup file found, can\'t recover ; you must start from scratch')
-            sys.exit(2)
+            logger.warning('NOT cleaning up reports: this is not the normal testing scheme !')
+
+        # f. Done.
+        logger.info(f'PASS testReports: MCDSResultsReport ctor, toExcel, toHtml')
+
+    # ## 7. Generate HTML and Excel pre-analyses reports through pyaudisam command line
+    def testReportsCli(self, sampleSpecMode, excelRefReport_fxt, htmlRefReportLines_fxt):
+
+        if sampleSpecMode != 'implicit':
+            msg = 'testReportsCli(explicit): skipped, as not relevant'
+            logger.info(msg)
+            pytest.skip(msg)  # Raises an exception => function execution stops here.
+
+        build = True  # Debug only: Set to False to avoid rebuilding the report
+
+        # a. Report "through the commande line"
+        workPath = uivu.pWorkDir
+        if build:
+            argv = f'-p {uivu.pTestDir.as_posix()}/valtests-ds-params.py -w {workPath.as_posix()}' \
+                   ' -n --prereports excel,html -u'.split()
+            rc = ads.main(argv, standaloneLogConfig=False)
+            logger.info(f'CLI run: rc={rc}')
         else:
-            logger.info('Backup files are there, recovery is very likely possible: let\'s try !')
+            logger.warning('NOT building the reports: this is not the normal testing scheme !')
+
+        # b. Load generated Excel report and compare it to reference one
+        ddfActRep = pd.read_excel(workPath / 'valtests-preanalyses-report.xlsx', sheet_name=None, index_col=0)
+
+        ddfRefRep = excelRefReport_fxt
+        self.compareExcelReports(ddfRefRep, ddfActRep)
 
-    # d. Run opt-analyses.
-    if args.realRun:
-        optResults = optAnlysr.run(implParamSpecs=optAnalysisSpecFile,
-                                   threads=args.threads, recoverOptims=args.recoverOpts)
-        dfExplOptAnlysSpecs.to_excel(optAnlysExplSpecFilePath, index=False)
-    optAnlysr.shutdown()
-
-    # e. Save results to disk.
-    if args.realRun:
-        optResults.toExcel(optAnlysResFilePath)
-
-    logger.closeOperation(oprText)
-
-# 14. Generate opt-analysis reports (if specified to).
-if args.optReports:
-
-    # a. Load opt-analysis results if not just computed
-    if not args.optAnalyses:
-
-        if not optAnlysResFilePath.exists():
-            logger.error('Cannot generate opt-analysis reports:'
-                         f' results file not found {optAnlysResFilePath.as_posix()}')
-            sys.exit(2)
-
-        logger.info(f'Loading opt-analysis results from {optAnlysResFilePath.as_posix()}')
-
-        optAnlysr = OptAnalyser(dfMonoCatObs, dfTransects=dfTransects, dSurveyArea=pars.studyAreaSpecs,
-                                effortConstVal=pars.passEffort, effortCol=pars.effortCol,
-                                transectPlaceCols=pars.transectPlaceCols, passIdCol=pars.passIdCol,
-                                sampleSelCols=pars.sampleSelCols, sampleDecCols=[pars.effortCol, pars.distanceCol],
-                                sampleDistCol=pars.distanceCol, anlysSpecCustCols=pars.optAnalysisSpecCustCols,
-                                abbrevCol=pars.analysisAbbrevCol, abbrevBuilder=pars.analysisAbbrev,
-                                anlysIndCol=pars.analysisIndCol, sampleIndCol=pars.sampleIndCol,
-                                distanceUnit=pars.distanceUnit, areaUnit=pars.areaUnit,
-                                surveyType=pars.surveyType, distanceType=pars.distanceType,
-                                clustering=pars.clustering,
-                                resultsHeadCols=pars.optResultsHeadCols)
-
-        optResults = optAnlysr.setupResults()
-        optAnlysr.shutdown()  # Not really needed, actually.
-
-        optResults.fromFile(optAnlysResFilePath)
-
-    # b. Generate specified reports
-    assert isinstance(pars.filsorReportSortAscend, bool) \
-           or len(pars.filsorReportSortCols) == len(pars.filsorReportSortAscend)
-
-    oprText = 'generation of {} opt-analysis report(s)'.format(','.join(args.optReports))
-    logger.openOperation(oprText)
-
-    optRepPrfx = f'{pars.studyName}{pars.subStudyName}-optanalyses-{reportWord}'
-
-    # * Auto-filtered reports.
-    if ('excel' in args.optReports and 'full' not in args.optReports['excel'] and 'filsorReportSchemes' in dir()) \
-       or ('html' in args.optReports and 'filsorOptAnlysReportSchemes' in dir()):
-
-        assert isinstance(pars.filsorReportSortAscend, bool) \
-               or len(pars.filsorReportSortCols) == len(pars.filsorReportSortAscend)
-
-        filsorOptReport = FilSorReport(resultsSet=optResults, lang=pars.studyLang,
-                                       title=pars.optAnlysFilsorReportStudyTitle,
-                                       subTitle=pars.optAnlysFilsorReportStudySubTitle,
-                                       anlysSubTitle=pars.optAnlysFilsorReportAnlysSubTitle,
-                                       description=pars.optAnlysFilsorReportStudyDescr,
-                                       keywords=pars.optAnlysFilsorReportStudyKeywords, pySources=paramFiles,
-                                       sampleCols=pars.filsorReportSampleCols, paramCols=pars.filsorReportParamCols,
-                                       resultCols=pars.filsorReportResultCols, synthCols=pars.filsorReportSynthCols,
-                                       sortCols=pars.filsorReportSortCols, sortAscend=pars.filsorReportSortAscend,
-                                       filSorSchemes=pars.filsorReportSchemes,
-                                       tgtFolder=workDir, tgtPrefix=optRepPrfx,
-                                       **pars.filsorReportPlotParams)
-
-        if 'excel' in args.optReports and 'full' not in args.optReports['excel'] and 'filsorReportSchemes' in dir():
-            logger.info1('* Auto-filtered Excel opt-analysis report to be generated: all schemes')
-            if args.realRun:
-                filsorOptReport.toExcel(rebuild=pars.filsorReportRebuild)
-
-        if 'html' in args.optReports and 'filsorOptAnlysReportSchemes' in dir():
-            logger.info1('* Auto-filtered HTML opt-analysis report(s) to be generated: {}'
-                         .format(', '.join(filsorOptAnlysReportSchemes.keys())))
-            if args.realRun:
-                for scheme in filsorOptAnlysReportSchemes.values():
-                    filsorOptReport.toHtml(filSorScheme=scheme, rebuild=pars.filsorReportRebuild)
-
-    # * Full reports.
-    if ('excel' in args.optReports and ('full' in args.optReports['excel'] or 'filsorReportSchemes' not in dir())) \
-       or ('html' in args.optReports and 'full' in args.optReports['html']):
-
-        assert isinstance(pars.fullReportSortAscend, bool) \
-               or len(pars.fullReportSortCols) == len(pars.fullReportSortAscend)
-
-        fullOptReport = FullReport(resultsSet=optResults, lang=pars.studyLang,
-                                   title=pars.optAnlysFullReportStudyTitle,
-                                   subTitle=pars.optAnlysFullReportStudySubTitle,
-                                   anlysSubTitle=pars.optAnlysFullReportAnlysSubTitle,
-                                   description=pars.optAnlysFullReportStudyDescr,
-                                   keywords=pars.optAnlysFullReportStudyKeywords, pySources=paramFiles,
-                                   sampleCols=pars.fullReportSampleCols, paramCols=pars.fullReportParamCols,
-                                   resultCols=pars.fullReportResultCols, synthCols=pars.fullReportSynthCols,
-                                   sortCols=pars.fullReportSortCols, sortAscend=pars.fullReportSortAscend,
-                                   tgtFolder=workDir, tgtPrefix=optRepPrfx,
-                                   **pars.fullReportPlotParams)
-
-        if 'excel' in args.optReports \
-           and ('full' in args.optReports['excel'] or 'filsorReportSchemes' not in dir()):
-            logger.info1('* Full Excel opt-analysis report to be generated')
-            if args.realRun:
-                fullOptReport.toExcel(rebuild=pars.fullReportRebuild)
-
-        if 'html' in args.optReports and 'full' in args.optReports['html']:
-            logger.info1('* Full HTML opt-analysis report to be generated')
-            if args.realRun:
-                fullOptReport.toHtml(rebuild=pars.fullReportRebuild,
-                                     generators=1 if args.threads is None else args.threads)
-
-    # if not any(rep in dir() for rep in ['fullOptReport', 'filsorOptReport']):  # This doesn't work ... !!??
-    if not any(['fullOptReport' in dir(), 'filsorOptReport' in dir()]):
-        logger.error('Neither full nor filter & sort opt-analysis report to be generated (whatever format)')
-        sys.exit(2)
+        # c. Load generated HTML report and compare it to reference one
+        with open(workPath / 'valtests-preanalyses-report.html') as file:
+            htmlActRepLines = file.readlines()
 
-    logger.closeOperation(oprText)
+        htmlRefRepLines = htmlRefReportLines_fxt
+        self.compareHtmlReports(htmlRefRepLines, htmlActRepLines)
 
-if not args.realRun and not emptyRun:
-    logger.info('Checks done, seems you can now really run this, through -u / --realrun :-)')
+        # d. No cleanup: let the final cleaning code operate in _inifinalizeClass()
 
-# 15. Done.
-sys.exit(0)
+        # e. Done.
+        logger.info(f'PASS testReports: main, MCDSResultsReport ctor, toExcel, toHtml (command line mode)')
```

### Comparing `pyaudisam-1.0.2/pyaudisam/analyser.py` & `pyaudisam-1.1.0/pyaudisam/analyser.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # If not, see https://www.gnu.org/licenses/.
 
 # Submodule "analyser": Run a bunch of DS analyses according to a user-friendly set of analysis specs
 
 import copy
 import re
 import pathlib as pl
+import shutil
+
 from packaging import version
 
 import numpy as np
 import pandas as pd
 
 from . import log, runtime
 from .data import MonoCategoryDataSet, ResultsSet
@@ -37,15 +39,16 @@
     """
     A result set for multiple analyses from the same engine.
     
     Internal columns index is a 3-level multi-index.
     """
     
     def __init__(self, analysisClass, miCustomCols=None, dfCustomColTrans=None,
-                 dComputedCols=None, dfComputedColTrans=None, sortCols=[], sortAscend=[]):
+                 dComputedCols=None, dfComputedColTrans=None, sortCols=[], sortAscend=[],
+                 dropNACols=True, miExemptNACols=None):
         
         assert issubclass(analysisClass, DSAnalysis), 'analysisClass must derive from DSAnalysis'
         assert miCustomCols is None \
                or (isinstance(miCustomCols, pd.MultiIndex) and len(miCustomCols.levels) == 3), \
                'customCols must be None or a 3 level pd.MultiIndex'
         
         self.analysisClass = analysisClass
@@ -58,43 +61,46 @@
         # DataFrame for translating 3-level multi-index columns to 1 level lang-translated columns
         dfColTrans = pd.concat([self.engineClass.statSampColTrans(), analysisClass.DfRunColumnTrans,
                                 self.engineClass.statModColTrans()])
         
         super().__init__(miCols=miCols, dfColTrans=dfColTrans,
                          miCustomCols=miCustomCols, dfCustomColTrans=dfCustomColTrans,
                          dComputedCols=dComputedCols, dfComputedColTrans=dfComputedColTrans,
-                         sortCols=sortCols, sortAscend=sortAscend)
+                         sortCols=sortCols, sortAscend=sortAscend,
+                         dropNACols=dropNACols, miExemptNACols=miExemptNACols)
     
     def copy(self, withData=True):
     
         """Clone function (shallow), with optional (deep) data copy"""
     
         # 1. Call ctor without computed columns stuff (we no more have initial data)
         clone = AnalysisResultsSet(analysisClass=self.analysisClass,
-                                   miCustomCols=self.miCustomCols, dfCustomColTrans=self.dfCustomColTrans,
-                                   sortCols=[], sortAscend=[])
+                                   miCustomCols=self.miCustomCols.copy(), dfCustomColTrans=self.dfCustomColTrans.copy(),
+                                   dComputedCols=None, dfComputedColTrans=None,
+                                   sortCols=self.sortCols.copy(), sortAscend=self.sortAscend.copy(),
+                                   dropNACols=self.dropNACols, miExemptNACols=self.miExemptNACols.copy())
     
         # 2. Complete clone initialisation.
         # 3-level multi-index columns (module, statistic, figure)
-        clone.miCols = self.miCols
-        clone.computedCols = self.computedCols
+        clone.miCols = self.miCols.copy()
+        clone.computedCols = self.computedCols.copy()
         
         # DataFrames for translating 3-level multi-index columns to 1 level lang-translated columns
-        clone.dfColTrans = self.dfColTrans
+        clone.dfColTrans = self.dfColTrans.copy()
         
         # Copy data if needed.
         if withData:
             clone._dfData = self._dfData.copy()
             clone.rightColOrder = self.rightColOrder
             clone.postComputed = self.postComputed
 
         return clone
                 
 
-class Analyser(object):
+class Analyser:
 
     """Tools for building analysis variants specifications and explicitating them.
     
     Abstract base class for DS analysers.
     """
 
     def __init__(self):
@@ -332,15 +338,15 @@
             
             colSetId = ':'.join(sorted(dfPsValues.columns))
             if colSetId not in dSameColsPsNames:
                 dSameColsPsNames[colSetId] = list()
                 
             dSameColsPsNames[colSetId].append(psName)
 
-        # For each group, concat. tables into one, after expliciting if needed
+        # For each group, concat. tables into one, after explicitating if needed
         ldfExplPartSpecs = list()
 
         for lPsNames in dSameColsPsNames.values():
 
             ldfSameColsPartSpecs = list()
             for psName in lPsNames:
 
@@ -709,30 +715,26 @@
             tplRslt += verdict, reasons
 
         return tplRslt
 
     def shutdown(self):
     
         """Shutdown engine and executor (only useful if run() raises an exception and so fails to do it),
-        but keep the remainder of the object state as is.
+        but keep the remainder of the object state as is: cleanup() not called.
         """
 
         if self._engine:
             self._engine.shutdown()
             self._engine = None
         if self._executor:
             self._executor.shutdown()
             self._executor = None
-        
-#    def __del__(self):
-#    
-#        self.shutdown()
 
 
-class _FilterSortSteps(object):
+class _FilterSortSteps:
 
     """Log = history of filter and sort steps for a given scheme"""
 
     def __init__(self, filSorSchId, resultsSet, lang):
         self.schemeId = filSorSchId
         self.lang = lang
         self.results = resultsSet  # only for resultsSet.transColumn(...)
@@ -757,15 +759,15 @@
             propValue = self.transColumns(propValue)
         self.steps.append([stepName, propName, propValue])
 
     def toList(self):
         return [[self.schemeId] + step for step in self.steps]
 
 
-class _FilterSortCache(object):
+class _FilterSortCache:
 
     def __init__(self):
         self.dResults = dict()
 
     def copy(self):
         clone = _FilterSortCache()
         clone.dResults = {schId: (iFilSor.copy(), filSorSteps.copy())
@@ -784,15 +786,15 @@
             # return a detached copy.
             iFilSor, filSorSteps = self.dResults[schemeId]
             logger.info1(f'Filter and sort scheme "{schemeId}" found in cache.')
             return iFilSor.copy(), filSorSteps.copy()
         return None, None
 
 
-class FilterSortSchemeIdManager(object):
+class FilterSortSchemeIdManager:
 
     """Filter and sort scheme Id generator"""
 
     # Constants for schemeId()
     MainSchSpecNames = ['method', 'deduplicate', 'filterSort',
                         'preselCols', 'preselAscs', 'preselThrhs', 'preselNum']
 
@@ -824,15 +826,15 @@
 
     def schemeId(self, scheme):
 
         """Human-readable but unique identification of a filter and sort scheme
 
         Built on the scheme name format and an additional int suffix when needed.
 
-        Definition: 2 equal schemes (dict ==) have the same Id
+        By definition: 2 equal schemes (dict ==) have the same Id
 
         Parameters:
         :param scheme: the scheme to identify
                        as a dict(method= filterSortOnXXX method to use,
                                  deduplicate= dict(dupSubset=, dDupRounds=) of deduplication params
                                      (if not or partially given, see filterSortOnXXX defaults)
                                  filterSort= dict of other <method> params (see filterSortOnXXX methods),
@@ -849,25 +851,25 @@
 
         :return: the unique Id.
         """
 
         # Check scheme specification (1st level properties: presence of mandatory ones, authorised list, ...)
         props = scheme.keys()
         assert all(prop in self.MainSchSpecNames for prop in props), \
-               'Unknown filter and sort scheme property/ies: {}' \
-                .format(', '.join(prop for prop in props if prop not in self.MainSchSpecNames))
+               'Unknown filter and sort scheme property/ies: ' \
+               + ', '.join(prop for prop in props if prop not in self.MainSchSpecNames)
         mandProps = ['method']
         assert all(prop in props for prop in mandProps), \
-               'Missing filter and sort scheme mandatory property/ies: {}' \
-                .format(', '.join(prop for prop in mandProps if prop not in props))
+               'Missing filter and sort scheme mandatory property/ies: ' \
+               + ', '.join(prop for prop in mandProps if prop not in props)
         method = scheme['method']
         assert callable(method), 'Filter and sort scheme method must be callable'
         assert method is MCDSAnalysisResultsSet.filterSortOnExecCode \
                or method is MCDSAnalysisResultsSet.filterSortOnExCAicMulQua, \
-               'Unsupported filter and sort scheme method: ' + str(method)
+               f'Unsupported filter and sort scheme method: {method}'
 
         # Compute the heading "name" part of the Id
         schemeId = 'ExCode' if method is MCDSAnalysisResultsSet.filterSortOnExecCode else 'ExAicMQua'
         methArgs = scheme.get('filterSort', {})
         if 'sightRate' in methArgs:
             schemeId += '-r{:.1f}'.format(methArgs['sightRate']).replace('.', '')
         if 'whichBestQua' in methArgs:
@@ -985,19 +987,29 @@
     CLGblOrdQuaChi2 = (CLCAutoFilSor, 'Bal. quality Chi2+ (global)', CLTSortOrder)
     CLGblOrdQuaKS = (CLCAutoFilSor, 'Bal. quality KS+ (global)', CLTSortOrder)
     CLGblOrdQuaDCv = (CLCAutoFilSor, 'Bal. quality DCv+ (global)', CLTSortOrder)
 
     CLGblOrdDAicChi2KSDCv = (CLCAutoFilSor, 'DeltaAIC Chi2 KS DCv (global)', CLTSortOrder)
 
     # Computed columns specs (name translation + position).
+    # Note: position is a 0-starting index in the initial (constructor) list of columns of the results set
+    #       (the miCols ctor argument; see DSAnalysisResultsSet above, it's basically the list of columns
+    #        for sample stats, appended with the engine run columns, appended with the full theoretical list
+    #        of columns output by MCDS, even if not all are actually filled for each analysis),
+    #       prepended by the custom columns (miCustomCols ctor arg.),
+    #       possibly appended by unexpected columns appearing in the analyses results as they are run,
+    #       and finally enhanced (through insert(index) or append(=> end)) according to DComputedCols,
+    #       one item by one ; meaning that you can fix a computed column index only once you have fixed
+    #       the index of the previous computed column in DComputedCols !
+    # TODO: Make this awful stuff simpler (using a "before column name" rather a "before column index" ?)
     _firstResColInd = len(MCDSEngine.statSampCols()) + len(MCDSAnalysis.MIRunColumns)
     DComputedCols = {CLSightRate: _firstResColInd + 10,  # After Encounter Rate / Left|Right Trunc. Dist.
                      CLDeltaAic: _firstResColInd + 12,  # Before AIC
                      CLChi2: _firstResColInd + 14,  # Before all Chi2 tests
-                     CLDeltaDCv: _firstResColInd + 72,  # Before Density of animals / Cv
+                     CLDeltaDCv: _firstResColInd + 83,  # Before Density of animals / Cv
                      # And, at the end ...
                      **{cl: -1 for cl in [CLCmbQuaBal1, CLCmbQuaBal2, CLCmbQuaBal3,
                                           CLCmbQuaChi2, CLCmbQuaKS, CLCmbQuaDCv,
                                           CLGroupTruncLeft, CLGroupTruncRight,
                                           CLGrpOrdSmTrAic,
                                           CLGrpOrdClTrChi2KSDCv,  # CLGrpOrdClTrChi2,
                                           CLGrpOrdClTrDCv,
@@ -1042,16 +1054,16 @@
                                    'Ordre Global DeltaAIC Chi2 KS DCv']))
 
     # Final-selection column label (empty, for user decision)
     CLFinalSelection = (CLCAutoFilSor, 'Final selection', 'Value')
     DFinalSelColTrans = dict(fr='Sélection finale', en='Final selection')
 
     def __init__(self, miCustomCols=None, dfCustomColTrans=None, miSampleCols=None, sampleIndCol=None,
-                 sortCols=[], sortAscend=[], distanceUnit='Meter', areaUnit='Hectare',
-                 surveyType='Point', distanceType='Radial', clustering=False,
+                 sortCols=[], sortAscend=[], dropNACols=True, miExemptNACols=None,
+                 distanceUnit='Meter', areaUnit='Hectare', surveyType='Point', distanceType='Radial', clustering=False,
                  ldTruncIntrvSpecs=[dict(col='left', minDist=5.0, maxLen=5.0),
                                     dict(col='right', minDist=25.0, maxLen=25.0)],
                  truncIntrvEpsilon=1e-6, ldFilSorKeySchemes=None):
         
         """Ctor
 
         Parameters:
@@ -1067,15 +1079,16 @@
         assert sampleIndCol is not None
 
         assert all(spec['col'] in self.DCLParTruncDist for spec in ldTruncIntrvSpecs)
 
         # Initialise base.
         super().__init__(MCDSAnalysis, miCustomCols=miCustomCols, dfCustomColTrans=dfCustomColTrans,
                          dComputedCols=self.DComputedCols, dfComputedColTrans=self.DfComputedColTrans,
-                         sortCols=sortCols, sortAscend=sortAscend)
+                         sortCols=sortCols, sortAscend=sortAscend,
+                         dropNACols=dropNACols, miExemptNACols=miExemptNACols)
         
         if self.CLFinalSelection:
             self.addColumnsTrans({self.CLFinalSelection: self.DFinalSelColTrans})
 
         # Sample columns
         self.miSampleCols = miSampleCols if miSampleCols is not None else self.miCustomCols
         self.sampleIndCol = sampleIndCol
@@ -1104,21 +1117,23 @@
         self.filSorCache = _FilterSortCache()
 
     def copy(self, withData=True):
     
         """Clone function, with optional data copy"""
     
         # Create new instance with same ctor params.
-        clone = MCDSAnalysisResultsSet(miCustomCols=self.miCustomCols, dfCustomColTrans=self.dfCustomColTrans,
-                                       miSampleCols=self.miSampleCols, sampleIndCol=self.sampleIndCol,
-                                       sortCols=self.sortCols, sortAscend=self.sortAscend,
+        clone = MCDSAnalysisResultsSet(miCustomCols=self.miCustomCols.copy(),
+                                       dfCustomColTrans=self.dfCustomColTrans.copy(),
+                                       miSampleCols=self.miSampleCols.copy(), sampleIndCol=self.sampleIndCol,
+                                       sortCols=self.sortCols.copy(), sortAscend=self.sortAscend.copy(),
+                                       dropNACols=self.dropNACols, miExemptNACols=self.miExemptNACols.copy(),
                                        distanceUnit=self.distanceUnit, areaUnit=self.areaUnit,
                                        surveyType=self.surveyType, distanceType=self.distanceType,
                                        clustering=self.clustering,
-                                       ldTruncIntrvSpecs=self.ldTruncIntrvSpecs,
+                                       ldTruncIntrvSpecs=self.ldTruncIntrvSpecs.copy(),
                                        truncIntrvEpsilon=self.truncIntrvEpsilon)
 
         # Copy data if needed.
         if withData:
             clone._dfData = self._dfData.copy()
             clone.rightColOrder = self.rightColOrder
             clone.postComputed = self.postComputed
@@ -2380,14 +2395,23 @@
                 self.ParmMinDist: sAnIntSpec.get(self.IntSpecMinDist, self.defMinDist),
                 self.ParmMaxDist: sAnIntSpec.get(self.IntSpecMaxDist, self.defMaxDist),
                 self.ParmFitDistCuts: sAnIntSpec.get(self.IntSpecFitDistCuts, self.defFitDistCuts),
                 self.ParmDiscrDistCuts: sAnIntSpec.get(self.IntSpecDiscrDistCuts, self.defDiscrDistCuts)}
 
     DAnlr2ResChapName = dict(before='header (head)', sample='header (sample)', after='header (tail)')
 
+    MIAllParmResultsCols = pd.MultiIndex.from_tuples([MCDSAnalysisResultsSet.CLParEstKeyFn,
+                                                      MCDSAnalysisResultsSet.CLParEstAdjSer,
+                                                      MCDSAnalysisResultsSet.CLParEstSelCrit,
+                                                      MCDSAnalysisResultsSet.CLParEstCVInt,
+                                                      MCDSAnalysisResultsSet.CLParTruncLeft,
+                                                      MCDSAnalysisResultsSet.CLParTruncRight,
+                                                      MCDSAnalysisResultsSet.CLParModFitDistCuts,
+                                                      MCDSAnalysisResultsSet.CLParModDiscrDistCuts])
+
     def prepareResultsColumns(self):
         
         # a. Sample multi-index columns
         sampleSelCols = self.resultsHeadCols['sample']
         sampMCols = [(self.DAnlr2ResChapName['sample'], col, 'Value') for col in sampleSelCols]
         miSampCols = pd.MultiIndex.from_tuples(sampMCols)
 
@@ -2404,38 +2428,42 @@
 
         # c. Translation for it (well, no translation actually ... only one language forced for all !)
         dfCustColTrans = pd.DataFrame(index=miCustCols, data={lang: customCols for lang in ['fr', 'en']})
 
         # d. The 3-columns index for the sample index column
         sampIndMCol = (self.DAnlr2ResChapName[self.sampIndResHChap], self.sampleIndCol, 'Value')
 
-        # e. And finally, the result object (sorted at the end by the analysis or else sample index column)
+        # e. The result column to sort the result table at the end by (ascending).
         if self.anlysIndCol or self.sampleIndCol:
             sortCols = [next(mCol for mCol in custMCols if mCol[1] == self.anlysIndCol or self.sampleIndCol)]
         else:
             sortCols = []
         sortAscend = [True] * len(sortCols)
 
-        return miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend
+        # f. The result analysis parameter columns to keep at the end (if present) even if all empty
+        miExemptNACols = self.MIAllParmResultsCols
+
+        return miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend, miExemptNACols
 
     def setupResults(self, ldFilSorKeySchemes=None):
     
         """Build an empty results objects.
 
         Parameters:
         :param ldFilSorKeySchemes: Replacement for MCDSAnalysisResultsSet predefined filter-sort key schemes
                                    None => use predefined ones MCDSAnalysisResultsSet.AutoFilSorKeySchemes.
         """
-    
-        miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend = \
+
+        miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend, miExemptNACols = \
             self.prepareResultsColumns()
-        
+
         return MCDSAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
                                       miSampleCols=miSampCols, sampleIndCol=sampIndMCol,
                                       sortCols=sortCols, sortAscend=sortAscend,
+                                      dropNACols=True, miExemptNACols=miExemptNACols,
                                       distanceUnit=self.distanceUnit, areaUnit=self.areaUnit,
                                       surveyType=self.surveyType, distanceType=self.distanceType,
                                       clustering=self.clustering,
                                       ldTruncIntrvSpecs=self.ldTruncIntrvSpecs,
                                       truncIntrvEpsilon=self.truncIntrvEpsilon,
                                       ldFilSorKeySchemes=ldFilSorKeySchemes)
     
@@ -2569,30 +2597,64 @@
                                  runtime=pd.Series(runtime, name='Version'))
         
         # Done.
         logger.info(f'Analyses completed ({len(self.results)} results).')
 
         return self.results
 
+    def cleanup(self):
+        
+        """Cleanup analyser:
+        * remove analysis folders if any run,
+        * reset results set,
+        * don't remove any other file (like those produced with the results set toXxx methods)"""
+        
+        if not self.results:
+            logger.info('Nothing to cleanup: no result available')
+            return
+
+        logger.info(f'Removing analysis folders ...')
+        nRemvd = 0
+        for anlysFolder in self.results.dfData[self.results.CLRunFolder]:
+            logger.info1(f'* {anlysFolder}')
+            dpn = pl.Path(anlysFolder)
+            if dpn.is_dir():
+                shutil.rmtree(dpn)
+                nRemvd += 1
+        logger.info(f'... done ({nRemvd}/{len(self.results)} removed).')
+
+        # Done.
+        self.results = None
+
 
 class MCDSPreAnalysisResultsSet(MCDSAnalysisResultsSet):
 
     """A specialized results set for MCDS pre-analyses
     (simpler post-computations that base class MCDSAnalysisResultsSet)
 
     TODO: Should obviously rather be the base class for MCDSAnalysisResultsSet !
     """
     
     # Computed columns specs (name translation + position).
+    # Note: position is a 0-starting index in the initial (constructor) list of columns of the results set
+    #       (the miCols ctor argument; see DSAnalysisResultsSet above, it's basically the list of columns
+    #        for sample stats, appended with the engine run columns, appended with the full theoretical list
+    #        of columns output by MCDS, even if not all are actually filled for each analysis),
+    #       prepended by the custom columns (miCustomCols ctor arg.),
+    #       possibly appended by unexpected columns appearing in the analyses results as they are run,
+    #       and finally enhanced (through insert(index) or append(=> end)) according to DComputedCols,
+    #       one item by one ; meaning that you can fix a computed column index only once you have fixed
+    #       the index of the previous computed column in DComputedCols !
+    # TODO: Make this awful stuff simpler (using a "before column name" rather a "before column index" ?)
     Super = MCDSAnalysisResultsSet
     _firstResColInd = len(MCDSEngine.statSampCols()) + len(MCDSAnalysis.MIRunColumns)
     DComputedCols = {Super.CLSightRate: _firstResColInd + 10,  # After Encounter Rate / Left|Right Trunc. Dist.
                      Super.CLDeltaAic: _firstResColInd + 12,  # Before AIC
                      Super.CLChi2: _firstResColInd + 14,  # Before all Chi2 tests
-                     Super.CLDeltaDCv: _firstResColInd + 72,  # Before Density of animals / Cv
+                     Super.CLDeltaDCv: _firstResColInd + 83,  # Before Density of animals / Cv
                      # And, at the end ...
                      **{cl: -1 for cl in [Super.CLCmbQuaBal1, Super.CLCmbQuaBal2, Super.CLCmbQuaBal3,
                                           Super.CLCmbQuaChi2, Super.CLCmbQuaKS, Super.CLCmbQuaDCv]}}
 
     DfComputedColTrans = \
         pd.DataFrame(index=DComputedCols.keys(),
                      data=dict(en=['Obs Rate', 'Delta AIC', 'Chi2 P', 'Delta CoefVar Density',
@@ -2602,37 +2664,40 @@
                                    'Qual Equi 1', 'Qual Equi 2', 'Qual Equi 3',
                                    'Qual Chi2+', 'Qual KS+', 'Qual DCv+']))
 
     # Needed presence in base class, but use inhibited.
     CLFinalSelection = None
 
     def __init__(self, miCustomCols=None, dfCustomColTrans=None, miSampleCols=None, sampleIndCol=None,
-                 sortCols=[], sortAscend=[], distanceUnit='Meter', areaUnit='Hectare',
-                 surveyType='Point', distanceType='Radial', clustering=False):
+                 sortCols=[], sortAscend=[], dropNACols=True, miExemptNACols=None,
+                 distanceUnit='Meter', areaUnit='Hectare', surveyType='Point', distanceType='Radial', clustering=False):
         
         """
         Parameters:
         :param miSampleCols: columns to use for grouping by sample ; defaults to miCustomCols if None
         :param sampleIndCol: multi-column index for the sample Id column ; no default, must be there !
         """
 
         # Initialise base.
         super().__init__(miCustomCols=miCustomCols, dfCustomColTrans=dfCustomColTrans,
                          miSampleCols=miSampleCols, sampleIndCol=sampleIndCol,
                          sortCols=sortCols, sortAscend=sortAscend,
+                         dropNACols=dropNACols, miExemptNACols=miExemptNACols,
                          distanceUnit=distanceUnit, areaUnit=areaUnit,
                          surveyType=surveyType, distanceType=distanceType, clustering=clustering)
 
     def copy(self, withData=True):
         """Clone function, with optional data copy"""
 
         # Create new instance with same ctor params.
-        clone = MCDSPreAnalysisResultsSet(miCustomCols=self.miCustomCols, dfCustomColTrans=self.dfCustomColTrans,
-                                          miSampleCols=self.miSampleCols, sampleIndCol=self.sampleIndCol,
-                                          sortCols=self.sortCols, sortAscend=self.sortAscend,
+        clone = MCDSPreAnalysisResultsSet(miCustomCols=self.miCustomCols.copy(),
+                                          dfCustomColTrans=self.dfCustomColTrans.copy(),
+                                          miSampleCols=self.miSampleCols.copy(), sampleIndCol=self.sampleIndCol,
+                                          sortCols=self.sortCols.copy(), sortAscend=self.sortAscend.copy(),
+                                          dropNACols=self.dropNACols, miExemptNACols=self.miExemptNACols.copy(),
                                           distanceUnit=self.distanceUnit, areaUnit=self.areaUnit,
                                           surveyType=self.surveyType, distanceType=self.distanceType,
                                           clustering=self.clustering)
 
         # Copy data if needed.
         if withData:
             clone._dfData = self._dfData.copy()
@@ -2684,16 +2749,31 @@
                          resultsHeadCols=resultsHeadCols, anlysIndCol=None, 
                          workDir=workDir, runMethod=runMethod, runTimeOut=runTimeOut, logData=logData,
                          logProgressEvery=logProgressEvery)
 
         assert runTimeOut is None or runMethod != 'os.system', \
                f"Can't care about {runTimeOut}s execution time limit with os.system run method (not implemented)"
 
+        # Set of file (names) exported to self.workDir (for later cleanup)
+        self.workDirExportedFiles = set()
+
     def computeSampleStats(self, implSampleSpecs, sampleDistCol='Distance'):
 
+        """Compute simple statistics for specified samples
+
+        Parameters:
+        :param implSampleSpecs: Implicit sample specs, suitable for explicitation
+          through explicitVariantSpecs
+        :param sampleDistCol: Name of the distance column in samples
+
+        Returns: DataFrame of stats:
+        * index: sample num. Id,
+        * columns: explicitated sample spec. columns + ['Distance Min', 'Distance Max', 'NTot Obs']
+        """
+
         dfExplSampleSpecs = self.explicitParamSpecs(implParamSpecs=implSampleSpecs, dropDupes=True)[0]
 
         lSampleStats = []
         for sampInd, sSampSpec in dfExplSampleSpecs.iterrows():
 
             # Select data sample to process
             sds = self._mcDataSet.sampleDataSet(sSampSpec[self.sampleSelCols])
@@ -2712,20 +2792,21 @@
         return dfSampleStats
 
     def setupResults(self):
     
         """Build an empty results objects.
         """
     
-        miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend = \
+        miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend, miExemptNACols = \
             self.prepareResultsColumns()
         
         return MCDSPreAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
                                          miSampleCols=miSampCols, sampleIndCol=sampIndMCol,
                                          sortCols=sortCols, sortAscend=sortAscend,
+                                         dropNACols=True, miExemptNACols=miExemptNACols,
                                          distanceUnit=self.distanceUnit, areaUnit=self.areaUnit,
                                          surveyType=self.surveyType, distanceType=self.distanceType,
                                          clustering=self.clustering)
     
     def run(self, dfExplSampleSpecs=None, implSampleSpecs=None, dModelStrategy=ModelStrategyDef, threads=None):
     
         """Run specified analyses
@@ -2781,15 +2862,15 @@
 
             # Pre-analysis object
             anlys = MCDSPreAnalysis(engine=self._engine, executor=self._executor,
                                     sampleDataSet=sds, name=sSampSpec[self.abbrevCol],
                                     customData=sSampSpec[customCols].copy(),
                                     logData=False, modelStrategy=dModelStrategy)
 
-            # Start running pre-analysis in parallel, but don't wait for it's finished, go on
+            # Start running pre-analysis in parallel, but don't wait for it's finished: go on
             anlysFut = anlys.submit()
             
             # Store pre-analysis object and associated "future" for later use (should be running sooner or later).
             dAnlyses[anlysFut] = anlys
             
             # Next analysis (loop).
 
@@ -2803,24 +2884,25 @@
                                  analyser=self.flatSpecs(), runtime=pd.Series(runtime, name='Version'))
         
         # Done.
         logger.info('Analyses completed.')
 
         return self.results
 
-    def exportDSInputData(self, dfExplSampleSpecs=None, implSampleSpecs=None, format='Distance'):
+    def exportDSInputData(self, dfExplSampleSpecs=None, implSampleSpecs=None, format='Distance', targetFolder=None):
     
         """Export specified data samples to the specified DS input format, for "manual" DS analyses
         
         Parameters:
         :param dfExplSampleSpecs: Explicit sample specs, as a DataFrame
           (generated through explicitVariantSpecs, as an example),
         :param implSampleSpecs: Implicit sample specs, suitable for explicitation
           through explicitVariantSpecs
         :param format: output files format, only 'Distance' supported for the moment.
+        :param targetFolder: output folder for exported files (str or Path) ; self.workDir if None.
         """
     
         assert format == 'Distance', 'Only Distance format supported for the moment'
     
         # MCDS analysis engine
         self._engine = MCDSEngine(workDir=self.workDir, runMethod=self.runMethod, timeOut=self.runTimeOut,
                                   distanceUnit=self.distanceUnit, areaUnit=self.areaUnit,
@@ -2828,31 +2910,65 @@
                                   clustering=self.clustering)
 
         # Explicitate and complete analysis specs, and check for usability
         # (should be also done before calling run, to avoid failure).
         dfExplSampleSpecs, _, _, _, checkVerdict, checkErrors = \
             self.explicitParamSpecs(implSampleSpecs, dfExplSampleSpecs, dropDupes=True, check=True)
         assert checkVerdict, 'Sample specs check failed: {}'.format('; '.join(checkErrors))
-        
+
+        # Export folder.
+        toWorkDir = False
+        if not targetFolder:
+            toWorkDir = True
+            targetFolder = self.workDir
+        targetFolder = pl.Path(targetFolder)
+
         # For each sample to export:
-        logger.info('Exporting {} samples to {} format ...'.format(len(dfExplSampleSpecs), format))
-        logger.debug(dfExplSampleSpecs)
+        logger.info(f'Exporting {len(dfExplSampleSpecs)} samples to {targetFolder.as_posix()} ({format} format) ...')
+        logger.debug('Sample specs:\n'+ dfExplSampleSpecs.to_string())
 
         for sampInd, sSampSpec in dfExplSampleSpecs.iterrows():
             
             # Selection des données
             sds = self._mcDataSet.sampleDataSet(sSampSpec[self.sampleSelCols])
             if not sds:
                 logger.warning('#{}/{} => No data in {} sample, no file exported'
                                .format(sampInd+1, len(dfExplSampleSpecs), sSampSpec[self.abbrevCol]))
                 continue
 
             # Export to Distance
-            fpn = pl.Path(self.workDir) / '{}-dist.txt'.format(sSampSpec[self.abbrevCol])
+            fpn = targetFolder / '{}-dist.txt'.format(sSampSpec[self.abbrevCol])
             fpn = self._engine.buildDistanceDataFile(sds, tgtFilePathName=fpn)
+            if toWorkDir:
+                self.workDirExportedFiles.add(fpn.name)
 
             logger.info1('#{}/{} => {}'.format(sampInd+1, len(dfExplSampleSpecs), fpn.name))
 
         # Done.
         self._engine.shutdown()
 
         logger.info(f'Done exporting.')
+
+    def cleanup(self):
+
+        """Cleanup pre-analyser:
+        * remove analysis folders if any run,
+        * reset results set,
+        * remove Distance-format files exported in self.workDir
+          (but neither those exported elsewhere, nor those produced with the results set toXxx methods)"""
+        
+        super().cleanup()
+        
+        logger.info(f'Removing files exported in workDir ({len(self.workDirExportedFiles)} expected) ...')
+        nRemvd = 0
+        if self.workDirExportedFiles:
+            workDir = pl.Path(self.workDir)
+            for fileName in self.workDirExportedFiles:
+                logger.info1(f'* {fileName}')
+                fpn = workDir / fileName
+                if fpn.isfile():
+                    fpn.unlink()
+                    nRemvd += 1
+        logger.info(f'... done ({nRemvd}/{len(self.workDirExportedFiles)} removed).')
+
+        # Done.
+        self.workDirExportedFiles.clear()
```

### Comparing `pyaudisam-1.0.2/pyaudisam/analysis.py` & `pyaudisam-1.1.0/pyaudisam/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from .engine import DSEngine, MCDSEngine
 from .executor import Executor
 
 logger = log.logger('ads.ans')
 
 
 # Analysis (abstract) : Gather input params, data set, results, debug and log files
-class DSAnalysis(object):
+class DSAnalysis:
     
     EngineClass = DSEngine
     
     # Run columns for output : root engine output (3-level multi-index)
     CLRunStatus = ('run output', 'run status', 'Value')
     CLRunStartTime = ('run output', 'start time', 'Value')
     CLRunElapsedTime = ('run output', 'elapsed time', 'Value')
@@ -180,19 +180,17 @@
     CLParEstSelCrit = ('parameters', 'estimator selection criterion', 'Value')
     CLParEstCVInt = ('parameters', 'CV interval', 'Value')
     CLParTruncLeft = ('parameters', 'left truncation distance', 'Value')
     CLParTruncRight = ('parameters', 'right truncation distance', 'Value')
     CLParModFitDistCuts = ('parameters', 'model fitting distance cut points', 'Value')
     CLParModDiscrDistCuts = ('parameters', 'distance discretisation cut points', 'Value')
 
-    MIRunColumns = pd.MultiIndex.from_tuples([CLParEstKeyFn, CLParEstAdjSer,
-                                              CLParEstSelCrit, CLParEstCVInt,
-                                              CLParTruncLeft, CLParTruncRight,
-                                              CLParModFitDistCuts, CLParModDiscrDistCuts]
-                                             + DSAnalysis.RunRunColumns)
+    RunParColumns = [CLParEstKeyFn, CLParEstAdjSer, CLParEstSelCrit, CLParEstCVInt,
+                     CLParTruncLeft, CLParTruncRight, CLParModFitDistCuts, CLParModDiscrDistCuts]
+    MIRunColumns = pd.MultiIndex.from_tuples(RunParColumns + DSAnalysis.RunRunColumns)
     
     # DataFrame for translating 3-level multi-index columns to 1 level lang-translated columns
     DfRunColumnTrans = \
         pd.DataFrame(index=MIRunColumns,
                      data=dict(en=['Mod Key Fn', 'Mod Adj Ser', 'Mod Chc Crit', 'Conf Interv',
                                    'Left Trunc Dist', 'Right Trunc Dist', 'Fit Dist Cuts', 'Discr Dist Cuts']
                                   + DSAnalysis.DRunRunColumnTrans['en'],
```

### Comparing `pyaudisam-1.0.2/pyaudisam/data.py` & `pyaudisam-1.1.0/pyaudisam/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # PyAuDiSam: Automation of Distance Sampling analyses with Distance software (http://distancesampling.org/)
 
-# Copyright (C) 2021 Jean-Philippe Meuret
+# Copyright (C) 2021 Jean-Philippe Meuret, Sylvain Sainnier
 
 # This program is free software: you can redistribute it and/or modify it under the terms
 # of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
@@ -28,15 +28,15 @@
 from . import log, runtime
 
 runtime.update(numpy=np.__version__, pandas=pd.__version__)
 
 logger = log.logger('ads.dat')
 
 
-class DataSet(object):
+class DataSet:
 
     """A tabular data set built by concatenating various-formatted source tables into one.
     
     Note: visionat module also defines this class: no reason it differs in any way => synchronise please !
           Why ? Just to keep the 2 modules independent ; might change in the future"""
     
     def __init__(self, sources, dRenameCols={}, dComputeCols={}, importDecFields=[],
@@ -380,29 +380,30 @@
         else:
             hValue = str(value)
         
         return hValue
     
     @classmethod
     def compareDataFrames(cls, dfLeft, dfRight, subsetCols=[], indexCols=[],
-                          dropCloser=np.inf, dropNans=True, dropCloserCols=False):
+                          noneIsNan=False, dropCloser=np.inf, dropNans=True, dropCloserCols=False):
     
         """
         Compare 2 DataFrames.
 
         The resulting diagnosis DataFrame will have the same columns and merged index,
         with a "closeness" value for each cell (see _closeness method) ;
         rows where all cells have closeness > dropCloser (or eventually NaN) are yet dropped.
         and columns where all cells have closeness > dropCloser (or eventually NaN) can also be dropped.
         
         Parameters:
         :param dfLeft: Left DataFrame
         :param dfRight: Right DataFrame
         :param list subsetCols: on a subset of columns,
         :param list indexCols: ignoring these columns, but keeping them as the index and sorting order,
+        :param bool noneIsNan: if True, replace any None by a np.nan in left and right before comparing
         :param float dropCloser: result will only include rows with all cell closeness > dropCloser
                                  (default: np.inf => all cols and rows kept).
         :param bool dropNans: smoother condition for dropCloser : if True, NaN values are also considered > dropCloser
                               ('cause NaN != NaN :-( ).
         :param bool dropCloserCols: if True, also drop all "> dropCloser (or eventually NaN)"-all-cell columns,
                                     just as rows
 
@@ -417,17 +418,17 @@
         dfRight = dfRight.copy()
         
         # Check input columns
         dColsSets = {'Subset column': subsetCols, 'Index column': indexCols}
         for colsSetName, colsSet in dColsSets.items():
             for col in colsSet:
                 if col not in dfLeft.columns:
-                    raise KeyError('{} {} not in left result set'.format(colsSetName, col))
+                    raise KeyError(f'{colsSetName} {col} not in left result set')
                 if col not in dfRight.columns:
-                    raise KeyError('{} {} not in right result set'.format(colsSetName, col))
+                    raise KeyError(f'{colsSetName} {col} not in right result set')
         
         # Set specified cols as the index (after making them hashable) and sort it.
         dfLeft[indexCols] = dfLeft[indexCols].applymap(cls._toHashable)
         dfLeft.set_index(indexCols, inplace=True)
         dfLeft = dfLeft.sort_index()  # Not inplace: don't modify a copy/slice
 
         dfRight[indexCols] = dfRight[indexCols].applymap(cls._toHashable)
@@ -442,25 +443,32 @@
         # Append mutually missing rows to the 2 tables => a complete and identical index.
         anyCol = dfLeft.columns[0]  # Need one, whichever.
         dfLeft = dfLeft.join(dfRight[[anyCol]], rsuffix='_r', how='outer')
         dfLeft.drop(columns=dfLeft.columns[-1], inplace=True)
         dfRight = dfRight.join(dfLeft[[anyCol]], rsuffix='_l', how='outer')
         dfRight.drop(columns=dfRight.columns[-1], inplace=True)
 
-        # Compare : Compute closeness 
+        # Replace None by NaNs if specified
+        if noneIsNan:
+            dfLeft.replace({None: np.nan}, inplace=True)
+            dfRight.replace({None: np.nan}, inplace=True)
+
+        # Compare : Compute closeness
         nColLevels = dfLeft.columns.nlevels
         KRightCol = 'tmp' if nColLevels == 1 else tuple('tmp{}'.format(i) for i in range(nColLevels))
         dfRelDiff = dfLeft.copy()
         exception = False
         for leftCol in dfLeft.columns:
             dfRelDiff[KRightCol] = dfRight[leftCol]
             try:
                 dfRelDiff[leftCol] = dfRelDiff[[leftCol, KRightCol]].apply(cls._closeness, axis='columns')
             except TypeError as exc:
-                logger.error(f'Column {leftCol} : {exc}')
+                logger.error(f'_closeness failed for left column {leftCol}: {exc} ...')
+                logger.error(f'* left: {dfRelDiff[leftCol].to_dict()}')
+                logger.error(f'* right: {dfRelDiff[KRightCol].to_dict()}')
                 exception = True
             dfRelDiff.drop(columns=[KRightCol], inplace=True)
             
         if exception:
             raise TypeError('Stopping: Some columns could not be compared (see errors logged above)')
             
         # Complete comparison : rows with index not in both frames forced to all-0 closeness
@@ -474,41 +482,43 @@
         if dropCloserCols:
             # dfRelDiff.drop(columns=dfRelDiff.T[dfCells2Drop.all(axis='index')].index, axis='index', inplace=True)
             dfRelDiff.drop(columns=[col for col, drop in dfCells2Drop.all(axis='index').items() if drop],
                            inplace=True)  # 40% faster.
             
         return dfRelDiff
 
-    def compare(self, other, subsetCols=[], indexCols=[], dropCloser=np.inf, dropNans=True, dropCloserCols=False):
+    def compare(self, other, subsetCols=[], indexCols=[],
+                noneIsNan=False, dropCloser=np.inf, dropNans=True, dropCloserCols=False):
     
         """
         Compare 2 data sets.
         
         The resulting diagnosis DataFrame will have the same columns and merged index,
         with a "closeness" value for each cell (see _closeness method) ;
         rows where all cells have closeness > dropCloser (or eventually NaN) are yet dropped.
         and columns where all cells have closeness > dropCloser (or eventually NaN) can also be dropped.
         
         Parameters:
         :param other: Right data set or DataFrame object to compare
         :param list subsetCols: on a subset of columns,
         :param list indexCols: ignoring these columns, but keeping them as the index and sorting order,
+        :param bool noneIsNan: if True, replace any None by a np.nan in left and right before comparing
         :param float dropCloser: result will only include rows with all cell closeness > dropCloser
                                  (default: np.inf => all cols and rows kept).
         :param bool dropNans: smoother condition for dropCloser : if True, NaN values are also considered > dropCloser
                               ('cause NaN != NaN :-( ).
         :param bool dropCloserCols: if True, also drop all "> dropCloser (or eventually NaN)" columns-all-cell,
                                     just as rows
 
         :return: the diagnostic DataFrame.
         """
         
         return self.compareDataFrames(dfLeft=self.dfData,
                                       dfRight=other if isinstance(other, pd.DataFrame) else other.dfData,
-                                      subsetCols=subsetCols, indexCols=indexCols,
+                                      subsetCols=subsetCols, indexCols=indexCols, noneIsNan=noneIsNan,
                                       dropCloser=dropCloser, dropNans=dropNans, dropCloserCols=dropCloserCols)
 
 
 class FieldDataSet(DataSet):
 
     """A tabular data set for producing mono-category or even individuals data sets from "raw sightings data",
     aka "field data" (with possibly multiple category counts on each row)
@@ -878,30 +888,31 @@
 
         # Report some basic stats.
         nAbscRows = self._dfData.isna().any(axis='columns').sum()
         logger.info('Sample data : {} sightings = {} individuals + {} absence rows'
                     .format(len(self), len(self) - nAbscRows, nAbscRows))
 
 
-class ResultsSet(object):
+class ResultsSet:
     
     """
     A tabular result set for some computation process repeated multiple times with different input / results,
     each process result(s) being given as a pd.Series (1 row for the target table) or a pd.DataFrame (multiple rows).
     
     With ability to prepend custom heading columns to each process results ones
     (same value for each 1-process results rows).
     
     The columns of the internal pd.DataFrame, like those of each process result(s), can be a multi-index.
     
     Support for column translation is included (a mono-indexed).
     """
 
     def __init__(self, miCols, dfColTrans=None, miCustomCols=None, dfCustomColTrans=None,
-                 dComputedCols=None, dfComputedColTrans=None, sortCols=[], sortAscend=[], dropNACols=True):
+                 dComputedCols=None, dfComputedColTrans=None, sortCols=[], sortAscend=[],
+                 dropNACols=True, miExemptNACols=None):
     
         """Ctor
         
         Parameters:
         :param miCols: process results columns (MultiIndex or not)
         :param dfColTrans: translation DataFrame for results column labels,
                            * index=column labels,
@@ -909,48 +920,50 @@
         :param miCustomCols: custom columns to prepend (on the left) to process results columns (MultiIndex or not)
         :param dfCustomColTrans: translation DataFrame for custom column labels,
         :param dComputedCols: dict(label: position) for inserting computed columns in results table (None = after end)
         :param dfComputedColTrans: translation DataFrame for computed column labels,
         :param sortCols: if not empty, iterable of columns to sort values by in dfData()
         :param sortAscend: sorting order for all (bool), or each column (iterable of bool) in dfData()
         :param dropNACols: If True, dfData() won't return columns with no relevant results data
-                           (except for custom cols).
+                           (except for custom cols and exempt cols).
+        :param miExemptNACols: if not None, non-custom columns to keep even if
+        dropNACols and all NaN
         """
         
         assert len(sortCols) == len(sortAscend), 'sortCols and sortAscend must have same length'
 
         # Columns stuff.
         if dComputedCols is None:
             dComputedCols = dict()
             dfComputedColTrans = pd.DataFrame()
 
-        # Columns : Process results + computed results (at the specified position if any)
+        # Columns: Process results + computed results (at the specified position if any)
         self.miCols = miCols.copy()
+        self.isMultiIndexedCols = isinstance(miCols, pd.MultiIndex)
         for col, ind in dComputedCols.items():
             if ind is not None:
                 self.miCols = self.miCols.insert(ind, col)
         lastCompCols = [col for col, ind in dComputedCols.items() if ind is None]
         if lastCompCols:
             self.miCols = self.miCols.append(pd.MultiIndex.from_tuples(lastCompCols))
 
-        # 
+        # Columns: post-computed ones, and custom ones (to prepend to process results)
         self.computedCols = list(dComputedCols.keys())
         self.miCustomCols = miCustomCols.copy() if miCustomCols is not None else list()
-        
-        self.isMultiIndexedCols = isinstance(miCols, pd.MultiIndex)
 
         # DataFrames for translating 3-level multi-index columns to 1 level lang-translated columns
         self.dfColTrans = pd.concat([dfColTrans if dfColTrans is not None else pd.DataFrame(),
-                                     dfComputedColTrans if dfColTrans is not None else pd.DataFrame()])
+                                     dfComputedColTrans if dfComputedColTrans is not None else pd.DataFrame()])
         self.dfCustomColTrans = dfCustomColTrans.copy() if dfCustomColTrans is not None else pd.DataFrame()
         
         # Sorting and cleaning parameters (after postComputing)
         self.sortCols = sortCols
         self.sortAscend = sortAscend
         self.dropNACols = dropNACols
+        self.miExemptNACols = miExemptNACols
         
         # Non-constant data members
         self._dfData = pd.DataFrame()  # The real data (frame).
         self.rightColOrder = False  # self._dfData columns are assumed to be in a wrong order.
         self.postComputed = False  # Post-computation not yet done.
     
         # Specifications of computations that led to the results
@@ -963,15 +976,15 @@
     @property
     def empty(self):
         
         return self._dfData.empty
 
     @property
     def columns(self):
-    
+        # Yes, using dfData triggers post-computation, we mean it !
         return self.dfData.columns
         
     @property
     def index(self):
         
         return self._dfData.index
 
@@ -988,15 +1001,16 @@
     
         """Clone function (shallow), with optional (deep) data copy"""
 
         # 1. Call ctor without computed columns stuff for now and here (we no more have initial data)
         clone = ResultsSet(miCols=self.miCols,
                            miCustomCols=self.miCustomCols.copy(),
                            dfCustomColTrans=self.dfCustomColTrans.copy(),
-                           sortCols=self.sortCols.copy(), sortAscend=self.sortAscend.copy())
+                           sortCols=self.sortCols.copy(), sortAscend=self.sortAscend.copy(),
+                           dropNACols=self.dropNACols, miExemptNACols=self.miExemptNACols.copy())
     
         # 2. Complete clone initialisation.
         clone.miCols = self.miCols.copy()
         clone.computedCols = self.computedCols.copy()
         
         # DataFrames for translating 3-level multi-index columns to 1 level lang-translated columns
         clone.dfColTrans = self.dfColTrans.copy()
@@ -1138,28 +1152,35 @@
                 if self.isMultiIndexedCols:
                     miTgtColumns = self.miCustomCols.append(miTgtColumns)
                 else:
                     miTgtColumns = self.miCustomCols + miTgtColumns
             self._dfData = self._dfData.reindex(columns=miTgtColumns)
             self.rightColOrder = True  # No need to do it again, until next append() !
         
-        # This is also documentation line !
+        # These are also documentation lines !
         if self.isMultiIndexedCols and not self._dfData.empty:
             assert isinstance(self._dfData.columns, pd.MultiIndex)
         
-        # If specified, don't return columns with no relevant results data (unless among custom cols).
+        # If specified, don't return columns with no relevant results data,
+        # unless among custom cols or explicitly exempt cols.
         if self.dropNACols and not self._dfData.empty:
             miCols2Cleanup = self._dfData.columns
-            if self.miCustomCols is not None:
-                if self.isMultiIndexedCols:
+            if self.isMultiIndexedCols:
+                if self.miCustomCols is not None:
                     miCols2Cleanup = miCols2Cleanup.drop(self.miCustomCols.to_list())
-                else:
+                if self.miExemptNACols is not None:
+                    miCols2Cleanup = miCols2Cleanup.drop(self.miExemptNACols.to_list())
+            else:
+                if self.miCustomCols is not None:
                     miCols2Cleanup = [col for col in miCols2Cleanup if col not in self.miCustomCols]
+                if self.miExemptNACols is not None:
+                    miCols2Cleanup = [col for col in miCols2Cleanup if col not in
+                                      self.miExemptNACols]
             cols2Drop = [col for col in miCols2Cleanup if self._dfData[col].isna().all()]
-            logger.debug(f'Dropping all-NaN columns {cols2Drop}')
+            logger.debug(f'Dropping all-NaN result columns {cols2Drop}')
             self._dfData.drop(columns=cols2Drop, inplace=True)
 
         # Done.
         return self._dfData.copy() if copy else self._dfData
 
     @property
     def dfData(self):
@@ -1283,17 +1304,17 @@
         Parameters:
         :param lang: target language for translation ('en' or 'fr')
         :param index: rows to select, as a list(int) or pd.Index (subset of self.dfData.index) ; None = all rows.
         :param columns: columns to select, as a list(string) or pd.Index when mono-indexed columns
                        or as a list(tuple(string*)) or pd.MultiIndex when multi-indexed ; None = all columns.
         """
 
-        assert lang in ['en', 'fr'], 'No support for "{}" language'.format(lang)
+        assert lang in ['en', 'fr'], f'No support for "{lang}" language'
         
-        # Extract (and maybe copy) selected rows and columns of dfData.
+        # Extract selected rows and columns of dfData.
         dfTrData = self.dfSubData(index=index, columns=columns, copy=True)
         
         # Translate column names.
         dfTrData.columns = self.transColumns(dfTrData.columns, lang)
         
         return dfTrData
 
@@ -1343,15 +1364,15 @@
         logger.info('{}x{} results rows x columns and {} specs saved to {} in {:.3f}s'
                     .format(len(dfOutData), len(dfOutData.columns),
                             len(self.specs) if specs else 'no', fileName,
                             (pd.Timestamp.now() - start).total_seconds()))
 
     def specs2Tables(self):
 
-        """Transform specs to tables
+        """Transform specs into tables
 
         :return: dict(name=DataFrame)
         """
         ddfSpecs = dict()
 
         for spName, spData in self.specs.items():
             if isinstance(spData, (dict, list, pd.Series)):
@@ -1599,15 +1620,15 @@
                        specs=specs, specSheetsPrfx=specSheetsPrfx, postComputed=postComputed,
                        acceptNewCols=acceptNewCols, dDefMissingCols=dDefMissingCols)
 
     def fromFile(self, fileName, sheetName=None, header=[0, 1, 2], skipRows=[3], indexCol=0,
                  specs=True, specSheetsPrfx='sp-', postComputed=False,
                  acceptNewCols=False, dDefMissingCols=dict()):
         
-        """Load (overwrite) data data and eventually specs from a given file,
+        """Load (overwrite) data and eventually specs from a given file,
         (supported formats are .pickle, .pickle.xz, .ods, .xlsx, .xls, auto-detected from file name)
         assuming ctor params match with the results object used to generate source file,
         which can well be ensured by using the same ctor params as used for saving !
         Notes: Needs odfpy module and pandas.version >= 0.25.1
 
         Parameters:
         :param fileName: source file name
@@ -1635,40 +1656,42 @@
         elif fpn.suffix in ['.xls', '.xlsx']:
             self.fromExcel(fileName, sheetName=sheetName, header=header, skipRows=skipRows,
                            indexCol=indexCol, specs=specs, specSheetsPrfx=specSheetsPrfx, postComputed=postComputed,
                            acceptNewCols=acceptNewCols, dDefMissingCols=dDefMissingCols)
         else:
             raise NotImplementedError(f'Unsupported ResultsSet input file format: {fileName}')
 
-    def compare(self, other, subsetCols=[], indexCols=[], dropCloser=np.inf, dropNans=True, dropCloserCols=False):
+    def compare(self, other, subsetCols=[], indexCols=[],
+                noneIsNan=False, dropCloser=np.inf, dropNans=True, dropCloserCols=False):
     
         """
         Compare 2 results sets.
         
         The resulting diagnosis DataFrame will have the same columns and merged index,
         with a "closeness" value for each cell (see _closeness method) ;
         rows where all cells have closeness > dropCloser (or eventually NaN) are yet dropped.
         and columns where all cells have closeness > dropCloser (or eventually NaN) can also be dropped.
         
         Parameters:
         :param other: Right results or DataFrame object to compare
         :param list subsetCols: on a subset of columns,
         :param list indexCols: ignoring these columns, but keeping them as the index and sorting order,
+        :param bool noneIsNan: if True, replace any None by a np.nan in left and right before comparing
         :param float dropCloser: result will only include rows with all cell closeness > dropCloser
                                  (default: np.inf => all cols and rows kept).
         :param bool dropNans: smoother condition for dropCloser : if True, NaN values are also considered > dropCloser
                               ('cause NaN != NaN :-( ).
         :param bool dropCloserCols: if True, also drop "> dropCloser (or eventually NaN)"-all-cell columns,
                                     just as rows
 
         :return: the diagnostic DataFrame.
         """
         
         return DataSet.compareDataFrames(dfLeft=self.dfData,
                                          dfRight=other if isinstance(other, pd.DataFrame) else other.dfData,
-                                         subsetCols=subsetCols, indexCols=indexCols,
+                                         subsetCols=subsetCols, indexCols=indexCols, noneIsNan=noneIsNan,
                                          dropCloser=dropCloser, dropNans=dropNans, dropCloserCols=dropCloserCols)
         
 
 if __name__ == '__main__':
 
     sys.exit(0)
```

### Comparing `pyaudisam-1.0.2/pyaudisam/engine.py` & `pyaudisam-1.1.0/pyaudisam/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,71 +31,65 @@
 
 from . import log, runtime
 
 logger = log.logger('ads.eng', level=log.INFO)  # Initial config (can be changed later)
 
 from .executor import Executor
 
-# Keep ruin'dows from opening a GPF dialog box every time a launched executable (like MCDS.exe) crashes !
+# Keep Ruin'dows from opening a GPF dialog box every time a launched executable (like MCDS.exe) crashes !
 # BUT: This does NOT work :-(
 if sys.platform.startswith('win'):
     import ctypes
     import msvcrt
     ctypes.windll.kernel32.SetErrorMode(msvcrt.SEM_NOGPFAULTERRORBOX)
 
 # Actual package install dir.
 KInstDirPath = pl.Path(__file__).parent.resolve()
 
 
 # DSEngine (abstract) classes.
 # An engine for running multiple DS analyses with same options (engine ctor params),
 # but various parameters (submitAnalysis() parameters), possibly as parallel threads / processes.
 # Warning: No option change allowed while started analyses are running / all their getResults() have returned.
-class DSEngine(object):
+class DSEngine:
     
     # Possible values for options.
     DistUnits = ['Meter', 'Kilometer', 'Mile', 'Inch', 'Feet', 'Yard', 'Nautical mile']
     AreaUnits = ['Hectare', 'Acre'] + ['Sq. ' + distUnit for distUnit in DistUnits]
     
     # Forbidden chars in workDir path name (Distance DS engines are real red necks)
     # TODO: Stronger protection (more special chars ? more generic method, through re ?)
     ForbidPathChars = [' ', '(', ')', ',']
     
-    # Distance software detection params.
-    DistanceMajorVersions = [7, 6]  # Lastest first.
-    DistanceInstDirNameFmt = 'Distance {majorVersion}'
-    DistancePossInstPaths = map(pl.Path, ['C:/Program files (x86)', 'C:/Program files', 'C:/PortableApps', '.'])
-
-    # Find given executable installation dir.
-    # Note: MCDS.exe is an autonomous executable : simply put it in a "Distance 7" sub-folder
-    #       of this package's one, and it'll work ! Or else install Distance 7 (or later) the normal way :-)
+    # Find executable installation dir.
     @staticmethod
-    def findExecutable(exeFileName):
+    def findExecutable(exeFileName, exeFileSearchPaths):
 
         exeFilePathName = None
-        logger.debug('Looking for {} ...'.format(exeFileName))
-        for ver in DSEngine.DistanceMajorVersions:
-            for path in DSEngine.DistancePossInstPaths:
-                exeFN = path / DSEngine.DistanceInstDirNameFmt.format(majorVersion=ver) / exeFileName
-                if not exeFN.exists():
-                    logger.info2('  Checking {} : No,'.format(exeFN))
-                else:
-                    logger.info('Found {} here: {}.'.format(exeFileName, exeFN))
-                    exeFilePathName = exeFN
-                    break
-            if exeFilePathName:
-                break
+        logger.info(f'Looking for {exeFileName} ...')
+        for path in exeFileSearchPaths:
+            exeFN = path / exeFileName
+            if not exeFN.exists():
+                logger.info(f'* checking {exeFN.as_posix()}: no,')
+                continue
+
+            logger.info(f'Found {exeFileName} here: {exeFN.as_posix()}.')
+            exeFilePathName = exeFN
+            break
 
         if not exeFilePathName:
-            raise Exception('Could not find {} ; please install Distance software (V6 or later)'.format(exeFileName))
+            raise OSError(f'Could not find {exeFileName} ; please install Distance software (V6 or later)')
 
-        runtime.update({'DS engine': exeFilePathName.as_posix()})
-            
         return exeFilePathName
     
+    # Find executable version.
+    @staticmethod
+    def findVersion():
+        raise NotImplementedError('Abstract DSEngine.findVersion method must no be called: see derived classes')
+
     # Specifications of output stats.
     DfStatRowSpecs, DfStatModSpecs, DfStatModNotes, MIStatModCols, DfStatModColTrans = None, None, None, None, None
     
     def __init__(self, workDir='.', executor=None, runMethod='subprocess.run', timeOut=None,
                  distanceUnit='Meter', areaUnit='Hectare', **options):
 
         """Ctor
@@ -219,15 +213,15 @@
     
         self.shutdown()
 
 
 # MCDS engine (Conventional Distance Sampling)
 class MCDSEngine(DSEngine):
     
-    # Possible suervy types and distance types.
+    # Possible survey types and distance types.
     SurveyTypes = ['Point', 'Line']
     DistTypes = ['Radial', 'Perpendicular', 'Radial & Angle']
     
     # First data fields in exports for distance / MCDS importing
     # (N/A ones may get removed before use, according to distance type and clustering options).
     FirstDataFields = {'Point': ['STR_LABEL', 'STR_AREA', 'SMP_LABEL', 'SMP_EFFORT', 'DISTANCE', 'SIZE'],
                        'Line': ['STR_LABEL', 'STR_AREA', 'SMP_LABEL', 'SMP_EFFORT', 'DISTANCE', 'ANGLE', 'SIZE']}
@@ -249,16 +243,25 @@
     
     # Distance truncation / cut points parameters.
     DistMinDef = None  # No left truncation (min = 0)
     DistMaxDef = None  # No right truncation (max = max. distance observed)
     DistFitCutsDef = None  # Model fitting : Automatic engine distance cuts determination.
     DistDiscrCutsDef = None  # Distance values discretisation : None (keep exact values).
 
-    # Executable 
-    ExeFilePathName = DSEngine.findExecutable('MCDS.exe')
+    # MCDS Executable
+    # * MCDS.exe is an autonomous executable: you can put a copy anywhere, or nearly ... see below
+    # * it'll be searched first in the folders (separated by a ;) referenced in the MCDS_PATH env. variable,
+    # * then in a "Distance 7" sub-folder of ., then C:/PortableApps, C:/Program files (x86), C:/Program files,
+    # * then in a "Distance 6" sub-folder of ., then C:/PortableApps, C:/Program files (x86), C:/Program files.
+    # (if you install Distance 7 (or 6, or newer) the normal way, it will then of course be found :-)
+    _ExeFileSearchPaths = [pl.Path(path) for path in os.environ.get('MCDS_PATH', '').split(';') if path] \
+                           + [pl.Path(rootFolder) / f'Distance {majorVersion}'
+                              for majorVersion in [7, 6]  # Latest first.
+                              for rootFolder in ['.', 'C:/PortableApps', 'C:/Program files (x86)', 'C:/Program files']]
+    ExeFilePathName = DSEngine.findExecutable('MCDS.exe', _ExeFileSearchPaths)
 
     # Output stats specs : load from external files (extracts from Distance doc).
     @classmethod
     def loadStatSpecs(cls, nMaxAdjParams=10):
         
         if MCDSEngine.DfStatRowSpecs is not None:
             return
@@ -274,49 +277,58 @@
                             for i in range(0, len(statRowSpecLines)-2, 3)]
             cls.DfStatRowSpecs = pd.DataFrame(columns=['Name', 'Description'],
                                               data=statRowSpecs).set_index('Name')
             assert not cls.DfStatRowSpecs.empty, 'Empty MCDS stats row specs'
         
         # Module and stats number to description table
         fileName = KInstDirPath / 'mcds/stat-mod-specs.txt'
-        logger.debug1('* {}'.format(fileName))
+        logger.debug1('* ' + fileName.as_posix())
         with open(fileName, mode='r', encoding='utf8') as fStatModSpecs:
             statModSpecLines = [line.rstrip('\n') for line in fStatModSpecs.readlines() if not line.startswith('#')]
             reModSpecNumName = re.compile('(.+) – (.+)')
             statModSpecs = list()
             moModule = None
             for line in statModSpecLines:
+                # logger.debug2(line)
                 if not line:
                     continue
                 if moModule is None:
                     moModule = reModSpecNumName.match(line.strip())
                     continue
                 if line == ' ':
                     moModule = None
                     continue
                 moStatistic = reModSpecNumName.match(line.strip())
                 modNum, modDesc, statNum, statDescNotes = \
                     moModule.group(1), moModule.group(2), moStatistic.group(1), moStatistic.group(2)
-                for i in range(len(statDescNotes)-1, -1, -1):
+                for i in range(len(statDescNotes) - 1, -1, -1):
                     if not re.match(r'[\d ,]', statDescNotes[i]):
-                        statDesc = statDescNotes[:i+1]
-                        statNotes = statDescNotes[i+1:].replace(' ', '')
+                        statDesc = statDescNotes[:i + 1]
+                        statNotes = statDescNotes[i + 1:].replace(' ', '')
                         break
                 modNum = int(modNum)
                 if statNum.startswith('101 '):
                     for num in range(nMaxAdjParams):  # Assume no more than that ... a bit hacky !
                         statModSpecs.append((modNum, modDesc, 101+num,  # Make statDesc unique for later indexing
-                                             statDesc.replace('each', 'A({})'.format(num+1)), statNotes))
+                                             statDesc.replace('each', f'A({num+1})'), statNotes))
                 else:
                     statNum = int(statNum)
-                    if modNum == 2 and statNum == 3:  # Actually, there are 0 or 3 of these ...
-                        for num in range(3):
-                            statModSpecs.append((modNum, modDesc, num+201,
-                                                 # Change statNum & Make statDesc unique for later indexing
-                                                 statDesc+' (distance set {})'.format(num+1), statNotes))
+                    if modNum == 2 and statNum in [3, 20, 21, 22]:
+                        if statNum == 3:
+                            # MCDS 6.2: Actually, there are 0 or 3 of these, but anyway ...
+                            for num in range(3):
+                                statModSpecs.append((modNum, modDesc, num + 1 + 200,
+                                                     # Change statNum & Make statDesc unique for later indexing
+                                                     statDesc + f' (distance set {num + 1})', statNotes))
+                        else:
+                            # MCDS 7.4: 20, 21 & 22 are new and undocumented, but assume behaviour same as for 3.
+                            for num in range(3):
+                                statModSpecs.append((modNum, modDesc, num + 1 + 10 * (statNum + 1),
+                                                     # Change statNum & Make statDesc unique for later indexing
+                                                     statDesc + f' (distance set {num + 1})', statNotes))
                     else:
                         statModSpecs.append((modNum, modDesc, statNum, statDesc, statNotes))
             cls.DfStatModSpecs = pd.DataFrame(columns=['modNum', 'modDesc', 'statNum', 'statDesc', 'statNotes'],
                                               data=statModSpecs).set_index(['modNum', 'statNum'])
             assert not cls.DfStatModSpecs.empty, 'Empty MCDS stats module specs'
         
         # Produce a MultiIndex for output stats as columns in the desired order.
@@ -783,44 +795,60 @@
         dfStats.drop(columns=['Stratum', 'Sample', 'Estimator'], inplace=True)
         
         # 3. Stack figure columns to rows, to get more comfortable
         dfStats.set_index(['Module', 'Statistic'], append=True, inplace=True)
         dfStats = dfStats.stack().reset_index()
         dfStats.rename(columns={'level_0': 'id', 'level_3': 'Figure', 0: 'Value'}, inplace=True)
 
-        # 4. Fix multiple Module=2 & Statistic=3 rows (before joining with cls.DfStatModSpecs)
+        # 4. Fix multiple Module=2 & Statistic=3, 20, 21, 22 rows (before joining with cls.DfStatModSpecs)
+        #    => change Statistic column for unicity = instance unambiguous identification
         newStatNum = 200
         for lbl, sRow in dfStats[(dfStats.Module == 2) & (dfStats.Statistic == 3)].iterrows():
-            if dfStats.loc[lbl, 'Figure'] == 'Value':
+            if dfStats.at[lbl, 'Figure'] == 'Value':
                 newStatNum += 1
-            dfStats.loc[lbl, 'Statistic'] = newStatNum
-        
+            dfStats.at[lbl, 'Statistic'] = newStatNum
+        for oldStatNum in [20, 21, 22]:
+            newStatNum = 10 * (oldStatNum + 1)
+            for lbl, sRow in dfStats[(dfStats.Module == 2) & (dfStats.Statistic == oldStatNum)].iterrows():
+                if dfStats.at[lbl, 'Figure'] == 'Value':
+                    newStatNum += 1
+                dfStats.at[lbl, 'Statistic'] = newStatNum
+
         # 5. Add descriptive / naming columns for modules and statistics,
         #    from cls.DfStatModSpecs (more user-friendly than numeric ids + help for detecting N/A figures)
         dfStats = dfStats.join(cls.DfStatModSpecs, on=['Module', 'Statistic'])
         
         # 6. Check that supposed N/A figures (as told by cls.DfStatModSpecs.statNotes) are really such
         #    Warning: There seems to be a bug in MCDS with Module=2 & Statistic=10x : some Cv values not always 0 ...
         sKeepOnlyValueFig = ~dfStats.statNotes.apply(lambda s: pd.notnull(s) and '1' in s)
         sFigs2Drop = (dfStats.Figure != 'Value') & sKeepOnlyValueFig
         assert ~dfStats[sFigs2Drop & ((dfStats.Module != 2) | (dfStats.Statistic < 100))].Value.any(), \
-               'Warning: Some so-called "N/A" figures are not zeroes !'
+               'Error: Some so-called "N/A" stat figures are not zeroes !'
         
         # 7. Remove so-called N/A figures
         dfStats.drop(dfStats[sFigs2Drop].index, inplace=True)
         
         # 8. Make some values more readable.
         lblKeyFn = (dfStats.Module == 2) & (dfStats.Statistic == 13)
         dfStats.loc[lblKeyFn, 'Value'] = \
             dfStats.loc[lblKeyFn, 'Value'].astype(int).apply(lambda n: cls.EstKeyFns[n-1])
         lblAdjFn = (dfStats.Module == 2) & (dfStats.Statistic == 14)
         dfStats.loc[lblAdjFn, 'Value'] = \
             dfStats.loc[lblAdjFn, 'Value'].astype(int).apply(lambda n: cls.EstAdjustFns[n-1])
-        
-        # 9. Final indexing
+
+        # 9. Check if any unexpected module / statistic present, and if so, warn and fix
+        #    (like after MCDS.exe changed version ... as an example)
+        dfUnexptdStats = dfStats[dfStats[['modDesc', 'statDesc']].isnull().any(axis='columns')]
+        if not dfUnexptdStats.empty:
+            logger.warning('Ignoring unexpected modules / stats found in results'
+                           ' from a likely unsupported yet MCDS version'
+                           f'\n{dfUnexptdStats.to_string(min_rows=30, max_rows=30)}')
+            dfStats.drop(dfUnexptdStats.index, inplace=True)
+
+        # 10. Final indexing
         dfStats = dfStats.reindex(columns=['modDesc', 'statDesc', 'Figure', 'Value'])
         dfStats.set_index(['modDesc', 'statDesc', 'Figure'], inplace=True)
 
         # That's all folks !
         logger.debug('Done decoding from {}.'.format(statsFileName))
         
         return dfStats.T.iloc[0]
@@ -930,7 +958,62 @@
         # Export.
         dfExport.to_csv(tgtFilePathName, index=False, sep='\t', encoding='utf-8',
                         header=self.distanceFields(self.options.firstDataFields) + extraFields)
 
         logger.debug('Data Distance-exported to {}.'.format(tgtFilePathName))
         
         return tgtFilePathName
+
+    # Retrieve MCDS.exe version
+    @classmethod
+    def findVersion(cls):
+
+        logger.debug(f'Running {cls.ExeFilePathName} to discover its version ...')
+
+        versionStr = None
+        lastExc = None
+        for tmpDirRoot in [None, '.']:
+            try:
+                # Create an auto-cleanup temporary folder for running MCDS.
+                logger.debug(f'* trying {tmpDirRoot or "default"} root dir for temporary run folder ...')
+                with tempfile.TemporaryDirectory(dir=tmpDirRoot) as tmpDir:
+
+                    if ' ' in tmpDir:
+                        logger.debug(f'  => skipped {tmpDir}: some space(s) in path')
+                        continue  # No space in folder path, MCDS does not support it
+
+                    # Create an engine instance
+                    engine = cls(workDir=tmpDir)
+
+                    # Setup run folder
+                    runPath = engine.setupRunFolder()
+
+                    # Generate command file into this folder
+                    cmdFileName = engine.buildCmdFile(runPath)
+
+                    # Run executable as an OS sub-process.
+                    engine._run(engine.ExeFilePathName, cmdFileName)
+
+                    # Extract and decode results.
+                    with open(runPath / cls.LogFileName) as logFile:
+                        firstLine = logFile.readline().strip()
+                        versionStr = firstLine[len('This is mcds.exe version'):].strip()
+
+                    # Done, with success.
+                    logger.debug(f'Successfully determined MCDS version: {versionStr}')
+                    break
+
+            except OSError as exc:
+                lastExc = str(exc)
+                logger.debug(f'  => exception: {lastExc}')
+
+        if lastExc is not None:
+            logger.warning(f'Failed to determine MCDS version: {lastExc}')
+            logger.warning('Hints: Current folder must be writable and its path must not contain any space !')
+        if versionStr is None:
+            logger.warning('Failed to determine MCDS version: unsupported (new ?) log file format ?')
+
+        return versionStr
+
+
+# Discover and save MCDS engine version (can't do it in the class itself, contrary to ExePathName).
+MCDSEngine.ExeVersion = MCDSEngine.findVersion()
```

### Comparing `pyaudisam-1.0.2/pyaudisam/executor.py` & `pyaudisam-1.1.0/pyaudisam/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import warnings
 
 from . import log
 
 logger = log.logger('ads.exr')
 
 
-class ImmediateFuture(object):
+class ImmediateFuture:
     
     """Synchronous concurrent.futures.Future minimal and trivial implementation,
        for use with SequentialExecutor
     """
 
     def __init__(self, result):
         
@@ -78,15 +78,15 @@
         return map(func, *iterables)  # Do it now !
     
     def shutdown(self, wait=True):
         
         pass
         
         
-class Executor(object):
+class Executor:
 
     """Wrapper class for simpler concurrent.futures.Executor interface,
        and access to added non-parallel SequentialExecutor
     """
 
     # The only SequentialExecutor (only one needed)
     TheSeqExor = None
```

### Comparing `pyaudisam-1.0.2/pyaudisam/log.py` & `pyaudisam-1.1.0/pyaudisam/log.py`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/anlys.htpl` & `pyaudisam-1.1.0/pyaudisam/mcds/anlys.htpl`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 <head>
 
   <meta charset="utf-8"/>
   <meta name="author" content="Jean-Philippe Meuret"/>
   <meta name="copyright" content="Jean-Philippe Meuret 2021"/>
   <meta name="license" content="CC BY NC SA"/>
   <meta name="description" content="{{title}}"/>
-  <meta name="keywords" content="distance, sampling, mcds, {{keywords}}"/>
+  <meta name="keywords" content="distance, sampling, mcds, report, {{keywords}}"/>
   <meta name="datetime" content="{{genDateTime}}"/>
   
   <title>{{title}}</title>
   
   <link rel="stylesheet" media="screen" type="text/css" href="../report.css"/>
   
   <script>
```

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/fulltop.htpl` & `pyaudisam-1.1.0/pyaudisam/mcds/fulltop.htpl`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 <head>
 
   <meta charset="utf-8"/>
   <meta name="author" content="Jean-Philippe Meuret"/>
   <meta name="copyright" content="Jean-Philippe Meuret 2021"/>
   <meta name="license" content="CC BY NC SA"/>
   <meta name="description" content="{{title}}"/>
-  <meta name="keywords" content="distance, sampling, mcds, full, {{keywords}}"/>
+  <meta name="keywords" content="distance, sampling, mcds, full, report, {{keywords}}"/>
   <meta name="datetime" content="{{genDateTime}}"/>
   
   <title>{{title}}</title>
   
   <link rel="stylesheet" media="screen" type="text/css" href="./report.css"/>
   
   <script>
```

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/pretop.htpl` & `pyaudisam-1.1.0/pyaudisam/mcds/pretop.htpl`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 <head>
 
   <meta charset="utf-8"/>
   <meta name="author" content="Jean-Philippe Meuret"/>
   <meta name="copyright" content="Jean-Philippe Meuret 2021"/>
   <meta name="license" content="CC BY NC SA"/>
   <meta name="description" content="{{title}}"/>
-  <meta name="keywords" content="distance, sampling, mcds, pre-analysis, {{keywords}}"/>
+  <meta name="keywords" content="distance, sampling, mcds, report, {{keywords}}"/>
   <meta name="datetime" content="{{genDateTime}}"/>
   
   <title>{{title}}</title>
   
   <link rel="stylesheet" media="screen" type="text/css" href="./report.css"/>
   
   <script>
```

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/stat-mod-notes.txt` & `pyaudisam-1.1.0/pyaudisam/mcds/stat-mod-notes.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/stat-mod-specs.txt` & `pyaudisam-1.1.0/pyaudisam/mcds/stat-mod-specs.old.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/stat-mod-trans.txt` & `pyaudisam-1.1.0/pyaudisam/mcds/stat-mod-trans.txt`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,25 @@
 detection probability	Cramér-von Mises (uniform weighting) test probability	Value	CvM Uw P	CvM Uw P
 detection probability	Cramér-von Mises (cosine weighting) test probability	Value	CvM Cw P	CvM Cw P
 detection probability	key function type	Value	Key Fn	Fn Clé
 detection probability	adjustment series type	Value	Adj Ser	Sér Ajust
 detection probability	number of key function parameters (NKP)	Value	NumPars KeyFn	NbPars FnClé
 detection probability	number of adjustment term parameters (NAP)	Value	NumPars AdjSer	NbPars SérAjust
 detection probability	number of covariate parameters (NCP)	Value	Num Covars	Nb Covars
+detection probability	undocumented #18 stat	Value	SansDoc #18	NoDoc #18
+detection probability	undocumented #19 stat	Value	SansDoc #19	NoDoc #19
+detection probability	undocumented #20 stat (distance set 1)	Value	SansDoc #20 1	NoDoc #20 1
+detection probability	undocumented #20 stat (distance set 2)	Value	SansDoc #20 2	NoDoc #20 2
+detection probability	undocumented #20 stat (distance set 3)	Value	SansDoc #20 3	NoDoc #20 3
+detection probability	undocumented #21 stat (distance set 1)	Value	SansDoc #21 1	NoDoc #21 1
+detection probability	undocumented #21 stat (distance set 2)	Value	SansDoc #21 2	NoDoc #21 2
+detection probability	undocumented #21 stat (distance set 3)	Value	SansDoc #21 3	NoDoc #21 3
+detection probability	undocumented #22 stat (distance set 1)	Value	SansDoc #22 1	NoDoc #22 1
+detection probability	undocumented #22 stat (distance set 2)	Value	SansDoc #22 2	NoDoc #22 2
+detection probability	undocumented #22 stat (distance set 3)	Value	SansDoc #22 3	NoDoc #22 3
 detection probability	estimated value of A(1) adjustment term parameter	Value	EstA(1)	EstA(1)
 detection probability	estimated value of A(2) adjustment term parameter	Value	EstA(2)	EstA(2)
 detection probability	estimated value of A(3) adjustment term parameter	Value	EstA(3)	EstA(3)
 detection probability	estimated value of A(4) adjustment term parameter	Value	EstA(4)	EstA(4)
 detection probability	estimated value of A(5) adjustment term parameter	Value	EstA(5)	EstA(5)
 detection probability	estimated value of A(6) adjustment term parameter	Value	EstA(6)	EstA(6)
 detection probability	estimated value of A(7) adjustment term parameter	Value	EstA(7)	EstA(7)
```

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/stat-row-specs.txt` & `pyaudisam-1.1.0/pyaudisam/mcds/stat-row-specs.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/mcds/top.htpl` & `pyaudisam-1.1.0/pyaudisam/mcds/top.htpl`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 <head>
 
   <meta charset="utf-8"/>
   <meta name="author" content="Jean-Philippe Meuret"/>
   <meta name="copyright" content="Jean-Philippe Meuret 2021"/>
   <meta name="license" content="CC BY NC SA"/>
   <meta name="description" content="{{title}}"/>
-  <meta name="keywords" content="distance, sampling, mcds, {{keywords}}"/>
+  <meta name="keywords" content="distance, sampling, mcds, report, {{keywords}}"/>
   <meta name="datetime" content="{{genDateTime}}"/>
   
   <title>{{title}}</title>
   
   <link rel="stylesheet" media="screen" type="text/css" href="./report.css"/>
   
   <script>
```

### Comparing `pyaudisam-1.0.2/pyaudisam/optanalyser.py` & `pyaudisam-1.1.0/pyaudisam/optanalyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     Super = MCDSAnalysisResultsSet
 
     # Name of the spec. column to hold the "is truncation stuff optimised" 0/1 flag.
     OptimTruncFlagCol = 'OptimTrunc'
     CLOptimTruncFlag = ('header (tail)', OptimTruncFlagCol, 'Value')
     
     def __init__(self, miCustomCols=None, dfCustomColTrans=None, miSampleCols=None, sampleIndCol=None,
-                 sortCols=[], sortAscend=[], distanceUnit='Meter', areaUnit='Hectare',
-                 surveyType='Point', distanceType='Radial', clustering=False,
+                 sortCols=[], sortAscend=[], dropNACols=True, miExemptNACols=None,
+                 distanceUnit='Meter', areaUnit='Hectare', surveyType='Point', distanceType='Radial', clustering=False,
                  ldTruncIntrvSpecs=[dict(col='left', minDist=5.0, maxLen=5.0),
                                     dict(col='right', minDist=25.0, maxLen=25.0)],
                  truncIntrvEpsilon=1e-6, ldFilSorKeySchemes=None):
         
         """Ctor
 
         Parameters:
@@ -55,33 +55,36 @@
         :param sampleIndCol: multi-column index for the sample Id column ; no default, must be there !
         :param ldFilSorKeySchemes: Replacement for predefined filter-sort key schemes
                                    None => use predefined ones AutoFilSorKeySchemes.
         """
 
         super().__init__(miCustomCols=miCustomCols, dfCustomColTrans=dfCustomColTrans,
                          miSampleCols=miSampleCols, sampleIndCol=sampleIndCol,
-                         sortCols=sortCols, sortAscend=sortAscend, distanceUnit=distanceUnit, areaUnit=areaUnit,
+                         sortCols=sortCols, sortAscend=sortAscend, dropNACols=dropNACols, miExemptNACols=miExemptNACols,
+                         distanceUnit=distanceUnit, areaUnit=areaUnit,
                          surveyType=surveyType, distanceType=distanceType, clustering=clustering,
                          ldTruncIntrvSpecs=ldTruncIntrvSpecs, truncIntrvEpsilon=truncIntrvEpsilon,
                          ldFilSorKeySchemes=ldFilSorKeySchemes)
 
         assert self.CLOptimTruncFlag in self.miCustomCols
 
     def copy(self, withData=True):
     
         """Clone function, with optional data copy"""
     
         # Create new instance with same ctor params.
-        clone = MCDSTruncOptanalysisResultsSet(miCustomCols=self.miCustomCols, dfCustomColTrans=self.dfCustomColTrans,
-                                               miSampleCols=self.miSampleCols, sampleIndCol=self.sampleIndCol,
-                                               sortCols=self.sortCols, sortAscend=self.sortAscend,
+        clone = MCDSTruncOptanalysisResultsSet(miCustomCols=self.miCustomCols,
+                                               dfCustomColTrans=self.dfCustomColTrans.copy(),
+                                               miSampleCols=self.miSampleCols.copy(), sampleIndCol=self.sampleIndCol,
+                                               sortCols=self.sortCols.copy(), sortAscend=self.sortAscend.copy(),
+                                               dropNACols=self.dropNACols, miExemptNACols=self.miExemptNACols.copy(),
                                                distanceUnit=self.distanceUnit, areaUnit=self.areaUnit,
                                                surveyType=self.surveyType, distanceType=self.distanceType,
                                                clustering=self.clustering,
-                                               ldTruncIntrvSpecs=self.ldTruncIntrvSpecs,
+                                               ldTruncIntrvSpecs=self.ldTruncIntrvSpecs.copy(),
                                                truncIntrvEpsilon=self.truncIntrvEpsilon)
 
         # Copy data if needed.
         if withData:
             clone._dfData = self._dfData.copy()
             clone.rightColOrder = self.rightColOrder
             clone.postComputed = self.postComputed
@@ -489,20 +492,21 @@
         """Build an empty results objects.
 
         Parameters:
         :param ldFilSorKeySchemes: Replacement for MCDSTruncOptanalysisResultsSet predefined filter-sort key schemes
                                    None => use predefined ones MCDSTruncOptanalysisResultsSet.AutoFilSorKeySchemes.
         """
 
-        miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend = \
+        miCustCols, dfCustColTrans, miSampCols, sampIndMCol, sortCols, sortAscend, miExemptNACols = \
             self.prepareResultsColumns()
 
         return MCDSTruncOptanalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
                                               miSampleCols=miSampCols, sampleIndCol=sampIndMCol,
                                               sortCols=sortCols, sortAscend=sortAscend,
+                                              dropNACols=True, miExemptNACols=miExemptNACols,
                                               distanceUnit=self.distanceUnit, areaUnit=self.areaUnit,
                                               surveyType=self.surveyType, distanceType=self.distanceType,
                                               clustering=self.clustering,
                                               ldTruncIntrvSpecs=self.ldTruncIntrvSpecs,
                                               truncIntrvEpsilon=self.truncIntrvEpsilon,
                                               ldFilSorKeySchemes=ldFilSorKeySchemes)
```

### Comparing `pyaudisam-1.0.2/pyaudisam/optimisation.py` & `pyaudisam-1.1.0/pyaudisam/optimisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .analyser import MCDSAnalysisResultsSet
 
 runtime.update({'zoopt': pkgrsc.get_distribution('zoopt').version})
 
 logger = log.logger('ads.opn')
 
 
-class Interval(object):
+class Interval:
 
     """A basic closed interval class for numbers"""
     
     def __init__(self, min=0, max=-1):
     
         """Ctor
         
@@ -81,21 +81,27 @@
         
         if maxRange[0] is not None and self.max < maxRange[0]:
             errors.append(f'max:{self.max} < {maxRange[0]}')
         if maxRange[1] is not None and self.max > maxRange[1]:
             errors.append(f'max:{self.max} > {maxRange[1]}')
         
         return ', '.join(errors)
-        
+
+    def __eq__(self, right):
+
+        if not isinstance(right, Interval):
+            right = Interval(right)
+        return self.min == right.min and self.max == right.max
+
     def __repr__(self):
-    
-        return '[{}, {}]'.format(self.min, self.max)
-        
 
-class Error(object):
+        return f'[{self.min}, {self.max}]'
+
+
+class Error:
 
     """Error class for shipping error messages to the end user"""
 
     def __init__(self, error=None, head=''):
         
         """Ctor
         
@@ -140,15 +146,15 @@
         return ' & '.join(msgs)
         
     def __bool__(self):
     
         return any(err for err in self.errors)
 
 
-class DSOptimisation(object):
+class DSOptimisation:
     
     """DSOptimisation (abstract) : A distance sampling analysis optimisation
          possibly run in parallel with others, through an asynchronous "submit then getResults" scheme.
     """
     
     def __init__(self, engine, sampleDataSet, name=None,
                  executor=None, customData=None, error=None,
```

### Comparing `pyaudisam-1.0.2/pyaudisam/optimiser.py` & `pyaudisam-1.1.0/pyaudisam/optimiser.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     
         """The names of the columns holding the real optimisation results
         """
     
         return [col for col in self.optimisationClass.SolutionDimensionNames if col in self.columns]
 
 
-class DSParamsOptimiser(object):
+class DSParamsOptimiser:
 
     """Run a bunch of DS analyses on samples extracted from a mono-category sightings data set,
        according to a user-friendly set of analysis specs (first set of fixed params),
        in order to determine best values for a second set of analysis params.
        Abstract class.
     """
 
@@ -288,15 +288,15 @@
          IntSpecOptimisationCore: [r'opt[a-z]*[\.\-_ ]*core', r'mot[a-z]*[\.\-_ ]*opt',
                                    r'noy[a-z]*[\.\-_ ]*opt'],
          IntSpecSubmitParams:     [r'sub[a-z]*[\.\-_ ]*par', r'par[a-z]*[\.\-_ ]*sou',
                                    r'run[a-z]*[\.\-_ ]*par', r'par[a-z]*[\.\-_ ]*ex',
                                    r'mul[a-z]*[\.\-_ ]*opt', r'opt[a-z]*[\.\-_ ]*mul']}
 
     # Types for user specs parsing (see usage below)
-    class Auto(object):
+    class Auto:
 
         def __repr__(self):
             return 'Auto()'
 
         def __eq__(self, other):
             return isinstance(other, self.__class__)
```

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-arrow-left-hover.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-arrow-left-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-arrow-left.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-arrow-left.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-arrow-right-hover.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-arrow-right-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-arrow-right.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-arrow-right.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-arrow-up-hover.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-arrow-up-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-arrow-up.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-feather-alt.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-feather-alt.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-file-excel-hover.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-file-excel-hover.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/fa-file-excel.svg` & `pyaudisam-1.1.0/pyaudisam/report/fa-file-excel.svg`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report/report.css` & `pyaudisam-1.1.0/pyaudisam/report/report.css`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam/report.py` & `pyaudisam-1.1.0/pyaudisam/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -2020,28 +2020,26 @@
 
                 # Apply it
                 filSorSchId, dfFilSorRes, filSorSteps = \
                     self.resultsSet.dfFilSorData(scheme=scheme, rebuild=rebuild,
                                                  columns=self.synthCols, lang=self.lang)
 
                 # Store results in workbook
-                ddfWbk['-'.join([self.tr('AFSM'), filSorSchId])] = (dfFilSorRes, False)
+                ddfWbk[self.tr('AFSM') + '-' + filSorSchId] = (dfFilSorRes, False)
 
                 # Update all-scheme log
                 repLog += filSorSteps
 
             # Log of opérations, for traceability.
             logger.info1('* filter & sort steps ...')
 
-            indexCols = [self.tr(col) for col in ['Scheme', 'Step']]
-            dataCols = [self.tr(col) for col in ['Property', 'Value']]
-            dfFilSorHist = pd.DataFrame(repLog, columns=indexCols + dataCols)
-            dfFilSorHist.set_index(indexCols, inplace=True)
+            repTransCols = [self.tr(col) for col in ['Scheme', 'Step', 'Property', 'Value']]
+            dfFilSorHist = pd.DataFrame(repLog, columns=repTransCols)
 
-            ddfWbk['-'.join([self.tr('AFS'), self.tr('Steps')])] = (dfFilSorHist, True)
+            ddfWbk[self.tr('AFS') + '-' + self.tr('Steps')] = (dfFilSorHist, True)
 
         # Append inherited worksheets.
         ddfWbk.update(super().asWorkbook(subset=subset, rebuild=rebuild))
 
         # Done
         logger.info('... done.')
```

### Comparing `pyaudisam-1.0.2/pyaudisam/utils.py` & `pyaudisam-1.1.0/pyaudisam/utils.py`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/pyaudisam.egg-info/PKG-INFO` & `pyaudisam-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,151 +1,189 @@
 Metadata-Version: 2.1
 Name: pyaudisam
-Version: 1.0.2
-Summary: Distance Sampling automation through python and Distance sofware
+Version: 1.1.0
+Summary: Distance Sampling automation through python and Distance software
 Home-page: https://github.com/denmedius/pyaudisam
 Author: denmedius
 Author-email: fefeqe22.vucuqu82@murena.io
 License: GPLv3+
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Win32 (MS Windows)
-Requires-Python: >=3.8
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy<1.25,>=1.16
 Requires-Dist: pandas<1.3,>=0.25
 Requires-Dist: openpyxl<3.2,>=3
 Requires-Dist: xlrd~=2.0
 Requires-Dist: matplotlib<3.8,>=3.1
 Requires-Dist: jinja2<3.2,>=2.10
 Requires-Dist: zoopt==0.4.0
 Requires-Dist: packaging
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
-# Python module for AUtomated DIstance SAMpling analyses
+# PYthon module for AUtomated DIstance SAMpling analyses
 
 This module interfaces **distance sampling** analysis engines from [Distance software](https://distancesampling.org/), and possibly others in the future ; thus, it has been designed in order to make it easier :
 * to run (in parallel) numerous [Distance Sampling](https://en.wikipedia.org/wiki/Distance_sampling) analyses with many (many) parameter variants on many field observation samples
   (possibly using some optimisation techniques for automated computation of right and left distance truncations),
 * to select the best analysis variant results through a mostly automated process, based on customisable statistical
   quality indicators,
 * to produce partly customisable reports in spreadsheet (numerical results only) and HTML formats
   (more complete, with full-featured plots like in Distance, and more).
 
-As for now, only the Windows MCDS.exe V6 engine and Point Transect analyses are supported, and so, it runs only under Windows.
+As for now, only the Windows MCDS.exe 6.x (Distance 6 to 7.3) and 7.4 (Distance 7.4 and 7.5 at least) engine and Point Transect analyses are supported, and so, it runs only under Windows.
 
 ## Requirements
 
 The module itself was actually tested extensively with:
 * python 3.8 only
 * pandas 0.25 to 1.2.5
 * openpyxl 3.0 to 3.1.2
 * matplotlib 3.1 to 3.7
 * jinja2 2.10 to 3.1
 * zoopt 0.4.0
 * xlrd 2.0 (only for .xls format support)
 
-You will get no support outside of this (but porting to python 3.12 is planned for 2024).
+You will get no support outside of this (but porting to python 3.12 & pandas 2.x is planned for 2024 or 2025).
 
 As for testing:
 * pytest, pytest-cov
 * plotly (sometimes)
-* xlrd >= 2 (only for old .xls format support)
 
 ## Installation
 
 You can install **pyaudisam** from [PyPI](https://pypi.org/project/pyaudisam/) in your current python environment (conda or venv, whatever):
 
-`$ pip install pyaudisam`
-
-TODO: Publish also on [Conda Forge](https://conda-forge.org/), probably following [this recipe](https://jacobtomlinson.dev/posts/2020/publishing-open-source-python-packages-on-github-pypi-and-conda-forge/#conda-forge).  
+`pip install pyaudisam`
 
 Or from a downloaded source package:
 
-`$ pip install pyaudisam-1.0.2.tar.gz`
+`pip install pyaudisam-1.1.0.tar.gz`
 
 Or from a downloaded wheel package:
 
-`$ pip install pyaudisam-1.0.2-py3-none-any.whl`
+`pip install pyaudisam-1.1.0-py3-none-any.whl`
 
 Or even directly from GitHub:
 
-* `$ pip install git+https://github.com/pypa/sampleproject.git@1.0.2`
-* `$ pip install git+https://github.com/pypa/sampleproject.git@main`
+* `pip install git+https://github.com/pypa/sampleproject.git@1.1.0`
+* `pip install git+https://github.com/pypa/sampleproject.git@main`
 
 ## Usage
 
 As a **python package**, pyaudisam can be used through its python API.
 
 But there's also a **command-line interface**: try and run it with the -h/--help option.
 
 `python -m pyaudisam --help`
 
-Whichever method, the best way to go is to read the concrete quick-start guide : see [Documentation](#documentation) below.
+Whichever method, the best way to go is to read the concrete quick-start guide : see [Documentation](#documentation) below
+(but be aware that you'll need to install an external Distance Sampling engine, like MCDS, to run analyses with paudisam).
 
 ## Documentation
 
 * a short ["how it works" guide](https://github.com/denmedius/pyaudisam/blob/main/docs/how-it-works/how-it-works-en.md) to understand the basics (also in [French](https://github.com/denmedius/pyaudisam/blob/main/docs/how-it-works/how-it-works-fr.md)),
 * a concrete ["quick-start" guide](https://github.com/denmedius/pyaudisam/blob/main/docs/howto-acdc19-nat/howto.md) with a real life use case and relevant field data to play with,
 * another similar but shorter concrete ["quick-start guide" (in French)](http://jpmeuret.free.fr/ds/acdc19/materiau-public.zip) (command-line only) with the full field data set of the "ACDC 2019" birding study.
 
-Note: You can also get a detailled idea of how to use pyaudisam python API by playing with the fully functional [jupyter](https://jupyter.org/) notebook [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) (see below [Running tests](#running-tests) for how to obtain and run it).
+Note: You can also get a detailed idea of how to use pyaudisam python API by playing with the fully functional [jupyter](https://jupyter.org/) notebook [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) (see below [Running tests](#running-tests) for how to obtain and run it).
+
+## Testing
+
+You first need to clone the [source tree](https://github.com/denmedius/pyaudisam) or download and install a [source package](https://pypi.org/project/pyaudisam/#files): once done, look in the _tests_ sub-folder, everything's inside.
+
+Then, you need to install test dependencies:
+
+`pip install pyaudisam[test]`
 
-TODO:
-* complete the quick start guides above by other small and focused articles to explain some mandatory details:
-  - how to build a sample or analysis specification workbook (see a short draft in [analyser.py:273](https://github.com/denmedius/pyaudisam/blob/main/pyaudisam/analyser.py)),
-  - ...
-* write a technical documentation of the whole module,
-* write a guide for building the module API documentation ([sphinx](https://www.sphinx-doc.org/) should work out of the box as [reStructured text](https://en.wikipedia.org/wiki/ReStructuredText) has been used in docstrings),
+Some tests are fully automated, simply run:
 
-## Running tests
+`pytest`
 
-You first need to clone the [source tree](https://github.com/denmedius/pyaudisam) or download and install a [source package](https://pypi.org/project/pyaudisam/#files): once done, look in the _tests_ sub-folder, everything's inside :
-* some tests are fully automated : after installing pytest, simply run it:
+For code coverage during tests, simply run:
 
-  `pytest`
+`pytest --cov`
 
-* for code corevage during tests, after installing pytest-cov, simply run:
+Or even, if you want an HTML report with annotated code coverage:
 
-  `pytest --cov`
+`pytest --cov --cov-report html`
 
-* some other tests not: they are implemented as [jupyter notebooks](https://jupyter.org/) (see [tests/unintests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/unintests.ipynb) and [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) that you must run step by step, as long as no one has fully automated them :-).
+Note: Some other tests are not yet automated: they are implemented as [jupyter notebooks](https://jupyter.org/) (see [tests/unintests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/unintests.ipynb) and [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) that you must run step by step, as long as no one has fully automated them :-).
 
 ## Building
 
-To build pyaudisam [PyPI](https://pypi.org/project/pyaudisam/) source and binary packages, you first need to clone the [source tree](https://github.com/denmedius/pyaudisam) or download and extract a [source package](https://pypi.org/project/pyaudisam/#files): once done, it's as simple as:
+To build pyaudisam [PyPI](https://pypi.org/project/pyaudisam/) source and binary packages, you need:
+* a source tree (clone the [source tree](https://github.com/denmedius/pyaudisam) or download and extract a [source package](https://pypi.org/project/pyaudisam/#files)),
+* a python environment where pyaudisam works,
+* the `build` module (to install through pip as an example).
+
+Then, it's as simple as:
 
 `python -m build`
 
-Note: Don't care about warnings about pyaudisam.mcds and pyaudisam.report being recognised as importable,
- but being absent from setuptools' packages configuration ... these folders simply contain
- pyaudisam config. and data files, no python code at all.
+You'll get 2 files in the `dist` folder (ex. for version 1.1.0) :
+* the wheel package: `pyaudisam-1.1.0-py3-none-any.whl`
+* the source package: `pyaudisam-1.1.0.tar.gz`
 
 ## Contributing
 
 Merge requests are very welcome !
 
 And if you are lacking ideas, here are some good ones below ;-)
 
 ### To do list
 
-* finish tests automation (move and complete[tests/unintests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/unintests.ipynb) and [tests/valtests.ipynb](https://github.com/denmedius/pyaudisam/blob/main/tests/valtests.ipynb) notebooks code to pytest scripts, after checking the state of this work in progress in tests/\*\_test.py scripts),
-* make pyaudisam work under Linux / Mac OS (all python: OK, but calling MCDS.exe):
-  - or: through some kind of external client-server interface to MCDS.exe (that runs only under Windows),
-  - or: by porting MCDS to Linux (closed Fortran source, but old, so might be obtained through a polite request to [this Distance Sampling forum](https://groups.google.com/g/distance-sampling) ; BUT, needs an IMSL license, which is horribly expensive).
-  - or: by rewriting MCDS from scratch, or by porting the [MRDS Distance package](https://distancesampling.org/) to Python,
-  - or: by rewriting MCDS using the [MRDS Distance package](https://distancesampling.org/), meaning some kind of interface to R,
-* build a GUI for pyaudisam command-line (with some kind of "project" concept, and parameter set template, and ...),
-* add support for line transects (only point transects for the moment),
-* add support for the co-variates feature of MCDS,
+* documentation:
+  * complete the quick start guides above by other small and focused articles to explain some mandatory details:
+    * how to build a sample or analysis specification workbook (see a short draft in [analyser.py:273](https://github.com/denmedius/pyaudisam/blob/main/pyaudisam/analyser.py)),
+    * ...
+  * write a technical documentation of the whole module and sub-modules,
+  * write a guide for building the module API documentation ([sphinx](https://www.sphinx-doc.org/) should work out of the box as [reStructured text](https://en.wikipedia.org/wiki/ReStructuredText) has been used in docstrings),
+* code quality and tests:
+  * add more tests for improving code coverage (thanks to HTML coverage report),
+  * configure and run pylint, and follow its useful advices, 
+  * main: split \_Application.\_run in feature sub-functions for clarity,
+* features:
+  * add support for line transects (only point transects for the moment),
+  * add support for the co-variates feature of MCDS,
+  * integrate the notebook prototype of "final reports" (workbook, HTML, and OpenDoc text formats) to automate most of the work of producing a publication-grade "full results appendix" for a Distance Sampling study (based on the auto-filtered report, but with semi-automated diagnosis at sample and analysis level in order to help in the final choice for each sample),
+  * add more features for selecting sample data before running analyses (to avoid the need of creating multiple data sets, run multiple analysis sessions, and then re-aggregate results and reports manually): exclude some specific transects, pre-truncate data above some fixed distance, ...
+* packaging:
+  * publish also pyaudisam on [Conda Forge](https://conda-forge.org/), probably following [this recipe](https://jacobtomlinson.dev/posts/2020/publishing-open-source-python-packages-on-github-pypi-and-conda-forge/#conda-forge),
+* platform support:
+  * add support for newer Python versions (probably 3.12 now) and updated pandas (2+) and zoopt dependencies,
+  * make pyaudisam work under Linux / macOS (all python: OK, but ... calling MCDS.exe, that runs exclusively under Windows):
+    * or: through some kind of external client-server interface to MCDS.exe (that runs only under Windows),
+    * or: by porting MCDS to Linux (closed Fortran source, but old, so might be obtained through a polite request to [this Distance Sampling forum](https://groups.google.com/g/distance-sampling) ;
+      BUT, you'll need an IMSL license, which is horribly expensive).
+    * or: by rewriting MCDS from scratch, or by porting the [MRDS Distance package](https://distancesampling.org/) to Python,
+    * or: by rewriting MCDS using the [MRDS Distance package](https://distancesampling.org/), meaning some kind of interface to R,
+* user interface:
+  * build a GUI for pyaudisam command-line (with some kind of "project" concept, and parameter set template, and ...),
 * ...
 
+### Known issues
+
+* AnalysisResultsSet.toOpenDoc sometimes produces broken header rows (the 3-row multi-index header is not rendered as it is on the right side),
+* The new undocumented MCDS 7.4 result column names are not translated correctly (switched fr and en translations) (minor, as not used actually for the moment),
+* The "Details" table header is not translated in auto-filtered reports (whereas the "Synthesis" one is),
+* Too many decimals rendered for the Max/Min dist figures in HTML reports when the distance unit is "meter",
+* The colorisation of HTML and workbook auto-filtered reports is of no use as it is now (need for a full rework).
+
+### Release notes
+
+You can [read them here](https://github.com/denmedius/pyaudisam/blob/main/docs/release-notes.md) :-)
+
 ### Some hints
 
 Some formal things that I don't plan to change (let's concentrate on substantive content) :-)
 * this code is not blacked or isorted or fully conform to pep8 (but it's clean, commented, and it works),
 * the identifier naming scheme used is old-fashioned: camel case everywhere.
```

### Comparing `pyaudisam-1.0.2/pyaudisam.egg-info/SOURCES.txt` & `pyaudisam-1.1.0/pyaudisam.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+.coveragerc
 LICENSE.txt
 MANIFEST.in
 README.md
+pytest.ini
 requirements.txt
 setup.cfg
 setup.py
+docs/release-notes.md
 docs/how-it-works/how-it-works-en.md
 docs/how-it-works/how-it-works-fr.md
 docs/how-it-works/common/fa-angle-up.svg
 docs/how-it-works/common/fa-arrow-left-hover.svg
 docs/how-it-works/common/fa-arrow-left.svg
 docs/how-it-works/common/fa-arrow-right-hover.svg
 docs/how-it-works/common/fa-arrow-right.svg
@@ -104,28 +107,30 @@
 pyaudisam/__main__.py
 pyaudisam/analyser.py
 pyaudisam/analysis.py
 pyaudisam/data.py
 pyaudisam/engine.py
 pyaudisam/executor.py
 pyaudisam/log.py
+pyaudisam/main.py
 pyaudisam/optanalyser.py
 pyaudisam/optimisation.py
 pyaudisam/optimiser.py
 pyaudisam/report.py
 pyaudisam/utils.py
 pyaudisam.egg-info/PKG-INFO
 pyaudisam.egg-info/SOURCES.txt
 pyaudisam.egg-info/dependency_links.txt
 pyaudisam.egg-info/requires.txt
 pyaudisam.egg-info/top_level.txt
 pyaudisam/mcds/anlys.htpl
 pyaudisam/mcds/fulltop.htpl
 pyaudisam/mcds/pretop.htpl
 pyaudisam/mcds/stat-mod-notes.txt
+pyaudisam/mcds/stat-mod-specs.old.txt
 pyaudisam/mcds/stat-mod-specs.txt
 pyaudisam/mcds/stat-mod-trans.txt
 pyaudisam/mcds/stat-row-specs.txt
 pyaudisam/mcds/top.htpl
 pyaudisam/report/fa-angle-up.svg
 pyaudisam/report/fa-arrow-left-hover.svg
 pyaudisam/report/fa-arrow-left.svg
@@ -137,29 +142,39 @@
 pyaudisam/report/fa-file-excel-hover.svg
 pyaudisam/report/fa-file-excel.svg
 pyaudisam/report/report.css
 tests/conftest.py
 tests/devarchives1.ipynb
 tests/devarchives2.ipynb
 tests/ipython_notebook_toc.js
+tests/requirements.txt
 tests/sensitivity.ipynb
-tests/unint_analyser_results_test.py
-tests/unint_data_test.py
-tests/unint_engine_test.py
+tests/test_unint_analysis_results.py
+tests/test_unint_data.py
+tests/test_unint_engine.py
+tests/test_unint_mcds_analyser.py
+tests/test_unint_mcds_analysis.py
+tests/test_unint_mcds_analysis_results.py
+tests/test_unint_mcds_optanalysis_results.py
+tests/test_unint_mcds_optimiser.py
+tests/test_unint_utils_logger.py
+tests/test_val_mcds_analyser.py
+tests/test_val_mcds_optanalyser.py
+tests/test_val_mcds_preanalyser.py
 tests/unintests.ipynb
 tests/unintval_utils.py
 tests/valarchives.ipynb
 tests/valtests-ds-params.py
 tests/valtests.ipynb
-tests/refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt
-tests/refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods
-tests/refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx
-tests/refin/ACDC2019-Naturalist-ExtraitSpecsEchants.ods
-tests/refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx
-tests/refin/ACDC2019-Naturalist-UnitestOptResultats.ods
+tests/refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt
+tests/refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods
+tests/refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.ods
+tests/refin/ACDC2019-Naturalist-extrait-SpecsEchants.ods
+tests/refin/ACDC2019-Naturalist-extrait-SpecsOptAnalyses.ods
+tests/refin/ACDC2019-Naturalist-extrait-UnitestOptResultats.ods
 tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dec-dist.txt
 tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dotdec-dist.txt
 tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-6dec-dist.txt
 tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-ttdec-dist.txt
 tests/refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods
 tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.ods
 tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xlsx
@@ -173,19 +188,24 @@
 tests/refin/ACDC2019-Papyrus-PHYCOL-AB-10mn-ttdec-dist.txt
 tests/refin/ACDC2019-Papyrus-SYLATR-AB-10mn-ttdec-dist.txt
 tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-1dec-dist.txt
 tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-6dec-dist.txt
 tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-ttdec-dist.txt
 tests/refin/ACDC2019-Papyrus-TURMER-AB-5mn-1dec-dist.txt
 tests/refin/TURMER-10mn-1dec-hnorm-cos.odt
-tests/refout/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist-sampleDataSet.xlsx
-tests/refout/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist-sampleDataSet_sep.xlsx
-tests/refout/ACDC2019-Naturalist-ExtraitOptResultats.ods
-tests/refout/ACDC2019-Naturalist-ExtraitPreResultats.ods
-tests/refout/ACDC2019-Naturalist-ExtraitResultats.ods
+tests/refout/ACDC2019-Naturalist-extrait-OptRapport.ExAicMQua-r900m6q3d15.html
+tests/refout/ACDC2019-Naturalist-extrait-OptRapport.ods
+tests/refout/ACDC2019-Naturalist-extrait-OptResultats.ods
+tests/refout/ACDC2019-Naturalist-extrait-PreRapport.html
+tests/refout/ACDC2019-Naturalist-extrait-PreRapport.ods
+tests/refout/ACDC2019-Naturalist-extrait-PreResultats.ods
+tests/refout/ACDC2019-Naturalist-extrait-Rapport.html
+tests/refout/ACDC2019-Naturalist-extrait-Rapport.ods
+tests/refout/ACDC2019-Naturalist-extrait-Resultats.ods
 tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-distance-73.xlsx
 tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-postcomp.ods
 tests/refout/ACDC2019-Papyrus-ALAARV-saisie-5-cols.txt
 tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-clusters.txt
 tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-noextra.txt
 tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-withextra.txt
-tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.txt
+tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.txt
+tests/refout/mcds-stat-specs.ods
```

### Comparing `pyaudisam-1.0.2/setup.py` & `pyaudisam-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # This script is for building the source and binary PyPI packages for pyaudisam:
 # you can use the official python way (after installing the 'build' package):
 # $ python -m build
 # ... or the old way (should also work out of the box):
 # $ python setup.py sdist bdist_wheel
 
-from setuptools import setup
+import setuptools as sut
 import pathlib as pl
 import re
 
 # The directory containing this file
 here = pl.Path(__file__).parent
 
 # Retrieve version from __init__.py
@@ -34,26 +34,32 @@
 with open(here / 'README.md') as file:
     long_desc = file.read()
 
 # Retrieve install_requires from requirements.txt
 with open(here / 'requirements.txt') as file:
     requirements = file.read().splitlines()
 
+# Retrieve extra_requires['test'] from test/requirements.txt
+with open(here / 'tests/requirements.txt') as file:
+    # Skip first line "-r requirements.txt" present for direct pip install -r
+    test_requirements = file.read().splitlines()[1:]
+
 # This call to setup() does all the final work !
-setup(name='pyaudisam', version=version, url='https://github.com/denmedius/pyaudisam',
-      description='Distance Sampling automation through python and Distance sofware',
-      long_description=long_desc, long_description_content_type='text/markdown',
-      author='denmedius', author_email='fefeqe22.vucuqu82@murena.io',
-      license='GPLv3+',
-      classifiers=['Topic :: Software Development :: Libraries',
-                   'Topic :: Software Development :: Libraries :: Python Modules',
-                   'Intended Audience :: Science/Research',
-                   'Development Status :: 3 - Alpha',
-                   'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-                   'Programming Language :: Python :: 3 :: Only',
-                   'Programming Language :: Python :: 3.8',
-                   'Environment :: Win32 (MS Windows)'],
-      packages=['pyaudisam'],
-      include_package_data=True,
-      python_requires='>=3.8',
-      install_requires=requirements,
-      entry_points={'console_scripts': []})
+sut.setup(name='pyaudisam', version=version, url='https://github.com/denmedius/pyaudisam',
+          description='Distance Sampling automation through python and Distance software',
+          long_description=long_desc, long_description_content_type='text/markdown',
+          author='denmedius', author_email='fefeqe22.vucuqu82@murena.io',
+          license='GPLv3+',
+          classifiers=['Topic :: Software Development :: Libraries',
+                       'Topic :: Software Development :: Libraries :: Python Modules',
+                       'Intended Audience :: Science/Research',
+                       'Development Status :: 3 - Alpha',
+                       'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
+                       'Programming Language :: Python :: 3 :: Only',
+                       'Programming Language :: Python :: 3.8',
+                       'Environment :: Win32 (MS Windows)'],
+          packages=['pyaudisam', 'pyaudisam.mcds', 'pyaudisam.report'],
+          include_package_data=True,
+          python_requires='~=3.8',
+          install_requires=requirements,
+          extras_require={'test': test_requirements},
+          entry_points={'console_scripts': []})
```

### Comparing `pyaudisam-1.0.2/tests/devarchives1.ipynb` & `pyaudisam-1.1.0/tests/devarchives1.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8749778368794326%*

 * *Differences: {"'cells'": '{188: {\'source\': {insert: [(0, "dfObs = '*

 * *            "pd.read_csv('refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt', sep='\\\\t', "*

 * *            'decimal=\',\')\\n")], delete: [0]}}}',*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -2534,15 +2534,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfObs = pd.read_csv('refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt', sep='\\t', decimal=',')\n",
+                "dfObs = pd.read_csv('refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt', sep='\\t', decimal=',')\n",
                 "dfObs.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -4905,9 +4905,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.8.2"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `pyaudisam-1.0.2/tests/devarchives2.ipynb` & `pyaudisam-1.1.0/tests/devarchives2.ipynb`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8749614632679149%*

 * *Differences: {"'cells'": "{27: {'metadata': {replace: OrderedDict()}}, 202: {'source': {insert: [(31, "*

 * *            '"indivObsFile = \'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods\'\\n")], delete: '*

 * *            '[31]}}}',*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -409,17 +409,15 @@
                 "    logger.info('Ecriture des resultats mis \u00e0 jour: {} ...'.format((tmpDir / resFileName.name).as_posix()))\n",
                 "    results.toExcel(tmpDir / resFileName.name)  # Note: This actually triggers post-computations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "scrolled": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "# In case not yet done, trigger post-compute columns (re)-computation (create/update quality indicators and sort orders).\n",
                 "dfActRes = results.dfTransData('fr')\n",
                 "dfActRes"
             ]
         },
@@ -2876,15 +2874,15 @@
                 "clustering = False\n",
                 "\n",
                 "# Results post-computation parameters\n",
                 "ldTruncIntrvSpecs = [dict(col='left', minDist=5.0, maxLen=5.0), dict(col='right', minDist=25.0, maxLen=25.0)]\n",
                 "truncIntrvEpsilon = 1e-6\n",
                 "\n",
                 "# Load individualised observations and actual transects\n",
-                "indivObsFile = 'refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods'\n",
+                "indivObsFile = 'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods'\n",
                 "\n",
                 "dfObsIndiv = ads.DataSet(indivObsFile, sheet='Donn\u00e9esIndiv').dfData\n",
                 "\n",
                 "dfTransects = ads.DataSet(indivObsFile, sheet='Inventaires').dfData\n",
                 "\n",
                 "dict(indivObs=len(dfObsIndiv), transects=len(dfTransects))"
             ]
@@ -5348,9 +5346,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.8.2"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `pyaudisam-1.0.2/tests/ipython_notebook_toc.js` & `pyaudisam-1.1.0/tests/ipython_notebook_toc.js`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-ExtraitSpecsEchants.ods` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-SpecsEchants.ods`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Naturalist-UnitestOptResultats.ods` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Naturalist-extrait-UnitestOptResultats.ods`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dotdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-1dotdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-6dec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-6dec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.ods` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.ods`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xlsx` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-ANTTRI-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-ANTTRI-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-COLPAL-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-COLPAL-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-DonneesBrutesPourAutoDS.xlsx` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-DonneesBrutesPourAutoDS.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-EMBCIR-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-EMBCIR-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-EMBCIT-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-EMBCIT-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-LUSMEG-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-LUSMEG-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-MILCAL-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-MILCAL-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-PHYCOL-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-PHYCOL-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-SYLATR-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-SYLATR-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-1dec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-1dec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-6dec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-6dec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-ttdec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-10mn-ttdec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/ACDC2019-Papyrus-TURMER-AB-5mn-1dec-dist.txt` & `pyaudisam-1.1.0/tests/refin/ACDC2019-Papyrus-TURMER-AB-5mn-1dec-dist.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refin/TURMER-10mn-1dec-hnorm-cos.odt` & `pyaudisam-1.1.0/tests/refin/TURMER-10mn-1dec-hnorm-cos.odt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-distance-73.xlsx` & `pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-distance-73.xlsx`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-postcomp.ods` & `pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-postcomp.ods`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-5-cols.txt` & `pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-5-cols.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-noextra.txt` & `pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-noextra.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-withextra.txt` & `pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-withextra.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.txt` & `pyaudisam-1.1.0/tests/refout/ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.txt`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/sensitivity.ipynb` & `pyaudisam-1.1.0/tests/sensitivity.ipynb`

 * *Files identical despite different names*

### Comparing `pyaudisam-1.0.2/tests/unint_analyser_results_test.py` & `pyaudisam-1.1.0/tests/test_unint_mcds_analysis_results.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,555 +1,209 @@
 # coding: utf-8
 # PyAuDiSam: Automation of Distance Sampling analyses with Distance software (http://distancesampling.org/)
 
-# Copyright (C) 2021 Jean-Philippe Meuret, Sylvain Sainnier
+# Copyright (C) 2021 Jean-Philippe Meuret
 
 # This program is free software: you can redistribute it and/or modify it under the terms
 # of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 
 # Automated unit and integration tests for "analyser" submodule, results set part
 
-# To run : simply run "pytest" or "python <this file>" in current folder
-#          and check standard output ; and ./tmp/unt-ars.{datetime}.log for details
+# To run : simply run "pytest" and check standard output + ./tmp/unt-ars.{datetime}.log for details
 
-# WARNING : Work in progress ... not working yet ... but soon ... patience !
-
-import sys
 import copy
 
 import numpy as np
 import pandas as pd
 
 import pytest
 
 import pyaudisam as ads
 
 import unintval_utils as uivu
 
 
+# Mark module
+pytestmark = pytest.mark.unintests
+
 # Setup local logger.
 logger = uivu.setupLogger('unt.ars', level=ads.DEBUG,
                           otherLoggers={'ads.eng': ads.INFO2, 'ads.dat': ads.INFO,
                                         'ads.anr': ads.INFO5})
 
-what2Test = 'analysis results set'
+# Set to False to skip final cleanup (useful for debugging)
+KFinalCleanup = True
+
+KWhat2Test = 'MCDS analysis results set'
 
 
 ###############################################################################
 #                         Actions to be done before any test                  #
 ###############################################################################
 def testBegin():
-    uivu.logBegin(what=what2Test)
+    uivu.logBegin(what=KWhat2Test)
+    # uivu.setupWorkDir('unt-mares')
 
 
 ###############################################################################
 #                                Test Cases                                   #
 ###############################################################################
 
-# AnalysisResultsSet class with specialised postComputeColumns
-# (with an extra. post-computed column: Delta AIC)
-class TestAnalysisResultsSet(ads.analyser.AnalysisResultsSet):
-
-    def __init__(self, miCustomCols=None, dfCustomColTrans=None,
-                 dComputedCols=None, dfComputedColTrans=None):
-        super().__init__(ads.MCDSAnalysis, miCustomCols, dfCustomColTrans, dComputedCols, dfComputedColTrans)
-
-    # Post-computations.
-    def postComputeColumns(self):
-        # Compute Delta AIC (AIC - min(group)) per { species, sample, precision, duration } group.
-        # a. Minimum AIC per group
-        aicColInd = ('detection probability', 'AIC value', 'Value')
-        aicGroupColInds = [('sample', 'species', 'Value'), ('sample', 'periods', 'Value'),
-                           ('sample', 'duration', 'Value'), ('variant', 'precision', 'Value')]
-        df2Join = self._dfData.groupby(aicGroupColInds)[[aicColInd]].min()
-
-        # b. Rename computed columns to target
-        deltaAicColInd = ('detection probability', 'Delta AIC', 'Value')
-        df2Join.columns = pd.MultiIndex.from_tuples([deltaAicColInd])
-
-        # c. Join the column to the target data-frame
-        self._dfData = self._dfData.join(df2Join, on=aicGroupColInds)
-
-        # d. Compute delta-AIC in-place
-        self._dfData[deltaAicColInd] = self._dfData[aicColInd] - self._dfData[deltaAicColInd]
-
-
-def testArsCtorGettersSettersToFromFiles():
-    # Results object construction
-    miCustCols = pd.MultiIndex.from_tuples([('id', 'index', 'Value'),
-                                            ('sample', 'species', 'Value'),
-                                            ('sample', 'periods', 'Value'),
-                                            ('sample', 'duration', 'Value'),
-                                            ('variant', 'precision', 'Value')])
-    dfCustColTrans = \
-        pd.DataFrame(index=miCustCols,
-                     data=dict(en=['index', 'species', 'periods', 'duration', 'precision'],
-                               fr=['numéro', 'espèce', 'périodes', 'durée', 'précision']))
-    dCompCols = {('detection probability', 'Delta AIC', 'Value'):
-                     len(ads.MCDSEngine.statSampCols()) + len(ads.MCDSAnalysis.MIRunColumns) + 11}  # Right before AIC
-    dfCompColTrans = \
-        pd.DataFrame(index=dCompCols.keys(),
-                     data=dict(en=['Delta AIC'], fr=['Delta AIC']))
-
-    rs = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-
-    # ### b. Some getters
-    # empty
-    assert rs.empty
-
-    # len
-    assert len(rs) == 0
-
-    # index
-    assert len(rs.index) == 0
-    assert rs.index.to_list() == []
-
-    # columns
-    assert len(rs.columns) == 0
-
-    # ### c. Append result rows
-    # append
-    sHead = pd.Series(index=miCustCols, data=list(range(len(miCustCols))))
-    miResCols = ads.MCDSEngine.statSampCols().append(ads.MCDSAnalysis.MIRunColumns).append(ads.MCDSEngine.statModCols())
-    sResult = pd.Series(index=miResCols, data=list(range(len(miResCols))))  # Fictive data, never mind !
-    rs.append(sResult, sCustomHead=sHead)
-    sResult = pd.Series(index=miResCols, data=list(range(1, len(miResCols) + 1)))  # Fictive data, never mind !
-    rs.append(sResult, sCustomHead=sHead)
-    sResult = pd.Series(index=miResCols, data=list(range(2, len(miResCols) + 2)))  # Fictive data, never mind !
-    rs.append(sResult, sCustomHead=sHead)
-
-    # ### d. Some getters again
-    # dfRawData (no post-computed columns)
-    dfRaw = rs.dfRawData
-    dfRaw
-
-    # columns (Beware: rs.columns does trigger computation of ... computed columns !)
-    assert len(rs._dfData.columns) == len(dfRaw.columns) and len(dfRaw.columns) == 113
-    rawCols = rs._dfData.columns.to_list()
-    rawCols
-
-    # columns
-    assert len(rs.columns) == 114  # The proof here !
-    postCols = rs.columns.to_list()
-    postCols
-
-    # Check added == compute column
-    assert set(rs.columns.to_list()) - set(dfRaw.columns.to_list()) == {('detection probability', 'Delta AIC', 'Value')}
-
-    # dfData (post-computations already done, never mind)
-    dfPost = rs.dfData
-    dfPost
-
-    # index
-    assert len(rs.index) == 3
-    assert rs.index.to_list() == [0, 1, 2]
-
-    # ### e. Getters: dfSubData
-    columns = [('id', 'index', 'Value'), ('sample', 'species', 'Value'),
-               ('sample', 'periods', 'Value'), ('sample', 'duration', 'Value'),
-               ('detection probability', 'Delta AIC', 'Value')]
-    index = [0, 2]
-    dfSub = rs.dfSubData(index=index, columns=columns)
-    assert len(dfSub) == 2
-    assert dfSub.index.to_list() == index
-    assert dfSub.columns.to_list() == columns
-    dfSub
-
-    # ### f. Getters: Translation
-    # dfTransData
-    dfTrans = rs.dfTransData('fr')
-    assert len(dfPost.columns) == len(dfTrans.columns)
-    dfTrans
-
-    dfTrans.columns.to_list()
-
-    dfTrSub = rs.dfTransData('en', index=index, columns=columns)
-    assert len(dfTrSub) == 2
-    assert dfTrSub.index.to_list() == index
-    assert dfTrSub.columns.to_list() == ['index', 'species', 'periods', 'duration', 'Delta AIC']
-    dfTrSub
-
-    # ### g. Specs management
-    rs.updateSpecs(d=dict(a=1, b=2), df=pd.DataFrame([dict(a=3, b=4), dict(a=7, b=9, v=90)]), reset=True)
-
-    rs.updateSpecs(l=[9, -9], s=pd.Series(dict(e=3, f=5), name='serie'))
-    rs.specs
-
-    try:
-        rs.updateSpecs(l=[8, -8, 0])
-        assert False, "Error: Should have refused to overwite already existing 'l'"
-    except AssertionError:
-        print('Good: Refused to overwrite existing spec if not explicitly authorised to')
-    assert rs.specs['l'] == [9, -9]
-    rs.specs
-
-    rs.updateSpecs(**dict(l=[7, -7, 77]), overwrite=True)
-    print('Good: Accepted to overwrite existing spec if explicitly authorised to')
-    assert rs.specs['l'] == [7, -7, 77]
-    rs.specs
-
-    # ### h. Imports and exports
-    # #### i. Exports (with specs)
-    # (see imports tests below for exported content checks)
-    rs.toExcel('tmp/results-set-uni.xlsx', sheetName='utest')
-
-    rs.toExcel('tmp/results-set-uni.xls', sheetName='utest')
-
-    rs.toOpenDoc('tmp/results-set-uni.ods', sheetName='utest')
-
-    rs.toPickle('tmp/results-set-uni.pickle.xz')
-
-    rs.toPickle('tmp/results-set-uni.pickle')
-
-    # ### h. Imports and exports
-    # #### ii. Imports with explicit format (with specs)
-    # A. XLSX Format
-    rs1 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs1.fromExcel('tmp/results-set-uni.xlsx', sheetName='utest')
-    rs1.dfData
-
-    # Data
-    assert rs1.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs1.specs['d'], dict) and rs1.specs['d'] == rs.specs['d']
-    assert isinstance(rs1.specs['df'], pd.DataFrame) and rs1.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs1.specs['l'], list) and rs1.specs['l'] == rs.specs['l']
-    assert isinstance(rs1.specs['s'], pd.Series) and rs1.specs['s'].name == rs.specs['s'].name \
-           and rs1.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs1.specs
-
-    # B. XLS Format
-    rs2 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs2.fromExcel('tmp/results-set-uni.xls', sheetName='utest')
-    rs2.dfData
-
-    # Data
-    assert rs2.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs2.specs['d'], dict) and rs2.specs['d'] == rs.specs['d']
-    assert isinstance(rs2.specs['df'], pd.DataFrame) and rs2.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs2.specs['l'], list) and rs2.specs['l'] == rs.specs['l']
-    assert isinstance(rs2.specs['s'], pd.Series) and rs2.specs['s'].name == rs.specs['s'].name \
-           and rs2.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs2.specs
-
-    # C. Format ODS
-    rs3 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs3.fromOpenDoc('tmp/results-set-uni.ods', sheetName='utest')
-    rs3.dfData
-
-    # Data
-    assert rs3.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs3.specs['d'], dict) and rs3.specs['d'] == rs.specs['d']
-    assert isinstance(rs3.specs['df'], pd.DataFrame) and rs3.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs3.specs['l'], list) and rs3.specs['l'] == rs.specs['l']
-    assert isinstance(rs3.specs['s'], pd.Series) and rs3.specs['s'].name == rs.specs['s'].name \
-           and rs3.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs3.specs
-
-    # D. Format pickle comprimé
-    rs4 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs4.fromPickle('tmp/results-set-uni.pickle.xz')
-    rs4.dfData
-
-    # Data
-    assert rs4.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs4.specs['d'], dict) and rs4.specs['d'] == rs.specs['d']
-    assert isinstance(rs4.specs['df'], pd.DataFrame) and rs4.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs4.specs['l'], list) and rs4.specs['l'] == rs.specs['l']
-    assert isinstance(rs4.specs['s'], pd.Series) and rs4.specs['s'].name == rs.specs['s'].name \
-           and rs4.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs4.specs
-
-    # E. Format pickle non comprimé
-    rs5 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs5.fromPickle('tmp/results-set-uni.pickle')
-    rs5.dfData
-
-    # Data
-    assert rs5.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs5.specs['d'], dict) and rs5.specs['d'] == rs.specs['d']
-    assert isinstance(rs5.specs['df'], pd.DataFrame) and rs5.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs5.specs['l'], list) and rs5.specs['l'] == rs.specs['l']
-    assert isinstance(rs5.specs['s'], pd.Series) and rs5.specs['s'].name == rs.specs['s'].name \
-           and rs5.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs5.specs
-
-    # #### iii. Imports with auto-detected format (with specs)
-    # A. XLSX Format
-    rs1 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs1.fromFile('tmp/results-set-uni.xlsx', sheetName='utest')
-    rs1.dfData
-
-    # Data
-    assert rs1.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs1.specs['d'], dict) and rs1.specs['d'] == rs.specs['d']
-    assert isinstance(rs1.specs['df'], pd.DataFrame) and rs1.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs1.specs['l'], list) and rs1.specs['l'] == rs.specs['l']
-    assert isinstance(rs1.specs['s'], pd.Series) and rs1.specs['s'].name == rs.specs['s'].name \
-           and rs1.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs1.specs
-
-    # B. XLS Format
-    rs2 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs2.fromFile('tmp/results-set-uni.xls', sheetName='utest')
-    rs2.dfData
-
-    # Data
-    assert rs2.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs2.specs['d'], dict) and rs2.specs['d'] == rs.specs['d']
-    assert isinstance(rs2.specs['df'], pd.DataFrame) and rs2.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs2.specs['l'], list) and rs2.specs['l'] == rs.specs['l']
-    assert isinstance(rs2.specs['s'], pd.Series) and rs2.specs['s'].name == rs.specs['s'].name \
-           and rs2.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs2.specs
-
-    # C. Format ODS
-    rs3 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs3.fromFile('tmp/results-set-uni.ods', sheetName='utest')
-    rs3.dfData
-
-    # Data
-    assert rs3.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs3.specs['d'], dict) and rs3.specs['d'] == rs.specs['d']
-    assert isinstance(rs3.specs['df'], pd.DataFrame) and rs3.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs3.specs['l'], list) and rs3.specs['l'] == rs.specs['l']
-    assert isinstance(rs3.specs['s'], pd.Series) and rs3.specs['s'].name == rs.specs['s'].name \
-           and rs3.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs3.specs
-
-    # D. Format pickle comprimé
-    rs4 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs4.fromFile('tmp/results-set-uni.pickle.xz')
-    rs4.dfData
-
-    # Data
-    assert rs4.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs4.specs['d'], dict) and rs4.specs['d'] == rs.specs['d']
-    assert isinstance(rs4.specs['df'], pd.DataFrame) and rs4.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs4.specs['l'], list) and rs4.specs['l'] == rs.specs['l']
-    assert isinstance(rs4.specs['s'], pd.Series) and rs4.specs['s'].name == rs.specs['s'].name \
-           and rs4.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs4.specs
-
-    # E. Format pickle non comprimé
-    rs5 = TestAnalysisResultsSet(miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
-                                 dComputedCols=dCompCols, dfComputedColTrans=dfCompColTrans)
-    rs5.fromFile('tmp/results-set-uni.pickle')
-    rs5.dfData
-
-    # Data
-    assert rs5.dfData.equals(rs.dfData)  # == fails on NaNs in same places ...
-
-    # Specs
-    assert isinstance(rs5.specs['d'], dict) and rs5.specs['d'] == rs.specs['d']
-    assert isinstance(rs5.specs['df'], pd.DataFrame) and rs5.specs['df'].equals(
-        rs.specs['df'])  # == fails on NaNs in same places
-    assert isinstance(rs5.specs['l'], list) and rs5.specs['l'] == rs.specs['l']
-    assert isinstance(rs5.specs['s'], pd.Series) and rs5.specs['s'].name == rs.specs['s'].name \
-           and rs5.specs['s'].equals(rs.specs['s'])  # == fails on NaNs in same places
-    rs5.specs
-
-    # #### iv. Imports with default values for missing columns
-    # TODO
-    # How ?
-    # For each file format,
-    # - read target file (written above) with pandas API (not ResultsSet one)
-    # - remove some columns
-    # - overwrite target file with pandas API
-    # - load target file with ResultsSet API, specifying default values for the missing columns
-    # - check that results is OK
-
-    logger.info0('PASS (testArsCtorGettersSettersToFromFiles) => Constructor, empty, len, columns, index, append,\n'
-                 ' dfRawData, dfData, dfTransData, updateSpecs, toExcel(xlsx, xls), toOpenDoc, toPickle(std, xz)\n'
-                 ' fromFile(xlsx, xls, ods, pickle.xz, pickle)')
-
-????????????????????????????????????????????
-
-# ### i. Comparison
+# 5. AnalysisResultsSet and ResultsSet classes (2/2, see test_unint_analysis_results.py for 1/2)
+# i. Comparison
 def testMcdsArsCompare():
 
     # MCDSAnalysisResultsSet objects and loading from files.
     modelIdCols = ['Model']
-    modelParamCols = ['LTrunc', 'RTrunc', 'FitDistCuts', 'DiscrDistCuts']
+    # modelParamCols = ['LTrunc', 'RTrunc', 'FitDistCuts', 'DiscrDistCuts']
     sampleIdCols = ['Species', 'Periods', 'Prec.', 'Duration']
     caseIdCols = ['AnlysNum', 'SampNum'] + sampleIdCols + modelIdCols
     sampCols = [('sample', col, 'Value') for col in sampleIdCols]
     miSampCols = pd.MultiIndex.from_tuples(sampCols)
-    custCols = [('sample', 'AnlysNum', 'Value'), ('sample', 'SampNum', 'Value')] + sampCols + [('model', 'Model', 'Value')]
+    custCols = [('sample', 'AnlysNum', 'Value'), ('sample', 'SampNum', 'Value')] \
+               + sampCols + [('model', 'Model', 'Value')]
     miCustCols = pd.MultiIndex.from_tuples(custCols)
     dfCustColTrans = \
         pd.DataFrame(index=miCustCols,
                      data=dict(en=caseIdCols,
                                fr=['NumAnlys', 'NumSamp', 'Espèce', 'Périodes', 'Préc.', 'Durée', 'Modèle']))
 
     # Réference (built with Distance 7.3)
     rsDist = ads.MCDSAnalysisResultsSet(miSampleCols=miSampCols, sampleIndCol=('sample', 'SampNum', 'Value'),
                                         miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
                                         distanceUnit='Meter', areaUnit='Hectare',
                                         surveyType='Point', distanceType='Radial', clustering=False)
-    rsDist.fromFile('refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods', sheetName='RefDist73',
-                    postComputed=True)  # Avoid recomputations, some columns are now missing, files are old actually !
+    rsDist.fromFile(uivu.pRefInDir / 'ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods', sheetName='RefDist73',
+                    postComputed=True)  # Avoid re-computations, some columns are now missing, files are old actually !
 
     # Results obtained with via pyaudisam.
     rsAuto = ads.MCDSAnalysisResultsSet(miSampleCols=miSampCols, sampleIndCol=('sample', 'SampNum', 'Value'),
                                         miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
                                         distanceUnit='Meter', areaUnit='Hectare',
                                         surveyType='Point', distanceType='Radial', clustering=False)
-    rsAuto.fromFile('refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods', sheetName='ActAuto',
-                    postComputed=True)  # Avoid recomputations, some columns are now missing, files are old actually !
+    rsAuto.fromFile(uivu.pRefInDir / 'ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods', sheetName='ActAuto',
+                    postComputed=True)  # Avoid re-computations, some columns are now missing, files are old actually !
 
     # Index columns
     indexCols = custCols + [('parameters', 'left truncation distance', 'Value'),
                             ('parameters', 'right truncation distance', 'Value'),
                             ('parameters', 'model fitting distance cut points', 'Value'),
                             ('parameters', 'distance discretisation cut points', 'Value')]
 
     # Columns to compare (after removing DeltaDCV and DeltaAIC because they depend on the whole analysis set,
     #                     which differs between the reference and the auto-produced,
     #                     and removing the execution time column).
-    subsetCols = [col for col in rsDist.columns.to_list() \
+    subsetCols = [col for col in rsDist.columns.to_list()
                   if col not in indexCols + [('run output', 'run time', 'Value'),
                                              ('density/abundance', 'density of animals', 'Delta Cv'),
                                              ('detection probability', 'Delta AIC', 'Value')]]
-    subsetCols
+    logger.info('subsetCols: ' + str(subsetCols))
 
     dfRelDiff = rsDist.compare(rsAuto, subsetCols=subsetCols, indexCols=indexCols)
+    logger.info('dfRelDiff: ' + dfRelDiff.to_string())
     assert len(dfRelDiff.columns) == 21
     assert len(dfRelDiff) == len(rsDist)
-    dfRelDiff
 
     dfRelDiff = rsDist.compare(rsAuto, subsetCols=subsetCols, indexCols=indexCols, dropCloser=16, dropNans=False)
+    logger.info('dfRelDiff: ' + dfRelDiff.to_string())
     assert len(dfRelDiff.columns) == 21
     assert len(dfRelDiff) == 8
-    dfRelDiff
 
     dfRelDiff = rsDist.compare(rsAuto, subsetCols=subsetCols, indexCols=indexCols, dropCloser=16, dropNans=True)
+    logger.info('dfRelDiff: ' + dfRelDiff.to_string())
     assert len(dfRelDiff.columns) == 21
     assert len(dfRelDiff) == 3
-    dfRelDiff
 
     dfRelDiff = rsDist.compare(rsAuto, subsetCols=subsetCols, indexCols=indexCols, dropCloser=5, dropNans=True)
+    logger.info('dfRelDiff: ' + dfRelDiff.to_string())
     assert len(dfRelDiff.columns) == 21
     assert len(dfRelDiff) == 2
-    dfRelDiff
 
     # Drop also closer columns
     dfRelDiff = rsDist.compare(rsAuto, subsetCols=subsetCols, indexCols=indexCols, dropCloser=5, dropNans=True,
                                dropCloserCols=True)
+    logger.info('dfRelDiff: ' + dfRelDiff.to_string())
     assert len(dfRelDiff.columns) == 19
-    dfRelDiff
 
-    logger.info0('PASS (testMcdsArsCompare) => compare')
+    logger.info0('PASS testMcdsArsCompare: constructor, fromFile(ODS), compare')
 
 
 # ### j. Post-computations
-# Note: Self-contained, nothing needing to be run before (but 0)
 def testMcdsArsPostCompute():
+    
     # MCDSAnalysisResultsSet object + loading from file
     modelIdCols = ['Model']
-    modelParamCols = ['LTrunc', 'RTrunc', 'FitDistCuts', 'DiscrDistCuts']
+    # modelParamCols = ['LTrunc', 'RTrunc', 'FitDistCuts', 'DiscrDistCuts']
     sampleIdCols = ['Species', 'Periods', 'Prec.', 'Duration']
     caseIdCols = ['AnlysNum', 'SampNum'] + sampleIdCols + modelIdCols
     sampCols = [('sample', col, 'Value') for col in sampleIdCols]
     miSampCols = pd.MultiIndex.from_tuples(sampCols)
-    custCols = [('sample', 'AnlysNum', 'Value'), ('sample', 'SampNum', 'Value')] + sampCols + [('model', 'Model', 'Value')]
+    custCols = [('sample', 'AnlysNum', 'Value'), ('sample', 'SampNum', 'Value')] \
+               + sampCols + [('model', 'Model', 'Value')]
     miCustCols = pd.MultiIndex.from_tuples(custCols)
     dfCustColTrans = \
         pd.DataFrame(index=miCustCols,
                      data=dict(en=caseIdCols,
                                fr=['NumAnlys', 'NumSamp', 'Espèce', 'Périodes', 'Préc.', 'Durée', 'Modèle']))
     rsAuto = ads.MCDSAnalysisResultsSet(miSampleCols=miSampCols, sampleIndCol=('sample', 'SampNum', 'Value'),
                                         miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
                                         distanceUnit='Meter', areaUnit='Hectare',
                                         surveyType='Point', distanceType='Radial', clustering=False)
-    rsAuto.fromFile('refin/ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods', sheetName='ActAuto')
+    rsAuto.fromFile(uivu.pRefInDir / 'ACDC2019-Papyrus-ALAARV-TURMER-comp-dist-auto.ods', sheetName='ActAuto')
 
     # Trigger post-computations
-    rsAuto.dfData
+    logger.info('rsAuto.dfData: ' + rsAuto.dfData.to_string())
 
     # Load reference from file
     rsAutoRef = ads.MCDSAnalysisResultsSet(miSampleCols=miSampCols, sampleIndCol=('sample', 'SampNum', 'Value'),
                                            miCustomCols=miCustCols, dfCustomColTrans=dfCustColTrans,
                                            distanceUnit='Meter', areaUnit='Hectare',
                                            surveyType='Point', distanceType='Radial', clustering=False)
-    rsAutoRef.fromFile('refout/ACDC2019-Papyrus-ALAARV-TURMER-resultats-postcomp.ods')
+    rsAutoRef.fromFile(uivu.pRefOutDir / 'ACDC2019-Papyrus-ALAARV-TURMER-resultats-postcomp.ods')
 
     # Comparison of loaded results to reference
     # a. Index columns
     indexCols = custCols + [('parameters', 'left truncation distance', 'Value'),
                             ('parameters', 'right truncation distance', 'Value'),
                             ('parameters', 'model fitting distance cut points', 'Value'),
                             ('parameters', 'distance discretisation cut points', 'Value'),
                             ('parameters', 'estimator key function', 'Value'),
                             ('parameters', 'estimator adjustment series', 'Value'),
                             ('parameters', 'estimator selection criterion', 'Value')]
     # b. Colonnes to compare : we ignore ...
     # * DeltaDCV et DeltaAIC because they depend on the whole set of analyses actually done to get the results,
     #   that is possibly different sets in the 2 cases.
     # * other string-typed columns (comparison not implemented)
-    subsetCols = [col for col in rsAutoRef.columns.to_list() \
+    subsetCols = [col for col in rsAutoRef.columns.to_list()
                   if col not in indexCols + [('run output', 'run time', 'Value'), ('run output', 'run folder', 'Value'),
                                              ('density/abundance', 'density of animals', 'Delta Cv'),
                                              ('detection probability', 'Delta AIC', 'Value'),
                                              ('detection probability', 'key function type', 'Value'),
                                              ('detection probability', 'adjustment series type', 'Value')]]
     # c. Comparison
     dfRelDiff = rsAuto.compare(rsAutoRef, subsetCols=subsetCols, indexCols=indexCols, dropCloser=15)
+    logger.info('dfRelDiff: ' + dfRelDiff.to_string())
     assert len(dfRelDiff) == 0
-    dfRelDiff
+
+    logger.info0('PASS testMcdsArsPostCompute: constructor, postCompute, columns, fromFile(ODS')
 
 
 # ## 13. MCDSAnalysisResultsSet
-def testMcdsArsGroupingIntervals():
+RS = ads.MCDSAnalysisResultsSet
 
-    RS = ads.MCDSAnalysisResultsSet
 
-    # ### a. _groupingIntervals
+# ### a. _groupingIntervals
+def testMcdsArsGroupingIntervals():
+
     # Old code that was slightly modified ... for non-regression tests.
     def intervalsOld(sDists, minIntrvDist, maxIntrvLen, intrvEpsilon):
         # For some reason, need for enforcing float dtype ... otherwise dtype='O' !?
         sSelDist = sDists.dropna().astype(float).sort_values()
         # List non-null differences between consecutive sorted distances
         dfIntrv = pd.DataFrame(dict(dist=sSelDist.values))
         if not dfIntrv.empty:
@@ -561,34 +215,33 @@
             dfIntrv['dMin'] = dfIntrv.loc[dfIntrv.deltaDist > minIntrvDist, 'dist']
             dfIntrv['dSup'] = dfIntrv.loc[dfIntrv.deltaDist > minIntrvDist, 'dist'].shift(-1).dropna()
             dfIntrv.loc[dfIntrv['dMin'].idxmax(), 'dSup'] = np.inf
             dfIntrv.dropna(inplace=True)
             dfIntrv['dSup'] = \
                 dfIntrv['dSup'].apply(lambda supV: sSelDist[sSelDist < supV].max() + intrvEpsilon)
             dfIntrv = dfIntrv[['dMin', 'dSup']].reset_index(drop=True)
-            # If these intervals are two wide, cut them up in equal sub-intervals and make them new intervals
+            # If these intervals are too wide, cut them up in equal sub-intervals and make them new intervals
             lsNewIntrvs = list()
             for _, sIntrv in dfIntrv.iterrows():
                 if sIntrv.dSup - sIntrv.dMin > maxIntrvLen:
-                    # print(sIntrv.dSup, '-', sIntrv.dMin, '>', maxIntrvLen)
+                    # logger.info(sIntrv.dSup, '-', sIntrv.dMin, '>', maxIntrvLen)
                     nSubIntrvs = (sIntrv.dSup - sIntrv.dMin) / maxIntrvLen
                     nSubIntrvs = int(nSubIntrvs) if nSubIntrvs - int(nSubIntrvs) < 0.5 else int(nSubIntrvs) + 1
                     subIntrvLen = (sIntrv.dSup - sIntrv.dMin) / nSubIntrvs
                     lsNewIntrvs += [pd.Series(dict(dMin=sIntrv.dMin + nInd * subIntrvLen,
                                                    dSup=min(sIntrv.dMin + (nInd + 1) * subIntrvLen,
                                                             sIntrv.dSup)))
                                     for nInd in range(nSubIntrvs)]
                 else:
                     lsNewIntrvs.append(sIntrv)
             dfIntrv = pd.DataFrame(lsNewIntrvs).reset_index(drop=True)
             dfIntrv.sort_values(by='dMin', inplace=True)
             dfIntrv.rename(columns=dict(dMin='vmin', dSup='vsup'), inplace=True)
         return dfIntrv
 
-
     minDist = 5
     maxLen = 10
     eps = 1e-6
     v0 = 1
     KCases = [dict(values=[np.nan],  # empty series (after cleanup)
                    intervals=[]),
               dict(values=[v0],  # 1 isolated value in 1 shortest interval
@@ -601,75 +254,74 @@
                               {'vmin': 44.9, 'vsup': 44.9 + eps}]),
               dict(values=[v0, 2, np.nan, 3, 8, 9, v0 + maxLen, v0 + maxLen * 1.5,  # Cut 1st interval
                            22, 27, 35, 37, 39, 44.9],
                    intervals=[{'vmin': v0, 'vsup': 8.5},
                               {'vmin': 8.5 + eps, 'vsup': 16.0 + eps},
                               {'vmin': 22, 'vsup': 27 + eps},
                               {'vmin': 35, 'vsup': 39 + eps},
-                              {'vmin': 44.9, 'vsup': 44.9 + eps}]),
-              ]
+                              {'vmin': 44.9, 'vsup': 44.9 + eps}])]
 
-    print(f'{minDist=}, {maxLen=}, {eps=}:')
+    logger.info(f'{minDist=}, {maxLen=}, {eps=}:')
     for case in KCases:
-        print('*', case['values'], ':', end=' ')
+        logger.info(f'* {case["values"]}: ')
         dfIntrvs = RS._groupingIntervals(pd.Series(case['values']), minDist=minDist, maxLen=maxLen, epsilon=eps)
-        print(dfIntrvs.to_dict('index'))
+        logger.info(' => ' + dfIntrvs.to_string())
         dfDiff = ads.DataSet.compareDataFrames(dfIntrvs.reset_index(), pd.DataFrame(case['intervals']).reset_index(),
                                                indexCols=['index'], dropCloser=4)
         assert dfDiff.empty, 'Oh, oh ... not what we expected ; diff to ref= ' + str(dfDiff.to_dict('index')) \
                              + '\nref= ' + str(case['intervals'])
 
         # Non regression, comparing to old code results
-        dfIntrvsOld = intervalsOld(pd.Series(case['values']), minIntrvDist=minDist, maxIntrvLen=maxLen, intrvEpsilon=eps)
+        dfIntrvsOld = intervalsOld(pd.Series(case['values']),
+                                   minIntrvDist=minDist, maxIntrvLen=maxLen, intrvEpsilon=eps)
         dfDiffOld = ads.DataSet.compareDataFrames(dfIntrvs.reset_index(), dfIntrvsOld.reset_index(),
                                                   indexCols=['index'], dropCloser=6)
         assert dfDiff.empty, 'Oh, oh ... not what we expected ; diff to old= ' + str(dfDiffOld.to_dict('index'))
 
-    logger.info('Success !')
+    logger.info0('PASS testMcdsArsGroupingIntervals: _groupingIntervals, compareDataFrames')
 
 
 # ### b. _intervalIndex
 def testMcdsArsIntervalIndex():
 
-    RS = ads.MCDSAnalysisResultsSet
-
     eps = 1e-6
 
     dfIntrvs = pd.DataFrame([{'vmin': 1, 'vsup': 8.5 + eps},
                              {'vmin': 8.5 + eps, 'vsup': 16 + eps},
                              {'vmin': 22, 'vsup': 27 + eps},
                              {'vmin': 35, 'vsup': 39 + eps},
                              {'vmin': 44.9, 'vsup': 44.9 + eps}])
-    dfIntrvs
+    logger.info('dfIntrvs: ' + dfIntrvs.to_string())
 
     sValues = pd.Series(
         [8.5, 39, 44.9, 1, 11, 16 + eps, 2, np.nan, 3, 8, 8.5 + eps, 9, 16, 22 - eps, 27, 27 + 2 * eps, 35, 22, 37])
 
     # Compute and show results
     sGroups = sValues.apply(RS._intervalIndex, dfIntervals=dfIntrvs)
     pd.DataFrame(dict(values=sValues, group=sGroups))
 
     # Auto-check
     assert sGroups.eq(pd.Series({0: 1, 1: 4, 2: 5, 3: 1, 4: 2, 5: -1, 6: 1, 7: 0, 8: 1, 9: 1, 10: 2,
                                  11: 2, 12: 2, 13: -1, 14: 3, 15: -1, 16: 4, 17: 3, 18: 4})).all()
-    logger.info('Success !')
+
+    logger.info0('PASS testMcdsArsIntervalIndex: _intervalIndex')
 
 
 # An MCDSAnalyser object for creating MCDSAnalysisResultsSet objects
 def mcdsAnalyser():
 
     # Source / Results data
     transectPlaceCols = ['Point']
     passIdCol = 'Passage'
     effortCol = 'Effort'
     sampleDistCol = 'Distance'
     sampleDecCols = [effortCol, sampleDistCol]
     sampleNumCol = 'NumEchant'
     sampleSelCols = ['Espèce', passIdCol, 'Adulte', 'Durée']
-    sampleAbbrevCol = 'AbrevEchant'
+    # sampleAbbrevCol = 'AbrevEchant'
     dSurveyArea = dict(Zone='ACDC', Surface='2400')
 
     # General DS analysis parameters
     varIndCol = 'NumAnlys'
     anlysAbbrevCol = 'AbrevAnlys'
     anlysParamCols = ['FonctionClé', 'SérieAjust', 'TrGche', 'TrDrte', 'NbTrchMod']
     distanceUnit = 'Meter'
@@ -679,24 +331,24 @@
     clustering = False
 
     # Results post-computation parameters
     ldTruncIntrvSpecs = [dict(col='left', minDist=5.0, maxLen=5.0), dict(col='right', minDist=25.0, maxLen=25.0)]
     truncIntrvEpsilon = 1e-6
 
     # Load individualised observations and actual transects
-    indivObsFile = 'refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods'
+    indivObsFile = uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-ObsIndiv.ods'
     dfObsIndiv = ads.DataSet(indivObsFile, sheet='DonnéesIndiv').dfData
     dfTransects = ads.DataSet(indivObsFile, sheet='Inventaires').dfData
     dict(indivObs=len(dfObsIndiv), transects=len(dfTransects))
 
     # What's better to create an MCDSAnalysisResultsSet objets than a MCDSAnalyser instance ?
     return ads.MCDSAnalyser(dfObsIndiv, dfTransects=dfTransects, dSurveyArea=dSurveyArea,
                             transectPlaceCols=transectPlaceCols, passIdCol=passIdCol, effortCol=effortCol,
                             sampleSelCols=sampleSelCols, sampleDecCols=sampleDecCols,
-                            abbrevCol=anlysAbbrevCol, abbrevBuilder=analysisAbbrev,
+                            abbrevCol=anlysAbbrevCol, abbrevBuilder=uivu.analysisAbbrev,
                             anlysIndCol=varIndCol, sampleIndCol=sampleNumCol,
                             distanceUnit=distanceUnit, areaUnit=areaUnit,
                             surveyType=surveyType, distanceType=distanceType, clustering=clustering,
                             resultsHeadCols=dict(before=[varIndCol, sampleNumCol], sample=sampleSelCols,
                                                  after=anlysParamCols + [anlysAbbrevCol]),
                             ldTruncIntrvSpecs=ldTruncIntrvSpecs, truncIntrvEpsilon=truncIntrvEpsilon)
 
@@ -722,19 +374,22 @@
             for preChi22 in [np.nan] + ([] if np.isnan(preChi21) else preChi2NormalRange):
                 expDetChi2 = preChi22 if not np.isnan(preChi22) else preChi21 if not np.isnan(preChi21) else preChi20
                 results.append(pd.Series({RS.CLsChi2All[2]: preChi20, RS.CLsChi2All[1]: preChi21,
                                           RS.CLsChi2All[0]: preChi22, clExpDetChi2: expDetChi2}))
 
     # iii. Post-compute Chi2
     results._postComputeChi2()
+
     # iv. Auto-check results
     assert results._dfData[RS.CLChi2].compare(results._dfData[clExpDetChi2]).empty
-    logger.info('Success !')
+
     # v. Done
-    # results._dfData
+    logger.info('results._dfData: ' + results._dfData.to_string())
+
+    logger.info0('PASS testMcdsArsPostComputeChi2: constructor, _postComputeChi2, compare')
 
 
 # ### e. _postComputeDeltaAicDCv
 # 1/2: normal case
 def testMcdsArsPostComputeDeltaAicDCv1(mcdsAnalyser_fxt):
     anlr = mcdsAnalyser_fxt
 
@@ -762,17 +417,19 @@
                                                   RS.CLDCv: dcv, clExpDeltaDcv: dExpDeltaDcv[dcv]}),
                                        sCustomHead=pd.Series(dSample))
     # iii. Post-compute Delta AIC and DeltaDCv
     results._postComputeDeltaAicDCv()
     # iv. Auto-check results
     assert results._dfData[RS.CLDeltaAic].compare(results._dfData[clExpDeltaAic]).empty
     assert results._dfData[RS.CLDeltaDCv].compare(results._dfData[clExpDeltaDcv]).empty
-    logger.info('Success !')
+
     # v. Done
-    # results._dfData  # .to_excel('tmp/_.xlsx')
+    logger.info('results._dfData: ' + results._dfData.to_string())
+
+    logger.info0('PASS testMcdsArsPostComputeDeltaAicDCv1: constructor, _postComputeDeltaAicDCv, compare')
 
 
 # ### e. _postComputeDeltaAicDCv
 # 2/2: special case with one all-NaN sample id column
 def testMcdsArsPostComputeDeltaAicDCv2(mcdsAnalyser_fxt):
     anlr = mcdsAnalyser_fxt
 
@@ -800,17 +457,19 @@
                                                   RS.CLDCv: dcv, clExpDeltaDcv: dExpDeltaDcv[dcv]}),
                                        sCustomHead=pd.Series(dSample))
     # iii. Post-compute Delta AIC and DeltaDCv
     results._postComputeDeltaAicDCv()
     # iv. Auto-check results
     assert results._dfData[RS.CLDeltaAic].compare(results._dfData[clExpDeltaAic]).empty
     assert results._dfData[RS.CLDeltaDCv].compare(results._dfData[clExpDeltaDcv]).empty
-    logger.info('Success !')
+
     # v. Done
-    results._dfData  # .to_excel('tmp/_2.xlsx')
+    logger.info('results._dfData: ' + results._dfData.to_string())
+
+    logger.info0('PASS testMcdsArsPostComputeDeltaAicDCv2: constructor, _postComputeDeltaAicDCv, compare')
 
 
 # ### f. _postComputeQualityIndicators (and callees)
 # 1/2 Normal case
 def testMcdsArsPostComputeQualityIndicators1(mcdsAnalyser_fxt):
     anlr = mcdsAnalyser_fxt
 
@@ -822,15 +481,15 @@
     densCvRange = [np.nan, 0.1, 0.3, 1]  # Range for density coef. of variation
 
     logger.info('Filling up results to post-compute')
     ldRes = list()
 
     # Try all key functions
     for keyFn in [np.nan, 'HNORMAL', 'UNIFORM', 'HAZARD', 'NEXPON']:
-        # CLNTotPars and CLNAdjPars are used independently, no need for combinations)
+        # CLNTotPars and CLNAdjPars are used independently, no need for combinations
         for nPars in [np.nan, 0, 2, 10]:
             # CLNObs and CLNTotObs are always used together, no need for full combination stuff
             for nObs, nTotObs in [(np.nan, 50), (10, np.nan), (25, 50), (50, 50)]:
                 for chi2 in statsRange:
                     for ks in statsRange:
                         for cvmUw in statsRange:
                             for cvmCw in statsRange:
@@ -859,107 +518,117 @@
 
     # Note: For 65536 results, Windows 10, total elapsed :
     # * 2021-11-21 : i5-8365U : ~20-25mn (unoptimized pd.DataFrame.apply(axis='columns')-based code)
     # * 2021-11-28 : i7-10850H : ~370ms ! (numpy-optimized column-array-operation-based code)
 
     # iv. Auto-check results (statistically, not always value by value)
     df = results._dfData
+
     # SightRate
     assert df[RS.CLSightRate].isnull().sum() == 40960
     assert df[RS.CLSightRate].value_counts().eq(pd.Series({100: 20480, 50: 20480})).all()
+
     # New quality indicators that should be killed by at least 1 NaN in source results
     miCompCols = [RS.CLKeyFn, RS.CLNAdjPars, RS.CLNTotPars, RS.CLNObs, RS.CLNTotObs,
                   RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw, RS.CLDCv]
     miNewQuaIndCols = [RS.CLCmbQuaBal2, RS.CLCmbQuaBal3, RS.CLCmbQuaChi2, RS.CLCmbQuaKS, RS.CLCmbQuaDCv]
     dfNaNKilledNewQuaIndics = df.loc[df[miCompCols].isnull().any(axis='columns'), miNewQuaIndCols]
     aHist = np.histogram(dfNaNKilledNewQuaIndics, bins=np.linspace(0, 0.15, 16))[0]
     logger.info('Histogram of NaN-killed new Qua Indics: ' + str(aHist))
     assert pd.Series(aHist).eq([378737, 423, 0, 2, 64, 189, 292, 245, 202, 120, 118, 40, 8, 0, 0]).all()
+
     # All quality indicators that were not killed by any NaN in source results
     miQuaIndCols = [RS.CLCmbQuaBal1] + miNewQuaIndCols
     dfNoNaNQuaIndics = df.loc[df[miCompCols].notnull().all(axis='columns'), miQuaIndCols]
     aHist = np.histogram(dfNoNaNQuaIndics, bins=np.linspace(0, 1, 11))[0]
     logger.info('Histogram of no-NaN Qua Indics: ' + str(aHist))
     assert pd.Series(aHist).eq([30788, 876, 0, 77, 403, 800, 918, 735, 339, 56]).all()
+
     # All quality indicators that were not killed by any NaN in source results
     # or 0 in source stat tests results or bad DCv or SightRate or NAdjustParams
     miStatestCols = [RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw]
     dfNotSoBadQuaIndics = df.loc[df[miCompCols].notnull().all(axis='columns')
                                  & df[miStatestCols].gt(0.01).all(axis='columns')
                                  & df[RS.CLDCv].lt(0.3) & df[RS.CLNAdjPars].lt(4)
                                  & (df[RS.CLNObs] / df[RS.CLNTotObs]).gt(0.7), miQuaIndCols]
     aHist = np.histogram(dfNotSoBadQuaIndics, bins=np.linspace(0.3, 1, 8))[0]
     logger.info('Histogram of not-so-bad Qua Indics: ' + str(aHist))
     assert pd.Series(aHist).eq([0, 4, 60, 174, 256, 224, 50]).all()
-    logger.info('Success !')
+
     # v. Done
-    results._dfData  # .to_excel('tmp/_2.xlsx')
+    logger.info('results._dfData: ' + results._dfData.to_string())
+
+    logger.info0('PASS testMcdsArsPostComputeQualityIndicators1: constructor, _postComputeQualityIndicators')
 
 
 # ### f. _postComputeQualityIndicators (and callees)
 # 2/2 Special case, with 1 missing input column, let's say CLCvMUw
 # Note: From far faster, only 72 results to compute
 def testMcdsArsPostComputeQualityIndicators2(mcdsAnalyser_fxt):
     anlr = mcdsAnalyser_fxt
 
     # i. Create empty results
     results = anlr.setupResults()
+
     # ii. Fill it up
     statestRange = [0, 0.5, 1]  # Range for statistic tests
     densCvRange = [0.1, 0.3]  # Range for density coef. of variation
     logger.info('Filling up results to post-compute')
     ldRes = list()
     nObs, nTotObs = 45, 50  # Make tests last less (already tests before)
     # Try all key functions
     for keyFn in ['HNORMAL', 'UNIFORM', 'HAZARD', 'NEXPON']:
-        # CLNTotPars and CLNAdjPars are used independently, no need for combinations)
+        # CLNTotPars and CLNAdjPars are used independently, no need for combinations
         for nPars in [0, 1, 2]:
             # CLNObs and CLNTotObs are always used together, no need for full combination stuff
             for chi2 in statestRange:
                 ks = cvmCw = chi2  # Make tests last less (already tests before)
                 for dcv in densCvRange:
                     ldRes.append({RS.CLKeyFn: keyFn, RS.CLNAdjPars: nPars, RS.CLNTotPars: nPars,
                                   RS.CLNObs: nObs, RS.CLNTotObs: nTotObs,
                                   RS.CLChi2: chi2, RS.CLKS: ks,
                                   RS.CLCvMCw: cvmCw, RS.CLDCv: dcv})  # Note: RS.CLCvMUw is missing
     results._dfData = pd.DataFrame(ldRes)
     results._dfData.columns = pd.MultiIndex.from_tuples(results._dfData.columns)
     logger.info('{} results'.format(len(results._dfData)))
+
     # iii. Post-compute Delta AIC and DeltaDCv
     results._postComputeQualityIndicators()
 
     # iv. Auto-check results (statistically, not value by value)
     df = results._dfData
     # New quality indicators that should be killed because of at least 1 NaN in source results (the missing CLCvMUw)
     miNewQuaIndCols = [RS.CLCmbQuaBal2, RS.CLCmbQuaBal3, RS.CLCmbQuaChi2, RS.CLCmbQuaKS, RS.CLCmbQuaDCv]
     assert df[miNewQuaIndCols].eq(0).all().all()
-    logger.info('Success !')
+
     # v. Done
-    results._dfData  # .to_excel('tmp/_3.xlsx')
+    logger.info('results._dfData: ' + results._dfData.to_string())
+
+    logger.info0('PASS testMcdsArsPostComputeQualityIndicators2: constructor, _postComputeQualityIndicators')
 
 
 # ### g. _sampleDistTruncGroups
 def testMcdsArsSampleDistTruncGroups(mcdsAnalyser_fxt):
     anlr = mcdsAnalyser_fxt
 
     # Load results to play with ...
     # Note: Okay, it's actually an MCDSTruncOptAnalysisResultsSet file ...
     #       but we'll ignore the extra columns, promised :-)
-    resFileName = uivu.pRefInDir / 'ACDC2019-Naturalist-UnitestOptResultats.ods'
+    resFileName = uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-UnitestOptResultats.ods'
     logger.info(f'Loading results from {resFileName.as_posix()} ...')
     results = anlr.setupResults()
     results.fromOpenDoc(resFileName, postComputed=True)  # Prevent re-post-computation : not a problem here, but longer
 
     # Get results table and extract only needed columns (promise fulfilled ;-)
-    # (Note: No post-computed column used here, so ... recomputation authorised, but not needed, and slower)
+    # (Note: No post-computed column used here, so ... re-computation authorised, but not needed, and slower)
     CLSampNum = ('header (head)', 'NumEchant', 'Value')
     dfRes = results.getData(copy=True)[[CLSampNum, RS.CLParTruncLeft, RS.CLParTruncRight]]
     dfRes.head()
 
-    # Test case: a hard-coded extract of once refin/ACDC2019-Naturalist-UnitestOptResultats.ods results file
+    # Test case: a hard-coded extract of once refin/ACDC2019-Naturalist-extrait-UnitestOptResultats.ods results file
     # CLSampNum = ('header (head)', 'NumEchant', 'Value')
     # dfRes = pd.DataFrame(
     #     index=[18, 17, 5, 16, 15, 0, 12, 8, 14, 9, 1, 19, 2, 22, 24, 21, 20, 26, 23, 27, 28, 30, 29, 32, 31,
     #            33, 35, 34, 37, 36, 40, 41, 39, 43, 44, 47, 48, 49, 50, 52, 51, 56, 53, 54, 57, 60, 62, 69,
     #            63, 65, 67, 68, 66, 64],
     #     columns=pd.MultiIndex.from_tuples([CLSampNum, RS.CLParTruncLeft, RS.CLParTruncRight]),
     #     data=[[0, np.nan, np.nan], [0, 10.0, np.nan], [0, np.nan, 280.0], [0, 15.0, 300.0], [0, 20.0, 300.0],
@@ -974,111 +643,121 @@
     #           [4, np.nan, np.nan], [4, 10.0, np.nan], [4, np.nan, 280.0], [4, 15.0, 300.0], [4, np.nan, 731.1],
     #           [4, np.nan, np.nan], [4, 10.0, np.nan], [4, np.nan, 280.0], [4, 15.0, 300.0], [4, np.nan, 477.6],
     #           [5, np.nan, np.nan], [5, 10.0, np.nan], [5, np.nan, 350.0], [5, 15.0, 370.0], [5, np.nan, np.nan],
     #           [5, 10.0, np.nan], [5, np.nan, 350.0], [5, 15.0, 370.0]])
     # dfRes.head()
 
     # Expected results per sample.
-    KDSampGroupNums = \
-    {
+    KDSampGroupNums = {
         0: dict(left={18: 0, 17: 1, 5: 0, 16: 2, 15: 3, 0: 1, 12: 0, 8: 1, 14: 0, 9: 2, 1: 3, 19: 3},
                 right={18: 0, 17: 0, 5: 2, 16: 2, 15: 2, 0: 3, 12: 0, 8: 0, 14: 2, 9: 2, 1: 2, 19: 1}),
         1: dict(left={2: 0, 22: 1, 24: 0, 21: 1, 20: 2, 26: 0, 23: 1, 27: 0, 28: 1, 30: 2},
                 right={2: 0, 22: 0, 24: 1, 21: 1, 20: 1, 26: 0, 23: 0, 27: 1, 28: 1, 30: 1}),
         2: dict(left={29: 0, 32: 0, 31: 0, 33: 0, 35: 0, 34: 0},
                 right={29: 0, 32: 1, 31: 2, 33: 0, 35: 1, 34: 2}),
         3: dict(left={37: 0, 36: 0, 40: 0, 41: 2, 39: 0, 43: 0, 44: 0, 47: 1},
                 right={37: 0, 36: 2, 40: 3, 41: 1, 39: 0, 43: 2, 44: 3, 47: 1}),
         4: dict(left={48: 0, 49: 1, 50: 0, 52: 1, 51: 0, 56: 0, 53: 1, 54: 0, 57: 1, 60: 0},
                 right={48: 0, 49: 0, 50: 1, 52: 1, 51: 3, 56: 0, 53: 0, 54: 1, 57: 1, 60: 2}),
         5: dict(left={62: 0, 69: 1, 63: 0, 65: 1, 67: 0, 68: 1, 66: 0, 64: 1},
                 right={62: 0, 69: 0, 63: 1, 65: 1, 67: 0, 68: 0, 66: 1, 64: 1})
     }
 
+    ldTruncIntrvSpecs = [dict(col='left', minDist=5.0, maxLen=5.0), dict(col='right', minDist=25.0, maxLen=25.0)]
+    truncIntrvEpsilon = 1e-6
+
     dRefGroupNums = dict()  # For building _distTruncGroups reference :-)
     for lblSamp in dfRes[CLSampNum].unique():
 
         logger.debug(f'* {lblSamp}')
         dSampGroupNums = RS._sampleDistTruncGroups(dfRes[dfRes[CLSampNum] == lblSamp],
                                                    ldIntrvSpecs=ldTruncIntrvSpecs, intrvEpsilon=truncIntrvEpsilon)
         assert all(sGroupNums.eq(pd.Series(KDSampGroupNums[lblSamp][colAlias])).all()
                    for colAlias, sGroupNums in dSampGroupNums.items())
 
         for colAlias, sGroupNums in dSampGroupNums.items():
             if colAlias not in dRefGroupNums:
                 dRefGroupNums[colAlias] = sGroupNums
             else:
                 dRefGroupNums[colAlias] = dRefGroupNums[colAlias].append(sGroupNums)
-    logger.info('Success !')
+
+    logger.info0('PASS testMcdsArsSampleDistTruncGroups(1): constructor, getData, fromOpenDoc, _sampleDistTruncGroups')
 
     # Check and build results reference
     # lblSamp = 5
     #
     # df = dfRes[dfRes[CLSampNum] == lblSamp].copy()
     #
     # dGroupNums = RS._sampleDistTruncGroups(df, ldIntrvSpecs=ldIntrvSpecs, intrvEpsilon=intrvEpsilon)
     # for colAlias, sGroupNums in dGroupNums.items():
     #    df[RS.DCLGroupTruncDist[colAlias]] = sGroupNums
-    #    print(colAlias, '=', sGroupNums.to_dict(), ',', sep='')
+    #    logger.info(colAlias, '=', sGroupNums.to_dict(), ',', sep='')
     # df
 
     # ### h. _distTruncGroups
     dGroupNums = results._distTruncGroups()
 
     # Auto-check
     assert all(sGroupNums.eq(dRefGroupNums[colAlias]).all() for colAlias, sGroupNums in dGroupNums.items())
-    logger.info('Success !')
+
+    logger.info0('PASS testMcdsArsSampleDistTruncGroups(2): _distTruncGroups')
 
 
 # ### i. _filterSortKeySchemes
 def testMcdsArsFilterSortKeySchemes(mcdsAnalyser_fxt):
     anlr = mcdsAnalyser_fxt
 
+    # 1. Using predefined filter-sort key generation schemes
     # Load results to play with ...
-    resFileName = 'refin/ACDC2019-Naturalist-UnitestOptResultats.ods'
-    print('Loading results from {} ...'.format(resFileName))
+    resFileName = uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-UnitestOptResultats.ods'
+    logger.info('Loading results from {} ...'.format(resFileName))
     results = anlr.setupResults(ldFilSorKeySchemes=None)  # Will use predefined filter-sort key generation schemes
     results.fromOpenDoc(resFileName, postComputed=True)  # Prevent re-post-computation : not a problem here, but longer
 
     assert results._filterSortKeySchemes() == ads.MCDSAnalysisResultsSet.AutoFilSorKeySchemes
-    logger.info('Success !')
 
+    logger.info0('PASS testMcdsArsFilterSortKeySchemes(predef): constructor, fromOpenDoc, _filterSortKeySchemes')
+
+    # 2. NOT using predefined filter-sort key generation schemes
     # Load results to play with ...
-    resFileName = 'refin/ACDC2019-Naturalist-UnitestOptResultats.ods'
-    print('Loading results from {} ...'.format(resFileName))
+    resFileName = uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-UnitestOptResultats.ods'
+    logger.info('Loading results from {} ...'.format(resFileName))
     ldFilSorKeySchemes = \
         [dict(key=RS.CLGrpOrdClTrChi2KSDCv,
               sort=[RS.CLGroupTruncLeft, RS.CLGroupTruncRight,
                     RS.CLChi2, RS.CLKS, RS.CLDCv, RS.CLNObs, RS.CLRunStatus],
               ascend=[True, True, False, False, True, False, True],
               group=[RS.CLGroupTruncLeft, RS.CLGroupTruncRight]),
          dict(key=RS.CLGblOrdDAicChi2KSDCv,
               sort=[RS.CLParTruncLeft, RS.CLParTruncRight, RS.CLParModFitDistCuts,
                     RS.CLDeltaAic, RS.CLChi2, RS.CLKS, RS.CLDCv, RS.CLNObs, RS.CLRunStatus],
               ascend=[True, True, True, True, False, False, True, False, True], napos='first')]
     results = anlr.setupResults(ldFilSorKeySchemes=ldFilSorKeySchemes)  # Will not use predefined ones.
     results.fromOpenDoc(resFileName, postComputed=True)  # Prevent re-post-computation : not a problem here, but longer
 
     assert results._filterSortKeySchemes() == ldFilSorKeySchemes
-    print('Yessssss !')
+
+    logger.info0('PASS testMcdsArsFilterSortKeySchemes(no predef): constructor, fromOpenDoc, _filterSortKeySchemes')
 
 
 # ### j. _sampleFilterSortKeys
-def testMcdsArsFilterSortKeySchemes(mcdsAnalyser_fxt):
+# ### k. _filterSortKeys
+def testMcdsArsFilterSortKeys(mcdsAnalyser_fxt):
     anlr = mcdsAnalyser_fxt
 
     # Load results to play with ...
-    # Note: Okay, it's actually an MCDSTruncOptAnalysisResultsSet file ... but we'll ignore the extra columns, promised :-)
-    resFileName = 'refin/ACDC2019-Naturalist-UnitestOptResultats.ods'
-    print('Loading results from {} ...'.format(resFileName))
+    # Note: Okay, it's actually an MCDSTruncOptAnalysisResultsSet file ...
+    # but we'll ignore the extra columns, promised :-)
+    resFileName = uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-UnitestOptResultats.ods'
+    logger.info('Loading results from {} ...'.format(resFileName))
     results = anlr.setupResults()
     results.fromOpenDoc(resFileName, postComputed=True)  # Prevent re-post-computation : not a problem here, but longer
 
     # Get results table and extract only needed columns (promise fulfilled ;-)
-    # (Note: No post-computed column used here, so ... recomputation authorised, but not needed, and slower)
+    # (Note: No post-computed column used here, so ... re-computation authorised, but not needed, and slower)
     CLSampNum = ('header (head)', 'NumEchant', 'Value')
     dfRes = results.getData(copy=True)[[CLSampNum, RS.CLParTruncLeft, RS.CLParTruncRight,
                                         RS.CLGroupTruncLeft, RS.CLGroupTruncRight, RS.CLChi2, RS.CLDCv]]
     dfRes.head()
 
     # Expected results per sample.
     CLGrpOrdClTrChi2 = (RS.CLCAutoFilSor, 'Chi2 (close trunc)', RS.CLTSortOrder)
@@ -1109,159 +788,136 @@
               sort=[RS.CLParTruncLeft, RS.CLParTruncRight, RS.CLDCv],
               ascend=[True, True, True], napos='first')]
 
     dRefFilSorKeys = dict()  # For building _filterSortKeys output reference :-)
     for lblSamp in dfRes[CLSampNum].unique():
 
         logger.debug(f'* {lblSamp}')
-        dSampFSKeys = RS._sampleFilterSortKeys(dfRes[dfRes[CLSampNum] == lblSamp], ldFilSorKeySchemes=ldFilSorKeySchemes)
+        dSampFSKeys = RS._sampleFilterSortKeys(dfRes[dfRes[CLSampNum] == lblSamp],
+                                               ldFilSorKeySchemes=ldFilSorKeySchemes)
         assert all(sFSKeys.eq(pd.Series(KDSampFilSorKeys[lblSamp][colLbl])).all()
                    for colLbl, sFSKeys in dSampFSKeys.items())
 
         for colLbl, sFSKeys in dSampFSKeys.items():
             if colLbl not in dRefFilSorKeys:
                 dRefFilSorKeys[colLbl] = sFSKeys
             else:
                 dRefFilSorKeys[colLbl] = dRefFilSorKeys[colLbl].append(sFSKeys)
-    print('Yesssssss !')
+
+    logger.info0('PASS testMcdsArsFilterSortKeys(1): constructor, fromOpenDoc, fromOpenDoc, _sampleFilterSortKeys')
 
     # Check (by eyes) and build material for results reference
     # lblSamp = 5
     # df = dfRes[dfRes[CLSampNum] == lblSamp].copy()
     #
     # dSampFSKeys = RS._sampleFilterSortKeys(df, ldFilSorKeySchemes=ldFilSorKeySchemes)
     # for colLbl, sFSKeys in dSampFSKeys.items():
     #    df[colLbl] = sFSKeys
-    #    print(sFSKeys.to_dict(), ',', sep='')
+    #    logger.info(sFSKeys.to_dict(), ',', sep='')
     #
     # display(df.sort_values(by=[RS.CLGroupTruncLeft, RS.CLGroupTruncRight, RS.CLChi2],
     #                       ascending=[True, True, False]) \
     #         [[RS.CLGroupTruncLeft, RS.CLGroupTruncRight, RS.CLChi2, CLGrpOrdClTrChi2]])
     # display(df.sort_values(by=[RS.CLParTruncLeft, RS.CLParTruncRight, RS.CLDCv],
     #                       ascending=[True, True, True], na_position='first') \
     #         [[RS.CLParTruncLeft, RS.CLParTruncRight, RS.CLDCv, CLGblOrdDCv]])
 
-
-# ### k. _filterSortKeys
-def testMcdsArsFilterSortKeys(mcdsAnalyser_fxt):
-    anlr = mcdsAnalyser_fxt
+    # ### k. _filterSortKeys
 
     # Load results to play with ...
-    # Note: Okay, it's actually an MCDSTruncOptAnalysisResultsSet file ... but we'll ignore the extra columns, promised :-)
-    resFileName = 'refin/ACDC2019-Naturalist-UnitestOptResultats.ods'
-    print('Loading results from {} ...'.format(resFileName))
+    # Note: Okay, it's actually an MCDSTruncOptAnalysisResultsSet file ...
+    #       but we'll ignore the extra columns, promised :-)
+    resFileName = uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-UnitestOptResultats.ods'
+    logger.info('Loading results from {} ...'.format(resFileName))
     # Make test simpler : replace filter and sort key predefined generation scheme set by a shorter one.
-    results = anlr.setupResults(
-        ldFilSorKeySchemes=ldFilSorKeySchemes)  # See f. right above for ldFilSorKeySchemes definition  !
+    results = anlr.setupResults(ldFilSorKeySchemes=ldFilSorKeySchemes)
     results.fromOpenDoc(resFileName, postComputed=True)  # Prevent re-post-computation : not a problem here, but longer
 
     # Get results table and extract only needed columns (promise fulfilled ;-)
-    # (Note: No post-computed column used here, so ... recomputation authorised, but not needed, and slower)
+    # (Note: No post-computed column used here, so ... re-computation authorised, but not needed, and slower)
     CLSampNum = ('header (head)', 'NumEchant', 'Value')
     dfRes = results.getData(copy=True)[[CLSampNum, RS.CLParTruncLeft, RS.CLParTruncRight,
                                         RS.CLGroupTruncLeft, RS.CLGroupTruncRight, RS.CLChi2, RS.CLDCv]]
     dfRes.head()
 
     dFilSorKeys = results._filterSortKeys()
 
     # Auto-check
     assert all(sFSKeys.eq(dRefFilSorKeys[colLbl]).all() for colLbl, sFSKeys in dFilSorKeys.items())
-    logger.info('Success !')
+
+    logger.info0('PASS testMcdsArsFilterSortKeys(2): fromOpenDoc, fromOpenDoc, _filterSortKeys')
 
 
 # ### l. _indexOfDuplicates
 def testMcdsArsIndexOfDuplicates():
     # Test cases
-    df = pd.DataFrame([dict(a=1.000, b=2.00, c=3.0, d='To be kept: first so as a.round(1) == 1.0, whatever c, b == 2'),
-                       dict(a=1.010, b=2.00, c=1.0, d='Duplicate: 2nd so as a.round(1) == 1.0, whatever c, b == 2'),
-                       dict(a=1.049, b=2.00, c=2.0, d='Duplicate: 3rd so as a.round(1) == 1.0, whatever c, b == 2'),
-                       dict(a=1.051, b=2.00, c=2.0, d='To be kept: first so as a.round(1) == 1.1, whatever c, b == 2'),
-                       dict(a=1.060, b=2.00, c=2.0, d='Duplicate: 2nd so as a.round(1) == 1.1, whatever c, b == 2'),
-                       dict(a=1.100, b=2.00, c=4.0, d='Duplicate: 3rd so as a.round(1) == 1.1, whatever c, b == 2'),
-                       dict(a=1.151, b=2.00, c=5.0, d='To be kept: first so as a.round(1) == 1.2, whatever c, b == 2'),
-                       dict(a=2.000, b=2.00, c=3.0, d='To be kept: first so as b == 2.0, whatever c, a == 2'),
-                       dict(a=2.000, b=2.00, c=5.0, d='Duplicate: 2nd so as b == 2.0, whatever c, a == 2'),
-                       dict(a=2.000, b=2.01, c=9.0, d='To be kept: first so as b == 2.0, whatever c, a == 2'),
-                       dict(a=2.000, b=1.9999999, c=3.0, d='To be kept: first so as b == 1.9999999, whatever c, a == 2')])
+    df = pd.DataFrame(
+        [dict(a=1.000, b=2.00, c=3.0, d='To be kept: first so as a.round(1) == 1.0, whatever c, b == 2'),
+         dict(a=1.010, b=2.00, c=1.0, d='Duplicate: 2nd so as a.round(1) == 1.0, whatever c, b == 2'),
+         dict(a=1.049, b=2.00, c=2.0, d='Duplicate: 3rd so as a.round(1) == 1.0, whatever c, b == 2'),
+         dict(a=1.051, b=2.00, c=2.0, d='To be kept: first so as a.round(1) == 1.1, whatever c, b == 2'),
+         dict(a=1.060, b=2.00, c=2.0, d='Duplicate: 2nd so as a.round(1) == 1.1, whatever c, b == 2'),
+         dict(a=1.100, b=2.00, c=4.0, d='Duplicate: 3rd so as a.round(1) == 1.1, whatever c, b == 2'),
+         dict(a=1.151, b=2.00, c=5.0, d='To be kept: first so as a.round(1) == 1.2, whatever c, b == 2'),
+         dict(a=2.000, b=2.00, c=3.0, d='To be kept: first so as b == 2.0, whatever c, a == 2'),
+         dict(a=2.000, b=2.00, c=5.0, d='Duplicate: 2nd so as b == 2.0, whatever c, a == 2'),
+         dict(a=2.000, b=2.01, c=9.0, d='To be kept: first so as b == 2.0, whatever c, a == 2'),
+         dict(a=2.000, b=1.9999999, c=3.0, d='To be kept: first so as b == 1.9999999, whatever c, a == 2')])
 
     # Compute filter
     iDupes = RS._indexOfDuplicates(df, keep='first', subset=['a', 'b'], round2decs=dict(a=1))
-    iDupes
+    logger.info('iDupes: ' + str(iDupes))
 
     # Apply filter
     df.drop(iDupes, inplace=True)
-    df
+    logger.info('df: ' + df.to_string())
 
     # Auto-check
     assert all(iDupes == [1, 2, 4, 5, 8])
     assert all('Duplicate' not in s for s in df.d)
-    logger.info('Success !')
+
+    logger.info0('PASS testMcdsArsIndexOfDuplicates: _indexOfDuplicates')
 
 
 # ### m. _indexOfWorstOneCriterion
 def testMcdsArsIndexOfWorstOneCriterion():
     # Test cases
-    df = pd.DataFrame([dict(s=0, a=1.000),
-                       dict(s=0, a=0.010),
-                       dict(s=0, a=1.049),
-                       dict(s=0, a=1.051),
-                       dict(s=0, a=0.060),
-                       dict(s=0, a=1.100),
-                       dict(s=0, a=1.151),
-                       dict(s=0, a=2.000),
-                       dict(s=0, a=1.020),
-                       dict(s=0, a=1.500),
-                       dict(s=0, a=2.000),
-                       dict(s=0, a=1.010),
-                       dict(s=0, a=1.049),
-                       dict(s=0, a=0.051),
-                       dict(s=1, a=1.060),
-                       dict(s=1, a=1.100),
-                       dict(s=1, a=1.151),
-                       dict(s=2, a=3.000),
-                       dict(s=2, a=2.000),
-                       dict(s=2, a=6.000),
-                       dict(s=2, a=0.060),
-                       dict(s=2, a=1.100),
-                       dict(s=2, a=3.010),
-                       dict(s=2, a=2.200),
-                       dict(s=2, a=2.230),
-                       dict(s=3, a=1.100),
-                       dict(s=3, a=1.151),
-                       dict(s=3, a=2.000),
-                       dict(s=3, a=2.000),
-                       dict(s=4, a=2.000),
-                       dict(s=4, a=2.000),
-                       dict(s=4, a=2.000),
-                       dict(s=4, a=2.000),
-                       dict(s=4, a=2.000),
-                       dict(s=4, a=2.000)])
+    df = pd.DataFrame([dict(s=0, a=1.000), dict(s=0, a=0.010), dict(s=0, a=1.049), dict(s=0, a=1.051),
+                       dict(s=0, a=0.060), dict(s=0, a=1.100), dict(s=0, a=1.151), dict(s=0, a=2.000),
+                       dict(s=0, a=1.020), dict(s=0, a=1.500), dict(s=0, a=2.000), dict(s=0, a=1.010),
+                       dict(s=0, a=1.049), dict(s=0, a=0.051), dict(s=1, a=1.060), dict(s=1, a=1.100),
+                       dict(s=1, a=1.151), dict(s=2, a=3.000), dict(s=2, a=2.000), dict(s=2, a=6.000),
+                       dict(s=2, a=0.060), dict(s=2, a=1.100), dict(s=2, a=3.010), dict(s=2, a=2.200),
+                       dict(s=2, a=2.230), dict(s=3, a=1.100), dict(s=3, a=1.151), dict(s=3, a=2.000),
+                       dict(s=3, a=2.000), dict(s=4, a=2.000), dict(s=4, a=2.000), dict(s=4, a=2.000),
+                       dict(s=4, a=2.000), dict(s=4, a=2.000), dict(s=4, a=2.000)])
     s2filter = [0, 2, 3, 5]  # Ignore sample 1 and 4, add empty sample 5
     maxRes = 6  # Keep 6 best values at most.
 
     df.s.value_counts().sort_index()
 
     # df.sort_values(by=['s', 'a'])
 
     # Compute filter
     i2drop = RS._indexOfWorstOneCriterion(df, sampleIds=s2filter, sampleIdCol='s', critCol='a', ascendCrit=False,
                                           nTgtRes=maxRes)
-    i2drop
+    logger.info('i2drop: ' + str(i2drop))
 
     # Apply filter
     df.drop(i2drop, inplace=True)
     df.sort_values(by=['s', 'a'])
 
     df.s.value_counts().sort_index()
 
     # Auto-check
     assert all(i2drop == [2, 12, 8, 11, 0, 4, 13, 1, 21, 20])
     assert df[df.s.isin(s2filter)].s.value_counts().le(maxRes).all()
     assert df.loc[df.s.isin(s2filter)].groupby('s').a.max().le([2, 6, 2]).all()
-    logger.info('Success !')
+
+    logger.info0('PASS testMcdsArsIndexOfWorstOneCriterion: _indexOfWorstOneCriterion')
 
 
 # ### n. _indexOfWorstMultiOrderCriteria
 def testMcdsArsIndexOfWorstMultiOrderCriteria():
     # Test cases
     df = pd.DataFrame([dict(s=0, a=1, b=1, c='Kept thanks to a and b'),
                        dict(s=0, a=0, b=1, c='Kept thanks to a and b'),
@@ -1270,32 +926,32 @@
                        dict(s=0, a=3, b=2, c='Dropped because of a and b'),
                        dict(s=0, a=5, b=1, c='Kept thanks to b'),
                        dict(s=1, a=2, b=4, c='Dropped because of a and b'),
                        dict(s=1, a=1, b=3, c='Kept thanks to a'),
                        dict(s=1, a=4, b=0, c='Kept thanks to b')])
     critCols = ['a', 'b']
     supCrit = 2
-    df
+    logger.info('df: ' + df.to_string())
 
     i2drop = RS._indexOfWorstMultiOrderCriteria(df, critCols=critCols, supCrit=supCrit)
-    i2drop
+    logger.info('i2drop: ' + str(i2drop))
 
     # Apply filter
     df.drop(i2drop, inplace=True)
     df.sort_values(by=['s', 'a'])
 
     # Auto-check
     assert all(i2drop == [2, 3, 4, 6])
     assert all('Dropped' not in s for s in df.c)
-    logger.info('Success !')
+
+    logger.info0('PASS testMcdsArsIndexOfWorstMultiOrderCriteria: _indexOfWorstMultiOrderCriteria')
 
 
 # ### o. filSorSchemeId
 def testMcdsArsFilSorSchemeId():
-    RS = ads.MCDSAnalysisResultsSet
 
     fsRes = ads.MCDSAnalysisResultsSet(sampleIndCol='Sample')
 
     dupSubset = [RS.CLNObs, RS.CLEffort, RS.CLDeltaAic, RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw, RS.CLDCv,
                  RS.CLPDetec, RS.CLPDetecMin, RS.CLPDetecMax, RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax]
     dDupRounds = {RS.CLDeltaAic: 1, RS.CLChi2: 2, RS.CLKS: 2, RS.CLCvMUw: 2, RS.CLCvMCw: 2, RS.CLDCv: 2,
                   RS.CLPDetec: 3, RS.CLPDetecMin: 3, RS.CLPDetecMax: 3, RS.CLDensity: 2, RS.CLDensityMin: 2,
@@ -1327,46 +983,17 @@
     assert fsRes.filSorSchemeId(schACCQ5).startswith(fsRes.filSorSchemeId(schACCQ1))
     logger.info('Success !')
 
     dict(schEx=fsRes.filSorSchemeId(schEx), schACCQ1=fsRes.filSorSchemeId(schACCQ1),
          schACCQ2=fsRes.filSorSchemeId(schACCQ2), schACCQ3=fsRes.filSorSchemeId(schACCQ3),
          schACCQ4=fsRes.filSorSchemeId(schACCQ4), schACCQ5=fsRes.filSorSchemeId(schACCQ5))
 
+    logger.info0('PASS testMcdsArsFilSorSchemeId: constructor, filSorSchemeId')
+
 
 ###############################################################################
 #                         Actions to be done after all tests                  #
 ###############################################################################
 def testEnd():
-    uivu.logEnd(what=what2Test)
-
-
-# This pytest-compatible module can also be run as a simple python script.
-if __name__ == '__main__':
-
-    run = True
-    # Run auto-tests (exit(0) if OK, 1 if not).
-    rc = -1
-
-    uivu.logBegin(what=what2Test)
-
-    if run:
-        try:
-            # Let's go.
-            testBegin()
-
-            # Tests for AnalysisResultsSet
-            testDataSetCtorLen(sources())
-
-
-            # Done.
-            testEnd()
-
-            # Success !
-            rc = 0
-
-        except Exception as exc:
-            logger.exception('Exception: ' + str(exc))
-            rc = 1
-
-    uivu.logEnd(what=what2Test, rc=rc)
-
-    sys.exit(rc)
+    # if KFinalCleanup:
+    #     uivu.cleanupWorkDir()
+    uivu.logEnd(what=KWhat2Test)
```

### Comparing `pyaudisam-1.0.2/tests/unint_data_test.py` & `pyaudisam-1.1.0/tests/test_unint_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 # coding: utf-8
 
 # PyAuDiSam: Automation of Distance Sampling analyses with Distance software (http://distancesampling.org/)
 
-# Copyright (C) 2021 Jean-Philippe Meuret, Sylvain Sainnier
+# Copyright (C) 2021 Sylvain Sainnier, Jean-Philippe Meuret
 
 # This program is free software: you can redistribute it and/or modify it under the terms
 # of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 
 # Automated unit and integration tests for "data" submodule
 
-# To run : simply run "pytest" or "python <this file>" in current folder
-#          and check standard output ; and ./tmp/unt-dat.{datetime}.log for details
+# To run : simply run "pytest" and check standard output + ./tmp/unt-dat.{datetime}.log for details
 
-import sys
 import time
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 
 import pytest
 
 import pyaudisam as ads
 
 import unintval_utils as uivu
 
 
+# Mark module
+pytestmark = pytest.mark.unintests
+
 # Setup local logger.
 logger = uivu.setupLogger('unt.dat', level=ads.DEBUG,
                           otherLoggers={'ads.eng': ads.INFO2, 'ads.dat': ads.INFO})
 
-what2Test = 'data'
+# Set to False to skip final cleanup (useful for debugging)
+KFinalCleanup = True
+
+KWhat2Test = 'data'
+
 
 ###############################################################################
 #                         Actions to be done after all tests                  #
 ###############################################################################
 def testBegin():
-    uivu.logBegin(what=what2Test)
+    uivu.logBegin(what=KWhat2Test)
+    uivu.setupWorkDir('unt-data')
 
 
 ###############################################################################
 #                         Input Data Preparation                              #
 ###############################################################################
 #   Generate DataFrame (returned) and other format files  from .ods source
 #   and return a list of sources (4 files and 1 DataFrame)
 def sources():
 
     dfPapAlaArv = pd.read_excel(uivu.pRefInDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.ods')
 
-    dfPapAlaArv.to_csv(uivu.pTmpDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.csv', sep='\t', index=False)
-    dfPapAlaArv.to_excel(uivu.pTmpDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xls', index=False)
+    dfPapAlaArv.to_csv(uivu.pWorkDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.csv', sep='\t', index=False)
+    dfPapAlaArv.to_excel(uivu.pWorkDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xls', index=False)
 
     # DataSet from multiple sources from various formats (same columns).
     # For test, list of require to contain 1 DataFrame, and one or several
     # source files (one for each different extension)
     # DataFrame and all files need to contain the same data
     srcs = [uivu.pRefInDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.ods',  # Need for module odfpy
             uivu.pRefInDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xlsx',  # Need for module openpyxl (or xlrd)
-            uivu.pTmpDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xls',  # No need for xlwt(openpyxl seems OK)
-            uivu.pTmpDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.csv',
+            uivu.pWorkDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xls',  # No need for xlwt(openpyxl seems OK)
+            uivu.pWorkDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.csv',
             dfPapAlaArv]
     return srcs
 
 
 # same as above => to allow using pytest
 @pytest.fixture
 def sources_fxt():
@@ -204,16 +210,16 @@
         ' Issue occurred with process of adding a new AND computed column.'
 
     # Checking adding a new column with computing process and rename it
     #   a new column also added to prepare following test step
     ds = ads.DataSet(sources_fxt, dRenameCols={'MALE': 'SEXE'},
                      dComputeCols={'MALE': sex2bool, 'NEWCOL': ''},
                      sheet='Sheet1', skipRows=None, separator='\t')
-    print(ds.columns)
-    print(ds.dfData.SEXE)
+    logger.info('ds.columns: ' + str(ds.columns))
+    logger.info('ds.dfData.SEXE: ' + str(ds.dfData.SEXE))
     assert ds.dfData['SEXE'].dtype == bool, \
         'Error: testDataSetAddComputedColumns: Issue occurred with process of adding' \
         ' and renaming a new AND computed column.'
 
     logger.info0('PASS (testDataSetAddComputedColumns) => DATASET => methods "addColumns" and "_addComputedColumns":\n'
                  + '\t'*5 + 'addition, recomputing, and combination addition/recomputing'
                  + ' for existing or new column checked\n'
@@ -342,21 +348,21 @@
                      sheet='Sheet1', skipRows=None, separator='\t')
     ds.dropColumns(['ZONE', 'HA', 'OBSERVATEUR'])
     ds.dropRows(ds.dfData.DISTANCE.isnull())
     
     # => toExcel, toOpenDoc, toPickle, compareDataFrames
     closenessThreshold = 15  # => max relative delta = 1e-15
     subsetCols = ['POINT', 'ESPECE', 'DISTANCE', 'INDIVIDUS', 'EFFORT']
-    filePathName = uivu.pTmpDir / 'dataset-uni.ods'
+    filePathName = uivu.pWorkDir / 'dataset-uni.ods'
     dfRef = ds.dfSubData(columns=subsetCols).reset_index(drop=True)
 
     for fpn in [filePathName, filePathName.with_suffix('.xlsx'), filePathName.with_suffix('.xls'),
                 filePathName.with_suffix('.pickle'), filePathName.with_suffix('.pickle.xz')]:
 
-        print(fpn.as_posix(), end=' : ')
+        logger.info(fpn.as_posix() + ' : ')
         if fpn.suffix == '.ods':
             ds.toOpenDoc(fpn, sheetName='utest', subset=subsetCols, index=False)
         elif fpn.suffix in ['.xlsx', '.xls']:
             ds.toExcel(fpn, sheetName='utest', subset=subsetCols, index=False)
         elif fpn.suffix in ['.pickle', '.xz']:
             ds.toPickle(fpn, subset=subsetCols, index=False)
         assert fpn.is_file(), 'Error: testDataSetToFiles'
@@ -367,17 +373,16 @@
             df = pd.read_pickle(fpn)
             df.reset_index(drop=True, inplace=True)
         else:
             raise Exception(f'No test for this input file format {fpn.as_posix()}')
         assert ds.compareDataFrames(df.reset_index(), dfRef.reset_index(),
                                     subsetCols=['POINT', 'DISTANCE', 'INDIVIDUS', 'EFFORT'],
                                     indexCols=['index'], dropCloser=closenessThreshold, dropNans=True).empty
-        print('1e-{} comparison OK (df.equals(dfRef) is {}, df.compare(dfRef) {}empty)'
-              .format(closenessThreshold, df.equals(dfRef), '' if df.compare(dfRef).empty else 'not')), \
-            'Error: testDataSetToFiles'
+        logger.info('1e-{} comparison OK (df.equals(dfRef) is {}, df.compare(dfRef) {}empty)'
+                    .format(closenessThreshold, df.equals(dfRef), '' if df.compare(dfRef).empty else 'not'))
 
     logger.info0('PASS (testDataSetToFiles) => DATASET => method "toExcel",'
                  ' "toOpenDoc", "toPickle", "compareDataFrames"')
 
 
 # Test of the base function for comparison (test from static hard-coded data, not from loaded DataSets)
 # method "_closeness" used for
@@ -391,15 +396,15 @@
     aClose = np.ndarray(shape=(len(values), len(values)))
 
     for r in range(len(values)):
         for c in range(len(values)):
             try:
                 aClose[r, c] = ds._closeness(pd.Series([values[r], values[c]]))
             except Exception as e:
-                print(e, r, c, values[r], values[c])
+                logger.info(f'{e} {r}, {c}, {values[r]}, {values[c]}')
                 raise
 
     # Infinite closeness on the diagonal (except for nan and +/-inf)
     assert all(np.isnan(values[i]) or np.isinf(values[i]) or np.isinf(aClose[i, i]) for i in range(len(values))), \
            'Error: testDataSetCloseness: Inequality on the diagonal'
 
     # No infinite proximity elsewhere
@@ -429,15 +434,15 @@
                 + [('sample', col, 'Value') for col in ['Species', 'Periods', 'Prec.', 'Duration']] \
                 + [('model', 'Model', 'Value')] \
                 + [('parameters', 'left truncation distance', 'Value'),
                    ('parameters', 'right truncation distance', 'Value'),
                    ('parameters', 'model fitting distance cut points', 'Value'),
                    ('parameters', 'distance discretisation cut points', 'Value')]
 
-    # # c. Columns to be compared (DeltaDCV and DeltaAIC were removed as results depend on a set of ran analyses,
+    # # c. Columns to be compared (DeltaDCV and DeltaAIC were removed as results depend on a set of run analyses,
     # #    different between reference and PyAuDiSam run).
     subsetCols = [col for col in dsDist.dfData.columns.to_list()
                   if col not in indexCols + [('run output', 'run time', 'Value'),
                                              ('density/abundance', 'density of animals', 'Delta Cv'),
                                              ('detection probability', 'Delta AIC', 'Value')]]
 
     # # d. "Exact" Comparison : no line pass (majority of epsilons due to IO ODS)
@@ -447,22 +452,24 @@
         ' of both DataSets should fail for all rows.'
 
     # # e. Comparison with 10**-16 accuracy : almost all lines pass, but 3 (majority of epsilons due to IO ODS)
     dfRelDiff = dsDist.compare(dsAuto, subsetCols=subsetCols, indexCols=indexCols, dropCloser=16, dropNans=True)
     assert len(dfRelDiff) == 3, \
         'Error: testCompare: compare: Issue occurred. Row by row comparison of both DataSet' \
         ' with accuracy of 10**-16 should fail for all rows but 3.'
-    print(dfRelDiff)
+    logger.info('dfRelDiff:' + dfRelDiff.to_string())
 
     # # e. Comparison with 10**-5 accuracy : all lines pass
     dfRelDiff = dsDist.compare(dsAuto, subsetCols=subsetCols, indexCols=indexCols, dropCloser=5, dropNans=True)
     assert len(dfRelDiff) == 2, \
         'Error: testCompare: compare: Issue occurred. Row by row comparison of both DataSet' \
         'with accuracy of 10**5 should pass for all rows.'
 
+    # # f. TODO: Comparison with noneIsNan=True
+
     logger.info0('PASS (testCompare) => DATASET => method "_closeness" and "compare"')
 
 
 # SAMPLEDATASET TESTS
 # test methods "toExcel", "toOpenDoc", "toPickle", "compareDataFrames"
 def testSDSCtor():
     # test: creation of SDS from DataFrame source.
@@ -571,20 +578,20 @@
 
 KFdsCountCols = ['nMalAd10', 'nAutAd10', 'nMalAd5', 'nAutAd5']
 
 
 def testFieldDataSet():
 
     # ### a. Load data sample
-    dfObs = pd.read_csv('refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt', sep='\t', decimal=',')
+    dfObs = pd.read_csv(uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt', sep='\t', decimal=',')
     dfObs.head()
 
     sCounts = dfObs[KFdsCountCols].sum()
 
-    logger.info('Data sample: len={len(dfObs)}, sums={sCounts.to_dict()}')
+    logger.info(f'Data sample: len={len(dfObs)}, sums={sCounts.to_dict()}')
 
     assert len(dfObs) == 724
     assert not any(sCounts - pd.Series({'nMalAd10': 613, 'nAutAd10': 192, 'nMalAd5': 326, 'nAutAd5': 102}))
 
     # ### b. FieldDataSet._separateMultiCategoryCounts
     dfObsMonoCat_ = ads.FieldDataSet._separateMultiCategoryCounts(dfObs, KFdsCountCols)
     len(dfObsMonoCat_), dfObsMonoCat_[KFdsCountCols].sum()
@@ -642,15 +649,15 @@
 
     logger.info('dfObsIndiv head: ' + dfObsIndiv.head().to_string())
     assert (dfObsIndiv == dfObsIndiv_).all().all()
 
     logger.info0('PASS (testFieldDataSet) => individualise')
 
     # Second, try from source CSV file
-    fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt',
+    fds = ads.FieldDataSet(source=uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt',
                            importDecFields=['distMem'], countCols=KFdsCountCols,
                            addMonoCatCols={'Adulte': count2AdultCat, 'Durée': count2DurationCat})
 
     dfObsIndiv = fds.individualise()
 
     logger.info('dfObsIndiv head: ' + dfObsIndiv.head().to_string())
 
@@ -661,15 +668,15 @@
 
 # ## 7. Class MonoCategoryDataSet (and base DataSet)
 # Note: For real unit tests of DataSet, see `visionat` module:
 # it defines the same class (have to be the same: check it !)
 def testMonoCategoryDataSet():
 
     # Setup source FDS
-    fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt',
+    fds = ads.FieldDataSet(source=uivu.pRefInDir / 'ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt',
                            importDecFields=['distMem'], countCols=KFdsCountCols,
                            addMonoCatCols={'Adulte': count2AdultCat, 'Durée': count2DurationCat})
 
     dfObsIndiv = fds.individualise()
 
     # Drop now unneeded count columns (only 0 or 1 inside + columns Adulte and Duree to explain what a 1 means)
     # No more need for count cols then (only 0 or 1 inside + columns Adulte and Duree to explain what 1 means)
@@ -791,71 +798,21 @@
                                                                        effortCol='Effort')
                     try:
                         dfObsIndivAbscSmpl_ = \
                             ads.MonoCategoryDataSet._addAbsenceSightings(dfObsIndivSmpl, sampleCols, dfTrPassEffSmpl)
                         logger.info(f'{esp}, {pas}, {ad}, {dur}: {len(dfObsIndivSmpl)}'
                                     f' => {len(dfObsIndivAbscSmpl_)}')
                     except Exception as e:
-                        print(e)
+                        logger.exception(e)
     end = time.perf_counter()
     logger.info(f'Elapsed time: {end - start}')
 
     logger.info0('PASS (testMonoCategoryDataSet) => performance: _selectSampleSightings + _addAbsenceSightings')
 
 
 ###############################################################################
 #                         Actions to be done after all tests                  #
 ###############################################################################
 def testEnd():
-    uivu.logEnd(what=what2Test)
-
-
-# This pytest-compatible module can also be run as a simple python script.
-if __name__ == '__main__':
-
-    run = True
-
-    # Run auto-tests (exit(0) if OK, 1 if not).
-    rc = -1
-
-    uivu.logBegin(what=what2Test)
-
-    if run:
-        try:
-            # Let's go.
-            testBegin()
-
-            # Tests for DataSet
-            testDataSetCtorLen(sources())
-            testDataSetDfData(sources())
-            testDataSetEmpty()
-            testDataSetColumns(sources())
-            testDataSetRenameColumns(sources())
-            testDataSetAddComputedColumns(sources())
-            testDataSetDropColumns(sources())
-            testDataSetDfSubData(sources())
-            testDataSetDropRows(sources())
-            testDataSetToFiles(sources())
-            testDataSetCloseness()
-            testDataSetCompare()
-
-            # Tests for other XxxDataSet
-            testSDSCtor()
-            testFieldDataSet()
-            testMonoCategoryDataSet()
-
-            # Tests for ResultsSet
-            # => See unint_analyser_results_test and unint_optanalyser_results_test
-
-            # Done.
-            testEnd()
-
-            # Success !
-            rc = 0
-
-        except Exception as exc:
-            logger.exception(f'Exception: {exc}')
-            rc = 1
-
-    uivu.logEnd(what=what2Test, rc=rc)
-
-    sys.exit(rc)
+    if KFinalCleanup:
+        uivu.cleanupWorkDir()
+    uivu.logEnd(what=KWhat2Test)
```

### Comparing `pyaudisam-1.0.2/tests/unint_engine_test.py` & `pyaudisam-1.1.0/tests/test_unint_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 
 # Automated unit and integration tests for "engine" submodule
 
-# To run : simply run "pytest" or "python <this file>" in current folder
-#          and check standard output ; and tmp/unt-eng.{datetime}.log for details
+# To run : simply run "pytest" and check standard output + tmp/unt-eng.{datetime}.log for details
 
-import sys
 import io
 import re
 import time
 import concurrent.futures as cofu
 import shutil
 import pathlib as pl
 
@@ -31,79 +29,133 @@
 import pytest
 
 import pyaudisam as ads
 
 import unintval_utils as uivu
 
 
+# Mark module
+pytestmark = pytest.mark.unintests
+
 # Setup local logger.
-logger = uivu.setupLogger('unt.eng', level=ads.DEBUG,
-                          otherLoggers={'ads.dat': ads.INFO})
+logger = uivu.setupLogger('unt.eng', level=ads.DEBUG, otherLoggers={'ads.dat': ads.INFO})
+
+# Set to False to skip final cleanup (useful for debugging)
+KFinalCleanup = True
 
-what2Test = 'engine'
+KWhat2Test = 'engine'
 
 
 ###############################################################################
 #                         Actions to be done before any test                  #
 ###############################################################################
 def testBegin():
-    uivu.logBegin(what=what2Test)
+    uivu.logBegin(what=KWhat2Test)
+    uivu.setupWorkDir('unt-eng')
 
 
 ###############################################################################
 #                Test function and related tooling functions                  #
 ###############################################################################
-def testDsExecutableNotFound():
+def testDsFindExecutable():
 
-    with pytest.raises(Exception) as e_info:
-        ads.MCDSEngine().findExecutable('WrongName')
-    logger.info0(f'PASS (test_executableNotFound) => EXCEPTION RAISED AS AWAITED:\n{e_info.value}')
+    with pytest.raises(OSError) as exc_info:
+        ads.DSEngine.findExecutable('WrongName', ads.MCDSEngine._ExeFileSearchPaths)
+    logger.info0(f'PASS testDsFindExecutable: Exception raised as awaited: {exc_info}')
+
+
+def testMcdsStatSpecs():
+
+    KRebuildRef = False  # Should normally be False, unless if you want to rebuild the ref. specs.
+
+    # Load module and statistic specs.
+    E = ads.MCDSEngine
+    dfStatRowSpecs = E.statRowSpecs()
+    logger.info('statRowSpecs:\n' + dfStatRowSpecs.to_string(min_rows=20, max_rows=20))
+
+    dfStatModSpecs = E.statModSpecs()
+    logger.info('statModSpecs:\n' + dfStatModSpecs.to_string(min_rows=90, max_rows=90))
+
+    dfStatModCols = E.statModCols().to_frame().reset_index(drop=True)
+    logger.info('statModCols:\n' + dfStatModCols.to_string(min_rows=150, max_rows=150))
+
+    dfStatModColTrans = E.statModColTrans()
+    logger.info('statModColTrans:\n' + dfStatModColTrans.to_string(min_rows=90, max_rows=90))
+
+    dfStatModNotes = E.statModNotes()
+    logger.info('statModNotes:\n' + dfStatModNotes.to_string(min_rows=20, max_rows=20))
+
+    # If specified, rebuild reference specs (when ABSOLUTELY certain that this IS a correct reference update !)
+    # and force the test to fail, to enforce this important check ! Then set KRebuildRef to False, and rerun test.
+    if KRebuildRef:
+        with pd.ExcelWriter(uivu.pRefOutDir / 'mcds-stat-specs.ods', engine='odf') as wbWrtr:
+            dfStatRowSpecs.reset_index().to_excel(wbWrtr, sheet_name='statRowSpecs', index=False)
+            dfStatModSpecs.reset_index().to_excel(wbWrtr, sheet_name='statModSpecs', index=False)
+            dfStatModCols.to_excel(wbWrtr, sheet_name='statModCols', index=False)
+            dfStatModColTrans.reset_index().to_excel(wbWrtr, sheet_name='statModColTrans', index=False)
+            dfStatModNotes.reset_index().to_excel(wbWrtr, sheet_name='statModNotes', index=False)
+        raise ValueError('testMcdsStatSpecs: reference rebuilt, did you mean it ? If so, inhibit it and rerun test')
+
+    # Compare to reference specs.
+    ddfStatSpecs = pd.read_excel(uivu.pRefOutDir / 'mcds-stat-specs.ods', sheet_name=None)
+    assert dfStatRowSpecs.reset_index().equals(ddfStatSpecs['statRowSpecs'])
+    assert dfStatModSpecs.reset_index().equals(ddfStatSpecs['statModSpecs'].fillna(''))
+    assert dfStatModCols.equals(ddfStatSpecs['statModCols'])
+    assert dfStatModColTrans.reset_index().equals(ddfStatSpecs['statModColTrans'])
+    assert dfStatModNotes.reset_index().equals(ddfStatSpecs['statModNotes'])
+
+    logger.info0('PASS testMcdsStatSpecs: class methods loadStatSpecs,'
+                 ' statRowSpecs, statModSpecs, statModCols, statModNotes, statModColTrans')
 
 
 def testMcdsCtor():
 
     # test Exception raising with one of unsupported characters in workdir string (space) - first way
-    with pytest.raises(Exception) as e_info:
-        ads.MCDSEngine(workDir=uivu.pTmpDir.as_posix() + '/test out')  # Simple string path
-    logger.info0(f'PASS (test_MCDS_Ctor) => EXCEPTION RAISED AS AWAITED:\n{e_info.value}')
+    with pytest.raises(Exception) as exc_info:
+        ads.MCDSEngine(uivu.pWorkDir.as_posix() + '/test out')  # Simple string path
+    logger.info0(f'PASS testMcdsCtor: Exception raised as awaited: {exc_info}')
 
     # test Exception raising with one of unsupported characters in workdir string (space) - second way
-    with pytest.raises(Exception) as e_info:
-        ads.MCDSEngine(workDir=uivu.pTmpDir / 'test out')  # pl.Path path
-    logger.info0(f'PASS (test_MCDS_Ctor) => EXCEPTION RAISED AS AWAITED:\n{e_info.value}')
+    with pytest.raises(Exception) as exc_info:
+        ads.MCDSEngine(workDir=uivu.pWorkDir / 'test out')  # pl.Path path
+    logger.info0(f'PASS testMcdsCtor: Exception raised as awaited: {exc_info}')
 
     # test preferred method to initiate MCDSEngine
-    assert ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out', runMethod='os.system'), \
+    assert ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out', runMethod='os.system'), \
            'MCDS Engine: Non identified issue at engine initiation'
 
     # test previous (older) method to initiate MCDSEngine
-    assert ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out'), 'MCDS Engine: Non identified issue at engine initiation'
+    assert ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out'), 'MCDS Engine: Non identified issue at engine initiation'
 
     # test Specs DataFrames not empty
     # TODO: improve for deeper test ???
-    assert not any([ads.MCDSEngine().statRowSpecs().empty, ads.MCDSEngine().statModSpecs().empty,
-                    ads.MCDSEngine().statModCols().empty, ads.MCDSEngine().statModNotes().empty,
-                    ads.MCDSEngine().statModColTrans().empty]), \
+    assert not any([ads.MCDSEngine.statRowSpecs().empty, ads.MCDSEngine.statModSpecs().empty,
+                    ads.MCDSEngine.statModCols().empty, ads.MCDSEngine.statModNotes().empty,
+                    ads.MCDSEngine.statModColTrans().empty]), \
         'Specs DataFrames: issue occurred with initialization from external files'
 
-    logger.info0('PASS => MCDSEngine => Constructor and methods "_run", "_runThroughOSSystem",'
-                 ' "_runThroughSubProcessRun", "loadStatSpecs" and setters for related class variables')
+    logger.info0('PASS testMcdsCtor: Constructor, _run, _runThroughOSSystem,'
+                 ' _runThroughSubProcessRun, loadStatSpecs, setters')
 
 
 def testDsSetupRunFolder():
 
+    # i. Non-empty run prefix with spaces and special chars
     runDir = ads.MCDSEngine().setupRunFolder(runPrefix=' t,e.s:t; ( )_setupRunFolder')
-
     assert not re.search('[ ,.:;()/]', str(runDir)), \
         'Error: test_MCDS_setupRunFolder: Setup directory: unsupported chars should have been cleaned up'
     assert runDir.exists(), 'Error: test_MCDS_setupRunFolder: temporary directory not created'
-    # clean-up: tmp directory deleted
-    runDir.rmdir()
+    runDir.rmdir()  # clean-up
 
-    logger.info0('PASS => MCDSEngine => method "setupRunFolder"')
+    # ii. Empty run prefix
+    runDir = ads.MCDSEngine().setupRunFolder()
+    assert runDir.exists(), 'Error: testDsSetupRunFolder: temporary directory not created'
+    runDir.rmdir()  # clean-up
+
+    logger.info0('PASS testDsSetupRunFolder: setupRunFolder')
 
 
 # Generate a DataFrame (returned) suite bale for creating a short SampleDataSet
 def dfShortSdsData():
 
     dfData = pd.DataFrame(columns=['Date', 'TrucDec', 'Espece', 'Point', 'Effort', 'Distance'],
                           data=[('2019-05-13', 3.5, 'TURMER', 23, 2, 83),
@@ -127,17 +179,17 @@
 def testMcdsBuildExportTable(dfShortSdsData_fxt):
 
     eng = ads.MCDSEngine()
     dfData = dfShortSdsData_fxt  # load source test data
     dfData.drop(['Surface'], axis=1, inplace=True)  # to create missing field
 
     # test exception raised if at least one field missing vs DSEngine.ImportFieldAliasREs
-    with pytest.raises(Exception) as e_info:
+    with pytest.raises(Exception) as exc_info:
         _, _ = eng.buildExportTable(ads.SampleDataSet(dfData), withExtraFields=True, decPoint='.')
-    logger.info0(f'PASS (test_buildExportTable) => EXCEPTION RAISED AS AWAITED:\n{e_info.value}')
+    logger.info0(f'PASS (test_buildExportTable) => EXCEPTION RAISED AS AWAITED:\n{exc_info}')
 
     # missing field added
     dfData['Surface'] = '2400'
 
     dfExport, extraFields = ads.MCDSEngine().buildExportTable(ads.SampleDataSet(dfData),
                                                               withExtraFields=False, decPoint='.')
 
@@ -162,20 +214,20 @@
     # test all decimal fields (those defined by MCDSEngine and by SampleDataSet) where changed to string type,
     # with '' instead of 'NaN'
     for col in ['Effort', 'Distance', 'TrucDec']:
         assert dfExport[col].compare(dfData[col].apply(lambda x: '' if np.isnan(x) else str(x))).empty, \
             'Error: test_buildExportTable: issue with decimal fields: values of exported DataFrame' \
             "should have same values than source, but as string type (and NaN changed to '')"
 
-    logger.info0('PASS => MCDSEngine => methods "buildExportTable", "matchDataFields" and "safeFloat2Str"')
+    logger.info0('PASS testMcdsBuildExportTable: buildExportTable, matchDataFields, safeFloat2Str')
 
 
 def testMcdsBuildDataFile(dfShortSdsData_fxt):
 
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out')
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out')
     runDir = eng.setupRunFolder(runPrefix='uni')
     dfData = dfShortSdsData_fxt  # load source test data
 
     # export data to file
     dataFileName = eng.buildDataFile(runDir, ads.SampleDataSet(dfData))
     # gather exported data, with columns indexed
     dfFiled = pd.read_csv(dataFileName, sep='\t', header=None)
@@ -183,27 +235,27 @@
     # prepare dfData for comparison - change type of 'Surface' to integer (due to data type as read by pd.read_csv)
     dfData.Surface = dfData.Surface.apply(int)
     # test exported data match to source
     assert dfFiled.compare(dfData[['Region', 'Surface', 'Point', 'Effort', 'Distance']]).empty, \
         'Error: test_buildDataFile: data exported to file do not match to source data'
 
     # clean-up: 'mcds-out' directory and content deleted
-    shutil.rmtree(uivu.pTmpDir / 'mcds-out')
+    shutil.rmtree(uivu.pWorkDir / 'mcds-out')
 
-    logger.info0('PASS => MCDSEngine => methods "buildDataFile"')
+    logger.info0('PASS testMcdsBuildDataFile: buildDataFile"')
 
 
 def testMcdsBuildCmdFile():
 
     # values selected for the test (t_values)
     t_estimKeyFn = 'HNORMAL'
     t_estimAdjustFn = 'COSINE'
     t_estimCriterion = 'AIC'
     t_cvInterval = 95
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out')
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out')
     runDir = eng.setupRunFolder(runPrefix='uni')
     cmdFileName = eng.buildCmdFile(estimKeyFn=t_estimKeyFn, estimAdjustFn=t_estimAdjustFn,
                                    estimCriterion=t_estimCriterion, cvInterval=t_cvInterval, runDir=runDir)
     # read cmd.txt file
     with open(cmdFileName, 'r') as cmdFile:
         lines = cmdFile.readlines()
 
@@ -217,43 +269,43 @@
                    recorded in cmd.txt (estimKeyFn, estimAdjustFn and estimCriterion)'
         elif re.match('^Confidence', line):
             val = re.search('=(.+)(;)$', line)
             assert val.group(1) == str(t_cvInterval), 'Error: test_buildCmdFile: issue with parameter \
                    recorded in cmd.txt (cvInterval)'
 
     # clean-up: 'mcds-out' directory and content deleted
-    shutil.rmtree(uivu.pTmpDir / 'mcds-out')
+    shutil.rmtree(uivu.pWorkDir / 'mcds-out')
 
-    logger.info0('PASS => MCDSEngine => methods "buildCmdFile"')
+    logger.info0('PASS testMcdsBuildCmdFile: buildCmdFile"')
 
 
 def testMcdsComputeSampleStats(dfShortSdsData_fxt):
 
     # init MCDSEngine
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out', runMethod='os.system')
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out', runMethod='os.system')
     # Prepare temporary working folder
     runDir = eng.setupRunFolder(runPrefix='uni')
     # Prepare SampleDataSet and data.txt file
     sds = ads.SampleDataSet(source=dfShortSdsData_fxt, decimalFields=['Effort', 'Distance', 'TrucDec'])
     eng.buildDataFile(sampleDataSet=sds, runDir=runDir)
 
     # Compute sample stats
     sSmpStats = eng.computeSampleStats(sds)
 
     # Check results
     assert (sSmpStats.index == eng.MIStatSampCols).all()
     assert (sSmpStats.values == [4, 7.2, 83.0]).all()
 
-    logger.info0('PASS => MCDSEngine => methods "computeSampleStats"')
+    logger.info0('PASS testMcdsComputeSampleStats: computeSampleStats"')
 
 
 def testMcdsRun(dfShortSdsData_fxt):
 
     # init MCDSEngine
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out', runMethod='os.system')
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out', runMethod='os.system')
     # Prepare temporary working folder
     runDir = eng.setupRunFolder(runPrefix='uni')
     # Prepare SampleDataSet and data.txt file
     sds = ads.SampleDataSet(source=dfShortSdsData_fxt, decimalFields=['Effort', 'Distance', 'TrucDec'])
     eng.buildDataFile(sampleDataSet=sds, runDir=runDir)
     # Prepare cmd.txt file
     cmdFileName = eng.buildCmdFile(estimKeyFn='HNORMAL', estimAdjustFn='COSINE', estimCriterion='AIC', cvInterval=95,
@@ -265,69 +317,66 @@
     assert runStatus == 0 and startTime is pd.NaT and elapsedTime == 0, \
         'Error: test__run: issue occurred with debug mode (forReal=False ; runMethod=os.system)'
 
     # Debug mode - subprocess.run method
     runStatus, startTime, elapsedTime = eng._run(eng.ExeFilePathName, cmdFileName, forReal=False,
                                                  method='subprocess.run')
     # test appropriate outputs
-    assert runStatus == 0 and startTime is pd.NaT and elapsedTime == 0, 'Error: test__run: issue occured with \
-    debug mode (forReal=False ; runMethod=subprocess.run)'
+    assert runStatus == 0 and startTime is pd.NaT and elapsedTime == 0, \
+        'Error: testMcdsRun: issue occurred with debug mode (forReal=False ; runMethod=subprocess.run)'
 
     # JUST TESTING that no exception is raised (no specific tests)
     # run with Warning Status (2) as for JPM test in notebook "unintests.ipynb"
     # Real mode -  os.system method
     _, _, _ = eng._run(eng.ExeFilePathName, cmdFileName, forReal=True, method=eng.runMethod)
 
     # Real mode -  subprocess.run method
     _, _, _ = eng._run(eng.ExeFilePathName, cmdFileName, forReal=True, method='subprocess.run')
 
+    # Unknown run method
+    with pytest.raises(NotImplementedError) as exc_info:
+        _, _, _ = eng._run(eng.ExeFilePathName, cmdFileName, method='unknown')
+    logger.info0(f'Unknown run method: NotImplementedError raised as awaited: {exc_info}')
+
     # Timeout
     runStatus, startTime, engElapsedTime = \
         eng._run(eng.ExeFilePathName, cmdFileName, forReal=True, method='subprocess.run', timeOut=0.01)
     assert runStatus == 555, 'Error: runStatus should be 555 (refer MCDSEngine doc)'
 
     # Measure of performances (low level analysis execution)
     # BE CAREFUL: time.process_time() uses relative time for comparison only of codes among the same environment
     # NOT A REAL TIME reference
-    timePerf = pd.DataFrame(columns=['OSS', 'SPR'], index=list('Cycle' + str(i) for i in range(1, 11)))
+    dfTimePerf = pd.DataFrame(columns=['OSS', 'SPR'])
 
-    i = 0
-    while i < 10:
-        j = 0
+    for cycle in range(10):
         start = time.perf_counter()
-        while j < 5:
+        for _ in range(5):
             _, _, _ = eng._run(eng.ExeFilePathName, cmdFileName, forReal=True, method=eng.runMethod)
-            j += 1
         end = time.perf_counter()
+        dfTimePerf.at[cycle + 1, 'OSS'] = end - start
 
-        timePerf.iloc[i, 0] = end - start
-        i += 1
-
-    i = 0
-    while i < 10:
-        j = 0
+    for cycle in range(10):
         start = time.perf_counter()
-        while j < 5:
+        for _ in range(5):
             _, _, _ = eng._run(eng.ExeFilePathName, cmdFileName, forReal=True, method='subprocess.run')
-            j += 1
         end = time.perf_counter()
+        dfTimePerf.at[cycle + 1, 'SPR'] = end - start
 
-        timePerf.iloc[i, 1] = end - start
-        i += 1
+    dfTimePerf['OSS-faster'] = dfTimePerf.OSS < dfTimePerf.SPR
+    dfTimePerf['%_vs_OSS'] = ((dfTimePerf.SPR - dfTimePerf.OSS) / dfTimePerf.OSS) * 100
 
-    timePerf['OSS-faster'] = timePerf['OSS'] < timePerf['SPR']
-    timePerf['%_vs_OSS'] = ((timePerf['SPR'] - timePerf['OSS']) / timePerf['OSS']) * 100
-
-    logger.info0('\n\nPerformance: 10 loops of 5 runs (OSS = "os.system" ; SPR = "subprocess.run")\n')
-    logger.info0(f'\n{timePerf.to_markdown(floatfmt=".2f")}\n')
-    logger.info0(f'For "os.system": Mean +/- Std Dev = {timePerf["OSS"].mean():.2f} +/- {timePerf["OSS"].std():.2f}')
+    logger.info0('Performance: 10 loops of 5 runs (OSS = "os.system" ; SPR = "subprocess.run")')
+    logger.info0('\n' + dfTimePerf.to_string(float_format=lambda f: f'{f:.2f}'))
+    logger.info0(f'For "os.system": Mean +/- Std Dev = {dfTimePerf.OSS.mean():.2f}s +/- {dfTimePerf.OSS.std():.2f}')
+    logger.info0(
+        f'For "subprocess.run": Mean +/- Std Dev = {dfTimePerf.SPR.mean():.2f}s +/- {dfTimePerf.SPR.std():.2f}')
     logger.info0(
-        f'For "subprocess.run": Mean +/- Std Dev = {timePerf["SPR"].mean():.2f} +/- {timePerf["SPR"].std():.2f}\n\n')
+        f"%_vs_OSS: Mean +/- Std Dev = {dfTimePerf['%_vs_OSS'].mean():.1f}% +/- {dfTimePerf['%_vs_OSS'].std():.1f}")
 
-    logger.info0('PASS => MCDSEngine => methods "_run", "_runThroughOSSystem" and "_runThroughSubProcessRun"')
+    logger.info0('PASS testMcdsRun: _run, _runThroughOSSystem, _runThroughSubProcessRun')
 
 
 #   Generate a reduced real-life SampleDataSet
 def sdsRealReduced():
     return ads.SampleDataSet(source=uivu.pRefInDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols.xlsx',
                              decimalFields=['EFFORT', 'DISTANCE', 'NOMBRE'])
 
@@ -341,15 +390,15 @@
 # ### f. High level analysis execution  (via executor), debug mode
 # (generate cmd and data input files, but no call to executable)
 def testMcdsSubmitAnalysisDebug(sdsRealReduced_fxt):
 
     sds = sdsRealReduced_fxt
 
     # init MCDSEngine
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out')
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out')
 
     # Prepare temporary working folder
     runDir = eng.setupRunFolder(runPrefix='uni')
     logger.info0(f'Debug run {runDir=}')
 
     # Asynchronous model, even if no parallelism involved : submitAnalysis() returns a "future" object
     # (see module concurrent)
@@ -367,40 +416,42 @@
         eng.submitAnalysis(sds, realRun=False, runPrefix='int',
                            estimKeyFn='UNIFORM', estimAdjustFn='POLY',
                            estimCriterion='AIC', cvInterval=95).result()
     assert runCode == ads.MCDSEngine.RCNotRun, 'Should have NOT run (run code = 0)'
     logger.info('Debug run:\n' + str(dict(runCode=runCode, runDir=runDir,
                                           startTime=startTime, elapsedTime=elapsedTime, sResults=sResults)))
 
+    logger.info0('PASS testMcdsSubmitAnalysisDebug: Ctor, setupRunFolder, submitAnalysis')
+
 
 # ### g. High level analysis execution  (via executor), real mode
 KRunCheckErrMsg = {ads.MCDSEngine.RCOK: 'Oh, oh, should have run smoothly and successfully !',
                    ads.MCDSEngine.RCWarnings: 'Oh, oh, should have run smoothly (even if with warnings) !',
                    ads.MCDSEngine.RCTimedOut: 'Oh, oh, should have timed-out !'}
 
 
 def checkEngineAnalysisRun(sampleDataSet, estimKeyFn='UNIFORM', estimAdjustFn='POLY', estimCriterion='AIC',
-                           cvInterval=95,
-                           minDist=None, maxDist=None, fitDistCuts=None, discrDistCuts=None,
+                           cvInterval=95, minDist=None, maxDist=None, fitDistCuts=None, discrDistCuts=None,
                            runMethod='os.system', timeOut=None, expectRunCode=ads.MCDSEngine.RCOK):
     # Need for an async. executor for time limit checking with os.system run method.
     exor = None if runMethod != 'os.system' or timeOut is None else ads.Executor(threads=1)
 
     # Engine
-    eng = ads.MCDSEngine(executor=exor, workDir=uivu.pTmpDir / 'mcds-out',
+    eng = ads.MCDSEngine(executor=exor, workDir=uivu.pWorkDir / 'mcds-out',
                          runMethod=runMethod, timeOut=timeOut)
 
     # Run analysis and get results
     fut = eng.submitAnalysis(sampleDataSet, realRun=True, runPrefix='int',
                              estimKeyFn=estimKeyFn, estimAdjustFn=estimAdjustFn,
                              estimCriterion=estimCriterion, cvInterval=cvInterval,
                              minDist=minDist, maxDist=maxDist,
                              fitDistCuts=fitDistCuts, discrDistCuts=discrDistCuts)
 
     try:
+        startTime = None
         if timeOut is not None:
             startTime = pd.Timestamp.now()  # In case of cofu.TimeoutError
         runCode, startTime, elapsedTime, runDir, sResults = fut.result(timeout=timeOut)
     except cofu.TimeoutError:
         logger.info('MCDS Analysis run timed-out after {}s'.format(timeOut))
         runCode, startTime, elapsedTime, runDir, sResults = eng.RCTimedOut, startTime, timeOut, None, None
 
@@ -419,57 +470,65 @@
 
 
 def testMcdsSubmitAnalysisReal(sdsRealReduced_fxt):
 
     sds = sdsRealReduced_fxt
 
     # init MCDSEngine
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out')
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out')
 
     # Prepare temporary working folder
     runDir = eng.setupRunFolder(runPrefix='uni')
     logger.info0(f'Real run: {runDir=}')
 
     # No time limit
     checkEngineAnalysisRun(sds, estimKeyFn='NEXPON', estimAdjustFn='COSINE', estimCriterion='AIC', cvInterval=95,
+                           minDist=None, maxDist=None, fitDistCuts=None, discrDistCuts=None,
                            runMethod='os.system', timeOut=None, expectRunCode=ads.MCDSEngine.RCWarnings)
 
     # Some time limit, but too long to stop analysis.
     checkEngineAnalysisRun(sds, estimKeyFn='HNORMAL', estimAdjustFn='COSINE', estimCriterion='AIC', cvInterval=95,
+                           minDist=40, maxDist=300, fitDistCuts=[60, 80, 100, 140, 180, 230], discrDistCuts=6,
                            runMethod='os.system', timeOut=3, expectRunCode=ads.MCDSEngine.RCWarnings)
 
     # Too short time limit => analysis time-out (but MCDS goes on to its end : no kill done by executor)
     checkEngineAnalysisRun(sds, estimKeyFn='UNIFORM', estimAdjustFn='POLY', estimCriterion='AIC', cvInterval=95,
+                           minDist=None, maxDist=None, fitDistCuts=None, discrDistCuts=None,
                            runMethod='os.system', timeOut=0.1, expectRunCode=ads.MCDSEngine.RCTimedOut)
 
     logger.info('Look: MCDS was not killed, it has gone to its end, whereas the analysis has timed-out')
 
     # No time limit
     checkEngineAnalysisRun(sds, estimKeyFn='NEXPON', estimAdjustFn='COSINE', estimCriterion='AIC', cvInterval=95,
+                           minDist=40, maxDist=250, fitDistCuts=7, discrDistCuts=[60, 80, 100, 120, 160, 200],
                            runMethod='subprocess.run', timeOut=None, expectRunCode=ads.MCDSEngine.RCWarnings)
 
     # Some time limit, but too long to stop analysis.
     checkEngineAnalysisRun(sds, estimKeyFn='HNORMAL', estimAdjustFn='POLY', estimCriterion='AIC', cvInterval=95,
+                           minDist=None, maxDist=None, fitDistCuts=None, discrDistCuts=None,
                            runMethod='subprocess.run', timeOut=3, expectRunCode=ads.MCDSEngine.RCErrors)
 
     # Too short time limit => analysis time-out (but MCDS goes on to its end : no kill done by executor)
     checkEngineAnalysisRun(sds, estimKeyFn='UNIFORM', estimAdjustFn='POLY', estimCriterion='AIC', cvInterval=95,
+                           minDist=None, maxDist=None, fitDistCuts=None, discrDistCuts=None,
                            runMethod='subprocess.run', timeOut=0.05, expectRunCode=ads.MCDSEngine.RCTimedOut)
 
     logger.info('Look: MCDS was actually killed on time-out')
 
+    logger.info0('PASS testMcdsSubmitAnalysisReal: Ctor, setupRunFolder, submitAnalysis')
+
 
 # h. Generate input data files for interactive Distance software
 #   ('point transect' mode only as for now)
 def testMcdsBuildDistanceDataFile(sdsRealReduced_fxt, dfShortSdsData_fxt):
 
     sds = sdsRealReduced_fxt
 
     # init MCDSEngine
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out')
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out')
 
     # Prepare target folder
     tgtDir = pl.Path(eng.workDir, 'distance-in')
     tgtDir.mkdir(exist_ok=True)
 
     # Case 1: Point transect with radial distance, no extra fields, no clustering.
     distDataFileName = \
@@ -487,15 +546,15 @@
     refDistDataFileName = uivu.pRefOutDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-withextra.txt'
     with io.open(distDataFileName) as tst_f, io.open(refDistDataFileName) as ref_f:
         assert list(tst_f) == list(ref_f)
 
     eng.shutdown()
 
     # Case 2: Point transect with radial distance, no extra fields, with clustering.
-    eng = ads.MCDSEngine(workDir=uivu.pTmpDir / 'mcds-out', clustering=True)
+    eng = ads.MCDSEngine(workDir=uivu.pWorkDir / 'mcds-out', clustering=True)
     # Add cluster data to the data set
     dfData = dfShortSdsData_fxt
     dfData['Nombre'] = [1, 2, 1, 1, 2, 3]
     sds = ads.SampleDataSet(source=dfData, decimalFields=['Effort', 'Distance', 'TrucDec'])
     # Generate distance file
     tgtDir = pl.Path(eng.workDir, 'distance-in')
     tgtDir.mkdir(exist_ok=True)
@@ -503,63 +562,29 @@
         eng.buildDistanceDataFile(sds, tgtFilePathName=tgtDir / 'import-data-clusters.txt')
     refDistDataFileName = uivu.pRefOutDir / 'ACDC2019-Papyrus-ALAARV-saisie-ttes-cols-import-data-clusters.txt'
     with io.open(distDataFileName) as tst_f, io.open(refDistDataFileName) as ref_f:
         assert list(tst_f) == list(ref_f)
 
     eng.shutdown()
 
+    logger.info0('PASS testMcdsBuildDistanceDataFile: Ctor, buildDistanceDataFile')
+
 
 # i. TODO:  Test lower level code
-# * loadDataFile
-# * buildExportTable
-# * decodeStats
-# * decodeLog
-# * decodePlots
-# * decodeOutput
+def testLowerLevelCode():
+    # * loadDataFile
+    # * buildExportTable
+    # * decodeStats
+    # * decodeLog
+    # * decodePlots
+    # * decodeOutput
+
+    raise NotImplementedError('TODO !')
 
 
 ###############################################################################
 #                         Actions to be done after all tests                  #
 ###############################################################################
 def testEnd():
-    uivu.logEnd(what=what2Test)
-
-
-# This pytest-compatible module can also be run as a simple python script.
-if __name__ == '__main__':
-
-    run = True
-
-    # Run auto-tests (exit(0) if OK, 1 if not).
-    rc = -1
-
-    uivu.logBegin(what=what2Test)
-
-    if run:
-        try:
-            testBegin()
-
-            testDsExecutableNotFound()
-            testMcdsCtor()
-            testDsSetupRunFolder()
-            testMcdsBuildExportTable(dfShortSdsData())
-            testMcdsBuildDataFile(dfShortSdsData())
-            testMcdsBuildCmdFile()
-            testMcdsComputeSampleStats(dfShortSdsData())
-            testMcdsRun(dfShortSdsData())
-
-            testMcdsSubmitAnalysisDebug(sdsRealReduced())
-            testMcdsSubmitAnalysisReal(sdsRealReduced())
-            testMcdsBuildDistanceDataFile(sdsRealReduced(), dfShortSdsData())
-
-            testEnd()
-
-            # Success !
-            rc = 0
-
-        except Exception as exc:
-            logger.exception(f'Exception: {exc}')
-            rc = 1
-
-    uivu.logEnd(what=what2Test, rc=rc)
-
-    sys.exit(rc)
+    if KFinalCleanup:
+        uivu.cleanupWorkDir()
+    uivu.logEnd(what=KWhat2Test)
```

### Comparing `pyaudisam-1.0.2/tests/unintests.ipynb` & `pyaudisam-1.1.0/tests/unintests.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959595194929867%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, 'import pickle, lzma\\n')]}}, 79: {'metadata': {replace: "*

 * *            'OrderedDict()}}, 84: {\'source\': {insert: [(12, "    anlys = '*

 * *            "ads.MCDSAnalysis(engine=eng, sampleDataSet=sampleDataSet, name='anlys', "*

 * *            'logData=True,\\n"), (13, \'                             estimKeyFn=estimKeyFn, '*

 * *            "estimAdjustFn=estimAdjustFn,\\n'), (14, '                             "*

 * *            "estimCriterion=estimCriterion, cvInterval=cvInterval,\\ […]*

```diff
@@ -55,14 +55,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import sys\n",
                 "import copy\n",
                 "import os\n",
                 "import pathlib as pl\n",
+                "import pickle, lzma\n",
                 "\n",
                 "import re\n",
                 "\n",
                 "import concurrent.futures as cofu\n",
                 "\n",
                 "import math\n",
                 "import numpy as np\n",
@@ -1157,17 +1158,15 @@
             "outputs": [],
             "source": [
                 "distDataFileName.as_posix()"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "jp-MarkdownHeadingCollapsed": true
-            },
+            "metadata": {},
             "source": [
                 "### i. TODO"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -1222,17 +1221,18 @@
                 "    exor = None if runMethod != 'os.system' or timeOut is None else ads.Executor(threads=1)\n",
                 "        \n",
                 "    # Engine\n",
                 "    eng = ads.MCDSEngine(executor=exor, workDir=tmpDir / 'mcds-out',\n",
                 "                         runMethod=runMethod, timeOut=timeOut)\n",
                 "    \n",
                 "    # Analysis\n",
-                "    anlys = ads.MCDSAnalysis(engine=eng, sampleDataSet=sds, name='anlys', logData=True,\n",
-                "                             estimKeyFn='UNIFORM', estimAdjustFn='POLY', estimCriterion='AIC', cvInterval=95,\n",
-                "                             minDist=None, maxDist=None, fitDistCuts=None, discrDistCuts=None)\n",
+                "    anlys = ads.MCDSAnalysis(engine=eng, sampleDataSet=sampleDataSet, name='anlys', logData=True,\n",
+                "                             estimKeyFn=estimKeyFn, estimAdjustFn=estimAdjustFn,\n",
+                "                             estimCriterion=estimCriterion, cvInterval=cvInterval,\n",
+                "                             minDist=minDist, maxDist=maxDist, fitDistCuts=fitDistCuts, discrDistCuts=discrDistCuts)\n",
                 "\n",
                 "    # Run\n",
                 "    anlys.submit()\n",
                 "    \n",
                 "    # Get result\n",
                 "    sResult = anlys.getResults()\n",
                 "\n",
@@ -2583,15 +2583,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfObs = pd.read_csv('refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt', sep='\\t', decimal=',')\n",
+                "dfObs = pd.read_csv('refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt', sep='\\t', decimal=',')\n",
                 "dfObs.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -2840,15 +2840,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Second, try from source CSV file\n",
-                "fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt',\n",
+                "fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt',\n",
                 "                       importDecFields=['distMem'], countCols=countCols,\n",
                 "                       addMonoCatCols={ 'Adulte': count2AdultCat, 'Dur\u00e9e': count2DurationCat })"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -3262,15 +3262,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "userVariantSpecs = 'refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx'\n",
+                "userVariantSpecs = 'refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.xlsx'\n",
                 "\n",
                 "if False: # Both method MUST work, but this one needs more code :-)\n",
                 "    userVariantSpecs = pd.read_excel(userVariantSpecs, sheet_name=None)\n",
                 "    print('sheets:', ', '.join(userVariantSpecs.keys()))\n",
                 "\n",
                 "userVariantSpecs"
             ]
@@ -3305,15 +3305,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Computational checks\n",
                 "if isinstance(userVariantSpecs, dict):\n",
                 "    ddfUserVariantSpecs = userVariantSpecs\n",
                 "else:\n",
-                "    ddfUserVariantSpecs = pd.read_excel('refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx', sheet_name=None)\n",
+                "    ddfUserVariantSpecs = pd.read_excel('refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.xlsx', sheet_name=None)\n",
                 "\n",
                 "nEch1Vars = 1\n",
                 "df = ddfUserVariantSpecs['Echant1_impl']\n",
                 "for col in df.columns:\n",
                 "    nEch1Vars *= len(df[col].dropna())\n",
                 "    \n",
                 "nEch2Vars = 1\n",
@@ -3429,15 +3429,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Via combinaisons implicites, par fichier.\n",
                 "dfExplParamSpecs, userParamSpecCols, intParamSpecCols, unmUserParamSpecCols = \\\n",
-                "    ads.DSAnalyser._explicitParamSpecs(implParamSpecs='refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx',\n",
+                "    ads.DSAnalyser._explicitParamSpecs(implParamSpecs='refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.xlsx',\n",
                 "                                       int2UserSpecREs=int2UserSpecREs,\n",
                 "                                       sampleSelCols=sampleSelCols, abbrevCol=anlysAbbrevCol,\n",
                 "                                       abbrevBuilder=analysisAbbrev, anlysIndCol=varIndCol,\n",
                 "                                       sampleIndCol=sampleIndCol, dropDupes=False)"
             ]
         },
         {
@@ -4281,15 +4281,15 @@
                 "\n",
                 "def count2AdultCat(sCounts):\n",
                 "    return 'm' if 'Mal' in sCounts[sCounts > 0].index[0] else 'a'\n",
                 "\n",
                 "def count2DurationCat(sCounts):\n",
                 "    return '5mn' if '5' in sCounts[sCounts > 0].index[0] else '10mn'\n",
                 "\n",
-                "fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt',\n",
+                "fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt',\n",
                 "                       importDecFields=['distMem'], countCols=countCols,\n",
                 "                       addMonoCatCols={ 'Adulte': count2AdultCat, 'Dur\u00e9e': count2DurationCat })\n",
                 "\n",
                 "dfObsIndiv = fds.individualise()\n",
                 "\n",
                 "dfObsIndiv.drop(columns=countCols, inplace=True)\n",
                 "\n",
@@ -4303,17 +4303,18 @@
             "outputs": [],
             "source": [
                 "transectPlaceCols = ['Point']\n",
                 "passIdCol = 'Passage'\n",
                 "effortCol = 'Effort'\n",
                 "\n",
                 "sampleDistCol = 'distMem'\n",
+                "sampleCols = [passIdCol, 'Adulte', 'Dur\u00e9e']\n",
                 "sampleDecCols=[effortCol, sampleDistCol]\n",
                 "\n",
-                "sampleSelCols = ['Esp\u00e8ce', passIdCol, 'Adulte', 'Dur\u00e9e']\n",
+                "sampleSelCols = ['Esp\u00e8ce'] + sampleCols\n",
                 "\n",
                 "varIndCol = 'IndAnlys'\n",
                 "anlysAbbrevCol = 'AbrevAnlys'\n",
                 "\n",
                 "dSurveyArea = dict(Zone='ACDC', Surface='2400')"
             ]
         },
@@ -4465,34 +4466,30 @@
             "source": [
                 "### e. getAnalysisOptimedParams"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [],
             "source": [
-                "# Get a \"random\" sample from indiv. data set\n",
-                "sAnSpec = pd.Series({ 'Esp\u00e8ce': 'Alauda arvensis', 'Passage': 'a+b', 'Adulte': 'm+a', 'Dur\u00e9e': '10mn'})\n",
+                "# Get a \"random\" sample from indiv. data set + compute some base figures for checking results\n",
+                "sAnSpec = pd.Series({'Esp\u00e8ce': 'Alauda arvensis', 'Passage': 'a+b', 'Adulte': 'm+a', 'Dur\u00e9e': '10mn'})\n",
                 "sds = optr._mcDataSet.sampleDataSet(sAnSpec[sampleCols])\n",
                 "sSampleDistances = sds.dfData[sampleDistCol].dropna()\n",
-                "len(sSampleDistances)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Some base figures for checking results\n",
+                "\n",
                 "sqd = np.sqrt(len(sSampleDistances.dropna()))\n",
                 "dMin = sSampleDistances.min()\n",
-                "dMax = sSampleDistances.max()"
+                "dMax = sSampleDistances.max()\n",
+                "\n",
+                "print(f'* Sample distances: dMin={dMin}, dMax={dMax}, ...')\n",
+                "print(f'  {len(sSampleDistances)} sample distances =>\\n{sorted(sSampleDistances.values)}')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -4526,32 +4523,67 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "outliersQuantCutPct = 2.5\n",
+                "d25, d75, d95, dPct = np.percentile(a=sSampleDistances, q=[25, 75, 95, 100-outliersQuantCutPct])\n",
+                "minMaxDist = min(max(d95, d75 + 1.5*(d75 - d25)), dPct)\n",
+                "\n",
+                "dict(d25=d25, d75=d75, dSup=d75 + 1.5*(d75 - d25), d95=d95, dPct=dPct, minMaxDist=minMaxDist)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [],
+            "source": [
+                "# Get a new \"random\" sample from indiv. data set + compute some base figures for checking results\n",
+                "sAnSpec = pd.Series({'Esp\u00e8ce': 'Alauda arvensis', 'Passage': 'a+b', 'Adulte': 'm+a', 'Dur\u00e9e': '5mn'})\n",
+                "sds = optr._mcDataSet.sampleDataSet(sAnSpec[sampleCols])\n",
+                "sSampleDistances = sds.dfData[sampleDistCol].dropna()\n",
+                "\n",
+                "sqd = np.sqrt(len(sSampleDistances.dropna()))\n",
+                "dMin = sSampleDistances.min()\n",
+                "dMax = sSampleDistances.max()\n",
+                "\n",
+                "print(f'* Sample distances: dMin={dMin}, dMax={dMax}, ...')\n",
+                "print(f'  {len(sSampleDistances)} sample distances =>\\n{sorted(sSampleDistances.values)}')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# All present and variant (check computations) 2\n",
                 "# a. Call method\n",
                 "sAnIntSpec = pd.Series({ adsto.IntSpecMinDist:'quant(5)', adsto.IntSpecMaxDist:'auto',\n",
                 "                         adsto.IntSpecFitDistCuts:'mult(3/4, 5/4)', adsto.IntSpecDiscrDistCuts:'abs(4, 6)',\n",
                 "                         adsto.IntSpecOutliersMethod:'tucquant(1)'})\n",
                 "e, r = optr.getAnalysisOptimedParams(sAnIntSpec, sSampleDistances)\n",
                 "\n",
                 "assert e is None\n",
                 "\n",
                 "sr = str({ k:str(v) for k,v in r.items() })\n",
                 "print('Actual result   :', sr)\n",
                 "\n",
                 "# b. Compute theorical result\n",
-                "qLeft, qRight = np.percentile(a=sSampleDistances, q=[5, 99])\n",
-                "\n",
-                "print('Base variables  :', dict(sqd=sqd, dMin=dMin, dMax=dMax, qLeft=qLeft, qRight=qRight))\n",
+                "qLeft, q25, q75, q95, qRight = np.percentile(a=sSampleDistances, q=[5, 25, 75, 95, 99])\n",
+                "qSup = q75 + 1.5 * (q75 - q25)\n",
+                "print('Base variables  :', dict(sqd=sqd, dMin=dMin, dMax=dMax, qLeft=qLeft,\n",
+                "                                q75=q75, qSup=qSup, q95=q95, qRight=qRight))\n",
                 "\n",
-                "sol = dict(minDist=ads.Interval(dMin, qLeft), maxDist=ads.Interval(qRight, dMax),\n",
+                "sol = dict(minDist=ads.Interval(dMin, qLeft), maxDist=ads.Interval(qSup, dMax),\n",
                 "           fitDistCuts=ads.Interval(int(round(sqd*3/4)), int(round(sqd*5/4))), discrDistCuts=ads.Interval(4, 6))\n",
                 "\n",
                 "ssol = str({ k:str(v) for k,v in sol.items() })\n",
                 "print('Theorical result:', ssol)\n",
                 "\n",
                 "# c. Check \"equality\" (for some reason, must use str repr for comparison ...)\n",
                 "assert sr == ssol"
@@ -4559,32 +4591,68 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "outliersQuantCutPct = 1\n",
+                "d25, d75, d95, dPct = np.percentile(a=sSampleDistances, q=[25, 75, 95, 100-outliersQuantCutPct])\n",
+                "minMaxDist = min(max(d95, d75 + 1.5*(d75 - d25)), dPct)\n",
+                "\n",
+                "dict(d25=d25, d75=d75, dSup=d75 + 1.5*(d75 - d25), d95=d95, dPct=dPct, minMaxDist=minMaxDist)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [],
+            "source": [
+                "# Get a new \"random\" sample from indiv. data set + compute some base figures for checking results\n",
+                "sAnSpec = pd.Series({'Esp\u00e8ce': 'Alauda arvensis', 'Passage': 'a+b', 'Adulte': 'm+a', 'Dur\u00e9e': '10mn'})\n",
+                "sds = optr._mcDataSet.sampleDataSet(sAnSpec[sampleCols])\n",
+                "sSampleDistances = sds.dfData[sampleDistCol].dropna()\n",
+                "\n",
+                "sqd = np.sqrt(len(sSampleDistances.dropna()))\n",
+                "dMin = sSampleDistances.min()\n",
+                "dMax = sSampleDistances.max()\n",
+                "\n",
+                "print(f'* Sample distances: dMin={dMin}, dMax={dMax}, ...')\n",
+                "print(f'  {len(sSampleDistances)} sample distances =>\\n{sorted(sSampleDistances.values)}')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [],
+            "source": [
                 "# All present and variant (check computations) 3\n",
                 "# a. Call method\n",
                 "sAnIntSpec = pd.Series({ adsto.IntSpecMinDist:'auto', adsto.IntSpecMaxDist:'auto',\n",
                 "                         adsto.IntSpecFitDistCuts:'auto', adsto.IntSpecDiscrDistCuts:'auto',\n",
                 "                         adsto.IntSpecOutliersMethod:'tucquant(2)'})\n",
                 "e, r = optr.getAnalysisOptimedParams(sAnIntSpec, sSampleDistances)\n",
                 "\n",
                 "assert e is None\n",
                 "\n",
                 "sr = str({ k:str(v) for k,v in r.items() })\n",
                 "print('Actual result   :', sr)\n",
                 "\n",
                 "# b. Compute theorical result\n",
-                "qLeft, qRight = np.percentile(a=sSampleDistances, q=[2, 98])\n",
+                "qLeft, q95, qRight = np.percentile(a=sSampleDistances, q=[2, 95, 98])\n",
                 "\n",
-                "print('Base variables  :', dict(sqd=sqd, dMin=dMin, dMax=dMax, qLeft=qLeft, qRight=qRight))\n",
+                "print('Base variables  :', dict(sqd=sqd, dMin=dMin, dMax=dMax, qLeft=qLeft, q95=q95, qRight=qRight))\n",
                 "\n",
-                "sol = dict(minDist=ads.Interval(dMin, qLeft), maxDist=ads.Interval(qRight, dMax),\n",
+                "sol = dict(minDist=ads.Interval(dMin, qLeft), maxDist=ads.Interval(q95, dMax),\n",
                 "           fitDistCuts=ads.Interval(int(round(sqd*2/3)), int(round(sqd*3/2))),\n",
                 "           discrDistCuts=ads.Interval(int(round(sqd/3)), int(round(sqd))))\n",
                 "\n",
                 "ssol = str({ k:str(v) for k,v in sol.items() })\n",
                 "print('Theorical result:', ssol)\n",
                 "\n",
                 "# c. Check \"equality\" (for some reason, must use str repr for comparison ...)\n",
@@ -4593,14 +4661,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "outliersQuantCutPct = 6\n",
+                "d25, d75, d95, dPct = np.percentile(a=sSampleDistances, q=[25, 75, 95, 100-outliersQuantCutPct])\n",
+                "minMaxDist = min(max(d95, d75 + 1.5*(d75 - d25)), dPct)\n",
+                "\n",
+                "dict(d25=d25, d75=d75, dSup=d75 + 1.5*(d75 - d25), d95=d95, dPct=dPct, minMaxDist=minMaxDist)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# All present and variant (check computations) 4\n",
                 "# a. Call method\n",
                 "sAnIntSpec = pd.Series({ adsto.IntSpecMinDist:'auto', adsto.IntSpecMaxDist:'auto',\n",
                 "                         adsto.IntSpecFitDistCuts:'auto', adsto.IntSpecDiscrDistCuts:'auto',\n",
                 "                         adsto.IntSpecOutliersMethod:'auto'})\n",
                 "e, r = optr.getAnalysisOptimedParams(sAnIntSpec, sSampleDistances)\n",
                 "\n",
@@ -4690,31 +4771,33 @@
                 "# c. Check \"equality\" (for some reason, must use str repr for comparison ...)\n",
                 "assert sr == ssol"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [],
             "source": [
                 "# All present, some variant, some consts (check computations) 3\n",
                 "# a. Call method\n",
                 "sAnIntSpec = pd.Series({ adsto.IntSpecMinDist:'auto', adsto.IntSpecMaxDist:'auto',\n",
                 "                         adsto.IntSpecFitDistCuts:17, adsto.IntSpecDiscrDistCuts:'auto',\n",
-                "                         adsto.IntSpecOutliersMethod:'tucquant(2)'})\n",
+                "                         adsto.IntSpecOutliersMethod:'tucquant(6)'})\n",
                 "e, r = optr.getAnalysisOptimedParams(sAnIntSpec, sSampleDistances)\n",
                 "\n",
                 "assert e is None\n",
                 "\n",
                 "sr = str({ k:str(v) for k,v in r.items() })\n",
                 "print('Actual result   :', sr)\n",
                 "\n",
                 "# b. Compute theorical result\n",
-                "qLeft, qRight = np.percentile(a=sSampleDistances, q=[2, 98])\n",
+                "qLeft, qRight = np.percentile(a=sSampleDistances, q=[6, 94])\n",
                 "\n",
                 "print('Base variables  :', dict(sqd=sqd, dMin=dMin, dMax=dMax, qLeft=qLeft, qRight=qRight))\n",
                 "\n",
                 "sol = dict(minDist=ads.Interval(dMin, qLeft), maxDist=ads.Interval(qRight, dMax),\n",
                 "           fitDistCuts=17, discrDistCuts=ads.Interval(int(round(sqd/3)), int(round(sqd))))\n",
                 "\n",
                 "ssol = str({ k:str(v) for k,v in sol.items() })\n",
@@ -4726,14 +4809,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "outliersQuantCutPct = 6\n",
+                "d25, d75, d95, dPct = np.percentile(a=sSampleDistances, q=[25, 75, 95, 100-outliersQuantCutPct])\n",
+                "minMaxDist = min(max(d95, d75 + 1.5*(d75 - d25)), dPct)\n",
+                "\n",
+                "dict(d25=d25, d75=d75, dSup=d75 + 1.5*(d75 - d25), d95=d95, dPct=dPct, minMaxDist=minMaxDist)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# All present, some variant, some consts (check computations) 4\n",
                 "# a. Call method\n",
                 "sAnIntSpec = pd.Series({ adsto.IntSpecMinDist:'auto', adsto.IntSpecMaxDist:'auto',\n",
                 "                         adsto.IntSpecFitDistCuts:'auto', adsto.IntSpecDiscrDistCuts:6,\n",
                 "                         adsto.IntSpecOutliersMethod:'auto'})\n",
                 "e, r = optr.getAnalysisOptimedParams(sAnIntSpec, sSampleDistances)\n",
                 "\n",
@@ -5223,15 +5319,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Load individualised observations and actual transects\n",
-                "indivObsFile = 'refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods'\n",
+                "indivObsFile = 'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods'\n",
                 "\n",
                 "dfObsIndiv = ads.DataSet(indivObsFile, sheet='Donn\u00e9esIndiv').dfData\n",
                 "\n",
                 "dfTransects = ads.DataSet(indivObsFile, sheet='Inventaires').dfData\n",
                 "\n",
                 "dict(indivObs=len(dfObsIndiv), transects=len(dfTransects))"
             ]
@@ -5942,15 +6038,15 @@
             "source": [
                 "# Load results to play with ...\n",
                 "# Note: Okay, it's actually an MCDSTruncOptAnalysisResultsSet file ... but we'll ignore the extra columns, promised :-)\n",
                 "resFileName = 'refin/ACDC2019-Naturalist-UnitestOptResultats.ods'\n",
                 "print('Loading results from {} ...'.format(resFileName))\n",
                 "\n",
                 "# Make test simpler : replace filter and sort key predefined generation scheme set by a shorter one.\n",
-                "results = anlr.setupResults(ldFilSorKeySchemes=ldFilSorKeySchemes)  # See f. right above for ldFilSorKeySchemes definition  !\n",
+                "results = anlr.setupResults(ldFilSorKeySchemes=ldFilSorKeySchemes)  # See j. right above for ldFilSorKeySchemes definition  !\n",
                 "\n",
                 "results.fromOpenDoc(resFileName, postComputed=True)  # Prevent re-post-computation : not a problem here, but longer"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -6419,15 +6515,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Load individualised observations and actual transects\n",
-                "indivObsFile = 'refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods'\n",
+                "indivObsFile = 'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods'\n",
                 "\n",
                 "dfObsIndiv = ads.DataSet(indivObsFile, sheet='Donn\u00e9esIndiv').dfData\n",
                 "\n",
                 "dfTransects = ads.DataSet(indivObsFile, sheet='Inventaires').dfData\n",
                 "\n",
                 "dict(indivObs=len(dfObsIndiv), transects=len(dfTransects))"
             ]
@@ -6921,41 +7017,23 @@
             "metadata": {
                 "scrolled": true
             },
             "outputs": [],
             "source": [
                 "refRes = optanlr.setupResults()\n",
                 "\n",
-                "resFileName = 'refout/ACDC2019-Naturalist-ExtraitOptResultats.ods'\n",
+                "resFileName = 'refout/ACDC2019-Naturalist-extrait-OptResultats.ods'\n",
                 "print('Loading results from {} ...'.format(resFileName))\n",
                 "\n",
                 "refRes.fromExcel(resFileName, postComputed=True)  # Prevent re-post-computation : this is our reference !\n",
                 "\n",
                 "optanlr.shutdown()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# TODO: No, rather ... rather what ????\n",
-                "# Remove analyses with non-unique 'NumAnlys' (because of multiple optimisation tries)\n",
-                "# (to make comparison easier, sorry)\n",
-                "numAnlysCols = ('header (head)', 'NumAnlys', 'Value')\n",
-                "numEchantCol = ('header (head)', 'NumEchant', 'Value')\n",
-                "\n",
-                "sb = refRes.dfData[[numAnlysCols, numEchantCol]].groupby([numAnlysCols]).transform(len)[numEchantCol] > 1\n",
-                "refRes.dropRows(sb)\n",
-                "\n",
-                "refRes.dfData"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### y.ii Trigger re-post-computation on a copy\n",
                 "\n",
                 "(post-computations are the first thing we want to check for non regression)"
             ]
@@ -6980,15 +7058,17 @@
                 "res = refRes.copy()\n",
                 "res.setPostComputed(False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [],
             "source": [
                 "# Trigger now !\n",
                 "res.dfData"
             ]
         },
         {
@@ -7002,86 +7082,115 @@
                 "* 29 results get different sort orders (for many or all of them)\n",
                 "* out of 54 total results !"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [],
             "source": [
                 "refRes.columns.to_list()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "indexCols = [('header (head)', 'NumAnlys', 'Value'), ('header (tail)', 'TrGche', 'Value'),\n",
-                " ('header (tail)', 'TrDrte', 'Value'),\n",
-                " ('header (tail)', 'NbTrchMod', 'Value'),\n",
-                " ('header (tail)', 'OptimTrunc', 'Value')]\n",
-                "subsetCols=[col for col in refRes.dfData.columns if col[0] == 'auto filter sort']\n",
+                "indexCols = [('header (head)', 'NumAnlys', 'Value'),\n",
+                "             ('run output', 'run folder', 'Value'),  # Needed for multiple optimisation tries kept per (same id) analysis\n",
+                "             ('header (tail)', 'TrGche', 'Value'),\n",
+                "             ('header (tail)', 'TrDrte', 'Value'),\n",
+                "             ('header (tail)', 'NbTrchMod', 'Value'),\n",
+                "             ('header (tail)', 'OptimTrunc', 'Value')]\n",
+                "subsetCols=[col for col in refRes.columns if col[0] == ads.MCDSAnalysisResultsSet.CLCAutoFilSor]\n",
                 "subsetCols"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [],
             "source": [
-                "refRes.dfData.set_index(indexCols).sort_index()[subsetCols] \\\n",
-                "    .compare(res.dfData.set_index(indexCols).sort_index()[subsetCols])"
+                "dfComp = refRes.dfData.set_index(indexCols).sort_index()[subsetCols] \\\n",
+                "         .compare(res.dfData.set_index(indexCols).sort_index()[subsetCols])\n",
+                "dfComp #.to_excel('tmp/comp.xlsx')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "dfComp[[col for col in dfComp.columns if col[2] == 'Group']].dropna(how='all')"
+            ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ads.DataSet.compareDataFrames(refRes.dfTransData('fr').sort_values(by='NumAnlys'),\n",
-                "                              res.dfTransData('fr').sort_values(by='NumAnlys'),\n",
-                "                              indexCols=['NumAnlys'],\n",
-                "                              subsetCols=[col for col in refRes.dfTransData('fr').columns\n",
-                "                                          if col.startswith('Ordre') or col.startswith('Qual') or col.startswith('Groupe')],\n",
-                "                              dropCloser=14)"
+                "dfComp[[col for col in dfComp.columns if col[2] == 'Order' and '(close trunc)' in col[1]]].dropna(how='all')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "dfComp[[col for col in dfComp.columns if col[2] == 'Order' and '(global)' in col[1]]].dropna(how='all')"
+            ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [],
             "source": [
-                "### z. Finalisation"
+                "relDiffCols = ['Chi2 P', 'Delta AIC', 'Delta CoefVar Densit\u00e9',\n",
+                "               'Qual Equi 1', 'Qual Equi 2', 'Qual Equi 3', 'Qual Chi2+', 'Qual KS+', 'Qual DCv+']\n",
+                "ads.DataSet.compareDataFrames(refRes.dfTransData('fr').sort_values(by='DossierExec'),\n",
+                "                              res.dfTransData('fr').sort_values(by='DossierExec'),\n",
+                "                              indexCols=['DossierExec'],\n",
+                "                              subsetCols=relDiffCols, \n",
+                "                              dropCloser=14)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "optanlr.shutdown()"
+                "relDiffCols = ['TrGche', 'TrDrte', 'NbTrchMod', 'NTot Obs', 'Min Dist', 'Max Dist', 'NObs', 'NEchant', 'Effort',\n",
+                "               'TxContact', 'CoefVar TxContact', 'Min TxContact', 'Max TxContact', 'DegLib TxContact', \n",
+                "               'Taux Obs', 'NbTot Pars', 'AIC', 'AICc', 'BIC', 'LogProba', 'KS P', 'CvM Uw P', 'CvM Cw P',\n",
+                "               'f/h(0)', 'CoefVar f/h(0)', 'Min f/h(0)', 'Max f/h(0)', 'DegLib f/h(0)',\n",
+                "               'PDetec', 'CoefVar PDetec', 'Min PDetec', 'Max PDetec', 'DegLib PDetec',\n",
+                "               'EDR/ESW', 'CoefVar EDR/ESW', 'Min EDR/ESW', 'Max EDR/ESW', 'DegLib EDR/ESW',\n",
+                "               'DensClu', 'CoefVar DensClu', 'Min DensClu', 'Max DensClu', 'DegLib DensClu',\n",
+                "               'Densit\u00e9', 'Delta CoefVar Densit\u00e9', 'CoefVar Densit\u00e9', 'Min Densit\u00e9', 'Max Densit\u00e9', 'DegLib Densit\u00e9',\n",
+                "               'Nombre', 'CoefVar Nombre', 'Min Nombre', 'Max Nombre', 'DegLib Nombre']\n",
+                "ads.DataSet.compareDataFrames(refRes.dfTransData('fr').sort_values(by='DossierExec'),\n",
+                "                              res.dfTransData('fr').sort_values(by='DossierExec'),\n",
+                "                              indexCols=['DossierExec'],\n",
+                "                              subsetCols=relDiffCols, \n",
+                "                              dropCloser=14)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -7131,15 +7240,15 @@
                 "\n",
                 "def count2AdultCat(sCounts):\n",
                 "    return 'm' if 'Mal' in sCounts[sCounts > 0].index[0] else 'a'\n",
                 "\n",
                 "def count2DurationCat(sCounts):\n",
                 "    return '5mn' if '5' in sCounts[sCounts > 0].index[0] else '10mn'\n",
                 "\n",
-                "fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-ExtraitObsBrutesAvecDist.txt',\n",
+                "fds = ads.FieldDataSet(source='refin/ACDC2019-Naturalist-extrait-ObsBrutesAvecDist.txt',\n",
                 "                       importDecFields=['distMem'], countCols=countCols,\n",
                 "                       addMonoCatCols={ 'Adulte': count2AdultCat, 'Dur\u00e9e': count2DurationCat })\n",
                 "\n",
                 "dfObsIndiv = fds.individualise()\n",
                 "\n",
                 "dfObsIndiv.drop(columns=countCols, inplace=True)\n",
                 "\n",
@@ -7183,15 +7292,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfAnlysExplSpecs = ads.DSAnalyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx', \n",
+                "dfAnlysExplSpecs = ads.DSAnalyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.xlsx', \n",
                 "                                                        keep=['Echant1_impl', 'Echant2_impl', 'Modl_impl',\n",
                 "                                                              'Params1_expl', 'Params2_expl'],\n",
                 "                                                        varIndCol='IndAnlys',\n",
                 "                                                        #convertCols={ 'Dur\u00e9e': int }, # float 'cause of Excel\n",
                 "                                                        computedCols={anlysAbbrevCol: analysisAbbrev})"
             ]
         },
@@ -7382,14 +7491,23 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
+            "source": [
+                "anlysr.cleanup()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
             "source": []
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 2. MCDSAnalyser : Run multiple analyses on real-life data (2/2)\n",
@@ -7446,15 +7564,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "anlysSpecFile = 'refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx'"
+                "anlysSpecFile = 'refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.xlsx'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -7524,14 +7642,23 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "results.toExcel(pl.Path(anlysr.workDir) / 'unintst-mcds-anlyser-results2-fr.xlsx', lang='fr')"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "anlysr.cleanup()"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 3. MCDSPreAnalyser : Run multiple pre-analyses with real-life data"
             ]
         },
         {
@@ -7768,17 +7895,17 @@
                 "# Python 3.8, Windows 10, Core i5 8365U (4 HT cores, 1.6-4.1GHz, cache  6Mb, bus 4GT/s) + SSD 256Gb NVME + RAM 16Gb, \"optimal performances\" power scheme\n",
                 "# * 2021-01: 12 optimisations, 1430 analyses, 12 threads : subprocess = 3mn13, system = 2mn35, 1mn54?\n",
                 "# * 2021-10-02: idem : system 2mn15\n",
                 "# Python 3.8, Windows 10, Core i7 10850H (6 HT cores, 2.7-5.1GHz, cache 12Mb, bus 8GT/s) + SSD 512Gb NVME + RAM 32Gb \"optimal performances\" power scheme\n",
                 "# * 2023-11-02: 12 optimisations, 1434 analyses, 12 threads : system = 1mn44s, 1mn46s, subprocess = 1mn47s\n",
                 "#               (N.B. non saturant = max 6 MCDS en // observ\u00e9s => augmenter threads . jeu top petit ?)\n",
                 "\n",
-                "results = zoptr.run(dfOptimExplSpecs, threads=12)\n",
-                "\n",
-                "#results = zoptr.run(dfOptimExplSpecs.iloc[:3], threads=3)  # Small subset for quicker run."
+                "#results = zoptr.run(dfOptimExplSpecs.iloc[:3], threads=3)  # Small subset for quicker run.\n",
+                "#results = zoptr.run(dfOptimExplSpecs.iloc[:6], threads=6)  # Half subset for quicker run, with 1 recovery file.\n",
+                "results = zoptr.run(dfOptimExplSpecs, threads=12)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -7824,28 +7951,35 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# TODO: Check presence, mtime and content (optims Id lists) of $workDir/optr-resbak-*.pickle.xz\n",
-                "#with lzma.open(fileName, 'rb') as file:\n",
-                "#    dfData, specs = pickle.load(file)\n",
-                "#    \n",
-                "#len(dfData), dfData.columns, len(dfData.columns), dfData.columns.duplicated().any()"
+                "# i. Quickly check content of the recovery file\n",
+                "optResBkpPath = pl.Path(zoptr.workDir / 'optr-resbak-0.pickle.xz')\n",
+                "with lzma.open(optResBkpPath, 'rb') as file:\n",
+                "    dfData, specs = pickle.load(file)\n",
+                "assert len(dfData) == 17\n",
+                "exptdCols = [optIndCol] + sampleSelCols + optimParamsSpecsCols + [speAbbrevCol]\n",
+                "exptdCols += ['OptAbbrev', 'KeyFn', 'AdjSer', 'EstCrit', 'CVInt', 'OptCrit',\n",
+                "              'MinDist', 'MaxDist', 'FitDistCuts', 'DiscrDistCuts',\n",
+                "              'SetupStatus', 'SubmitStatus', 'NFunEvals', 'MeanFunElapd',\n",
+                "              '1-ks', 'maxDist', 'discrDistCuts', 'chi2', 'minDist',\n",
+                "              'fitDistCuts', 'ks', '1-chi2', 'cvmuw*cvmcw']\n",
+                "assert dfData.columns.tolist() == exptdCols"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Create the optimiser object : have to be a clone of the one whose execution that was backed up\n",
+                "# ii. Create the optimiser object : have to be a clone of the one whose execution was backed up\n",
                 "zoptr = ads.MCDSZerothOrderTruncationOptimiser \\\n",
                 "                (dfObsIndiv, effortConstVal=1, dSurveyArea=dSurveyArea, \n",
                 "                 transectPlaceCols=transectPlaceCols, passIdCol=passIdCol, effortCol=effortCol,\n",
                 "                 sampleSelCols=sampleSelCols, sampleDecCols=sampleDecCols, sampleDistCol=sampleDistCol,\n",
                 "                 anlysSpecCustCols=[speAbbrevCol], abbrevCol=optAbbrevCol, abbrevBuilder=analysisAbbrev,\n",
                 "                 anlysIndCol=optIndCol, sampleIndCol=sampleIndCol,\n",
                 "                 distanceUnit='Meter', areaUnit='Hectare',\n",
@@ -7866,18 +8000,18 @@
             "metadata": {
                 "scrolled": true
             },
             "outputs": [],
             "source": [
                 "%%time\n",
                 "\n",
-                "# Run optimisation with recovery results ... using exact same optim. specs (MANDATORY)\n",
-                "results2 = zoptr.run(dfOptimExplSpecs, recover=True, threads=12)\n",
-                "\n",
-                "#results2 = zoptr.run(dfOptimExplSpecs.iloc[:3], recover=True, threads=3)  # Petit sous-ensemble pour aller vite."
+                "# iii.Run optimisation with recovery results ... using exact same optim. specs (MANDATORY)\n",
+                "#results2 = zoptr.run(dfOptimExplSpecs.iloc[:3], recover=True, threads=3)  # Small subset for quicker run.\n",
+                "#results2 = zoptr.run(dfOptimExplSpecs.iloc[:3], recover=True, threads=3)  # Half subset for quicker run, with 1 recovery file.\n",
+                "results2 = zoptr.run(dfOptimExplSpecs, recover=True, threads=12)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -7896,22 +8030,53 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# TODO: Check equality of 1st 10 results in `results` and `results2`, + added num of results"
+                "results2.toExcel(pl.Path(zoptr.workDir) / 'unintst-mcds-optimiser-results2-fr.xlsx', lang='fr')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# iv. Quickly check results\n",
+                "assert len(results2) == 20 # Given the ParExec column of dfOptimExplSpecs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# v. Check equality of 1st 17 results in `results` and `results2`, + added num of results\n",
+                "# (20 results at the end, 1st 17 ones in backup file, so only reloaded => only 3 left to be recomputed)\n",
+                "dfComp = results.dfTransData(lang='fr').compare(results2.dfTransData(lang='fr'))\n",
+                "logger.info(f'First run vs recovery compared results: n={len(dfComp)} =>\\n' + dfComp.to_string())\n",
+                "\n",
+                "assert len(dfComp) <= 3"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 4. MCDSTruncationOptAnalyser : Run multiple analyses with optimised truncation params, on real-life data"
+                "## 5. MCDSTruncationOptAnalyser : Run multiple analyses with optimised truncation params, on real-life data"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Not implemented here (but see [valtests.ipynb](valtests.ipynb#IV.-Run-truncation-opt-analyses-with-same-real-life-field-data))"
@@ -7992,15 +8157,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Load individualised observations and actual transects\n",
-                "indivObsFile = 'refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods'\n",
+                "indivObsFile = 'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods'\n",
                 "\n",
                 "dfObsIndiv = ads.DataSet(indivObsFile, sheet='Donn\u00e9esIndiv').dfData\n",
                 "\n",
                 "dfTransects = ads.DataSet(indivObsFile, sheet='Inventaires').dfData\n",
                 "\n",
                 "dict(indivObs=len(dfObsIndiv), transects=len(dfTransects))"
             ]
@@ -8176,88 +8341,36 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": [
-                "np.ndarray()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "df = pd.DataFrame([dict(i=0, a=1, b=2, c=5), dict(i=1, a=3, b=4, c=10)])\n",
-                "df"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "def f(a):\n",
-                "    return a[1]*2+a[2], a[0]*4-a[2]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "df2 = df[['a', 'b', 'c']].apply(f, axis='columns', raw=True)\n",
-                "df.join(pd.DataFrame(df2.values, columns=['c', 'd'], index=df.index))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "df2"
-            ]
+            "source": []
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "cls = RS\n",
-                "CLsQuaIndicSources = [cls.CLKeyFn, cls.CLNAdjPars, cls.CLNTotPars, cls.CLNObs, cls.CLNTotObs,\n",
-                "                      cls.CLChi2, cls.CLKS, cls.CLCvMUw, cls.CLCvMCw, cls.CLDCv]\n",
-                "CINAdjPars = CLsQuaIndicSources.index(cls.CLNAdjPars)\n",
-                "CINAdjPars"
+                "# Sandbox"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": [
-                "a = np.array([1, 2, 3, 4, 5])\n",
-                "a"
-            ]
+            "source": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": [
-                "a[1:3].prod()"
-            ]
+            "source": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
```

### Comparing `pyaudisam-1.0.2/tests/unintval_utils.py` & `pyaudisam-1.1.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,81 @@
 # coding: utf-8
+
 # PyAuDiSam: Automation of Distance Sampling analyses with Distance software (http://distancesampling.org/)
 
 # Copyright (C) 2021 Jean-Philippe Meuret, Sylvain Sainnier
 
 # This program is free software: you can redistribute it and/or modify it under the terms
 # of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 
-# Common tools for automated unit, integration and validation tests
+# Pytest configuration file for all automated unit, integration and validation tests
 
+import sys
+import time
 import pathlib as pl
+import typing
+import pytest
 
-import pandas as pd
-
-import pyaudisam as ads
-
-
-# Useful test folders
+# The test root folder.
 pTestDir = pl.Path(__file__).parent
-pRefInDir = pl.Path('refin')
-pRefOutDir = pl.Path('refout')
 
-# Temporary work folder.
+# Temporary work folder root.
 pTmpDir = pTestDir / 'tmp'
 pTmpDir.mkdir(exist_ok=True)
 
-# Setup local logger
-_logger = ads.logger('uiv.tst')
+# Update PYTHONPATH for pyaudisam package to be importable.
+sys.path.insert(0, pTestDir.parent.as_posix())
+
+# Configure the logging system.
+from pyaudisam import log
+
+_logLevels = [dict(name='matplotlib', level=log.WARNING),
+              dict(name='ads', level=log.INFO)]
+_dateTime = time.strftime('%y%m%d.%H%M', time.localtime())
+pLogFile = pTmpDir / f'pytest.{_dateTime}.log'
+log.configure(loggers=_logLevels, handlers=[pLogFile], reset=True, verbose=True)
+
+# A plugin to make test report available to fixture ini/finalisation
+_phase_report_key = pytest.StashKey[typing.Dict[str, pytest.CollectReport]]()
+
+@pytest.hookimpl(wrapper=True, tryfirst=True)
+def pytest_runtest_makereport(item, call):
+
+    # Execute all other hooks to obtain the report object
+    rep = yield
+
+    # Store test results for each phase of a call, which can
+    # be "setup", "call", "teardown"
+    item.stash.setdefault(_phase_report_key, {})[rep.when] = rep
+
+    return rep
+
+# An auto-use function-scope fixture for logging its begin and end
+_logr = log.logger('uiv.tst')
+
+@pytest.fixture(autouse=True, scope='function')
+def inifinalizeFunction(request):
+
+    # Code that will run before the test function
+    _logr.info(f'Starting {request.node.nodeid} ...')
+
+    yield  # The test function will be run at this point
 
+    # Code that will run after the test function
+    report = request.node.stash[_phase_report_key]
+    if report['setup'].failed:
+        status = 'NOT SETUP'
+        details = report['setup'].longreprtext + '\n'
+    elif 'call' not in report:
+        status = 'SKIPPED'
+        details = ''
+    else:
+        status = report['call'].outcome.upper()
+        details = report['call'].longreprtext + '\n'
 
-# Create logger for tests and configure logging.
-def setupLogger(name, level=ads.DEBUG, otherLoggers={'ads': ads.INFO}):
-    logLevels = [dict(name='matplotlib', level=ads.WARNING),
-                 dict(name='ads', level=otherLoggers.get('ads', ads.INFO))] \
-                + [dict(name=nm, level=lvl) for nm, lvl in otherLoggers.items() if nm != 'ads'] \
-                + [dict(name='uiv.tst', level=level),
-                   dict(name=name, level=level)]
-    dateTime = pd.Timestamp.now().strftime('%Y%m%d%H%M')
-    fpnLogFile = pTmpDir / f'{name}.{dateTime}.log'
-    ads.log.configure(loggers=logLevels, handlers=[fpnLogFile], reset=True)
-
-    return ads.logger(name)
-
-
-# Show testing configuration (traceability).
-def logPlatform():
-    _logger.info('Testing platform:')
-    for k, v in ads.runtime:
-        if k != 'pyaudisam':
-            _logger.info(f'* {k}: {v}')
-    _logger.info(f'PyAuDiSam {ads.__version__} from {pl.Path(ads.__path__[0]).resolve().as_posix()}')
-
-
-# Log beginning of tests
-def logBegin(what):
-    _logger.info(f'Testing pyaudisam: {what} ...')
-
-
-# Log end of tests
-def logEnd(what, rc=None):
-    sts = {-1: 'Not run', 0: 'Success', None: None}.get(rc, 'Error')
-    msg = 'see pytest report' if sts is None else f'{sts} (code: {rc})'
-    _logger.info(f'Done testing pyaudisam: {what} => {msg}.')
+    _logr.info(f'Done ({status}) with {request.node.nodeid}\n{details}')
```

### Comparing `pyaudisam-1.0.2/tests/valarchives.ipynb` & `pyaudisam-1.1.0/tests/valarchives.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8748990379085488%*

 * *Differences: {"'cells'": '{134: {\'source\': {insert: [(0, "dfObsIndiv = '*

 * *            "ads.DataSet('refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods', "*

 * *            'sheet=\'DonnéesIndiv\').dfData\\n")], delete: [0]}}, 137: {\'source\': {insert: [(0, '*

 * *            '"dfTransects = ads.DataSet(\'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods\', '*

 * *            'sheet=\'Inventaires\').dfData\\n")], delete: [0]}}, 143: {\'source\': {insert: [(0, '*

 * *            '"dfRawOptimExplSpecs = '*

 * *            "ads.Analyser.explicitVariantS […]*

```diff
@@ -2124,15 +2124,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfObsIndiv = ads.DataSet('refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods', sheet='Donn\u00e9esIndiv').dfData\n",
+                "dfObsIndiv = ads.DataSet('refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods', sheet='Donn\u00e9esIndiv').dfData\n",
                 "dfObsIndiv"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -2152,15 +2152,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfTransects = ads.DataSet('refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods', sheet='Inventaires').dfData\n",
+                "dfTransects = ads.DataSet('refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods', sheet='Inventaires').dfData\n",
                 "dfTransects"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -2203,15 +2203,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfRawOptimExplSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx', \n",
+                "dfRawOptimExplSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.xlsx', \n",
                 "                                                        ignore=['Params3_expl'])\n",
                 "\n",
                 "# No use of these cols, as we'll compute them !\n",
                 "dfRawOptimExplSpecs = dfRawOptimExplSpecs.drop(columns=['TrGche', 'TrDrte', 'NbTrchMod']) \\\n",
                 "                                         .drop_duplicates().reset_index(drop=True)\n",
                 "\n",
                 "nOptimExplSpecs = len(dfRawOptimExplSpecs)"
@@ -2283,15 +2283,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfRawOptimExplSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx', \n",
+                "dfRawOptimExplSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-extrait-SpecsOptanalyses.xlsx', \n",
                 "                                                        ignore=['Params1_expl', 'Params2_expl'])\n",
                 "\n",
                 "dfRawOptimExplSpecs.drop(dfRawOptimExplSpecs[dfRawOptimExplSpecs[['TrGche', 'TrDrte', 'NbTrchMod', 'MultiOpt']]\n",
                 "                                    .isnull().all(axis='columns')].index,\n",
                 "                         inplace=True)\n",
                 "\n",
                 "dfRawOptimExplSpecs"
@@ -2422,15 +2422,15 @@
                 "**Target:**\n",
                 "* Computer: Windows 10, 4-core i5-8350U, PCI-e SSD, \"optimal performances\" power scheme\n",
                 "* runMethod: os.system\n",
                 "\n",
                 "**Variant 3a: \"all\"**\n",
                 "\n",
                 "* 22 analyses specs (12 parallel threads)\n",
-                "* Param\u00e8tres dans refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx nettoy\u00e9 de Param1_expl et Param2_expl.\n",
+                "* Param\u00e8tres dans refin/ACDC2019-Naturalist-extrait-SpecsOptanalyses.xlsx nettoy\u00e9 de Param1_expl et Param2_expl.\n",
                 "* MoteurOpt='zoopt(120)' => 2020-08-21 22:41:56,626 2880 analyses => 22 results, Wall time: 4min 21s\n",
                 "* MoteurOpt='zoopt(160)' => 2021-08-22 1920 analyses => 12 results, Wall time: 2min 44s\n",
                 "\n",
                 "**Variant 3b: \"main\"**\n",
                 "\n",
                 "* 12 analyses specs (6 parallel threads)\n",
                 "* CritChx='AIC', IntervConf=95, TroncGche='auto', TroncDrte='auto', MethOutliers='tucquant(2.5)', NbTrModel='mult(2/3, 3/2)', NbTrDiscr=None, ExprOpt='max(chi2)'\n",
@@ -2451,15 +2451,15 @@
                 "**Target:**\n",
                 "* Computer: Windows 10, 4-core i5-8350U, PCI-e SSD, \"optimal performances\" power scheme\n",
                 "* runMethod: subprocess.run\n",
                 "\n",
                 "**Variant 3a: \"all\"**\n",
                 "\n",
                 "* 12 analyses specs (12 parallel threads)\n",
-                "* Parameters from refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx, after removing Param1_expl and Param2_expl.\n",
+                "* Parameters from refin/ACDC2019-Naturalist-extrait-SpecsOptanalyses.xlsx, after removing Param1_expl and Param2_expl.\n",
                 "* Default: CritChx='AIC', IntervConf=95, MethOutliers='tucquant(7)', NbTrModel='mult(0.6, 1.4)', NbTrDiscr='mult(0.5, 1.2)', ExprOpt='max(chi2)'\n",
                 "* MoteurOpt='zoopt(100)' => 2021-01-14 10:52:28,040 1920 analyses => 12 results, Wall time: 3min 45s\n",
                 "* MoteurOpt='zoopt(100)' => 2021-08-22 10:52:28,040 1920 analyses => 12 results, Wall time: 3min 45s\n",
                 "\n",
                 "**Variant 3b: \"main\"**\n",
                 "\n",
                 "* 12 analyses specs (12 parallel threads)\n",
@@ -3014,15 +3014,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfOptimExplSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx', \n",
+                "dfOptimExplSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-extrait-SpecsOptanalyses.xlsx', \n",
                 "                                                     ignore=['Params1_expl', 'Params2_expl'])\n",
                 "\n",
                 "dfOptimExplSpecs.drop(dfOptimExplSpecs[dfOptimExplSpecs[['TrGche', 'TrDrte', 'NbTrchMod', 'MultiOpt']]\n",
                 "                                           .isnull().all(axis='columns')].index,\n",
                 "                      inplace=True)\n",
                 "\n",
                 "dfOptimExplSpecs.drop(columns=['TrGche', 'TrDrte', 'NbTrchMod', 'MultiOpt'], inplace=True)\n",
@@ -3840,9 +3840,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.8.2"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `pyaudisam-1.0.2/tests/valtests-ds-params.py` & `pyaudisam-1.1.0/tests/valtests-ds-params.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # coding: utf-8
 
 """Parameter module for command line validation tests of pyaudisam (for -p option)
 
-(as far as possible same data and parameters than in valtests.ipynb)
+(same data and parameters than in test_val_*.py test modules, and obsolete valtests.ipynb notebook)
 
 Parameters (pass them through -k key1=value1,key2=value2,... options to pyaudisam main command-line script):
 :param lang: report language, en or fr
 
 Usage (after cloning https://github.com/denmedius/pyaudisam to <pyaudisam dir>):
 * cd <pyaudisam dir>
 * python -m pyaudisam -p tests/valtests-ds-params -n -w tests/tmp/mcds-preanlr ...
   * -x/--distexport : export input files for manual analyses in Distance 6+ software
   * -e/--preanalyses : run pre-analyses for samples specified in this param file (see below)
   * -t/--prereports excel,html : generate english HTML and Excel reports of pre-analyses results
-  * -s/--speparams lang=fr -t/--prereports html : generate french HTML report of pre-analyses results
+  * -s/--speparams lang=fr -t/--prereports html : generate French HTML report of pre-analyses results
 * python -m pyaudisam -p tests/valtests-ds-params -n -w tests/tmp/mcds-anlr ...
   * -a/--analyses : run analyses specified in this param file (see below)
   * -r/--reports excel,html:mqua-r92 : generate auto-filtered Excel report (all filters)
      and HTML report (ExAicMQua-r920m6q3d12 filter)... of analyses results
 * python -m pyaudisam -p tests/valtests-ds-params -n -w tests/tmp/mcds-optanlr ...
   * -o/--optanalyses : run opt-analyses specified in this param file (see below)
   * -f/--optreports excel:full,html:r92,html:r96 : generate full Excel report and 2 HTML reports
      (ExAicMQua-r920m6q3d12 and ExAicMQua-r960m6q3d8 filters) ... of opt-analyses results
-* Note: if -u option not present, nothing actually run, no file written, only checks done and informations
+* Note: if -u option not present, nothing actually run, no file written, only checks done and information
   listed about what should happen if ... useful before jumping, isn't it ?
 """
 
 import pathlib as pl
 
 import pandas as pd
 
-# from pyaudisam import log
 from pyaudisam.optimisation import Interval
-from pyaudisam.optanalyser import MCDSTruncOptanalysisResultsSet as rs
+from pyaudisam.optanalyser import MCDSTruncOptanalysisResultsSet as RS
 
-# Pas d'autres fichiers de paramètres inclus ici via pyaudisam.utils.loadPythonData.
+# No other parameter files included here through pyaudisam.utils.loadPythonData.
 parameterFiles = []
 
 
 # Input data ##############################################
 
 instDir = pl.Path(__file__).parent
 
@@ -49,15 +48,15 @@
 speciesCol = 'Espèce'
 passIdCol = 'Passage'
 distanceCol = 'Distance'
 effortCol = 'Effort'
 transectPlaceCols = ['Point']  # Columns for identifying places of transects, whatever pass number
 
 # Survey field data: Individualised sightings + transects definition
-surveyDataFile = instDir / 'refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods'
+surveyDataFile = instDir / 'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods'
 indivDistDataSheet = 'DonnéesIndiv'
 transectsDataSheet = 'Inventaires'
 
 # DS analysis common parameters ##############################################
 # a. Input / output data
 
 # b. DS and run params
@@ -84,15 +83,15 @@
     sampAbbrev = '{}-{}-{}-{}'.format(abrvSpe, sSample.Passage.replace('+', ''),
                                       sSample.Adulte.replace('+', ''), sSample['Durée'])
     return sampAbbrev
 
 sampleSpecCustCols = []
 
 # b. Samples to analyse
-sampleSpecFile = instDir / 'refin/ACDC2019-Naturalist-ExtraitSpecsEchants.ods'
+sampleSpecFile = instDir / 'refin/ACDC2019-Naturalist-extrait-SpecsEchants.ods'
 
 # c. DS and run params
 preResultsHeadCols = dict(before=[sampleIndCol],
                           sample=sampleSelCols,
                           after=[sampleAbbrevCol] + sampleSpecCustCols)
 
 modelPreStrategy = [dict(keyFn=kf, adjSr=js, estCrit='AIC', cvInt=95)
@@ -111,97 +110,93 @@
     abbrevs = [sampleAbbrev(sAnlys)]
     abbrevs += [sAnlys['FonctionClé'][:3].lower(), sAnlys['SérieAjust'][:3].lower()]
     dTroncAbrv = {'l': 'TrGche' if 'TrGche' in sAnlys.index else 'TroncGche',
                   'r': 'TrDrte' if 'TrDrte' in sAnlys.index else 'TroncDrte',
                   'm': 'NbTrches' if 'NbTrches' in sAnlys.index else 'NbTrModel'
                   if 'NbTrModel' in sAnlys.index else 'NbTrchMod',
                   'd': 'NbTrDiscr'}
-    for abrv, name in dTroncAbrv.items():
+    for trAbrv, name in dTroncAbrv.items():
         if name in sAnlys.index and not pd.isnull(sAnlys[name]):
-            abbrevs.append('{}{}'.format(abrv, sAnlys[name][0].lower() if isinstance(sAnlys[name], str)
-                                                                       else int(sAnlys[name])))
+            nmAbrv = sAnlys[name][0].lower() if isinstance(sAnlys[name], str) else str(int(sAnlys[name]))
+            abbrevs.append(trAbrv + nmAbrv)
     return '-'.join(abbrevs)
 
-analysisIndCol = 'NumAnlys'  # Analysis abbreviation (computed through sampleAbbrev() below)
-analysisAbbrevCol = 'AbrevAnlys'  # Unique analysis Id (number)
+analysisIndCol = 'NumAnlys'  # Unique analysis Id (number)
+analysisAbbrevCol = 'AbrevAnlys'  # Analysis abbreviation (computed through analysisAbbrev() above)
 
 # b. DS and run params
 analysisSpecCustCols = []
 
 resultsHeadCols = dict(before=[analysisIndCol, sampleIndCol],
                        sample=sampleSelCols,
                        after=[analysisAbbrevCol] + analysisSpecCustCols)
 
 analysisParamCols = ['FonctionClé', 'SérieAjust', 'TrGche', 'TrDrte', 'NbTrchMod']
 
-defEstimKeyFn = 'HNORMAL'
-defEstimAdjustFn = 'COSINE'
+defEstimKeyFn = 'UNIFORM'
+defEstimAdjustFn = 'POLY'
 defEstimCriterion = 'AIC'
 defCVInterval = 95
 
 defMinDist = None
-defMaxDist = None,
+defMaxDist = None
 defFitDistCuts = None
 defDiscrDistCuts = None
 
 ldTruncIntrvSpecs = [dict(col='left', minDist=5.0, maxLen=5.0),
                      dict(col='right', minDist=25.0, maxLen=25.0)]
 truncIntrvEpsilon = 1e-6
 
 runAnalysisMethod = 'subprocess.run'
 runAnalysisTimeOut = 300
 logAnalysisData = False
 logAnalysisProgressEvery = 5
 
-# c. Analyses to run (reuse valtests notebook spec. file)
-_ddfAnlysSpecs = pd.read_excel(instDir / 'refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx', sheet_name=None)
-analysisSpecFile = instDir / 'tmp/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx'
-with pd.ExcelWriter(analysisSpecFile) as xlWrtr:
-    for sn in ['Echant1_impl', 'Echant2_impl', 'Modl_impl', 'Params1_expl', 'Params2_expl']:
-        _ddfAnlysSpecs[sn].to_excel(xlWrtr, sheet_name=sn, index=False)
+# c. Analyses to run (reuse val-tests spec. file)
+analysisSpecFile = instDir / 'refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.ods'
 
 # DS opt-analysis parameters ########################################################
 # a. Input / output data
 
 # b. DS and run params
 optAnalysisParamCols = ['FonctionClé', 'SérieAjust', 'TrGche', 'TrDrte', 'NbTrchMod', 'MultiOpt']
 optAnalysisSpecCustCols = []
 
 optResultsHeadCols = dict(before=[analysisIndCol, sampleIndCol],
                           sample=sampleSelCols,
                           after=['FonctionClé', 'SérieAjust', 'TrGche', 'TrDrte', 'NbTrchMod']
                                 + [analysisAbbrevCol] + optAnalysisSpecCustCols)
 
 runOptAnalysisMethod = 'subprocess.run'
-runOptAnalysisTimeOut = 300
+runOptAnalysisTimeOut = 120
 logOptAnalysisData = False
 logOptAnalysisProgressEvery = 5
 logOptimisationProgressEvery = 3
 backupOptimisationsEvery = 5
 
-defExpr2Optimise = 'chi2'
+defExpr2Optimise = 'balq3'  # Usable variables defined in MCDSTruncationOptimisation.AnlysResultsIndex
 defMinimiseExpr = False
 defOutliersMethod = 'tucquant'
 defOutliersQuantCutPct = 7
 defFitDistCutsFctr = Interval(min=0.6, max=1.4)
 defDiscrDistCutsFctr = Interval(min=0.5, max=1.2)
 
-defSubmitTimes = 1
+defSubmitTimes = 2
 defSubmitOnlyBest = None
 
 dDefSubmitOtherParams = dict()
 
 defCoreEngine = 'zoopt'
-defCoreMaxIters = 100
+defCoreMaxIters = 150
 defCoreTermExprValue = None
 defCoreAlgorithm = 'racos'
 defCoreMaxRetries = 0
 
-# c. Opt-analyses to run (reuse valtests notebook spec. file)
-optAnalysisSpecFile = instDir / 'refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx'
+# c. Opt-analyses to run (reuse valtests spec. file)
+optAnalysisSpecFile = instDir / 'refin/ACDC2019-Naturalist-extrait-SpecsOptAnalyses.ods'
 
 
 # Reports (all types) ##############################################################
 # Use pre-parameter 'lang' if available (you can pass it through -k lang=fr)
 studyLang = 'en' if 'lang' not in dir() else lang
 assert studyLang in ['en', 'fr']
 
@@ -217,238 +212,233 @@
                            plotLineWidth=1, plotDotWidth=4,
                            plotFontSizes=dict(title=11, axes=10, ticks=9, legend=10))
 
 # Column selection for the various report tables
 # a. Main HTML page (super-synthesis): Column 1 (top) for sample description
 preReportSampleCols = [('header (head)', sampleIndCol, 'Value')] \
                       + [('header (sample)', col, 'Value') for col in sampleSelCols] \
-                      + [rs.CLNTotObs, rs.CLMinObsDist, rs.CLMaxObsDist]
+                      + [RS.CLNTotObs, RS.CLMinObsDist, RS.CLMaxObsDist]
 
 # b. Main HTML page (super-synthesis): Column 1 (bottom) for analysis model parameters
-preReportParamCols = [rs.CLParEstKeyFn, rs.CLParEstAdjSer]  # rs.CLParEstCVInt, rs.CLParEstSelCrit]
+preReportParamCols = [RS.CLParEstKeyFn, RS.CLParEstAdjSer]  # RS.CLParEstCVInt, RS.CLParEstSelCrit]
 
 # c. Main HTML page (super-synthesis): Columns 2 & 3 for analysis results (columns 4, 5, & 6 for plots)
-preReportResultCols = [rs.CLRunStatus,
-                       rs.CLNObs, rs.CLEffort,
-                       rs.CLAic, rs.CLChi2, rs.CLKS, rs.CLDCv,
-                       rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3,
-                       rs.CLPDetec, rs.CLEswEdr,
-                       rs.CLDensity, rs.CLDensityMin, rs.CLDensityMax,
-                       rs.CLNumber, rs.CLNumberMin, rs.CLNumberMax]
+preReportResultCols = [RS.CLRunStatus,
+                       RS.CLNObs, RS.CLEffort,
+                       RS.CLAic, RS.CLChi2, RS.CLKS, RS.CLDCv,
+                       RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3,
+                       RS.CLPDetec, RS.CLEswEdr,
+                       RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+                       RS.CLNumber, RS.CLNumberMin, RS.CLNumberMax]
 
 # d. Detail HTML pages & Excel reports : Synthesis table
 preReportSynthCols = [('header (head)', sampleIndCol, 'Value')] \
                      + [('header (sample)', col, 'Value') for col in sampleSelCols] \
-                     + [rs.CLParEstKeyFn, rs.CLParEstAdjSer,
-                        rs.CLNTotObs, rs.CLNObs, rs.CLNTotPars, rs.CLEffort, rs.CLDeltaAic,
-                        rs.CLChi2, rs.CLKS, rs.CLCvMUw, rs.CLCvMCw, rs.CLDCv,
-                        rs.CLSightRate,
-                        rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3,
-                        rs.CLCmbQuaChi2, rs.CLCmbQuaKS, rs.CLCmbQuaDCv,
-                        rs.CLPDetec, rs.CLPDetecMin, rs.CLPDetecMax,
-                        rs.CLDensity, rs.CLDensityMin, rs.CLDensityMax,
-                        rs.CLNumber, rs.CLNumberMin, rs.CLNumberMax]
+                     + [RS.CLParEstKeyFn, RS.CLParEstAdjSer,
+                        RS.CLNTotObs, RS.CLNObs, RS.CLNTotPars, RS.CLEffort, RS.CLDeltaAic,
+                        RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw, RS.CLDCv,
+                        RS.CLSightRate,
+                        RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3,
+                        RS.CLCmbQuaChi2, RS.CLCmbQuaKS, RS.CLCmbQuaDCv,
+                        RS.CLPDetec, RS.CLPDetecMin, RS.CLPDetecMax,
+                        RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+                        RS.CLNumber, RS.CLNumberMin, RS.CLNumberMax]
 
 # e. Excel & HTML super-synthesis, synthesis & details : Sorting parameters.
 preReportSortCols = [('header (head)', sampleIndCol, 'Value')]
 preReportSortAscend = True
 
 preReportRebuild = False
 
 
 # Full reports ######################################################################
 # 1. Specific to analysis reports
 anlysFullReportStudyTitle = 'PyAuDiSam Validation: Analyses'
 anlysFullReportStudySubTitle = 'Global analysis full report'
 anlysFullReportAnlysSubTitle = 'Detailed report'
 anlysFullReportStudyDescr = 'Easy and parallel run through MCDSAnalyser'
-anlysFullReportStudyKeywords = 'pyaudisam, validation, analysis, full, report'
+anlysFullReportStudyKeywords = 'pyaudisam, validation, analysis'
 
 # 2. Specific to opt-analysis reports
 optAnlysFullReportStudyTitle = 'PyAuDiSam Validation: Opt-analyses'
 optAnlysFullReportStudySubTitle = 'Global opt-analysis full report'
 optAnlysFullReportAnlysSubTitle = 'Detailed report'
 optAnlysFullReportStudyDescr = 'Easy and parallel run through MCDSTruncationOptAnalyser'
-optAnlysFullReportStudyKeywords = 'pyaudisam, validation, opt-analysis, full, report'
+optAnlysFullReportStudyKeywords = 'pyaudisam, validation, opt-analysis'
 
 # 3. Common to analysis reports and opt-analysis reports
 # Plot parameters
 fullReportPlotParams = \
     dict(plotImgSize=(640, 400), superSynthPlotsHeight=288,
          plotImgFormat='png', plotImgQuality=90,
          plotLineWidth=1, plotDotWidth=4,
          plotFontSizes=dict(title=11, axes=10, ticks=9, legend=10))
 
 # Column selection for the various report tables
 # a. Main HTML page (super-synthesis): Column 1 (top) for sample description
 fullReportSampleCols = \
     [('header (head)', sampleIndCol, 'Value')] \
     + [('header (sample)', col, 'Value') for col in sampleSelCols] \
-    + [rs.CLNTotObs, rs.CLMinObsDist, rs.CLMaxObsDist]
+    + [RS.CLNTotObs, RS.CLMinObsDist, RS.CLMaxObsDist]
 
 # b. Main HTML page (super-synthesis): Column 1 (bottom) for analysis model parameters
 fullReportParamCols = \
-    [rs.CLParEstKeyFn, rs.CLParEstAdjSer,
-     # rs.CLParEstCVInt, rs.CLParEstSelCrit,
-     rs.CLParTruncLeft, rs.CLParTruncRight, rs.CLParModFitDistCuts]
+    [RS.CLParEstKeyFn, RS.CLParEstAdjSer,
+     # RS.CLParEstCVInt, RS.CLParEstSelCrit,
+     RS.CLParTruncLeft, RS.CLParTruncRight, RS.CLParModFitDistCuts]
 
 # c. Main HTML page (super-synthesis): Columns 2 & 3 for analysis results (columns 4, 5, & 6 for plots)
 fullReportResultCols = \
     [('header (head)', analysisIndCol, 'Value'),
-     rs.CLRunStatus,
-     rs.CLNObs, rs.CLEffort, rs.CLSightRate, rs.CLNAdjPars,
-     rs.CLAic, rs.CLChi2, rs.CLKS, rs.CLDCv,
-     rs.CLCmbQuaBal3, rs.CLCmbQuaBal2, rs.CLCmbQuaBal1,
-     rs.CLDensity, rs.CLDensityMin, rs.CLDensityMax,
-     rs.CLNumber, rs.CLNumberMin, rs.CLNumberMax,
-     rs.CLEswEdr, rs.CLPDetec]
+     RS.CLRunStatus,
+     RS.CLNObs, RS.CLEffort, RS.CLSightRate, RS.CLNAdjPars,
+     RS.CLAic, RS.CLChi2, RS.CLKS, RS.CLDCv,
+     RS.CLCmbQuaBal3, RS.CLCmbQuaBal2, RS.CLCmbQuaBal1,
+     RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+     RS.CLNumber, RS.CLNumberMin, RS.CLNumberMax,
+     RS.CLEswEdr, RS.CLPDetec]
 
 # d. Main & detail HTML pages & Excel reports : Synthesis table
 fullReportSynthCols = \
     [('header (head)', sampleIndCol, 'Value')] \
     + [('header (sample)', col, 'Value') for col in sampleSelCols] \
     + [('header (head)', analysisIndCol, 'Value')] + fullReportParamCols \
-    + [rs.CLNTotObs, rs.CLNObs, rs.CLNTotPars, rs.CLEffort,
-       rs.CLDeltaAic, rs.CLChi2, rs.CLKS, rs.CLCvMUw, rs.CLCvMCw, rs.CLDCv,
-       rs.CLPDetec, rs.CLPDetecMin, rs.CLPDetecMax,
-       rs.CLDensity, rs.CLDensityMin, rs.CLDensityMax,
-       rs.CLSightRate,
-       rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3,
-       rs.CLCmbQuaChi2, rs.CLCmbQuaKS, rs.CLCmbQuaDCv,
-       rs.CLGrpOrdSmTrAic,
-       rs.CLGrpOrdClTrChi2KSDCv,  # rs.CLGrpOrdClTrChi2,
-       rs.CLGrpOrdClTrDCv,
-       rs.CLGrpOrdClTrQuaBal1, rs.CLGrpOrdClTrQuaBal2, rs.CLGrpOrdClTrQuaBal3, rs.CLGrpOrdClTrQuaChi2,
-       rs.CLGrpOrdClTrQuaKS, rs.CLGrpOrdClTrQuaDCv,
-       rs.CLGblOrdChi2KSDCv, rs.CLGblOrdQuaBal1, rs.CLGblOrdQuaBal2, rs.CLGblOrdQuaBal3,
-       rs.CLGblOrdQuaChi2, rs.CLGblOrdQuaKS, rs.CLGblOrdQuaDCv,
-       rs.CLGblOrdDAicChi2KSDCv,
-       rs.CLRunFolder]
+    + [RS.CLNTotObs, RS.CLNObs, RS.CLNTotPars, RS.CLEffort,
+       RS.CLDeltaAic, RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw, RS.CLDCv,
+       RS.CLPDetec, RS.CLPDetecMin, RS.CLPDetecMax,
+       RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+       RS.CLSightRate,
+       RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3,
+       RS.CLCmbQuaChi2, RS.CLCmbQuaKS, RS.CLCmbQuaDCv,
+       RS.CLGrpOrdSmTrAic,
+       RS.CLGrpOrdClTrChi2KSDCv,  # RS.CLGrpOrdClTrChi2,
+       RS.CLGrpOrdClTrDCv,
+       RS.CLGrpOrdClTrQuaBal1, RS.CLGrpOrdClTrQuaBal2, RS.CLGrpOrdClTrQuaBal3, RS.CLGrpOrdClTrQuaChi2,
+       RS.CLGrpOrdClTrQuaKS, RS.CLGrpOrdClTrQuaDCv,
+       RS.CLGblOrdChi2KSDCv, RS.CLGblOrdQuaBal1, RS.CLGblOrdQuaBal2, RS.CLGblOrdQuaBal3,
+       RS.CLGblOrdQuaChi2, RS.CLGblOrdQuaKS, RS.CLGblOrdQuaDCv,
+       RS.CLGblOrdDAicChi2KSDCv,
+       RS.CLRunFolder]
 
 # e. Excel & HTML super-synthesis, synthesis & details : Sorting parameters.
 fullReportSortCols = \
     [('header (head)', sampleIndCol, 'Value')] \
-    + [rs.CLParTruncLeft, rs.CLParTruncRight,
-       rs.CLDeltaAic, rs.CLCmbQuaBal3]
+    + [RS.CLParTruncLeft, RS.CLParTruncRight,
+       RS.CLDeltaAic, RS.CLCmbQuaBal3]
 fullReportSortAscend = [True] * (len(fullReportSortCols) - 1) + [False]
 
 fullReportRebuild = False
 
 
 # Auto-filtered reports ######################################################################
 # a. Specific to analysis reports
 anlysFilsorReportStudyTitle = 'PyAuDiSam Validation: Analyses'
-anlysFilsorReportStudySubTitle = 'Global analysis auto-filtered report'
+anlysFilsorReportStudySubTitle = 'Auto-selection of best analysis results'
 anlysFilsorReportAnlysSubTitle = 'Detailed report'
-anlysFilsorReportStudyDescr = 'Automated filtering et sorting : method "{fsId}" ;' \
+anlysFilsorReportStudyDescr = 'Automated filtering and sorting: method "{fsId}" ;' \
                               ' after easy and parallel run through MCDSAnalyser'
-anlysFilsorReportStudyKeywords = 'pyaudisam, validation, analysis, auto-filter, report'
+anlysFilsorReportStudyKeywords = 'pyaudisam, validation, analysis, auto-filter'
 
 # c. Specific to opt-analysis reports
-optAnlysFilsorReportStudyTitle = 'PyAuDiSam Validation: Opt-analyses'
-optAnlysFilsorReportStudySubTitle = 'Global opt-analysis auto-filtered report'
+optAnlysFilsorReportStudyTitle = 'PyAuDiSam Validation: Analyses with optimised truncations'
+optAnlysFilsorReportStudySubTitle = 'Auto-selection of best opt-analysis results'
 optAnlysFilsorReportAnlysSubTitle = 'Detailed report'
-optAnlysFilsorReportStudyDescr = 'Automated filtering et sorting : method "{fsId}" ;' \
+optAnlysFilsorReportStudyDescr = 'Automated filtering and sorting: method "{fsId}" ;' \
                                  ' after easy and parallel run through MCDSTruncationOptAnalyser'
-optAnlysFilsorReportStudyKeywords = 'pyaudisam, validation, opt-analysis, auto-filter, report'
+optAnlysFilsorReportStudyKeywords = 'pyaudisam, validation, opt-analysis, auto-filter'
 
 # c. Common to analysis reports and opt-analysis reports
 filsorReportPlotParams = dict(plotImgSize=(640, 400), superSynthPlotsHeight=288,
                               plotImgFormat='png', plotImgQuality=90,
                               plotLineWidth=1, plotDotWidth=4,
                               plotFontSizes=dict(title=11, axes=10, ticks=9, legend=10))
 
 # Available filter & sort schemes
-_whichFinalQua = rs.CLCmbQuaBal3
+_whichFinalQua = RS.CLCmbQuaBal3
 _ascFinalQua = False
 
-_whichBestQua = [rs.CLGrpOrdClTrChi2KSDCv, rs.CLGrpOrdClTrDCv, _whichFinalQua,
-                rs.CLGrpOrdClTrQuaChi2, rs.CLGrpOrdClTrQuaKS, rs.CLGrpOrdClTrQuaDCv]
+_whichBestQua = [RS.CLGrpOrdClTrChi2KSDCv, RS.CLGrpOrdClTrDCv, _whichFinalQua,
+                 RS.CLGrpOrdClTrQuaChi2, RS.CLGrpOrdClTrQuaKS, RS.CLGrpOrdClTrQuaDCv]
 
-_dupSubset = [rs.CLNObs, rs.CLEffort, rs.CLDeltaAic, rs.CLChi2, rs.CLKS, rs.CLCvMUw, rs.CLCvMCw, rs.CLDCv, 
-              rs.CLPDetec, rs.CLPDetecMin, rs.CLPDetecMax, rs.CLDensity, rs.CLDensityMin, rs.CLDensityMax]
-_dDupRounds = {rs.CLDeltaAic: 1, rs.CLChi2: 2, rs.CLKS: 2, rs.CLCvMUw: 2, rs.CLCvMCw: 2, rs.CLDCv: 2, 
-               rs.CLPDetec: 3, rs.CLPDetecMin: 3, rs.CLPDetecMax: 3,
-               rs.CLDensity: 2, rs.CLDensityMin: 2, rs.CLDensityMax: 2}
+_dupSubset = [RS.CLNObs, RS.CLEffort, RS.CLDeltaAic, RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw, RS.CLDCv,
+              RS.CLPDetec, RS.CLPDetecMin, RS.CLPDetecMax, RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax]
+_dDupRounds = {RS.CLDeltaAic: 1, RS.CLChi2: 2, RS.CLKS: 2, RS.CLCvMUw: 2, RS.CLCvMCw: 2, RS.CLDCv: 2,
+               RS.CLPDetec: 3, RS.CLPDetecMin: 3, RS.CLPDetecMax: 3,
+               RS.CLDensity: 2, RS.CLDensityMin: 2, RS.CLDensityMax: 2}
 
 filsorReportSchemes = \
-    [dict(method=rs.filterSortOnExecCode,
+    [dict(method=RS.filterSortOnExecCode,
           deduplicate=dict(dupSubset=_dupSubset, dDupRounds=_dDupRounds),
           filterSort=dict(whichFinalQua=_whichFinalQua, ascFinalQua=_ascFinalQua),
-          preselCols=[rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3],
+          preselCols=[RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3],
           preselAscs=False, preselThrhs=0.2, preselNum=4),
-     dict(method=rs.filterSortOnExCAicMulQua,
+     dict(method=RS.filterSortOnExCAicMulQua,
           deduplicate=dict(dupSubset=_dupSubset, dDupRounds=_dDupRounds),
-          filterSort=dict(sightRate=90, nBestAIC=4, nBestQua=2, whichBestQua=_whichBestQua,
+          filterSort=dict(sightRate=87.5, nBestAIC=5, nBestQua=4, whichBestQua=_whichBestQua,
+                          nFinalRes=18, whichFinalQua=_whichFinalQua, ascFinalQua=_ascFinalQua),
+          preselCols=[RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3],
+          preselAscs=False, preselThrhs=0.2, preselNum=5),
+     dict(method=RS.filterSortOnExCAicMulQua,
+          deduplicate=dict(dupSubset=_dupSubset, dDupRounds=_dDupRounds),
+          filterSort=dict(sightRate=90, nBestAIC=4, nBestQua=3, whichBestQua=_whichBestQua,
                           nFinalRes=15, whichFinalQua=_whichFinalQua, ascFinalQua=_ascFinalQua),
-          preselCols=[rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3],
-          preselAscs=False, preselThrhs=0.2, preselNum=3),
-     dict(method=rs.filterSortOnExCAicMulQua,
+          preselCols=[RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3],
+          preselAscs=False, preselThrhs=0.2, preselNum=4),
+     dict(method=RS.filterSortOnExCAicMulQua,
           deduplicate=dict(dupSubset=_dupSubset, dDupRounds=_dDupRounds),
-          filterSort=dict(sightRate=92, nBestAIC=3, nBestQua=2, whichBestQua=_whichBestQua,
+          filterSort=dict(sightRate=92.5, nBestAIC=3, nBestQua=2, whichBestQua=_whichBestQua,
                           nFinalRes=12, whichFinalQua=_whichFinalQua, ascFinalQua=_ascFinalQua),
-          preselCols=[rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3],
-          preselAscs=False, preselThrhs=0.2, preselNum=3),
-     dict(method=rs.filterSortOnExCAicMulQua,
-          deduplicate=dict(dupSubset=_dupSubset, dDupRounds=_dDupRounds),
-          filterSort=dict(sightRate=94, nBestAIC=2, nBestQua=1, whichBestQua=_whichBestQua,
-                          nFinalRes=10, whichFinalQua=_whichFinalQua, ascFinalQua=_ascFinalQua),
-          preselCols=[rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3],
-          preselAscs=False, preselThrhs=0.2, preselNum=3),
-     dict(method=rs.filterSortOnExCAicMulQua,
-          deduplicate=dict(dupSubset=_dupSubset, dDupRounds=_dDupRounds),
-          filterSort=dict(sightRate=96, nBestAIC=2, nBestQua=1, whichBestQua=_whichBestQua,
-                          nFinalRes=8, whichFinalQua=_whichFinalQua, ascFinalQua=_ascFinalQua),
-          preselCols=[rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3],
+          preselCols=[RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3],
           preselAscs=False, preselThrhs=0.2, preselNum=3)]
 
 # Column selection for the various report tables
 # a. Main HTML page (super-synthesis): Column 1 (top) for sample description
 filsorReportSampleCols = \
     [('header (head)', sampleIndCol, 'Value')] \
     + [('header (sample)', col, 'Value') for col in sampleSelCols] \
-    + [rs.CLNTotObs, rs.CLMinObsDist, rs.CLMaxObsDist]
+    + [RS.CLNTotObs, RS.CLMinObsDist, RS.CLMaxObsDist]
 
 # b. Main HTML page (super-synthesis): Column 1 (bottom) for analysis model parameters
 filsorReportParamCols = \
     [('header (head)', analysisIndCol, 'Value'),
-     rs.CLParEstKeyFn, rs.CLParEstAdjSer,
-     # rs.CLParEstCVInt, rs.CLParEstSelCrit,
-     rs.CLParTruncLeft, rs.CLParTruncRight, rs.CLParModFitDistCuts]
+     RS.CLParEstKeyFn, RS.CLParEstAdjSer,
+     # RS.CLParEstCVInt, RS.CLParEstSelCrit,
+     RS.CLParTruncLeft, RS.CLParTruncRight, RS.CLParModFitDistCuts]
 
 # c. Main HTML page (super-synthesis): Columns 2 & 3 for analysis results (columns 4, 5, & 6 for plots)
 filsorReportResultCols = \
-    [rs.CLRunStatus,
-     rs.CLNObs, rs.CLEffort, rs.CLSightRate, rs.CLNAdjPars,
-     rs.CLAic, rs.CLChi2, rs.CLKS, rs.CLDCv,
-     rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3,
-     rs.CLEswEdr, rs.CLPDetec,
-     rs.CLDensity, rs.CLDensityMin, rs.CLDensityMax,
-     rs.CLNumber, rs.CLNumberMin, rs.CLNumberMax]
+    [RS.CLRunStatus,
+     RS.CLNObs, RS.CLEffort, RS.CLSightRate, RS.CLNAdjPars,
+     RS.CLAic, RS.CLChi2, RS.CLKS, RS.CLDCv,
+     RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3,
+     RS.CLEswEdr, RS.CLPDetec,
+     RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+     RS.CLNumber, RS.CLNumberMin, RS.CLNumberMax]
 
 # d. Main & detail HTML pages & Excel reports : Auto-filtered & synthesis tables
 filsorReportSynthCols = \
     [('header (head)', sampleIndCol, 'Value')] \
     + [('header (sample)', col, 'Value') for col in sampleSelCols] \
     + filsorReportParamCols \
-    + [rs.CLNTotObs, rs.CLNObs, rs.CLNTotPars, rs.CLEffort,
-       rs.CLDeltaAic, rs.CLChi2, rs.CLKS, rs.CLCvMUw, rs.CLCvMCw, rs.CLDCv,
-       rs.CLSightRate,
-       rs.CLCmbQuaBal1, rs.CLCmbQuaBal2, rs.CLCmbQuaBal3,
-       rs.CLCmbQuaChi2, rs.CLCmbQuaKS, rs.CLCmbQuaDCv,
-       rs.CLPDetec, rs.CLPDetecMin, rs.CLPDetecMax,
-       rs.CLDensity, rs.CLDensityMin, rs.CLDensityMax,
-       rs.CLNumber, rs.CLNumberMin, rs.CLNumberMax,
-       rs.CLGrpOrdSmTrAic,
-       rs.CLGrpOrdClTrChi2KSDCv,  # rs.CLGrpOrdClTrChi2,
-       rs.CLGrpOrdClTrDCv,
-       rs.CLGrpOrdClTrQuaBal1, rs.CLGrpOrdClTrQuaBal2, rs.CLGrpOrdClTrQuaBal3, rs.CLGrpOrdClTrQuaChi2,
-       rs.CLGrpOrdClTrQuaKS, rs.CLGrpOrdClTrQuaDCv,
-       rs.CLGblOrdChi2KSDCv, rs.CLGblOrdQuaBal1, rs.CLGblOrdQuaBal2, rs.CLGblOrdQuaBal3,
-       rs.CLGblOrdQuaChi2, rs.CLGblOrdQuaKS, rs.CLGblOrdQuaDCv,
-       rs.CLGblOrdDAicChi2KSDCv]
+    + [RS.CLOptimTruncFlag] \
+    + [RS.CLNTotObs, RS.CLNObs, RS.CLNTotPars, RS.CLEffort,
+       RS.CLDeltaAic, RS.CLChi2, RS.CLKS, RS.CLCvMUw, RS.CLCvMCw, RS.CLDCv,
+       RS.CLSightRate,
+       RS.CLCmbQuaBal1, RS.CLCmbQuaBal2, RS.CLCmbQuaBal3,
+       RS.CLCmbQuaChi2, RS.CLCmbQuaKS, RS.CLCmbQuaDCv,
+       RS.CLPDetec, RS.CLPDetecMin, RS.CLPDetecMax,
+       RS.CLDensity, RS.CLDensityMin, RS.CLDensityMax,
+       RS.CLNumber, RS.CLNumberMin, RS.CLNumberMax,
+       RS.CLGrpOrdSmTrAic,
+       RS.CLGrpOrdClTrChi2KSDCv,  # RS.CLGrpOrdClTrChi2,
+       RS.CLGrpOrdClTrDCv,
+       RS.CLGrpOrdClTrQuaBal1, RS.CLGrpOrdClTrQuaBal2, RS.CLGrpOrdClTrQuaBal3, RS.CLGrpOrdClTrQuaChi2,
+       RS.CLGrpOrdClTrQuaKS, RS.CLGrpOrdClTrQuaDCv,
+       RS.CLGblOrdChi2KSDCv, RS.CLGblOrdQuaBal1, RS.CLGblOrdQuaBal2, RS.CLGblOrdQuaBal3,
+       RS.CLGblOrdQuaChi2, RS.CLGblOrdQuaKS, RS.CLGblOrdQuaDCv,
+       RS.CLGblOrdDAicChi2KSDCv]
 
 # e. Excel & HTML super-synthesis, synthesis & details : Sorting parameters.
 filsorReportSortCols = [('header (head)', sampleIndCol, 'Value'), _whichFinalQua]
 filsorReportSortAscend = [True, False]
 
 filsorReportRebuild = False
```

### Comparing `pyaudisam-1.0.2/tests/valtests.ipynb` & `pyaudisam-1.1.0/tests/valtests.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9584949366381728%*

 * *Differences: {"'cells'": "{14: {'source': {insert: [(3, '* and a reference output file set, proved as OK by "*

 * *            "using it in Distance software ;\\n'), (4, '* automated comparison to reference is "*

 * *            "achieved at the end.\\n'), (5, '\\n'), (6, 'WARNING: \\n'), (7, '* Obsolete, as the "*

 * *            'same can be done through an MCDSPreAnalyser (see '*

 * *            '[II.4A.c.](#(option)-c.-Generate-input-files-for-manual-analyses-with-Distance-GUI) '*

 * *            "below).\\n'), (8, '* And ... such unit test […]*

```diff
@@ -87,14 +87,21 @@
             "source": [
                 "import pyaudisam as ads\n",
                 "\n",
                 "ads.runtime"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Commons"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create temporary directory if not yet done.\n",
                 "tmpDir = pl.Path('tmp')\n",
@@ -154,14 +161,58 @@
                 "    print('Backingup to', (tp / tn).as_posix())\n",
                 "    tpn = tp / tn\n",
                 "    shutil.copy(fpn, tpn)\n",
                 "    return tpn"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Short string for sample \"identification\"\n",
+                "def sampleAbbrev(sSample):\n",
+                "    \n",
+                "    abrvSpe = ''.join(word[:4].title() for word in sSample['Esp\u00e8ce'].split(' ')[:2])\n",
+                "    \n",
+                "    sampAbbrev = '{}-{}-{}-{}'.format(abrvSpe, sSample.Passage.replace('+', ''),\n",
+                "                                      sSample.Adulte.replace('+', ''), sSample['Dur\u00e9e'])\n",
+                "    \n",
+                "    return sampAbbrev"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Short string for analysis \"identification\"\n",
+                "def analysisAbbrev(sAnlys):\n",
+                "    \n",
+                "    # Sample abbreviation\n",
+                "    abbrevs = [sampleAbbrev(sAnlys)]\n",
+                "\n",
+                "    # Model + Parameters abbreviation\n",
+                "    abbrevs += [sAnlys['FonctionCl\u00e9'][:3].lower(), sAnlys['S\u00e9rieAjust'][:3].lower()]\n",
+                "    dTroncAbrv = { 'l': 'TrGche' if 'TrGche' in sAnlys.index else 'TroncGche',\n",
+                "                   'r': 'TrDrte' if 'TrDrte' in sAnlys.index else 'TroncDrte',\n",
+                "                   'm': 'NbTrches' if 'NbTrches' in sAnlys.index else 'NbTrModel'\n",
+                "                                   if 'NbTrModel' in sAnlys.index else  'NbTrchMod',\n",
+                "                   'd': 'NbTrDiscr' }\n",
+                "    for abrv, name in dTroncAbrv.items():\n",
+                "        if name in sAnlys.index and not pd.isnull(sAnlys[name]):\n",
+                "            abbrevs.append('{}{}'.format(abrv, sAnlys[name][0].lower() if isinstance(sAnlys[name], str)\n",
+                "                                               else int(sAnlys[name])))\n",
+                "   \n",
+                "    return '-'.join(abbrevs)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Jump to :\n",
                 "* [II. Run pre-analyses / 0. Data Description](#II.-Run-pre-analyses)\n",
                 "* [III. Run analyses with same real life field data / 0. Data Description](#III.-Run-analyses-with-same-real-life-field-data)\n",
                 "* [IV. Run truncation opt-analyses with same real life field data](#IV.-Run-truncation-opt-analyses-with-same-real-life-field-data)"
@@ -170,16 +221,20 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# I. Generate input files for manual analyses in Distance interactive software\n",
                 "\n",
                 "* through an Excel input field data file,\n",
-                "* and a reference output file set, prooved as OK by using it in Distance software ;\n",
-                "* automated comparison to reference is achied at the end."
+                "* and a reference output file set, proved as OK by using it in Distance software ;\n",
+                "* automated comparison to reference is achieved at the end.\n",
+                "\n",
+                "WARNING: \n",
+                "* Obsolete, as the same can be done through an MCDSPreAnalyser (see [II.4A.c.](#(option)-c.-Generate-input-files-for-manual-analyses-with-Distance-GUI) below).\n",
+                "* And ... such unit tests already done in unintests.ipynb and unint_engine_test.py !"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -274,31 +329,14 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Short string for sample \"identification\"\n",
-                "def sampleAbbrev(sSample):\n",
-                "    \n",
-                "    abrvSpe = ''.join(word[:4].title() for word in sSample['Esp\u00e8ce'].split(' ')[:2])\n",
-                "    \n",
-                "    sampAbbrev = '{}-{}-{}-{}'.format(abrvSpe, sSample.Passage.replace('+', ''),\n",
-                "                                      sSample.Adulte.replace('+', ''), sSample['Dur\u00e9e'])\n",
-                "    \n",
-                "    return sampAbbrev"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "transectPlaceCols = ['Point']\n",
                 "passIdCol = 'Passage'\n",
                 "effortCol = 'Effort'\n",
                 "\n",
                 "sampleDecCols = [effortCol, 'Distance']\n",
                 "\n",
                 "sampleNumCol = 'NumEchant'\n",
@@ -327,15 +365,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfObsIndiv = ads.DataSet('refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods', sheet='Donn\u00e9esIndiv').dfData\n",
+                "dfObsIndiv = ads.DataSet('refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods', sheet='Donn\u00e9esIndiv').dfData\n",
                 "dfObsIndiv"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -355,15 +393,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfTransects = ads.DataSet('refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods', sheet='Inventaires').dfData\n",
+                "dfTransects = ads.DataSet('refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods', sheet='Inventaires').dfData\n",
                 "dfTransects"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -427,23 +465,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "computed = False"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "workDir = tmpDir / 'mcds-preanlr'"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 4A. Or : Really run pre-analyses\n",
                 "\n",
                 "Note: The exact same results (implicit mode) can be produced through the command line :\n",
                 "```\n",
@@ -479,17 +508,33 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert len(preAnlysr.specs) == 17\n",
-                "\n",
-                "preAnlysr.specs"
+                "assert preAnlysr.specs == {\n",
+                "    'Zone': 'ACDC',\n",
+                "    'Surface': '2400',\n",
+                "    'distanceUnit': 'Meter',\n",
+                "    'areaUnit': 'Hectare',\n",
+                "    'runMethod': 'subprocess.run',\n",
+                "    'runTimeOut': 300,\n",
+                "    'surveyType': 'Point',\n",
+                "    'distanceType': 'Radial',\n",
+                "    'clustering': False,\n",
+                "    'defEstimKeyFn': 'UNIFORM',\n",
+                "    'defEstimAdjustFn': 'POLY',\n",
+                "    'defEstimCriterion': 'AIC',\n",
+                "    'defCVInterval': 95,\n",
+                "    'defMinDist': None,\n",
+                "    'defMaxDist': None,\n",
+                "    'defFitDistCuts': None,\n",
+                "    'defDiscrDistCuts': None\n",
+                "}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### b. Check pre-analyses specs"
@@ -520,17 +565,17 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### (option) c. Generate input files for manual analyses with Distance GUI\n",
                 "\n",
                 "(not needed for pre-analyses: here only for example)\n",
                 "\n",
-                "TODO: Make this a real validation and non-regression test with comparison of output to reference, as a replacement of I. above, which is more a unit test (to be moved to unintests notebook).\n",
-                "\n",
-                "Note: The exact same results can be produced through the command line:\n",
+                "Notes:\n",
+                "* Only minimalistic checks done here, as already more deeply tested in unintests.ipynb and unint_engine_test.py\n",
+                "* The exact same results can be produced through the command line:\n",
                 "```\n",
                 "$ cd ..\n",
                 "$ python -m pyaudisam -p tests/valtests-ds-params.py -w tests/tmp/mcds-preanlr -n --distexport -u\n",
                 "```"
             ]
         },
         {
@@ -541,14 +586,54 @@
             "source": [
                 "preAnlysr.exportDSInputData(dfExplSampleSpecs=dfExplSampleSpecs if specsAreExplicit else None,\n",
                 "                            implSampleSpecs=implSampleSpecs if not specsAreExplicit else None,\n",
                 "                            format='Distance')"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Check generated file list\n",
+                "expdGenFileNames = []\n",
+                "for esp in varEspeces:\n",
+                "    for pas in varPassages:\n",
+                "        for ad in varAdultes:\n",
+                "            for dur in varDurees:\n",
+                "                sampAbbrv = sampleAbbrev(pd.Series({'Esp\u00e8ce': esp, passIdCol: pas, 'Adulte': ad, 'Dur\u00e9e': dur}))\n",
+                "                fileName = f'{sampAbbrv}-dist.txt'\n",
+                "                expdGenFileNames.append(fileName)\n",
+                "                print('*', fileName)\n",
+                "assert all(fpn.name in expdGenFileNames for fpn in preAnlysr.workDir.glob('*-dist.txt'))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Check 1 generated file\n",
+                "sampAbbrv = sampleAbbrev(pd.Series({'Esp\u00e8ce': 'Luscinia megarynchos', 'Passage': 'a+b', 'Adulte': 'm', 'Dur\u00e9e': '10mn'}))\n",
+                "fpnSamp = preAnlysr.workDir / f'{sampAbbrv}-dist.txt'\n",
+                "dfSampDist = pd.read_csv(fpnSamp, sep='\\t', decimal=',')\n",
+                "dfSampDist\n",
+                "\n",
+                "assert len(dfSampDist) == 182\n",
+                "assert dfSampDist.columns.tolist() == ['Region*Label', 'Region*Area', 'Point transect*Label', 'Point transect*Survey effort', 'Observation*Radial distance']\n",
+                "assert dfSampDist['Point transect*Label'].nunique() == 96\n",
+                "assert all(dfSampDist['Region*Label'].unique() == [dSurveyArea['Zone']])\n",
+                "assert all(dfSampDist['Region*Area'].unique() == [int(dSurveyArea['Surface'])])\n",
+                "assert dfSampDist['Point transect*Survey effort'].sum() == 362\n",
+                "assert dfSampDist['Observation*Radial distance'].isnull().sum() == 26"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### d. Run pre-analyses"
             ]
         },
         {
@@ -574,15 +659,15 @@
             },
             "outputs": [],
             "source": [
                 "%%time\n",
                 "\n",
                 "preResults = preAnlysr.run(dfExplSampleSpecs if specsAreExplicit else None,\n",
                 "                           implSampleSpecs=implSampleSpecs if not specsAreExplicit else None, \n",
-                "                           dModelStrategy=modelStrategy, threads=6)\n",
+                "                           dModelStrategy=modelStrategy, threads=12)\n",
                 "\n",
                 "preAnlysr.shutdown()\n",
                 "\n",
                 "computed = True\n",
                 "\n",
                 "preResults.specs"
             ]
@@ -591,15 +676,20 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Performances figures on a Ruindows 10 laptop with PCI-e SSD, \"optimal performances\" power scheme, Python 3.8 :\n",
                 "* 4-HT-core i5-8350U:\n",
                 "  * 2021 (precise date ?): 50s to ~1mn10s elapsed for 12 samples, 6-12 threads\n",
                 "* 6-core i7-10750H (HT off):\n",
-                "  * 2022-01-17, 2023-11-02: 39-40s elapsed for 12 samples, 6-12 threads (N=5)"
+                "  * 2022-01-17, 2023-11-02: 39-40s elapsed for 12 samples, 6-12 threads (N=5)\n",
+                "\n",
+                "Performances figures on a Ruindows 11 laptop with PCI-e SSD, \"high performances\" power scheme, Python 3.8 :\n",
+                "* 6-core i7-10750H (HT on):\n",
+                "  * 2024-03-02: 40s elapsed for 12 samples, 6 threads (N=1)\n",
+                "  * 2024-03-02: 39s elapsed for 12 samples, 12 threads (N=1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -609,24 +699,36 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "preResults.dfTransData('fr')"
+                "preResults.dfData"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "preResults.dfData"
+                "dfFrRes = preResults.dfTransData('fr')\n",
+                "dfFrRes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for anlysFolderPath in dfFrRes.DossierExec:\n",
+                "    print(anlysFolderPath)\n",
+                "    assert {fpn.name for fpn in pl.Path(anlysFolderPath).iterdir()} == {'cmd.txt', 'data.txt', 'log.txt', 'output.txt', 'plots.txt', 'stats.txt'}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### e. Save results for later reload or examination"
@@ -767,15 +869,15 @@
             "outputs": [],
             "source": [
                 "# Load reference\n",
                 "# 1. Clone results _without_ data.\n",
                 "rsRef = preResults.copy(withData=False)\n",
                 "\n",
                 "# 2. Load it with reference data (prevent re-postComputation as this ref. file is old, with now missing computed cols)\n",
-                "rsRef.fromOpenDoc('refout/ACDC2019-Naturalist-ExtraitPreResultats.ods', postComputed=True)  \n",
+                "rsRef.fromOpenDoc('refout/ACDC2019-Naturalist-extrait-PreResultats.ods', postComputed=True)  \n",
                 "\n",
                 "rsRef.dfData"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -1085,41 +1187,14 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Short string for analysis \"identification\"\n",
-                "def analysisAbbrev(sAnlys):\n",
-                "    \n",
-                "    # Sample abbreviation\n",
-                "    abbrevs = [sampleAbbrev(sAnlys)]\n",
-                "\n",
-                "    # Model + Parameters abbreviation\n",
-                "    abbrevs += [sAnlys['FonctionCl\u00e9'][:3].lower(), sAnlys['S\u00e9rieAjust'][:3].lower()]\n",
-                "    dTroncAbrv = { 'l': 'TrGche' if 'TrGche' in sAnlys.index else 'TroncGche',\n",
-                "                   'r': 'TrDrte' if 'TrDrte' in sAnlys.index else 'TroncDrte',\n",
-                "                   'm': 'NbTrches' if 'NbTrches' in sAnlys.index else 'NbTrModel'\n",
-                "                                   if 'NbTrModel' in sAnlys.index else  'NbTrchMod',\n",
-                "                   'd': 'NbTrDiscr' }\n",
-                "    for abrv, name in dTroncAbrv.items():\n",
-                "        if name in sAnlys.index and not pd.isnull(sAnlys[name]):\n",
-                "            abbrevs.append('{}{}'.format(abrv, sAnlys[name][0].lower() if isinstance(sAnlys[name], str)\n",
-                "                                               else int(sAnlys[name])))\n",
-                "   \n",
-                "    return '-'.join(abbrevs)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "transectPlaceCols = ['Point']\n",
                 "passIdCol = 'Passage'\n",
                 "effortCol = 'Effort'\n",
                 "\n",
                 "sampleDecCols = [effortCol, 'Distance']\n",
                 "\n",
                 "sampleNumCol = 'NumEchant'\n",
@@ -1147,15 +1222,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfObsIndiv = ads.DataSet('refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods', sheet='Donn\u00e9esIndiv').dfData"
+                "dfObsIndiv = ads.DataSet('refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods', sheet='Donn\u00e9esIndiv').dfData"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1183,15 +1258,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfTransects = ads.DataSet('refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods', sheet='Inventaires').dfData\n",
+                "dfTransects = ads.DataSet('refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods', sheet='Inventaires').dfData\n",
                 "len(dfTransects)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -1209,15 +1284,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dfAnlysSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-ExtraitSpecsAnalyses.xlsx', \n",
+                "dfAnlysSpecs = ads.Analyser.explicitVariantSpecs('refin/ACDC2019-Naturalist-extrait-SpecsAnalyses.xlsx', \n",
                 "                                                 keep=['Echant1_impl', 'Echant2_impl', 'Modl_impl',\n",
                 "                                                       'Params1_expl', 'Params2_expl'],\n",
                 "                                                 varIndCol=varIndCol,\n",
                 "                                                 #convertCols={ 'Dur\u00e9e': int }, # float 'cause of Excel\n",
                 "                                                 computedCols={ anlysAbbrevCol: analysisAbbrev })\n",
                 "\n",
                 "len(dfAnlysSpecs)"
@@ -1371,14 +1446,15 @@
                 "* 6-HT-core i7-8850H (python 3.7?):\n",
                 "  * 2019 or 2020 before 06: min=5, max=11s elapsed for 64 analyses, 6 threads ?\n",
                 "* 4-HT-core i5-8350U (python 3.8):\n",
                 "  * 2021-01: min=5.3, max=5.7s elapsed for 48 analyses, 6 threads ?\n",
                 "  * 2021-10-02: min=4.2s, max=5.7s (n=3) elapsed for 48 analyses, 6 threads ?\n",
                 "* 6-core i7-10750H, HT disabled (python 3.8):\n",
                 "  * 2022-01-01: mean=3.4s (n=4) elapsed for 48 analyses, 6 threads\n",
+                "* 6-HT-core i7-10750H, HT on (python 3.8):\n",
                 "  * 2023-11-02: mean=3.1s (n=2) elapsed for 48 analyses, 6 threads"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -1547,15 +1623,15 @@
             "outputs": [],
             "source": [
                 "# Load reference\n",
                 "# 1. Clone results _without_ data.\n",
                 "rsRef = results.copy(withData=False)\n",
                 "\n",
                 "# 2. Load it with reference data (prevent re-postComputation as this ref. file is old, with now missing computed cols)\n",
-                "rsRef.fromFile('refout/ACDC2019-Naturalist-ExtraitResultats.ods', postComputed=True)\n",
+                "rsRef.fromFile('refout/ACDC2019-Naturalist-extrait-Resultats.ods', postComputed=True)\n",
                 "\n",
                 "rsRef.dfData"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -1954,16 +2030,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Les analyses \u00e0 faire (avec specs d'optimisation dedans si n\u00e9cessaire)\n",
-                "optanlysSpecFile = 'refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx'\n",
-                "#optanlysSpecFile = '../donnees/acdc/ACDC2019-Naturalist-ExtraitSpecsOptanalyses-reduit.ods'"
+                "optanlysSpecFile = 'refin/ACDC2019-Naturalist-extrait-SpecsOptanalyses.xlsx'\n",
+                "#optanlysSpecFile = '../donnees/acdc/ACDC2019-Naturalist-extrait-SpecsOptanalyses-reduit.ods'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1991,15 +2067,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Les donn\u00e9es individualis\u00e9es et transects\n",
-                "indivObsFile = 'refin/ACDC2019-Naturalist-ExtraitObsIndiv.ods'"
+                "indivObsFile = 'refin/ACDC2019-Naturalist-extrait-ObsIndiv.ods'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -2128,14 +2204,32 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert len(optanlr.specs) == 27"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "optanlr.specs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "type(optanlr.specs['defFitDistCutsFctr'])"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### b. Check opt-analyses specs"
             ]
         },
         {
@@ -2223,15 +2317,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Performances figures on a 4-HT-core i5-8365U Ruindows 10 laptop with PCI-e SSD, \"optimal performance power scheme\", 12 threads, Python 3.8 :\n",
                 "* 2021-01-05\n",
                 "  * OptAnalyserspecs: Zone=ACDC, Surface=2400, distanceUnit=Meter, areaUnit=Hectare, surveyType=Point, distanceType=Radial, clustering=False, defEstimKeyFn=HNORMAL, defEstimAdjustFn=COSINE, defEstimCriterion=AIC, defCVInterval=95, defMinDist=None, defMaxDist=None, defFitDistCuts=None, defDiscrDistCuts=None, defExpr2Optimise=chi2, defMinimiseExpr=False, dDefOptimCoreParams={'core': 'zoopt', 'maxIters': 100, 'termExprValue': None, 'algorithm': 'racos', 'maxRetries': 0}, defSubmitTimes=1, defSubmitOnlyBest=None, dDefSubmitOtherParams={}, defOutliersMethod=tucquant, defOutliersQuantCutPct=7, defFitDistCutsFctr=[0.6, 1.4], defDiscrDistCutsFctr=[0.5, 1.2]\n",
-                "  * OptAnalyses specs: 60 optimisations, from refin/ACDC2019-Naturalist-ExtraitSpecsOptanalyses.xlsx => 70 resultats,\n",
+                "  * OptAnalyses specs: 60 optimisations, from refin/ACDC2019-Naturalist-extrait-SpecsOptanalyses.xlsx => 70 resultats,\n",
                 "  * runMethod: subprocess.run => 4mn40, 4mn52, 4mn38, 4mn23, 4mn40, 5mn00, 4mn41, 4mn35, 4mn47 (mean 4mn42)\n",
                 "  * runMethod: os.system      => 4mn35, 4mn24, 4mn20, 4mn30 (mean 4mn27)\n",
                 "\n",
                 "* 2021-08-22, 2021-10-02\n",
                 "  * same OptAnalyserspecs, OptAnalyses specs\n",
                 "  * runMethod: subprocess.run => 4mn35 (n >= 2)\n",
                 "  \n",
@@ -2676,15 +2770,15 @@
             "outputs": [],
             "source": [
                 "# Load unoptimised reference\n",
                 "# 1. Clone optResults _without_ data.\n",
                 "rsUnoptRef = optResults.copy(withData=False)\n",
                 "\n",
                 "# 2. Load it with reference data (prevent re-postComputation as this ref. file is old, with now missing computed cols)\n",
-                "rsUnoptRef.fromOpenDoc('refout/ACDC2019-Naturalist-ExtraitResultats.ods', postComputed=True)\n",
+                "rsUnoptRef.fromOpenDoc('refout/ACDC2019-Naturalist-extrait-Resultats.ods', postComputed=True)\n",
                 "\n",
                 "unoptAnlysAbbrevs = list(rsUnoptRef.dfData[('header (tail)', anlysAbbrevCol, 'Value')])\n",
                 "\n",
                 "excludeUnoptCols = []\n",
                 "\n",
                 "len(unoptAnlysAbbrevs)"
             ]
@@ -3584,21 +3678,1141 @@
                 "dfRelDiff = \\\n",
                 "    ads.DataSet.compareDataFrames(dfAfsXlsxRefRes, dfAfsXlsxRes, indexCols=['UniqueId'], subsetCols=quaCols, dropCloser=14)\n",
                 "\n",
                 "assert dfRelDiff.empty  # Don't even think of it ..."
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Sandbox"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Opt-analysis results"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct = pd.read_excel('C:/git/pyaudisam/tests/tmp/valtests-optanalyses-results-api.xlsx', header=[0, 1, 2], skiprows=[3], index_col=0)\n",
+                "dfAct"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef = pd.read_excel('C:/git/pyaudisam/tests/refout/ACDC2019-Naturalist-extrait-OptResultats.ods', header=[0, 1, 2], skiprows=[3], index_col=0)\n",
+                "dfRef"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "optTruncFlagCol = ads.MCDSTruncationOptanalyser.OptimTruncFlagCol\n",
+                "dfRef = dfRef[dfRef[('header (tail)', optTruncFlagCol, 'Value')] == 0]\n",
+                "dfAct = dfAct[dfAct[('header (tail)', optTruncFlagCol, 'Value')] == 0]\n",
+                "len(dfRef), len(dfAct)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#dfRef.reset_index(inplace=True, drop=True)\n",
+                "#dfAct.reset_index(inplace=True, drop=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct.head(10)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct.to_excel('tmp/act.xlsx')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct[('header (tail)', 'AbrevAnlys', 'Value')]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef.head(10)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef.to_excel('tmp/ref.xlsx')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "indexCols = [('header (head)', 'NumAnlys', 'Value'),\n",
+                "             ('header (head)', 'NumEchant', 'Value'),\n",
+                "             ('header (sample)', 'Esp\u00e8ce', 'Value'),\n",
+                "             ('header (sample)', 'Passage', 'Value'),\n",
+                "             ('header (sample)', 'Adulte', 'Value'),\n",
+                "             ('header (sample)', 'Dur\u00e9e', 'Value'),\n",
+                "             ('header (tail)', 'FonctionCl\u00e9', 'Value'),\n",
+                "             ('header (tail)', 'S\u00e9rieAjust', 'Value'),\n",
+                "             ('header (tail)', 'TrGche', 'Value'),\n",
+                "             ('header (tail)', 'TrDrte', 'Value'),\n",
+                "             ('header (tail)', 'NbTrchMod', 'Value'),\n",
+                "             #('header (tail)', 'AbrevAnlys', 'Value'),\n",
+                "             ('parameters', 'estimator key function', 'Value'),\n",
+                "             ('parameters', 'estimator adjustment series', 'Value'),\n",
+                "             ('parameters', 'left truncation distance', 'Value'),\n",
+                "             ('parameters', 'right truncation distance', 'Value'),\n",
+                "             ('parameters', 'model fitting distance cut points', 'Value')]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "igndUnoptCols = [col for col in dfAct.columns.to_list() if col[2] == 'Order']  # TODO: Check why really.\n",
+                "subsetCols = [col for col in dfAct.columns.to_list()\n",
+                "              if col in dfRef.columns\n",
+                "              and col not in (indexCols + igndUnoptCols\n",
+                "                              + [('parameters', 'estimator selection criterion', 'Value'),\n",
+                "                                 ('run output', 'start time', 'Value'),\n",
+                "                                 ('run output', 'elapsed time', 'Value'),\n",
+                "                                 ('run output', 'run folder', 'Value'),\n",
+                "                                 ('detection probability', 'key function type', 'Value'),\n",
+                "                                 ('detection probability', 'adjustment series type', 'Value'),\n",
+                "                                 ('detection probability', 'Delta AIC', 'Value')])]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfDiff = ads.DataSet.compareDataFrames(dfAct, dfRef, subsetCols=subsetCols, indexCols=indexCols, noneIsNan=True, dropCloser=14, dropNans=True)\n",
+                "dfDiff"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfDiff.to_excel('tmp/diff.xlsx')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct.columns.to_list()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct = pd.read_excel('C:/git/pyaudisam/tests/tmp/valtests-optanalyses-results-api.xlsx', sheet_name='sp-analyser', index_col=0)\n",
+                "dfAct"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef = pd.read_excel('C:/git/pyaudisam/tests/refout/ACDC2019-Naturalist-extrait-OptResultats.ods', sheet_name='sp-analyser', index_col=0)\n",
+                "dfRef"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "s = pd.Series(dict(a='1', b=2))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "print(s.to_string())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActAnlysSpecs = pd.read_excel('C:/git/pyaudisam/tests/tmp/val-oanlr/valtests-optanalyses-results.xlsx', index_col=0, sheet_name='sp-analyses')\n",
+                "dfActAnlysSpecs = dfActAnlysSpecs[dfActAnlysSpecs.OptimTrunc == 1]\n",
+                "dfActAnlysSpecs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "set(dfActAnlysSpecs.MultiOpt.unique()) == {np.nan, 'times(2)', 'times(3, b=2)', 'times(4)'}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "anlysNOptParamCols = ['Esp\u00e8ce', 'Passage', 'Adulte', 'Dur\u00e9e', 'FonctionCl\u00e9', 'S\u00e9rieAjust']"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActMTimes = dfActAnlysSpecs[['NumAnlys', 'MultiOpt'] + anlysNOptParamCols].groupby(['NumAnlys'] + anlysNOptParamCols).count().replace(0, 1)\n",
+                "#dfActMTimes.reset_index(inplace=True)\n",
+                "#dfActMTimes.set_index('NumAnlys', inplace=True)\n",
+                "dfActMTimes.rename(columns=dict(MultiOpt='actualNTimes'), inplace=True)\n",
+                "dfActMTimes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActAnlysSpecs = dfActAnlysSpecs.set_index(['NumAnlys'] + anlysNOptParamCols).join(dfActMTimes)\n",
+                "dfActAnlysSpecs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def nTimes(mOpt):\n",
+                "    return 1 if pd.isnull(mOpt) else 2 if 'b=2' in mOpt or '(2)' in mOpt else 4 if '(4)' in mOpt else 0\n",
+                "dfActAnlysSpecs['exptdNTimes'] = dfActAnlysSpecs.MultiOpt.apply(nTimes)\n",
+                "dfActAnlysSpecs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActAnlysSpecs.actualNTimes.eq(dfActAnlysSpecs.exptdNTimes).all()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActAnlysSpecs.drop(columns=['actualNTimes', 'exptdNTimes', 'NTimes'], inplace=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfDiffStatHistory = pd.DataFrame(data=[dict(source='a', table='b', n=1, m=2, p='r')], index=[pd.Timestamp.now()])\n",
+                "dfDiffStatHistory"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfDiffStatHistory = pd.DataFrame()\n",
+                "dfDiffStatHistory"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfDiffStats = pd.DataFrame(data=[dict(p='t', n=4, m=7)], index=['mean'])\n",
+                "dfDiffStats"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dNewDiffStats.update(dfDiffStats.loc['mean'])\n",
+                "pd.concat([dfDiffStatHistory, pd.DataFrame([dNewDiffStats], index=[pd.Timestamp.now()])])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dNewDiffStats = dict(source='x', table='y')\n",
+                "dNewDiffStats.update(pd.Series(dict(n=9, p='y')))\n",
+                "pd.concat([dfDiffStatHistory, pd.DataFrame([dNewDiffStats], index=[pd.Timestamp.now()])])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dNewDiffStats = dict(source='x', table='y')\n",
+                "dNewDiffStats.update(pd.Series(dict(n=9, p='y', m=22, z=34)))\n",
+                "pd.concat([dfDiffStatHistory, pd.DataFrame([dNewDiffStats], index=[pd.Timestamp.now()])])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfDiffStats = pd.DataFrame(data=[dict(AIC=7, PDetect=1)], index=['mean'])\n",
+                "dfDiffStats"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dNewDiffStats = dict(source='x', table='y')\n",
+                "dNewDiffStats.update(dfDiffStats.loc['mean'].to_dict())\n",
+                "\n",
+                "fpnDiffStatHistory = 'tmp/dont-remove-valtests-optanalyses-opt-diff-stats-history.xlsx'\n",
+                "dfDiffStatHistory = pd.read_excel(fpnDiffStatHistory, index_col=0)\n",
+                "dfDiffStatHistory = pd.concat([dfDiffStatHistory, \n",
+                "                               pd.DataFrame(data=[dNewDiffStats],\n",
+                "                                            index=pd.Index([pd.Timestamp.now()], name='timestamp'))])\n",
+                "dfDiffStatHistory.to_excel('tmp/dont-remove-valtests-optanalyses-opt-diff-stats-history.test.xlsx', index=True)\n",
+                "dfDiffStatHistory"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pd.Index([pd.Timestamp.now()], name='timestamp')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Opt-analysis tabular workbook reports"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ddfRefRep = pd.read_excel('refout/ACDC2019-Naturalist-extrait-OptRapport.ods', sheet_name=None, index_col=0)\n",
+                "ddfRefRep.keys()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ddfActRep = pd.read_excel('tmp/val-oanlr/valtests-optanalyses-report.xlsx', sheet_name=None, index_col=0)\n",
+                "ddfActRep.keys()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "indexCols = ['Scheme', 'Step', 'Property']"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef = ddfRefRep['AFS-Steps'].reset_index(drop=True)\n",
+                "dfRef = dfRef[dfRef.Property != 'datetime'].copy()\n",
+                "dfRef"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRefPars = dfRef[dfRef.Property != 'results'].set_index(indexCols)\n",
+                "dfRefPars"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct = ddfActRep['AFS-Steps'].reset_index(drop=True)\n",
+                "dfAct = dfAct[dfAct.Property != 'datetime'].copy()\n",
+                "dfAct"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActPars = dfAct[dfAct.Property != 'results'].set_index(indexCols)\n",
+                "dfActPars"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfComp = dfRefPars.compare(dfActPars)\n",
+                "dfComp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRefRes = dfRef[dfRef.Property == 'results'].set_index(indexCols)\n",
+                "dfRefRes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActRes = dfAct[dfAct.Property == 'results'].set_index(indexCols)\n",
+                "dfActRes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfCompRes = dfRefRes.join(dfActRes, lsuffix=' Ref', rsuffix=' Act')\n",
+                "dfCompRes['Delta'] = dfCompRes['Value Ref'].subtract(dfCompRes['Value Act']).abs()\n",
+                "\n",
+                "KSDeltaResThresh = pd.Series({\n",
+                "    'before': 10,\n",
+                "    'run status': 5,\n",
+                "    'duplicates on params': 5,\n",
+                "    'best AIC': 5,\n",
+                "    'best results for >= 1 indicator': 5,\n",
+                "    'non-outlier sightings': 10,\n",
+                "    'final best results': 5,\n",
+                "    'after': 5,\n",
+                "}, name='Threshold')\n",
+                "dfCompRes = dfCompRes.reset_index().join(KSDeltaResThresh, on='Step').set_index(indexCols)\n",
+                "dfCompRes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef = ddfRefRep['Analyses']\n",
+                "dfRef"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct = ddfActRep['Analyses']\n",
+                "dfAct"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef = dfRef[dfRef.OptimTrunc == 1]\n",
+                "dfRef"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct = dfAct[dfAct.OptimTrunc == 1]\n",
+                "dfAct"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "optCols = ['TrGche', 'TrDrte', 'NbTrchMod']\n",
+                "unoptCols = [col for col in dfRef if col not in optCols]\n",
+                "dfRef = dfRef[unoptCols].drop_duplicates()\n",
+                "print(len(dfRef))\n",
+                "dfRef.set_index('NumAnlys')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfAct = dfAct[unoptCols].drop_duplicates()\n",
+                "print(len(dfAct))\n",
+                "dfAct.set_index('NumAnlys')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfComp = dfRef.compare(dfAct)\n",
+                "dfComp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sRefAnrSpecs = ddfRefRep['Analyser']['Value']\n",
+                "sRefAnrSpecs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sActAnrSpecs = ddfActRep['Analyser']['Value']\n",
+                "sActAnrSpecs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for anrSpecName in ['defFitDistCutsFctr', 'defDiscrDistCutsFctr']:\n",
+                "    if not isinstance(sActAnrSpecs[anrSpecName], str):\n",
+                "        sActAnrSpecs[anrSpecName] = str(sActAnrSpecs[anrSpecName])\n",
+                "\n",
+                "dfComp = sRefAnrSpecs.compare(sActAnrSpecs)\n",
+                "dfComp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRef = ddfRefRep['AFSM-ExAicMQua-r900m6q3d15'].reset_index()\n",
+                "dfRef"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [],
+            "source": [
+                "dfAct = ddfActRep['AFSM-ExAicMQua-r900m6q3d15'].reset_index()\n",
+                "dfAct"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sampleCols = ['NumEchant', 'Esp\u00e8ce', 'Passage', 'Adulte', 'Dur\u00e9e']\n",
+                "dfRefSampCnts = dfRef[sampleCols + ['Density']].groupby(sampleCols).count()\n",
+                "dfRefSampCnts.rename(columns=dict(Density='number'), inplace=True)\n",
+                "dfRefSampCnts"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActSampCnts = dfAct[sampleCols + ['Density']].groupby(sampleCols).count()\n",
+                "dfActSampCnts.rename(columns=dict(Density='number'), inplace=True)\n",
+                "dfActSampCnts"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRefSampCnts.subtract(dfActSampCnts).number.abs().lt(3).all()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#anlysNumCol = 'NumAnlys'\n",
+                "sampleNumCol = 'NumEchant'\n",
+                "sampleCols = [sampleNumCol, 'Esp\u00e8ce', 'Passage', 'Adulte', 'Dur\u00e9e']\n",
+                "# modelCols = ['Mod Key Fn', 'Mod Adj Ser']\n",
+                "indexCols = sampleCols # [anlysNumCol] + sampleCols  # + modelCols\n",
+                "compCols = ['Qual Bal 3', 'Qual Bal 2', 'Qual Bal 1', 'PDetec', 'Density']"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRefStats = dfRef[indexCols + compCols].groupby(indexCols).agg(['mean', 'std'])\n",
+                "dfRefStats.columns = [lvl0 + ' ' + lvl1 for lvl0, lvl1 in dfRefStats.columns]\n",
+                "dfRefStats"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActStats = dfAct[indexCols + compCols].groupby(indexCols).agg(['mean', 'std'])\n",
+                "dfActStats.columns = [lvl0 + ' ' + lvl1 for lvl0, lvl1 in dfActStats.columns]\n",
+                "dfActStats"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "compStatCols = dfActStats.columns.to_list()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfDiffStats = ads.DataSet.compareDataFrames(dfRefStats.reset_index(), dfActStats.reset_index(), indexCols=indexCols, subsetCols=compStatCols)\n",
+                "dfDiffStats"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sampleNumCol = 'NumEchant'\n",
+                "sampleCols = [sampleNumCol, 'Esp\u00e8ce', 'Passage', 'Adulte', 'Dur\u00e9e']\n",
+                "dfRefSampCnts = dfRef[sampleCols + ['Density']].groupby(sampleCols).count().rename(columns=dict(Density='count'))\n",
+                "dfRefSampCnts"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActSampCnts = dfAct[sampleCols + ['Density']].groupby(sampleCols).count()\n",
+                "dfActSampCnts.rename(columns=dict(Density='count'), inplace=True)\n",
+                "\n",
+                "dfActSampCnts"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Opt-analysis HTML reports"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf = pd.read_html('refout/ACDC2019-Naturalist-extrait-OptRapport.ExAicMQua-r900m6q3d15.html')\n",
+                "len(ldf)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldfTables = ldf"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "nResults = (len(ldfTables) - 9) // 3\n",
+                "nResults"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[0].values[:, 0]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[1]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[3]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[4]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pd.concat([ldf[i] for i in [2, 3, 4]]).set_index(0).loc[:, 1]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfRes = pd.DataFrame([pd.concat([ldf[subTblInd] for subTblInd in range(resInd, resInd + 3)]).set_index(0).loc[:, 1]\n",
+                "                      for resInd in range(2, 2 + 3 * nResults, 3)])\n",
+                "dfRes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "', '.join(ldf[2 + 87*3 + 0].columns)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 0].drop(columns=['Unnamed: 0']).set_index('NumEchant')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "', '.join(ldf[2 + 87*3 + 1].columns)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 1].drop(columns=['Unnamed: 0']).set_index('NumEchant')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 1][ ['Qual Bal 3', 'Qual Bal 2', 'Qual Bal 1', 'PDetec', 'Density']].dtypes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 2]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "indexCols = ['Scheme', 'Step', 'Property']\n",
+                "df = ldf[2 + 87*3 + 2]\n",
+                "df.columns = ['Scheme', 'Step', 'Property', 'Value']\n",
+                "dfActRes = df[df.Property == 'results'].set_index(indexCols)\n",
+                "dfActRes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dfActRes.Value[0]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 3]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 4]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 5].set_index('Unnamed: 0').Value"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 6]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ldf[2 + 87*3 + 7]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pd.Series(dtype=float)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "p.suffix"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "p.stem"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "p.parent"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
```


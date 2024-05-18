# Comparing `tmp/soxr-0.3.7.tar.gz` & `tmp/soxr-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soxr-0.3.7.tar", last modified: Thu Oct  5 01:57:30 2023, max compression
+gzip compressed data, was "soxr-0.4.0b1.tar", last modified: Sat May 18 09:20:09 2024, max compression
```

## Comparing `soxr-0.3.7.tar` & `soxr-0.4.0b1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.621770 soxr-0.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.601770 soxr-0.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.605770 soxr-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2023-10-05 01:57:13.000000 soxr-0.3.7/.github/workflows/build-dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-10-05 01:57:13.000000 soxr-0.3.7/.github/workflows/run-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-05 01:57:13.000000 soxr-0.3.7/BUILDING.md
--rw-r--r--   0 runner    (1001) docker     (127)    26432 2023-10-05 01:57:13.000000 soxr-0.3.7/COPYING.LGPL
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-10-05 01:57:13.000000 soxr-0.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-10-05 01:57:13.000000 soxr-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2023-10-05 01:57:30.621770 soxr-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-10-05 01:57:13.000000 soxr-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.605770 soxr-0.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-10-05 01:57:13.000000 soxr-0.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-05 01:57:13.000000 soxr-0.3.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-10-05 01:57:13.000000 soxr-0.3.7/docs/soxr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.605770 soxr-0.3.7/libsoxr/
--rw-r--r--   0 runner    (1001) docker     (127)    26432 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/COPYING.LGPL
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/LICENCE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.617770 soxr-0.3.7/libsoxr/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/aliases.h
--rw-r--r--   0 runner    (1001) docker     (127)      989 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/avfft32.c
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/avfft32s.c
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/ccrw2.h
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/cr-core.c
--rw-r--r--   0 runner    (1001) docker     (127)    22393 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/cr.c
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/cr.h
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/cr32.c
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/cr32s.c
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/cr64.c
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/cr64s.c
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/data-io.c
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/data-io.h
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/dbesi0.c
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/dev32s.h
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/dev64s.h
--rw-r--r--   0 runner    (1001) docker     (127)    37406 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/fft4g.c
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/fft4g.h
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/fft4g32.c
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/fft4g32s.c
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/fft4g64.c
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/fft4g_cache.h
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/fifo.h
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/filter.c
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/filter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/half-coefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/half-fir.h
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/internal.h
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/math-wrap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/pffft-avx.h
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/pffft-wrap.c
--rw-r--r--   0 runner    (1001) docker     (127)    68038 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/pffft.c
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/pffft.h
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/pffft32.c
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/pffft32s.c
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/pffft64s.c
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/poly-fir.h
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/poly-fir0.h
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/rdft.h
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/rdft_t.h
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/rint-clip.h
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/rint.h
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/samplerate.h
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/soxr-lsr.c
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/soxr-lsr.h
--rw-r--r--   0 runner    (1001) docker     (127)    22880 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/soxr.c
--rw-r--r--   0 runner    (1001) docker     (127)    13984 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/soxr.h
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/std-types.h
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/util-simd.c
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/util32s.c
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/util32s.h
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/util64s.c
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/util64s.h
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/vr-coefs.c
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/vr-coefs.h
--rw-r--r--   0 runner    (1001) docker     (127)    21401 2023-10-05 01:57:14.000000 soxr-0.3.7/libsoxr/src/vr32.c
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-10-05 01:57:13.000000 soxr-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-10-05 01:57:30.621770 soxr-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2023-10-05 01:57:13.000000 soxr-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.601770 soxr-0.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.621770 soxr-0.3.7/src/soxr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:13.000000 soxr-0.3.7/src/soxr/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2023-10-05 01:57:13.000000 soxr-0.3.7/src/soxr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-05 01:57:30.000000 soxr-0.3.7/src/soxr/_csoxr_version.c
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-05 01:57:30.000000 soxr-0.3.7/src/soxr/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-10-05 01:57:13.000000 soxr-0.3.7/src/soxr/csoxr.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-05 01:57:13.000000 soxr-0.3.7/src/soxr/csoxr_version.c
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-05 01:57:13.000000 soxr-0.3.7/src/soxr/csoxr_version.h
--rw-r--r--   0 runner    (1001) docker     (127)  1636624 2023-10-05 01:57:29.000000 soxr-0.3.7/src/soxr/cysoxr.c
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2023-10-05 01:57:13.000000 soxr-0.3.7/src/soxr/cysoxr.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-10-05 01:57:13.000000 soxr-0.3.7/src/soxr/soxr-config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.621770 soxr-0.3.7/src/soxr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2023-10-05 01:57:30.000000 soxr-0.3.7/src/soxr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-10-05 01:57:30.000000 soxr-0.3.7/src/soxr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 01:57:30.000000 soxr-0.3.7/src/soxr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 01:57:29.000000 soxr-0.3.7/src/soxr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-05 01:57:30.000000 soxr-0.3.7/src/soxr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-05 01:57:30.000000 soxr-0.3.7/src/soxr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:57:30.621770 soxr-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-10-05 01:57:13.000000 soxr-0.3.7/tests/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-10-05 01:57:13.000000 soxr-0.3.7/tests/bench_soxr_oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-10-05 01:57:13.000000 soxr-0.3.7/tests/test_resample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.343475 soxr-0.4.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.319475 soxr-0.4.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.323475 soxr-0.4.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-18 09:19:59.000000 soxr-0.4.0b1/.github/workflows/build-dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-18 09:19:59.000000 soxr-0.4.0b1/.github/workflows/run-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-18 09:19:59.000000 soxr-0.4.0b1/BUILDING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    26432 2024-05-18 09:19:59.000000 soxr-0.4.0b1/COPYING.LGPL
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-18 09:19:59.000000 soxr-0.4.0b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-18 09:19:59.000000 soxr-0.4.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-18 09:20:09.343475 soxr-0.4.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-18 09:19:59.000000 soxr-0.4.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.323475 soxr-0.4.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-18 09:19:59.000000 soxr-0.4.0b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 09:19:59.000000 soxr-0.4.0b1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-18 09:19:59.000000 soxr-0.4.0b1/docs/soxr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.323475 soxr-0.4.0b1/libsoxr/
+-rw-r--r--   0 runner    (1001) docker     (127)    26432 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/COPYING.LGPL
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/LICENCE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.335475 soxr-0.4.0b1/libsoxr/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/aliases.h
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/avfft32.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/avfft32s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/ccrw2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/cr-core.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/cr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/cr.h
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/cr32.c
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/cr32s.c
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/cr64.c
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/cr64s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/data-io.c
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/data-io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/dbesi0.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/dev32s.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/dev64s.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37406 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/fft4g.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/fft4g.h
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/fft4g32.c
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/fft4g32s.c
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/fft4g64.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/fft4g_cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/fifo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/filter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/filter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/half-coefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/half-fir.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/math-wrap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/pffft-avx.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/pffft-wrap.c
+-rw-r--r--   0 runner    (1001) docker     (127)    68038 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/pffft.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/pffft.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/pffft32.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/pffft32s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/pffft64s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/poly-fir.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/poly-fir0.h
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/rdft.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/rdft_t.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/rint-clip.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/rint.h
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/samplerate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/soxr-lsr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/soxr-lsr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22880 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/soxr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13984 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/soxr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/std-types.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/util-simd.c
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/util32s.c
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/util32s.h
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/util64s.c
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/util64s.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/vr-coefs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/vr-coefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21401 2024-05-18 09:19:59.000000 soxr-0.4.0b1/libsoxr/src/vr32.c
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-18 09:19:59.000000 soxr-0.4.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-18 09:20:09.343475 soxr-0.4.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-18 09:19:59.000000 soxr-0.4.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.319475 soxr-0.4.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.339475 soxr-0.4.0b1/src/soxr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:19:59.000000 soxr-0.4.0b1/src/soxr/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-18 09:19:59.000000 soxr-0.4.0b1/src/soxr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-18 09:20:09.000000 soxr-0.4.0b1/src/soxr/_csoxr_version.c
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-18 09:20:09.000000 soxr-0.4.0b1/src/soxr/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-18 09:19:59.000000 soxr-0.4.0b1/src/soxr/csoxr.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-18 09:19:59.000000 soxr-0.4.0b1/src/soxr/csoxr_version.c
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 09:19:59.000000 soxr-0.4.0b1/src/soxr/csoxr_version.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1668371 2024-05-18 09:20:08.000000 soxr-0.4.0b1/src/soxr/cysoxr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-18 09:19:59.000000 soxr-0.4.0b1/src/soxr/cysoxr.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-18 09:19:59.000000 soxr-0.4.0b1/src/soxr/soxr-config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.343475 soxr-0.4.0b1/src/soxr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-18 09:20:09.000000 soxr-0.4.0b1/src/soxr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-18 09:20:09.000000 soxr-0.4.0b1/src/soxr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:20:09.000000 soxr-0.4.0b1/src/soxr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:20:08.000000 soxr-0.4.0b1/src/soxr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-18 09:20:09.000000 soxr-0.4.0b1/src/soxr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 09:20:09.000000 soxr-0.4.0b1/src/soxr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:20:09.343475 soxr-0.4.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-18 09:19:59.000000 soxr-0.4.0b1/tests/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-18 09:19:59.000000 soxr-0.4.0b1/tests/bench_soxr_oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-18 09:19:59.000000 soxr-0.4.0b1/tests/test_resample.py
```

### Comparing `soxr-0.3.7/.github/workflows/build-dist.yml` & `soxr-0.4.0b1/.github/workflows/build-dist.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,87 +12,89 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-20.04, windows-2019, macos-11]
+        os: [ubuntu-22.04, windows-2022, macos-13]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           submodules: true
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16.2
+        uses: pypa/cibuildwheel@v2.16.5
         env:
           # Skip builds(save time / avoid build error)
-          CIBW_SKIP: "cp36-* pp* *-musllinux_* *_i686 *-win32"
+          CIBW_SKIP: "pp* *-musllinux_* *_i686 *-win32"
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_BUILD_FRONTEND: "build"
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: ${{ matrix.os }}
           path: ./wheelhouse/*.whl
 
       - uses: softprops/action-gh-release@v1
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
         with:
           files: ./wheelhouse/*.whl
 
   build_archs:
     name: Build wheels manylinux_aarch64
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           submodules: true
 
       - name: Set up QEMU
-        uses: docker/setup-qemu-action@v2
+        uses: docker/setup-qemu-action@v3
         with:
           platforms: all
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16.2
+        uses: pypa/cibuildwheel@v2.16.5
         env:
           CIBW_ARCHS_LINUX: aarch64
           CIBW_BUILD: cp*-manylinux_aarch64
-          CIBW_SKIP: "cp36-*"
           CIBW_BUILD_FRONTEND: "build"
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: archs
           path: ./wheelhouse/*.whl
 
       - uses: softprops/action-gh-release@v1
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
         with:
           files: ./wheelhouse/*.whl
 
   build_sdist:
     name: Build source distribution
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           submodules: true
 
       - name: Build sdist
         run: |
           python -m pip install build
           python -m build --sdist
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: sdist
           path: dist/*.tar.gz
 
       - uses: softprops/action-gh-release@v1
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
         with:
           files: dist/*.tar.gz
 
@@ -100,20 +102,19 @@
     needs: [build_wheels, build_archs, build_sdist]
     runs-on: ubuntu-latest
     # upload to PyPI on every tag starting with 'v'
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
     # alternatively, to publish when a GitHub Release is created, use the following rule:
     # if: github.event_name == 'release' && github.event.action == 'published'
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          # unpacks default artifact into dist/
-          # if `name: artifact` is omitted, the action will create extra parent dir
-          name: artifact
           path: dist
+          pattern: "*"
+          merge-multiple: true
 
       - uses: pypa/gh-action-pypi-publish@v1.8.8
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
           # To test
           # password: ${{ secrets.TEST_PYPI_API_TOKEN }}
```

### Comparing `soxr-0.3.7/.github/workflows/run-test.yml` & `soxr-0.4.0b1/.github/workflows/run-test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     strategy:
       matrix:
         python-version: ["3.9", "3.10", "3.11", "3.12", "pypy3.9"]
         os: [ubuntu-latest, windows-latest, macos-latest]
     runs-on: ${{ matrix.os }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         submodules: true
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install library
       run: |
         python -m pip install --upgrade pip
         python -m pip install .[test]
```

### Comparing `soxr-0.3.7/BUILDING.md` & `soxr-0.4.0b1/BUILDING.md`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/COPYING.LGPL` & `soxr-0.4.0b1/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/LICENSE.txt` & `soxr-0.4.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/PKG-INFO` & `soxr-0.4.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soxr
-Version: 0.3.7
+Version: 0.4.0b1
 Summary: High quality, one-dimensional sample-rate conversion library
 Home-page: https://github.com/dofuuz/python-soxr
 Author: Myungchul Keum
 License: LGPLv2.1+
 Project-URL: Documentation, https://python-soxr.readthedocs.io
 Project-URL: Source, https://github.com/dofuuz/python-soxr
 Project-URL: Bug Tracker, https://github.com/dofuuz/python-soxr/issues
@@ -16,15 +16,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: COPYING.LGPL
 Requires-Dist: numpy
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
```

### Comparing `soxr-0.3.7/README.md` & `soxr-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/docs/conf.py` & `soxr-0.4.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/COPYING.LGPL` & `soxr-0.4.0b1/libsoxr/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/LICENCE` & `soxr-0.4.0b1/libsoxr/LICENCE`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/aliases.h` & `soxr-0.4.0b1/libsoxr/src/aliases.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/avfft32.c` & `soxr-0.4.0b1/libsoxr/src/avfft32.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/avfft32s.c` & `soxr-0.4.0b1/libsoxr/src/avfft32s.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/ccrw2.h` & `soxr-0.4.0b1/libsoxr/src/ccrw2.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/cr-core.c` & `soxr-0.4.0b1/libsoxr/src/cr-core.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/cr.c` & `soxr-0.4.0b1/libsoxr/src/cr.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/cr.h` & `soxr-0.4.0b1/libsoxr/src/cr.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/data-io.c` & `soxr-0.4.0b1/libsoxr/src/data-io.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/data-io.h` & `soxr-0.4.0b1/libsoxr/src/data-io.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/dbesi0.c` & `soxr-0.4.0b1/libsoxr/src/dbesi0.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/dev32s.h` & `soxr-0.4.0b1/libsoxr/src/dev32s.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/dev64s.h` & `soxr-0.4.0b1/libsoxr/src/dev64s.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/fft4g.c` & `soxr-0.4.0b1/libsoxr/src/fft4g.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/fft4g.h` & `soxr-0.4.0b1/libsoxr/src/fft4g.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/fft4g32.c` & `soxr-0.4.0b1/libsoxr/src/fft4g32.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/fft4g32s.c` & `soxr-0.4.0b1/libsoxr/src/fft4g32s.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/fft4g64.c` & `soxr-0.4.0b1/libsoxr/src/fft4g64.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/fft4g_cache.h` & `soxr-0.4.0b1/libsoxr/src/fft4g_cache.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/fifo.h` & `soxr-0.4.0b1/libsoxr/src/fifo.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/filter.c` & `soxr-0.4.0b1/libsoxr/src/filter.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/filter.h` & `soxr-0.4.0b1/libsoxr/src/filter.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/half-coefs.h` & `soxr-0.4.0b1/libsoxr/src/half-coefs.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/half-fir.h` & `soxr-0.4.0b1/libsoxr/src/half-fir.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/internal.h` & `soxr-0.4.0b1/libsoxr/src/internal.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/math-wrap.h` & `soxr-0.4.0b1/libsoxr/src/math-wrap.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/pffft-avx.h` & `soxr-0.4.0b1/libsoxr/src/pffft-avx.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/pffft-wrap.c` & `soxr-0.4.0b1/libsoxr/src/pffft-wrap.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/pffft.c` & `soxr-0.4.0b1/libsoxr/src/pffft.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/pffft.h` & `soxr-0.4.0b1/libsoxr/src/pffft.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/pffft32.c` & `soxr-0.4.0b1/libsoxr/src/pffft32.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/pffft32s.c` & `soxr-0.4.0b1/libsoxr/src/pffft32s.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/pffft64s.c` & `soxr-0.4.0b1/libsoxr/src/pffft64s.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/poly-fir.h` & `soxr-0.4.0b1/libsoxr/src/poly-fir.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/poly-fir0.h` & `soxr-0.4.0b1/libsoxr/src/poly-fir0.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/rdft.h` & `soxr-0.4.0b1/libsoxr/src/rdft.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/rdft_t.h` & `soxr-0.4.0b1/libsoxr/src/rdft_t.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/rint-clip.h` & `soxr-0.4.0b1/libsoxr/src/rint-clip.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/rint.h` & `soxr-0.4.0b1/libsoxr/src/rint.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/soxr-lsr.c` & `soxr-0.4.0b1/libsoxr/src/soxr-lsr.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/soxr-lsr.h` & `soxr-0.4.0b1/libsoxr/src/soxr-lsr.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/soxr.c` & `soxr-0.4.0b1/libsoxr/src/soxr.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/soxr.h` & `soxr-0.4.0b1/libsoxr/src/soxr.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/std-types.h` & `soxr-0.4.0b1/libsoxr/src/std-types.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/util-simd.c` & `soxr-0.4.0b1/libsoxr/src/util-simd.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/util32s.h` & `soxr-0.4.0b1/libsoxr/src/util32s.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/util64s.h` & `soxr-0.4.0b1/libsoxr/src/util64s.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/vr-coefs.c` & `soxr-0.4.0b1/libsoxr/src/vr-coefs.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/vr-coefs.h` & `soxr-0.4.0b1/libsoxr/src/vr-coefs.h`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/libsoxr/src/vr32.c` & `soxr-0.4.0b1/libsoxr/src/vr32.c`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/setup.cfg` & `soxr-0.4.0b1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 	Programming Language :: C
 	Programming Language :: Cython
 	Programming Language :: Python :: 3
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = >= 3.6
+python_requires = >= 3.9
 install_requires = 
 	numpy
 packages = find:
 package_dir = 
 	=src
 
 [options.packages.find]
```

### Comparing `soxr-0.3.7/setup.py` & `soxr-0.4.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/src/soxr/__init__.py` & `soxr-0.4.0b1/src/soxr/__init__.py`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/src/soxr/csoxr.pxd` & `soxr-0.4.0b1/src/soxr/csoxr.pxd`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/src/soxr/cysoxr.c` & `soxr-0.4.0b1/src/soxr/cysoxr.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* Generated by Cython 3.0.2 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-hfz5eyov/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-hfz5eyov/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-hfz5eyov/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-hfz5eyov/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-hfz5eyov/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/_core/include/numpy/arrayobject.h",
+            "/tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/_core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/_core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/_core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/_core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-DSOXR_LIB",
             "-std=gnu99",
             "-Werror=implicit"
         ],
         "include_dirs": [
             "libsoxr/src",
             "src/soxr",
-            "/tmp/build-env-hfz5eyov/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/_core/include"
         ],
         "language": "c",
         "name": "soxr.cysoxr",
         "sources": [
             "src/soxr/cysoxr.pyx",
             "libsoxr/src/soxr.c",
             "libsoxr/src/data-io.c",
@@ -58,23 +58,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030002F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -158,14 +158,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -219,14 +221,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -280,60 +284,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -416,14 +443,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -607,25 +637,28 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
-        PyObject *version_info; // borrowed
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -638,15 +671,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -671,15 +703,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -757,16 +789,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -782,14 +819,39 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
 #if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
@@ -808,14 +870,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -883,27 +947,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -939,15 +1003,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1083,14 +1147,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1161,15 +1234,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1188,15 +1261,15 @@
 
 #define __PYX_HAVE__soxr__cysoxr
 #define __PYX_HAVE_API__soxr__cysoxr
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 
-    /* Using NumPy API declarations from "Cython/Includes/numpy/" */
+    /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
     
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 #include "soxr.h"
@@ -1247,17 +1320,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1277,32 +1351,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1344,15 +1401,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1365,14 +1422,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1415,14 +1473,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1462,15 +1521,15 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1485,15 +1544,15 @@
 #endif
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "src/soxr/cysoxr.pyx",
   "<stringsource>",
-  "__init__.pxd",
+  "__init__.cython-30.pxd",
   "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
@@ -1592,14 +1651,15 @@
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
 #elif CYTHON_ATOMICS && defined(_MSC_VER)
     #include <intrin.h>
     #undef __pyx_atomic_int_type
     #define __pyx_atomic_int_type long
+    #undef __pyx_nonatomic_int_type
     #define __pyx_nonatomic_int_type long
     #pragma intrinsic (_InterlockedExchangeAdd)
     #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
     #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
@@ -1631,182 +1691,164 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":736
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":770
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":739
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":745
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":751
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":760
- * # The int types are mapped a bit surprising --
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ * ctypedef double complex complex128_t
  * 
- */
-typedef npy_long __pyx_t_5numpy_int_t;
-
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":761
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
- * 
- * ctypedef npy_ulong      uint_t
- */
-typedef npy_longlong __pyx_t_5numpy_longlong_t;
-
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":763
- * ctypedef npy_longlong   longlong_t
- * 
- * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
-typedef npy_ulong __pyx_t_5numpy_uint_t;
+typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":764
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
- * ctypedef npy_ulong      uint_t
+ * ctypedef npy_longlong   longlong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":766
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":795
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":767
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":769
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":798
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":770
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":799
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":771
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":800
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
- * ctypedef npy_cfloat      cfloat_t
+ * ctypedef float complex       cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 /* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
@@ -1826,58 +1868,52 @@
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* Declarations.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    typedef ::std::complex< long double > __pyx_t_long_double_complex;
+  #else
+    typedef long double _Complex __pyx_t_long_double_complex;
+  #endif
+#else
+    typedef struct { long double real, imag; } __pyx_t_long_double_complex;
+#endif
+static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double, long double);
+
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_4soxr_6cysoxr_CySoxr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":773
- * ctypedef npy_longdouble longdouble_t
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1096
  * 
- * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t
- */
-typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
-
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":774
- * 
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
- * ctypedef npy_clongdouble clongdouble_t
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil             # <<<<<<<<<<<<<<
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil
  * 
  */
-typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
+typedef int (*__pyx_t_5numpy_NpyIter_IterNextFunc)(NpyIter *);
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1097
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil             # <<<<<<<<<<<<<<
  * 
- * ctypedef npy_cdouble     complex_t
+ * cdef extern from "numpy/arrayobject.h":
  */
-typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
-
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
- * ctypedef npy_clongdouble clongdouble_t
- * 
- * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew1(a):
- */
-typedef npy_cdouble __pyx_t_5numpy_complex_t;
+typedef void (*__pyx_t_5numpy_NpyIter_GetMultiIndexFunc)(NpyIter *, npy_intp *);
 struct __pyx_fuse_0__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process;
 struct __pyx_fuse_1__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process;
 struct __pyx_fuse_2__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process;
 struct __pyx_fuse_3__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process;
 struct __pyx_defaults;
 typedef struct __pyx_defaults __pyx_defaults;
 
@@ -2237,29 +2273,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2574,17 +2615,14 @@
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
 #if PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* ssize_strlen.proto */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
-
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
@@ -2602,15 +2640,19 @@
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
         PyList_SET_ITEM(list, len, x);
+        #endif
         __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
@@ -2642,15 +2684,19 @@
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+#define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
+#else
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+#endif
 
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
 }
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
@@ -2747,15 +2793,15 @@
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
 /* ListExtend.proto */
 static CYTHON_INLINE int __Pyx_PyList_Extend(PyObject* L, PyObject* v) {
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000
     PyObject* none = _PyList_Extend((PyListObject*)L, v);
     if (unlikely(!none))
         return -1;
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
@@ -2790,22 +2836,45 @@
                ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
                __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
         __Pyx__CallUnboundCMethod0(cfunc, self))
 #else
 #define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
 #endif
 
+/* dict_getitem_default.proto */
+static PyObject* __Pyx_PyDict_GetItemDefault(PyObject* d, PyObject* key, PyObject* default_value);
+
+/* CallUnboundCMethod1.proto */
+static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#else
+#define __Pyx_CallUnboundCMethod1(cfunc, self, arg)  __Pyx__CallUnboundCMethod1(cfunc, self, arg)
+#endif
+
+/* CallUnboundCMethod2.proto */
+static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
+static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
+#else
+#define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
+#endif
+
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
         PyList_SET_ITEM(list, len, x);
+        #endif
         __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
@@ -2860,30 +2929,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
-#define __PYX_HAVE_RT_ImportType_proto_3_0_2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_2 {
-   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -2968,25 +3037,29 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -3122,14 +3195,17 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_int__const__(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_short__const__(PyObject *, int writable_flag);
 
+/* PyUCS4InUnicode.proto */
+static CYTHON_INLINE int __Pyx_UnicodeContainsUCS4(PyObject* unicode, Py_UCS4 character);
+
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_float__const__(const char *itemp);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_double__const__(const char *itemp);
 
 /* MemviewDtypeToObject.proto */
@@ -3244,14 +3320,52 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
+/* Arithmetic.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+    #define __Pyx_c_eq_long__double(a, b)   ((a)==(b))
+    #define __Pyx_c_sum_long__double(a, b)  ((a)+(b))
+    #define __Pyx_c_diff_long__double(a, b) ((a)-(b))
+    #define __Pyx_c_prod_long__double(a, b) ((a)*(b))
+    #define __Pyx_c_quot_long__double(a, b) ((a)/(b))
+    #define __Pyx_c_neg_long__double(a)     (-(a))
+  #ifdef __cplusplus
+    #define __Pyx_c_is_zero_long__double(z) ((z)==(long double)0)
+    #define __Pyx_c_conj_long__double(z)    (::std::conj(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (::std::abs(z))
+        #define __Pyx_c_pow_long__double(a, b)  (::std::pow(a, b))
+    #endif
+  #else
+    #define __Pyx_c_is_zero_long__double(z) ((z)==0)
+    #define __Pyx_c_conj_long__double(z)    (conjl(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (cabsl(z))
+        #define __Pyx_c_pow_long__double(a, b)  (cpowl(a, b))
+    #endif
+ #endif
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex);
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex);
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    #endif
+#endif
+
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object);
 
@@ -3303,17 +3417,14 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value);
 
-/* BytesContains.proto */
-static CYTHON_INLINE int __Pyx_BytesContains(PyObject* bytes, char character);
-
 /* ImportNumPyArray.proto */
 static PyObject *__pyx_numpy_ndarray = NULL;
 static PyObject* __Pyx_ImportNumPyArrayTypeIfAvailable(void);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
@@ -3330,15 +3441,16 @@
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
@@ -3348,14 +3460,26 @@
 static PyObject *__pyx_memoryview_setitem_indexed(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview_convert_item_to_object(struct __pyx_memoryview_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
 static PyObject *__pyx_memoryview_assign_item_from_object(struct __pyx_memoryview_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self); /* proto*/
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
 static PyObject *__pyx_memoryviewslice_assign_item_from_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
@@ -3489,14 +3613,15 @@
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_VHQ[] = "VHQ";
 static const char __pyx_k__13[] = "()";
 static const char __pyx_k__14[] = "|";
 static const char __pyx_k__55[] = "?";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
+static const char __pyx_k_get[] = "get";
 static const char __pyx_k_got[] = " (got ";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
@@ -3639,15 +3764,14 @@
 static const char __pyx_k_pyx_fuse_0cysoxr_divide_proc[] = "__pyx_fuse_0cysoxr_divide_proc";
 static const char __pyx_k_pyx_fuse_1cysoxr_divide_proc[] = "__pyx_fuse_1cysoxr_divide_proc";
 static const char __pyx_k_pyx_fuse_2cysoxr_divide_proc[] = "__pyx_fuse_2cysoxr_divide_proc";
 static const char __pyx_k_pyx_fuse_3cysoxr_divide_proc[] = "__pyx_fuse_3cysoxr_divide_proc";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_Input_must_be_1_D_or_2_D_array[] = "Input must be 1-D or 2-D array";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
-static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Cannot_transpose_memoryview_with[] = "Cannot transpose memoryview with indirect dimensions";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
@@ -3656,15 +3780,16 @@
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got ";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis ";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension ";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
-static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static const char __pyx_k_numpy__core_multiarray_failed_to[] = "numpy._core.multiarray failed to import";
+static const char __pyx_k_numpy__core_umath_failed_to_impo[] = "numpy._core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 /* #### Code section: decls ### */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -3721,14 +3846,15 @@
 static PyObject *__pyx_pf_4soxr_6cysoxr_12__pyx_fuse_3cysoxr_divide_proc(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_in_rate, double __pyx_v_out_rate, __Pyx_memviewslice __pyx_v_x, unsigned long __pyx_v_quality); /* proto */
 static PyObject *__pyx_pf_4soxr_6cysoxr_4cysoxr_oneshot(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_in_rate, double __pyx_v_out_rate, PyArrayObject *__pyx_v_x, unsigned long __pyx_v_quality); /* proto */
 static PyObject *__pyx_tp_new_4soxr_6cysoxr_CySoxr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, 0, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_values = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -3907,14 +4033,15 @@
   PyObject *__pyx_n_s_float32;
   PyObject *__pyx_n_s_float64;
   PyObject *__pyx_n_s_format;
   PyObject *__pyx_n_s_fortran;
   PyObject *__pyx_n_u_fortran;
   PyObject *__pyx_n_s_fused_sigindex;
   PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_kp_u_got;
   PyObject *__pyx_kp_u_got_differing_extents_in_dimensi;
   PyObject *__pyx_n_s_id;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_in_rate;
   PyObject *__pyx_n_s_index;
@@ -3938,16 +4065,16 @@
   PyObject *__pyx_n_s_ndim;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_ntype;
   PyObject *__pyx_n_s_num_channels;
   PyObject *__pyx_n_s_numpy;
-  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_kp_u_numpy__core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy__core_umath_failed_to_impo;
   PyObject *__pyx_n_s_obj;
   PyObject *__pyx_n_s_order;
   PyObject *__pyx_n_s_out_rate;
   PyObject *__pyx_n_s_pack;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_process;
   PyObject *__pyx_n_s_pyx_PickleError;
@@ -4225,14 +4352,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_float32);
   Py_CLEAR(clear_module_state->__pyx_n_s_float64);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_n_s_fortran);
   Py_CLEAR(clear_module_state->__pyx_n_u_fortran);
   Py_CLEAR(clear_module_state->__pyx_n_s_fused_sigindex);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_got);
   Py_CLEAR(clear_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_CLEAR(clear_module_state->__pyx_n_s_id);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_in_rate);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
@@ -4256,16 +4384,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_ndim);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_ntype);
   Py_CLEAR(clear_module_state->__pyx_n_s_num_channels);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
   Py_CLEAR(clear_module_state->__pyx_n_s_order);
   Py_CLEAR(clear_module_state->__pyx_n_s_out_rate);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_process);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
@@ -4521,14 +4649,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_float32);
   Py_VISIT(traverse_module_state->__pyx_n_s_float64);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_n_s_fortran);
   Py_VISIT(traverse_module_state->__pyx_n_u_fortran);
   Py_VISIT(traverse_module_state->__pyx_n_s_fused_sigindex);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_got);
   Py_VISIT(traverse_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_VISIT(traverse_module_state->__pyx_n_s_id);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_in_rate);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
@@ -4552,16 +4681,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_ndim);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_ntype);
   Py_VISIT(traverse_module_state->__pyx_n_s_num_channels);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
   Py_VISIT(traverse_module_state->__pyx_n_s_order);
   Py_VISIT(traverse_module_state->__pyx_n_s_out_rate);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_process);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
@@ -4855,14 +4984,15 @@
 #define __pyx_n_s_float32 __pyx_mstate_global->__pyx_n_s_float32
 #define __pyx_n_s_float64 __pyx_mstate_global->__pyx_n_s_float64
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_n_s_fortran __pyx_mstate_global->__pyx_n_s_fortran
 #define __pyx_n_u_fortran __pyx_mstate_global->__pyx_n_u_fortran
 #define __pyx_n_s_fused_sigindex __pyx_mstate_global->__pyx_n_s_fused_sigindex
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_kp_u_got __pyx_mstate_global->__pyx_kp_u_got
 #define __pyx_kp_u_got_differing_extents_in_dimensi __pyx_mstate_global->__pyx_kp_u_got_differing_extents_in_dimensi
 #define __pyx_n_s_id __pyx_mstate_global->__pyx_n_s_id
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_in_rate __pyx_mstate_global->__pyx_n_s_in_rate
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
@@ -4886,16 +5016,16 @@
 #define __pyx_n_s_ndim __pyx_mstate_global->__pyx_n_s_ndim
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_ntype __pyx_mstate_global->__pyx_n_s_ntype
 #define __pyx_n_s_num_channels __pyx_mstate_global->__pyx_n_s_num_channels
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
-#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
-#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_kp_u_numpy__core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy__core_multiarray_failed_to
+#define __pyx_kp_u_numpy__core_umath_failed_to_impo __pyx_mstate_global->__pyx_kp_u_numpy__core_umath_failed_to_impo
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
 #define __pyx_n_s_order __pyx_mstate_global->__pyx_n_s_order
 #define __pyx_n_s_out_rate __pyx_mstate_global->__pyx_n_s_out_rate
 #define __pyx_n_s_pack __pyx_mstate_global->__pyx_n_s_pack
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_process __pyx_mstate_global->__pyx_n_s_process
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
@@ -5033,16 +5163,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 131, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shape,&__pyx_n_s_itemsize,&__pyx_n_s_format,&__pyx_n_s_mode,&__pyx_n_s_allocate_buffer,0};
     values[3] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)__pyx_n_s_c));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -5135,18 +5264,19 @@
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, __pyx_nargs); __PYX_ERR(1, 131, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -5421,21 +5551,28 @@
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError, f"Invalid shape in axis {idx}: {dim}."
  */
   __pyx_t_7 = 0;
-  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4); __pyx_t_1 = 0;
+  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = 0;
   for (;;) {
-    if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
+      #endif
+      if (__pyx_t_1 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_7;
     __pyx_t_7 = (__pyx_t_7 + 1);
@@ -6070,18 +6207,16 @@
   __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":211
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data and self.data is not NULL:
@@ -6185,15 +6320,14 @@
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":219
  *         PyObject_Free(self._shape)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def memview(self):
@@ -6218,15 +6352,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":221
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
@@ -6271,15 +6405,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_memview", 0);
+  __Pyx_RefNannySetupContext("get_memview", 1);
 
   /* "View.MemoryView":225
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
@@ -6358,16 +6492,14 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":229
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
@@ -6381,15 +6513,14 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":231
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
@@ -6416,15 +6547,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getattr__", 0);
+  __Pyx_RefNannySetupContext("__getattr__", 1);
 
   /* "View.MemoryView":232
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
@@ -6486,15 +6617,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":235
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
@@ -6555,15 +6686,15 @@
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_12__setitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setitem__", 0);
+  __Pyx_RefNannySetupContext("__setitem__", 1);
 
   /* "View.MemoryView":238
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
@@ -6614,53 +6745,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.array.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_array___reduce_cython__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_array___reduce_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -6716,16 +6836,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -6752,18 +6871,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -6786,15 +6906,15 @@
 
 static PyObject *__pyx_pf___pyx_array_2__setstate_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -6824,23 +6944,21 @@
  * 
  */
 
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_v_i;
   PyObject **__pyx_v_p;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_allocate_buffer", 0);
 
   /* "View.MemoryView":254
  *     cdef PyObject **p
  * 
  *     self.free_data = True             # <<<<<<<<<<<<<<
  *     self.data = <char *>malloc(self.len)
  *     if not self.data:
@@ -6970,15 +7088,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._allocate_buffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":268
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):             # <<<<<<<<<<<<<<
@@ -6994,15 +7111,15 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("array_cwrapper", 0);
+  __Pyx_RefNannySetupContext("array_cwrapper", 1);
 
   /* "View.MemoryView":270
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):
  *     cdef array result
  *     cdef str mode = "fortran" if c_mode[0] == b'f' else "c"  # this often comes from a constant C string.             # <<<<<<<<<<<<<<
  * 
  *     if buf is NULL:
@@ -7171,16 +7288,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 304, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -7206,18 +7322,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 304, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -7237,15 +7354,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "View.MemoryView":305
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
@@ -7292,15 +7409,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(struct __pyx_MemviewEnum_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":307
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
@@ -7346,39 +7463,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.Enum.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_MemviewEnum___reduce_cython__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -7391,15 +7497,15 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.name,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
@@ -7628,16 +7734,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 16, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -7664,18 +7769,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -7699,15 +7805,15 @@
 static PyObject *__pyx_pf___pyx_MemviewEnum_2__setstate_cython__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0x82a3537, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -7757,16 +7863,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 349, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,&__pyx_n_s_flags,&__pyx_n_s_dtype_is_object,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -7824,18 +7929,19 @@
     __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     if (values[2]) {
       __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, __pyx_nargs); __PYX_ERR(1, 349, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -7863,15 +7969,15 @@
   int __pyx_t_2;
   int __pyx_t_3;
   Py_intptr_t __pyx_t_4;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__cinit__", 1);
 
   /* "View.MemoryView":350
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
@@ -8198,22 +8304,20 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_2__dealloc__(struct __pyx_memoryview_obj *__pyx_v_self) {
   int __pyx_v_i;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyThread_type_lock __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":377
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
@@ -8403,15 +8507,14 @@
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":397
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
@@ -8430,15 +8533,15 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_item_pointer", 0);
+  __Pyx_RefNannySetupContext("get_item_pointer", 1);
 
   /* "View.MemoryView":399
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
@@ -8450,37 +8553,50 @@
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
-    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
     __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 401, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -8581,15 +8697,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char *__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":408
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
@@ -9192,15 +9308,15 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assignment", 1);
 
   /* "View.MemoryView":448
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  *         cdef __Pyx_memviewslice msrc = get_slice_from_memview(src, &src_slice)[0]             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mdst = get_slice_from_memview(dst, &dst_slice)[0]
  * 
@@ -9285,15 +9401,15 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 1);
 
   /* "View.MemoryView":455
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
@@ -9558,15 +9674,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_indexed", 0);
+  __Pyx_RefNannySetupContext("setitem_indexed", 1);
 
   /* "View.MemoryView":486
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
@@ -9629,15 +9745,15 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":492
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
@@ -9879,15 +9995,15 @@
   char *__pyx_t_9;
   char *__pyx_t_10;
   char *__pyx_t_11;
   char *__pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":508
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
@@ -10432,15 +10548,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":556
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
@@ -10518,15 +10634,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":562
  *     @property
  *     def base(self):
  *         return self._get_base()             # <<<<<<<<<<<<<<
  * 
  *     cdef _get_base(self):
@@ -10564,15 +10680,15 @@
  *         return self.obj
  * 
  */
 
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":565
  * 
  *     cdef _get_base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10628,15 +10744,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":569
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10714,15 +10830,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":573
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError, "Buffer view does not expose strides"
@@ -10829,15 +10945,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":581
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
@@ -10942,15 +11058,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":588
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -11007,15 +11123,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":592
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -11074,15 +11190,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":596
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -11153,15 +11269,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":600
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
@@ -11283,17 +11399,15 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":611
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
@@ -11336,15 +11450,14 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":616
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
@@ -11372,15 +11485,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":617
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
@@ -11475,15 +11588,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__str__", 0);
+  __Pyx_RefNannySetupContext("__str__", 1);
 
   /* "View.MemoryView":621
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
@@ -11552,39 +11665,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_c_contig (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 624, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_c_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_c_contig", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.is_c_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_16is_c_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11594,15 +11696,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_c_contig", 0);
+  __Pyx_RefNannySetupContext("is_c_contig", 1);
 
   /* "View.MemoryView":627
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
@@ -11666,39 +11768,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_f_contig (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 630, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_f_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_f_contig", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.is_f_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_18is_f_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11708,15 +11799,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_f_contig", 0);
+  __Pyx_RefNannySetupContext("is_f_contig", 1);
 
   /* "View.MemoryView":633
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
@@ -11780,39 +11871,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 636, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.copy", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_20copy(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11822,15 +11902,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy", 0);
+  __Pyx_RefNannySetupContext("copy", 1);
 
   /* "View.MemoryView":638
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
@@ -11912,39 +11992,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy_fortran (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 648, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy_fortran", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy_fortran", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.copy_fortran", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_22copy_fortran(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11955,15 +12024,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy_fortran", 0);
+  __Pyx_RefNannySetupContext("copy_fortran", 1);
 
   /* "View.MemoryView":650
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
@@ -12043,53 +12112,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryview___reduce_cython__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -12145,16 +12203,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -12181,18 +12238,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -12215,15 +12273,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -12259,15 +12317,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
+  __Pyx_RefNannySetupContext("memoryview_cwrapper", 1);
 
   /* "View.MemoryView":663
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
@@ -12342,17 +12400,15 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("memoryview_check", 0);
 
   /* "View.MemoryView":669
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o) noexcept:
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
@@ -12367,15 +12423,14 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":671
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
@@ -12399,15 +12454,15 @@
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_UCS4 __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_unellipsify", 0);
+  __Pyx_RefNannySetupContext("_unellipsify", 1);
 
   /* "View.MemoryView":677
  *     """
  *     cdef Py_ssize_t idx
  *     tup = <tuple>index if isinstance(index, tuple) else (index,)             # <<<<<<<<<<<<<<
  * 
  *     result = [slice(None)] * ndim
@@ -12481,21 +12536,28 @@
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   if (unlikely(__pyx_v_tup == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(1, 683, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_4 = 0;
   for (;;) {
-    if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
+      #endif
+      if (__pyx_t_4 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "View.MemoryView":684
  *     idx = 0
@@ -12756,23 +12818,21 @@
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
 static int assert_direct_dimensions(Py_ssize_t *__pyx_v_suboffsets, int __pyx_v_ndim) {
   Py_ssize_t __pyx_v_suboffset;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
   /* "View.MemoryView":701
  * 
  * cdef int assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim) except -1:
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError, "Indirect dimensions not supported"
@@ -12831,15 +12891,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView.assert_direct_dimensions", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":711
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
@@ -12877,15 +12936,15 @@
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memview_slice", 0);
+  __Pyx_RefNannySetupContext("memview_slice", 1);
 
   /* "View.MemoryView":712
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
@@ -13027,37 +13086,50 @@
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             cindex = index
  */
   __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
-    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
+    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
     __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 747, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 747, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       } else {
-        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       }
     } else {
       __pyx_t_8 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_8)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -13428,25 +13500,23 @@
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
 static int __pyx_memoryview_slice_memviewslice(__Pyx_memviewslice *__pyx_v_dst, Py_ssize_t __pyx_v_shape, Py_ssize_t __pyx_v_stride, Py_ssize_t __pyx_v_suboffset, int __pyx_v_dim, int __pyx_v_new_ndim, int *__pyx_v_suboffset_dim, Py_ssize_t __pyx_v_start, Py_ssize_t __pyx_v_stop, Py_ssize_t __pyx_v_step, int __pyx_v_have_start, int __pyx_v_have_stop, int __pyx_v_have_step, int __pyx_v_is_slice) {
   Py_ssize_t __pyx_v_new_shape;
   int __pyx_v_negative_step;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("slice_memviewslice", 1);
 
   /* "View.MemoryView":813
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
@@ -14193,15 +14263,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.slice_memviewslice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":896
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
@@ -14221,15 +14290,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_UCS4 __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pybuffer_index", 0);
+  __Pyx_RefNannySetupContext("pybuffer_index", 1);
 
   /* "View.MemoryView":898
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
@@ -14548,15 +14617,14 @@
 static int __pyx_memslice_transpose(__Pyx_memviewslice *__pyx_v_memslice) {
   int __pyx_v_ndim;
   Py_ssize_t *__pyx_v_shape;
   Py_ssize_t *__pyx_v_strides;
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   long __pyx_t_3;
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
@@ -14564,15 +14632,14 @@
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("transpose_memslice", 1);
 
   /* "View.MemoryView":930
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) except -1 nogil:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
@@ -14707,15 +14774,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.transpose_memslice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":963
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
@@ -14733,16 +14799,14 @@
   __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":964
  * 
  *     def __dealloc__(self):
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
@@ -14754,15 +14818,14 @@
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":966
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
@@ -14773,15 +14836,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":967
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
@@ -14860,15 +14923,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":973
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
@@ -14937,15 +15000,15 @@
  *         return self.from_object
  * 
  */
 
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":979
  * 
  *     cdef _get_base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  * 
@@ -14991,53 +15054,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryviewslice___reduce_cython__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -15093,16 +15145,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -15129,18 +15180,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -15163,15 +15215,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -15215,15 +15267,15 @@
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
+  __Pyx_RefNannySetupContext("memoryview_fromslice", 1);
 
   /* "View.MemoryView":1007
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
@@ -15592,15 +15644,15 @@
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
+  __Pyx_RefNannySetupContext("get_slice_from_memview", 1);
 
   /* "View.MemoryView":1055
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
@@ -15689,22 +15741,20 @@
  */
 
 static void __pyx_memoryview_slice_copy(struct __pyx_memoryview_obj *__pyx_v_memview, __Pyx_memviewslice *__pyx_v_dst) {
   int __pyx_v_dim;
   Py_ssize_t *__pyx_v_shape;
   Py_ssize_t *__pyx_v_strides;
   Py_ssize_t *__pyx_v_suboffsets;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
-  __Pyx_RefNannySetupContext("slice_copy", 0);
 
   /* "View.MemoryView":1067
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
@@ -15801,15 +15851,14 @@
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1080
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
@@ -15820,15 +15869,15 @@
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy", 1);
 
   /* "View.MemoryView":1083
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
@@ -15884,15 +15933,15 @@
   int __pyx_t_1;
   PyObject *(*__pyx_t_2)(char *);
   int (*__pyx_t_3)(char *, PyObject *);
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 1);
 
   /* "View.MemoryView":1094
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
@@ -16693,28 +16742,26 @@
 
 static void *__pyx_memoryview_copy_data_to_temp(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_tmpslice, char __pyx_v_order, int __pyx_v_ndim) {
   int __pyx_v_i;
   void *__pyx_v_result;
   size_t __pyx_v_itemsize;
   size_t __pyx_v_size;
   void *__pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("copy_data_to_temp", 1);
 
   /* "View.MemoryView":1216
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
@@ -16934,15 +16981,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.copy_data_to_temp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":1247
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
@@ -17154,22 +17200,20 @@
  * cdef int _err_no_memory() except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise MemoryError
  * 
  */
 
 static int __pyx_memoryview_err_no_memory(void) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("_err_no_memory", 0);
 
   /* "View.MemoryView":1261
  * @cname('__pyx_memoryview_err_no_memory')
  * cdef int _err_no_memory() except -1 with gil:
  *     raise MemoryError             # <<<<<<<<<<<<<<
  * 
  * 
@@ -17184,15 +17228,14 @@
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._err_no_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
 /* "View.MemoryView":1265
@@ -17209,29 +17252,27 @@
   int __pyx_v_i;
   char __pyx_v_order;
   int __pyx_v_broadcasting;
   int __pyx_v_direct_copy;
   __Pyx_memviewslice __pyx_v_tmp;
   int __pyx_v_ndim;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("memoryview_copy_contents", 1);
 
   /* "View.MemoryView":1273
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
@@ -17768,15 +17809,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.memoryview_copy_contents", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
@@ -17942,19 +17982,17 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
-  __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
   /* "View.MemoryView":1368
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
@@ -17966,15 +18004,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
 /* "View.MemoryView":1371
  * 
@@ -17983,20 +18020,18 @@
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   CYTHON_UNUSED Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_stride;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
   /* "View.MemoryView":1374
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(shape[0]):
@@ -18102,15 +18137,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1391
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
@@ -18324,16 +18358,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -18388,18 +18421,19 @@
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Enum", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 1, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -18429,15 +18463,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 1);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x82a3537, 0x6ae9995, 0xb068931):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
@@ -18611,15 +18645,15 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 1);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  *     __pyx_result.name = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
@@ -18727,293 +18761,717 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":250
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":287
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:
+ *             return PyDataType_ELSIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_ELSIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:
+ *             return PyDataType_ALIGNMENT(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use fields/names with care as they may be NULL.  You must check
+ */
+  __pyx_r = PyDataType_ALIGNMENT(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("fields", 1);
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":297
+ *         @property
+ *         cdef inline object fields(self):
+ *             return <object>PyDataType_FIELDS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_FIELDS(__pyx_v_self);
+  __Pyx_INCREF(((PyObject *)__pyx_t_1));
+  __pyx_r = ((PyObject *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("names", 1);
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":301
+ *         @property
+ *         cdef inline tuple names(self):
+ *             return <tuple>PyDataType_NAMES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use PyDataType_HASSUBARRAY to test whether this field is
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_NAMES(__pyx_v_self);
+  __Pyx_INCREF(((PyObject*)__pyx_t_1));
+  __pyx_r = ((PyObject*)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self) {
+  PyArray_ArrayDescr *__pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":308
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:
+ *             return PyDataType_SUBARRAY(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_SUBARRAY(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
+ * 
+ *         @property
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self) {
+  npy_uint64 __pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":313
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyDataType_FLAGS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
+ * 
+ *         @property
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":325
+ *         cdef inline int numiter(self) noexcept nogil:
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NUMITER(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":330
+ *         cdef inline npy_intp size(self) noexcept nogil:
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":335
+ *         cdef inline npy_intp index(self) noexcept nogil:
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_INDEX(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":340
+ *         cdef inline int nd(self) noexcept nogil:
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":345
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self) {
+  void **__pyx_r;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":351
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ *             return PyArray_MultiIter_ITERS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyArray_MultiIter_ITERS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":253
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":369
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":250
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":256
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
-  __Pyx_RefNannySetupContext("descr", 0);
+  __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":259
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":375
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":256
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":262
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":381
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":262
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":273
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":389
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":396
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":402
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":295
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":411
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
- *     ctypedef unsigned char      npy_bool
+ * 
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":779
- * ctypedef npy_cdouble     complex_t
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":780
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":808
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":779
- * ctypedef npy_cdouble     complex_t
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
   /* function exit code */
@@ -19023,46 +19481,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":811
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19073,46 +19531,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":786
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":814
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 814, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19123,46 +19581,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":788
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":817
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 789, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":788
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19173,46 +19631,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":791
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":792
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":820
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 792, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":791
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19223,212 +19681,219 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":794
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+  PyObject *__pyx_t_2;
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":795
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":796
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":824
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    __pyx_t_2 = __pyx_f_5numpy_5dtype_8subarray_subarray(__pyx_v_d)->shape;
+    __Pyx_INCREF(((PyObject*)__pyx_t_2));
+    __pyx_r = ((PyObject*)__pyx_t_2);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":795
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":798
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":826
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":794
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":975
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("set_array_base", 0);
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":976
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  * 
- * cdef inline void set_array_base(ndarray arr, object base):
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":977
- * cdef inline void set_array_base(ndarray arr, object base):
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1012
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 1012, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":975
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":979
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
+  __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":980
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1015
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":982
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":981
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":983
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1018
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":987
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19442,17 +19907,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
+  __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":988
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19460,68 +19925,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":989
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1024
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 989, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1024, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":988
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":990
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 990, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1025, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":991
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 991, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1026, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 991, __pyx_L5_except_error)
+      __PYX_ERR(2, 1026, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":988
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19529,15 +19994,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":987
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19552,16 +20017,16 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":993
- *         raise ImportError("numpy.core.multiarray failed to import")
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
@@ -19574,17 +20039,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
+  __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19592,68 +20057,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":995
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1030
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 995, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1030, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":994
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":996
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1031
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 996, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1031, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":997
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 997, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1032, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 997, __pyx_L5_except_error)
+      __PYX_ERR(2, 1032, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":994
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19661,16 +20126,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":993
- *         raise ImportError("numpy.core.multiarray failed to import")
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -19684,16 +20149,16 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":999
- *         raise ImportError("numpy.core.umath failed to import")
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
@@ -19706,17 +20171,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
+  __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1000
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19724,68 +20189,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1001
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1001, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1036, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1000
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1002
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1037
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1002, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1037, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1003
+      /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1003, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1038, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 1003, __pyx_L5_except_error)
+      __PYX_ERR(2, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1000
+    /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19793,16 +20258,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":999
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -19816,179 +20281,175 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1068
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1078
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1050
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1085
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1053
+/* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1057
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1092
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1053
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -20003,48 +20464,50 @@
  */
 
 static PyObject *__pyx_pw_4soxr_6cysoxr_1libsoxr_version(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static PyObject *__pyx_f_4soxr_6cysoxr_libsoxr_version(CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char const *__pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("libsoxr_version", 0);
+  __Pyx_RefNannySetupContext("libsoxr_version", 1);
 
   /* "soxr/cysoxr.pyx":28
  * 
  * cpdef str libsoxr_version():
  *     return csoxr.libsoxr_version().decode('UTF-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = libsoxr_version();
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_2)) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_INCREF(__pyx_t_2);
-  __pyx_r = ((PyObject*)__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ssize_strlen(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_1, 0, __pyx_t_2, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_t_3);
+  __pyx_r = ((PyObject*)__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "soxr/cysoxr.pyx":27
  * 
  * 
  * cpdef str libsoxr_version():             # <<<<<<<<<<<<<<
  *     return csoxr.libsoxr_version().decode('UTF-8')
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("soxr.cysoxr.libsoxr_version", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -20068,15 +20531,15 @@
 static PyObject *__pyx_pf_4soxr_6cysoxr_libsoxr_version(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("libsoxr_version", 0);
+  __Pyx_RefNannySetupContext("libsoxr_version", 1);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_4soxr_6cysoxr_libsoxr_version(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -20105,15 +20568,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("to_io_spec", 0);
+  __Pyx_RefNannySetupContext("to_io_spec", 1);
 
   /* "soxr/cysoxr.pyx":34
  * cdef csoxr.soxr_io_spec_t to_io_spec(type ntype):
  *     cdef csoxr.soxr_datatype_t io_type
  *     if ntype == np.float32:             # <<<<<<<<<<<<<<
  *         io_type = csoxr.SOXR_FLOAT32_I
  *     elif ntype == np.float64:
@@ -20328,16 +20791,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 56, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_in_rate,&__pyx_n_s_out_rate,&__pyx_n_s_num_channels,&__pyx_n_s_ntype,&__pyx_n_s_quality,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -20419,18 +20881,19 @@
     }
     __pyx_v_in_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_in_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L3_error)
     __pyx_v_out_rate = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_out_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L3_error)
     __pyx_v_num_channels = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_num_channels == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L3_error)
     __pyx_v_ntype = ((PyTypeObject*)values[3]);
     __pyx_v_quality = __Pyx_PyInt_As_unsigned_long(values[4]); if (unlikely((__pyx_v_quality == (unsigned long)-1) && PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 56, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -20465,15 +20928,15 @@
   soxr_io_spec_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__cinit__", 1);
 
   /* "soxr/cysoxr.pyx":59
  *                   double in_rate, double out_rate, unsigned num_channels,
  *                   type ntype, unsigned long quality):
  *         self._in_rate = in_rate             # <<<<<<<<<<<<<<
  *         self._out_rate = out_rate
  *         self._ntype = ntype
@@ -20631,16 +21094,14 @@
   __pyx_pf_4soxr_6cysoxr_6CySoxr_2__dealloc__(((struct __pyx_obj_4soxr_6cysoxr_CySoxr *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_4soxr_6cysoxr_6CySoxr_2__dealloc__(struct __pyx_obj_4soxr_6cysoxr_CySoxr *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "soxr/cysoxr.pyx":77
  * 
  *     def __dealloc__(self):
  *         csoxr.soxr_delete(self._soxr)             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
@@ -20652,15 +21113,14 @@
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         csoxr.soxr_delete(self._soxr)
  * 
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "soxr/cysoxr.pyx":81
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef np.ndarray process(self, const datatype_t[:, ::1] x, bint last=False):             # <<<<<<<<<<<<<<
  *         cdef size_t ilen = x.shape[0]
@@ -20683,16 +21143,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fused_cpdef (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 81, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_args,&__pyx_n_s_kwargs,&__pyx_n_s_defaults,&__pyx_n_s_fused_sigindex,0};
     values[3] = __Pyx_Arg_NewRef_VARARGS(__pyx_k__12);
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -20761,18 +21220,19 @@
       }
     }
     __pyx_v_args = values[0];
     __pyx_v_kwargs = values[1];
     __pyx_v_defaults = values[2];
     __pyx_v__fused_sigindex = values[3];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -20791,37 +21251,38 @@
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4soxr_6cysoxr_6CySoxr_4process(struct __pyx_obj_4soxr_6cysoxr_CySoxr *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults, PyObject *__pyx_v__fused_sigindex) {
   PyObject *__pyx_v_search_list = 0;
-  PyObject *__pyx_v_sn = 0;
   PyObject *__pyx_v_sigindex_node = 0;
   PyObject *__pyx_v_dest_sig = NULL;
   PyTypeObject *__pyx_v_ndarray = 0;
   PyObject *__pyx_v_arg_as_memoryview = 0;
   __Pyx_memviewslice __pyx_v_memslice;
   Py_ssize_t __pyx_v_itemsize;
   int __pyx_v_dtype_signed;
-  char __pyx_v_kind;
+  Py_UCS4 __pyx_v_kind;
   int __pyx_v_const_int_is_signed;
   int __pyx_v_const_short_is_signed;
   PyObject *__pyx_v_arg = NULL;
   PyObject *__pyx_v_dtype = NULL;
   PyObject *__pyx_v_arg_base = NULL;
   PyObject *__pyx_v_sig = NULL;
   PyObject *__pyx_v_sig_series = NULL;
   PyObject *__pyx_v_last_type = NULL;
   PyObject *__pyx_v_sig_type = NULL;
   PyObject *__pyx_v_sigindex_matches = NULL;
   PyObject *__pyx_v_sigindex_candidates = NULL;
   PyObject *__pyx_v_dst_type = NULL;
   PyObject *__pyx_v_found_matches = NULL;
   PyObject *__pyx_v_found_candidates = NULL;
+  PyObject *__pyx_v_sn = NULL;
+  PyObject *__pyx_v_type_match = NULL;
   PyObject *__pyx_v_candidates = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
@@ -20990,18 +21451,18 @@
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
         __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
-        __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
+        __pyx_v_dtype_signed = (__pyx_v_kind == 0x69);
         switch (__pyx_v_kind) {
-          case 'i':
-          case 'u':
+          case 0x69:
+          case 0x75:
           __pyx_t_4 = ((sizeof(int const )) == __pyx_v_itemsize);
           if (__pyx_t_4) {
           } else {
             __pyx_t_2 = __pyx_t_4;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
@@ -21041,15 +21502,15 @@
           __pyx_t_2 = __pyx_t_4;
           __pyx_L20_bool_binop_done:;
           if (__pyx_t_2) {
             if (unlikely((__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_short, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
-          case 'f':
+          case 0x66:
           __pyx_t_4 = ((sizeof(float const )) == __pyx_v_itemsize);
           if (__pyx_t_4) {
           } else {
             __pyx_t_2 = __pyx_t_4;
             goto __pyx_L24_bool_binop_done;
           }
           __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
@@ -21077,17 +21538,17 @@
           __pyx_t_2 = __pyx_t_4;
           __pyx_L27_bool_binop_done:;
           if (__pyx_t_2) {
             if (unlikely((__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
-          case 'c':
+          case 99:
           break;
-          case 'O':
+          case 79:
           break;
           default: break;
         }
       }
     }
     __pyx_t_2 = (__pyx_v_arg == Py_None);
     if (__pyx_t_2) {
@@ -21312,15 +21773,14 @@
     while (1) {
       __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_13, __pyx_t_14, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_11);
       if (unlikely(__pyx_t_15 == 0)) break;
       if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
       __pyx_t_1 = 0;
-      if (!(likely(PyDict_CheckExact(__pyx_v__fused_sigindex))||((__pyx_v__fused_sigindex) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_v__fused_sigindex))) __PYX_ERR(0, 81, __pyx_L1_error)
       __pyx_t_1 = __pyx_v__fused_sigindex;
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_1));
       __pyx_t_1 = 0;
       __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __pyx_t_17 = NULL;
@@ -21392,21 +21852,28 @@
       #else
       CYTHON_UNUSED_VAR(__pyx_t_17);
       #endif
       __Pyx_XDECREF_SET(__pyx_v_sig_series, ((PyObject*)__pyx_t_16));
       __pyx_t_16 = 0;
       __Pyx_XDECREF_SET(__pyx_v_last_type, __pyx_t_6);
       __pyx_t_6 = 0;
-      __pyx_t_1 = __pyx_v_sig_series; __Pyx_INCREF(__pyx_t_1); __pyx_t_18 = 0;
+      __pyx_t_1 = __pyx_v_sig_series; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_18 = 0;
       for (;;) {
-        if (__pyx_t_18 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+          #endif
+          if (__pyx_t_18 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_sig_type, __pyx_t_6);
         __pyx_t_6 = 0;
         if (unlikely(__pyx_v_sigindex_node == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 81, __pyx_L1_error)
@@ -21428,17 +21895,19 @@
         /*else*/ {
           if (unlikely(__pyx_v_sigindex_node == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
             __PYX_ERR(0, 81, __pyx_L1_error)
           }
           __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_sigindex_node, __pyx_v_sig_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 81, __pyx_L1_error)
-          __Pyx_DECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_6));
-          __pyx_t_6 = 0;
+          __pyx_t_16 = __pyx_t_6;
+          __Pyx_INCREF(__pyx_t_16);
+          __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+          __Pyx_DECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_16));
+          __pyx_t_16 = 0;
         }
         __pyx_L69:;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(__pyx_v_sigindex_node == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
         __PYX_ERR(0, 81, __pyx_L1_error)
@@ -21454,137 +21923,160 @@
   __pyx_t_13 = PyList_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_v__fused_sigindex);
   __Pyx_GIVEREF(__pyx_v__fused_sigindex);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_13, 0, __pyx_v__fused_sigindex)) __PYX_ERR(0, 81, __pyx_L1_error);
   __pyx_v_sigindex_candidates = ((PyObject*)__pyx_t_13);
   __pyx_t_13 = 0;
-  __pyx_t_13 = __pyx_v_dest_sig; __Pyx_INCREF(__pyx_t_13); __pyx_t_14 = 0;
+  __pyx_t_13 = __pyx_v_dest_sig; __Pyx_INCREF(__pyx_t_13);
+  __pyx_t_14 = 0;
   for (;;) {
-    if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_13)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_13);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+      #endif
+      if (__pyx_t_14 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_1 = PyList_GET_ITEM(__pyx_t_13, __pyx_t_14); __Pyx_INCREF(__pyx_t_1); __pyx_t_14++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
     #else
-    __pyx_t_1 = PySequence_ITEM(__pyx_t_13, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_13, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_found_matches, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
     __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_found_candidates, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
     __pyx_t_4 = (__pyx_v_dst_type == Py_None);
     if (__pyx_t_4) {
-      __pyx_t_1 = __pyx_v_sigindex_matches; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
+      __pyx_t_1 = __pyx_v_sigindex_matches; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_5 = 0;
       for (;;) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_6); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+        __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_16); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_16 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 81, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
         #endif
-        if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_6));
-        __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_16);
+        __pyx_t_16 = 0;
         if (unlikely(__pyx_v_sn == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
           __PYX_ERR(0, 81, __pyx_L1_error)
         }
-        __pyx_t_6 = __Pyx_PyDict_Values(__pyx_v_sn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_matches, __pyx_t_6); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __pyx_t_16 = __Pyx_PyDict_Values(((PyObject*)__pyx_v_sn)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 81, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
+        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_matches, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __pyx_v_sigindex_candidates; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
+      __pyx_t_1 = __pyx_v_sigindex_candidates; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_5 = 0;
       for (;;) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_6); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+        __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_16); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_16 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 81, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
         #endif
-        if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_6));
-        __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_16);
+        __pyx_t_16 = 0;
         if (unlikely(__pyx_v_sn == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
           __PYX_ERR(0, 81, __pyx_L1_error)
         }
-        __pyx_t_6 = __Pyx_PyDict_Values(__pyx_v_sn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_candidates, __pyx_t_6); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __pyx_t_16 = __Pyx_PyDict_Values(((PyObject*)__pyx_v_sn)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 81, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
+        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_candidates, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L73;
     }
     /*else*/ {
       __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_sigindex_matches);
       __Pyx_GIVEREF(__pyx_v_sigindex_matches);
       if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_sigindex_matches)) __PYX_ERR(0, 81, __pyx_L1_error);
       __Pyx_INCREF(__pyx_v_sigindex_candidates);
       __Pyx_GIVEREF(__pyx_v_sigindex_candidates);
       if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_sigindex_candidates)) __PYX_ERR(0, 81, __pyx_L1_error);
-      __pyx_t_6 = __pyx_t_1; __Pyx_INCREF(__pyx_t_6); __pyx_t_5 = 0;
+      __pyx_t_16 = __pyx_t_1; __Pyx_INCREF(__pyx_t_16);
+      __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       for (;;) {
         if (__pyx_t_5 >= 2) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_16, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_6, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_16, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_search_list, ((PyObject*)__pyx_t_1));
         __pyx_t_1 = 0;
         if (unlikely(__pyx_v_search_list == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 81, __pyx_L1_error)
         }
-        __pyx_t_1 = __pyx_v_search_list; __Pyx_INCREF(__pyx_t_1); __pyx_t_18 = 0;
+        __pyx_t_1 = __pyx_v_search_list; __Pyx_INCREF(__pyx_t_1);
+        __pyx_t_18 = 0;
         for (;;) {
-          if (__pyx_t_18 >= PyList_GET_SIZE(__pyx_t_1)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+            #endif
+            if (__pyx_t_18 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_16); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
           #else
-          __pyx_t_16 = PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 81, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_16);
+          __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_6);
           #endif
-          if (!(likely(PyDict_CheckExact(__pyx_t_16))||((__pyx_t_16) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_16))) __PYX_ERR(0, 81, __pyx_L1_error)
-          __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_16));
-          __pyx_t_16 = 0;
+          __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_6);
+          __pyx_t_6 = 0;
           if (unlikely(__pyx_v_sn == Py_None)) {
-            PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+            PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
             __PYX_ERR(0, 81, __pyx_L1_error)
           }
-          __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_v_dst_type, __pyx_v_sn, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyDict_GetItemDefault(((PyObject*)__pyx_v_sn), __pyx_v_dst_type, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 81, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_6);
+          __Pyx_XDECREF_SET(__pyx_v_type_match, __pyx_t_6);
+          __pyx_t_6 = 0;
+          __pyx_t_4 = (__pyx_v_type_match != Py_None);
           if (__pyx_t_4) {
-            if (unlikely(__pyx_v_sn == Py_None)) {
-              PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-              __PYX_ERR(0, 81, __pyx_L1_error)
-            }
-            __pyx_t_16 = __Pyx_PyDict_GetItem(__pyx_v_sn, __pyx_v_dst_type); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 81, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_16);
-            __pyx_t_19 = __Pyx_PyList_Append(__pyx_v_found_matches, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
-            __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+            __pyx_t_19 = __Pyx_PyList_Append(__pyx_v_found_matches, __pyx_v_type_match); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 81, __pyx_L1_error)
           }
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     }
     __pyx_L73:;
     __Pyx_INCREF(__pyx_v_found_matches);
     __Pyx_DECREF_SET(__pyx_v_sigindex_matches, __pyx_v_found_matches);
     __Pyx_INCREF(__pyx_v_found_candidates);
     __Pyx_DECREF_SET(__pyx_v_sigindex_candidates, __pyx_v_found_candidates);
     __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_found_matches) != 0);
@@ -21647,15 +22139,14 @@
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_AddTraceback("soxr.cysoxr.CySoxr.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_search_list);
-  __Pyx_XDECREF(__pyx_v_sn);
   __Pyx_XDECREF(__pyx_v_sigindex_node);
   __Pyx_XDECREF(__pyx_v_dest_sig);
   __Pyx_XDECREF((PyObject *)__pyx_v_ndarray);
   __Pyx_XDECREF(__pyx_v_arg_as_memoryview);
   __Pyx_XDECREF(__pyx_v_arg);
   __Pyx_XDECREF(__pyx_v_dtype);
   __Pyx_XDECREF(__pyx_v_arg_base);
@@ -21664,14 +22155,16 @@
   __Pyx_XDECREF(__pyx_v_last_type);
   __Pyx_XDECREF(__pyx_v_sig_type);
   __Pyx_XDECREF(__pyx_v_sigindex_matches);
   __Pyx_XDECREF(__pyx_v_sigindex_candidates);
   __Pyx_XDECREF(__pyx_v_dst_type);
   __Pyx_XDECREF(__pyx_v_found_matches);
   __Pyx_XDECREF(__pyx_v_found_candidates);
+  __Pyx_XDECREF(__pyx_v_sn);
+  __Pyx_XDECREF(__pyx_v_type_match);
   __Pyx_XDECREF(__pyx_v_candidates);
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -21697,19 +22190,18 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   size_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
-  char *__pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_0process", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_last = __pyx_optional_args->last;
     }
   }
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
@@ -21718,20 +22210,15 @@
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_process); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      #ifdef __Pyx_CyFunction_USED
-      if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
-      #else
-      if (!PyCFunction_Check(__pyx_t_1)
-      #endif
-              || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
+      if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
         __Pyx_XDECREF((PyObject *)__pyx_r);
         if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
         __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_x, 2, (PyObject *(*)(char *)) __pyx_memview_get_float__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_last); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
@@ -22003,31 +22490,22 @@
  *             &x[0,0], ilen, NULL,             # <<<<<<<<<<<<<<
  *             y.data, olen, &odone)
  * 
  */
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
 
-  /* "soxr/cysoxr.pyx":111
- *             self._soxr,
- *             &x[0,0], ilen, NULL,
- *             y.data, olen, &odone)             # <<<<<<<<<<<<<<
- * 
- *         y = y[:odone]
- */
-  __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
-
   /* "soxr/cysoxr.pyx":108
  * 
  *         cdef size_t odone
  *         csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *             self._soxr,
  *             &x[0,0], ilen, NULL,
  */
-  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((float const  *) ( /* dim=1 */ ((char *) (((float const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_t_13, __pyx_v_olen, (&__pyx_v_odone)));
+  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((float const  *) ( /* dim=1 */ ((char *) (((float const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y), __pyx_v_olen, (&__pyx_v_odone)));
 
   /* "soxr/cysoxr.pyx":113
  *             y.data, olen, &odone)
  * 
  *         y = y[:odone]             # <<<<<<<<<<<<<<
  * 
  *         # flush if last input
@@ -22113,31 +22591,22 @@
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 123, __pyx_L1_error)
       __pyx_v_last_buf = ((PyArrayObject *)__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "soxr/cysoxr.pyx":128
- *                     self._soxr,
- *                     NULL, 0, NULL,
- *                     last_buf.data, delay, &odone)             # <<<<<<<<<<<<<<
- * 
- *                 last_buf = last_buf[:odone]
- */
-      __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
-
       /* "soxr/cysoxr.pyx":125
  *                 last_buf = np.zeros([delay, channels], dtype=ntype, order='c')
  * 
  *                 csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *                     self._soxr,
  *                     NULL, 0, NULL,
  */
-      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_t_13, __pyx_v_delay, (&__pyx_v_odone)));
+      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf), __pyx_v_delay, (&__pyx_v_odone)));
 
       /* "soxr/cysoxr.pyx":130
  *                     last_buf.data, delay, &odone)
  * 
  *                 last_buf = last_buf[:odone]             # <<<<<<<<<<<<<<
  * 
  *                 y = np.concatenate([y, last_buf])
@@ -22266,16 +22735,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_0process (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 81, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_last,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -22319,18 +22787,19 @@
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_float__const__(values[0], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 81, __pyx_L3_error)
     if (values[1]) {
       __pyx_v_last = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_last == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
     } else {
       __pyx_v_last = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0process", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -22357,15 +22826,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_fuse_0__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_0process", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.last = __pyx_v_last;
   __pyx_t_1 = ((PyObject *)__pyx_vtabptr_4soxr_6cysoxr_CySoxr->__pyx_fuse_0process(__pyx_v_self, __pyx_v_x, 1, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
@@ -22405,19 +22874,18 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   size_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
-  char *__pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_1process", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_last = __pyx_optional_args->last;
     }
   }
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
@@ -22426,20 +22894,15 @@
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_process); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      #ifdef __Pyx_CyFunction_USED
-      if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
-      #else
-      if (!PyCFunction_Check(__pyx_t_1)
-      #endif
-              || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
+      if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
         __Pyx_XDECREF((PyObject *)__pyx_r);
         if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
         __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_x, 2, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_last); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
@@ -22711,31 +23174,22 @@
  *             &x[0,0], ilen, NULL,             # <<<<<<<<<<<<<<
  *             y.data, olen, &odone)
  * 
  */
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
 
-  /* "soxr/cysoxr.pyx":111
- *             self._soxr,
- *             &x[0,0], ilen, NULL,
- *             y.data, olen, &odone)             # <<<<<<<<<<<<<<
- * 
- *         y = y[:odone]
- */
-  __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
-
   /* "soxr/cysoxr.pyx":108
  * 
  *         cdef size_t odone
  *         csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *             self._soxr,
  *             &x[0,0], ilen, NULL,
  */
-  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_t_13, __pyx_v_olen, (&__pyx_v_odone)));
+  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((double const  *) ( /* dim=1 */ ((char *) (((double const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y), __pyx_v_olen, (&__pyx_v_odone)));
 
   /* "soxr/cysoxr.pyx":113
  *             y.data, olen, &odone)
  * 
  *         y = y[:odone]             # <<<<<<<<<<<<<<
  * 
  *         # flush if last input
@@ -22821,31 +23275,22 @@
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 123, __pyx_L1_error)
       __pyx_v_last_buf = ((PyArrayObject *)__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "soxr/cysoxr.pyx":128
- *                     self._soxr,
- *                     NULL, 0, NULL,
- *                     last_buf.data, delay, &odone)             # <<<<<<<<<<<<<<
- * 
- *                 last_buf = last_buf[:odone]
- */
-      __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
-
       /* "soxr/cysoxr.pyx":125
  *                 last_buf = np.zeros([delay, channels], dtype=ntype, order='c')
  * 
  *                 csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *                     self._soxr,
  *                     NULL, 0, NULL,
  */
-      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_t_13, __pyx_v_delay, (&__pyx_v_odone)));
+      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf), __pyx_v_delay, (&__pyx_v_odone)));
 
       /* "soxr/cysoxr.pyx":130
  *                     last_buf.data, delay, &odone)
  * 
  *                 last_buf = last_buf[:odone]             # <<<<<<<<<<<<<<
  * 
  *                 y = np.concatenate([y, last_buf])
@@ -22974,16 +23419,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_1process (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 81, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_last,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -23027,18 +23471,19 @@
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[0], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 81, __pyx_L3_error)
     if (values[1]) {
       __pyx_v_last = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_last == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
     } else {
       __pyx_v_last = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1process", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -23065,15 +23510,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_fuse_1__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_1process", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.last = __pyx_v_last;
   __pyx_t_1 = ((PyObject *)__pyx_vtabptr_4soxr_6cysoxr_CySoxr->__pyx_fuse_1process(__pyx_v_self, __pyx_v_x, 1, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
@@ -23113,19 +23558,18 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   size_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
-  char *__pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_2process", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_last = __pyx_optional_args->last;
     }
   }
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
@@ -23134,20 +23578,15 @@
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_process); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      #ifdef __Pyx_CyFunction_USED
-      if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
-      #else
-      if (!PyCFunction_Check(__pyx_t_1)
-      #endif
-              || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
+      if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
         __Pyx_XDECREF((PyObject *)__pyx_r);
         if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
         __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_x, 2, (PyObject *(*)(char *)) __pyx_memview_get_int__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_last); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
@@ -23419,31 +23858,22 @@
  *             &x[0,0], ilen, NULL,             # <<<<<<<<<<<<<<
  *             y.data, olen, &odone)
  * 
  */
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
 
-  /* "soxr/cysoxr.pyx":111
- *             self._soxr,
- *             &x[0,0], ilen, NULL,
- *             y.data, olen, &odone)             # <<<<<<<<<<<<<<
- * 
- *         y = y[:odone]
- */
-  __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
-
   /* "soxr/cysoxr.pyx":108
  * 
  *         cdef size_t odone
  *         csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *             self._soxr,
  *             &x[0,0], ilen, NULL,
  */
-  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((int const  *) ( /* dim=1 */ ((char *) (((int const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_t_13, __pyx_v_olen, (&__pyx_v_odone)));
+  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((int const  *) ( /* dim=1 */ ((char *) (((int const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y), __pyx_v_olen, (&__pyx_v_odone)));
 
   /* "soxr/cysoxr.pyx":113
  *             y.data, olen, &odone)
  * 
  *         y = y[:odone]             # <<<<<<<<<<<<<<
  * 
  *         # flush if last input
@@ -23529,31 +23959,22 @@
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 123, __pyx_L1_error)
       __pyx_v_last_buf = ((PyArrayObject *)__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "soxr/cysoxr.pyx":128
- *                     self._soxr,
- *                     NULL, 0, NULL,
- *                     last_buf.data, delay, &odone)             # <<<<<<<<<<<<<<
- * 
- *                 last_buf = last_buf[:odone]
- */
-      __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
-
       /* "soxr/cysoxr.pyx":125
  *                 last_buf = np.zeros([delay, channels], dtype=ntype, order='c')
  * 
  *                 csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *                     self._soxr,
  *                     NULL, 0, NULL,
  */
-      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_t_13, __pyx_v_delay, (&__pyx_v_odone)));
+      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf), __pyx_v_delay, (&__pyx_v_odone)));
 
       /* "soxr/cysoxr.pyx":130
  *                     last_buf.data, delay, &odone)
  * 
  *                 last_buf = last_buf[:odone]             # <<<<<<<<<<<<<<
  * 
  *                 y = np.concatenate([y, last_buf])
@@ -23682,16 +24103,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_2process (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 81, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_last,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -23735,18 +24155,19 @@
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int__const__(values[0], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 81, __pyx_L3_error)
     if (values[1]) {
       __pyx_v_last = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_last == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
     } else {
       __pyx_v_last = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2process", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -23773,15 +24194,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_fuse_2__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_2process", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.last = __pyx_v_last;
   __pyx_t_1 = ((PyObject *)__pyx_vtabptr_4soxr_6cysoxr_CySoxr->__pyx_fuse_2process(__pyx_v_self, __pyx_v_x, 1, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
@@ -23821,19 +24242,18 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   double __pyx_t_8;
   size_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
-  char *__pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_3process", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_last = __pyx_optional_args->last;
     }
   }
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
@@ -23842,20 +24262,15 @@
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_process); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      #ifdef __Pyx_CyFunction_USED
-      if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
-      #else
-      if (!PyCFunction_Check(__pyx_t_1)
-      #endif
-              || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
+      if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_4soxr_6cysoxr_6CySoxr_5process)) {
         __Pyx_XDECREF((PyObject *)__pyx_r);
         if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
         __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_x, 2, (PyObject *(*)(char *)) __pyx_memview_get_short__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_last); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
@@ -24127,31 +24542,22 @@
  *             &x[0,0], ilen, NULL,             # <<<<<<<<<<<<<<
  *             y.data, olen, &odone)
  * 
  */
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
 
-  /* "soxr/cysoxr.pyx":111
- *             self._soxr,
- *             &x[0,0], ilen, NULL,
- *             y.data, olen, &odone)             # <<<<<<<<<<<<<<
- * 
- *         y = y[:odone]
- */
-  __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
-
   /* "soxr/cysoxr.pyx":108
  * 
  *         cdef size_t odone
  *         csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *             self._soxr,
  *             &x[0,0], ilen, NULL,
  */
-  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((short const  *) ( /* dim=1 */ ((char *) (((short const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_t_13, __pyx_v_olen, (&__pyx_v_odone)));
+  (void)(soxr_process(__pyx_v_self->_soxr, (&(*((short const  *) ( /* dim=1 */ ((char *) (((short const  *) ( /* dim=0 */ (__pyx_v_x.data + __pyx_t_11 * __pyx_v_x.strides[0]) )) + __pyx_t_12)) )))), __pyx_v_ilen, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y), __pyx_v_olen, (&__pyx_v_odone)));
 
   /* "soxr/cysoxr.pyx":113
  *             y.data, olen, &odone)
  * 
  *         y = y[:odone]             # <<<<<<<<<<<<<<
  * 
  *         # flush if last input
@@ -24237,31 +24643,22 @@
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 123, __pyx_L1_error)
       __pyx_v_last_buf = ((PyArrayObject *)__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "soxr/cysoxr.pyx":128
- *                     self._soxr,
- *                     NULL, 0, NULL,
- *                     last_buf.data, delay, &odone)             # <<<<<<<<<<<<<<
- * 
- *                 last_buf = last_buf[:odone]
- */
-      __pyx_t_13 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf); if (unlikely(__pyx_t_13 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
-
       /* "soxr/cysoxr.pyx":125
  *                 last_buf = np.zeros([delay, channels], dtype=ntype, order='c')
  * 
  *                 csoxr.soxr_process(             # <<<<<<<<<<<<<<
  *                     self._soxr,
  *                     NULL, 0, NULL,
  */
-      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_t_13, __pyx_v_delay, (&__pyx_v_odone)));
+      (void)(soxr_process(__pyx_v_self->_soxr, NULL, 0, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_last_buf), __pyx_v_delay, (&__pyx_v_odone)));
 
       /* "soxr/cysoxr.pyx":130
  *                     last_buf.data, delay, &odone)
  * 
  *                 last_buf = last_buf[:odone]             # <<<<<<<<<<<<<<
  * 
  *                 y = np.concatenate([y, last_buf])
@@ -24390,16 +24787,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_3process (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 81, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,&__pyx_n_s_last,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -24443,18 +24839,19 @@
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_short__const__(values[0], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 81, __pyx_L3_error)
     if (values[1]) {
       __pyx_v_last = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_last == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
     } else {
       __pyx_v_last = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3process", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -24481,15 +24878,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_fuse_3__pyx_opt_args_4soxr_6cysoxr_6CySoxr_process __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3process", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_3process", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 81, __pyx_L1_error) }
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.last = __pyx_v_last;
   __pyx_t_1 = ((PyObject *)__pyx_vtabptr_4soxr_6cysoxr_CySoxr->__pyx_fuse_3process(__pyx_v_self, __pyx_v_x, 1, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
@@ -24529,53 +24926,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("soxr.cysoxr.CySoxr.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4soxr_6cysoxr_6CySoxr_16__reduce_cython__(((struct __pyx_obj_4soxr_6cysoxr_CySoxr *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4soxr_6cysoxr_6CySoxr_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_4soxr_6cysoxr_CySoxr *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -24632,16 +25018,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -24668,18 +25053,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -24702,15 +25088,15 @@
 
 static PyObject *__pyx_pf_4soxr_6cysoxr_6CySoxr_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_4soxr_6cysoxr_CySoxr *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -24757,16 +25143,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fused_cpdef (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 139, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_signatures,&__pyx_n_s_args,&__pyx_n_s_kwargs,&__pyx_n_s_defaults,&__pyx_n_s_fused_sigindex,0};
     __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
     values[4] = __Pyx_Arg_NewRef_VARARGS(__pyx_dynamic_args->__pyx_arg__fused_sigindex);
     if (__pyx_kwds) {
@@ -24850,18 +25235,19 @@
     }
     __pyx_v_signatures = values[0];
     __pyx_v_args = values[1];
     __pyx_v_kwargs = values[2];
     __pyx_v_defaults = values[3];
     __pyx_v__fused_sigindex = values[4];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 139, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -24880,37 +25266,38 @@
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4soxr_6cysoxr_2cysoxr_divide_proc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults, PyObject *__pyx_v__fused_sigindex) {
   PyObject *__pyx_v_search_list = 0;
-  PyObject *__pyx_v_sn = 0;
   PyObject *__pyx_v_sigindex_node = 0;
   PyObject *__pyx_v_dest_sig = NULL;
   PyTypeObject *__pyx_v_ndarray = 0;
   PyObject *__pyx_v_arg_as_memoryview = 0;
   __Pyx_memviewslice __pyx_v_memslice;
   Py_ssize_t __pyx_v_itemsize;
   int __pyx_v_dtype_signed;
-  char __pyx_v_kind;
+  Py_UCS4 __pyx_v_kind;
   int __pyx_v_const_int_is_signed;
   int __pyx_v_const_short_is_signed;
   PyObject *__pyx_v_arg = NULL;
   PyObject *__pyx_v_dtype = NULL;
   PyObject *__pyx_v_arg_base = NULL;
   PyObject *__pyx_v_sig = NULL;
   PyObject *__pyx_v_sig_series = NULL;
   PyObject *__pyx_v_last_type = NULL;
   PyObject *__pyx_v_sig_type = NULL;
   PyObject *__pyx_v_sigindex_matches = NULL;
   PyObject *__pyx_v_sigindex_candidates = NULL;
   PyObject *__pyx_v_dst_type = NULL;
   PyObject *__pyx_v_found_matches = NULL;
   PyObject *__pyx_v_found_candidates = NULL;
+  PyObject *__pyx_v_sn = NULL;
+  PyObject *__pyx_v_type_match = NULL;
   PyObject *__pyx_v_candidates = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
@@ -25079,18 +25466,18 @@
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
         __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
-        __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
+        __pyx_v_dtype_signed = (__pyx_v_kind == 0x69);
         switch (__pyx_v_kind) {
-          case 'i':
-          case 'u':
+          case 0x69:
+          case 0x75:
           __pyx_t_4 = ((sizeof(int const )) == __pyx_v_itemsize);
           if (__pyx_t_4) {
           } else {
             __pyx_t_2 = __pyx_t_4;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
@@ -25130,15 +25517,15 @@
           __pyx_t_2 = __pyx_t_4;
           __pyx_L20_bool_binop_done:;
           if (__pyx_t_2) {
             if (unlikely((__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_short, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
-          case 'f':
+          case 0x66:
           __pyx_t_4 = ((sizeof(float const )) == __pyx_v_itemsize);
           if (__pyx_t_4) {
           } else {
             __pyx_t_2 = __pyx_t_4;
             goto __pyx_L24_bool_binop_done;
           }
           __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
@@ -25166,17 +25553,17 @@
           __pyx_t_2 = __pyx_t_4;
           __pyx_L27_bool_binop_done:;
           if (__pyx_t_2) {
             if (unlikely((__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
-          case 'c':
+          case 99:
           break;
-          case 'O':
+          case 79:
           break;
           default: break;
         }
       }
     }
     __pyx_t_2 = (__pyx_v_arg == Py_None);
     if (__pyx_t_2) {
@@ -25401,15 +25788,14 @@
     while (1) {
       __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_13, __pyx_t_14, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_11);
       if (unlikely(__pyx_t_15 == 0)) break;
       if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
       __pyx_t_1 = 0;
-      if (!(likely(PyDict_CheckExact(__pyx_v__fused_sigindex))||((__pyx_v__fused_sigindex) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_v__fused_sigindex))) __PYX_ERR(0, 139, __pyx_L1_error)
       __pyx_t_1 = __pyx_v__fused_sigindex;
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_1));
       __pyx_t_1 = 0;
       __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __pyx_t_17 = NULL;
@@ -25481,21 +25867,28 @@
       #else
       CYTHON_UNUSED_VAR(__pyx_t_17);
       #endif
       __Pyx_XDECREF_SET(__pyx_v_sig_series, ((PyObject*)__pyx_t_16));
       __pyx_t_16 = 0;
       __Pyx_XDECREF_SET(__pyx_v_last_type, __pyx_t_6);
       __pyx_t_6 = 0;
-      __pyx_t_1 = __pyx_v_sig_series; __Pyx_INCREF(__pyx_t_1); __pyx_t_18 = 0;
+      __pyx_t_1 = __pyx_v_sig_series; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_18 = 0;
       for (;;) {
-        if (__pyx_t_18 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+          #endif
+          if (__pyx_t_18 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_sig_type, __pyx_t_6);
         __pyx_t_6 = 0;
         if (unlikely(__pyx_v_sigindex_node == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 139, __pyx_L1_error)
@@ -25517,17 +25910,19 @@
         /*else*/ {
           if (unlikely(__pyx_v_sigindex_node == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
             __PYX_ERR(0, 139, __pyx_L1_error)
           }
           __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_sigindex_node, __pyx_v_sig_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 139, __pyx_L1_error)
-          __Pyx_DECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_6));
-          __pyx_t_6 = 0;
+          __pyx_t_16 = __pyx_t_6;
+          __Pyx_INCREF(__pyx_t_16);
+          __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+          __Pyx_DECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_16));
+          __pyx_t_16 = 0;
         }
         __pyx_L69:;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(__pyx_v_sigindex_node == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
         __PYX_ERR(0, 139, __pyx_L1_error)
@@ -25543,137 +25938,160 @@
   __pyx_t_13 = PyList_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_v__fused_sigindex);
   __Pyx_GIVEREF(__pyx_v__fused_sigindex);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_13, 0, __pyx_v__fused_sigindex)) __PYX_ERR(0, 139, __pyx_L1_error);
   __pyx_v_sigindex_candidates = ((PyObject*)__pyx_t_13);
   __pyx_t_13 = 0;
-  __pyx_t_13 = __pyx_v_dest_sig; __Pyx_INCREF(__pyx_t_13); __pyx_t_14 = 0;
+  __pyx_t_13 = __pyx_v_dest_sig; __Pyx_INCREF(__pyx_t_13);
+  __pyx_t_14 = 0;
   for (;;) {
-    if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_13)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_13);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+      #endif
+      if (__pyx_t_14 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_1 = PyList_GET_ITEM(__pyx_t_13, __pyx_t_14); __Pyx_INCREF(__pyx_t_1); __pyx_t_14++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
     #else
-    __pyx_t_1 = PySequence_ITEM(__pyx_t_13, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_13, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_found_matches, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
     __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_found_candidates, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
     __pyx_t_4 = (__pyx_v_dst_type == Py_None);
     if (__pyx_t_4) {
-      __pyx_t_1 = __pyx_v_sigindex_matches; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
+      __pyx_t_1 = __pyx_v_sigindex_matches; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_5 = 0;
       for (;;) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_6); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_16); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_16 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
         #endif
-        if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_6));
-        __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_16);
+        __pyx_t_16 = 0;
         if (unlikely(__pyx_v_sn == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
           __PYX_ERR(0, 139, __pyx_L1_error)
         }
-        __pyx_t_6 = __Pyx_PyDict_Values(__pyx_v_sn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_matches, __pyx_t_6); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __pyx_t_16 = __Pyx_PyDict_Values(((PyObject*)__pyx_v_sn)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
+        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_matches, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __pyx_v_sigindex_candidates; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
+      __pyx_t_1 = __pyx_v_sigindex_candidates; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_5 = 0;
       for (;;) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_6); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_16); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_16 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
         #endif
-        if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_6));
-        __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_16);
+        __pyx_t_16 = 0;
         if (unlikely(__pyx_v_sn == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
           __PYX_ERR(0, 139, __pyx_L1_error)
         }
-        __pyx_t_6 = __Pyx_PyDict_Values(__pyx_v_sn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_candidates, __pyx_t_6); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __pyx_t_16 = __Pyx_PyDict_Values(((PyObject*)__pyx_v_sn)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
+        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_candidates, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L73;
     }
     /*else*/ {
       __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_sigindex_matches);
       __Pyx_GIVEREF(__pyx_v_sigindex_matches);
       if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_sigindex_matches)) __PYX_ERR(0, 139, __pyx_L1_error);
       __Pyx_INCREF(__pyx_v_sigindex_candidates);
       __Pyx_GIVEREF(__pyx_v_sigindex_candidates);
       if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_sigindex_candidates)) __PYX_ERR(0, 139, __pyx_L1_error);
-      __pyx_t_6 = __pyx_t_1; __Pyx_INCREF(__pyx_t_6); __pyx_t_5 = 0;
+      __pyx_t_16 = __pyx_t_1; __Pyx_INCREF(__pyx_t_16);
+      __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       for (;;) {
         if (__pyx_t_5 >= 2) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_16, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_6, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_16, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_search_list, ((PyObject*)__pyx_t_1));
         __pyx_t_1 = 0;
         if (unlikely(__pyx_v_search_list == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 139, __pyx_L1_error)
         }
-        __pyx_t_1 = __pyx_v_search_list; __Pyx_INCREF(__pyx_t_1); __pyx_t_18 = 0;
+        __pyx_t_1 = __pyx_v_search_list; __Pyx_INCREF(__pyx_t_1);
+        __pyx_t_18 = 0;
         for (;;) {
-          if (__pyx_t_18 >= PyList_GET_SIZE(__pyx_t_1)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+            #endif
+            if (__pyx_t_18 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_16); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
           #else
-          __pyx_t_16 = PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 139, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_16);
+          __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_6);
           #endif
-          if (!(likely(PyDict_CheckExact(__pyx_t_16))||((__pyx_t_16) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_16))) __PYX_ERR(0, 139, __pyx_L1_error)
-          __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_16));
-          __pyx_t_16 = 0;
+          __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_6);
+          __pyx_t_6 = 0;
           if (unlikely(__pyx_v_sn == Py_None)) {
-            PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+            PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
             __PYX_ERR(0, 139, __pyx_L1_error)
           }
-          __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_v_dst_type, __pyx_v_sn, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyDict_GetItemDefault(((PyObject*)__pyx_v_sn), __pyx_v_dst_type, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_6);
+          __Pyx_XDECREF_SET(__pyx_v_type_match, __pyx_t_6);
+          __pyx_t_6 = 0;
+          __pyx_t_4 = (__pyx_v_type_match != Py_None);
           if (__pyx_t_4) {
-            if (unlikely(__pyx_v_sn == Py_None)) {
-              PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-              __PYX_ERR(0, 139, __pyx_L1_error)
-            }
-            __pyx_t_16 = __Pyx_PyDict_GetItem(__pyx_v_sn, __pyx_v_dst_type); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 139, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_16);
-            __pyx_t_19 = __Pyx_PyList_Append(__pyx_v_found_matches, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
-            __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+            __pyx_t_19 = __Pyx_PyList_Append(__pyx_v_found_matches, __pyx_v_type_match); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
           }
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     }
     __pyx_L73:;
     __Pyx_INCREF(__pyx_v_found_matches);
     __Pyx_DECREF_SET(__pyx_v_sigindex_matches, __pyx_v_found_matches);
     __Pyx_INCREF(__pyx_v_found_candidates);
     __Pyx_DECREF_SET(__pyx_v_sigindex_candidates, __pyx_v_found_candidates);
     __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_found_matches) != 0);
@@ -25736,15 +26154,14 @@
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_AddTraceback("soxr.cysoxr.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_search_list);
-  __Pyx_XDECREF(__pyx_v_sn);
   __Pyx_XDECREF(__pyx_v_sigindex_node);
   __Pyx_XDECREF(__pyx_v_dest_sig);
   __Pyx_XDECREF((PyObject *)__pyx_v_ndarray);
   __Pyx_XDECREF(__pyx_v_arg_as_memoryview);
   __Pyx_XDECREF(__pyx_v_arg);
   __Pyx_XDECREF(__pyx_v_dtype);
   __Pyx_XDECREF(__pyx_v_arg_base);
@@ -25753,14 +26170,16 @@
   __Pyx_XDECREF(__pyx_v_last_type);
   __Pyx_XDECREF(__pyx_v_sig_type);
   __Pyx_XDECREF(__pyx_v_sigindex_matches);
   __Pyx_XDECREF(__pyx_v_sigindex_candidates);
   __Pyx_XDECREF(__pyx_v_dst_type);
   __Pyx_XDECREF(__pyx_v_found_matches);
   __Pyx_XDECREF(__pyx_v_found_candidates);
+  __Pyx_XDECREF(__pyx_v_sn);
+  __Pyx_XDECREF(__pyx_v_type_match);
   __Pyx_XDECREF(__pyx_v_candidates);
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -25795,15 +26214,15 @@
   __Pyx_memviewslice __pyx_t_10 = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_t_11;
   size_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_0cysoxr_divide_proc", 1);
 
   /* "soxr/cysoxr.pyx":142
  *                                     const datatype_t[:, ::1] x,
  *                                     unsigned long quality):
  *     cdef size_t ilen = x.shape[0]             # <<<<<<<<<<<<<<
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef size_t chunk_len = int(48000 * in_rate / out_rate)
@@ -26304,16 +26723,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_0cysoxr_divide_proc (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 139, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_in_rate,&__pyx_n_s_out_rate,&__pyx_n_s_x,&__pyx_n_s_quality,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -26381,18 +26799,19 @@
       values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
     }
     __pyx_v_in_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_in_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_out_rate = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_out_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_float__const__(values[2], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 140, __pyx_L3_error)
     __pyx_v_quality = __Pyx_PyInt_As_unsigned_long(values[3]); if (unlikely((__pyx_v_quality == (unsigned long)-1) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0cysoxr_divide_proc", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 139, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -26418,15 +26837,15 @@
 static PyObject *__pyx_pf_4soxr_6cysoxr_6__pyx_fuse_0cysoxr_divide_proc(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_in_rate, double __pyx_v_out_rate, __Pyx_memviewslice __pyx_v_x, unsigned long __pyx_v_quality) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_0cysoxr_divide_proc", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 139, __pyx_L1_error) }
   __pyx_t_1 = ((PyObject *)__pyx_fuse_0__pyx_f_4soxr_6cysoxr_cysoxr_divide_proc(__pyx_v_in_rate, __pyx_v_out_rate, __pyx_v_x, __pyx_v_quality, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -26473,15 +26892,15 @@
   __Pyx_memviewslice __pyx_t_10 = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_t_11;
   size_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_1cysoxr_divide_proc", 1);
 
   /* "soxr/cysoxr.pyx":142
  *                                     const datatype_t[:, ::1] x,
  *                                     unsigned long quality):
  *     cdef size_t ilen = x.shape[0]             # <<<<<<<<<<<<<<
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef size_t chunk_len = int(48000 * in_rate / out_rate)
@@ -26982,16 +27401,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_1cysoxr_divide_proc (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 139, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_in_rate,&__pyx_n_s_out_rate,&__pyx_n_s_x,&__pyx_n_s_quality,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -27059,18 +27477,19 @@
       values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
     }
     __pyx_v_in_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_in_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_out_rate = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_out_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double__const__(values[2], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 140, __pyx_L3_error)
     __pyx_v_quality = __Pyx_PyInt_As_unsigned_long(values[3]); if (unlikely((__pyx_v_quality == (unsigned long)-1) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1cysoxr_divide_proc", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 139, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -27096,15 +27515,15 @@
 static PyObject *__pyx_pf_4soxr_6cysoxr_8__pyx_fuse_1cysoxr_divide_proc(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_in_rate, double __pyx_v_out_rate, __Pyx_memviewslice __pyx_v_x, unsigned long __pyx_v_quality) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_1cysoxr_divide_proc", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 139, __pyx_L1_error) }
   __pyx_t_1 = ((PyObject *)__pyx_fuse_1__pyx_f_4soxr_6cysoxr_cysoxr_divide_proc(__pyx_v_in_rate, __pyx_v_out_rate, __pyx_v_x, __pyx_v_quality, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -27151,15 +27570,15 @@
   __Pyx_memviewslice __pyx_t_10 = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_t_11;
   size_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_2cysoxr_divide_proc", 1);
 
   /* "soxr/cysoxr.pyx":142
  *                                     const datatype_t[:, ::1] x,
  *                                     unsigned long quality):
  *     cdef size_t ilen = x.shape[0]             # <<<<<<<<<<<<<<
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef size_t chunk_len = int(48000 * in_rate / out_rate)
@@ -27660,16 +28079,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_2cysoxr_divide_proc (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 139, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_in_rate,&__pyx_n_s_out_rate,&__pyx_n_s_x,&__pyx_n_s_quality,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -27737,18 +28155,19 @@
       values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
     }
     __pyx_v_in_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_in_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_out_rate = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_out_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int__const__(values[2], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 140, __pyx_L3_error)
     __pyx_v_quality = __Pyx_PyInt_As_unsigned_long(values[3]); if (unlikely((__pyx_v_quality == (unsigned long)-1) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2cysoxr_divide_proc", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 139, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -27774,15 +28193,15 @@
 static PyObject *__pyx_pf_4soxr_6cysoxr_10__pyx_fuse_2cysoxr_divide_proc(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_in_rate, double __pyx_v_out_rate, __Pyx_memviewslice __pyx_v_x, unsigned long __pyx_v_quality) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_2cysoxr_divide_proc", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 139, __pyx_L1_error) }
   __pyx_t_1 = ((PyObject *)__pyx_fuse_2__pyx_f_4soxr_6cysoxr_cysoxr_divide_proc(__pyx_v_in_rate, __pyx_v_out_rate, __pyx_v_x, __pyx_v_quality, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -27829,15 +28248,15 @@
   __Pyx_memviewslice __pyx_t_10 = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_t_11;
   size_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_3cysoxr_divide_proc", 1);
 
   /* "soxr/cysoxr.pyx":142
  *                                     const datatype_t[:, ::1] x,
  *                                     unsigned long quality):
  *     cdef size_t ilen = x.shape[0]             # <<<<<<<<<<<<<<
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef size_t chunk_len = int(48000 * in_rate / out_rate)
@@ -28338,16 +28757,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fuse_3cysoxr_divide_proc (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 139, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_in_rate,&__pyx_n_s_out_rate,&__pyx_n_s_x,&__pyx_n_s_quality,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -28415,18 +28833,19 @@
       values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
     }
     __pyx_v_in_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_in_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_out_rate = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_out_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
     __pyx_v_x = __Pyx_PyObject_to_MemoryviewSlice_d_dc_short__const__(values[2], 0); if (unlikely(!__pyx_v_x.memview)) __PYX_ERR(0, 140, __pyx_L3_error)
     __pyx_v_quality = __Pyx_PyInt_As_unsigned_long(values[3]); if (unlikely((__pyx_v_quality == (unsigned long)-1) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3cysoxr_divide_proc", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 139, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -28452,15 +28871,15 @@
 static PyObject *__pyx_pf_4soxr_6cysoxr_12__pyx_fuse_3cysoxr_divide_proc(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_in_rate, double __pyx_v_out_rate, __Pyx_memviewslice __pyx_v_x, unsigned long __pyx_v_quality) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3cysoxr_divide_proc", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_3cysoxr_divide_proc", 1);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_x.memview)) { __Pyx_RaiseUnboundLocalError("x"); __PYX_ERR(0, 139, __pyx_L1_error) }
   __pyx_t_1 = ((PyObject *)__pyx_fuse_3__pyx_f_4soxr_6cysoxr_cysoxr_divide_proc(__pyx_v_in_rate, __pyx_v_out_rate, __pyx_v_x, __pyx_v_quality, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -28500,53 +28919,49 @@
   soxr_io_spec_t __pyx_v_io_spec;
   soxr_quality_spec_t __pyx_v_quality_spec;
   size_t __pyx_v_odone;
   PyArrayObject *__pyx_v_y = 0;
   PyArrayObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  int __pyx_t_2;
+  PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  npy_intp *__pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  double __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  size_t __pyx_t_9;
-  soxr_io_spec_t __pyx_t_10;
-  char *__pyx_t_11;
-  char *__pyx_t_12;
+  int __pyx_t_7;
+  size_t __pyx_t_8;
+  soxr_io_spec_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cysoxr_oneshot", 0);
   __Pyx_INCREF((PyObject *)__pyx_v_x);
 
   /* "soxr/cysoxr.pyx":211
  *                                 np.ndarray x,
  *                                 unsigned long quality):
  *     if 2 < x.ndim:             # <<<<<<<<<<<<<<
  *         raise ValueError('Input must be 1-D or 2-D array')
  * 
  */
-  __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_x); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L1_error)
-  __pyx_t_2 = (2 < __pyx_t_1);
-  if (unlikely(__pyx_t_2)) {
+  __pyx_t_1 = (2 < __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_x));
+  if (unlikely(__pyx_t_1)) {
 
     /* "soxr/cysoxr.pyx":212
  *                                 unsigned long quality):
  *     if 2 < x.ndim:
  *         raise ValueError('Input must be 1-D or 2-D array')             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t ilen = x.shape[0]
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 212, __pyx_L1_error)
 
     /* "soxr/cysoxr.pyx":211
  *                                 np.ndarray x,
  *                                 unsigned long quality):
  *     if 2 < x.ndim:             # <<<<<<<<<<<<<<
  *         raise ValueError('Input must be 1-D or 2-D array')
@@ -28557,62 +28972,61 @@
   /* "soxr/cysoxr.pyx":214
  *         raise ValueError('Input must be 1-D or 2-D array')
  * 
  *     cdef size_t ilen = x.shape[0]             # <<<<<<<<<<<<<<
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef unsigned channels = 1
  */
-  __pyx_t_4 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_x); if (unlikely(__pyx_t_4 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L1_error)
-  __pyx_v_ilen = (__pyx_t_4[0]);
+  __pyx_v_ilen = (__pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_x)[0]);
 
   /* "soxr/cysoxr.pyx":215
  * 
  *     cdef size_t ilen = x.shape[0]
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)             # <<<<<<<<<<<<<<
  *     cdef unsigned channels = 1
  *     if 2 == x.ndim:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ceil); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_7 = (__pyx_v_ilen * __pyx_v_out_rate);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ceil); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = (__pyx_v_ilen * __pyx_v_out_rate);
   if (unlikely(__pyx_v_in_rate == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
     __PYX_ERR(0, 215, __pyx_L1_error)
   }
-  __pyx_t_5 = PyFloat_FromDouble((__pyx_t_7 / __pyx_v_in_rate)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = NULL;
-  __pyx_t_1 = 0;
+  __pyx_t_3 = PyFloat_FromDouble((__pyx_t_5 / __pyx_v_in_rate)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_8);
+  if (unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-      __pyx_t_1 = 1;
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_7 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_3};
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_9 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_olen = __pyx_t_9;
+  __pyx_t_8 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_8 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_olen = __pyx_t_8;
 
   /* "soxr/cysoxr.pyx":216
  *     cdef size_t ilen = x.shape[0]
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef unsigned channels = 1             # <<<<<<<<<<<<<<
  *     if 2 == x.ndim:
  *         channels = x.shape[1]
@@ -28622,27 +29036,25 @@
   /* "soxr/cysoxr.pyx":217
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef unsigned channels = 1
  *     if 2 == x.ndim:             # <<<<<<<<<<<<<<
  *         channels = x.shape[1]
  * 
  */
-  __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_x); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L1_error)
-  __pyx_t_2 = (2 == __pyx_t_1);
-  if (__pyx_t_2) {
+  __pyx_t_1 = (2 == __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_x));
+  if (__pyx_t_1) {
 
     /* "soxr/cysoxr.pyx":218
  *     cdef unsigned channels = 1
  *     if 2 == x.ndim:
  *         channels = x.shape[1]             # <<<<<<<<<<<<<<
  * 
  *     cdef type ntype = x.dtype.type
  */
-    __pyx_t_4 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_x); if (unlikely(__pyx_t_4 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L1_error)
-    __pyx_v_channels = (__pyx_t_4[1]);
+    __pyx_v_channels = (__pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_x)[1]);
 
     /* "soxr/cysoxr.pyx":217
  *     cdef size_t olen = np.ceil(ilen * out_rate / in_rate)
  *     cdef unsigned channels = 1
  *     if 2 == x.ndim:             # <<<<<<<<<<<<<<
  *         channels = x.shape[1]
  * 
@@ -28652,22 +29064,22 @@
   /* "soxr/cysoxr.pyx":220
  *         channels = x.shape[1]
  * 
  *     cdef type ntype = x.dtype.type             # <<<<<<<<<<<<<<
  * 
  *     # make soxr config
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_x), __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyType_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("type", __pyx_t_6))) __PYX_ERR(0, 220, __pyx_L1_error)
-  __pyx_v_ntype = ((PyTypeObject*)__pyx_t_6);
-  __pyx_t_6 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_x), __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (!(likely(PyType_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("type", __pyx_t_4))) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_v_ntype = ((PyTypeObject*)__pyx_t_4);
+  __pyx_t_4 = 0;
 
   /* "soxr/cysoxr.pyx":223
  * 
  *     # make soxr config
  *     cdef csoxr.soxr_error_t err = NULL             # <<<<<<<<<<<<<<
  *     cdef csoxr.soxr_io_spec_t io_spec = to_io_spec(ntype)
  *     cdef csoxr.soxr_quality_spec_t quality_spec = csoxr.soxr_quality_spec(quality, 0)
@@ -28677,16 +29089,16 @@
   /* "soxr/cysoxr.pyx":224
  *     # make soxr config
  *     cdef csoxr.soxr_error_t err = NULL
  *     cdef csoxr.soxr_io_spec_t io_spec = to_io_spec(ntype)             # <<<<<<<<<<<<<<
  *     cdef csoxr.soxr_quality_spec_t quality_spec = csoxr.soxr_quality_spec(quality, 0)
  * 
  */
-  __pyx_t_10 = __pyx_f_4soxr_6cysoxr_to_io_spec(__pyx_v_ntype); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L1_error)
-  __pyx_v_io_spec = __pyx_t_10;
+  __pyx_t_9 = __pyx_f_4soxr_6cysoxr_to_io_spec(__pyx_v_ntype); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_v_io_spec = __pyx_t_9;
 
   /* "soxr/cysoxr.pyx":225
  *     cdef csoxr.soxr_error_t err = NULL
  *     cdef csoxr.soxr_io_spec_t io_spec = to_io_spec(ntype)
  *     cdef csoxr.soxr_quality_spec_t quality_spec = csoxr.soxr_quality_spec(quality, 0)             # <<<<<<<<<<<<<<
  * 
  *     x = np.ascontiguousarray(x)    # make array C-contiguous
@@ -28696,92 +29108,91 @@
   /* "soxr/cysoxr.pyx":227
  *     cdef csoxr.soxr_quality_spec_t quality_spec = csoxr.soxr_quality_spec(quality, 0)
  * 
  *     x = np.ascontiguousarray(x)    # make array C-contiguous             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t odone
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = NULL;
-  __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_3);
+  if (unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-      __pyx_t_1 = 1;
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_7 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_3, ((PyObject *)__pyx_v_x)};
-    __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 227, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, ((PyObject *)__pyx_v_x)};
+    __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_DECREF_SET(__pyx_v_x, ((PyArrayObject *)__pyx_t_6));
-  __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_DECREF_SET(__pyx_v_x, ((PyArrayObject *)__pyx_t_4));
+  __pyx_t_4 = 0;
 
   /* "soxr/cysoxr.pyx":231
  *     cdef size_t odone
  *     cdef np.ndarray y
  *     if 1 == x.ndim:             # <<<<<<<<<<<<<<
  *         y = np.zeros([olen], dtype=ntype, order='c')
  *     else:
  */
-  __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_x); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L1_error)
-  __pyx_t_2 = (1 == __pyx_t_1);
-  if (__pyx_t_2) {
+  __pyx_t_1 = (1 == __pyx_f_5numpy_7ndarray_4ndim_ndim(__pyx_v_x));
+  if (__pyx_t_1) {
 
     /* "soxr/cysoxr.pyx":232
  *     cdef np.ndarray y
  *     if 1 == x.ndim:
  *         y = np.zeros([olen], dtype=ntype, order='c')             # <<<<<<<<<<<<<<
  *     else:
  *         y = np.zeros([olen, channels], dtype=ntype, order='c')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 232, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_olen); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error);
-    __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_olen); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error);
+    __pyx_t_4 = 0;
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_2);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error);
+    __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)__pyx_v_ntype)) < 0) __PYX_ERR(0, 232, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_order, __pyx_n_u_c) < 0) __PYX_ERR(0, 232, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error);
-    __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, ((PyObject *)__pyx_v_ntype)) < 0) __PYX_ERR(0, 232, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_order, __pyx_n_u_c) < 0) __PYX_ERR(0, 232, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 232, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 232, __pyx_L1_error)
-    __pyx_v_y = ((PyArrayObject *)__pyx_t_8);
-    __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 232, __pyx_L1_error)
+    __pyx_v_y = ((PyArrayObject *)__pyx_t_6);
+    __pyx_t_6 = 0;
 
     /* "soxr/cysoxr.pyx":231
  *     cdef size_t odone
  *     cdef np.ndarray y
  *     if 1 == x.ndim:             # <<<<<<<<<<<<<<
  *         y = np.zeros([olen], dtype=ntype, order='c')
  *     else:
@@ -28793,102 +29204,84 @@
  *         y = np.zeros([olen], dtype=ntype, order='c')
  *     else:
  *         y = np.zeros([olen, channels], dtype=ntype, order='c')             # <<<<<<<<<<<<<<
  * 
  *     err = csoxr.soxr_oneshot(
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_olen); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_channels); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_8);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_8)) __PYX_ERR(0, 234, __pyx_L1_error);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_olen); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_channels); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error);
-    __pyx_t_8 = 0;
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error);
     __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_t_4 = 0;
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, ((PyObject *)__pyx_v_ntype)) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_order, __pyx_n_u_c) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_5);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error);
-    __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, ((PyObject *)__pyx_v_ntype)) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_order, __pyx_n_u_c) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 234, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 234, __pyx_L1_error)
-    __pyx_v_y = ((PyArrayObject *)__pyx_t_8);
-    __pyx_t_8 = 0;
+    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_v_y = ((PyArrayObject *)__pyx_t_6);
+    __pyx_t_6 = 0;
   }
   __pyx_L5:;
 
-  /* "soxr/cysoxr.pyx":238
- *     err = csoxr.soxr_oneshot(
- *         in_rate, out_rate, channels,
- *         x.data, ilen, NULL,             # <<<<<<<<<<<<<<
- *         y.data, olen, &odone,
- *         &io_spec, &quality_spec, NULL)
- */
-  __pyx_t_11 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_x); if (unlikely(__pyx_t_11 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
-
-  /* "soxr/cysoxr.pyx":239
- *         in_rate, out_rate, channels,
- *         x.data, ilen, NULL,
- *         y.data, olen, &odone,             # <<<<<<<<<<<<<<
- *         &io_spec, &quality_spec, NULL)
- * 
- */
-  __pyx_t_12 = __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y); if (unlikely(__pyx_t_12 == ((char *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L1_error)
-
   /* "soxr/cysoxr.pyx":236
  *         y = np.zeros([olen, channels], dtype=ntype, order='c')
  * 
  *     err = csoxr.soxr_oneshot(             # <<<<<<<<<<<<<<
  *         in_rate, out_rate, channels,
  *         x.data, ilen, NULL,
  */
-  __pyx_v_err = soxr_oneshot(__pyx_v_in_rate, __pyx_v_out_rate, __pyx_v_channels, __pyx_t_11, __pyx_v_ilen, NULL, __pyx_t_12, __pyx_v_olen, (&__pyx_v_odone), (&__pyx_v_io_spec), (&__pyx_v_quality_spec), NULL);
+  __pyx_v_err = soxr_oneshot(__pyx_v_in_rate, __pyx_v_out_rate, __pyx_v_channels, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_x), __pyx_v_ilen, NULL, __pyx_f_5numpy_7ndarray_4data_data(__pyx_v_y), __pyx_v_olen, (&__pyx_v_odone), (&__pyx_v_io_spec), (&__pyx_v_quality_spec), NULL);
 
   /* "soxr/cysoxr.pyx":242
  *         &io_spec, &quality_spec, NULL)
  * 
  *     if err is not NULL:             # <<<<<<<<<<<<<<
  *         raise RuntimeError(err)
  * 
  */
-  __pyx_t_2 = (__pyx_v_err != NULL);
-  if (unlikely(__pyx_t_2)) {
+  __pyx_t_1 = (__pyx_v_err != NULL);
+  if (unlikely(__pyx_t_1)) {
 
     /* "soxr/cysoxr.pyx":243
  * 
  *     if err is not NULL:
  *         raise RuntimeError(err)             # <<<<<<<<<<<<<<
  * 
  *     return y[:odone]
  */
-    __pyx_t_8 = __Pyx_PyBytes_FromString(__pyx_v_err); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 243, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_err); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 243, __pyx_L1_error)
 
     /* "soxr/cysoxr.pyx":242
  *         &io_spec, &quality_spec, NULL)
  * 
  *     if err is not NULL:             # <<<<<<<<<<<<<<
  *         raise RuntimeError(err)
@@ -28898,35 +29291,35 @@
 
   /* "soxr/cysoxr.pyx":245
  *         raise RuntimeError(err)
  * 
  *     return y[:odone]             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_5 = __Pyx_PyObject_GetSlice(((PyObject *)__pyx_v_y), 0, __pyx_v_odone, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 245, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 245, __pyx_L1_error)
-  __pyx_r = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetSlice(((PyObject *)__pyx_v_y), 0, __pyx_v_odone, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_r = ((PyArrayObject *)__pyx_t_3);
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "soxr/cysoxr.pyx":208
  * 
  * 
  * cpdef np.ndarray cysoxr_oneshot(double in_rate, double out_rate,             # <<<<<<<<<<<<<<
  *                                 np.ndarray x,
  *                                 unsigned long quality):
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("soxr.cysoxr.cysoxr_oneshot", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_ntype);
   __Pyx_XDECREF((PyObject *)__pyx_v_y);
   __Pyx_XDECREF((PyObject *)__pyx_v_x);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
@@ -28965,16 +29358,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cysoxr_oneshot (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 208, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_in_rate,&__pyx_n_s_out_rate,&__pyx_n_s_x,&__pyx_n_s_quality,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -29043,18 +29435,19 @@
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
     __pyx_v_in_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_in_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L3_error)
     __pyx_v_out_rate = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_out_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L3_error)
     __pyx_v_x = ((PyArrayObject *)values[2]);
     __pyx_v_quality = __Pyx_PyInt_As_unsigned_long(values[3]); if (unlikely((__pyx_v_quality == (unsigned long)-1) && PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("cysoxr_oneshot", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 208, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -29083,15 +29476,15 @@
 static PyObject *__pyx_pf_4soxr_6cysoxr_4cysoxr_oneshot(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_in_rate, double __pyx_v_out_rate, PyArrayObject *__pyx_v_x, unsigned long __pyx_v_quality) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("cysoxr_oneshot", 0);
+  __Pyx_RefNannySetupContext("cysoxr_oneshot", 1);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_f_4soxr_6cysoxr_cysoxr_oneshot(__pyx_v_in_rate, __pyx_v_out_rate, __pyx_v_x, __pyx_v_quality, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -30343,14 +30736,15 @@
     {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
     {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
     {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
     {&__pyx_n_s_fused_sigindex, __pyx_k_fused_sigindex, sizeof(__pyx_k_fused_sigindex), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_kp_u_got, __pyx_k_got, sizeof(__pyx_k_got), 0, 1, 0, 0},
     {&__pyx_kp_u_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 1, 0, 0},
     {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_in_rate, __pyx_k_in_rate, sizeof(__pyx_k_in_rate), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
@@ -30374,16 +30768,16 @@
     {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_ntype, __pyx_k_ntype, sizeof(__pyx_k_ntype), 0, 0, 1, 1},
     {&__pyx_n_s_num_channels, __pyx_k_num_channels, sizeof(__pyx_k_num_channels), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_multiarray_failed_to, __pyx_k_numpy__core_multiarray_failed_to, sizeof(__pyx_k_numpy__core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_umath_failed_to_impo, __pyx_k_numpy__core_umath_failed_to_impo, sizeof(__pyx_k_numpy__core_umath_failed_to_impo), 0, 1, 0, 0},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
     {&__pyx_n_s_order, __pyx_k_order, sizeof(__pyx_k_order), 0, 0, 1, 1},
     {&__pyx_n_s_out_rate, __pyx_k_out_rate, sizeof(__pyx_k_out_rate), 0, 0, 1, 1},
     {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_process, __pyx_k_process, sizeof(__pyx_k_process), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
@@ -30452,15 +30846,15 @@
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 261, __pyx_L1_error)
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 373, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 991, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 1026, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -30499,33 +30893,33 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":991
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 991, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 1026, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-hfz5eyov/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-ks4jxa7z/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 997, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_umath_failed_to_impo); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 1032, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "soxr/cysoxr.pyx":43
  *         io_type = csoxr.SOXR_INT16_I
  *     else:
  *         raise ValueError('Data type not support')             # <<<<<<<<<<<<<<
@@ -30785,14 +31179,16 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
+  __pyx_umethod_PyDict_Type_get.method_name = &__pyx_n_s_get;
   __pyx_umethod_PyDict_Type_values.type = (PyObject*)&PyDict_Type;
   __pyx_umethod_PyDict_Type_values.method_name = &__pyx_n_s_values;
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -31070,41 +31466,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 207, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 207, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 234, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 243, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 833, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 871, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 271, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 316, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 320, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 359, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 848, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 850, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 852, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 854, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 856, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 858, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 860, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 862, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 864, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 930, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -31316,42 +31712,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("cysoxr", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to cysoxr pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "cysoxr" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_cysoxr(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -32304,14 +32698,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -32361,33 +32757,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -32595,21 +32998,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
@@ -32694,15 +33115,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -32713,15 +33134,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -32745,15 +33166,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -33032,17 +33453,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -33111,16 +33538,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -33129,30 +33561,36 @@
 #endif
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
     PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
@@ -33160,36 +33598,25 @@
         if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
   bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -33205,33 +33632,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    #if Py_VERSION_HEX < 0x03090000
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    #else
-    vectorcallfunc f = PyVectorcall_Function(func);
-    #endif
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
@@ -33526,15 +33959,15 @@
         if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
             memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            #if PY_VERSION_HEX >= 0x030D0000
+            #if PY_VERSION_HEX >= 0x030d0000
             if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
             #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
@@ -33655,15 +34088,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCallOneArg */
@@ -33690,15 +34123,17 @@
     }
     return NULL;
 }
 static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
     __Pyx_TypeName obj_type_name;
     if (likely(PyType_Check(obj))) {
         PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (meth) {
+        if (!meth) {
+            PyErr_Clear();
+        } else {
             PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
             Py_DECREF(meth);
             return result;
         }
     }
     obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
@@ -33799,36 +34234,43 @@
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
 /* GetAttr3 */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
     __Pyx_PyErr_Clear();
     Py_INCREF(d);
     return d;
 }
+#endif
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r;
-#if CYTHON_USE_TYPE_SLOTS
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    int res = PyObject_GetOptionalAttr(o, n, &r);
+    return (res != 0) ? r : __Pyx_NewRef(d);
+#else
+  #if CYTHON_USE_TYPE_SLOTS
     if (likely(PyString_Check(n))) {
         r = __Pyx_PyObject_GetAttrStrNoError(o, n);
         if (unlikely(!r) && likely(!PyErr_Occurred())) {
             r = __Pyx_NewRef(d);
         }
         return r;
     }
-#endif
+  #endif
     r = PyObject_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
+#endif
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -33858,15 +34300,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -34184,15 +34626,15 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -34347,24 +34789,14 @@
     } else if (PyErr_Occurred()) {
         PyErr_Clear();
     }
 #endif
     return __Pyx__ImportDottedModule(name, parts_tuple);
 }
 
-/* ssize_strlen */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
-    size_t len = strlen(s);
-    if (unlikely(len > PY_SSIZE_T_MAX)) {
-        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
-        return -1;
-    }
-    return (Py_ssize_t) len;
-}
-
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
@@ -34540,19 +34972,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_ass_item(o, i, v);
         }
     }
 #else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
+    if (is_list || !PyMapping_Check(o))
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
@@ -34609,14 +35037,15 @@
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* HasAttr */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
     }
@@ -34625,14 +35054,15 @@
         PyErr_Clear();
         return 0;
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
+#endif
 
 /* decode_c_string */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
@@ -34784,30 +35214,31 @@
     Py_XDECREF(attr);
     return -1;
 }
 #endif
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
 }
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg = NULL;
-    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     __Pyx_TypeName type_name;
@@ -34993,14 +35424,17 @@
     Py_XDECREF(value1);
     Py_XDECREF(value2);
     if (decref_tuple) { Py_XDECREF(tuple); }
     return -1;
 }
 
 /* dict_iter */
+#if CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+#include <string.h>
+#endif
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_source_is_dict) {
     is_dict = is_dict || likely(PyDict_CheckExact(iterable));
     *p_source_is_dict = is_dict;
     if (is_dict) {
 #if !CYTHON_COMPILING_IN_PYPY
         *p_orig_length = PyDict_Size(iterable);
@@ -35107,17 +35541,18 @@
         *pvalue = next_item;
     }
     return 1;
 }
 
 /* UnpackUnboundCMethod */
 static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *result;
     PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
     if (unlikely(!selfless_args)) return NULL;
-    PyObject *result = PyObject_Call(method, selfless_args, kwargs);
+    result = PyObject_Call(method, selfless_args, kwargs);
     Py_DECREF(selfless_args);
     return result;
 }
 static PyMethodDef __Pyx_UnboundCMethod_Def = {
      "CythonUnboundCMethod",
      __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
      METH_VARARGS | METH_KEYWORDS,
@@ -35129,25 +35564,23 @@
     if (unlikely(!method))
         return -1;
     target->method = method;
 #if CYTHON_COMPILING_IN_CPYTHON
     #if PY_MAJOR_VERSION >= 3
     if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
     #else
-    if (likely(!PyCFunction_Check(method)))
+    if (likely(!__Pyx_CyOrPyCFunction_Check(method)))
     #endif
     {
         PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
         target->func = descr->d_method->ml_meth;
         target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
     } else
 #endif
-#if defined(CYTHON_COMPILING_IN_PYPY)
-#elif PY_VERSION_HEX >= 0x03090000
-    if (PyCFunction_CheckExact(method))
+#if CYTHON_COMPILING_IN_PYPY
 #else
     if (PyCFunction_Check(method))
 #endif
     {
         PyObject *self;
         int self_found;
 #if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
@@ -35195,14 +35628,152 @@
 static CYTHON_INLINE PyObject* __Pyx_PyDict_Values(PyObject* d) {
     if (PY_MAJOR_VERSION >= 3)
         return __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyDict_Type_values, d);
     else
         return PyDict_Values(d);
 }
 
+/* CallUnboundCMethod1 */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
+    if (likely(cfunc->func)) {
+        int flag = cfunc->flag;
+        if (flag == METH_O) {
+            return (*(cfunc->func))(self, arg);
+        } else if ((PY_VERSION_HEX >= 0x030600B1) && flag == METH_FASTCALL) {
+            #if PY_VERSION_HEX >= 0x030700A0
+                return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
+            #else
+                return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
+            #endif
+        } else if ((PY_VERSION_HEX >= 0x030700A0) && flag == (METH_FASTCALL | METH_KEYWORDS)) {
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
+        }
+    }
+    return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
+}
+#endif
+static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg){
+    PyObject *args, *result = NULL;
+    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
+        args = PyTuple_New(1);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(arg);
+        PyTuple_SET_ITEM(args, 0, arg);
+        if (cfunc->flag & METH_KEYWORDS)
+            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
+        else
+            result = (*cfunc->func)(self, args);
+    } else {
+        args = PyTuple_New(2);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(self);
+        PyTuple_SET_ITEM(args, 0, self);
+        Py_INCREF(arg);
+        PyTuple_SET_ITEM(args, 1, arg);
+        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+    }
+#else
+    args = PyTuple_Pack(2, self, arg);
+    if (unlikely(!args)) goto bad;
+    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+#endif
+bad:
+    Py_XDECREF(args);
+    return result;
+}
+
+/* CallUnboundCMethod2 */
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
+static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2) {
+    if (likely(cfunc->func)) {
+        PyObject *args[2] = {arg1, arg2};
+        if (cfunc->flag == METH_FASTCALL) {
+            #if PY_VERSION_HEX >= 0x030700A0
+            return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, args, 2);
+            #else
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
+            #endif
+        }
+        #if PY_VERSION_HEX >= 0x030700A0
+        if (cfunc->flag == (METH_FASTCALL | METH_KEYWORDS))
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
+        #endif
+    }
+    return __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2);
+}
+#endif
+static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2){
+    PyObject *args, *result = NULL;
+    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
+        args = PyTuple_New(2);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(arg1);
+        PyTuple_SET_ITEM(args, 0, arg1);
+        Py_INCREF(arg2);
+        PyTuple_SET_ITEM(args, 1, arg2);
+        if (cfunc->flag & METH_KEYWORDS)
+            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
+        else
+            result = (*cfunc->func)(self, args);
+    } else {
+        args = PyTuple_New(3);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(self);
+        PyTuple_SET_ITEM(args, 0, self);
+        Py_INCREF(arg1);
+        PyTuple_SET_ITEM(args, 1, arg1);
+        Py_INCREF(arg2);
+        PyTuple_SET_ITEM(args, 2, arg2);
+        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+    }
+#else
+    args = PyTuple_Pack(3, self, arg1, arg2);
+    if (unlikely(!args)) goto bad;
+    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+#endif
+bad:
+    Py_XDECREF(args);
+    return result;
+}
+
+/* dict_getitem_default */
+static PyObject* __Pyx_PyDict_GetItemDefault(PyObject* d, PyObject* key, PyObject* default_value) {
+    PyObject* value;
+#if PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (unlikely(PyErr_Occurred()))
+            return NULL;
+        value = default_value;
+    }
+    Py_INCREF(value);
+    if ((1));
+#else
+    if (PyString_CheckExact(key) || PyUnicode_CheckExact(key) || PyInt_CheckExact(key)) {
+        value = PyDict_GetItem(d, key);
+        if (unlikely(!value)) {
+            value = default_value;
+        }
+        Py_INCREF(value);
+    }
+#endif
+    else {
+        if (default_value == Py_None)
+            value = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_get, d, key);
+        else
+            value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
+    }
+    return value;
+}
+
 /* SliceObject */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
         Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
         int has_cstart, int has_cstop, int wraparound) {
     __Pyx_TypeName obj_type_name;
 #if CYTHON_USE_TYPE_SLOTS
@@ -35469,46 +36040,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -35794,18 +36365,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_2
-#define __PYX_HAVE_RT_ImportType_3_0_2
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -35851,23 +36422,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -35875,18 +36446,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -36039,14 +36607,28 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
@@ -36848,15 +37430,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -37545,16 +38127,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -37566,14 +38148,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -37663,15 +38247,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -38655,14 +39239,83 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* PyUCS4InUnicode */
+  #if PY_VERSION_HEX < 0x03090000 || (defined(PyUnicode_WCHAR_KIND) && defined(PyUnicode_AS_UNICODE))
+#if PY_VERSION_HEX < 0x03090000
+#define __Pyx_PyUnicode_AS_UNICODE(op) PyUnicode_AS_UNICODE(op)
+#define __Pyx_PyUnicode_GET_SIZE(op) PyUnicode_GET_SIZE(op)
+#else
+#define __Pyx_PyUnicode_AS_UNICODE(op) (((PyASCIIObject *)(op))->wstr)
+#define __Pyx_PyUnicode_GET_SIZE(op) ((PyCompactUnicodeObject *)(op))->wstr_length
+#endif
+#if !defined(Py_UNICODE_SIZE) || Py_UNICODE_SIZE == 2
+static int __Pyx_PyUnicodeBufferContainsUCS4_SP(Py_UNICODE* buffer, Py_ssize_t length, Py_UCS4 character) {
+    Py_UNICODE high_val, low_val;
+    Py_UNICODE* pos;
+    high_val = (Py_UNICODE) (0xD800 | (((character - 0x10000) >> 10) & ((1<<10)-1)));
+    low_val  = (Py_UNICODE) (0xDC00 | ( (character - 0x10000)        & ((1<<10)-1)));
+    for (pos=buffer; pos < buffer+length-1; pos++) {
+        if (unlikely((high_val == pos[0]) & (low_val == pos[1]))) return 1;
+    }
+    return 0;
+}
+#endif
+static int __Pyx_PyUnicodeBufferContainsUCS4_BMP(Py_UNICODE* buffer, Py_ssize_t length, Py_UCS4 character) {
+    Py_UNICODE uchar;
+    Py_UNICODE* pos;
+    uchar = (Py_UNICODE) character;
+    for (pos=buffer; pos < buffer+length; pos++) {
+        if (unlikely(uchar == pos[0])) return 1;
+    }
+    return 0;
+}
+#endif
+static CYTHON_INLINE int __Pyx_UnicodeContainsUCS4(PyObject* unicode, Py_UCS4 character) {
+#if CYTHON_PEP393_ENABLED
+    const int kind = PyUnicode_KIND(unicode);
+    #ifdef PyUnicode_WCHAR_KIND
+    if (likely(kind != PyUnicode_WCHAR_KIND))
+    #endif
+    {
+        Py_ssize_t i;
+        const void* udata = PyUnicode_DATA(unicode);
+        const Py_ssize_t length = PyUnicode_GET_LENGTH(unicode);
+        for (i=0; i < length; i++) {
+            if (unlikely(character == PyUnicode_READ(kind, udata, i))) return 1;
+        }
+        return 0;
+    }
+#elif PY_VERSION_HEX >= 0x03090000
+    #error Cannot use "UChar in Unicode" in Python 3.9 without PEP-393 unicode strings.
+#elif !defined(PyUnicode_AS_UNICODE)
+    #error Cannot use "UChar in Unicode" in Python < 3.9 without Py_UNICODE support.
+#endif
+#if PY_VERSION_HEX < 0x03090000 || (defined(PyUnicode_WCHAR_KIND) && defined(PyUnicode_AS_UNICODE))
+#if !defined(Py_UNICODE_SIZE) || Py_UNICODE_SIZE == 2
+    if ((sizeof(Py_UNICODE) == 2) && unlikely(character > 65535)) {
+        return __Pyx_PyUnicodeBufferContainsUCS4_SP(
+            __Pyx_PyUnicode_AS_UNICODE(unicode),
+            __Pyx_PyUnicode_GET_SIZE(unicode),
+            character);
+    } else
+#endif
+    {
+        return __Pyx_PyUnicodeBufferContainsUCS4_BMP(
+            __Pyx_PyUnicode_AS_UNICODE(unicode),
+            __Pyx_PyUnicode_GET_SIZE(unicode),
+            character);
+    }
+#endif
+}
+
 /* MemviewDtypeToObject */
   static CYTHON_INLINE PyObject *__pyx_memview_get_float__const__(const char *itemp) {
     return (PyObject *) PyFloat_FromDouble(*(float const  *) itemp);
 }
 
 /* MemviewDtypeToObject */
   static CYTHON_INLINE PyObject *__pyx_memview_get_double__const__(const char *itemp) {
@@ -39075,14 +39728,168 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
+/* Declarations */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return ::std::complex< long double >(x, y);
+    }
+  #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return x + y*(__pyx_t_long_double_complex)_Complex_I;
+    }
+  #endif
+#else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      __pyx_t_long_double_complex z;
+      z.real = x;
+      z.imag = y;
+      return z;
+    }
+#endif
+
+/* Arithmetic */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+       return (a.real == b.real) && (a.imag == b.imag);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real + b.real;
+        z.imag = a.imag + b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real - b.real;
+        z.imag = a.imag - b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real * b.real - a.imag * b.imag;
+        z.imag = a.real * b.imag + a.imag * b.real;
+        return z;
+    }
+    #if 1
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else if (fabsl(b.real) >= fabsl(b.imag)) {
+            if (b.real == 0 && b.imag == 0) {
+                return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.imag);
+            } else {
+                long double r = b.imag / b.real;
+                long double s = (long double)(1.0) / (b.real + b.imag * r);
+                return __pyx_t_long_double_complex_from_parts(
+                    (a.real + a.imag * r) * s, (a.imag - a.real * r) * s);
+            }
+        } else {
+            long double r = b.real / b.imag;
+            long double s = (long double)(1.0) / (b.imag + b.real * r);
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * r + a.imag) * s, (a.imag * r - a.real) * s);
+        }
+    }
+    #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else {
+            long double denom = b.real * b.real + b.imag * b.imag;
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * b.real + a.imag * b.imag) / denom,
+                (a.imag * b.real - a.real * b.imag) / denom);
+        }
+    }
+    #endif
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real = -a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex a) {
+       return (a.real == 0) && (a.imag == 0);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real =  a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex z) {
+          #if !defined(HAVE_HYPOT) || defined(_MSC_VER)
+            return sqrtl(z.real*z.real + z.imag*z.imag);
+          #else
+            return hypotl(z.real, z.imag);
+          #endif
+        }
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+            __pyx_t_long_double_complex z;
+            long double r, lnr, theta, z_r, z_theta;
+            if (b.imag == 0 && b.real == (int)b.real) {
+                if (b.real < 0) {
+                    long double denom = a.real * a.real + a.imag * a.imag;
+                    a.real = a.real / denom;
+                    a.imag = -a.imag / denom;
+                    b.real = -b.real;
+                }
+                switch ((int)b.real) {
+                    case 0:
+                        z.real = 1;
+                        z.imag = 0;
+                        return z;
+                    case 1:
+                        return a;
+                    case 2:
+                        return __Pyx_c_prod_long__double(a, a);
+                    case 3:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, a);
+                    case 4:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, z);
+                }
+            }
+            if (a.imag == 0) {
+                if (a.real == 0) {
+                    return a;
+                } else if ((b.imag == 0) && (a.real >= 0)) {
+                    z.real = powl(a.real, b.real);
+                    z.imag = 0;
+                    return z;
+                } else if (a.real > 0) {
+                    r = a.real;
+                    theta = 0;
+                } else {
+                    r = -a.real;
+                    theta = atan2l(0.0, -1.0);
+                }
+            } else {
+                r = __Pyx_c_abs_long__double(a);
+                theta = atan2l(a.imag, a.real);
+            }
+            lnr = logl(r);
+            z_r = expl(lnr * b.real - theta * b.imag);
+            z_theta = theta * b.real + lnr * b.imag;
+            z.real = z_r * cosl(z_theta);
+            z.imag = z_r * sinl(z_theta);
+            return z;
+        }
+    #endif
+#endif
+
 /* MemviewSliceCopyTemplate */
   static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object)
 {
@@ -39310,38 +40117,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(unsigned long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(unsigned long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
@@ -39509,15 +40318,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -39782,15 +40591,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -39918,38 +40727,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
@@ -40117,15 +40928,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -40253,38 +41064,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(unsigned int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
@@ -40452,15 +41265,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -40588,38 +41401,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value) {
@@ -40650,50 +41465,45 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(short),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(short));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
-/* BytesContains */
-  static CYTHON_INLINE int __Pyx_BytesContains(PyObject* bytes, char character) {
-    const Py_ssize_t length = PyBytes_GET_SIZE(bytes);
-    char* char_start = PyBytes_AS_STRING(bytes);
-    return memchr(char_start, (unsigned char)character, (size_t)length) != NULL;
-}
-
 /* ImportNumPyArray */
   static PyObject* __Pyx__ImportNumPyArray(void) {
     PyObject *numpy_module, *ndarray_object = NULL;
     numpy_module = __Pyx_Import(__pyx_n_s_numpy, NULL, 0);
     if (likely(numpy_module)) {
         ndarray_object = PyObject_GetAttrString(numpy_module, "ndarray");
         Py_DECREF(numpy_module);
@@ -40882,15 +41692,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -41155,15 +41965,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -41275,49 +42085,58 @@
         name = __Pyx_NewRef(__pyx_n_s__55);
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+  static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
   #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -41355,16 +42174,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `soxr-0.3.7/src/soxr/cysoxr.pyx` & `soxr-0.4.0b1/src/soxr/cysoxr.pyx`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/src/soxr.egg-info/PKG-INFO` & `soxr-0.4.0b1/src/soxr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soxr
-Version: 0.3.7
+Version: 0.4.0b1
 Summary: High quality, one-dimensional sample-rate conversion library
 Home-page: https://github.com/dofuuz/python-soxr
 Author: Myungchul Keum
 License: LGPLv2.1+
 Project-URL: Documentation, https://python-soxr.readthedocs.io
 Project-URL: Source, https://github.com/dofuuz/python-soxr
 Project-URL: Bug Tracker, https://github.com/dofuuz/python-soxr/issues
@@ -16,15 +16,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: COPYING.LGPL
 Requires-Dist: numpy
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
```

### Comparing `soxr-0.3.7/src/soxr.egg-info/SOURCES.txt` & `soxr-0.4.0b1/src/soxr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/tests/bench.py` & `soxr-0.4.0b1/tests/bench.py`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/tests/bench_soxr_oneshot.py` & `soxr-0.4.0b1/tests/bench_soxr_oneshot.py`

 * *Files identical despite different names*

### Comparing `soxr-0.3.7/tests/test_resample.py` & `soxr-0.4.0b1/tests/test_resample.py`

 * *Files identical despite different names*


# Comparing `tmp/python-rapidjson-1.8.tar.gz` & `tmp/python-rapidjson-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-rapidjson-1.8.tar", last modified: Thu Jul  7 05:21:51 2022, max compression
+gzip compressed data, was "python-rapidjson-1.9.tar", last modified: Mon Oct 17 06:30:59 2022, max compression
```

## Comparing `python-rapidjson-1.8.tar` & `python-rapidjson-1.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.599568 python-rapidjson-1.8/
--rw-r--r--   0 lele      (1000) lele      (1000)      179 2022-01-22 10:12:24.000000 python-rapidjson-1.8/.dir-locals.el
--rw-r--r--   0 lele      (1000) lele      (1000)    14645 2022-07-07 05:21:34.000000 python-rapidjson-1.8/CHANGES.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     1143 2017-08-23 09:03:37.000000 python-rapidjson-1.8/LICENSE
--rw-r--r--   0 lele      (1000) lele      (1000)      388 2021-06-19 08:26:51.000000 python-rapidjson-1.8/MANIFEST.in
--rw-rw-r--   0 lele      (1000) lele      (1000)    19490 2022-07-07 05:21:51.599568 python-rapidjson-1.8/PKG-INFO
--rw-rw-r--   0 lele      (1000) lele      (1000)     3876 2022-07-06 07:26:19.000000 python-rapidjson-1.8/README.rst
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.591569 python-rapidjson-1.8/benchmarks/
--rw-r--r--   0 lele      (1000) lele      (1000)     5564 2020-12-12 18:37:53.000000 python-rapidjson-1.8/benchmarks/conftest.py
--rw-r--r--   0 lele      (1000) lele      (1000)     6369 2022-07-06 07:01:19.000000 python-rapidjson-1.8/benchmarks/tablize.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     6034 2020-10-11 08:44:16.000000 python-rapidjson-1.8/benchmarks/test_benchmark.py
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.591569 python-rapidjson-1.8/docs/
--rw-r--r--   0 lele      (1000) lele      (1000)      620 2017-08-21 10:55:07.000000 python-rapidjson-1.8/docs/Makefile
--rw-rw-r--   0 lele      (1000) lele      (1000)     7996 2021-06-09 15:30:53.000000 python-rapidjson-1.8/docs/api.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)    21653 2022-07-06 07:51:06.000000 python-rapidjson-1.8/docs/benchmarks-tables.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     1794 2020-12-09 13:14:58.000000 python-rapidjson-1.8/docs/benchmarks.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     5273 2022-07-06 07:28:04.000000 python-rapidjson-1.8/docs/conf.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     6766 2021-06-12 07:47:53.000000 python-rapidjson-1.8/docs/decoder.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     3029 2020-12-08 18:26:18.000000 python-rapidjson-1.8/docs/dump.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)    23302 2022-07-06 07:39:06.000000 python-rapidjson-1.8/docs/dumps.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)     7418 2020-12-20 20:10:08.000000 python-rapidjson-1.8/docs/encoder.rst
--rw-r--r--   0 lele      (1000) lele      (1000)      715 2020-12-09 13:14:57.000000 python-rapidjson-1.8/docs/index.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     2280 2020-02-22 11:23:47.000000 python-rapidjson-1.8/docs/load.rst
--rw-rw-r--   0 lele      (1000) lele      (1000)    11291 2021-06-09 15:30:53.000000 python-rapidjson-1.8/docs/loads.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     8660 2021-06-12 07:39:04.000000 python-rapidjson-1.8/docs/quickstart.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     1202 2020-02-22 11:23:47.000000 python-rapidjson-1.8/docs/rawjson.rst
--rw-r--r--   0 lele      (1000) lele      (1000)     2463 2020-02-22 11:23:44.000000 python-rapidjson-1.8/docs/validator.rst
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.591569 python-rapidjson-1.8/python_rapidjson.egg-info/
--rw-rw-r--   0 lele      (1000) lele      (1000)    19490 2022-07-07 05:21:51.000000 python-rapidjson-1.8/python_rapidjson.egg-info/PKG-INFO
--rw-rw-r--   0 lele      (1000) lele      (1000)     2692 2022-07-07 05:21:51.000000 python-rapidjson-1.8/python_rapidjson.egg-info/SOURCES.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)        1 2022-07-07 05:21:51.000000 python-rapidjson-1.8/python_rapidjson.egg-info/dependency_links.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)       10 2022-07-07 05:21:51.000000 python-rapidjson-1.8/python_rapidjson.egg-info/top_level.txt
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.591569 python-rapidjson-1.8/rapidjson/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.587569 python-rapidjson-1.8/rapidjson/include/
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.595569 python-rapidjson-1.8/rapidjson/include/rapidjson/
--rw-rw-r--   0 lele      (1000) lele      (1000)    22522 2021-06-09 11:14:42.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/allocators.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2260 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/cursorstreamwrapper.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   133763 2022-07-06 17:45:19.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/document.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10660 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/encodedstream.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    29260 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/encodings.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.595569 python-rapidjson-1.8/rapidjson/include/rapidjson/error/
--rw-rw-r--   0 lele      (1000) lele      (1000)     8831 2021-06-09 11:14:42.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/error/en.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9744 2021-06-09 11:14:42.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/error/error.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2980 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/filereadstream.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3125 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/filewritestream.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4013 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/fwd.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.595569 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/
--rw-rw-r--   0 lele      (1000) lele      (1000)     9271 2022-07-06 17:45:19.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/biginteger.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2045 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/clzll.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    11559 2022-07-06 17:45:19.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/diyfp.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     8433 2021-10-16 08:38:47.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/dtoa.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2973 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/ieee754.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10110 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/itoa.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6620 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/meta.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3574 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/pow10.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    26120 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/regex.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     7163 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/stack.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2726 2021-10-16 08:38:47.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/strfunc.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9045 2021-10-16 08:38:47.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/strtod.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     1398 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/internal/swap.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     4061 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/istreamwrapper.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2539 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/memorybuffer.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2646 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/memorystream.h
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.595569 python-rapidjson-1.8/rapidjson/include/rapidjson/msinttypes/
--rw-rw-r--   0 lele      (1000) lele      (1000)     8372 2017-08-22 14:49:06.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/msinttypes/inttypes.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     9386 2017-08-22 14:49:06.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/msinttypes/stdint.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     2310 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/ostreamwrapper.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    63725 2021-10-16 08:38:47.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/pointer.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    10518 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/prettywriter.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    25599 2021-06-09 11:14:42.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/rapidjson.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    94332 2022-07-06 17:45:19.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/reader.h
--rw-rw-r--   0 lele      (1000) lele      (1000)   121678 2022-07-06 17:45:19.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/schema.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     6732 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/stream.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     3972 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/stringbuffer.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    19752 2021-10-16 08:38:47.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/uri.h
--rw-rw-r--   0 lele      (1000) lele      (1000)    26856 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/include/rapidjson/writer.h
--rw-rw-r--   0 lele      (1000) lele      (1000)     5152 2017-08-22 14:49:06.000000 python-rapidjson-1.8/rapidjson/license.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)    11146 2020-10-24 07:19:14.000000 python-rapidjson-1.8/rapidjson/readme.md
--rw-rw-r--   0 lele      (1000) lele      (1000)   141279 2022-07-07 04:45:03.000000 python-rapidjson-1.8/rapidjson.cpp
--rw-rw-r--   0 lele      (1000) lele      (1000)       21 2022-07-06 17:45:50.000000 python-rapidjson-1.8/rapidjson_exact_version.txt
--rw-r--r--   0 lele      (1000) lele      (1000)      348 2022-07-06 07:26:57.000000 python-rapidjson-1.8/requirements-test.txt
--rw-r--r--   0 lele      (1000) lele      (1000)      535 2022-07-06 07:27:10.000000 python-rapidjson-1.8/requirements.txt
--rw-rw-r--   0 lele      (1000) lele      (1000)      108 2022-07-07 05:21:51.599568 python-rapidjson-1.8/setup.cfg
--rw-r--r--   0 lele      (1000) lele      (1000)     4252 2022-07-07 04:51:40.000000 python-rapidjson-1.8/setup.py
-drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-07-07 05:21:51.599568 python-rapidjson-1.8/tests/
--rw-r--r--   0 lele      (1000) lele      (1000)     2493 2018-01-07 12:36:49.000000 python-rapidjson-1.8/tests/conftest.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     5353 2021-06-09 12:32:14.000000 python-rapidjson-1.8/tests/test_base_types.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     1484 2022-07-06 17:54:01.000000 python-rapidjson-1.8/tests/test_circular.py
--rw-r--r--   0 lele      (1000) lele      (1000)     1672 2021-06-10 07:18:07.000000 python-rapidjson-1.8/tests/test_dict_subclass.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      473 2020-10-11 08:44:16.000000 python-rapidjson-1.8/tests/test_enum.py
--rw-r--r--   0 lele      (1000) lele      (1000)     4009 2020-03-12 08:05:22.000000 python-rapidjson-1.8/tests/test_float.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     2956 2022-07-06 17:54:01.000000 python-rapidjson-1.8/tests/test_memory_leaks.py
--rw-rw-r--   0 lele      (1000) lele      (1000)    25001 2021-10-15 16:14:11.000000 python-rapidjson-1.8/tests/test_params.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     1852 2020-10-11 08:44:16.000000 python-rapidjson-1.8/tests/test_pass1.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      493 2020-10-11 08:44:16.000000 python-rapidjson-1.8/tests/test_pass2.py
--rw-rw-r--   0 lele      (1000) lele      (1000)      588 2020-10-11 08:44:16.000000 python-rapidjson-1.8/tests/test_pass3.py
--rw-r--r--   0 lele      (1000) lele      (1000)      834 2020-03-12 08:05:19.000000 python-rapidjson-1.8/tests/test_rawjson.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     6216 2022-02-19 08:30:06.000000 python-rapidjson-1.8/tests/test_refs_count.py
--rw-r--r--   0 lele      (1000) lele      (1000)     2153 2020-03-12 08:05:18.000000 python-rapidjson-1.8/tests/test_streams.py
--rw-r--r--   0 lele      (1000) lele      (1000)     1606 2020-10-24 07:34:09.000000 python-rapidjson-1.8/tests/test_unicode.py
--rw-rw-r--   0 lele      (1000) lele      (1000)     1910 2020-03-12 08:05:17.000000 python-rapidjson-1.8/tests/test_validator.py
--rw-r--r--   0 lele      (1000) lele      (1000)      768 2021-10-15 07:51:50.000000 python-rapidjson-1.8/tox.ini
--rw-r--r--   0 lele      (1000) lele      (1000)        3 2022-07-07 05:21:18.000000 python-rapidjson-1.8/version.txt
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.844108 python-rapidjson-1.9/
+-rw-r--r--   0 lele      (1000) lele      (1000)      179 2022-01-22 10:12:24.000000 python-rapidjson-1.9/.dir-locals.el
+-rw-r--r--   0 lele      (1000) lele      (1000)    14819 2022-10-17 06:30:44.000000 python-rapidjson-1.9/CHANGES.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1143 2017-08-23 09:03:37.000000 python-rapidjson-1.9/LICENSE
+-rw-r--r--   0 lele      (1000) lele      (1000)      388 2021-06-19 08:26:51.000000 python-rapidjson-1.9/MANIFEST.in
+-rw-rw-r--   0 lele      (1000) lele      (1000)    19664 2022-10-17 06:30:59.844108 python-rapidjson-1.9/PKG-INFO
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3876 2022-07-06 07:26:19.000000 python-rapidjson-1.9/README.rst
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.836108 python-rapidjson-1.9/benchmarks/
+-rw-r--r--   0 lele      (1000) lele      (1000)     5564 2020-12-12 18:37:53.000000 python-rapidjson-1.9/benchmarks/conftest.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     6369 2022-07-06 07:01:19.000000 python-rapidjson-1.9/benchmarks/tablize.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6034 2020-10-11 08:44:16.000000 python-rapidjson-1.9/benchmarks/test_benchmark.py
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.836108 python-rapidjson-1.9/docs/
+-rw-r--r--   0 lele      (1000) lele      (1000)      620 2017-08-21 10:55:07.000000 python-rapidjson-1.9/docs/Makefile
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7996 2021-06-09 15:30:53.000000 python-rapidjson-1.9/docs/api.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    21653 2022-07-06 07:51:06.000000 python-rapidjson-1.9/docs/benchmarks-tables.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1794 2020-12-09 13:14:58.000000 python-rapidjson-1.9/docs/benchmarks.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     5273 2022-07-06 07:28:04.000000 python-rapidjson-1.9/docs/conf.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6766 2021-06-12 07:47:53.000000 python-rapidjson-1.9/docs/decoder.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     3029 2020-12-08 18:26:18.000000 python-rapidjson-1.9/docs/dump.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    23302 2022-07-06 07:39:06.000000 python-rapidjson-1.9/docs/dumps.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7418 2020-12-20 20:10:08.000000 python-rapidjson-1.9/docs/encoder.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)      715 2020-12-09 13:14:57.000000 python-rapidjson-1.9/docs/index.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     2280 2020-02-22 11:23:47.000000 python-rapidjson-1.9/docs/load.rst
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11291 2021-06-09 15:30:53.000000 python-rapidjson-1.9/docs/loads.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     8660 2021-06-12 07:39:04.000000 python-rapidjson-1.9/docs/quickstart.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     1202 2020-02-22 11:23:47.000000 python-rapidjson-1.9/docs/rawjson.rst
+-rw-r--r--   0 lele      (1000) lele      (1000)     2463 2020-02-22 11:23:44.000000 python-rapidjson-1.9/docs/validator.rst
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.836108 python-rapidjson-1.9/python_rapidjson.egg-info/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    19664 2022-10-17 06:30:59.000000 python-rapidjson-1.9/python_rapidjson.egg-info/PKG-INFO
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2692 2022-10-17 06:30:59.000000 python-rapidjson-1.9/python_rapidjson.egg-info/SOURCES.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)        1 2022-10-17 06:30:59.000000 python-rapidjson-1.9/python_rapidjson.egg-info/dependency_links.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)       10 2022-10-17 06:30:59.000000 python-rapidjson-1.9/python_rapidjson.egg-info/top_level.txt
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.836108 python-rapidjson-1.9/rapidjson/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.832108 python-rapidjson-1.9/rapidjson/include/
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.840108 python-rapidjson-1.9/rapidjson/include/rapidjson/
+-rw-rw-r--   0 lele      (1000) lele      (1000)    22522 2021-06-09 11:14:42.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/allocators.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2260 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/cursorstreamwrapper.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   133763 2022-07-06 17:45:19.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/document.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10660 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/encodedstream.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    29260 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/encodings.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.840108 python-rapidjson-1.9/rapidjson/include/rapidjson/error/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8831 2021-06-09 11:14:42.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/error/en.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9744 2021-06-09 11:14:42.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/error/error.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2980 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/filereadstream.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3125 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/filewritestream.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4013 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/fwd.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.844108 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9271 2022-07-06 17:45:19.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/biginteger.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2045 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/clzll.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11559 2022-07-06 17:45:19.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/diyfp.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8433 2021-10-16 08:38:47.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/dtoa.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2973 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/ieee754.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10110 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/itoa.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6620 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/meta.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3574 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/pow10.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    26120 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/regex.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     7163 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/stack.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2726 2021-10-16 08:38:47.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/strfunc.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9045 2021-10-16 08:38:47.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/strtod.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1398 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/internal/swap.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     4061 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/istreamwrapper.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2539 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/memorybuffer.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2646 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/memorystream.h
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.844108 python-rapidjson-1.9/rapidjson/include/rapidjson/msinttypes/
+-rw-rw-r--   0 lele      (1000) lele      (1000)     8372 2017-08-22 14:49:06.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/msinttypes/inttypes.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     9386 2017-08-22 14:49:06.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/msinttypes/stdint.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2310 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/ostreamwrapper.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    63725 2021-10-16 08:38:47.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/pointer.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    10518 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/prettywriter.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    25599 2021-06-09 11:14:42.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/rapidjson.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    94332 2022-07-06 17:45:19.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/reader.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)   121678 2022-07-06 17:45:19.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/schema.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6732 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/stream.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     3972 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/stringbuffer.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)    19752 2021-10-16 08:38:47.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/uri.h
+-rw-r--r--   0 lele      (1000) lele      (1000)    26856 2022-07-09 13:30:06.000000 python-rapidjson-1.9/rapidjson/include/rapidjson/writer.h
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5152 2017-08-22 14:49:06.000000 python-rapidjson-1.9/rapidjson/license.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)    11146 2020-10-24 07:19:14.000000 python-rapidjson-1.9/rapidjson/readme.md
+-rw-r--r--   0 lele      (1000) lele      (1000)   141556 2022-10-17 06:23:19.000000 python-rapidjson-1.9/rapidjson.cpp
+-rw-rw-r--   0 lele      (1000) lele      (1000)       21 2022-07-06 17:45:50.000000 python-rapidjson-1.9/rapidjson_exact_version.txt
+-rw-r--r--   0 lele      (1000) lele      (1000)      348 2022-07-06 07:26:57.000000 python-rapidjson-1.9/requirements-test.txt
+-rw-r--r--   0 lele      (1000) lele      (1000)      535 2022-07-06 07:27:10.000000 python-rapidjson-1.9/requirements.txt
+-rw-rw-r--   0 lele      (1000) lele      (1000)      108 2022-10-17 06:30:59.844108 python-rapidjson-1.9/setup.cfg
+-rw-r--r--   0 lele      (1000) lele      (1000)     4252 2022-07-07 04:51:40.000000 python-rapidjson-1.9/setup.py
+drwxrwxr-x   0 lele      (1000) lele      (1000)        0 2022-10-17 06:30:59.844108 python-rapidjson-1.9/tests/
+-rw-r--r--   0 lele      (1000) lele      (1000)     2493 2018-01-07 12:36:49.000000 python-rapidjson-1.9/tests/conftest.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     5353 2021-06-09 12:32:14.000000 python-rapidjson-1.9/tests/test_base_types.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1484 2022-07-06 17:54:01.000000 python-rapidjson-1.9/tests/test_circular.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     1672 2021-06-10 07:18:07.000000 python-rapidjson-1.9/tests/test_dict_subclass.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      473 2020-10-11 08:44:16.000000 python-rapidjson-1.9/tests/test_enum.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     4009 2020-03-12 08:05:22.000000 python-rapidjson-1.9/tests/test_float.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     2956 2022-07-06 17:54:01.000000 python-rapidjson-1.9/tests/test_memory_leaks.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)    25001 2021-10-15 16:14:11.000000 python-rapidjson-1.9/tests/test_params.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1852 2020-10-11 08:44:16.000000 python-rapidjson-1.9/tests/test_pass1.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      493 2020-10-11 08:44:16.000000 python-rapidjson-1.9/tests/test_pass2.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)      588 2020-10-11 08:44:16.000000 python-rapidjson-1.9/tests/test_pass3.py
+-rw-r--r--   0 lele      (1000) lele      (1000)      834 2020-03-12 08:05:19.000000 python-rapidjson-1.9/tests/test_rawjson.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     6214 2022-08-26 08:26:39.000000 python-rapidjson-1.9/tests/test_refs_count.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     2153 2020-03-12 08:05:18.000000 python-rapidjson-1.9/tests/test_streams.py
+-rw-r--r--   0 lele      (1000) lele      (1000)     1606 2020-10-24 07:34:09.000000 python-rapidjson-1.9/tests/test_unicode.py
+-rw-rw-r--   0 lele      (1000) lele      (1000)     1910 2020-03-12 08:05:17.000000 python-rapidjson-1.9/tests/test_validator.py
+-rw-r--r--   0 lele      (1000) lele      (1000)      768 2021-10-15 07:51:50.000000 python-rapidjson-1.9/tox.ini
+-rw-r--r--   0 lele      (1000) lele      (1000)        3 2022-10-17 06:30:33.000000 python-rapidjson-1.9/version.txt
```

### Comparing `python-rapidjson-1.8/CHANGES.rst` & `python-rapidjson-1.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 -------
 
+1.9 (2022-10-17)
+~~~~~~~~~~~~~~~~
+
+* Produce Python 3.11 wheels, thanks to ``cibuildwheel`` `2.11.1`__
+
+  __ https://cibuildwheel.readthedocs.io/en/stable/changelog/#v2111
+
+
 1.8 (2022-07-07)
 ~~~~~~~~~~~~~~~~
 
 * Fix `problem on macOS`__ explicitly requiring C++11, thanks to agate-pris (`issue
   #166`__)
 
   __ https://github.com/Tencent/rapidjson/commit/9965ab37f6cfae3d58a0a6e34c76112866ace0b1#commitcomment-77875054
```

### Comparing `python-rapidjson-1.8/LICENSE` & `python-rapidjson-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/PKG-INFO` & `python-rapidjson-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rapidjson
-Version: 1.8
+Version: 1.9
 Summary: Python wrapper around rapidjson
 Home-page: https://github.com/python-rapidjson/python-rapidjson
 Author: Ken Robbins
 Author-email: ken@kenrobbins.com
 Maintainer: Lele Gaifax
 Maintainer-email: lele@metapensiero.it
 License: MIT License
@@ -151,14 +151,22 @@
 
 .. _RapidJSON: http://rapidjson.org/
 
 
 Changes
 -------
 
+1.9 (2022-10-17)
+~~~~~~~~~~~~~~~~
+
+* Produce Python 3.11 wheels, thanks to ``cibuildwheel`` `2.11.1`__
+
+  __ https://cibuildwheel.readthedocs.io/en/stable/changelog/#v2111
+
+
 1.8 (2022-07-07)
 ~~~~~~~~~~~~~~~~
 
 * Fix `problem on macOS`__ explicitly requiring C++11, thanks to agate-pris (`issue
   #166`__)
 
   __ https://github.com/Tencent/rapidjson/commit/9965ab37f6cfae3d58a0a6e34c76112866ace0b1#commitcomment-77875054
```

### Comparing `python-rapidjson-1.8/README.rst` & `python-rapidjson-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/benchmarks/conftest.py` & `python-rapidjson-1.9/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/benchmarks/tablize.py` & `python-rapidjson-1.9/benchmarks/tablize.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/benchmarks/test_benchmark.py` & `python-rapidjson-1.9/benchmarks/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/Makefile` & `python-rapidjson-1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/api.rst` & `python-rapidjson-1.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/benchmarks-tables.rst` & `python-rapidjson-1.9/docs/benchmarks-tables.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/benchmarks.rst` & `python-rapidjson-1.9/docs/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/conf.py` & `python-rapidjson-1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/decoder.rst` & `python-rapidjson-1.9/docs/decoder.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/dump.rst` & `python-rapidjson-1.9/docs/dump.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/dumps.rst` & `python-rapidjson-1.9/docs/dumps.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/encoder.rst` & `python-rapidjson-1.9/docs/encoder.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/index.rst` & `python-rapidjson-1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/load.rst` & `python-rapidjson-1.9/docs/load.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/loads.rst` & `python-rapidjson-1.9/docs/loads.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/quickstart.rst` & `python-rapidjson-1.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/rawjson.rst` & `python-rapidjson-1.9/docs/rawjson.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/docs/validator.rst` & `python-rapidjson-1.9/docs/validator.rst`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/python_rapidjson.egg-info/PKG-INFO` & `python-rapidjson-1.9/python_rapidjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rapidjson
-Version: 1.8
+Version: 1.9
 Summary: Python wrapper around rapidjson
 Home-page: https://github.com/python-rapidjson/python-rapidjson
 Author: Ken Robbins
 Author-email: ken@kenrobbins.com
 Maintainer: Lele Gaifax
 Maintainer-email: lele@metapensiero.it
 License: MIT License
@@ -151,14 +151,22 @@
 
 .. _RapidJSON: http://rapidjson.org/
 
 
 Changes
 -------
 
+1.9 (2022-10-17)
+~~~~~~~~~~~~~~~~
+
+* Produce Python 3.11 wheels, thanks to ``cibuildwheel`` `2.11.1`__
+
+  __ https://cibuildwheel.readthedocs.io/en/stable/changelog/#v2111
+
+
 1.8 (2022-07-07)
 ~~~~~~~~~~~~~~~~
 
 * Fix `problem on macOS`__ explicitly requiring C++11, thanks to agate-pris (`issue
   #166`__)
 
   __ https://github.com/Tencent/rapidjson/commit/9965ab37f6cfae3d58a0a6e34c76112866ace0b1#commitcomment-77875054
```

### Comparing `python-rapidjson-1.8/python_rapidjson.egg-info/SOURCES.txt` & `python-rapidjson-1.9/python_rapidjson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/allocators.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/allocators.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/cursorstreamwrapper.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/cursorstreamwrapper.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/document.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/document.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/encodedstream.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/encodedstream.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/encodings.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/encodings.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/error/en.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/error/en.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/error/error.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/error/error.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/filereadstream.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/filereadstream.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/filewritestream.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/filewritestream.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/fwd.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/fwd.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/biginteger.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/biginteger.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/clzll.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/clzll.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/diyfp.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/diyfp.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/dtoa.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/dtoa.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/ieee754.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/ieee754.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/itoa.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/itoa.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/meta.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/meta.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/pow10.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/pow10.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/regex.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/regex.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/stack.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/stack.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/strfunc.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/strfunc.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/strtod.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/strtod.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/internal/swap.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/internal/swap.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/istreamwrapper.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/istreamwrapper.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/memorybuffer.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/memorybuffer.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/memorystream.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/memorystream.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/msinttypes/inttypes.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/msinttypes/inttypes.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/msinttypes/stdint.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/msinttypes/stdint.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/ostreamwrapper.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/ostreamwrapper.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/pointer.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/pointer.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/prettywriter.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/prettywriter.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/rapidjson.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/rapidjson.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/reader.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/reader.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/schema.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/schema.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/stream.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/stream.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/stringbuffer.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/stringbuffer.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/uri.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/uri.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/include/rapidjson/writer.h` & `python-rapidjson-1.9/rapidjson/include/rapidjson/writer.h`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/license.txt` & `python-rapidjson-1.9/rapidjson/license.txt`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson/readme.md` & `python-rapidjson-1.9/rapidjson/readme.md`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/rapidjson.cpp` & `python-rapidjson-1.9/rapidjson.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 static PyObject* timezone_type = NULL;
 static PyObject* timezone_utc = NULL;
 static PyObject* uuid_type = NULL;
 static PyObject* validation_error = NULL;
 static PyObject* decode_error = NULL;
 
 
-/* These are the names of oftenly used methods or literal values, interned in the module
+/* These are the names of often used methods or literal values, interned in the module
    initialization function, to avoid repeated creation/destruction of PyUnicode values
    from plain C strings.
 
    We cannot use _Py_IDENTIFIER() because that upsets the GNU C++ compiler in -pedantic
    mode. */
 
 static PyObject* astimezone_name = NULL;
@@ -389,15 +389,15 @@
                 else
                     std::memmove(buffer, multiByteChar, remaining);
                 cursor = buffer + remaining;
                 multiByteChar = NULL;
             }
         }
         if (c == NULL) {
-            // Propagate the error state, it will be catched by dumps_internal()
+            // Propagate the error state, it will be caught by dumps_internal()
         } else {
             PyObject* res = PyObject_CallMethodObjArgs(stream, write_name, c, NULL);
             if (res == NULL) {
                 // Likewise
             } else {
                 Py_DECREF(res);
             }
@@ -2489,17 +2489,17 @@
         if (s == NULL) {
             Py_DECREF(unicodeObj);
             return false;
         }
         ASSERT_VALID_SIZE(l);
         writer->String(s, (SizeType) l);
         Py_DECREF(unicodeObj);
-    } else if ((!(iterableMode & IM_ONLY_LISTS) && PyList_Check(object))
+    } else if (PyList_CheckExact(object)
                ||
-               PyList_CheckExact(object)) {
+               (!(iterableMode & IM_ONLY_LISTS) && PyList_Check(object))) {
         writer->StartArray();
 
         Py_ssize_t size = PyList_GET_SIZE(object);
 
         for (Py_ssize_t i = 0; i < size; i++) {
             if (Py_EnterRecursiveCall(" while JSONifying list object"))
                 return false;
@@ -2523,17 +2523,17 @@
             bool r = RECURSE(item);
             Py_LeaveRecursiveCall();
             if (!r)
                 return false;
         }
 
         writer->EndArray();
-    } else if (((!(mappingMode & MM_ONLY_DICTS) && PyDict_Check(object))
+    } else if ((PyDict_CheckExact(object)
                 ||
-                PyDict_CheckExact(object))
+                (!(mappingMode & MM_ONLY_DICTS) && PyDict_Check(object)))
                &&
                ((mappingMode & MM_SKIP_NON_STRING_KEYS)
                 ||
                 (mappingMode & MM_COERCE_KEYS_TO_STRINGS)
                 ||
                 all_keys_are_string(object))) {
         writer->StartObject();
@@ -2630,15 +2630,19 @@
         PyObject* dtObject = object;
         PyObject* asUTC = NULL;
 
         const int ISOFORMAT_LEN = 42;
         char isoformat[ISOFORMAT_LEN];
         memset(isoformat, 0, ISOFORMAT_LEN);
 
-        const int TIMEZONE_LEN = 16;
+        // The timezone is always shorter than this, but gcc12 emits a warning about
+        // sprintf() that *may* produce longer results, because we pass int values when
+        // concretely they are constrained to 24*3600 seconds: pacify gcc using a bigger
+        // buffer
+        const int TIMEZONE_LEN = 24;
         char timeZone[TIMEZONE_LEN] = { 0 };
 
         if (!(datetimeMode & DM_IGNORE_TZ)
             && PyObject_HasAttr(object, utcoffset_name)) {
             PyObject* utcOffset = PyObject_CallMethodObjArgs(object,
                                                              utcoffset_name,
                                                              NULL);
```

### Comparing `python-rapidjson-1.8/requirements.txt` & `python-rapidjson-1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/setup.py` & `python-rapidjson-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/conftest.py` & `python-rapidjson-1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_base_types.py` & `python-rapidjson-1.9/tests/test_base_types.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_circular.py` & `python-rapidjson-1.9/tests/test_circular.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_dict_subclass.py` & `python-rapidjson-1.9/tests/test_dict_subclass.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_float.py` & `python-rapidjson-1.9/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_memory_leaks.py` & `python-rapidjson-1.9/tests/test_memory_leaks.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_params.py` & `python-rapidjson-1.9/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_pass1.py` & `python-rapidjson-1.9/tests/test_pass1.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_pass3.py` & `python-rapidjson-1.9/tests/test_pass3.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_rawjson.py` & `python-rapidjson-1.9/tests/test_rawjson.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_refs_count.py` & `python-rapidjson-1.9/tests/test_refs_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # :Project:   python-rapidjson -- Refs leaks tests
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   MIT License
 # :Copyright: © 2017, 2018, 2020, 2022 Lele Gaifax
 #
 
-# NB: this is a simplicistic test that uses sys.gettotalrefcount(), available
+# NB: this is a simplistic test that uses sys.gettotalrefcount(), available
 # when the interpreter is built --with-pydebug, that tries to assert that
 # repeated calls to dumps() and loads() does not leak object references.
 # Since it's not an exact science, it should be taken with a grain of salt.
 
 import datetime
 import io
 import sys
```

### Comparing `python-rapidjson-1.8/tests/test_streams.py` & `python-rapidjson-1.9/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_unicode.py` & `python-rapidjson-1.9/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tests/test_validator.py` & `python-rapidjson-1.9/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `python-rapidjson-1.8/tox.ini` & `python-rapidjson-1.9/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/media-management-scripts-0.5.2.tar.gz` & `tmp/media_management_scripts-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media-management-scripts-0.5.2.tar", last modified: Sun Oct 22 01:28:27 2023, max compression
+gzip compressed data, was "media_management_scripts-0.5.3.tar", last modified: Sat May 18 01:58:11 2024, max compression
```

## Comparing `media-management-scripts-0.5.2.tar` & `media_management_scripts-0.5.3.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 01:28:27.133120 media-management-scripts-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2023-10-22 01:28:27.133120 media-management-scripts-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 01:28:27.121120 media-management-scripts-0.5.2/media_management_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 01:28:27.133120 media-management-scripts-0.5.2/media_management_scripts/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/combine_subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/compare_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/concat_mp4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/create_test_video.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/filebot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/find_episodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/itunes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/metadata_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/movie_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/select_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/commands/tv_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/convert_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/moviedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/renamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 01:28:27.133120 media-management-scripts-0.5.2/media_management_scripts/support/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/combine_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/concat_mp4.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/episode_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/interlace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11830 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/movie_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/search_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/test_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/support/ttml2srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/tvdb_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/media_management_scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 01:28:27.125120 media-management-scripts-0.5.2/media_management_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2023-10-22 01:28:27.000000 media-management-scripts-0.5.2/media_management_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-10-22 01:28:27.000000 media-management-scripts-0.5.2/media_management_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-22 01:28:27.000000 media-management-scripts-0.5.2/media_management_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-10-22 01:28:27.000000 media-management-scripts-0.5.2/media_management_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-22 01:28:26.000000 media-management-scripts-0.5.2/media_management_scripts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-22 01:28:27.000000 media-management-scripts-0.5.2/media_management_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-22 01:28:27.000000 media-management-scripts-0.5.2/media_management_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-22 01:28:27.133120 media-management-scripts-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 01:28:27.133120 media-management-scripts-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_concat_mp4.py
--rw-r--r--   0 runner    (1001) docker     (127)     9097 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_convert_dvd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_find_episodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_search_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-10-22 01:28:14.000000 media-management-scripts-0.5.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:11.359873 media_management_scripts-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-18 01:58:11.359873 media_management_scripts-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:11.351873 media_management_scripts-0.5.3/media_management_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:11.355873 media_management_scripts-0.5.3/media_management_scripts/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/combine_subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/compare_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/concat_mp4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/create_test_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/filebot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/find_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/itunes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/map_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/metadata_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/movie_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/select_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/commands/tv_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/convert_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/moviedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/renamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:11.355873 media_management_scripts-0.5.3/media_management_scripts/support/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/combine_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/concat_mp4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/episode_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/interlace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/movie_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/search_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/support/ttml2srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/tvdb_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/media_management_scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:11.359873 media_management_scripts-0.5.3/media_management_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-18 01:58:11.000000 media_management_scripts-0.5.3/media_management_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-18 01:58:11.000000 media_management_scripts-0.5.3/media_management_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:58:11.000000 media_management_scripts-0.5.3/media_management_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-18 01:58:11.000000 media_management_scripts-0.5.3/media_management_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:58:11.000000 media_management_scripts-0.5.3/media_management_scripts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-18 01:58:11.000000 media_management_scripts-0.5.3/media_management_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 01:58:11.000000 media_management_scripts-0.5.3/media_management_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:58:11.359873 media_management_scripts-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:58:11.359873 media_management_scripts-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_concat_mp4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_convert_dvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_find_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_search_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-18 01:58:02.000000 media_management_scripts-0.5.3/tests/test_utils.py
```

### Comparing `media-management-scripts-0.5.2/LICENSE` & `media_management_scripts-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/PKG-INFO` & `media_management_scripts-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 Metadata-Version: 2.1
 Name: media-management-scripts
-Version: 0.5.2
+Version: 0.5.3
 Summary: Media Management Scripts
 Author: Ray Douglass
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/raydouglass/media_management_scripts
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pycaption
+Requires-Dist: pyparsing
+Requires-Dist: python-magic
+Requires-Dist: pythondialog
+Requires-Dist: pyyaml
 Requires-Dist: requests
-Requires-Dist: pyOpenSSL
+Requires-Dist: tempita
 Requires-Dist: texttable
 Requires-Dist: tmdbsimple
-Requires-Dist: argcomplete
-Requires-Dist: tempita
-Requires-Dist: pysrt
-Requires-Dist: pythondialog
-Requires-Dist: pyyaml
-Requires-Dist: pyparsing
-Requires-Dist: pycaption
-Requires-Dist: python-magic
 
 # Media Management Scripts
 
 This is a collection of command line tools for managing media files such as movies or TV shows.
 
 It also simplifies some common tasks such as converting files by wrapping complex `ffmpeg` commands.
 
 For example, to convert a file to H.265/HEVC with GPU acceleration and AAC audio, plus scale it down to 480p, you would normally have to run a command like:
 ```sh
-ffmpeg -hwaccel cuda -hwaccel_output_format cuda -i test.mp4 -vf scale=-1:480 -c:v h264_nvenc -preset fast -c:a aac -c:s copy -map 0 out.mp4
+ffmpeg -hwaccel cuda -hwaccel_output_format cuda -i test.mp4 -vf scale=-1:480 -c:v hevc_nvenc -preset fast -c:a aac -c:s copy -map 0 out.mp4
 ```
 Using this toolkit, it would be this instead:
 ```sh
-manage-media convert --hw-nv --scale 480 --vc h264 test.mp4 out.mp4
+manage-media convert --hw-nv --scale 480 --vc h265 test.mp4 out.mp4
 ```
 
 ## Installation
 
 Install the tools:
 
 `pip install media_management_scripts`
```

### Comparing `media-management-scripts-0.5.2/README.md` & `media_management_scripts-0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 This is a collection of command line tools for managing media files such as movies or TV shows.
 
 It also simplifies some common tasks such as converting files by wrapping complex `ffmpeg` commands.
 
 For example, to convert a file to H.265/HEVC with GPU acceleration and AAC audio, plus scale it down to 480p, you would normally have to run a command like:
 ```sh
-ffmpeg -hwaccel cuda -hwaccel_output_format cuda -i test.mp4 -vf scale=-1:480 -c:v h264_nvenc -preset fast -c:a aac -c:s copy -map 0 out.mp4
+ffmpeg -hwaccel cuda -hwaccel_output_format cuda -i test.mp4 -vf scale=-1:480 -c:v hevc_nvenc -preset fast -c:a aac -c:s copy -map 0 out.mp4
 ```
 Using this toolkit, it would be this instead:
 ```sh
-manage-media convert --hw-nv --scale 480 --vc h264 test.mp4 out.mp4
+manage-media convert --hw-nv --scale 480 --vc h265 test.mp4 out.mp4
 ```
 
 ## Installation
 
 Install the tools:
 
 `pip install media_management_scripts`
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/__init__.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import ABCMeta, abstractmethod
 import shutil
+import sys
 from typing import List, Tuple, Callable
 from media_management_scripts.support.files import check_exists, create_dirs
+from media_management_scripts.utils import to_int
 
 
 class SubCommand(metaclass=ABCMeta):
     def __init__(self):
         self.dry_run = False
         self.ns = None
 
@@ -21,30 +23,33 @@
     @abstractmethod
     def subexecute(self, ns):
         raise Exception("Not implemented")
 
     def execute(self, ns):
         self.dry_run = ns["dry_run"]
         self.ns = ns
-        self.subexecute(ns)
+        result = self.subexecute(ns)
+        result = to_int(result)
+        if result is not None and result != 0:
+            sys.exit(int(result))
 
-    def _move(self, src, dst, overwrite=False):
-        if self.dry_run:
+    def _move(self, src, dst, overwrite=False, print_output=False):
+        if self.dry_run or print_output:
             print("Move: {}=>{}".format(src, dst))
-        else:
+        if not self.dry_run:
             if not overwrite and check_exists(dst, log=self.dry_run):
                 return False
             create_dirs(dst)
             shutil.move(src, dst)
             return True
 
-    def _copy(self, src, dst, overwrite=False):
-        if self.dry_run:
+    def _copy(self, src, dst, overwrite=False, print_output=False):
+        if self.dry_run or print_output:
             print("Copy: {}=>{}".format(src, dst))
-        else:
+        if not self.dry_run:
             if not overwrite and check_exists(dst, log=self.dry_run):
                 return False
             create_dirs(dst)
             shutil.copy(src, dst)
             return True
 
     def _bulk(
@@ -147,14 +152,15 @@
     "combine_subtitles",
     #'compare_directories',
     "concat_mp4",
     "convert",
     "executables",
     "find_episodes",
     "itunes",
+    "map_rename",
     "metadata",
     "metadata_compare",
     "movie_rename",
     "rename",
     "search",
     "select_streams",
     #'split',
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/combine_subtitles.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/combine_subtitles.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/common.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/common.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/compare_directories.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/compare_directories.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/concat_mp4.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/convert.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from .common import *
 import argparse
 import os
 from media_management_scripts.support.files import get_input_output, movie_files_filter
 from media_management_scripts.convert import convert_with_config
 
 
-def _bulk_convert(i, o, config, overwrite):
+def _bulk_convert(i, o, config, overwrite, dry_run):
     print("Starting {}".format(i))
     os.makedirs(os.path.dirname(o), exist_ok=True)
-    convert_with_config(i, o, config, print_output=True, overwrite=overwrite)
+    convert_with_config(
+        i, o, config, print_output=True, overwrite=overwrite, dry_run=dry_run
+    )
 
 
 class ConvertCommand(SubCommand):
     @property
     def name(self):
         return "convert"
 
@@ -59,14 +61,15 @@
 
         input_to_cmd = ns["input"]
         output = ns["output"]
         overwrite = ns["overwrite"]
         bulk = ns["bulk"]
         bulk_ext = ns["bulk_ext"]
         config = convert_config_from_ns(ns)
+        dry_run = ns["dry_run"]
 
         if os.path.isdir(input_to_cmd):
             if bulk:
                 os.makedirs(output, exist_ok=True)
                 files = list(
                     get_input_output(input_to_cmd, output, filter=movie_files_filter)
                 )
@@ -78,21 +81,26 @@
                                 os.path.splitext(i[1])[0] + "." + bulk_ext,
                             ),
                             files,
                         )
                     )
                 self._bulk(
                     files,
-                    lambda i, o: _bulk_convert(i, o, config, overwrite),
+                    lambda i, o: _bulk_convert(i, o, config, overwrite, dry_run),
                     ["Input", "Output"],
                 )
             else:
-                print("Cowardly refusing to convert a direction without --bulk flag")
+                print("Cowardly refusing to convert a directory without --bulk flag")
         elif not overwrite and os.path.exists(output):
             print("Cowardly refusing to overwrite existing file: {}".format(output))
         else:
             convert_with_config(
-                input_to_cmd, output, config, print_output=True, overwrite=overwrite
+                input_to_cmd,
+                output,
+                config,
+                print_output=True,
+                overwrite=overwrite,
+                dry_run=dry_run,
             )
 
 
 SubCommand.register(ConvertCommand)
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/create_test_video.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/create_test_video.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/executables.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/executables.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/filebot.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/filebot.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/find_episodes.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/find_episodes.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/itunes.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/itunes.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/metadata.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/metadata_compare.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/metadata_compare.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/movie_rename.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/movie_rename.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/rename.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/rename.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/search.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/search.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/select_streams.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/select_streams.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/split.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/split.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/subtitles.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/subtitles.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/thumbnail.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/thumbnail.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/commands/tv_rename.py` & `media_management_scripts-0.5.3/media_management_scripts/commands/tv_rename.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/convert.py` & `media_management_scripts-0.5.3/media_management_scripts/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     VideoCodec,
     AudioCodec,
 )
 from media_management_scripts.support.executables import (
     execute_with_output,
     ffmpeg,
     nice_exe,
+    log_command,
 )
 from media_management_scripts.support.files import (
     check_exists,
     create_dirs,
     get_input_output,
 )
 from media_management_scripts.support.formatting import sizeof_fmt
@@ -66,14 +67,15 @@
     output,
     config: ConvertConfig,
     print_output=True,
     overwrite=False,
     metadata=None,
     mappings=None,
     use_nice=True,
+    dry_run=False,
 ):
     """
 
     :param input:
     :param output:
     :param config:
     :param print_output:
@@ -201,28 +203,36 @@
             args.extend(["-ac:a:{}".format(index), "8"])
         index += 1
 
     if config.include_subtitles:
         args.extend(["-c:s", "copy"])
 
     if not mappings:
-        args.extend(["-map", "0"])
+        if metadata.video_streams:
+            args.extend(["-map", "0:v"])
+        if metadata.audio_streams:
+            args.extend(["-map", "0:a"])
+        if metadata.subtitle_streams:
+            args.extend(["-map", "0:s"])
     else:
         for m in mappings:
             if type(m) == int:
                 args.extend(["-map", "0:{}".format(m)])
             else:
                 args.extend(["-map", m])
 
     if config.include_meta:
         args.extend(["-metadata", "ripped=true"])
         args.extend(["-metadata:s:v:0", "ripped=true"])
     args.append(output)
 
-    return execute(args, print_output)
+    if dry_run:
+        log_command(args, True)
+    else:
+        return execute(args, print_output)
 
 
 def create_remux_args(
     input_files: List[str],
     output_file: str,
     mappings: List,
     overwrite=False,
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/convert_daemon.py` & `media_management_scripts-0.5.3/media_management_scripts/convert_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         return chain(
             self.get_existing_success(self.movie_in_dir, self.movie_out_dir),
             self.get_existing_success(self.tv_in_dir, self.tv_out_dir),
         )
 
 
 def main():
-    import argparse, argcomplete
+    import argparse
 
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(help="Sub commands", dest="command")
     parent_parser = argparse.ArgumentParser(add_help=False)
     parent_parser.add_argument("config", type=str)
     run_parser = subparsers.add_parser(
         "run", help="Run the convert DVD process", parents=[parent_parser]
@@ -307,15 +307,14 @@
     list_parser = subparsers.add_parser(
         "list",
         help="List files that have been processed successfully",
         parents=[parent_parser],
     )
     list_parser.add_argument("-0", action="store_const", const=True, default=False)
 
-    argcomplete.autocomplete(parser)
     ns = vars(parser.parse_args())
     cmd = ns["command"]
     config = ns["config"]
     convert_dvds = ConvertDvds(config)
 
     if cmd == "run":
         convert_dvds.run()
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/main.py` & `media_management_scripts-0.5.3/media_management_scripts/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import argcomplete
 import sys
 
 from media_management_scripts.commands import *
 from media_management_scripts import __version__ as version
 
 COMMANDS = {k.name: k for k in [x() for x in SubCommand.__subclasses__()]}
 
@@ -33,15 +32,14 @@
         const=True,
         default=False,
     )
     subparsers = parser.add_subparsers(help="Sub commands", dest="command")
 
     for cmd in COMMANDS.values():
         cmd.build_argparse(subparsers)
-    argcomplete.autocomplete(parser)
     return parser
 
 
 def main():
     parser = build_argparse()
     try:
         ns = vars(parser.parse_args())
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/moviedb.py` & `media_management_scripts-0.5.3/media_management_scripts/moviedb.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/renamer.py` & `media_management_scripts-0.5.3/media_management_scripts/renamer.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/combine_all.py` & `media_management_scripts-0.5.3/media_management_scripts/support/combine_all.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/concat_mp4.py` & `media_management_scripts-0.5.3/media_management_scripts/support/concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/encoding.py` & `media_management_scripts-0.5.3/media_management_scripts/support/encoding.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/episode_finder.py` & `media_management_scripts-0.5.3/media_management_scripts/support/episode_finder.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/executables.py` & `media_management_scripts-0.5.3/media_management_scripts/support/executables.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,30 @@
             speed = float(self.speed[:-1])
             time_as_seconds = self.time_as_seconds
             return (duration - time_as_seconds) / speed if time_as_seconds else None
         except ValueError:
             return None
 
 
+def log_command(args, print_output=False):
+    import shlex
+
+    logger.debug(f"Executing: {shlex.join(args)}")
+    if print_output:
+        print(f"Executing: {shlex.join(args)}")
+
+
+def maybe_add_nice(args, use_nice=False):
+    if args and use_nice and nice_exe and args[0] != nice_exe:
+        a = [nice_exe]
+        a.extend(args)
+        return a
+    return args
+
+
 def create_ffmpeg_callback(
     cb: Callable[[FFMpegProgress], None]
 ) -> Callable[[str], None]:
     """
     Converts a callback function that accepts a FFMpegProgress to one that accepts a str for use in execute_with_callback
     :param cb:
     :return:
@@ -132,19 +148,16 @@
 
     return wrapper
 
 
 def execute_with_timeout(
     args, timeout: int, use_nice=True, log_output=False
 ) -> Tuple[int, str]:
-    if use_nice:
-        a = [nice_exe]
-        a.extend(args)
-        args = a
-    logger.debug("Executing: {}".format(args))
+    args = maybe_add_nice(args, use_nice)
+    log_command(args, False)
     with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as p:
         stdout, stderr = p.communicate()
         if stdout and log_output:
             exe_logger.info(stdout)
         if stderr and log_output:
             exe_logger.error(stderr)
         try:
@@ -152,21 +165,18 @@
         except subprocess.TimeoutExpired as e:
             p.kill()
             p.communicate()
             raise e
 
 
 def execute_with_output(args, print_output=False, use_nice=True) -> Tuple[int, str]:
-    if use_nice and nice_exe:
-        a = [nice_exe]
-        a.extend(args)
-        args = a
-    logger.debug("Executing: {}".format(args))
-    if print_output:
-        print("Executing: {}".format(" ".join([str(a) for a in args])))
+    if not args:
+        raise ValueError("No args provided")
+    args = maybe_add_nice(args, use_nice)
+    log_command(args, print_output)
     if DEBUG_MODE:
         logger.debug("Debug mod enabled, skipping actual execution")
         return 0
     with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT) as p:
         output = StringIO()
         while p.poll() is None:
             l = p.stdout.read(1)
@@ -197,19 +207,16 @@
         output.close()
         return p.poll(), result
 
 
 def execute_with_callback(
     args: List[str], callback: Callable[[str], None], use_nice: bool = True
 ) -> int:
-    if use_nice and nice_exe:
-        a = [nice_exe]
-        a.extend(args)
-        args = a
-    logger.debug("Executing: {}".format(args))
+    args = maybe_add_nice(args, use_nice)
+    log_command(args, False)
     with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT) as p:
         output = StringIO()
 
         while p.poll() is None:
             try:
                 l = p.stdout.read(1)
             except IOError:
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/files.py` & `media_management_scripts-0.5.3/media_management_scripts/support/files.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/formatting.py` & `media_management_scripts-0.5.3/media_management_scripts/support/formatting.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/interlace.py` & `media_management_scripts-0.5.3/media_management_scripts/support/interlace.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/metadata.py` & `media_management_scripts-0.5.3/media_management_scripts/support/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
                 if tag.startswith("DURATION") and DURATION_PATTERN.match(
                     self.tags[tag]
                 ):
                     # 01:31:21.856000000
                     parts = [float(s) for s in self.tags[tag].split(":")]
                     self.duration = parts[0] * 60 * 60 + parts[1] * 60 + parts[2]
         if self.is_video():
+            self.level = stream.get("level", None)
             self.bit_depth = None
             if self.codec in ("h264", "hevc"):
                 pix_fmt = stream.get("pix_fmt", None)
                 # TODO: This is not really accurate
                 try:
                     depth = BitDepth.get_from_pix_fmt(pix_fmt)
                     self.bit_depth = depth.bits if depth else None
@@ -245,14 +246,15 @@
             d["channel_layout"] = self.channel_layout
         if self.is_audio() or self.is_subtitle():
             d["language"] = self.language
         if self.is_video():
             d["width"] = self.width
             d["height"] = self.height
             d["bit_depth"] = self.bit_depth
+            d["level"] = self.level
         d["tags"] = self.tags
         return d
 
     def __repr__(self):
         return "<Stream: index={}, codec={}, type={}, lang={}, width={}, height={}>".format(
             self.index,
             self.codec,
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/movie_rename.py` & `media_management_scripts-0.5.3/media_management_scripts/support/movie_rename.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/search_parser.py` & `media_management_scripts-0.5.3/media_management_scripts/support/search_parser.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/split.py` & `media_management_scripts-0.5.3/media_management_scripts/support/split.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/test_video.py` & `media_management_scripts-0.5.3/media_management_scripts/support/test_video.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/support/ttml2srt.py` & `media_management_scripts-0.5.3/media_management_scripts/support/ttml2srt.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/tvdb_api.py` & `media_management_scripts-0.5.3/media_management_scripts/tvdb_api.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts/utils.py` & `media_management_scripts-0.5.3/media_management_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/media_management_scripts.egg-info/PKG-INFO` & `media_management_scripts-0.5.3/media_management_scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 Metadata-Version: 2.1
 Name: media-management-scripts
-Version: 0.5.2
+Version: 0.5.3
 Summary: Media Management Scripts
 Author: Ray Douglass
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/raydouglass/media_management_scripts
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pycaption
+Requires-Dist: pyparsing
+Requires-Dist: python-magic
+Requires-Dist: pythondialog
+Requires-Dist: pyyaml
 Requires-Dist: requests
-Requires-Dist: pyOpenSSL
+Requires-Dist: tempita
 Requires-Dist: texttable
 Requires-Dist: tmdbsimple
-Requires-Dist: argcomplete
-Requires-Dist: tempita
-Requires-Dist: pysrt
-Requires-Dist: pythondialog
-Requires-Dist: pyyaml
-Requires-Dist: pyparsing
-Requires-Dist: pycaption
-Requires-Dist: python-magic
 
 # Media Management Scripts
 
 This is a collection of command line tools for managing media files such as movies or TV shows.
 
 It also simplifies some common tasks such as converting files by wrapping complex `ffmpeg` commands.
 
 For example, to convert a file to H.265/HEVC with GPU acceleration and AAC audio, plus scale it down to 480p, you would normally have to run a command like:
 ```sh
-ffmpeg -hwaccel cuda -hwaccel_output_format cuda -i test.mp4 -vf scale=-1:480 -c:v h264_nvenc -preset fast -c:a aac -c:s copy -map 0 out.mp4
+ffmpeg -hwaccel cuda -hwaccel_output_format cuda -i test.mp4 -vf scale=-1:480 -c:v hevc_nvenc -preset fast -c:a aac -c:s copy -map 0 out.mp4
 ```
 Using this toolkit, it would be this instead:
 ```sh
-manage-media convert --hw-nv --scale 480 --vc h264 test.mp4 out.mp4
+manage-media convert --hw-nv --scale 480 --vc h265 test.mp4 out.mp4
 ```
 
 ## Installation
 
 Install the tools:
 
 `pip install media_management_scripts`
```

### Comparing `media-management-scripts-0.5.2/media_management_scripts.egg-info/SOURCES.txt` & `media_management_scripts-0.5.3/media_management_scripts.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 media_management_scripts/commands/concat_mp4.py
 media_management_scripts/commands/convert.py
 media_management_scripts/commands/create_test_video.py
 media_management_scripts/commands/executables.py
 media_management_scripts/commands/filebot.py
 media_management_scripts/commands/find_episodes.py
 media_management_scripts/commands/itunes.py
+media_management_scripts/commands/map_rename.py
 media_management_scripts/commands/metadata.py
 media_management_scripts/commands/metadata_compare.py
 media_management_scripts/commands/movie_rename.py
 media_management_scripts/commands/rename.py
 media_management_scripts/commands/search.py
 media_management_scripts/commands/select_streams.py
 media_management_scripts/commands/split.py
```

### Comparing `media-management-scripts-0.5.2/pyproject.toml` & `media_management_scripts-0.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,26 +21,23 @@
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "Ray Douglass" },
 ]
 license = { text = "Apache 2.0" }
 requires-python = ">=3.9"
 dependencies = [
+  "pycaption",
+  "pyparsing",
+  "python-magic",
+  "pythondialog",
+  "pyyaml",
   "requests",
-  "pyOpenSSL",
+  "tempita",
   "texttable",
   "tmdbsimple",
-  "argcomplete",
-  "tempita",
-  "pysrt",
-  "pythondialog",
-  "pyyaml",
-  "pyparsing",
-  "pycaption",
-  "python-magic",
 ]
 classifiers = [
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
 ]
```

### Comparing `media-management-scripts-0.5.2/tests/test_combine.py` & `media_management_scripts-0.5.3/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_concat_mp4.py` & `media_management_scripts-0.5.3/tests/test_concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_convert.py` & `media_management_scripts-0.5.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_convert_dvd.py` & `media_management_scripts-0.5.3/tests/test_convert_dvd.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_find_episodes.py` & `media_management_scripts-0.5.3/tests/test_find_episodes.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_formatting.py` & `media_management_scripts-0.5.3/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_metadata.py` & `media_management_scripts-0.5.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_rename.py` & `media_management_scripts-0.5.3/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_search.py` & `media_management_scripts-0.5.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_search_parser.py` & `media_management_scripts-0.5.3/tests/test_search_parser.py`

 * *Files identical despite different names*

### Comparing `media-management-scripts-0.5.2/tests/test_utils.py` & `media_management_scripts-0.5.3/tests/test_utils.py`

 * *Files identical despite different names*


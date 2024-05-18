# Comparing `tmp/hgitaly-1.4.1.tar.gz` & `tmp/hgitaly-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgitaly-1.4.1.tar", last modified: Wed May  8 21:11:38 2024, max compression
+gzip compressed data, was "hgitaly-1.5.0.tar", last modified: Sat May 18 14:06:03 2024, max compression
```

## Comparing `hgitaly-1.4.1.tar` & `hgitaly-1.5.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.073813 hgitaly-1.4.1/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2022-07-07 20:49:19.000000 hgitaly-1.4.1/LICENSE
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2022-07-07 20:49:19.000000 hgitaly-1.4.1/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-08 21:11:38.073813 hgitaly-1.4.1/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-02-14 14:38:06.000000 hgitaly-1.4.1/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.056813 hgitaly-1.4.1/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.056813 hgitaly-1.4.1/hgext3rd/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgext3rd/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgext3rd/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.056813 hgitaly-1.4.1/hgext3rd/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgext3rd/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgext3rd/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgext3rd/hgitaly/tests/test_serve.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.059813 hgitaly-1.4.1/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-08 20:50:17.000000 hgitaly-1.4.1/hgitaly/VERSION
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/changelog.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-04-03 07:33:18.000000 hgitaly-1.4.1/hgitaly/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4985 2024-05-08 20:48:41.000000 hgitaly-1.4.1/hgitaly/errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5607 2024-05-08 20:48:41.000000 hgitaly-1.4.1/hgitaly/file_content.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgitaly/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6908 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/gitlab_ref.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.060813 hgitaly-1.4.1/hgitaly/license_detector/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2023-11-21 17:47:45.000000 hgitaly-1.4.1/hgitaly/license_detector/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2023-11-21 17:47:45.000000 hgitaly-1.4.1/hgitaly/license_detector/spdx-licenses.json
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.061813 hgitaly-1.4.1/hgitaly/linguist/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/linguist/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/linguist/languages.json
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/logging.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgitaly/message.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-04-03 07:33:18.000000 hgitaly-1.4.1/hgitaly/oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2022-07-20 18:29:40.000000 hgitaly-1.4.1/hgitaly/pagination.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/path.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/procutil.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8872 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.061813 hgitaly-1.4.1/hgitaly/server/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6288 2024-05-08 20:48:41.000000 hgitaly-1.4.1/hgitaly/server/mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/prefork.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.062813 hgitaly-1.4.1/hgitaly/server/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/tests/test_address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/tests/test_mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/tests/test_prefork.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/tests/test_worker.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/server/worker.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.063813 hgitaly-1.4.1/hgitaly/service/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/service/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1787 2024-05-08 20:48:41.000000 hgitaly-1.4.1/hgitaly/service/analysis.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2023-09-04 20:36:56.000000 hgitaly-1.4.1/hgitaly/service/blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    46662 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/service/commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgitaly/service/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/service/interceptors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/service/mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16868 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/service/mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/service/mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/service/operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-04-03 07:33:18.000000 hgitaly-1.4.1/hgitaly/service/ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    35623 2024-03-14 20:29:37.000000 hgitaly-1.4.1/hgitaly/service/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/service/server.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.065813 hgitaly-1.4.1/hgitaly/service/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/service/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/service/tests/fixture.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3972 2024-05-08 20:48:41.000000 hgitaly-1.4.1/hgitaly/service/tests/test_analysis.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2023-09-04 20:36:56.000000 hgitaly-1.4.1/hgitaly/service/tests/test_blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    52689 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/service/tests/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2023-11-14 22:18:49.000000 hgitaly-1.4.1/hgitaly/service/tests/test_default_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgitaly/service/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/service/tests/test_mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/service/tests/test_mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/service/tests/test_mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/service/tests/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-04-03 07:33:18.000000 hgitaly-1.4.1/hgitaly/service/tests/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    49404 2024-03-14 20:29:37.000000 hgitaly-1.4.1/hgitaly/service/tests/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/service/tests/test_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgitaly/stream.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.068813 hgitaly-1.4.1/hgitaly/stub/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/stub/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2812 2024-05-08 20:48:41.000000 hgitaly-1.4.1/hgitaly/stub/analysis_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3419 2024-05-08 20:48:41.000000 hgitaly-1.4.1/hgitaly/stub/analysis_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9342 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/stub/blob_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/stub/blob_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-04-03 07:33:18.000000 hgitaly-1.4.1/hgitaly/stub/commit_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/stub/commit_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16478 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/stub/diff_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15634 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/stub/diff_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-04-03 07:33:18.000000 hgitaly-1.4.1/hgitaly/stub/errors_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/stub/errors_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/stub/lint_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/stub/lint_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/stub/mercurial_changeset_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/stub/mercurial_changeset_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/stub/mercurial_operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/stub/mercurial_operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11048 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/stub/mercurial_repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/stub/mercurial_repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29658 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/stub/operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/stub/operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-02-14 14:37:31.000000 hgitaly-1.4.1/hgitaly/stub/ref_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-02-14 14:37:31.000000 hgitaly-1.4.1/hgitaly/stub/ref_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47292 2024-04-03 07:33:18.000000 hgitaly-1.4.1/hgitaly/stub/repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    79550 2024-05-08 20:48:35.000000 hgitaly-1.4.1/hgitaly/stub/repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/stub/server_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/stub/server_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-01-20 14:39:14.000000 hgitaly-1.4.1/hgitaly/stub/shared_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/stub/shared_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.069813 hgitaly-1.4.1/hgitaly/testing/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/testing/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/testing/bundle.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/testing/context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/testing/grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/testing/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/testing/sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.069813 hgitaly-1.4.1/hgitaly/testing/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/testing/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/testing/tests/test_sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.071813 hgitaly-1.4.1/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/tests/common.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgitaly/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-02-13 21:06:34.000000 hgitaly-1.4.1/hgitaly/tests/test_errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/tests/test_file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4599 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_gitlab_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2023-11-21 17:47:45.000000 hgitaly-1.4.1/hgitaly/tests/test_license_detector.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2023-11-21 17:47:45.000000 hgitaly-1.4.1/hgitaly/tests/test_linguist.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/tests/test_manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_messages.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2022-07-07 20:49:19.000000 hgitaly-1.4.1/hgitaly/tests/test_oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/tests/test_servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-02-14 14:38:06.000000 hgitaly-1.4.1/hgitaly/tests/test_stream.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2023-07-26 15:42:21.000000 hgitaly-1.4.1/hgitaly/tests/test_tag.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/tests/test_workdir.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2023-11-13 22:51:48.000000 hgitaly-1.4.1/hgitaly/util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-01-20 11:36:48.000000 hgitaly-1.4.1/hgitaly/workdir.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.060813 hgitaly-1.4.1/hgitaly.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-08 21:11:38.000000 hgitaly-1.4.1/hgitaly.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4680 2024-05-08 21:11:38.000000 hgitaly-1.4.1/hgitaly.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-08 21:11:38.000000 hgitaly-1.4.1/hgitaly.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-08 21:11:38.000000 hgitaly-1.4.1/hgitaly.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-05-08 21:11:38.000000 hgitaly-1.4.1/hgitaly.egg-info/top_level.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-02-13 21:06:34.000000 hgitaly-1.4.1/install-requirements.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-08 21:11:38.073813 hgitaly-1.4.1/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2023-11-21 17:46:05.000000 hgitaly-1.4.1/setup.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-08 21:11:38.073813 hgitaly-1.4.1/tests_with_gitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24261 2024-05-08 20:48:41.000000 hgitaly-1.4.1/tests_with_gitaly/comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3545 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/conftest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/gitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1775 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2509 2024-03-14 20:29:37.000000 hgitaly-1.4.1/tests_with_gitaly/rhgitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25320 2024-05-08 20:48:41.000000 hgitaly-1.4.1/tests_with_gitaly/test_blob_tree.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    31285 2024-05-08 20:48:35.000000 hgitaly-1.4.1/tests_with_gitaly/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/test_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-04-03 07:33:18.000000 hgitaly-1.4.1/tests_with_gitaly/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/test_gitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-02-13 21:06:34.000000 hgitaly-1.4.1/tests_with_gitaly/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-04-03 07:33:18.000000 hgitaly-1.4.1/tests_with_gitaly/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32102 2024-04-03 07:33:18.000000 hgitaly-1.4.1/tests_with_gitaly/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/test_rhgitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      820 2023-07-26 15:42:21.000000 hgitaly-1.4.1/tests_with_gitaly/test_server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.646772 hgitaly-1.5.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2024-05-01 16:09:12.000000 hgitaly-1.5.0/LICENSE
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2024-05-01 16:09:12.000000 hgitaly-1.5.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-18 14:06:03.646772 hgitaly-1.5.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-05-01 16:09:12.000000 hgitaly-1.5.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.625772 hgitaly-1.5.0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.625772 hgitaly-1.5.0/hgext3rd/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.626772 hgitaly-1.5.0/hgext3rd/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_serve.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.630772 hgitaly-1.5.0/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-18 14:05:28.000000 hgitaly-1.5.0/hgitaly/VERSION
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/changelog.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4985 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5607 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/file_content.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7133 2024-05-18 12:05:55.000000 hgitaly-1.5.0/hgitaly/gitlab_ref.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.631772 hgitaly-1.5.0/hgitaly/license_detector/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/license_detector/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/license_detector/spdx-licenses.json
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.631772 hgitaly-1.5.0/hgitaly/linguist/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/linguist/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/linguist/languages.json
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/logging.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/message.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/pagination.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/path.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/procutil.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8872 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.632772 hgitaly-1.5.0/hgitaly/server/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6288 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/server/mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/prefork.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.632772 hgitaly-1.5.0/hgitaly/server/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_prefork.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_worker.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/worker.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.634772 hgitaly-1.5.0/hgitaly/service/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1787 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/service/analysis.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    46662 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/interceptors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16868 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    35623 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.635772 hgitaly-1.5.0/hgitaly/service/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/fixture.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3972 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/service/tests/test_analysis.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    52689 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_default_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    49404 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stream.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.641772 hgitaly-1.5.0/hgitaly/stub/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2812 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/stub/analysis_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3419 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/stub/analysis_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9342 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/blob_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/blob_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/commit_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/commit_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16478 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/diff_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15634 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/diff_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/errors_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/errors_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/lint_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/lint_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11048 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29658 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/ref_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/ref_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47292 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    79550 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/server_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/server_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/shared_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/shared_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.642772 hgitaly-1.5.0/hgitaly/testing/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/bundle.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.642772 hgitaly-1.5.0/hgitaly/testing/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/tests/test_sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.644772 hgitaly-1.5.0/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/common.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4932 2024-05-18 12:11:23.000000 hgitaly-1.5.0/hgitaly/tests/test_gitlab_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_license_detector.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_linguist.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_messages.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_stream.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_tag.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_workdir.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/workdir.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.630772 hgitaly-1.5.0/hgitaly.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4680 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/top_level.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-01 16:09:12.000000 hgitaly-1.5.0/install-requirements.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-18 14:06:03.646772 hgitaly-1.5.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2024-05-01 16:09:12.000000 hgitaly-1.5.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.645772 hgitaly-1.5.0/tests_with_gitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24577 2024-05-18 11:58:42.000000 hgitaly-1.5.0/tests_with_gitaly/comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3545 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/conftest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/gitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1775 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2509 2024-05-18 13:40:58.000000 hgitaly-1.5.0/tests_with_gitaly/rhgitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25320 2024-05-17 13:05:58.000000 hgitaly-1.5.0/tests_with_gitaly/test_blob_tree.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    34125 2024-05-18 13:51:59.000000 hgitaly-1.5.0/tests_with_gitaly/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_gitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32317 2024-05-17 18:28:22.000000 hgitaly-1.5.0/tests_with_gitaly/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_rhgitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      820 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_server.py
```

### Comparing `hgitaly-1.4.1/LICENSE` & `hgitaly-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/PKG-INFO` & `hgitaly-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 1.4.1
+Version: 1.5.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Requires-Python: >=3.8
```

### Comparing `hgitaly-1.4.1/README.md` & `hgitaly-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgext3rd/hgitaly/__init__.py` & `hgitaly-1.5.0/hgext3rd/hgitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgext3rd/hgitaly/revset.py` & `hgitaly-1.5.0/hgext3rd/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgext3rd/hgitaly/tests/test_revset.py` & `hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgext3rd/hgitaly/tests/test_serve.py` & `hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/branch.py` & `hgitaly-1.5.0/hgitaly/branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/changelog.py` & `hgitaly-1.5.0/hgitaly/changelog.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/diff.py` & `hgitaly-1.5.0/hgitaly/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/errors.py` & `hgitaly-1.5.0/hgitaly/errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/feature.py` & `hgitaly-1.5.0/hgitaly/feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/file_content.py` & `hgitaly-1.5.0/hgitaly/file_content.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/file_context.py` & `hgitaly-1.5.0/hgitaly/file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/git.py` & `hgitaly-1.5.0/hgitaly/git.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/gitlab_ref.py` & `hgitaly-1.5.0/hgitaly/gitlab_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,19 @@
 from hgext3rd.heptapod import ensure_gitlab_special_refs
 from hgext3rd.heptapod import ensure_gitlab_keep_arounds
 from hgext3rd.heptapod.special_ref import (
     GITLAB_TYPED_REFS_MISSING,
     parse_special_ref,
     special_refs,
 )
-from hgext3rd.heptapod.keep_around import iter_keep_arounds
+from hgext3rd.heptapod.keep_around import (
+    iter_keep_arounds,
+    KEEP_AROUND_REF_PREFIX,
+    KEEP_AROUND_REF_PREFIX_LEN,
+)
 
 
 def gitlab_special_ref_target(repo, ref_path):
     """Return the changeset for a special ref.
 
     :returns: a :class:`changectx` instance, for the unfiltered version of
        ``repo``. The changeset itself may be obsolete.
@@ -126,15 +130,21 @@
         if ka == sha:
             return True
     return False
 
 
 def keep_around_ref_path(sha):
     # TODO should move to py-heptapod
-    return b'refs/keep-around/' + sha
+    return KEEP_AROUND_REF_PREFIX + sha
+
+
+def parse_keep_around_ref_path(ref):
+    if not ref.startswith(KEEP_AROUND_REF_PREFIX):
+        return None
+    return ref[KEEP_AROUND_REF_PREFIX_LEN:]
 
 
 def iter_keep_arounds_as_refs(repo, deref=True, patterns=None):
     for sha in iter_keep_arounds(repo):
         if sha is GITLAB_TYPED_REFS_MISSING:
             ensure_gitlab_keep_arounds(repo.ui, repo)
             yield from iter_keep_arounds_as_refs(repo, deref=deref)
```

### Comparing `hgitaly-1.4.1/hgitaly/license_detector/__init__.py` & `hgitaly-1.5.0/hgitaly/license_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/license_detector/spdx-licenses.json` & `hgitaly-1.5.0/hgitaly/license_detector/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/linguist/__init__.py` & `hgitaly-1.5.0/hgitaly/linguist/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/linguist/languages.json` & `hgitaly-1.5.0/hgitaly/linguist/languages.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/logging.py` & `hgitaly-1.5.0/hgitaly/logging.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/manifest.py` & `hgitaly-1.5.0/hgitaly/manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/message.py` & `hgitaly-1.5.0/hgitaly/message.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/oid.py` & `hgitaly-1.5.0/hgitaly/oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/pagination.py` & `hgitaly-1.5.0/hgitaly/pagination.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/path.py` & `hgitaly-1.5.0/hgitaly/path.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/peer.py` & `hgitaly-1.5.0/hgitaly/peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/procutil.py` & `hgitaly-1.5.0/hgitaly/procutil.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/repository.py` & `hgitaly-1.5.0/hgitaly/repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/revision.py` & `hgitaly-1.5.0/hgitaly/revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/revset.py` & `hgitaly-1.5.0/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/address.py` & `hgitaly-1.5.0/hgitaly/server/address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/mono.py` & `hgitaly-1.5.0/hgitaly/server/mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/prefork.py` & `hgitaly-1.5.0/hgitaly/server/prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/tests/test_address.py` & `hgitaly-1.5.0/hgitaly/server/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/tests/test_mono.py` & `hgitaly-1.5.0/hgitaly/server/tests/test_mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/tests/test_prefork.py` & `hgitaly-1.5.0/hgitaly/server/tests/test_prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/tests/test_worker.py` & `hgitaly-1.5.0/hgitaly/server/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/server/worker.py` & `hgitaly-1.5.0/hgitaly/server/worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/analysis.py` & `hgitaly-1.5.0/hgitaly/service/analysis.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/blob.py` & `hgitaly-1.5.0/hgitaly/service/blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/commit.py` & `hgitaly-1.5.0/hgitaly/service/commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/diff.py` & `hgitaly-1.5.0/hgitaly/service/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/interceptors.py` & `hgitaly-1.5.0/hgitaly/service/interceptors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/mercurial_changeset.py` & `hgitaly-1.5.0/hgitaly/service/mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/mercurial_operations.py` & `hgitaly-1.5.0/hgitaly/service/mercurial_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/mercurial_repository.py` & `hgitaly-1.5.0/hgitaly/service/mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/operations.py` & `hgitaly-1.5.0/hgitaly/service/operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/ref.py` & `hgitaly-1.5.0/hgitaly/service/ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/repository.py` & `hgitaly-1.5.0/hgitaly/service/repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/server.py` & `hgitaly-1.5.0/hgitaly/service/server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/fixture.py` & `hgitaly-1.5.0/hgitaly/service/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_analysis.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_blob.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_commit.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_default_branch.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_default_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_diff.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_mercurial_changeset.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_mercurial_operations.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_mercurial_repository.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_operations.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_ref.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_repository_service.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_repository_service.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/service/tests/test_server.py` & `hgitaly-1.5.0/hgitaly/service/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/servicer.py` & `hgitaly-1.5.0/hgitaly/servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/ssh.py` & `hgitaly-1.5.0/hgitaly/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stream.py` & `hgitaly-1.5.0/hgitaly/stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/analysis_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/analysis_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/analysis_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/analysis_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/blob_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/blob_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/blob_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/commit_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/commit_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/diff_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/diff_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/diff_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/diff_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/errors_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/lint_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/lint_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/mercurial_changeset_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/mercurial_changeset_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/mercurial_operations_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/mercurial_operations_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/mercurial_repository_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/mercurial_repository_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/operations_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/operations_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/ref_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/ref_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/ref_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/repository_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/repository_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/repository_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/server_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/server_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/server_pb2_grpc.py` & `hgitaly-1.5.0/hgitaly/stub/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/stub/shared_pb2.py` & `hgitaly-1.5.0/hgitaly/stub/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tag.py` & `hgitaly-1.5.0/hgitaly/tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/testing/bundle.py` & `hgitaly-1.5.0/hgitaly/testing/bundle.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/testing/context.py` & `hgitaly-1.5.0/hgitaly/testing/context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/testing/grpc.py` & `hgitaly-1.5.0/hgitaly/testing/grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/testing/ssh.py` & `hgitaly-1.5.0/hgitaly/testing/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/testing/sshd.py` & `hgitaly-1.5.0/hgitaly/testing/sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/testing/tests/test_sshd.py` & `hgitaly-1.5.0/hgitaly/testing/tests/test_sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/common.py` & `hgitaly-1.5.0/hgitaly/tests/common.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_branch.py` & `hgitaly-1.5.0/hgitaly/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_diff.py` & `hgitaly-1.5.0/hgitaly/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_errors.py` & `hgitaly-1.5.0/hgitaly/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_feature.py` & `hgitaly-1.5.0/hgitaly/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_file_context.py` & `hgitaly-1.5.0/hgitaly/tests/test_file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_gitlab_ref.py` & `hgitaly-1.5.0/hgitaly/tests/test_gitlab_ref.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from .common import (
     MINIMAL_HG_CONFIG,
 )
 from ..gitlab_ref import (
     gitlab_special_ref_target,
     iter_gitlab_special_refs_as_refs,
     iter_keep_arounds_as_refs,
+    keep_around_ref_path,
+    parse_keep_around_ref_path,
 )
 
 
 @pytest.fixture
 def repo_wrapper(tmpdir):
     wrapper = LocalRepoWrapper.init(tmpdir, config=MINIMAL_HG_CONFIG)
     yield wrapper.repo, wrapper
@@ -139,7 +141,16 @@
     assert list(iter_keep_arounds_as_refs(repo)) == []
     create_keep_around(repo, sha_bytes)
 
     assert list(iter_keep_arounds_as_refs(repo)) == [
         (b'refs/keep-around/' + sha_bytes, ctx)]
     assert list(iter_keep_arounds_as_refs(repo, deref=False)) == [
         (b'refs/keep-around/' + sha_bytes, sha_str)]
+
+
+def test_parse_keep_around_ref_path():
+    sha = b'12abdc43' * 5
+    ka_ref = b'refs/keep-around/' + sha
+    assert parse_keep_around_ref_path(ka_ref) == sha
+    assert keep_around_ref_path(sha) == ka_ref
+
+    assert parse_keep_around_ref_path(b'refs/pipeline/17') is None
```

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_license_detector.py` & `hgitaly-1.5.0/hgitaly/tests/test_license_detector.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_linguist.py` & `hgitaly-1.5.0/hgitaly/tests/test_linguist.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_manifest.py` & `hgitaly-1.5.0/hgitaly/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_messages.py` & `hgitaly-1.5.0/hgitaly/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_oid.py` & `hgitaly-1.5.0/hgitaly/tests/test_oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_peer.py` & `hgitaly-1.5.0/hgitaly/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_repository.py` & `hgitaly-1.5.0/hgitaly/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_revision.py` & `hgitaly-1.5.0/hgitaly/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_revset.py` & `hgitaly-1.5.0/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_servicer.py` & `hgitaly-1.5.0/hgitaly/tests/test_servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_stream.py` & `hgitaly-1.5.0/hgitaly/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_tag.py` & `hgitaly-1.5.0/hgitaly/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/tests/test_workdir.py` & `hgitaly-1.5.0/hgitaly/tests/test_workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/util.py` & `hgitaly-1.5.0/hgitaly/util.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly/workdir.py` & `hgitaly-1.5.0/hgitaly/workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/hgitaly.egg-info/PKG-INFO` & `hgitaly-1.5.0/hgitaly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 1.4.1
+Version: 1.5.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Requires-Python: >=3.8
```

### Comparing `hgitaly-1.4.1/hgitaly.egg-info/SOURCES.txt` & `hgitaly-1.5.0/hgitaly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/setup.py` & `hgitaly-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/__init__.py` & `hgitaly-1.5.0/tests_with_gitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/comparison.py` & `hgitaly-1.5.0/tests_with_gitaly/comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     STATUS_DETAILS_KEY,
     parse_structured_error,
 )
 from hgitaly import feature
 from hgitaly.errors import HGITALY_ISSUES_URL
 from hgitaly.gitlab_ref import (
     keep_around_ref_path,
+    parse_keep_around_ref_path,
 )
 from hgitaly.stub.shared_pb2 import Repository
 
 try:
     from itertools import batched
 except ImportError:  # Python<3.12
     def batched(it, n):
@@ -317,14 +318,24 @@
         """
         # if hg_sha is None or not 40 bytes long it certainly won't
         # be found in the hg-git mapping, we don't need a special case
         # for that
         git_sha = self.comparison.hg_git.map_git_get(as_bytes(hg_sha))
         return hg_sha if git_sha is None else git_sha
 
+    def normalize_keep_around(self, ref, vcs):
+        if vcs != 'hg':
+            return ref
+
+        hg_sha = parse_keep_around_ref_path(ref)
+        if hg_sha is None:
+            # not a keep-around
+            return ref
+        return keep_around_ref_path(self.hg2git(hg_sha))
+
     def request_kwargs_to_git(self, hg_kwargs):
         git_kwargs = hg_kwargs.copy()
         for sha_attr in self.request_sha_attrs:
             sha = hg_kwargs.get(sha_attr)
             if sha is None:
                 continue
             if isinstance(sha, list):
```

### Comparing `hgitaly-1.4.1/tests_with_gitaly/conftest.py` & `hgitaly-1.5.0/tests_with_gitaly/conftest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/gitaly.py` & `hgitaly-1.5.0/tests_with_gitaly/gitaly.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/hgitaly_rhgitaly_comparison.py` & `hgitaly-1.5.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/rhgitaly.py` & `hgitaly-1.5.0/tests_with_gitaly/rhgitaly.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_blob_tree.py` & `hgitaly-1.5.0/tests_with_gitaly/test_blob_tree.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_commit.py` & `hgitaly-1.5.0/tests_with_gitaly/test_commit.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from hgitaly.stub.commit_pb2 import (
     CommitLanguagesRequest,
     FindCommitRequest,
     FindCommitsRequest,
     LastCommitForPathRequest,
     ListCommitsRequest,
     ListCommitsByOidRequest,
+    ListCommitsByRefNameRequest,
     ListFilesRequest,
     ListLastCommitsForTreeRequest,
     RawBlameRequest,
 )
 from hgitaly.stub.commit_pb2_grpc import CommitServiceStub
 from google.protobuf.timestamp_pb2 import Timestamp
 
@@ -741,14 +742,97 @@
     # a wrong argument does not interfere with correct ones
     rpc_helper.assert_compare(oid=['not-hexadecimal', hexes[0]])
     # NULL_NODE gets ignored
     rpc_helper.assert_compare(oid=[NULL_HEX])
     rpc_helper.assert_compare(oid=[NULL_HEX, hexes[0]])
 
 
+@parametrize('hg_server', ('hgitaly', 'rhgitaly'))
+def test_compare_list_commits_by_ref_name(gitaly_rhgitaly_comparison,
+                                          hg_server):
+    fixture = gitaly_rhgitaly_comparison
+    wrapper = fixture.hg_repo_wrapper
+
+    def normalizer(rpc_helper, responses, vcs=None):
+        for chunk in responses:
+            for commit_ref in chunk.commit_refs:
+                normalize_commit_message(commit_ref.commit)
+                commit_ref.ref_name = rpc_helper.hg2git(  # call w/ direct SHA
+                    rpc_helper.normalize_keep_around(
+                        commit_ref.ref_name, vcs=vcs)
+                )
+
+    rpc_helper = fixture.rpc_helper(
+        hg_server=hg_server,
+        stub_cls=CommitServiceStub,
+        method_name='ListCommitsByRefName',
+        request_cls=ListCommitsByRefNameRequest,
+        streaming=True,
+        response_sha_attrs=[
+            'commit_refs[].commit.id',
+            'commit_refs[].commit.parent_ids[]'
+        ],
+        normalizer=normalizer,
+    )
+
+    def request_kwargs_to_git(hg_kwargs):
+        git_kwargs = hg_kwargs.copy()
+        ref_names = hg_kwargs.get('ref_names')
+        if ref_names is None:
+            return git_kwargs
+        git_kwargs['ref_names'] = [
+            rpc_helper.hg2git(  # for direct SHA
+                rpc_helper.normalize_keep_around(name, vcs='hg')
+            )
+            for name in ref_names
+        ]
+        return git_kwargs
+
+    rpc_helper.request_kwargs_to_git = request_kwargs_to_git
+
+    assert_compare = rpc_helper.assert_compare
+
+    # branches
+    hg_branches = {
+        b'br%02d' % i: wrapper.commit_file('foo', branch='br%02d' % i).hex()
+        for i in range(3)
+    }
+    assert_compare()
+    assert_compare(ref_names=[b'refs/heads/branch/' + branch
+                              for branch in hg_branches.keys()])
+
+    # implicit GitLab branch notation
+    assert_compare(ref_names=[b'branch/br01'])
+
+    # unknown refs are ignored
+    unknown_ref = b'refs/unknown'
+    assert_compare(ref_names=[b'branch/br01', unknown_ref])
+    assert_compare(ref_names=[unknown_ref])
+    assert_compare(ref_names=[unknown_ref, b'refs/heads/branch/br02'])
+
+    # with tags
+    wrapper.command('tag', b'v3.1', rev=b'br01')
+    wrapper.command('gitlab-mirror')
+    fixture.invalidate()
+    assert_compare(ref_names=[b'refs/heads/tags/v3.1'])
+    assert_compare(ref_names=[b'v3.1'])
+
+    # with special refs
+    fixture.write_special_ref(b'pipeline/13', hg_branches[b'br02'])
+    assert_compare(ref_names=[b'refs/heads/pipelines/13'])
+
+    # with a keep-around
+    hg_sha = hg_branches[b'br01']
+    fixture.create_keep_around(hg_sha)
+    rpc_helper.assert_compare(ref_names=[b'refs/keep-around/' + hg_sha])
+
+    # direct SHA
+    rpc_helper.assert_compare(ref_names=[hg_sha])
+
+
 def test_compare_commit_languages(gitaly_comparison):
     fixture = gitaly_comparison
     wrapper = fixture.hg_repo_wrapper
 
     rpc_helper = fixture.rpc_helper(
         stub_cls=CommitServiceStub,
         method_name='CommitLanguages',
```

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_comparison.py` & `hgitaly-1.5.0/tests_with_gitaly/test_comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_diff.py` & `hgitaly-1.5.0/tests_with_gitaly/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_gitaly_server.py` & `hgitaly-1.5.0/tests_with_gitaly/test_gitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_operations.py` & `hgitaly-1.5.0/tests_with_gitaly/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_ref.py` & `hgitaly-1.5.0/tests_with_gitaly/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_repository_service.py` & `hgitaly-1.5.0/tests_with_gitaly/test_repository_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 
 parametrize = pytest.mark.parametrize
 
 TESTS_DATA_DIR = Path(__file__).parent / 'data'
 TIP_TAG_NAME = b'tip'
 
 
-def test_compare_find_merge_base(gitaly_comparison):
-    fixture = gitaly_comparison
+@parametrize('hg_server', ('hgitaly', 'rhgitaly'))
+def test_compare_find_merge_base(gitaly_rhgitaly_comparison, hg_server):
+    fixture = gitaly_rhgitaly_comparison
     gitaly_repo = fixture.gitaly_repo
     git_repo = fixture.git_repo
     wrapper = fixture.hg_repo_wrapper
 
     # repo structure:
     #
     #   o 3 add animal (branch/stable)
@@ -91,17 +92,21 @@
     git_shas[sha3] = git_repo.branches()[b'branch/stable']['sha']
     # commiting a new root, which will test the case when there
     # is no merge_base (gca)
     sha4 = wrapper.commit_file('tut', branch='other',
                                parent=node_mod.nullid).hex()
     git_shas[sha4] = git_repo.branches()[b'branch/other']['sha']
 
+    if hg_server == 'rhgitaly':
+        hgitaly_channel = fixture.rhgitaly_channel
+    else:
+        hgitaly_channel = fixture.hgitaly_channel
     diff_stubs = dict(
         git=RepositoryServiceStub(fixture.gitaly_channel),
-        hg=RepositoryServiceStub(fixture.hgitaly_channel),
+        hg=RepositoryServiceStub(hgitaly_channel),
     )
 
     def do_rpc(vcs, revisions):
         if vcs == 'git':
             revs = [git_shas.get(rev, rev) for rev in revisions]
             revisions = revs
```

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_rhgitaly_server.py` & `hgitaly-1.5.0/tests_with_gitaly/test_rhgitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.4.1/tests_with_gitaly/test_server.py` & `hgitaly-1.5.0/tests_with_gitaly/test_server.py`

 * *Files identical despite different names*


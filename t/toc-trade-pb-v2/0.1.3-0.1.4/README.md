# Comparing `tmp/toc_trade_pb_v2-0.1.3.tar.gz` & `tmp/toc_trade_pb_v2-0.1.4.tar.gz`

## Comparing `toc_trade_pb_v2-0.1.3.tar` & `toc_trade_pb_v2-0.1.4.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/Makefile
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/go.mod
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/go.sum
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/package-lock.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/package.json
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/app/app.proto
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/forwarder/basic.proto
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/forwarder/entity.proto
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/forwarder/history.proto
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/forwarder/mq.proto
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/forwarder/realtime.proto
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/forwarder/subscribe.proto
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/protos/v3/forwarder/trade.proto
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/scripts/gomod_update.sh
--rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/app.pb.go
--rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/basic.pb.go
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/basic_grpc.pb.go
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/entity.pb.go
--rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/history.pb.go
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/history_grpc.pb.go
--rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/mq.pb.go
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/realtime.pb.go
--rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/realtime_grpc.pb.go
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/subscribe.pb.go
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/subscribe_grpc.pb.go
--rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/trade.pb.go
--rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/golang/pb/trade_grpc.pb.go
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/app/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/app/app_pb2.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/app/app_pb2.pyi
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/app/app_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/__init__.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/basic_pb2.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
--rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/entity_pb2.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/history_pb2.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/history_pb2.pyi
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/mq_pb2.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/realtime_pb2.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
--rw-r--r--   0        0        0    20640 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/trade_pb2.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
--rw-r--r--   0        0        0    35674 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
--rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/app/app.ts
--rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/forwarder/basic.ts
--rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/forwarder/entity.ts
--rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/forwarder/history.ts
--rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/forwarder/mq.ts
--rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/forwarder/realtime.ts
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/forwarder/subscribe.ts
--rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/forwarder/trade.ts
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/src/ts/google/protobuf/empty.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/tests/.gitkeep
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/Makefile
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/go.mod
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/go.sum
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/package-lock.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/package.json
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/app/app.proto
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/basic.proto
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/entity.proto
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/history.proto
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/mq.proto
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/realtime.proto
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/subscribe.proto
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/trade.proto
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/scripts/gomod_update.sh
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/scripts/modify_py_import.sh
+-rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/app.pb.go
+-rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/basic.pb.go
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/basic_grpc.pb.go
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/entity.pb.go
+-rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/history.pb.go
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/history_grpc.pb.go
+-rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/mq.pb.go
+-rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/realtime.pb.go
+-rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/realtime_grpc.pb.go
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe.pb.go
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe_grpc.pb.go
+-rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/trade.pb.go
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/trade_grpc.pb.go
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/__init__.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.pyi
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/__init__.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.pyi
+-rw-r--r--   0        0        0     9478 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
+-rw-r--r--   0        0        0    20666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
+-rw-r--r--   0        0        0    35687 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
+-rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/app/app.ts
+-rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/basic.ts
+-rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/entity.ts
+-rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/history.ts
+-rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/mq.ts
+-rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/realtime.ts
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/subscribe.ts
+-rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/trade.ts
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/google/protobuf/empty.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/tests/.gitkeep
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/PKG-INFO
```

### Comparing `toc_trade_pb_v2-0.1.3/Makefile` & `toc_trade_pb_v2-0.1.4/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	@rm -rf src/python/toc_trade_pb && mkdir -p src/python/toc_trade_pb
 	@$(PYTHON) -m grpc_tools.protoc \
 	--grpc_python_out=src/python/toc_trade_pb \
 	--python_out=pyi_out:src/python/toc_trade_pb \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
 
+	@./scripts/modify_py_import.sh
 	@touch src/python/toc_trade_pb/__init__.py
 	@touch src/python/toc_trade_pb/app/__init__.py
 	@touch src/python/toc_trade_pb/forwarder/__init__.py
 
 compile-ts:
 	@rm -rf src/ts && mkdir -p src/ts
 	@protoc \
```

### Comparing `toc_trade_pb_v2-0.1.3/go.sum` & `toc_trade_pb_v2-0.1.4/go.sum`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/package-lock.json` & `toc_trade_pb_v2-0.1.4/package-lock.json`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/package.json` & `toc_trade_pb_v2-0.1.4/package.json`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/.github/workflows/main.yml` & `toc_trade_pb_v2-0.1.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/protos/v3/app/app.proto` & `toc_trade_pb_v2-0.1.4/protos/v3/app/app.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/protos/v3/forwarder/basic.proto` & `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/basic.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/protos/v3/forwarder/history.proto` & `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/history.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/protos/v3/forwarder/mq.proto` & `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/mq.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/protos/v3/forwarder/realtime.proto` & `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/realtime.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/protos/v3/forwarder/subscribe.proto` & `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/subscribe.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/protos/v3/forwarder/trade.proto` & `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/trade.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/app.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/app.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/basic.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/basic.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/basic_grpc.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/basic_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/entity.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/entity.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/history.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/history.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/history_grpc.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/history_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/mq.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/mq.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/realtime.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/realtime.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/realtime_grpc.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/realtime_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/subscribe.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/subscribe_grpc.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/trade.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/trade.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/golang/pb/trade_grpc.pb.go` & `toc_trade_pb_v2-0.1.4/src/golang/pb/trade_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/app/app_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from forwarder import history_pb2 as forwarder_dot_history__pb2
-from forwarder import realtime_pb2 as forwarder_dot_realtime__pb2
-from forwarder import basic_pb2 as forwarder_dot_basic__pb2
-from forwarder import mq_pb2 as forwarder_dot_mq__pb2
+from toc_trade_pb.forwarder import history_pb2 as forwarder_dot_history__pb2
+from toc_trade_pb.forwarder import realtime_pb2 as forwarder_dot_realtime__pb2
+from toc_trade_pb.forwarder import basic_pb2 as forwarder_dot_basic__pb2
+from toc_trade_pb.forwarder import mq_pb2 as forwarder_dot_mq__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rapp/app.proto\x12\x03\x61pp\x1a\x17\x66orwarder/history.proto\x1a\x18\x66orwarder/realtime.proto\x1a\x15\x66orwarder/basic.proto\x1a\x12\x66orwarder/mq.proto\"\x81\x01\n\x0bPickRealMap\x12/\n\x08pick_map\x18\x01 \x03(\x0b\x32\x1d.app.PickRealMap.PickMapEntry\x1a\x41\n\x0cPickMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12 \n\x05value\x18\x02 \x01(\x0e\x32\x11.app.PickListType:\x02\x38\x01\"\x1a\n\nPickFuture\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\x99\x02\n\tWSMessage\x12\x37\n\rfuture_detail\x18\x01 \x01(\x0b\x32\x1e.forwarder.FutureDetailMessageH\x00\x12;\n\x0b\x66uture_tick\x18\x02 \x01(\x0b\x32$.forwarder.FutureRealTimeTickMessageH\x00\x12\x36\n\x0chistory_kbar\x18\x03 \x01(\x0b\x32\x1e.forwarder.HistoryKbarResponseH\x00\x12.\n\x08snapshot\x18\x04 \x01(\x0b\x32\x1a.forwarder.SnapshotMessageH\x00\x12&\n\x0btrade_index\x18\x05 \x01(\x0b\x32\x0f.app.TradeIndexH\x00\x42\x06\n\x04\x64\x61ta\"\x8a\x01\n\nTradeIndex\x12\x1d\n\x03tse\x18\x01 \x01(\x0b\x32\x10.app.IndexStatus\x12\x1d\n\x03otc\x18\x02 \x01(\x0b\x32\x10.app.IndexStatus\x12 \n\x06nasdaq\x18\x03 \x01(\x0b\x32\x10.app.IndexStatus\x12\x1c\n\x02nf\x18\x04 \x01(\x0b\x32\x10.app.IndexStatus\"5\n\x0bIndexStatus\x12\x13\n\x0b\x62reak_count\x18\x01 \x01(\x03\x12\x11\n\tprice_chg\x18\x02 \x01(\x01*-\n\x0cPickListType\x12\x0c\n\x08TYPE_ADD\x10\x00\x12\x0f\n\x0bTYPE_REMOVE\x10\x01\x42\x06Z\x04./pbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'app.app_pb2', _globals)
```

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/app/app_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/app/app_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/basic_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/basic_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
-from forwarder import basic_pb2 as forwarder_dot_basic__pb2
+from toc_trade_pb.forwarder import basic_pb2 as forwarder_dot_basic__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 GRPC_GENERATED_VERSION = '1.63.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
```

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/entity_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/entity_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/history_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/history_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
-from forwarder import history_pb2 as forwarder_dot_history__pb2
+from toc_trade_pb.forwarder import history_pb2 as forwarder_dot_history__pb2
 
 GRPC_GENERATED_VERSION = '1.63.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
```

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/mq_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/mq_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/realtime_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from forwarder import entity_pb2 as forwarder_dot_entity__pb2
+from toc_trade_pb.forwarder import entity_pb2 as forwarder_dot_entity__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x66orwarder/realtime.proto\x12\tforwarder\x1a\x1bgoogle/protobuf/empty.proto\x1a\x16\x66orwarder/entity.proto\"<\n\x10SnapshotResponse\x12(\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1a.forwarder.SnapshotMessage\"0\n\x11YahooFinancePrice\x12\r\n\x05price\x18\x01 \x01(\x01\x12\x0c\n\x04last\x18\x02 \x01(\x01\"0\n\x11VolumeRankRequest\x12\r\n\x05\x63ount\x18\x01 \x01(\x03\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\"\xab\x03\n\x0fSnapshotMessage\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x10\n\x08\x65xchange\x18\x03 \x01(\t\x12\x0c\n\x04open\x18\x04 \x01(\x01\x12\x0c\n\x04high\x18\x05 \x01(\x01\x12\x0b\n\x03low\x18\x06 \x01(\x01\x12\r\n\x05\x63lose\x18\x07 \x01(\x01\x12\x11\n\ttick_type\x18\x08 \x01(\t\x12\x14\n\x0c\x63hange_price\x18\t \x01(\x01\x12\x13\n\x0b\x63hange_rate\x18\n \x01(\x01\x12\x13\n\x0b\x63hange_type\x18\x0b \x01(\t\x12\x15\n\raverage_price\x18\x0c \x01(\x01\x12\x0e\n\x06volume\x18\r \x01(\x03\x12\x14\n\x0ctotal_volume\x18\x0e \x01(\x03\x12\x0e\n\x06\x61mount\x18\x0f \x01(\x03\x12\x14\n\x0ctotal_amount\x18\x10 \x01(\x03\x12\x18\n\x10yesterday_volume\x18\x11 \x01(\x01\x12\x11\n\tbuy_price\x18\x12 \x01(\x01\x12\x12\n\nbuy_volume\x18\x13 \x01(\x01\x12\x12\n\nsell_price\x18\x14 \x01(\x01\x12\x13\n\x0bsell_volume\x18\x15 \x01(\x03\x12\x14\n\x0cvolume_ratio\x18\x16 \x01(\x01\"J\n\x17StockVolumeRankResponse\x12/\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32!.forwarder.StockVolumeRankMessage\"\x8e\x04\n\x16StockVolumeRankMessage\x12\x0c\n\x04\x64\x61te\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02ts\x18\x04 \x01(\x03\x12\x0c\n\x04open\x18\x05 \x01(\x01\x12\x0c\n\x04high\x18\x06 \x01(\x01\x12\x0b\n\x03low\x18\x07 \x01(\x01\x12\r\n\x05\x63lose\x18\x08 \x01(\x01\x12\x13\n\x0bprice_range\x18\t \x01(\x01\x12\x11\n\ttick_type\x18\n \x01(\x03\x12\x14\n\x0c\x63hange_price\x18\x0b \x01(\x01\x12\x13\n\x0b\x63hange_type\x18\x0c \x01(\x03\x12\x15\n\raverage_price\x18\r \x01(\x01\x12\x0e\n\x06volume\x18\x0e \x01(\x03\x12\x14\n\x0ctotal_volume\x18\x0f \x01(\x03\x12\x0e\n\x06\x61mount\x18\x10 \x01(\x03\x12\x14\n\x0ctotal_amount\x18\x11 \x01(\x03\x12\x18\n\x10yesterday_volume\x18\x12 \x01(\x03\x12\x14\n\x0cvolume_ratio\x18\x13 \x01(\x01\x12\x11\n\tbuy_price\x18\x14 \x01(\x01\x12\x12\n\nbuy_volume\x18\x15 \x01(\x03\x12\x12\n\nsell_price\x18\x16 \x01(\x01\x12\x13\n\x0bsell_volume\x18\x17 \x01(\x03\x12\x12\n\nbid_orders\x18\x18 \x01(\x03\x12\x13\n\x0b\x62id_volumes\x18\x19 \x01(\x03\x12\x12\n\nask_orders\x18\x1a \x01(\x03\x12\x13\n\x0b\x61sk_volumes\x18\x1b \x01(\x03\x32\x95\x05\n\x15RealTimeDataInterface\x12L\n\x13GetAllStockSnapshot\x12\x16.google.protobuf.Empty\x1a\x1b.forwarder.SnapshotResponse\"\x00\x12Q\n\x18GetStockSnapshotByNumArr\x12\x16.forwarder.StockNumArr\x1a\x1b.forwarder.SnapshotResponse\"\x00\x12L\n\x13GetStockSnapshotTSE\x12\x16.google.protobuf.Empty\x1a\x1b.forwarder.SnapshotResponse\"\x00\x12L\n\x13GetStockSnapshotOTC\x12\x16.google.protobuf.Empty\x1a\x1b.forwarder.SnapshotResponse\"\x00\x12\x43\n\tGetNasdaq\x12\x16.google.protobuf.Empty\x1a\x1c.forwarder.YahooFinancePrice\"\x00\x12I\n\x0fGetNasdaqFuture\x12\x16.google.protobuf.Empty\x1a\x1c.forwarder.YahooFinancePrice\"\x00\x12X\n\x12GetStockVolumeRank\x12\x1c.forwarder.VolumeRankRequest\x1a\".forwarder.StockVolumeRankResponse\"\x00\x12U\n\x1aGetFutureSnapshotByCodeArr\x12\x18.forwarder.FutureCodeArr\x1a\x1b.forwarder.SnapshotResponse\"\x00\x42\x06Z\x04./pbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'forwarder.realtime_pb2', _globals)
```

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
-from forwarder import entity_pb2 as forwarder_dot_entity__pb2
-from forwarder import realtime_pb2 as forwarder_dot_realtime__pb2
+from toc_trade_pb.forwarder import entity_pb2 as forwarder_dot_entity__pb2
+from toc_trade_pb.forwarder import realtime_pb2 as forwarder_dot_realtime__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 GRPC_GENERATED_VERSION = '1.63.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
```

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from forwarder import entity_pb2 as forwarder_dot_entity__pb2
+from toc_trade_pb.forwarder import entity_pb2 as forwarder_dot_entity__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66orwarder/subscribe.proto\x12\tforwarder\x1a\x1bgoogle/protobuf/empty.proto\x1a\x16\x66orwarder/entity.proto\"%\n\x11SubscribeResponse\x12\x10\n\x08\x66\x61il_arr\x18\x01 \x03(\t2\xb8\x06\n\x16SubscribeDataInterface\x12L\n\x12SubscribeStockTick\x12\x16.forwarder.StockNumArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12N\n\x14UnSubscribeStockTick\x12\x16.forwarder.StockNumArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12N\n\x14SubscribeStockBidAsk\x12\x16.forwarder.StockNumArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12P\n\x16UnSubscribeStockBidAsk\x12\x16.forwarder.StockNumArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12O\n\x13SubscribeFutureTick\x12\x18.forwarder.FutureCodeArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12Q\n\x15UnSubscribeFutureTick\x12\x18.forwarder.FutureCodeArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12Q\n\x15SubscribeFutureBidAsk\x12\x18.forwarder.FutureCodeArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12S\n\x17UnSubscribeFutureBidAsk\x12\x18.forwarder.FutureCodeArr\x1a\x1c.forwarder.SubscribeResponse\"\x00\x12G\n\x12UnSubscribeAllTick\x12\x16.google.protobuf.Empty\x1a\x17.forwarder.ErrorMessage\"\x00\x12I\n\x14UnSubscribeAllBidAsk\x12\x16.google.protobuf.Empty\x1a\x17.forwarder.ErrorMessage\"\x00\x42\x06Z\x04./pbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'forwarder.subscribe_pb2', _globals)
```

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
-from forwarder import entity_pb2 as forwarder_dot_entity__pb2
-from forwarder import subscribe_pb2 as forwarder_dot_subscribe__pb2
+from toc_trade_pb.forwarder import entity_pb2 as forwarder_dot_entity__pb2
+from toc_trade_pb.forwarder import subscribe_pb2 as forwarder_dot_subscribe__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 GRPC_GENERATED_VERSION = '1.63.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
```

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/trade_pb2.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/trade_pb2.pyi` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py` & `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
-from forwarder import trade_pb2 as forwarder_dot_trade__pb2
+from toc_trade_pb.forwarder import trade_pb2 as forwarder_dot_trade__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 GRPC_GENERATED_VERSION = '1.63.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
```

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/app/app.ts` & `toc_trade_pb_v2-0.1.4/src/ts/app/app.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/forwarder/basic.ts` & `toc_trade_pb_v2-0.1.4/src/ts/forwarder/basic.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/forwarder/entity.ts` & `toc_trade_pb_v2-0.1.4/src/ts/forwarder/entity.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/forwarder/history.ts` & `toc_trade_pb_v2-0.1.4/src/ts/forwarder/history.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/forwarder/mq.ts` & `toc_trade_pb_v2-0.1.4/src/ts/forwarder/mq.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/forwarder/realtime.ts` & `toc_trade_pb_v2-0.1.4/src/ts/forwarder/realtime.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/forwarder/subscribe.ts` & `toc_trade_pb_v2-0.1.4/src/ts/forwarder/subscribe.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/forwarder/trade.ts` & `toc_trade_pb_v2-0.1.4/src/ts/forwarder/trade.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/src/ts/google/protobuf/empty.ts` & `toc_trade_pb_v2-0.1.4/src/ts/google/protobuf/empty.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/LICENSE` & `toc_trade_pb_v2-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.3/pyproject.toml` & `toc_trade_pb_v2-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toc-trade-pb-v2"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Tim Hsu", email = "maochindada@gmail.com" }]
 description = "Pre-compiled Python protobuf files for ToC Trade"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `toc_trade_pb_v2-0.1.3/PKG-INFO` & `toc_trade_pb_v2-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: toc-trade-pb-v2
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pre-compiled Python protobuf files for ToC Trade
 Project-URL: Homepage, https://github.com/ToC-Taiwan/toc-trade-protobuf
 Project-URL: Issues, https://github.com/ToC-Taiwan/toc-trade-protobuf/issues
 Author-email: Tim Hsu <maochindada@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


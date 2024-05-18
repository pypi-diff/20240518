# Comparing `tmp/hexdoc_hexdebug-0.1.0.1.20.1.1.0.tar.gz` & `tmp/hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0.tar.gz`

## Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0.tar` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/gradle.properties
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/__version__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/__init__.py
--rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.patterns.hexdoc.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/empty.json
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/full.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/empty.json
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/full.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/empty.json
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/full.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/empty.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/full.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/empty.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/full.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/empty.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/full.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/empty.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/full.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/empty.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/full.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/empty.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/full.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/empty.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/full.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/empty.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/full.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/empty.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/full.json
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/debug_state/debugging.png
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/debugger.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_templates/__init__.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/LICENSE
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/gradle.properties
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/__gradle_version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/__version__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/py.typed
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/__init__.py
+-rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.patterns.hexdoc.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/empty.json
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/full.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/empty.json
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/full.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/empty.json
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/full.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/empty.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/full.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/empty.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/full.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/empty.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/full.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/empty.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/full.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/empty.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/full.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/empty.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/full.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/empty.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/full.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/empty.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/full.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/empty.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/full.json
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/debug_state/debugging.png
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/debugger.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_templates/__init__.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/LICENSE
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/README.md
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/PKG-INFO
```

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6613541666666667%*

 * *Differences: {"'asset_url'": "'https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939'",*

 * * "'book_url'": "'https://hexdebug.hexxy.media/v/0.1.0+1.20.1/1.0.dev0/en_us'",*

 * * "'textures'": "{'PNGTexture': {'hexdebug:textures/item/debugger.png': {'url': "*

 * *               "'https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png'}, "*

 * *               "'hexdebug:textures/item/debu […]*

```diff
@@ -1,78 +1,78 @@
 {
-    "asset_url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d",
-    "book_url": "https://hexdebug.hexxy.media/v/0.1.0+1.20.1/1.0/en_us",
+    "asset_url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939",
+    "book_url": "https://hexdebug.hexxy.media/v/0.1.0+1.20.1/1.0.dev0/en_us",
     "textures": {
         "PNGTexture": {
             "hexdebug:textures/item/debugger.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
             },
             "hexdebug:textures/item/debugger/debug_state/debugging.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/debug_state/debugging.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/debug_state/debugging.png"
             },
             "hexdebug:textures/item/debugger/has_hex/full.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/has_hex/full.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/has_hex/full.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/continue.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/in.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/out.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/over.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/restart.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/stop.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/continue.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/in.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/out.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/over.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/restart.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/stop.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png"
             }
         },
         "SingleItemTexture": {
             "hexdebug:debugger": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/378f07837cdea85e90634cad5ce079473fd9222d/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/06e734a958cb5d3af672a0284e58fde8c8e52939/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
                 }
             },
             "hexdebug:debugger/debugging/continue/empty": {
                 "inner": {
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
                 }
```

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/.gitignore` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/LICENSE` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/pyproject.toml` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/doc/README.md` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.20.1.1.0/PKG-INFO` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hexdoc-hexdebug
-Version: 0.1.0.1.20.1.1.0
+Version: 0.1.0.1.20.1.1.0.dev0
 Summary: Python web book docgen and hexdoc plugin for HexDebug.
 Project-URL: Homepage, https://hexdebug.hexxy.media
 Project-URL: Source, https://github.com/object-Object/HexDebug
 Author: object-Object
 License-File: LICENSE
 Keywords: hexdoc
 Requires-Python: >=3.11
```


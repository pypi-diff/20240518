# Comparing `tmp/hexdoc_hexdebug-0.1.0.1.0.dev0.tar.gz` & `tmp/hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0.tar.gz`

## Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0.tar` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0.tar`

### file list

```diff
@@ -1,38 +1,64 @@
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/gradle.properties
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/__version__.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/__init__.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.patterns.hexdoc.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/continue/active.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/continue/inactive.json
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/continue/waiting_for_client.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/in/active.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/in/inactive.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/in/waiting_for_client.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/over/active.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/over/inactive.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/over/waiting_for_client.json
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger.png
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/state/active.png
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/state/waiting_for_client.png
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/continue.png
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/in.png
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/out.png
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/over.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_templates/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/doc/README.md
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.0.1.0.dev0/PKG-INFO
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

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_hooks.py` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_hooks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from importlib.resources import Package
-from typing_extensions import override
 
 from hexdoc.plugin import (
     HookReturn,
     ModPlugin,
     ModPluginImpl,
     ModPluginWithBook,
     hookimpl,
 )
+from typing_extensions import override
 
 import hexdoc_hexdebug
 
-from .__gradle_version__ import FULL_VERSION, GRADLE_VERSION
+from .__gradle_version__ import FULL_VERSION, MINECRAFT_VERSION, MOD_VERSION
 from .__version__ import PY_VERSION
 
 
 class HexDebugPlugin(ModPluginImpl):
     @staticmethod
     @hookimpl
     def hexdoc_mod_plugin(branch: str) -> ModPlugin:
@@ -32,26 +32,26 @@
     @override
     def full_version(self) -> str:
         return FULL_VERSION
 
     @property
     @override
     def mod_version(self) -> str:
-        return GRADLE_VERSION
+        return f"{MOD_VERSION}+{MINECRAFT_VERSION}"
 
     @property
     @override
     def plugin_version(self) -> str:
         return PY_VERSION
 
     @override
     def resource_dirs(self) -> HookReturn[Package]:
         # lazy import because generated may not exist when this file is loaded
         # eg. when generating the contents of generated
         # so we only want to import it if we actually need it
         from ._export import generated
 
         return generated
-    
+
     @override
     def jinja_template_root(self) -> tuple[Package, str]:
         return hexdoc_hexdebug, "_templates"
```

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5`

 * *Files 6% similar despite different names*

```diff
@@ -19,9 +19,16 @@
     },
     {
       type: "hexcasting:pattern",
       op_id: "hexdebug:breakpoint/after",
       anchor: "hexdebug:breakpoint/after",
       text: "hexdebug.category.patterns.entry.debugging.page.breakpoint/after",
     },
+    {
+      type: "hexcasting:pattern",
+      op_id: "hexdebug:craft/debugger",
+      anchor: "hexdebug:craft/debugger",
+      input: "entity, [pattern]",
+      text: "hexdebug.category.patterns.entry.debugging.page.craft/debugger",
+    }
   ],
 }
```

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/state/active.png` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png`

 * *Files 20% similar despite different names*

#### sng

```diff
@@ -2,49 +2,49 @@
 IHDR {
     width: 16; height: 16; bitdepth: 8;
     using color alpha;
 }
 iCCP {
     name: "ICC profile"
     profile: hex
-000002a0 6c636d73 04400000 6d6e7472 52474220 58595a20 07e80004 001b0013 0008000a 61637370 4d534654 00000000 00000000 00000000 00000000 00000000 00000000 0000f6d6 00010000 0000d32d 6c636d73 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 0000000d 64657363 00000120 00000040 63707274 00000160 00000036 77747074 00000198 00000014 63686164 000001ac 0000002c 7258595a 000001d8 00000014 6258595a 000001ec 00000014 6758595a 00000200 00000014 72545243 00000214 00000020 67545243 00000214 00000020 62545243 00000214 00000020 6368726d 00000234 00000024 646d6e64 00000258 00000024 646d6464 0000027c 00000024 6d6c7563 00000000 00000001 0000000c 656e5553 00000024 0000001c 00470049 004d0050 00200062 00750069 006c0074 002d0069 006e0020 00730052 00470042 6d6c7563 00000000 00000001 0000000c 656e5553 0000001a 0000001c 00500075 0062006c 00690063 00200044 006f006d 00610069 006e0000 58595a20 00000000 0000f6d6 00010000 0000d32d 73663332 00000000 00010c42 000005de fffff325 00000793 0000fd90 fffffba1 fffffda2 000003dc 0000c06e 58595a20 00000000 00006fa0 000038f5 00000390 58595a20 00000000 0000249f 00000f84 0000b6c4 58595a20 00000000 00006297 0000b787 000018d9 70617261 00000000 00030000 00026666 0000f2a7 00000d59 000013d0 00000a5b 6368726d 00000000 00030000 0000a3d7 0000547c 00004ccd 0000999a 00002667 00000f5c 6d6c7563 00000000 00000001 0000000c 656e5553 00000008 0000001c 00470049 004d0050 6d6c7563 00000000 00000001 0000000c 656e5553 00000008 0000001c 00730052 00470042 ;
+000002a0 6c636d73 04400000 6d6e7472 52474220 58595a20 07e80005 000c0012 00210021 61637370 4d534654 00000000 00000000 00000000 00000000 00000000 00000000 0000f6d6 00010000 0000d32d 6c636d73 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 0000000d 64657363 00000120 00000040 63707274 00000160 00000036 77747074 00000198 00000014 63686164 000001ac 0000002c 7258595a 000001d8 00000014 6258595a 000001ec 00000014 6758595a 00000200 00000014 72545243 00000214 00000020 67545243 00000214 00000020 62545243 00000214 00000020 6368726d 00000234 00000024 646d6e64 00000258 00000024 646d6464 0000027c 00000024 6d6c7563 00000000 00000001 0000000c 656e5553 00000024 0000001c 00470049 004d0050 00200062 00750069 006c0074 002d0069 006e0020 00730052 00470042 6d6c7563 00000000 00000001 0000000c 656e5553 0000001a 0000001c 00500075 0062006c 00690063 00200044 006f006d 00610069 006e0000 58595a20 00000000 0000f6d6 00010000 0000d32d 73663332 00000000 00010c42 000005de fffff325 00000793 0000fd90 fffffba1 fffffda2 000003dc 0000c06e 58595a20 00000000 00006fa0 000038f5 00000390 58595a20 00000000 0000249f 00000f84 0000b6c4 58595a20 00000000 00006297 0000b787 000018d9 70617261 00000000 00030000 00026666 0000f2a7 00000d59 000013d0 00000a5b 6368726d 00000000 00030000 0000a3d7 0000547c 00004ccd 0000999a 00002667 00000f5c 6d6c7563 00000000 00000001 0000000c 656e5553 00000008 0000001c 00470049 004d0050 6d6c7563 00000000 00000001 0000000c 656e5553 00000008 0000001c 00730052 00470042 ;
 }
 bKGD {red: 255;  green: 255;  blue: 255;}
 pHYs {xpixels: 2835; ypixels: 2835; per: meter;}  # (72 dpi)
 tIME {
-    # 27 Apr 2024 19:18:10 GMT
+    # 12 May 2024 18:33:47 GMT
     year:   2024
-    month:  4
-    day:    27
-    hour:   19
-    minute: 18
-    second: 10
+    month:  5
+    day:    12
+    hour:   18
+    minute: 33
+    second: 47
 }
 zTXt {
     keyword: "Raw profile type exif";
-    text: "\nexif\n     214\n45786966000049492a00080000000a000001040001000000100000000101040001000000\n100000000201030003000000860000001201030001000000010000001a01050001000000\n8c0000001b0105000100000094000000280103000100000003000000310102000d000000\n9c0000003201020014000000aa0000006987040001000000be0000000000000008000800\n08003702000014000000370200001400000047494d5020322e31302e3334000032303234\n3a30343a32372031353a31383a313000010001a00300010000000100000000000000\n";
+    text: "\nexif\n     214\n45786966000049492a00080000000a000001040001000000100000000101040001000000\n100000000201030003000000860000001201030001000000010000001a01050001000000\n8c0000001b0105000100000094000000280103000100000003000000310102000d000000\n9c0000003201020014000000aa0000006987040001000000be0000000000000008000800\n08003702000014000000370200001400000047494d5020322e31302e3334000032303234\n3a30353a31322031343a33333a343700010001a00300010000000100000000000000\n";
 }
 iTXt {
     language: "";
     keyword: "XML:com.adobe.xmp";
     translated: "";
-    text: "<?xpacket begin=\"\xef\xbb\xbf\" id=\"W5M0MpCehiHzreSzNTczkc9d\"?>\n<x:xmpmeta xmlns:x=\"adobe:ns:meta/\" x:xmptk=\"XMP Core 4.4.0-Exiv2\">\n <rdf:RDF xmlns:rdf=\"http://www.w3.org/1999/02/22-rdf-syntax-ns#\">\n  <rdf:Description rdf:about=\"\"\n    xmlns:xmpMM=\"http://ns.adobe.com/xap/1.0/mm/\"\n    xmlns:stEvt=\"http://ns.adobe.com/xap/1.0/sType/ResourceEvent#\"\n    xmlns:dc=\"http://purl.org/dc/elements/1.1/\"\n    xmlns:GIMP=\"http://www.gimp.org/xmp/\"\n    xmlns:tiff=\"http://ns.adobe.com/tiff/1.0/\"\n    xmlns:xmp=\"http://ns.adobe.com/xap/1.0/\"\n   xmpMM:DocumentID=\"gimp:docid:gimp:c40b31e4-41d2-4e79-a781-be0923c46689\"\n   xmpMM:InstanceID=\"xmp.iid:01f960e2-80e6-47c9-8acd-815502c8316e\"\n   xmpMM:OriginalDocumentID=\"xmp.did:9700cc4d-1e46-4bfb-a171-0935721ffb9c\"\n   dc:Format=\"image/png\"\n   GIMP:API=\"2.0\"\n   GIMP:Platform=\"Windows\"\n   GIMP:TimeStamp=\"1714245490908221\"\n   GIMP:Version=\"2.10.34\"\n   tiff:Orientation=\"1\"\n   xmp:CreatorTool=\"GIMP 2.10\"\n   xmp:MetadataDate=\"2024:04:27T15:18:10-04:00\"\n   xmp:ModifyDate=\"2024:04:27T15:18:10-04:00\">\n   <xmpMM:History>\n    <rdf:Seq>\n     <rdf:li\n      stEvt:action=\"saved\"\n      stEvt:changed=\"/\"\n      stEvt:instanceID=\"xmp.iid:25b7c3cd-09b8-4b71-930c-74bafd1a8c5e\"\n      stEvt:softwareAgent=\"Gimp 2.10 (Windows)\"\n      stEvt:when=\"2024-04-27T01:08:31\"/>\n     <rdf:li\n      stEvt:action=\"saved\"\n      stEvt:changed=\"/\"\n      stEvt:instanceID=\"xmp.iid:31a61e1d-3f3a-4bc4-8fb7-65eb7d9c1fef\"\n      stEvt:softwareAgent=\"Gimp 2.10 (Windows)\"\n      stEvt:when=\"2024-04-27T15:18:10\"/>\n    </rdf:Seq>\n   </xmpMM:History>\n  </rdf:Description>\n </rdf:RDF>\n</x:xmpmeta>\n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                           \n<?xpacket end=\"w\"?>";
+    text: "<?xpacket begin=\"\xef\xbb\xbf\" id=\"W5M0MpCehiHzreSzNTczkc9d\"?>\n<x:xmpmeta xmlns:x=\"adobe:ns:meta/\" x:xmptk=\"XMP Core 4.4.0-Exiv2\">\n <rdf:RDF xmlns:rdf=\"http://www.w3.org/1999/02/22-rdf-syntax-ns#\">\n  <rdf:Description rdf:about=\"\"\n    xmlns:xmpMM=\"http://ns.adobe.com/xap/1.0/mm/\"\n    xmlns:stEvt=\"http://ns.adobe.com/xap/1.0/sType/ResourceEvent#\"\n    xmlns:dc=\"http://purl.org/dc/elements/1.1/\"\n    xmlns:GIMP=\"http://www.gimp.org/xmp/\"\n    xmlns:tiff=\"http://ns.adobe.com/tiff/1.0/\"\n    xmlns:xmp=\"http://ns.adobe.com/xap/1.0/\"\n   xmpMM:DocumentID=\"gimp:docid:gimp:c40b31e4-41d2-4e79-a781-be0923c46689\"\n   xmpMM:InstanceID=\"xmp.iid:a751420e-1f93-4565-8a15-dec3e098e3f5\"\n   xmpMM:OriginalDocumentID=\"xmp.did:9700cc4d-1e46-4bfb-a171-0935721ffb9c\"\n   dc:Format=\"image/png\"\n   GIMP:API=\"2.0\"\n   GIMP:Platform=\"Windows\"\n   GIMP:TimeStamp=\"1715538827509302\"\n   GIMP:Version=\"2.10.34\"\n   tiff:Orientation=\"1\"\n   xmp:CreatorTool=\"GIMP 2.10\"\n   xmp:MetadataDate=\"2024:05:12T14:33:47-04:00\"\n   xmp:ModifyDate=\"2024:05:12T14:33:47-04:00\">\n   <xmpMM:History>\n    <rdf:Seq>\n     <rdf:li\n      stEvt:action=\"saved\"\n      stEvt:changed=\"/\"\n      stEvt:instanceID=\"xmp.iid:25b7c3cd-09b8-4b71-930c-74bafd1a8c5e\"\n      stEvt:softwareAgent=\"Gimp 2.10 (Windows)\"\n      stEvt:when=\"2024-04-27T01:08:31\"/>\n     <rdf:li\n      stEvt:action=\"saved\"\n      stEvt:changed=\"/\"\n      stEvt:instanceID=\"xmp.iid:31a61e1d-3f3a-4bc4-8fb7-65eb7d9c1fef\"\n      stEvt:softwareAgent=\"Gimp 2.10 (Windows)\"\n      stEvt:when=\"2024-04-27T15:18:10\"/>\n     <rdf:li\n      stEvt:action=\"saved\"\n      stEvt:changed=\"/\"\n      stEvt:instanceID=\"xmp.iid:7b730593-b526-40c8-b636-5cca7b29c7d2\"\n      stEvt:softwareAgent=\"Gimp 2.10 (Windows)\"\n      stEvt:when=\"2024-05-12T14:33:47\"/>\n    </rdf:Seq>\n   </xmpMM:History>\n  </rdf:Description>\n </rdf:RDF>\n</x:xmpmeta>\n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                                                                                                    \n                           \n<?xpacket end=\"w\"?>";
 }
 IMAGE {
     pixels hex
-00000000 00000000 00000000 fad64aff 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
-00000000 00000000 00000000 fdf55fff 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
-00000000 00000000 fad64aff fdf55fff fad64aff 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
-fad64aff fdf55fff fdf55fff fffde0ff fdf55fff fdf55fff fad64aff 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
-00000000 00000000 fad64aff fdf55fff fad64aff 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
-00000000 00000000 00000000 fdf55fff 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
-00000000 00000000 00000000 fad64aff 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 
+00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 fad64aff 00000000 00000000 00000000 
+00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 fdf55fff 00000000 00000000 00000000 
+00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 fad64aff fdf55fff fad64aff 00000000 00000000 
+00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 fad64aff fdf55fff fdf55fff fffde0ff fdf55fff fdf55fff fad64aff 
+00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 fad64aff fdf55fff fad64aff 00000000 00000000 
+00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 fdf55fff 00000000 00000000 00000000 
+00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000000 fad64aff 00000000 00000000 00000000 
 }
```

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/.gitignore` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 build/
 *.ipr
 run/
 *.iws
-out/
+/out/
 *.iml
 .gradle/
 output/
 bin/
 
 .classpath
 .project
```

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/LICENSE` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/pyproject.toml` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
 requires = [
     "hatchling",
-    "hatch-gradle-version>=0.9.6",
+    "hatch-gradle-version>=0.9.8",
 ]
 build-backend = "hatchling.build"
 
 # project metadata
 
 [project]
 name = "hexdoc-hexdebug"
@@ -25,18 +25,19 @@
 # Gradle version/deps
 
 [tool.hatch.version]
 scheme = "gradle"
 source = "gradle-properties"
 py-path = "doc/src/hexdoc_hexdebug/__version__.py"
 key = "modVersion"
+gradle-version-regex = { regex='^(.+?)(-.+)?$', repl='\1.{minecraftVersion}\2' }
 
 [tool.hatch.metadata.hooks.version-catalog]
 dependencies = [
-    "hexdoc>=1!0.1.0a13",
+    "hexdoc>=1!0.1.0a16",
     { package="hexdoc-hexcasting", op="~=", py-version="1.0", key="hexcasting" },
 ]
 
 [tool.hatch.metadata.hooks.version-catalog.optional-dependencies]
 dev = [
     "ruff~=0.3.7",
 ]
```

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/doc/README.md` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.0.1.0.dev0/PKG-INFO` & `hexdoc_hexdebug-0.1.0.1.20.1.1.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: hexdoc-hexdebug
-Version: 0.1.0.1.0.dev0
+Version: 0.1.0.1.20.1.1.0.dev0
 Summary: Python web book docgen and hexdoc plugin for HexDebug.
 Project-URL: Homepage, https://hexdebug.hexxy.media
 Project-URL: Source, https://github.com/object-Object/HexDebug
 Author: object-Object
 License-File: LICENSE
 Keywords: hexdoc
 Requires-Python: >=3.11
 Requires-Dist: hexdoc-hexcasting~=0.11.1.1.0rc7
-Requires-Dist: hexdoc>=1!0.1.0a13
+Requires-Dist: hexdoc>=1!0.1.0a16
 Provides-Extra: dev
 Requires-Dist: ruff~=0.3.7; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # hexdoc-hexdebug
 
 Python web book docgen and [hexdoc](https://pypi.org/project/hexdoc) plugin for HexDebug.
```


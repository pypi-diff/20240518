# Comparing `tmp/yambs-3.0.1.tar.gz` & `tmp/yambs-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-3.0.1.tar", last modified: Fri Mar 15 02:48:19 2024, max compression
+gzip compressed data, was "yambs-3.0.2.tar", last modified: Sat May 18 07:35:04 2024, max compression
```

## Comparing `yambs-3.0.1.tar` & `yambs-3.0.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.280334 yambs-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-15 02:46:06.000000 yambs-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-03-15 02:48:19.280334 yambs-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-03-15 02:46:06.000000 yambs-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-15 02:46:06.000000 yambs-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 02:48:19.280334 yambs-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-15 02:46:06.000000 yambs-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.264334 yambs-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-15 02:46:06.000000 yambs-3.0.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-15 02:46:06.000000 yambs-3.0.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.264334 yambs-3.0.1/yambs/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.268334 yambs-3.0.1/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.268334 yambs-3.0.1/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/compile_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.268334 yambs-3.0.1/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.268334 yambs-3.0.1/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.268334 yambs-3.0.1/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/includes/wasm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.272334 yambs-3.0.1/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Dependency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Github.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.276334 yambs-3.0.1/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/regenerate.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/data/yambs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.276334 yambs-3.0.1/yambs/dependency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.276334 yambs-3.0.1/yambs/dependency/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/handlers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.276334 yambs-3.0.1/yambs/dependency/handlers/yambs/
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/handlers/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/handlers/yambs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/handlers/yambs/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dependency/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.276334 yambs-3.0.1/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.276334 yambs-3.0.1/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.276334 yambs-3.0.1/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.280334 yambs-3.0.1/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/generate/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.280334 yambs-3.0.1/yambs/github/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.280334 yambs-3.0.1/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.280334 yambs-3.0.1/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-03-15 02:46:06.000000 yambs-3.0.1/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:48:19.280334 yambs-3.0.1/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-03-15 02:48:19.000000 yambs-3.0.1/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-15 02:48:19.000000 yambs-3.0.1/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 02:48:19.000000 yambs-3.0.1/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-15 02:48:19.000000 yambs-3.0.1/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-15 02:48:19.000000 yambs-3.0.1/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 02:48:19.000000 yambs-3.0.1/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-18 07:32:49.000000 yambs-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-18 07:35:04.015226 yambs-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-18 07:32:49.000000 yambs-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-18 07:32:49.000000 yambs-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 07:35:04.015226 yambs-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-18 07:32:49.000000 yambs-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.003225 yambs-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-18 07:32:49.000000 yambs-3.0.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-18 07:32:49.000000 yambs-3.0.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.003225 yambs-3.0.2/yambs/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.003225 yambs-3.0.2/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/compile_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/wasm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Dependency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Github.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/regenerate.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/yambs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dependency/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dependency/handlers/yambs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/yambs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/yambs/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/top_level.txt
```

### Comparing `yambs-3.0.1/LICENSE` & `yambs-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/PKG-INFO` & `yambs-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 3.0.1
+Version: 3.0.2
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -14,17 +14,17 @@
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rcmpy>=1.5.0
-Requires-Dist: datazen
 Requires-Dist: requests
 Requires-Dist: vcorelib>=2.4.2
+Requires-Dist: datazen
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -37,19 +37,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=454db224964265a8f876fd45d5428729
+    hash=72271a00d30bf23159c35289b5ff7a00
     =====================================
 -->
 
-# yambs ([3.0.1](https://pypi.org/project/yambs/))
+# yambs ([3.0.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -166,15 +166,15 @@
 
 1. Sane out-of-the-box conventions: put your code here (and organize it by
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/mbs -h
+$ ./venv3.12/bin/mbs -h
 
 usage: mbs [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
            {compile_config,dist,download,gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
@@ -200,15 +200,15 @@
 ```
 
 ## Sub-command Options
 
 ### `compile_config`
 
 ```
-$ ./venv3.11/bin/mbs compile_config -h
+$ ./venv3.12/bin/mbs compile_config -h
 
 usage: mbs compile_config [-h] [-i INCLUDES_KEY] [-u] [-e]
                           output inputs [inputs ...]
 
 positional arguments:
   output                file to write
   inputs                files to read
@@ -225,15 +225,15 @@
                         loaded
 
 ```
 
 ### `dist`
 
 ```
-$ ./venv3.11/bin/mbs dist -h
+$ ./venv3.12/bin/mbs dist -h
 
 usage: mbs dist [-h] [-c CONFIG] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -241,15 +241,15 @@
   -s, --sources         set this flag to only capture source files
 
 ```
 
 ### `download`
 
 ```
-$ ./venv3.11/bin/mbs download -h
+$ ./venv3.12/bin/mbs download -h
 
 usage: mbs download [-h] [-o OWNER] [-r REPO] [-O OUTPUT] [-p PATTERN]
 
 options:
   -h, --help            show this help message and exit
   -o OWNER, --owner OWNER
                         repository owner (default: 'vkottler')
@@ -261,15 +261,15 @@
                         filtered by name
 
 ```
 
 ### `gen`
 
 ```
-$ ./venv3.11/bin/mbs gen -h
+$ ./venv3.12/bin/mbs gen -h
 
 usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s] [-n]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -281,15 +281,15 @@
   -n, --no-build        whether or not to skip running 'ninja'
 
 ```
 
 ### `native`
 
 ```
-$ ./venv3.11/bin/mbs native -h
+$ ./venv3.12/bin/mbs native -h
 
 usage: mbs native [-h] [-c CONFIG] [-i] [-w] [-s] [-n]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -301,15 +301,15 @@
   -n, --no-build        whether or not to skip running 'ninja'
 
 ```
 
 ### `uf2conv`
 
 ```
-$ ./venv3.11/bin/mbs uf2conv -h
+$ ./venv3.12/bin/mbs uf2conv -h
 
 usage: mbs uf2conv [-h] [-b BASE] [-f FAMILY] [-o FILE] [-d DEVICE_PATH] [-l]
                    [-c] [-D] [-w] [-C] [-i]
                    [INPUT]
 
 positional arguments:
   INPUT                 input file (HEX, BIN or UF2)
```

### Comparing `yambs-3.0.1/README.md` & `yambs-3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=454db224964265a8f876fd45d5428729
+    hash=72271a00d30bf23159c35289b5ff7a00
     =====================================
 -->
 
-# yambs ([3.0.1](https://pypi.org/project/yambs/))
+# yambs ([3.0.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -127,15 +127,15 @@
 
 1. Sane out-of-the-box conventions: put your code here (and organize it by
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/mbs -h
+$ ./venv3.12/bin/mbs -h
 
 usage: mbs [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
            {compile_config,dist,download,gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
@@ -161,15 +161,15 @@
 ```
 
 ## Sub-command Options
 
 ### `compile_config`
 
 ```
-$ ./venv3.11/bin/mbs compile_config -h
+$ ./venv3.12/bin/mbs compile_config -h
 
 usage: mbs compile_config [-h] [-i INCLUDES_KEY] [-u] [-e]
                           output inputs [inputs ...]
 
 positional arguments:
   output                file to write
   inputs                files to read
@@ -186,15 +186,15 @@
                         loaded
 
 ```
 
 ### `dist`
 
 ```
-$ ./venv3.11/bin/mbs dist -h
+$ ./venv3.12/bin/mbs dist -h
 
 usage: mbs dist [-h] [-c CONFIG] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -202,15 +202,15 @@
   -s, --sources         set this flag to only capture source files
 
 ```
 
 ### `download`
 
 ```
-$ ./venv3.11/bin/mbs download -h
+$ ./venv3.12/bin/mbs download -h
 
 usage: mbs download [-h] [-o OWNER] [-r REPO] [-O OUTPUT] [-p PATTERN]
 
 options:
   -h, --help            show this help message and exit
   -o OWNER, --owner OWNER
                         repository owner (default: 'vkottler')
@@ -222,15 +222,15 @@
                         filtered by name
 
 ```
 
 ### `gen`
 
 ```
-$ ./venv3.11/bin/mbs gen -h
+$ ./venv3.12/bin/mbs gen -h
 
 usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s] [-n]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -242,15 +242,15 @@
   -n, --no-build        whether or not to skip running 'ninja'
 
 ```
 
 ### `native`
 
 ```
-$ ./venv3.11/bin/mbs native -h
+$ ./venv3.12/bin/mbs native -h
 
 usage: mbs native [-h] [-c CONFIG] [-i] [-w] [-s] [-n]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -262,15 +262,15 @@
   -n, --no-build        whether or not to skip running 'ninja'
 
 ```
 
 ### `uf2conv`
 
 ```
-$ ./venv3.11/bin/mbs uf2conv -h
+$ ./venv3.12/bin/mbs uf2conv -h
 
 usage: mbs uf2conv [-h] [-b BASE] [-f FAMILY] [-o FILE] [-d DEVICE_PATH] [-l]
                    [-c] [-D] [-w] [-C] [-i]
                    [INPUT]
 
 positional arguments:
   INPUT                 input file (HEX, BIN or UF2)
```

### Comparing `yambs-3.0.1/pyproject.toml` & `yambs-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "3.0.1"
+version = "3.0.2"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-3.0.1/setup.py` & `yambs-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/tests/test_entry.py` & `yambs-3.0.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/aggregation/__init__.py` & `yambs-3.0.2/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/app.py` & `yambs-3.0.2/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/all.py` & `yambs-3.0.2/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/common.py` & `yambs-3.0.2/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/compile_config.py` & `yambs-3.0.2/yambs/commands/compile_config.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/dist.py` & `yambs-3.0.2/yambs/commands/dist.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/download.py` & `yambs-3.0.2/yambs/commands/download.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/gen.py` & `yambs-3.0.2/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/native.py` & `yambs-3.0.2/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/commands/uf2conv.py` & `yambs-3.0.2/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/config/__init__.py` & `yambs-3.0.2/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/config/board.py` & `yambs-3.0.2/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/config/common.py` & `yambs-3.0.2/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/config/native.py` & `yambs-3.0.2/yambs/config/native.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/includes/chips.yaml` & `yambs-3.0.2/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/includes/infineon.yaml` & `yambs-3.0.2/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/includes/microchip.yaml` & `yambs-3.0.2/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/native.yaml` & `yambs-3.0.2/yambs/data/native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/schemas/Chip.yaml` & `yambs-3.0.2/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/schemas/Config.yaml` & `yambs-3.0.2/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/schemas/Native.yaml` & `yambs-3.0.2/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/schemas/config_common.yaml` & `yambs-3.0.2/yambs/data/schemas/config_common.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/templates/native_rules.ninja.j2` & `yambs-3.0.2/yambs/data/templates/native_rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/templates/regenerate.ninja.j2` & `yambs-3.0.2/yambs/data/templates/regenerate.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/templates/rules.ninja.j2` & `yambs-3.0.2/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/templates/variant.ninja.j2` & `yambs-3.0.2/yambs/data/templates/variant.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/data/uf2families.json` & `yambs-3.0.2/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/dependency/config.py` & `yambs-3.0.2/yambs/dependency/config.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/dependency/github.py` & `yambs-3.0.2/yambs/dependency/github.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/dependency/handlers/types.py` & `yambs-3.0.2/yambs/dependency/handlers/types.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/dependency/handlers/yambs/__init__.py` & `yambs-3.0.2/yambs/dependency/handlers/yambs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,27 @@
 
 
 def handle_source(task: DependencyTask) -> Path:
     """
     Determine the directory that a given dependency's sources can be found in.
     """
 
+    directory = None
+
     if task.dep.source == DependencySource.GITHUB:
         audit_downloads(
             task.root, task.data, github_release(task.dep, task.data)
         )
         directory = audit_extract(task.root, task.data)
 
     elif task.dep.source == DependencySource.DIRECTORY:
         assert task.dep.directory is not None
         directory = task.dep.directory
 
+    assert directory is not None
     return directory
 
 
 def handle_static_lib(directory: Path, task: DependencyTask) -> None:
     """Handle the third-party dependency's static library."""
 
     static_lib = directory.joinpath(
```

### Comparing `yambs-3.0.1/yambs/dependency/handlers/yambs/config.py` & `yambs-3.0.2/yambs/dependency/handlers/yambs/config.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/dependency/handlers/yambs/github.py` & `yambs-3.0.2/yambs/dependency/handlers/yambs/github.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/dependency/manager.py` & `yambs-3.0.2/yambs/dependency/manager.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/dist/__init__.py` & `yambs-3.0.2/yambs/dist/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 # built-in
 from pathlib import Path
 from shutil import copy2, copytree, make_archive
 from typing import Any, Dict
 
 # third-party
+from vcorelib.paths import rel
 from vcorelib.paths.context import in_dir
 
 # internal
 from yambs import VERSION
 from yambs.config.common import CommonConfig
 
 ARCHIVES = [
@@ -57,16 +58,21 @@
             config.ninja_root,
             root.joinpath("build.ninja"),
             config.file,
         ]
         + [root.joinpath(x) for x in config.data.get("extra_dist", [])]
         if x and x.exists()
     ]:
+        relpath = rel(item, base=root)
+
+        curr_dest = dest.joinpath(relpath)
+        curr_dest.parent.mkdir(parents=True, exist_ok=True)
+
         if item.is_dir():
-            copytree(item, dest.joinpath(item.name))
+            copytree(item, curr_dest)
         else:
-            copy2(item, dest.joinpath(item.name))
+            copy2(item, curr_dest)
 
 
 def dist_metadata() -> Dict[str, Any]:
     """Get metadata for packaged distributions."""
     return {"yambs_version": VERSION}
```

### Comparing `yambs-3.0.1/yambs/entry.py` & `yambs-3.0.2/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/environment/__init__.py` & `yambs-3.0.2/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/environment/native.py` & `yambs-3.0.2/yambs/environment/native.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/__init__.py` & `yambs-3.0.2/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/architectures.py` & `yambs-3.0.2/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/boards.py` & `yambs-3.0.2/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/chips.py` & `yambs-3.0.2/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/common.py` & `yambs-3.0.2/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/ninja/__init__.py` & `yambs-3.0.2/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/ninja/format.py` & `yambs-3.0.2/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/toolchains.py` & `yambs-3.0.2/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/generate/variants.py` & `yambs-3.0.2/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/github/__init__.py` & `yambs-3.0.2/yambs/github/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/paths.py` & `yambs-3.0.2/yambs/paths.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/schemas.py` & `yambs-3.0.2/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/translation/__init__.py` & `yambs-3.0.2/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs/uf2/__init__.py` & `yambs-3.0.2/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.1/yambs.egg-info/PKG-INFO` & `yambs-3.0.2/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 3.0.1
+Version: 3.0.2
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -14,17 +14,17 @@
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rcmpy>=1.5.0
-Requires-Dist: datazen
 Requires-Dist: requests
 Requires-Dist: vcorelib>=2.4.2
+Requires-Dist: datazen
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -37,19 +37,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=454db224964265a8f876fd45d5428729
+    hash=72271a00d30bf23159c35289b5ff7a00
     =====================================
 -->
 
-# yambs ([3.0.1](https://pypi.org/project/yambs/))
+# yambs ([3.0.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -166,15 +166,15 @@
 
 1. Sane out-of-the-box conventions: put your code here (and organize it by
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/mbs -h
+$ ./venv3.12/bin/mbs -h
 
 usage: mbs [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
            {compile_config,dist,download,gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
@@ -200,15 +200,15 @@
 ```
 
 ## Sub-command Options
 
 ### `compile_config`
 
 ```
-$ ./venv3.11/bin/mbs compile_config -h
+$ ./venv3.12/bin/mbs compile_config -h
 
 usage: mbs compile_config [-h] [-i INCLUDES_KEY] [-u] [-e]
                           output inputs [inputs ...]
 
 positional arguments:
   output                file to write
   inputs                files to read
@@ -225,15 +225,15 @@
                         loaded
 
 ```
 
 ### `dist`
 
 ```
-$ ./venv3.11/bin/mbs dist -h
+$ ./venv3.12/bin/mbs dist -h
 
 usage: mbs dist [-h] [-c CONFIG] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -241,15 +241,15 @@
   -s, --sources         set this flag to only capture source files
 
 ```
 
 ### `download`
 
 ```
-$ ./venv3.11/bin/mbs download -h
+$ ./venv3.12/bin/mbs download -h
 
 usage: mbs download [-h] [-o OWNER] [-r REPO] [-O OUTPUT] [-p PATTERN]
 
 options:
   -h, --help            show this help message and exit
   -o OWNER, --owner OWNER
                         repository owner (default: 'vkottler')
@@ -261,15 +261,15 @@
                         filtered by name
 
 ```
 
 ### `gen`
 
 ```
-$ ./venv3.11/bin/mbs gen -h
+$ ./venv3.12/bin/mbs gen -h
 
 usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s] [-n]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -281,15 +281,15 @@
   -n, --no-build        whether or not to skip running 'ninja'
 
 ```
 
 ### `native`
 
 ```
-$ ./venv3.11/bin/mbs native -h
+$ ./venv3.12/bin/mbs native -h
 
 usage: mbs native [-h] [-c CONFIG] [-i] [-w] [-s] [-n]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
@@ -301,15 +301,15 @@
   -n, --no-build        whether or not to skip running 'ninja'
 
 ```
 
 ### `uf2conv`
 
 ```
-$ ./venv3.11/bin/mbs uf2conv -h
+$ ./venv3.12/bin/mbs uf2conv -h
 
 usage: mbs uf2conv [-h] [-b BASE] [-f FAMILY] [-o FILE] [-d DEVICE_PATH] [-l]
                    [-c] [-D] [-w] [-C] [-i]
                    [INPUT]
 
 positional arguments:
   INPUT                 input file (HEX, BIN or UF2)
```

### Comparing `yambs-3.0.1/yambs.egg-info/SOURCES.txt` & `yambs-3.0.2/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


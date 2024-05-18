# Comparing `tmp/sqlite-bedrock-packs-3.1.0.tar.gz` & `tmp/sqlite_bedrock_packs-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite-bedrock-packs-3.1.0.tar", last modified: Sun Aug 27 10:55:01 2023, max compression
+gzip compressed data, was "sqlite_bedrock_packs-3.2.0.tar", last modified: Sat May 18 08:02:52 2024, max compression
```

## Comparing `sqlite-bedrock-packs-3.1.0.tar` & `sqlite_bedrock_packs-3.2.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-08-27 10:55:01.865422 sqlite-bedrock-packs-3.1.0/
--rw-rw-rw-   0        0        0     1083 2022-09-28 23:50:58.000000 sqlite-bedrock-packs-3.1.0/LICENSE
--rw-rw-rw-   0        0        0     5918 2023-08-27 10:55:01.866423 sqlite-bedrock-packs-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4264 2023-08-27 10:43:52.000000 sqlite-bedrock-packs-3.1.0/README.rst
--rw-rw-rw-   0        0        0       90 2022-09-28 21:38:25.000000 sqlite-bedrock-packs-3.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      881 2023-08-27 10:55:01.867422 sqlite-bedrock-packs-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-09-28 23:50:58.000000 sqlite-bedrock-packs-3.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-27 10:55:01.810451 sqlite-bedrock-packs-3.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-27 10:55:01.851904 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/
--rw-rw-rw-   0        0        0    26882 2023-08-27 10:38:21.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/__init__.py
--rw-rw-rw-   0        0        0     9500 2023-08-13 19:04:56.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_attachable.py
--rw-rw-rw-   0        0        0      790 2023-08-13 19:04:56.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_behavior_pack.py
--rw-rw-rw-   0        0        0     1960 2023-08-13 19:04:55.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_animation.py
--rw-rw-rw-   0        0        0     2104 2023-08-13 19:04:55.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_animation_controller.py
--rw-rw-rw-   0        0        0     5710 2023-08-20 19:55:24.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_block.py
--rw-rw-rw-   0        0        0     3411 2023-08-18 18:50:25.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_item.py
--rw-rw-rw-   0        0        0     7760 2023-08-20 11:21:24.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_client_entity.py
--rw-rw-rw-   0        0        0     5190 2023-08-20 10:21:31.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_entity.py
--rw-rw-rw-   0        0        0     2739 2023-08-13 19:04:53.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_geometry.py
--rw-rw-rw-   0        0        0     7029 2023-08-13 19:04:52.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_loot_table.py
--rw-rw-rw-   0        0        0     2313 2023-08-13 19:04:52.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_particle.py
--rw-rw-rw-   0        0        0     9684 2023-08-13 19:04:51.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_render_controller.py
--rw-rw-rw-   0        0        0      790 2023-08-13 19:04:51.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_resource_pack.py
--rw-rw-rw-   0        0        0     3586 2023-08-13 19:04:50.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_rp_animation.py
--rw-rw-rw-   0        0        0     3835 2023-08-13 19:04:50.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_rp_animation_controller.py
--rw-rw-rw-   0        0        0     2021 2023-08-13 19:04:49.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_rp_item.py
--rw-rw-rw-   0        0        0     1417 2023-08-13 19:04:48.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_sound.py
--rw-rw-rw-   0        0        0     3678 2023-08-13 19:04:49.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_sound_definitions.py
--rw-rw-rw-   0        0        0    12036 2023-08-27 09:17:46.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_terrain_texture.py
--rw-rw-rw-   0        0        0     1461 2023-08-13 19:04:48.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_texture.py
--rw-rw-rw-   0        0        0     4898 2023-08-13 19:04:47.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_trade_table.py
--rw-rw-rw-   0        0        0    23370 2023-08-20 11:21:44.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_views.py
-drwxrwxrwx   0        0        0        0 2023-08-27 10:55:01.863425 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/
--rw-rw-rw-   0        0        0      812 2023-08-15 20:14:04.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/__init__.py
--rw-rw-rw-   0        0        0     3234 2023-08-15 20:14:04.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/compact_encoder.py
--rw-rw-rw-   0        0        0    18027 2022-09-28 23:51:39.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/json_walker.py
--rw-rw-rw-   0        0        0     8972 2022-09-28 23:51:39.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/jsonc.py
--rw-rw-rw-   0        0        0        0 2023-08-13 21:14:31.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/py.typed
--rw-rw-rw-   0        0        0     2650 2022-10-05 21:14:45.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/utils.py
--rw-rw-rw-   0        0        0      780 2023-08-27 08:54:14.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/views.py
--rw-rw-rw-   0        0        0    16809 2023-08-27 10:33:34.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/views.pyi
-drwxrwxrwx   0        0        0        0 2023-08-27 10:55:01.856905 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs.egg-info/
--rw-rw-rw-   0        0        0     5918 2023-08-27 10:55:01.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1635 2023-08-27 10:55:01.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-27 10:55:01.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-08-27 10:55:01.000000 sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-27 10:55:01.864422 sqlite-bedrock-packs-3.1.0/tests/
--rw-rw-rw-   0        0        0     2996 2023-08-15 18:09:27.000000 sqlite-bedrock-packs-3.1.0/tests/test_db.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:02:52.293261 sqlite_bedrock_packs-3.2.0/
+-rw-rw-rw-   0        0        0     1083 2022-09-28 23:51:00.000000 sqlite_bedrock_packs-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6148 2024-05-18 08:02:52.293261 sqlite_bedrock_packs-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4492 2024-05-18 07:59:07.000000 sqlite_bedrock_packs-3.2.0/README.rst
+-rw-rw-rw-   0        0        0       90 2023-08-27 21:19:24.000000 sqlite_bedrock_packs-3.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      883 2024-05-18 08:02:52.294398 sqlite_bedrock_packs-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-09-28 23:51:00.000000 sqlite_bedrock_packs-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:02:52.244293 sqlite_bedrock_packs-3.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 08:02:52.277768 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/
+-rw-rw-rw-   0        0        0    27963 2024-05-17 21:17:32.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/__init__.py
+-rw-rw-rw-   0        0        0     9902 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_attachable.py
+-rw-rw-rw-   0        0        0      960 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_behavior_pack.py
+-rw-rw-rw-   0        0        0     2199 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_animation.py
+-rw-rw-rw-   0        0        0     2364 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_animation_controller.py
+-rw-rw-rw-   0        0        0     6017 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_block.py
+-rw-rw-rw-   0        0        0     3635 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_item.py
+-rw-rw-rw-   0        0        0     8144 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_client_entity.py
+-rw-rw-rw-   0        0        0     5484 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_entity.py
+-rw-rw-rw-   0        0        0     7462 2024-05-18 07:28:41.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_feature.py
+-rw-rw-rw-   0        0        0     2484 2024-05-17 14:40:59.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_feature_rule.py
+-rw-rw-rw-   0        0        0     2978 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_geometry.py
+-rw-rw-rw-   0        0        0     7151 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_loot_table.py
+-rw-rw-rw-   0        0        0     2590 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_particle.py
+-rw-rw-rw-   0        0        0     9936 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_render_controller.py
+-rw-rw-rw-   0        0        0      960 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_resource_pack.py
+-rw-rw-rw-   0        0        0     3824 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_rp_animation.py
+-rw-rw-rw-   0        0        0     4097 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_rp_animation_controller.py
+-rw-rw-rw-   0        0        0     2204 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_rp_item.py
+-rw-rw-rw-   0        0        0     1650 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_sound.py
+-rw-rw-rw-   0        0        0     3961 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_sound_definitions.py
+-rw-rw-rw-   0        0        0    12998 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_terrain_texture.py
+-rw-rw-rw-   0        0        0     1698 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_texture.py
+-rw-rw-rw-   0        0        0     5184 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_trade_table.py
+-rw-rw-rw-   0        0        0    24136 2024-05-17 17:12:30.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_views.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:02:52.290260 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/
+-rw-rw-rw-   0        0        0     1028 2023-09-02 09:20:00.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/__init__.py
+-rw-rw-rw-   0        0        0     3591 2023-09-02 09:20:00.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/compact_encoder.py
+-rw-rw-rw-   0        0        0    18281 2023-09-02 09:20:00.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/json_walker.py
+-rw-rw-rw-   0        0        0     9061 2024-01-04 12:42:10.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/jsonc.py
+-rw-rw-rw-   0        0        0        0 2022-09-28 23:51:40.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/py.typed
+-rw-rw-rw-   0        0        0        0 2023-08-13 21:14:32.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/py.typed
+-rw-rw-rw-   0        0        0     2615 2023-09-16 10:57:58.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/utils.py
+-rw-rw-rw-   0        0        0     2086 2024-05-17 15:46:28.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/views.py
+-rw-rw-rw-   0        0        0    20449 2024-05-18 07:59:46.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/views.pyi
+drwxrwxrwx   0        0        0        0 2024-05-18 08:02:52.292259 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs.egg-info/
+-rw-rw-rw-   0        0        0     6148 2024-05-18 08:02:52.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1772 2024-05-18 08:02:52.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 08:02:52.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-18 08:02:52.000000 sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 08:02:52.290260 sqlite_bedrock_packs-3.2.0/tests/
+-rw-rw-rw-   0        0        0     3105 2023-09-16 09:26:34.000000 sqlite_bedrock_packs-3.2.0/tests/test_db.py
```

### Comparing `sqlite-bedrock-packs-3.1.0/LICENSE` & `sqlite_bedrock_packs-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite-bedrock-packs-3.1.0/PKG-INFO` & `sqlite_bedrock_packs-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sqlite-bedrock-packs
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python package that loads data from Minecraft: Bedrock Edition packs into SQLite database
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/sqlite_bedrock_packs/tree/master
 Project-URL: Documentation, https://sqlite-bedrock-packs.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/sqlite-bedrock-packs/badge/?version=latest
     :target: https://sqlite-bedrock-packs.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 SQLite bedrock packs
@@ -34,14 +34,33 @@
 .. code-block:: bash
 
    pip install sqlite-bedrock-packs
 
 Changelog
 =========
 
+3.2.0
+-----
+
+Added new tables:
+
+- FeatureFile
+- Feature
+- FeaturePlacesFeatureField
+- FeaturePlacesFeatureFieldValue
+- FeatureFeaturetypeEnum
+- FeatureRuleFile
+- FeatureRule
+
+
+3.1.1
+-----
+
+Better type hints.
+
 3.1.0
 -----
 
 Added new tables for behavior pack blocks and terrain textures:
 
 - BpBlockFile
 - BpBlock
```

### Comparing `sqlite-bedrock-packs-3.1.0/README.rst` & `sqlite_bedrock_packs-3.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,33 @@
 .. code-block:: bash
 
    pip install sqlite-bedrock-packs
 
 Changelog
 =========
 
+3.2.0
+-----
+
+Added new tables:
+
+- FeatureFile
+- Feature
+- FeaturePlacesFeatureField
+- FeaturePlacesFeatureFieldValue
+- FeatureFeaturetypeEnum
+- FeatureRuleFile
+- FeatureRule
+
+
+3.1.1
+-----
+
+Better type hints.
+
 3.1.0
 -----
 
 Added new tables for behavior pack blocks and terrain textures:
 
 - BpBlockFile
 - BpBlock
```

### Comparing `sqlite-bedrock-packs-3.1.0/setup.cfg` & `sqlite_bedrock_packs-3.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,36 +21,36 @@
 00000140: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
 00000150: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
 00000160: 6c65 0d0a 094c 6963 656e 7365 203a 3a20  le...License :: 
 00000170: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
 00000180: 4d49 5420 4c69 6365 6e73 650d 0a09 5072  MIT License...Pr
 00000190: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 000001a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001b0: 332e 390d 0a70 726f 6a65 6374 5f75 726c  3.9..project_url
-000001c0: 7320 3d20 0d0a 0953 6f75 7263 6520 3d20  s = ...Source = 
-000001d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001e0: 6f6d 2f4e 7573 6971 2f73 716c 6974 655f  om/Nusiq/sqlite_
-000001f0: 6265 6472 6f63 6b5f 7061 636b 732f 7472  bedrock_packs/tr
-00000200: 6565 2f6d 6173 7465 720d 0a09 446f 6375  ee/master...Docu
-00000210: 6d65 6e74 6174 696f 6e20 3d20 6874 7470  mentation = http
-00000220: 733a 2f2f 7371 6c69 7465 2d62 6564 726f  s://sqlite-bedro
-00000230: 636b 2d70 6163 6b73 2e72 6561 6474 6865  ck-packs.readthe
-00000240: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-00000250: 652f 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  e/....[options].
-00000260: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000270: 203d 203e 3d33 2e39 0d0a 7061 636b 6167   = >=3.9..packag
-00000280: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
-00000290: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-000002a0: 3a0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  :....[options.pa
-000002b0: 636b 6167 6573 2e66 696e 645d 0d0a 6578  ckages.find]..ex
-000002c0: 636c 7564 6520 3d20 0d0a 092a 2e74 6573  clude = ...*.tes
-000002d0: 7473 0d0a 092a 2e74 6573 7473 2e2a 0d0a  ts...*.tests.*..
-000002e0: 0974 6573 7473 2e2a 0d0a 0974 6573 7473  .tests.*...tests
-000002f0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000300: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000310: 655f 6461 7461 5d0d 0a73 716c 6974 655f  e_data]..sqlite_
-00000320: 6265 6472 6f63 6b5f 7061 636b 7320 3d20  bedrock_packs = 
-00000330: 0d0a 0970 792e 7479 7065 640d 0a09 2a2e  ...py.typed...*.
-00000340: 7079 690d 0a0d 0a5b 6567 675f 696e 666f  pyi....[egg_info
-00000350: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000360: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000370: 0a                                       .
+000001b0: 332e 3130 0d0a 7072 6f6a 6563 745f 7572  3.10..project_ur
+000001c0: 6c73 203d 200d 0a09 536f 7572 6365 203d  ls = ...Source =
+000001d0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000001e0: 636f 6d2f 4e75 7369 712f 7371 6c69 7465  com/Nusiq/sqlite
+000001f0: 5f62 6564 726f 636b 5f70 6163 6b73 2f74  _bedrock_packs/t
+00000200: 7265 652f 6d61 7374 6572 0d0a 0944 6f63  ree/master...Doc
+00000210: 756d 656e 7461 7469 6f6e 203d 2068 7474  umentation = htt
+00000220: 7073 3a2f 2f73 716c 6974 652d 6265 6472  ps://sqlite-bedr
+00000230: 6f63 6b2d 7061 636b 732e 7265 6164 7468  ock-packs.readth
+00000240: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+00000250: 6c65 2f0d 0a0d 0a5b 6f70 7469 6f6e 735d  le/....[options]
+00000260: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000270: 7320 3d20 3e3d 332e 3130 0d0a 7061 636b  s = >=3.10..pack
+00000280: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
+00000290: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
+000002a0: 6e64 3a0d 0a0d 0a5b 6f70 7469 6f6e 732e  nd:....[options.
+000002b0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000002c0: 6578 636c 7564 6520 3d20 0d0a 092a 2e74  exclude = ...*.t
+000002d0: 6573 7473 0d0a 092a 2e74 6573 7473 2e2a  ests...*.tests.*
+000002e0: 0d0a 0974 6573 7473 2e2a 0d0a 0974 6573  ...tests.*...tes
+000002f0: 7473 0d0a 7768 6572 6520 3d20 7372 630d  ts..where = src.
+00000300: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000310: 6167 655f 6461 7461 5d0d 0a73 716c 6974  age_data]..sqlit
+00000320: 655f 6265 6472 6f63 6b5f 7061 636b 7320  e_bedrock_packs 
+00000330: 3d20 0d0a 0970 792e 7479 7065 640d 0a09  = ...py.typed...
+00000340: 2a2e 7079 690d 0a0d 0a5b 6567 675f 696e  *.pyi....[egg_in
+00000350: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000360: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000370: 0a0d 0a                                  ...
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/__init__.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+'''
+A module that creates a SQLite database and loads resource packs and behavior
+packs into it for easier querying.
+'''
 from __future__ import annotations
 
 import sqlite3
 from collections import deque
 from collections.abc import Container
 from dataclasses import dataclass
 from pathlib import Path
 from sqlite3 import Connection
 from typing import (
-    Iterable, Iterator, Literal, NamedTuple, Optional, Union,
-    TypeVar, overload, TYPE_CHECKING, Any, Type)
+    Iterable, Iterator, Literal, Optional, Union,
+    TypeVar, overload, Type, Generic, TYPE_CHECKING)
 
 # The BP and RP must be imported before other _db_* modules because they are
 # roots of the dependency graph.
 from .views import *
 from ._views import (
     RELATION_MAP, WRAPPER_CLASSES, add_reverse_connections,
     validate_weak_connections, AbstractDBView)
 
-VERSION = (3, 1, 0)  # COMPATIBILITY BREAK, NEW FEATURE, BUGFIX
+VERSION: tuple[int, int, int] = (3, 2, 0)
 __version__ = '.'.join([str(x) for x in VERSION])
 
 # SQLite3 converters/adapters
 def _path_adapter(path: Path):
     return path.as_posix()
 
 def _path_converter(path: bytes):
@@ -47,15 +51,17 @@
 DbBpItems = Literal[
     "entities",
     "loot_tables",
     "trade_tables",
     "bp_animations",
     "bp_animation_controllers",
     "bp_items",
-    "bp_blocks"
+    "bp_blocks",
+    "feature_rules",
+    "features"
 ]
 
 # THE MAIN DATABASE CLASS
 @dataclass
 class Database:
     '''
     A class that represents a database with resource packs and behavior packs.
@@ -87,16 +93,15 @@
     def create(db_path: Union[str, Path] = ":memory:") -> Database:
         '''
         Creates a new database for storing resource packs and behavior packs in
         memory or in a file. The default value is :code:`":memory:"` which
         means that the database is created in memory (just like in sqlite3).
 
         :param db_path: The path to the database file or :code:`":memory:"`.
-        '''
-        '''
+
         Creates a new dtabase in :code:`db_path`. Runs all of the build scripts of
         the database components.
 
         :param db_path: The path to the database file. The argument is passed to
             :func:`sqlite3.connect` If the argument is :code:`":memory:"`, the
             database is created in memory. :code:`":memory:"` is the default value.
         '''
@@ -125,20 +130,22 @@
         db.executescript(ENTITY_BUILD_SCRIPT)
         db.executescript(LOOT_TABLE_BUILD_SCRIPT)
         db.executescript(TRADE_TABLE_BUILD_SCRIPT)
         db.executescript(BP_ANIMATION_BUILD_SCRIPT)
         db.executescript(BP_ANIMATION_CONTROLLER_BUILD_SCRIPT)
         db.executescript(BP_ITEM_BUILD_SCRIPT)
         db.executescript(BP_BLOCK_BUILD_SCRIPT)
+        db.executescript(FEATURE_RULE_BUILD_SCRIPT)
+        db.executescript(FEATURE_BUILD_SCRIPT)
 
         return Database(db)
 
     def load_rp(
         self,
-        rp_path: Path, *,
+        rp_path: Path | str, *,
         include: Container[DbRpItems] = (
             "geometries",
             "client_entities",
             "render_controllers",
             "textures",
             "particles",
             "rp_animations",
@@ -214,23 +221,25 @@
         if (
                 "terrain_texture" in include and
                 "terrain_texture" not in exclude):
             load_terrain_texture(self.connection, rp_pk)
         self.connection.commit()
     def load_bp(
             self,
-            bp_path: Path, *,
+            bp_path: Path | str, *,
             include: Container[DbBpItems] = (
                 "entities",
                 "loot_tables",
                 "trade_tables",
                 "bp_animations",
                 "bp_animation_controllers",
                 "bp_items",
-                "bp_blocks"
+                "bp_blocks",
+                "feature_rules",
+                "features"
             ),
             exclude: Container[DbBpItems] = tuple()) -> None:
         '''
         Loads behavior pack data into the database.
 
         :param db: The database connection.
         :param bp_path: The path to the resource pack.
@@ -268,14 +277,22 @@
                 "bp_items" in include and
                 "bp_items" not in exclude):
             load_bp_items(self.connection, bp_pk)
         if (
                 "bp_blocks" in include and
                 "bp_blocks" not in exclude):
             load_bp_blocks(self.connection, bp_pk)
+        if (
+                "feature_rules" in include and
+                "feature_rules" not in exclude):
+            load_feature_rules(self.connection, bp_pk)
+        if (
+                "features" in include and
+                "features" not in exclude):
+            load_features(self.connection, bp_pk)
         self.connection.commit()
 
     def close(self):
         '''
         Runs close() function on the database connection.
         '''
         self.connection.close()
@@ -293,33 +310,27 @@
 _T4 = TypeVar("_T4", bound=AbstractDBView)
 _T5 = TypeVar("_T5", bound=AbstractDBView)
 _T6 = TypeVar("_T6", bound=AbstractDBView)
 _T7 = TypeVar("_T7", bound=AbstractDBView)
 _T8 = TypeVar("_T8", bound=AbstractDBView)
 _T9 = TypeVar("_T9", bound=AbstractDBView)
 
-class Left(NamedTuple):
+class Left(Generic[_T]):
     '''
     A helper class to indicate that a table should be joined using LEFT join in
     the query of :class:`EasyQuery` class.
     '''
-    value: str
-    '''The name of the table'''
-
-if TYPE_CHECKING:
-    # This is a hack to satisfy the type checker. IT makes it think that
-    # Left is a function that returns the same type as the argument which
-    # is later used in the EasyQuery class to deterimine the types of the
-    # arguments to yield.
-    def Left(value: Type[_T]) -> Type[_T]:
-        return value
+    def __init__(self, value: Type[_T]):
+        self.value = value
 
+    if TYPE_CHECKING:
+        __name__: str
 def build_easy_query(
-        root: _T2,
-        *tables: Any,
+        root: Type[AbstractDBView],
+        *tables: Type[AbstractDBView] | Left[AbstractDBView],
         blacklist: Iterable[str] = ("BehaviorPack", "ResourcePack"),
         accept_non_pk: bool = True,
         distinct: bool = True,
         where: Optional[list[str]] = None,
         group_by: Optional[list[str]] = None,
         having: Optional[list[str]] = None,
         order_by: Optional[list[str]] = None) -> str:
@@ -388,15 +399,16 @@
     :param having: A list of constraints to add to the query. This is a
         list of strings with raw SQL code which is inserted into the HAVING
         part of the query. The constraints are joined using AND.
     :param order_by: A list of columns to order the results by. This is a
         list of strings with raw SQL code which is inserted into the ORDER BY
         part of the query.
     '''
-    all_tables: list[Union[_T, Left]] = [root, *tables]
+    all_tables: list[Union[type[AbstractDBView], Left[AbstractDBView]]] = [
+        root, *tables]
     for t in all_tables:
         t_name = t.value.__name__ if isinstance(t, Left) else t.__name__
         if t_name not in RELATION_MAP.keys():
             raise ValueError(
                 f"Table '{t_name}' does not exist in the database.")
     prev_t = None
     joined_connections: list[_EasyQueryConnection] = []
@@ -417,15 +429,15 @@
                 f"after excluding tables: {', '.join(blacklist)}")
         # if left and len(connection) > 1:
         if left:
             connection[-1].left_join = True
         joined_connections.extend(connection)
         prev_t = t
     # Strip joined_connections of duplicates
-    reduced_joined_connections = []
+    reduced_joined_connections: list[_EasyQueryConnection] = []
     if len(joined_connections) > 0:
         known_connections = {joined_connections[0].left}
         for jc in joined_connections:
             if jc.right in known_connections:
                 continue
             known_connections.add(jc.right)
             reduced_joined_connections.append(jc)
@@ -445,194 +457,195 @@
         join = "LEFT JOIN" if c.left_join else "JOIN"
         query += (
             f'\n{join} {c.right}\n'
             f'\tON {c.left}.{c.left_column} = {c.right}.{c.right_column}')
     if where is not None:
         if isinstance(where, str):
             where = [where]
-        query += f'\nWHERE\n\t'+"\n\tAND ".join(where)
+        query += '\nWHERE\n\t'+"\n\tAND ".join(where)
     if group_by is not None:
         if isinstance(group_by, str):
             group_by = [group_by]
-        query += f'\nGROUP BY\n\t'+"\n\t, ".join(group_by)
+        query += '\nGROUP BY\n\t'+"\n\t, ".join(group_by)
     if having is not None:
         if isinstance(having, str):
             having = [having]
-        query += f'\nHAVING\n\t'+"\n\tAND ".join(having)
+        query += '\nHAVING\n\t'+"\n\tAND ".join(having)
     if order_by is not None:
         if isinstance(order_by, str):
             order_by = [order_by]
-        query += f'\nORDER BY\n\t'+"\n\t, ".join(order_by)
+        query += '\nORDER BY\n\t'+"\n\t, ".join(order_by)
     return query
 
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        /,
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        t3: Type[_T3],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        t3: Type[_T3] | Left[_T3],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2, _T3]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        t3: Type[_T3],
-        t4: Type[_T4],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        t3: Type[_T3] | Left[_T3],
+        t4: Type[_T4] | Left[_T4],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2, _T3, _T4]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        t3: Type[_T3],
-        t4: Type[_T4],
-        t5: Type[_T5],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        t3: Type[_T3] | Left[_T3],
+        t4: Type[_T4] | Left[_T4],
+        t5: Type[_T5] | Left[_T5],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2, _T3, _T4, _T5]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        t3: Type[_T3],
-        t4: Type[_T4],
-        t5: Type[_T5],
-        t6: Type[_T6],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        t3: Type[_T3] | Left[_T3],
+        t4: Type[_T4] | Left[_T4],
+        t5: Type[_T5] | Left[_T5],
+        t6: Type[_T6] | Left[_T6],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2, _T3, _T4, _T5, _T6]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        t3: Type[_T3],
-        t4: Type[_T4],
-        t5: Type[_T5],
-        t6: Type[_T6],
-        t7: Type[_T7],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        t3: Type[_T3] | Left[_T3],
+        t4: Type[_T4] | Left[_T4],
+        t5: Type[_T5] | Left[_T5],
+        t6: Type[_T6] | Left[_T6],
+        t7: Type[_T7] | Left[_T7],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2, _T3, _T4, _T5, _T6, _T7]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        t3: Type[_T3],
-        t4: Type[_T4],
-        t5: Type[_T5],
-        t6: Type[_T6],
-        t7: Type[_T7],
-        t8: Type[_T8],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        t3: Type[_T3] | Left[_T3],
+        t4: Type[_T4] | Left[_T4],
+        t5: Type[_T5] | Left[_T5],
+        t6: Type[_T6] | Left[_T6],
+        t7: Type[_T7] | Left[_T7],
+        t8: Type[_T8] | Left[_T8],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2, _T3, _T4, _T5, _T6, _T7, _T8]]: ...
 @overload
 def yield_from_easy_query(
         db: Union[Connection, Database],
         t1: Type[_T],
-        t2: Type[_T2],
-        t3: Type[_T3],
-        t4: Type[_T4],
-        t5: Type[_T5],
-        t6: Type[_T6],
-        t7: Type[_T7],
-        t8: Type[_T8],
-        t9: Type[_T9],
-        /,
+        t2: Type[_T2] | Left[_T2],
+        t3: Type[_T3] | Left[_T3],
+        t4: Type[_T4] | Left[_T4],
+        t5: Type[_T5] | Left[_T5],
+        t6: Type[_T6] | Left[_T6],
+        t7: Type[_T7] | Left[_T7],
+        t8: Type[_T8] | Left[_T8],
+        t9: Type[_T9] | Left[_T9],
+        /, *,
         blacklist: Iterable[str] = ...,
         accept_non_pk: bool = ...,
         distinct: bool = ...,
         where: Optional[list[str]] = ...,
         group_by: Optional[list[str]] = ...,
         having: Optional[list[str]] = ...,
         order_by: Optional[list[str]] = ...
 ) -> Iterator[tuple[_T, _T2, _T3, _T4, _T5, _T6, _T7, _T8, _T9]]: ...
 
 def yield_from_easy_query(
         db: Union[Connection, Database],
-        root: Any,
-        *tables: Any,
+        root: Type[AbstractDBView],
+        /,
+        *tables: Type[AbstractDBView] | Left[AbstractDBView],
         blacklist: Iterable[str] = ("BehaviorPack", "ResourcePack"),
         accept_non_pk: bool = True,
         distinct: bool = True,
         where: Optional[list[str]] = None,
         group_by: Optional[list[str]] = None,
         having: Optional[list[str]] = None,
-        order_by: Optional[list[str]] = None) -> Iterator[tuple]:
+        order_by: Optional[list[str]] = None) -> Iterator[tuple[AbstractDBView | None, ...]]:
     '''
     Returns an iterator that yields the wrapper classes from the query
     results. The arguments are the same as for :func:`build_easy_query`.
     The first argument is the Database object or the sqlite3.Connection.
     '''
 
     # Copy the arguments and pass them to build_easy_query
@@ -644,29 +657,31 @@
         where=where,
         group_by=group_by,
         having=having,
         order_by=order_by
     )
     yield from yield_from_any_query(db, sql_query)
 
-def yield_from_any_query(db: Union[Connection, Database], sql_query: str) -> Iterator[tuple]:
+def yield_from_any_query(
+        db: Union[Connection, Database],
+        sql_query: str) -> Iterator[tuple[AbstractDBView | None, ...]]:
     '''
     Yields the results from any query generated by :func:`build_easy_query`
     function and wraps them in the wrapper classes. This function in
     combination with :func:`build_easy_query` is equivalent to the
     :func:`yield_from_easy_query` function.
     '''
     if isinstance(db, Database):
         db = db.connection
     cursor = db.execute(sql_query)
     wrappers = [
         WRAPPER_CLASSES[d[0]] for d in cursor.description
     ]
     for row in cursor:
-        yield tuple(
+        yield tuple(  # type: ignore
             None if value is None else wrapper(db, value)
             for value, wrapper in zip(row, wrappers)
         )
 
 # Private functions
 @dataclass
 class _EasyQueryConnection:
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_attachable.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_attachable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
-from .better_json_tools import load_jsonc
-from ._views import dbtableview
 import json
+from .better_json_tools import load_jsonc
+from ._views import dbtableview, WeakTableConnection
 
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
@@ -25,16 +26,16 @@
     properties={
         "identifier": (str, "NOT NULL"),
         "condition": (str, ""),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["Attachable"],
     weak_connects_to=[
-        ("identifier", "RpItem", "identifier"),
-        ("identifier", "BpItem", "identifier")
+        WeakTableConnection("identifier", "RpItem", "identifier"),
+        WeakTableConnection("identifier", "BpItem", "identifier")
     ]
 )
 class AttachableItemField:
     '''
     This maps the item used by the attachable. Attachables have two types of
     connecting items. They can either have an identifier matching to the item
     or they can have the 'item' property which maps the item with a condition.
@@ -55,94 +56,100 @@
     properties={
         "shortName": (str, "NOT NULL"),
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["Attachable"],
     weak_connects_to=[
-        ("identifier", "TextureFile", "identifier")
+        WeakTableConnection("identifier", "TextureFile", "identifier")
     ]
 )
 class AttachableTextureField: ...
 
 @dbtableview(
     properties={
         "shortName": (str, "NOT NULL"),
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["Attachable"],
     weak_connects_to=[
-        ("identifier", "Geometry", "identifier")
+        WeakTableConnection("identifier", "Geometry", "identifier")
     ]
 )
 class AttachableGeometryField: ...
 
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "condition": (str, ""),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["Attachable"],
     weak_connects_to=[
-        ("identifier", "RenderController", "identifier")
+        WeakTableConnection("identifier", "RenderController", "identifier")
     ]
 )
 class AttachableRenderControllerField: ...
 
 @dbtableview(
     properties={
         "shortName": (str, "NOT NULL"),
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["Attachable"],
     weak_connects_to=[
-        ("identifier", "RpAnimation", "identifier")
+        WeakTableConnection("identifier", "RpAnimation", "identifier")
     ]
 )
 class AttachableAnimationField: ...
 
 @dbtableview(
     properties={
         "shortName": (str, "NOT NULL"),
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["Attachable"],
     weak_connects_to=[
-        ("identifier", "RpAnimationController", "identifier")
+        WeakTableConnection("identifier", "RpAnimationController", "identifier")
     ]
 )
 class AttachableAnimationControllerField: ...
 
 
-ATTACHABLE_BUILD_SCRIPT = (
+ATTACHABLE_BUILD_SCRIPT: str = (
     AttachableFile.build_script +
     Attachable.build_script +
     AttachableItemField.build_script +
     AttachableMaterialField.build_script +
     AttachableTextureField.build_script +
     AttachableGeometryField.build_script +
     AttachableRenderControllerField.build_script +
     AttachableAnimationField.build_script +
     AttachableAnimationControllerField.build_script
 )
 
 def load_attachables(db: Connection, rp_id: int):
+    '''
+    Loads all attachables from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for attachable_path in (rp_path / "attachables").rglob("*.json"):
         load_attachable(db, attachable_path, rp_id)
 
 def load_attachable(db: Connection, attachable_path: Path, rp_id: int):
+    '''
+    Loads a single attachable from the resource pack.
+    '''
     cursor = db.cursor()
     # ATTACHABLE FILE
     cursor.execute(
         "INSERT INTO AttachableFile (path, ResourcePack_fk) VALUES (?, ?)",
         (attachable_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_behavior_pack.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_behavior_pack.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
 from typing import Union
 from ._views import dbtableview
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     }
 )
 class BehaviorPack: ...
 
 
-BEHAVIOR_PACK_BUILD_SCRIPT = BehaviorPack.build_script
+BEHAVIOR_PACK_BUILD_SCRIPT: str = BehaviorPack.build_script
 
 def load_behavior_pack(db: Connection, rp_path: Union[Path, str]) -> int:
+    '''
+    Loads a behavior pack into the database.
+    '''
     if isinstance(rp_path, Path):
         rp_path = rp_path.as_posix()
     count = db.execute(
         "SELECT total(1) FROM BehaviorPack WHERE path = ?",
         (rp_path,)).fetchone()[0]
     if count != 0:
         raise ValueError("RP already loaded.")
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_animation.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_animation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,54 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from typing import cast
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
 from ._views import dbtableview
-import json
 
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["BehaviorPack"]
 )
 class BpAnimationFile: ...
- 
+
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["BpAnimationFile"]
 )
 class BpAnimation: ...
 
-BP_ANIMATION_BUILD_SCRIPT = (
+BP_ANIMATION_BUILD_SCRIPT: str = (
     BpAnimationFile.build_script +
     BpAnimation.build_script
 )
 
 def load_bp_animations(db: Connection, bp_id: int):
+    '''
+    Loads all animations from the behavior pack.
+    '''
     bp_path: Path = db.execute(
         "SELECT path FROM BehaviorPack WHERE BehaviorPack_pk = ?",
         (bp_id,)
     ).fetchone()[0]
 
     for animation_path in (bp_path / "animations").rglob("*.json"):
         load_bp_animation(db, animation_path, bp_id)
 
 def load_bp_animation(db: Connection, animation_path: Path, bp_id: int):
+    '''
+    Loads an animation from the behavior pack.
+    '''
     cursor = db.cursor()
     # BP ANIMATION FILE
     cursor.execute(
         "INSERT INTO BpAnimationFile (path, BehaviorPack_fk) VALUES (?, ?)",
         (animation_path.as_posix(), bp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_animation_controller.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_animation_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from typing import cast
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
 from ._views import dbtableview
-import json
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["BehaviorPack"]
 )
@@ -19,30 +20,36 @@
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["BpAnimationControllerFile"]
 )
 class BpAnimationController: ...
 
 
-BP_ANIMATION_CONTROLLER_BUILD_SCRIPT = (
+BP_ANIMATION_CONTROLLER_BUILD_SCRIPT: str = (
     BpAnimationControllerFile.build_script +
     BpAnimationController.build_script
 )
 
 def load_bp_animation_controllers(db: Connection, bp_id: int):
+    '''
+    Loads all animation controllers from the behavior pack.
+    '''
     bp_path: Path = db.execute(
         "SELECT path FROM BehaviorPack WHERE BehaviorPack_pk = ?",
         (bp_id,)
     ).fetchone()[0]
 
     for ac_path in (bp_path / "animation_controllers").rglob("*.json"):
         load_bp_animation_controller(db, ac_path, bp_id)
 
 
 def load_bp_animation_controller(db: Connection, animation_controller_path: Path, bp_id: int):
+    '''
+    Loads an animation controller from the behavior pack.
+    '''
     cursor = db.cursor()
     # BP ANIMATION FILE
     cursor.execute(
         "INSERT INTO BpAnimationControllerFile (path, BehaviorPack_fk) VALUES (?, ?)",
         (animation_controller_path.as_posix(), bp_id)
     )
     file_pk = cursor.lastrowid
@@ -61,8 +68,7 @@
             INSERT INTO BpAnimationController (
                 BpAnimationControllerFile_fk, identifier, jsonPath
             ) VALUES (?, ?, ?)
             ''',
             (file_pk, identifier_data, ac_walker.path_str)
         )
         # bp_anim_pk = cursor.lastrowid
-
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_block.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from typing import cast
 from sqlite3 import Connection
 from pathlib import Path
-from .better_json_tools import load_jsonc
-from ._views import dbtableview
 import json
+from .better_json_tools import load_jsonc
+from ._views import dbtableview, WeakTableConnection
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["BehaviorPack"]
 )
@@ -24,27 +25,27 @@
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL"),
     },
     connects_to=["BpBlock"],
     weak_connects_to=[
-        ("identifier", "LootTable", "identifier")
+        WeakTableConnection("identifier", "LootTable", "identifier")
     ]
 )
 class BpBlockLootField: ...
 
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL"),
     },
     connects_to=["BpBlock"],
     weak_connects_to=[
-        ("identifier", "Geometry", "identifier")
+        WeakTableConnection("identifier", "Geometry", "identifier")
     ]
 )
 class BpBlockGeometryField: ...
 
 @dbtableview(
     properties={
         "jsonPath": (str, "NOT NULL"),
@@ -58,51 +59,57 @@
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL"),
         "texture": (str, "NOT NULL"),
         "renderMethod": (str, "NOT NULL"),
     },
     connects_to=["BpBlockMaterialInstancesField"],
     weak_connects_to=[
-        ("texture", "TerrainTexture", "identifier")
+        WeakTableConnection("texture", "TerrainTexture", "identifier")
     ]
 )
 class BpBlockMaterialInstancesFieldInstance: ...
 
-BP_BLOCK_BUILD_SCRIPT = (
+BP_BLOCK_BUILD_SCRIPT: str = (
     BpBlockFile.build_script +
     BpBlock.build_script +
     BpBlockLootField.build_script +
     BpBlockGeometryField.build_script +
     BpBlockMaterialInstancesField.build_script +
     BpBlockMaterialInstancesFieldInstance.build_script
 )
 
 
 def load_bp_blocks(db: Connection, bp_id: int):
+    '''
+    Loads all blocks from the behavior pack.
+    '''
     bp_path: Path = db.execute(
         "SELECT path FROM BehaviorPack WHERE BehaviorPack_pk = ?",
         (bp_id,)
     ).fetchone()[0]
     for bp_block_path in (bp_path / "blocks").rglob("*.json"):
         load_bp_block(db, bp_block_path, bp_id)
 
 def load_bp_block(db: Connection, bp_block_path: Path, bp_id: int):
+    '''
+    Loads a block from the behavior pack.
+    '''
     cursor = db.cursor()
     # BP BLOCK FILE
     cursor.execute(
         "INSERT INTO BpBlockFile (path, BehaviorPack_fk) VALUES (?, ?)",
         (bp_block_path.as_posix(), bp_id)
     )
     file_pk = cursor.lastrowid
     # BP BLOCK
     try:
         bp_block_json = load_jsonc(bp_block_path)
     except json.JSONDecodeError:
         return  # Skip silently
-    
+
     block_walker = (
         bp_block_json / "minecraft:block")
     block_identifier = (block_walker / "description" / "identifier").data
     if not isinstance(block_identifier, str):
         return  # Skip blocks without identifier
     cursor.execute(
         '''
@@ -172,8 +179,8 @@
                 ''',
                 (
                     instance_identifier,
                     instance_walker.path_str,
                     instance_texture,
                     instance_render_method,
                     material_instances_pk
-                ))
+                ))
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_bp_item.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_bp_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import cast, Optional
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
+from typing import Optional
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
 from .utils import parse_format_version
 from ._views import dbtableview
-import json
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["BehaviorPack"]
 )
@@ -30,29 +31,35 @@
         "parserVersion": ["1.10", "1.16.100"]
     },
     connects_to=["BpItemFile"]
 )
 class BpItem: ...
 
 
-BP_ITEM_BUILD_SCRIPT = (
+BP_ITEM_BUILD_SCRIPT: str = (
     BpItemFile.build_script +
     BpItem.build_script
 )
 
 def load_bp_items(db: Connection, bp_id: int):
+    '''
+    Loads all items from the behavior pack.
+    '''
     bp_path: Path = db.execute(
         "SELECT path FROM BehaviorPack WHERE BehaviorPack_pk = ?",
         (bp_id,)
     ).fetchone()[0]
 
     for item_path in (bp_path / "items").rglob("*.json"):
         load_bp_item(db, item_path, bp_id)
 
 def load_bp_item(db: Connection, item_path: Path, bp_id: int):
+    '''
+    Loads an item from the behavior pack.
+    '''
     cursor = db.cursor()
     # BP ITEM FILE
     cursor.execute(
         "INSERT INTO BpItemFile (path, BehaviorPack_fk) VALUES (?, ?)",
         (item_path.as_posix(), bp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_client_entity.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_client_entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
-from .better_json_tools import load_jsonc
 import json
-from ._views import dbtableview
+from .better_json_tools import load_jsonc
+from ._views import dbtableview, WeakTableConnection
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
@@ -14,41 +15,41 @@
 
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL")
     },
     connects_to=["ClientEntityFile"],
     weak_connects_to=[
-        ("identifier", "Entity", "identifier")
+        WeakTableConnection("identifier", "Entity", "identifier")
     ]
 )
 class ClientEntity: ...
 
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "condition": (str, ""),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["ClientEntity"],
     weak_connects_to=[
-        ("identifier", "RenderController", "identifier")
+        WeakTableConnection("identifier", "RenderController", "identifier")
     ]
 )
 class ClientEntityRenderControllerField: ...
 
 @dbtableview(
     properties={
         "shortName": (str, "NOT NULL"),
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["ClientEntity"],
     weak_connects_to=[
-        ("identifier", "Geometry", "identifier")
+        WeakTableConnection("identifier", "Geometry", "identifier")
     ]
 )
 class ClientEntityGeometryField: ...
 
 @dbtableview(
     properties={
         "shortName": (str, "NOT NULL"),
@@ -56,15 +57,15 @@
         # identifier is the path without the extension
         "identifier": (str, "NOT NULL"),
 
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["ClientEntity"],
     weak_connects_to=[
-        ("identifier", "TextureFile", "identifier")
+        WeakTableConnection("identifier", "TextureFile", "identifier")
     ]
 )
 class ClientEntityTextureField: ...
 
 @dbtableview(
     properties={
         "shortName": (str, "NOT NULL"),
@@ -79,53 +80,59 @@
     properties={
         "shortName": (str, "NOT NULL"),
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["ClientEntity"],
     weak_connects_to=[
-        ("identifier", "RpAnimation", "identifier")
+        WeakTableConnection("identifier", "RpAnimation", "identifier")
     ]
 )
 class ClientEntityAnimationField: ...
 
 @dbtableview(
     properties={
         "shortName": (str, "NOT NULL"),
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["ClientEntity"],
     weak_connects_to=[
-        ("identifier", "RpAnimationController", "identifier")
+        WeakTableConnection("identifier", "RpAnimationController", "identifier")
     ]
 )
 class ClientEntityAnimationControllerField: ...
 
-CLIENT_ENTITY_BUILD_SCRIPT = (
+CLIENT_ENTITY_BUILD_SCRIPT: str = (
     ClientEntityFile.build_script +
     ClientEntity.build_script +
     ClientEntityRenderControllerField.build_script +
     ClientEntityGeometryField.build_script +
     ClientEntityTextureField.build_script +
     ClientEntityMaterialField.build_script +
     ClientEntityAnimationField.build_script +
     ClientEntityAnimationControllerField.build_script
 )
 
 def load_client_entities(db: Connection, rp_id: int):
+    '''
+    Loads all client entities from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for entity_path in (rp_path / "entity").rglob("*.json"):
         load_client_entity(db, entity_path, rp_id)
 
 def load_client_entity(db: Connection, entity_path: Path, rp_id: int):
+    '''
+    Loads a client entity from the resource pack.
+    '''
     cursor = db.cursor()
     # ENTITY FILE
     cursor.execute(
         "INSERT INTO ClientEntityFile (path, ResourcePack_fk) VALUES (?, ?)",
         (entity_path.as_posix(), rp_id))
 
     file_pk = cursor.lastrowid
@@ -160,15 +167,15 @@
                 ClientEntity_fk, identifier, jsonPath
             ) VALUES (?, ?, ?)
             ''',
             (entity_pk, identifier, rc.path_str))
     # RENDER CONTROLLERS - conditional
     for rc in (description / "render_controllers" // int // str):
         if isinstance(rc.data, str):
-           condition = rc.data
+            condition = rc.data
         else:
             condition = None
         cursor.execute(
             '''
             INSERT INTO ClientEntityRenderControllerField (
                 ClientEntity_fk, identifier, condition, jsonPath
             ) VALUES (?, ?, ?, ?)
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_entity.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
-from .better_json_tools import load_jsonc
-from ._views import dbtableview
 import json
+from .better_json_tools import load_jsonc
+from ._views import dbtableview, WeakTableConnection
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["BehaviorPack"]
 )
@@ -26,30 +27,30 @@
         "jsonPath": (str, "NOT NULL"),
     },
     enum_properties={
         "componentType": ["minecraft:loot", "minecraft:equipment"]
     },
     connects_to=["Entity"],
     weak_connects_to=[
-        ("identifier", "LootTable", "identifier")
+        WeakTableConnection("identifier", "LootTable", "identifier")
     ]
 )
 class EntityLootField: ...
 
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL"),
     },
     enum_properties={
         "componentType": ["minecraft:economy_trade_table", "minecraft:trade_table"]
     },
     connects_to=["Entity"],
     weak_connects_to=[
-        ("identifier", "TradeTable", "identifier")
+        WeakTableConnection("identifier", "TradeTable", "identifier")
     ]
 )
 class EntityTradeField: ...
 
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
@@ -59,32 +60,38 @@
 class EntitySpawnEggField:
     '''
     Spawn eggs are added to the database based on entities that use the
     is_spawnable property. The name of the spawn egg is based on the entity
     identifier.
     '''
 
-ENTITY_BUILD_SCRIPT = (
+ENTITY_BUILD_SCRIPT: str = (
     EntityFile.build_script +
     Entity.build_script +
     EntityLootField.build_script +
     EntityTradeField.build_script +
     EntitySpawnEggField.build_script
 )
 
 def load_entities(db: Connection, bp_id: int):
+    '''
+    Loads all entities from the behavior pack.
+    '''
     bp_path: Path = db.execute(
         "SELECT path FROM BehaviorPack WHERE BehaviorPack_pk = ?",
         (bp_id,)
     ).fetchone()[0]
 
     for entity_path in (bp_path / "entities").rglob("*.json"):
         load_entity(db, entity_path, bp_id)
 
 def load_entity(db: Connection, entity_path: Path, bp_id: int):
+    '''
+    Loads an entity from the behavior pack.
+    '''
     cursor = db.cursor()
     # ENTITY FILE
     cursor.execute(
         "INSERT INTO EntityFile (path, BehaviorPack_fk) VALUES (?, ?)",
         (entity_path.as_posix(), bp_id))
 
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_geometry.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_geometry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from typing import cast, Optional
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
 from ._views import dbtableview
-import json
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
@@ -19,29 +20,35 @@
         "parent": (str, ""),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["GeometryFile"]
 )
 class Geometry: ...
 
-GEOMETRY_BUILD_SCRIPT = (
+GEOMETRY_BUILD_SCRIPT: str = (
     GeometryFile.build_script +
     Geometry.build_script
 )
 
 def load_geometries(db: Connection, rp_id: int):
+    '''
+    Loads all geometries from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for geometry_path in (rp_path / "models").rglob("*.json"):
         load_geometry(db, geometry_path, rp_id)
 
 def load_geometry(db: Connection, geometry_path: Path, rp_id: int):
+    '''
+    Loads a geometry from the resource pack.
+    '''
     cursor = db.cursor()
     # GEOMETRY FILE
     cursor.execute(
         "INSERT INTO GeometryFile (path, ResourcePack_fk) VALUES (?, ?)",
         (geometry_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
@@ -53,28 +60,28 @@
     # Try with 1.8.0 format
     for identifier in geometry_jsonc // str:
         full_identifier = cast(str, identifier.parent_key)
         if not full_identifier.startswith("geometry."):
             continue
         # Check for inheritance
         split = full_identifier.split(":", 1)
-        id = full_identifier
+        id_ = full_identifier
         parent: Optional[str] = None
         if len(split)  == 2:
-            id, parent = split
+            id_, parent = split
         cursor.execute(
             '''
             INSERT INTO Geometry (
                 identifier, parent, GeometryFile_fk, jsonPath
             ) VALUES (?, ?, ?, ?)
             ''',
-            (id, parent, file_pk, identifier.path_str)
+            (id_, parent, file_pk, identifier.path_str)
         )
     # Try with 1.12.0 format
-    geometries = (geometry_jsonc / "minecraft:geometry" // int)
+    geometries = geometry_jsonc / "minecraft:geometry" // int
     for geometry in geometries:
         identifier = geometry / 'description' / 'identifier'
         identifier_data = identifier.data
         if not isinstance(identifier_data, str):
             continue
         if not identifier_data.startswith("geometry."):
             continue
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_loot_table.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_loot_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import cast, Optional
-from sqlite3 import Connection
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
+from sqlite3 import Connection, Cursor
 from pathlib import Path
-from .better_json_tools import load_jsonc
-from ._views import dbtableview
 import json
+from typing import cast
+from .better_json_tools import load_jsonc, JSONWalker
+from ._views import dbtableview, WeakTableConnection
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["BehaviorPack"]
 )
@@ -27,16 +28,16 @@
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["LootTable"],
     weak_connects_to=[
-        ("identifier", "RpItem", "identifier"),
-        ("identifier", "BpItem", "identifier")
+        WeakTableConnection("identifier", "RpItem", "identifier"),
+        WeakTableConnection("identifier", "BpItem", "identifier")
     ]
 )
 class LootTableItemField: ...
 
 @dbtableview(
     properties={
         "entityIdentifier": (str, "NOT NULL"),
@@ -50,50 +51,56 @@
         # LootTableItemSpawnEggReferenceField.connectionType column.
         # Stores the type of connection, it can be either "direct" or
         # "set_actor_id_function".
         "connectionType": ["direct", "set_actor_id_function"]
     },
     connects_to=["LootTableItemField"],
     weak_connects_to=[
-        ("spawnEggIdentifier", "EntitySpawnEggField", "identifier")
+        WeakTableConnection("spawnEggIdentifier", "EntitySpawnEggField", "identifier")
     ]
 )
 class LootTableItemSpawnEggReferenceField: ...
 
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["LootTable"],
     weak_connects_to=[
-        ("identifier", "LootTable", "identifier")
+        WeakTableConnection("identifier", "LootTable", "identifier")
     ]
 )
 class LootTableLootTableField: ...
 
-LOOT_TABLE_BUILD_SCRIPT = (
+LOOT_TABLE_BUILD_SCRIPT: str = (
     LootTableFile.build_script +
     LootTable.build_script +
     LootTableItemField.build_script +
     LootTableItemSpawnEggReferenceField.build_script +
     LootTableLootTableField.build_script
 )
 
 def load_loot_tables(db: Connection, rp_id: int):
+    '''
+    Loads all loot tables from the behavior pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM BehaviorPack WHERE BehaviorPack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for loot_table_path in (rp_path / "loot_tables").rglob("*.json"):
         load_loot_table(db, loot_table_path, rp_path, rp_id)
 
 def load_loot_table(
         db: Connection, loot_table_path: Path, rp_path: Path, rp_id: int):
+    '''
+    Loads a single loot table from the behavior pack.
+    '''
     cursor = db.cursor()
     # LOOT TABLE FILE
     cursor.execute(
         "INSERT INTO LootTableFile (path, BehaviorPack_fk) VALUES (?, ?)",
         (loot_table_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
@@ -110,85 +117,95 @@
         INSERT INTO LootTable (
             identifier, LootTableFile_fk
         ) VALUES (?, ?)
         ''',
         (identifier, file_pk)
     )
     loot_table_pk = cursor.lastrowid
+    loot_table_pk = cast(int, loot_table_pk)
 
     # LOOT TABLE ITEM & LOOT TABLE FIELDS
     entry_walker = loot_table_jsonc / "pools" // int / "entries" // int
     while len(entry_walker) > 0:
         for ew in entry_walker:
-            ew_name = ew / "name"
-            if not isinstance(ew_name.data, str):
-                continue
-            entry_name = ew_name.data
-            ew_type = ew / "type"
-            if ew_type.data == "item":
-                # ITEM
-                cursor.execute(
-                    '''
-                    INSERT INTO LootTableItemField (
-                        identifier, jsonPath, LootTable_fk
-                    ) VALUES (?, ?, ?)
-                    ''',
-                    (entry_name, ew_name.path_str, loot_table_pk)
+            _load_loot_table_or_loot_table_item_field(
+                ew, cursor, loot_table_pk)
+        # Entry property can have pools. This is a nested structure.
+        entry_walker = entry_walker / "pools" // int / "entries" // int
+
+
+def _load_loot_table_or_loot_table_item_field(
+        ew: JSONWalker, cursor: Cursor, loot_table_pk: int):
+    '''
+    Helper function for load_loot_table to reduce nesting.
+    '''
+    ew_name = ew / "name"
+    if not isinstance(ew_name.data, str):
+        return
+    entry_name = ew_name.data
+    ew_type = ew / "type"
+    if ew_type.data == "item":
+        # ITEM
+        cursor.execute(
+            '''
+            INSERT INTO LootTableItemField (
+                identifier, jsonPath, LootTable_fk
+            ) VALUES (?, ?, ?)
+            ''',
+            (entry_name, ew_name.path_str, loot_table_pk)
+        )
+        item_pk = cursor.lastrowid
+        # ITEM SPAWN EGG REFERENCE
+        if entry_name.endswith("_spawn_egg"):
+            # DIRECT REFERENCE
+            cursor.execute(
+                '''
+                INSERT INTO LootTableItemSpawnEggReferenceField (
+                    entityIdentifier, spawnEggIdentifier,
+                    connectionType, jsonPath, LootTableItemField_fk
+                ) VALUES (?, ?, ?, ?, ?)
+                ''',
+                (
+                    entry_name[:-10],  # remove "_spawn_egg"
+                    entry_name,
+                    "direct",
+                    ew_name.path_str,
+                    item_pk,
                 )
-                item_pk = cursor.lastrowid
-                # ITEM SPAWN EGG REFERENCE
-                if entry_name.endswith("_spawn_egg"):
-                    # DIRECT REFERENCE
-                    cursor.execute(
-                        '''
-                        INSERT INTO LootTableItemSpawnEggReferenceField (
-                            entityIdentifier, spawnEggIdentifier,
-                            connectionType, jsonPath, LootTableItemField_fk
-                        ) VALUES (?, ?, ?, ?, ?)
-                        ''',
-                        (
-                            entry_name[:-10],  # remove "_spawn_egg"
-                            entry_name,
-                            "direct",
-                            ew_name.path_str,
-                            item_pk,
-                        )
-                    )
-                elif entry_name == 'minecraft:spawn_egg':
-                    # REFERENCE USING set_actor_id FUNCTION
-                    functions_walker = ew / "functions" // int
-                    for fw in functions_walker:
-                        function_name = fw / "function"
-                        if not (
-                                isinstance(function_name.data, str) and 
-                                function_name.data == "set_actor_id"):
-                            continue
-                        entity_identifier = fw / "id"
-                        if not isinstance(entity_identifier.data, str):
-                            continue
-                        cursor.execute(
-                            '''
-                            INSERT INTO LootTableItemSpawnEggReferenceField (
-                                entityIdentifier, spawnEggIdentifier,
-                                connectionType, jsonPath, LootTableItemField_fk
-                            ) VALUES (?, ?, ?, ?, ?)
-                            ''',
-                            (
-                                entity_identifier.data,
-                                entity_identifier.data + "_spawn_egg",
-                                "set_actor_id_function",
-                                fw.path_str,
-                                item_pk,
-                            )
-                        )
-            elif ew_type.data == "loot_table":
-                # LOOT TABLE
+            )
+        elif entry_name == 'minecraft:spawn_egg':
+            # REFERENCE USING set_actor_id FUNCTION
+            functions_walker = ew / "functions" // int
+            for fw in functions_walker:
+                function_name = fw / "function"
+                if not (
+                        isinstance(function_name.data, str) and
+                        function_name.data == "set_actor_id"):
+                    continue
+                entity_identifier = fw / "id"
+                if not isinstance(entity_identifier.data, str):
+                    continue
                 cursor.execute(
                     '''
-                    INSERT INTO LootTableLootTableField (
-                        identifier, jsonPath, LootTable_fk
-                    ) VALUES (?, ?, ?)
+                    INSERT INTO LootTableItemSpawnEggReferenceField (
+                        entityIdentifier, spawnEggIdentifier,
+                        connectionType, jsonPath, LootTableItemField_fk
+                    ) VALUES (?, ?, ?, ?, ?)
                     ''',
-                    (entry_name, ew_name.path_str, loot_table_pk)
+                    (
+                        entity_identifier.data,
+                        entity_identifier.data + "_spawn_egg",
+                        "set_actor_id_function",
+                        fw.path_str,
+                        item_pk,
+                    )
                 )
-        # Entry property can have pools. This is a nested structure.
-        entry_walker = entry_walker / "pools" // int / "entries" // int
+    elif ew_type.data == "loot_table":
+        # LOOT TABLE
+        cursor.execute(
+            '''
+            INSERT INTO LootTableLootTableField (
+                identifier, jsonPath, LootTable_fk
+            ) VALUES (?, ?, ?)
+            ''',
+            (entry_name, ew_name.path_str, loot_table_pk)
+        )
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_particle.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_particle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
-from .better_json_tools import load_jsonc
-from ._views import dbtableview
 import json
+from .better_json_tools import load_jsonc
+from ._views import dbtableview, WeakTableConnection
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
@@ -16,34 +17,40 @@
     properties={
         "identifier": (str, "NOT NULL"),
         "material": (str, ""),
         "texture": (str, "")
     },
     connects_to=["ParticleFile"],
     weak_connects_to=[
-        ("texture", "TextureFile", "identifier")
+        WeakTableConnection("texture", "TextureFile", "identifier")
     ]
 )
 class Particle: ...
 
-PARTICLE_BUILD_SCRIPT = (
+PARTICLE_BUILD_SCRIPT: str = (
     ParticleFile.build_script +
     Particle.build_script
 )
 
 def load_particles(db: Connection, rp_id: int):
+    '''
+    Loads all particles from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for particle_path in (rp_path / "particles").rglob("*.json"):
         load_particle(db, particle_path, rp_id)
 
 def load_particle(db: Connection, particle_path: Path, rp_id: int):
+    '''
+    Loads a particle from the resource pack.
+    '''
     cursor = db.cursor()
     # PARTICLE FILE
     cursor.execute(
         "INSERT INTO ParticleFile (path, ResourcePack_fk) VALUES (?, ?)",
         (particle_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_render_controller.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_render_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import cast
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
+from typing import cast, Literal, NamedTuple
 from collections import defaultdict
 from sqlite3 import Connection
 from pathlib import Path
-from typing import Literal, NamedTuple
 from copy import copy
 import json
 
 from ._views import dbtableview
 from .better_json_tools import JSONWalker, load_jsonc
 from .utils import find_molang_resources
 
@@ -68,23 +68,26 @@
         "shortName": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["RenderController"]
 )
 class RenderControllerGeometryField: ...
 
-RENDER_CONTROLLER_BUILD_SCRIPT = (
+RENDER_CONTROLLER_BUILD_SCRIPT: str = (
     RenderControllerFile.build_script +
     RenderController.build_script +
     RenderControllerTexturesField.build_script +
     RenderControllerMaterialsField.build_script +
     RenderControllerGeometryField.build_script
 )
 
 def load_render_controllers(db: Connection, rp_id: int):
+    '''
+    Loads all render controllers from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for geometry_path in (rp_path / "render_controllers").rglob("*.json"):
         load_render_controller(db, geometry_path, rp_id)
@@ -108,15 +111,15 @@
         array_path = rc / "arrays" / "geometries" // str // int
     elif array_type == "material":
         array_path = rc / "arrays" / "materials" // str // int
     elif array_type == "texture":
         array_path = rc / "arrays" / "textures" // str // int
     else:
         raise ValueError(f"Invalid array type {array_type}")
-    result = defaultdict(list)
+    result: dict[str, list[_LoadRcArraysItem]] = defaultdict(list)
     for obj in array_path:
         if not isinstance(obj.data, str):
             continue
         array_name = cast(str, obj.parent.parent_key)
         array_name = array_name.lower()
         if not array_name.startswith("array."):
             continue
@@ -124,14 +127,17 @@
         values = find_molang_resources(obj.data, [array_type])[array_type]
         path_str = obj.path_str
         result[array_name].extend(
             [_LoadRcArraysItem(v, path_str) for v in values])
     return dict(result)
 
 def load_render_controller(db: Connection, entity_path: Path, rp_id: int):
+    '''
+    Loads a render controller from the resource pack.
+    '''
     cursor = db.cursor()
     # RENDER CONTROLLER FILE
     cursor.execute(
         "INSERT INTO RenderControllerFile (path, ResourcePack_fk) VALUES (?, ?)",
         (entity_path.as_posix(), rp_id))
     file_pk = cursor.lastrowid
     try:
@@ -226,15 +232,15 @@
                             material_reference.short_name,
                             field.path_str,
                             array_name,
                             material_reference.json_path,
                             pattern
                         )
                     )
-                    
+
         # LOAD GEOMETRIES
         geo_arrays = _load_rc_arrays(rc, "geometry")
         field = rc / "geometry"
         if isinstance(field.data, str):
             values = find_molang_resources(field.data, ["geometry", "array"])
             # Direct access
             for short_name in copy(values["geometry"]):
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_rp_animation.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_rp_animation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from typing import cast
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
 from ._views import dbtableview
-import json
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
@@ -36,31 +37,37 @@
         "shortName": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["RpAnimation"]
 )
 class RpAnimationSoundEffect: ...
 
-RP_ANIMATION_BUILD_SCRIPT = (
+RP_ANIMATION_BUILD_SCRIPT: str = (
     RpAnimationFile.build_script +
     RpAnimation.build_script +
     RpAnimationParticleEffect.build_script +
     RpAnimationSoundEffect.build_script
 )
 
 def load_rp_animations(db: Connection, rp_id: int):
+    '''
+    Loads all animations from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for animation_path in (rp_path / "animations").rglob("*.json"):
         load_rp_animation(db, animation_path, rp_id)
 
 def load_rp_animation(db: Connection, animation_path: Path, rp_id: int):
+    '''
+    Loads an animation from the resource pack.
+    '''
     cursor = db.cursor()
     # RP ANIMATION FILE
     cursor.execute(
         "INSERT INTO RpAnimationFile (path, ResourcePack_fk) VALUES (?, ?)",
         (animation_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
@@ -106,8 +113,7 @@
                 '''
                 INSERT INTO RpAnimationSoundEffect (
                     RpAnimation_fk, shortName, jsonPath
                 ) VALUES (?, ?, ?)
                 ''',
                 (rpanim_pk, short_name.data, sound_effect_walker.path_str)
             )
-
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_rp_animation_controller.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_rp_animation_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from typing import cast
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
 from ._views import dbtableview
-import json
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
@@ -36,32 +37,38 @@
         "shortName": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["RpAnimationController"]
 )
 class RpAnimationControllerSoundEffect: ...
 
-RP_ANIMATION_CONTROLLER_BUILD_SCRIPT = (
+RP_ANIMATION_CONTROLLER_BUILD_SCRIPT: str = (
     RpAnimationControllerFile.build_script +
     RpAnimationController.build_script +
     RpAnimationControllerParticleEffect.build_script +
     RpAnimationControllerSoundEffect.build_script
 )
 
 def load_rp_animation_controllers(db: Connection, rp_id: int):
+    '''
+    Loads all animation controllers from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for ac_path in (rp_path / "animation_controllers").rglob("*.json"):
         load_rp_animation_controller(db, ac_path, rp_id)
 
 
 def load_rp_animation_controller(db: Connection, animation_controller_path: Path, rp_id: int):
+    '''
+    Loads an animation controller from the resource pack.
+    '''
     cursor = db.cursor()
     # RP ANIMATION FILE
     cursor.execute(
         "INSERT INTO RpAnimationControllerFile (path, ResourcePack_fk) VALUES (?, ?)",
         (animation_controller_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_rp_item.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_rp_item.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import cast, Optional
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
+from typing import Optional
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
-from .utils import parse_format_version
 from ._views import dbtableview
-import json
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
@@ -19,29 +19,35 @@
         "identifier": (str, "NOT NULL"),
         "icon": (str, "")
     },
     connects_to=["RpItemFile"]
 )
 class RpItem: ...
 
-RP_ITEM_BUILD_SCRIPT = (
+RP_ITEM_BUILD_SCRIPT: str = (
     RpItemFile.build_script +
     RpItem.build_script
 )
 
 def load_rp_items(db: Connection, rp_id: int):
+    '''
+    Loads all items from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for item_path in (rp_path / "items").rglob("*.json"):
         load_rp_item(db, item_path, rp_id)
 
 def load_rp_item(db: Connection, item_path: Path, rp_id: int):
+    '''
+    Loads an item from the resource pack.
+    '''
     cursor = db.cursor()
     # RP ITEM FILE
     cursor.execute(
         "INSERT INTO RpItemFile (path, ResourcePack_fk) VALUES (?, ?)",
         (item_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_sound.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_sound.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
 from ._views import dbtableview
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL"),
@@ -10,37 +11,43 @@
         # make searches easier.
         "identifier": (str, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
 class SoundFile: ...
 
-SOUND_BUILD_SCRIPT = SoundFile.build_script
+SOUND_BUILD_SCRIPT: str = SoundFile.build_script
 
 def load_sounds(db: Connection, rp_id: int):
+    '''
+    Loads all sounds from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for sound_path in (rp_path / "sounds").rglob("*.wav"):
         load_sound(db, sound_path, rp_path, rp_id)
     for sound_path in (rp_path / "sounds").rglob("*.ogg"):
         load_sound(db, sound_path, rp_path, rp_id)
     for sound_path in (rp_path / "sounds").rglob("*.fsb"):
         load_sound(db, sound_path, rp_path, rp_id)
 
 def load_sound(db: Connection, sound_path: Path, rp_path: Path, rp_id: int):
+    '''
+    Loads a sound from the resource pack.
+    '''
     cursor = db.cursor()
     # SOUND FILE AND ITS IDENTIFIER
     cursor.execute(
         """
         INSERT INTO SoundFile (
             path, identifier, ResourcePack_fk
         ) VALUES (?, ?, ?)
         """,
         (
             sound_path.as_posix(),
             sound_path.relative_to(rp_path).with_suffix("").as_posix(),
             rp_id
         )
-    )
+    )
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_sound_definitions.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_sound_definitions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import cast, Optional
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
+from typing import cast
 from sqlite3 import Connection
 from pathlib import Path
-from .better_json_tools import load_jsonc
-from ._views import dbtableview
 import json
+from .better_json_tools import load_jsonc
+from ._views import dbtableview, WeakTableConnection
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
@@ -25,37 +26,43 @@
 @dbtableview(
     properties={
         "identifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["SoundDefinition"],
     weak_connects_to=[
-        ("identifier", "SoundFile", "identifier")
+        WeakTableConnection("identifier", "SoundFile", "identifier")
     ]
 )
 class SoundDefinitionSoundField: ...
 
-SOUND_DEFINITIONS_BUILD_SCRIPT = (
+SOUND_DEFINITIONS_BUILD_SCRIPT: str = (
     SoundDefinitionsFile.build_script +
     SoundDefinition.build_script +
     SoundDefinitionSoundField.build_script
 )
 
 def load_sound_definitions(db: Connection, rp_id: int):
+    '''
+    Loads all sound definitions from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     sound_definitions_path = rp_path / "sounds" / "sound_definitions.json"
     if sound_definitions_path.exists():
         load_sound_definition(db, sound_definitions_path, rp_id)
 
 
 def load_sound_definition(db: Connection, sound_definition_path: Path, rp_id: int):
+    '''
+    Loads a sound definition from the resource pack.
+    '''
     cursor = db.cursor()
     # GEOMETRY FILE
     cursor.execute(
         "INSERT INTO SoundDefinitionsFile (path, ResourcePack_fk) VALUES (?, ?)",
         (sound_definition_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_terrain_texture.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_terrain_texture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import cast, Optional, NamedTuple
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
+from typing import cast, Optional, NamedTuple, Iterator, TYPE_CHECKING
 from sqlite3 import Connection
 from pathlib import Path
-from .better_json_tools import load_jsonc, JSONWalker
-from ._views import dbtableview
 import json
+from .better_json_tools import load_jsonc, JSONWalker
+from ._views import dbtableview, WeakTableConnection
 
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["ResourcePack"]
@@ -31,15 +32,15 @@
         "variationIndex": (int, ""),  # For convinience (could be deduced from the path)
         "weight": (int, ""),  # Only makes sense if the texture is a variation
         "tintColor": (str, ""),
         "overlayColor": (str, ""),
     },
     connects_to=["TerrainTexture"],
     weak_connects_to=[
-        ("identifier", "TextureFile", "identifier")
+        WeakTableConnection("identifier", "TextureFile", "identifier")
     ]
 )
 class TerrainTextureVariation:
     '''
     Represents a singl file path mentioned in the terrain_texture.json file.
 
     It is called "variation" because in the most deeply nested configuration
@@ -56,32 +57,38 @@
     - root.textures.<identifier>.textures[<variant_index>].path
     - root.textures.<identifier>.textures[<variant_index>].
         variations[variation_index]
     - root.textures.<identifier>.textures[<variant_index>].
         variations[variation_index].path
     '''
 
-TERRAIN_TEXTURE_BUILD_SCRIPT = (
+TERRAIN_TEXTURE_BUILD_SCRIPT: str = (
     TerrainTextureFile.build_script +
     TerrainTexture.build_script +
     TerrainTextureVariation.build_script
 )
 
 def load_terrain_texture(db: Connection, rp_id: int):
+    '''
+    Loads the terrain_texture.json file from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     terrain_texture_path = rp_path / "textures" / "terrain_texture.json"
     if not terrain_texture_path.exists():
         return
     load_terrain_texture_items(db, terrain_texture_path, rp_id)
 
 def load_terrain_texture_items(db: Connection, terrain_texture_path: Path, rp_id: int):
+    '''
+    Loads all terrain textures from the terrain_texture.json file.
+    '''
     cursor = db.cursor()
     # TERRAIN TEXTURE FILE
     cursor.execute(
         "INSERT INTO TerrainTextureFile (path, ResourcePack_fk) VALUES (?, ?)",
         (terrain_texture_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
@@ -113,14 +120,15 @@
         else:
             cursor.execute(
                 "INSERT INTO TerrainTexture "
                 "(identifier, TerrainTextureFile_fk) VALUES (?, ?)",
                 (terrain_texture_identifier, file_pk)
             )
             terrain_texture_pk = cursor.lastrowid
+            terrain_texture_pk = cast(int, terrain_texture_pk)
             inserted_textures[terrain_texture_identifier] = terrain_texture_pk
 
         cursor.execute(
             "INSERT INTO TerrainTextureVariation "
             "(identifier, jsonPath, variantIndex, variationIndex, weight, "
             "tintColor, overlayColor, TerrainTexture_fk) "
             "VALUES (?, ?, ?, ?, ?, ?, ?, ?)",
@@ -145,14 +153,17 @@
                 terrain_texture_identifier=identifier,
                 identifier=textures_walker.data,
                 json_path=textures_walker.path_str)
         elif isinstance(textures_walker.data, list):
             for variant_walker, variant_index, variant_data in _yield_variants(
                     textures_walker):
                 if variant_data.is_variation:
+                    if TYPE_CHECKING:  # We know that from is_variation.
+                        assert isinstance(variant_data.path, str)
+                        assert isinstance(variant_data.json_path, str)
                     _insert_terrain_texture_variation(
                        terrain_texture_identifier=identifier,
                        identifier=variant_data.path,
                        json_path=variant_data.json_path,
                        variant_index=variant_index,
                        tint_color=variant_data.tint_color,
                        overlay_color=variant_data.overlay_color)
@@ -172,14 +183,17 @@
                     )
         elif isinstance(textures_walker.data, dict):
             try:
                 variant_data = _get_variant_data(textures_walker)
             except ValueError:
                 return
             if variant_data.is_variation:
+                if TYPE_CHECKING:  # We know that from is_variation.
+                    assert isinstance(variant_data.path, str)
+                    assert isinstance(variant_data.json_path, str)
                 _insert_terrain_texture_variation(
                     terrain_texture_identifier=identifier,
                     identifier=variant_data.path,
                     json_path=variant_data.json_path,
                     tint_color=variant_data.tint_color,
                     overlay_color=variant_data.overlay_color)
             else:
@@ -230,17 +244,20 @@
     path: Optional[str]
     json_path: Optional[str]
     tint_color: Optional[str]
     overlay_color: Optional[str]
 
     @property
     def is_variation(self) -> bool:
+        '''
+        Whether this variant is a variation or variations are nested inside.
+        '''
         return self.path is not None
 
-def _yield_variations(variant_walker: JSONWalker) -> tuple[int, _VariationData]:
+def _yield_variations(variant_walker: JSONWalker) -> Iterator[tuple[int, _VariationData]]:
     '''
     Yields the variation data from the JSONWalker that represents a variant.
     '''
     for variation_walker in variant_walker / "variations" // int:
         variation_index = variation_walker.parent_key
         variation_index = cast(int, variation_index)
         try:
@@ -274,15 +291,17 @@
     tint_color_walker = variant_walker / "tint_color"
     tint_color = None
     if tint_color_walker.exists and isinstance(tint_color_walker.data, str):
         tint_color = tint_color_walker.data
     return _VariantData(
         path, json_path, tint_color, overlay_color)
 
-def _yield_variants(variant_list_walker: JSONWalker) -> tuple[int, _VariantData]:
+def _yield_variants(
+    variant_list_walker: JSONWalker
+) -> Iterator[tuple[JSONWalker, int, _VariantData]]:
     '''
     Yields the variant data from the JSONWalker that represents a variant list.
     '''
     for variant_walker in variant_list_walker // int:
         variant_index = variant_walker.parent_key
         variant_index = cast(int, variant_index)
         try:
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_texture.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_texture.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
 from ._views import dbtableview
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL"),
@@ -10,37 +11,43 @@
         # make searches easier.
         "identifier": (str, "NOT NULL")
     },
     connects_to=["ResourcePack"]
 )
 class TextureFile: ...
 
-TEXTURE_BUILD_SCRIPT = TextureFile.build_script
+TEXTURE_BUILD_SCRIPT: str = TextureFile.build_script
 
 def load_textures(db: Connection, rp_id: int):
+    '''
+    Loads all textures from the resource pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM ResourcePack WHERE ResourcePack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for texture_path in (rp_path / "textures").rglob("*.png"):
         load_texture(db, texture_path, rp_path, rp_id)
     for texture_path in (rp_path / "textures").rglob("*.tga"):
         load_texture(db, texture_path, rp_path, rp_id)
     for texture_path in (rp_path / "textures").rglob("*.jpg"):
         load_texture(db, texture_path, rp_path, rp_id)
 
 def load_texture(db: Connection, texture_path: Path, rp_path: Path, rp_id: int):
+    '''
+    Loads a texture from the resource pack.
+    '''
     cursor = db.cursor()
     # TEXTURE FILE AND ITS IDENTIFIER
     cursor.execute(
         """
         INSERT INTO TextureFile (
             path, identifier, ResourcePack_fk
         ) VALUES (?, ?, ?)
         """,
         (
             texture_path.as_posix(),
             texture_path.relative_to(rp_path).with_suffix("").as_posix(),
             rp_id
         )
-    )
+    )
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_db_trade_table.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_db_trade_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import cast, Optional
+# pylint: disable=no-member, multiple-statements, missing-module-docstring, missing-class-docstring
 from sqlite3 import Connection
 from pathlib import Path
+import json
 from .better_json_tools import load_jsonc
 from .utils import split_item_name
-from ._views import dbtableview
-import json
+from ._views import dbtableview, WeakTableConnection
 
 @dbtableview(
     properties={
         "path": (Path, "NOT NULL")
     },
     connects_to=["BehaviorPack"]
 )
@@ -29,51 +29,57 @@
     properties={
         "identifier": (str, "NOT NULL"),
         "dataValue": (int, ""),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["TradeTable"],
     weak_connects_to=[
-        ("identifier", "RpItem", "identifier"),
-        ("identifier", "BpItem", "identifier")
+        WeakTableConnection("identifier", "RpItem", "identifier"),
+        WeakTableConnection("identifier", "BpItem", "identifier")
     ]
 )
 class TradeTableItemField: ...
 
 @dbtableview(
     properties={
         "entityIdentifier": (str, "NOT NULL"),
         "spawnEggIdentifier": (str, "NOT NULL"),
         "jsonPath": (str, "NOT NULL")
     },
     connects_to=["TradeTableItemField"],
     weak_connects_to=[
-        ("spawnEggIdentifier", "EntitySpawnEggField", "identifier")
+        WeakTableConnection("spawnEggIdentifier", "EntitySpawnEggField", "identifier")
     ]
 )
 class TradeTableItemSpawnEggReferenceField: ...
 
-TRADE_TABLE_BUILD_SCRIPT = (
+TRADE_TABLE_BUILD_SCRIPT: str = (
     TradeTableFile.build_script +
     TradeTable.build_script +
     TradeTableItemField.build_script +
     TradeTableItemSpawnEggReferenceField.build_script
 )
 
 def load_trade_tables(db: Connection, rp_id: int):
+    '''
+    Loads all trade tables from the behavior pack.
+    '''
     rp_path: Path = db.execute(
         "SELECT path FROM BehaviorPack WHERE BehaviorPack_pk = ?",
         (rp_id,)
     ).fetchone()[0]
 
     for trade_table_path in (rp_path / "trading").rglob("*.json"):
         load_trade_table(db, trade_table_path, rp_path, rp_id)
 
 def load_trade_table(
         db: Connection, trade_table_path: Path, rp_path: Path, rp_id: int):
+    '''
+    Loads a trade table from the behavior pack.
+    '''
     cursor = db.cursor()
     # LOOT TABLE FILE
     cursor.execute(
         "INSERT INTO TradeTableFile (path, BehaviorPack_fk) VALUES (?, ?)",
         (trade_table_path.as_posix(), rp_id)
     )
     file_pk = cursor.lastrowid
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/_views.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 '''
 This file contains the decorators that create the view classes for the tables
 of the database.
 '''
+# pylint: disable=protected-access
 
 from __future__ import annotations
-from typing import Literal, Callable
+from typing import Literal, NamedTuple, Any, TYPE_CHECKING
 from pathlib import Path
-from collections import namedtuple
-from typing import NamedTuple
 from abc import ABC
-from textwrap import dedent
 import sqlite3
 
 _SUPPORTED_TYPES = {
     Path: "Path",
     str: "TEXT",
     int: "INTEGER",
 }
@@ -21,15 +19,15 @@
 class _TableConnection(NamedTuple):
     columns: tuple[str, str]
     '''The pair of collumn names (this table column, other table column).'''
 
     is_pk: bool
     '''Whether the connection is referencing a primary key of other table.'''
 
-class _WeakTableConnection(NamedTuple):
+class WeakTableConnection(NamedTuple):
     '''
     Used for type annotation in the 'dbtableview' decorator for
     weak_connects_to argument.
     '''
     this_table_column_name: str
     other_table_name: str
     other_table_column_name: str
@@ -74,125 +72,128 @@
     reverse connections to the relation map.
     '''
     for this_table, v in RELATION_MAP.items():
         for other_table, v2 in v.items():
             if this_table not in RELATION_MAP[other_table]:
                 RELATION_MAP[other_table][this_table] = _TableConnection(
                     columns=(v2.columns[1], v2.columns[0]),
-                    is_pk=RELATION_MAP[this_table][other_table].is_pk
+                    is_pk=v[other_table].is_pk
                 )
 
 
 class AbstractDBView(ABC):
     '''
     This abstract class is used in the PYI files as a parent of all of
     the wrapped classes.
     '''
+    if TYPE_CHECKING:
+        __name__: str
+        build_script: str
 
 class _DbTableView:
     '''
     Used for dbtableview decorator. For more information see the decorator
     documentation.
     '''
     def __init__(
             self,
             cls: type,
             properties: dict[str, tuple[type,Literal["NOT NULL", ""]]],
             enum_properties: dict[str, list[str]],
             connects_to: list[str],
-            weak_connects_to: list[_WeakTableConnection]):
+            weak_connects_to: list[WeakTableConnection]):
         # VALIDATE THE PARAMETERS
         # Properties
-        if not isinstance(properties, dict):
+        if not isinstance(properties, dict):  # pyright: ignore[reportUnnecessaryIsInstance]
             raise TypeError("The 'properties' parameter must be a dict")
         for name, value in properties.items():
-            if not isinstance(name, str):
+            if not isinstance(name, str):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The keys of the 'properties' parameter must be strings")
             if not name.isidentifier():
                 raise ValueError(
                     f"The key '{name}' of the 'properties' parameter is not a "
                     "valid identifier")
-            if not isinstance(value, tuple):
+            if not isinstance(value, tuple):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The values of the 'properties' parameter must be tuples")
             if len(value) != 2:
                 raise ValueError(
                     "The values of the 'properties' parameter must be tuples "
                     "of length 2")
             if not isinstance(value[0], type):
                 raise TypeError(
                     "The first value of the tuples of the 'properties' "
                     "parameter must be a type")
             if value[0] not in _SUPPORTED_TYPES:
                 raise ValueError(
                     f"The type {value[0]} is not supported by the decorator")
         # Enum properties
-        if not isinstance(enum_properties, dict):
+        if not isinstance(enum_properties, dict):  # pyright: ignore[reportUnnecessaryIsInstance]
             raise TypeError("The 'enum_properties' parameter must be a dict")
         for name, value in enum_properties.items():
-            if not isinstance(name, str):
+            if not isinstance(name, str):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The keys of the 'enum_properties' parameter must be "
                     "strings")
             if not name.isidentifier():
                 raise ValueError(
                     f"The key '{name}' of the 'enum_properties' parameter is "
                     "not a valid identifier")
-            if not isinstance(value, list):
+            if not isinstance(value, list):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The values of the 'enum_properties' parameter must be "
                     "lists")
             for item in value:
-                if not isinstance(item, str):
+                if not isinstance(item, str):  # pyright: ignore[reportUnnecessaryIsInstance]
                     raise TypeError(
                         "The values of the lists of the 'enum_properties' "
                         "parameter must be strings")
         # Connects to
-        if not isinstance(connects_to, list):
+        if not isinstance(connects_to, list):  # pyright: ignore[reportUnnecessaryIsInstance]
             raise TypeError(
                 "The 'connects_to' parameter must be a list of strings")
         for name in connects_to:
-            if not isinstance(name, str):
+            if not isinstance(name, str):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The 'connects_to' parameter must be a list of strings")
             if not name.isidentifier():
                 raise ValueError(
                     f"The value '{name}' of the 'connects_to' parameter is not "
                     "a valid identifier")
         # Weak connects to
-        if not isinstance(weak_connects_to, list):
+        if not isinstance(weak_connects_to, list):  # pyright: ignore[reportUnnecessaryIsInstance]
             raise TypeError(
                 "The 'weak_connects_to' parameter must be a list of tuples")
         for item in weak_connects_to:
-            if not isinstance(item, tuple):
+            if not isinstance(item, tuple):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The 'weak_connects_to' parameter must be a list of "
                     "tuples")
             if len(item) != 3:
                 raise ValueError(
                     "The tuples of the 'weak_connects_to' parameter must be "
                     "of length 3")
-            if not isinstance(item[0], str):
+            if not isinstance(item[0], str):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The first value of the tuples of the 'weak_connects_to' "
                     "parameter must be a string")
             if not item[0].isidentifier():
                 raise ValueError(
                     f"The first value '{item[0]}' of the tuples of the "
                     "'weak_connects_to' parameter is not a valid identifier")
-            if not isinstance(item[1], str):
+            if not isinstance(item[1], str):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The second value of the tuples of the "
                     "'weak_connects_to' parameter must be a string")
             if not item[1].isidentifier():
                 raise ValueError(
                     f"The second value '{item[1]}' of the tuples of the "
                     "'weak_connects_to' parameter is not a valid identifier")
-            if not isinstance(item[2], str):
+            if not isinstance(item[2], str):  # pyright: ignore[reportUnnecessaryIsInstance]
                 raise TypeError(
                     "The third value of the tuples of the "
                     "'weak_connects_to' parameter must be a string")
             if not item[2].isidentifier():
                 raise ValueError(
                     f"The third value '{item[2]}' of the tuples of the "
                     "'weak_connects_to' parameter is not a valid identifier")
@@ -279,16 +280,16 @@
         '''
         build_script_lines: list[str] = []
         # If there are enum properties, build the enum tables
         for name, values in self.enum_properties.items():
             table_name = f"{self.cls.__name__}{name.capitalize()}Enum"
             build_script_lines.extend([
                 f"CREATE TABLE {table_name} (",
-                f"    value TEXT PRIMARY KEY",
-                f");"
+                "    value TEXT PRIMARY KEY",
+                ");"
             ])
             for value in values:
                 build_script_lines.append(
                     f"INSERT INTO {table_name} (value) VALUES ('{value}');")
         # Start defining the main table
         build_script_lines.append(f"CREATE TABLE {self.cls.__name__} (")
         # Internal lines of the class are later indented and connected with commans
@@ -331,32 +332,32 @@
         build_script = "\n".join(build_script_lines) + "\n"
         return build_script
 
     def generate_init(self):
         '''
         Creates the init method of the class.
         '''
-        def init(self_, connection: sqlite3.Connection, id: int):
-            self_._connection: sqlite3.Connection = connection
-            self_._id: int = id
+        def init(self_: Any, connection: sqlite3.Connection, id_: int):
+            self_._connection = connection
+            self_._id = id_
             self_._query_result_cache = None
         init.__qualname__ = f"{self.cls.__name__}.__init__"
         return init
 
     def generate_query_result(self):
         '''
         Creates the query_result method of the class.
         '''
         _query_result_columns = ", ".join(
             [f"{name}_fk" for name in self.connects_to] +
-            [name for name in self.properties] +
-            [name for name in self.enum_properties]
+            list(self.properties) +
+            list(self.enum_properties)
         )
 
-        def query_result(self_):
+        def query_result(self_: Any):
             if self_._query_result_cache is None:
                 self_._query_result_cache = self_.connection.execute(
                     f"SELECT {_query_result_columns} "
                     f"FROM {self.cls.__name__} "
                     f"WHERE {self.cls.__name__}_pk = ?",
                     (self_.id,)
                 ).fetchone()
@@ -364,45 +365,45 @@
         query_result.__qualname__ = f"{self.cls.__name__}.query_result"
         return query_result
 
     def generate_properties(self):
         '''
         Creates the @property decorated properties of the class.
         '''
-        properties = {}
+        properties: dict[str, Any] = {}
         # FOREIGN KEYS
         for i, name in enumerate(self.connects_to):
             @property
-            def property_method(self, /, _i=i) -> int:
+            def fk_prop_method(self: Any, /, _i: int=i) -> int:
                 return self.query_result()[_i]
-            properties[f"{name}_fk"] = property_method
+            properties[f"{name}_fk"] = fk_prop_method
         # REGULAR PROPERTIES
-        for i, (name, (type_, _)) in enumerate(
+        for i, (name, (_, _)) in enumerate(
                 self.properties.items(),
                 start=len(self.connects_to)):
             @property
-            def property_method(self, /, _i=i) -> type_:
+            def prop_method(self: Any, /, _i: int=i) -> Any:  # pyright: ignore
                 return self.query_result()[_i]
-            properties[name] = property_method
+            properties[name] = prop_method
         # ENUM PROPERTIES
         for i, name in enumerate(
                 self.enum_properties,
                 start=len(self.connects_to) + len(self.properties)):
             @property
-            def property_method(self, /, _i=i) -> str:
+            def enum_prop_method(self: Any, /, _i: int = i) -> str:
                 return self.query_result()[_i]
-            properties[name] = property_method
+            properties[name] = enum_prop_method
         # ID and CONNECTION
         @property
-        def id_(self) -> int:
+        def id_(self: Any) -> int:
             return self._id
         properties["id"] = id_
 
         @property
-        def connection(self) -> sqlite3.Connection:
+        def connection(self: Any) -> sqlite3.Connection:
             return self._connection
         properties["connection"] = connection
         return properties
 
     def generate_annotations(self):
         '''
         Creates the __annotations__ attribute of the class.
@@ -421,36 +422,36 @@
         # Add the annotations of the enum properties
         for name in self.enum_properties:
             annotations_[name] = str
         # Add the annotations of the id and connection
         annotations_["id"] = int
         annotations_["connection"] = sqlite3.Connection
         # Add the annotations of the query_result method
-        annotations_["query_result"] = Callable[[], tuple]
+        annotations_["query_result"] = "Callable[[], tuple[Any, ...]]"
         # Add the annotations of the build_script method
         annotations_["build_script"] = str
         return annotations_
 
-    def __call__(self) -> type:
+    def __call__(self) -> AbstractDBView:
         # VALIDATE THE PARAMETERS
         self.assert_valid()
-        
+
         # BUILD THE SCRIPT
         build_script = self.generate_build_script()
 
         # BUILD THE CLASS
         init = self.generate_init()
         query_result = self.generate_query_result()
         properties = self.generate_properties()
         annotations_ = self.generate_annotations()
 
         # CREATE THE TYPE OBJECT
         result = type(
             self.cls.__name__,
-            tuple(),
+            (AbstractDBView,),
             {
                 "__init__": init,
                 "__doc__": f'{self.cls.__name__}(connection, id)',
                 "__slots__": ("_id", "_connection", "_query_result_cache"),
                 "__module__": "sqlite_bedrock_packs.views",
                 "__annotations__": annotations_,
                 "query_result": query_result,
@@ -461,21 +462,21 @@
                 for name, value in list(self.cls.__dict__.items())
                 if not (name.startswith("__") and name.endswith("__"))
             }
         )
         # REGISTER IN THE WRAPPER_CLASSES MAP
         WRAPPER_CLASSES[self.cls.__name__] = result
 
-        return result
+        return result  # type: ignore
 
 def dbtableview(
-        properties: dict[str, tuple[type, Literal["NOT NULL", ""]]] = None,
-        enum_properties: dict[str, list[str]] = None,
-        connects_to: list[str] = None,
-        weak_connects_to: list[_WeakTableConnection] = None,
+        properties: dict[str, tuple[type, Literal["NOT NULL", ""]]] | None = None,
+        enum_properties: dict[str, list[str]] | None = None,
+        connects_to: list[str] | None = None,
+        weak_connects_to: list[WeakTableConnection] | None = None,
 ):
     '''
     The "dbtableview" is a decorator that turns a class into a read-only view
     of a row in a table in the database. It also registers the class in the
     relation map and adds some attributes to the class.
 
     This decorator uses additional parameters, so in order to use it, you have
@@ -485,15 +486,15 @@
         @dbtable()
         class MyClassName: ...
 
     The decorator adds following properties properties:
 
     The constructor method takes 2 parameters - the Connection object to the
     database, and the ID of the row in the table.
-    
+
     Other parameters are not stored directly in the class and are accessed by
     querying the database. Accessing any of the properties runs a query, which
     gets all of the properties of the row at once. The results are cached to
     provide the data to any subsequent calls to the properties. Note that the
     cache is not invalidated if the data in the database changes.
 
     Running the query without accessing the properties can be forced by calling
@@ -511,15 +512,15 @@
         table that are enums. In the database, the enums are stored as separate
         tables that use their values as primary keys. The creation and
         population of the enum tables is added at the top of the
         'build_script'. The table that references the enum table has a property
         with a constraint that it can only contain values from the enum table.
     :param connects_to: A list of names of the other previously defined tables
         that this table has a foreign key to. The names of the foreign keys are
-        generated by the name of the table and the suffix '_fk'. If the 
+        generated by the name of the table and the suffix '_fk'. If the
         referenced table is not defined yet, the decorator will raise an
         exception.
     :param weak_connects_to: A list of connections to the other tables in the
         database. The tables don't need to be defined at the time of the
         decorator call. The weak connections don't have any effect on the
         database schema, but they are used to generate the "easy queries".
         Unlike the "connects_to" connections, the weak connections can connect
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/__init__.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,36 @@
+'''
+A collection of tools for working with JSON, JSONC files and
+JSON-like data structures.
+'''
 from pathlib import Path
 from typing import Union
 import json
 
-from .compact_encoder import CompactEncoder
-from .jsonc import JSONCDecoder
-from .json_walker import JSONWalker, JSONSplitWalker, SKIP_LIST, JSONPath
+from .compact_encoder import CompactEncoder as CompactEncoder
+from .jsonc import (
+    JSONCDecoder as JSONCDecoder
+)
+from .json_walker import (
+    JSONWalker as JSONWalker,
+    JSONSplitWalker as JSONSplitWalker,
+    SKIP_LIST as SKIP_LIST,
+    JSONPath as JSONPath
+)
 
-VERSION = (1, 0, 3)
+VERSION = (1, 0, 4)
 __version__ = '.'.join([str(x) for x in VERSION])
 
 
 def load_jsonc(jsonc_path: Union[Path, str]) -> JSONWalker:
     '''
     Loads JSONC file into a JSON walker object.
     '''
     if isinstance(jsonc_path, str):
         jsonc_path = Path(jsonc_path)
     try:
         with jsonc_path.open(encoding='utf8') as jsonc_file:
             data = json.load(jsonc_file)
-    except json.JSONDecodeError as err:
+    except json.JSONDecodeError:
         with jsonc_path.open(encoding='utf8') as jsonc_file:
             data = json.load(jsonc_file, cls=JSONCDecoder)
     return JSONWalker(data)
-
-
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/compact_encoder.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/compact_encoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,100 @@
+'''
+A module that provides a custom JSON encoder for JSON-like data structures,
+that is more compact than the default encoder but still readable.
+'''
+from typing import Any, TypeGuard, Union, Iterator, cast
 import json
 
 class CompactEncoder(json.JSONEncoder):
     '''
     JSONEncoder can be used as `cls` argument to `json.dump` and `json.dumps`.
     It creates formatted JSON strings, with indentation that are more compact
     than the dafault formatting from `json` module. The main difference is that
-    the lists of primitives are not split into multiple lines. 
+    the lists of primitives are not split into multiple lines.
     '''
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
-        self.indent = -1
-        self.respect_indent = True
+        self.__indent: int = -1
+        self.respect_indent: bool = True
 
-    def _is_primitive(self, obj):
+    def _is_primitive(self, obj: Any) -> TypeGuard[Union[int, bool, str, float]]:
         return isinstance(obj, (int, bool, str, float))
 
-    def encode(self, obj):
+    def encode(self, o: Any) -> str:
         '''
         Return a JSON string representation of a Python data structure.
 
         Example:
             >>> CompactEncoder().encode({"foo": ["bar", "baz"]})
             '{\\n\\t"foo": ["bar", "baz"]\\n}'
         '''
-        return ''.join([i for i in self.iterencode(obj)])
+        return ''.join(self.iterencode(o))
 
-    def iterencode(self, obj):
+    def iterencode(self, o: Any, *args: Any) -> Iterator[str]:
         '''
         Encode the given object and yield each string representation line by
         line.
 
         Example:
             >>> item = {"foo": ["bar", "baz"]}
             >>> ''.join(list(CompactEncoder().iterencode(item))) == \\
             ... CompactEncoder().encode(item)
             True
         '''
-        self.indent += 1
+        self.__indent += 1
         if self.respect_indent:
-            ind = self.indent*'\t'
+            ind = self.__indent*'\t'
         else:
             ind = ''
-        if isinstance(obj, dict):
-            if len(obj) == 0:
+        if isinstance(o, dict):
+            o = cast(dict[Any, Any], o)
+            if len(o) == 0:
                 yield f"{ind}{{}}"
             else:
-                body = []
-                for k, v in obj.items():
+                body: list[str] = []
+                for k, v in o.items():
                     body.extend([
-                        f'{j[:self.indent]}{json.dumps(k)}: {j[self.indent:]}'
+                        f'{j[:self.__indent]}{json.dumps(k)}: {j[self.__indent:]}'
                         for j in self.iterencode(v)
                     ])
                 body_str = ",\n".join(body)
                 yield (
                     f'{ind}{{\n'
                     f'{body_str}\n'
                     f'{ind}}}'
                 )
-        elif isinstance(obj, (list, tuple)):
+        elif isinstance(o, (list, tuple)):
+            o = cast(list[Any], o)
             primitive_list = True
-            for i in obj:
+            for i in o:
                 if not self._is_primitive(i):
                     primitive_list = False
                     break
             if primitive_list:
                 body = []
                 self.respect_indent = False
-                for i in obj:
-                    body.extend([j for j in self.iterencode(i)])
+                for i in o:
+                    body.extend(self.iterencode(i))
                 self.respect_indent = True
                 yield f'{ind}[{", ".join(body)}]'
             else:
                 body = []
-                for i in obj:
-                    body.extend([j for j in self.iterencode(i)])
+                for i in o:
+                    body.extend(self.iterencode(i))
                 body_str = ",\n".join(body)
                 yield (
                     f'{ind}[\n'
                     f'{body_str}\n'
                     f'{ind}]'
                 )
-        elif self._is_primitive(obj):
-            if isinstance(obj, str):
-                yield f'{ind}{json.dumps(obj)}'
+        elif self._is_primitive(o):
+            if isinstance(o, str):
+                yield f'{ind}{json.dumps(o)}'
             else:
-                yield f'{ind}{str(obj).lower()}'
-        elif obj is None:
+                yield f'{ind}{str(o).lower()}'
+        elif o is None:
             yield f'{ind}null'
         else:
             raise TypeError('Object of type set is not JSON serializable')
-        self.indent -= 1
+        self.__indent -= 1
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/json_walker.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/json_walker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+'''
+A module that provides tools for easy access to JSON data using JSON paths.
+'''
 from __future__ import annotations
 import json
 import re
-from typing import Union, Type, Optional, IO, Callable, Iterator
+from typing import Union, Type, Optional, IO, Callable, Iterator, Any
 
 class SKIP_LIST:
     '''Used as literal value for JSONSplitWalker paths'''
 
 # def _remove_escape_characters(text: str) -> str:
 #     '''Prints to a string, removint the escape characters'''
 #     with io.StringIO() as output:
 #         print(text, file=output, end='')
 #         contents = output.getvalue()
 #     return contents
 
 def _tuple_to_path_str(path: tuple[Union[str, int], ...]):
-    result = []
+    result: list[str] = []
     for k in path:
         if isinstance(k, int):
             result.append(f'[{k}]')
-        elif isinstance(k, str):
+        elif isinstance(k, str): # pyright: ignore[reportUnnecessaryIsInstance]
             if re.fullmatch("[a-zA-Z$_]+[a-zA-Z$_0-9]*", k):
                 # Mathes JS variable name (like connect like a.b.c)
                 if len(result) == 0:  # First item skip the dot
                     result.append(k)
                 else: # Add dot before
                     result.append(f".{k}")
             else:
@@ -40,15 +43,15 @@
     the keys, but they can be represented or created from a string. The string
     representation is similar to the one used in JavaScript.
 
     The path objects can be used to access the data of :class:`JSONWalker`.
 
     Example:
         >>> from better_json_tools import JSONPath
-        >>> path = JSONPath(("a", "$abc", 1, 2, 'with quote "')) 
+        >>> path = JSONPath(("a", "$abc", 1, 2, 'with quote "'))
         >>> print(path.data)
         ... ('a', '$abc', 1, 2, 'with quote "')
         >>> print(path)
         ... a.$abc[1][2]["with quote \""]
         >>> another_path = JSONPath(str(path))
         >>> print(another_path)
         ... a.$abc[1][2]["with quote \""]
@@ -68,15 +71,15 @@
     @staticmethod
     def _from_path_str(path_str: str) -> tuple[Union[str, int], ...]:
         '''Converts a path string to a JSONPath.'''
         if path_str == "":
             return tuple()
 
         # Results
-        path = []
+        path: list[int | str] = []
         curr_path = path_str
 
         # Add . to the start of the string to make the patterm matching work
         # better
         if not curr_path.startswith("["):
             curr_path = "." + curr_path
         while True:
@@ -107,19 +110,19 @@
                     path.append(int(match.group(1)))
                     curr_path = curr_path[match.end():]
             else:
                 raise ValueError(f"Invalid path: {path_str}")
         return tuple(path)
 
 ## Type definitions
-JSON = Union[dict, list, str, float, int, bool, None]
+JSON = Union[dict[str, Any], list[Any], str, float, int, bool, None]
 JSON_KEY = Union[str, int]
 JSON_PATH_KEY = Union[str, int, JSONPath]
 JSON_SPLIT_KEY = Union[str, Type[int], Type[str], None, Type[SKIP_LIST]]
-JSON_WALKER_DATA = Union[dict, list, str, float, int, bool, None, Exception]
+JSON_WALKER_DATA = Union[dict[str, Any], list[Any], str, float, int, bool, None, Exception]
 
 
 
 class JSONWalker:
     '''
     A class that represents a path in the JSON file for easy access to its
     values.
@@ -156,24 +159,24 @@
             object
         '''
         if self._parent_key is None:
             raise KeyError("You can't get parent of the root object.")
         return self._parent_key
 
     @staticmethod
-    def loads(json_text: Union[str, bytes], **kwargs) -> JSONWalker:
+    def loads(json_text: Union[str, bytes], **kwargs: Any) -> JSONWalker:
         '''
         Creates json walker using `json.loads()` function. Passes all arguments
         to `json.loads` and tries to creat the walker base on the result.
         '''
         data = json.loads(json_text, **kwargs)
         return JSONWalker(data)
 
     @staticmethod
-    def load(json_file: IO, **kwargs) -> JSONWalker:
+    def load(json_file: IO[Any], **kwargs: Any) -> JSONWalker:
         '''
         Creates json walker using `json.load()` function. Passes all arguments
         to `json.load` and tries to creat the walker base on the result.
         '''
         data = json.load(json_file, **kwargs)
         return JSONWalker(data)
 
@@ -234,15 +237,16 @@
                 if not isinstance(curr_item.data, dict):
                     if not can_break_data_structure:
                         raise KeyError(key)
                     curr_item.data = {}
                 if key not in curr_item.data:
                     can_break_data_structure = True  # Creating new data
                 curr_item = curr_item / key
-            elif isinstance(key, int):  # key is an int data must be a list
+            elif isinstance(key, int):  # pyright: ignore[reportUnnecessaryIsInstance]
+                # key is an int data must be a list
                 if key < 0:
                     raise KeyError(key)
                 if not isinstance(curr_item.data, list):
                     if not can_break_data_structure:
                         raise KeyError(key)
                     curr_item.data = []
                 if len(curr_item.data)-1 < key:
@@ -327,21 +331,20 @@
         The `/` operator creates descendant path in the JSON file.
         '''
         if isinstance(key, JSONPath):
             walker = self
             for k in key.data:
                 walker = walker / k
             return walker
-        else:
-            try:
-                return JSONWalker(
-                    self.data[key],  # type: ignore
-                    parent=self, parent_key=key)
-            except Exception as e:  # pylint: disable=broad-except
-                return JSONWalker(e, parent=self, parent_key=key)
+        try:
+            return JSONWalker(
+                self.data[key],  # type: ignore
+                parent=self, parent_key=key)
+        except Exception as e:  # pylint: disable=broad-except
+            return JSONWalker(e, parent=self, parent_key=key)
 
     def __floordiv__(self, key: JSON_SPLIT_KEY) -> JSONSplitWalker:
         '''
         The `//` operator creates JSONSplitWalker object with multiple
         alternative paths that matched provided key.
 
         :raises:
@@ -427,15 +430,15 @@
         return self._data
 
     def __truediv__(self, key: JSON_PATH_KEY) -> JSONSplitWalker:
         '''
         Applies `/` operator to all of the :class:`JSONWalkers` in this split
         walker.
         '''
-        result = []
+        result: list[JSONWalker] = []
         for walker in self.data:
             new_walker = walker / key
             if not isinstance(new_walker.data, Exception):
                 result.append(new_walker)
         return JSONSplitWalker(result)
 
     def __floordiv__(self, key: JSON_SPLIT_KEY) -> JSONSplitWalker:
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/better_json_tools/jsonc.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/better_json_tools/jsonc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# type: ignore
+'''
+A module that provides a parser for JSON with C-style comments.
+'''
 from __future__ import annotations
 
 import json
 import re
 from json import JSONDecodeError
 from json import scanner  # type: ignore
 from json.decoder import WHITESPACE, WHITESPACE_STR, scanstring  # type: ignore
@@ -250,8 +254,7 @@
         except IndexError:
             pass
         obj, end = self.raw_decode(s, idx)
         end = _w(s, end).end()
         if end != len(s):
             raise JSONDecodeError("Extra data", s, end)
         return obj
-
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/utils.py` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 '''
 Functions for analyzing Molang expressions.
 '''
 import re
-from collections import defaultdict
 
 def find_molang_resources(
         molang: str, resource_prefixes: list[str]) -> dict[str, list[str]]:
     '''
     Finds all resources of specified types in a molang expression. Returns
     a dictionary keyed by the resource type, with values being a list of
     found resources.
@@ -70,8 +69,8 @@
         data = 0
     return namespace, name, data
 
 def parse_format_version(version: str) -> tuple[int, ...]:
     '''
     Parses string with format version (dot separated numbers).
     '''
-    return tuple(int(part) for part in version.split('.'))
+    return tuple(int(part) for part in version.split('.'))
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs/views.pyi` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs/views.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,609 +1,657 @@
 import pathlib
 import sqlite3
-import typing
-from ._views import AbstractDBView
+# pylint: disable=unused-wildcard-import, unused-import, wildcard-import, missing-module-docstring
+from typing import Any, Callable # pyright: ignore[reportUnusedImport]
+from ._views import AbstractDBView # pyright: ignore[reportUnusedImport]
 # First bp and rp
-from ._db_resource_pack import *
-from ._db_behavior_pack import *
+from ._db_resource_pack import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_behavior_pack import *   # pyright: ignore[reportGeneralTypeIssues]
 # Then other tables that rely on them
-from ._db_attachable import *
-from ._db_bp_animation import *
-from ._db_bp_animation_controller import *
-from ._db_bp_block import *
-from ._db_bp_item import *
-from ._db_client_entity import *
-from ._db_entity import *
-from ._db_geometry import *
-from ._db_loot_table import *
-from ._db_particle import *
-from ._db_render_controller import *
-from ._db_rp_animation import *
-from ._db_rp_animation_controller import *
-from ._db_rp_item import *
-from ._db_sound import *
-from ._db_sound_definitions import *
-from ._db_texture import *
-from ._db_trade_table import *
-from ._db_terrain_texture import *
+from ._db_attachable import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_bp_animation import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_bp_animation_controller import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_bp_block import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_bp_item import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_client_entity import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_entity import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_geometry import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_loot_table import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_particle import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_render_controller import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_rp_animation import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_rp_animation_controller import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_rp_item import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_sound import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_sound_definitions import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_texture import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_trade_table import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_terrain_texture import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_feature_rule import *   # pyright: ignore[reportGeneralTypeIssues]
+from ._db_feature import *   # pyright: ignore[reportGeneralTypeIssues]
 class ResourcePack(AbstractDBView):
     path: pathlib.Path
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BehaviorPack(AbstractDBView):
     path: pathlib.Path
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class Attachable(AbstractDBView):
     identifier: str
     AttachableFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableItemField(AbstractDBView):
     identifier: str
     condition: str
     jsonPath: str
     Attachable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableMaterialField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     Attachable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableTextureField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     Attachable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableGeometryField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     Attachable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableRenderControllerField(AbstractDBView):
     identifier: str
     condition: str
     jsonPath: str
     Attachable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableAnimationField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     Attachable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class AttachableAnimationControllerField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     Attachable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpAnimationFile(AbstractDBView):
     path: pathlib.Path
     BehaviorPack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpAnimation(AbstractDBView):
     identifier: str
     jsonPath: str
     BpAnimationFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpAnimationControllerFile(AbstractDBView):
     path: pathlib.Path
     BehaviorPack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpAnimationController(AbstractDBView):
     identifier: str
     jsonPath: str
     BpAnimationControllerFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpBlockFile(AbstractDBView):
     path: pathlib.Path
     BehaviorPack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpBlock(AbstractDBView):
     identifier: str
     BpBlockFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpBlockLootField(AbstractDBView):
     identifier: str
     jsonPath: str
     BpBlock_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpBlockGeometryField(AbstractDBView):
     identifier: str
     jsonPath: str
     BpBlock_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpBlockMaterialInstancesField(AbstractDBView):
     jsonPath: str
     BpBlock_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpBlockMaterialInstancesFieldInstance(AbstractDBView):
     identifier: str
     jsonPath: str
     texture: str
     renderMethod: str
     BpBlockMaterialInstancesField_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpItemFile(AbstractDBView):
     path: pathlib.Path
     BehaviorPack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class BpItem(AbstractDBView):
     identifier: str
     texture: str
     BpItemFile_fk: int
     parserVersion: str
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntityFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntity(AbstractDBView):
     identifier: str
     ClientEntityFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntityRenderControllerField(AbstractDBView):
     identifier: str
     condition: str
     jsonPath: str
     ClientEntity_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntityGeometryField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     ClientEntity_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntityTextureField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     ClientEntity_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntityMaterialField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     ClientEntity_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntityAnimationField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     ClientEntity_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ClientEntityAnimationControllerField(AbstractDBView):
     shortName: str
     identifier: str
     jsonPath: str
     ClientEntity_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class EntityFile(AbstractDBView):
     path: pathlib.Path
     BehaviorPack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class Entity(AbstractDBView):
     identifier: str
     EntityFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class EntityLootField(AbstractDBView):
     identifier: str
     jsonPath: str
     Entity_fk: int
     componentType: str
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class EntityTradeField(AbstractDBView):
     identifier: str
     jsonPath: str
     Entity_fk: int
     componentType: str
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class EntitySpawnEggField(AbstractDBView):
     identifier: str
     Entity_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class GeometryFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class Geometry(AbstractDBView):
     identifier: str
     parent: str
     jsonPath: str
     GeometryFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class LootTableFile(AbstractDBView):
     path: pathlib.Path
     BehaviorPack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class LootTable(AbstractDBView):
     identifier: str
     LootTableFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class LootTableItemField(AbstractDBView):
     identifier: str
     jsonPath: str
     LootTable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class LootTableItemSpawnEggReferenceField(AbstractDBView):
     entityIdentifier: str
     spawnEggIdentifier: str
     jsonPath: str
     LootTableItemField_fk: int
     connectionType: str
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class LootTableLootTableField(AbstractDBView):
     identifier: str
     jsonPath: str
     LootTable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class ParticleFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class Particle(AbstractDBView):
     identifier: str
     material: str
     texture: str
     ParticleFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RenderControllerFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RenderController(AbstractDBView):
     identifier: str
     jsonPath: str
     RenderControllerFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RenderControllerTexturesField(AbstractDBView):
     ownerArray: str
     inOwnerArrayJsonPath: str
     shortName: str
     jsonPath: str
     RenderController_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RenderControllerMaterialsField(AbstractDBView):
     ownerArray: str
     inOwnerArrayJsonPath: str
     shortName: str
     jsonPath: str
     boneNamePattern: str
     RenderController_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RenderControllerGeometryField(AbstractDBView):
     ownerArray: str
     inOwnerArrayJsonPath: str
     shortName: str
     jsonPath: str
     RenderController_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimationFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimation(AbstractDBView):
     identifier: str
     jsonPath: str
     RpAnimationFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimationParticleEffect(AbstractDBView):
     shortName: str
     jsonPath: str
     RpAnimation_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimationSoundEffect(AbstractDBView):
     shortName: str
     jsonPath: str
     RpAnimation_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimationControllerFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimationController(AbstractDBView):
     identifier: str
     jsonPath: str
     RpAnimationControllerFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimationControllerParticleEffect(AbstractDBView):
     shortName: str
     jsonPath: str
     RpAnimationController_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpAnimationControllerSoundEffect(AbstractDBView):
     shortName: str
     jsonPath: str
     RpAnimationController_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpItemFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class RpItem(AbstractDBView):
     identifier: str
     icon: str
     RpItemFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class SoundFile(AbstractDBView):
     path: pathlib.Path
     identifier: str
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class SoundDefinitionsFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class SoundDefinition(AbstractDBView):
     identifier: str
     jsonPath: str
     SoundDefinitionsFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class SoundDefinitionSoundField(AbstractDBView):
     identifier: str
     jsonPath: str
     SoundDefinition_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TextureFile(AbstractDBView):
     path: pathlib.Path
     identifier: str
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TradeTableFile(AbstractDBView):
     path: pathlib.Path
     BehaviorPack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TradeTable(AbstractDBView):
     identifier: str
     TradeTableFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TradeTableItemField(AbstractDBView):
     identifier: str
     dataValue: int
     jsonPath: str
     TradeTable_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TradeTableItemSpawnEggReferenceField(AbstractDBView):
     entityIdentifier: str
     spawnEggIdentifier: str
     jsonPath: str
     TradeTableItemField_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TerrainTextureFile(AbstractDBView):
     path: pathlib.Path
     ResourcePack_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TerrainTexture(AbstractDBView):
     identifier: str
     TerrainTextureFile_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
 class TerrainTextureVariation(AbstractDBView):
     identifier: str
     jsonPath: pathlib.Path
     variantIndex: int
     variationIndex: int
     weight: int
     tintColor: str
     overlayColor: str
     TerrainTexture_fk: int
     id: int
     connection: sqlite3.Connection
-    query_result: typing.Callable
+    query_result: Callable[[], tuple[Any, ...]]
+    build_script: str
+class FeatureRuleFile(AbstractDBView):
+    path: pathlib.Path
+    BehaviorPack_fk: int
+    id: int
+    connection: sqlite3.Connection
+    query_result: Callable[[], tuple[Any, ...]]
+    build_script: str
+class FeatureRule(AbstractDBView):
+    identifier: str
+    placesFeature: str
+    FeatureRuleFile_fk: int
+    id: int
+    connection: sqlite3.Connection
+    query_result: Callable[[], tuple[Any, ...]]
+    build_script: str
+class FeatureFile(AbstractDBView):
+    path: pathlib.Path
+    BehaviorPack_fk: int
+    id: int
+    connection: sqlite3.Connection
+    query_result: Callable[[], tuple[Any, ...]]
+    build_script: str
+class Feature(AbstractDBView):
+    identifier: str
+    jsonPath: str
+    FeatureFile_fk: int
+    featureType: str
+    id: int
+    connection: sqlite3.Connection
+    query_result: Callable[[], tuple[Any, ...]]
+    build_script: str
+class FeaturePlacesFeatureFieldValue(AbstractDBView):
+    identifier: str
+    jsonPath: str
+    id: int
+    connection: sqlite3.Connection
+    query_result: Callable[[], tuple[Any, ...]]
+    build_script: str
+class FeaturePlacesFeatureField(AbstractDBView):
+    Feature_fk: int
+    FeaturePlacesFeatureFieldValue_fk: int
+    id: int
+    connection: sqlite3.Connection
+    query_result: Callable[[], tuple[Any, ...]]
     build_script: str
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs.egg-info/PKG-INFO` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sqlite-bedrock-packs
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python package that loads data from Minecraft: Bedrock Edition packs into SQLite database
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/sqlite_bedrock_packs/tree/master
 Project-URL: Documentation, https://sqlite-bedrock-packs.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/sqlite-bedrock-packs/badge/?version=latest
     :target: https://sqlite-bedrock-packs.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 SQLite bedrock packs
@@ -34,14 +34,33 @@
 .. code-block:: bash
 
    pip install sqlite-bedrock-packs
 
 Changelog
 =========
 
+3.2.0
+-----
+
+Added new tables:
+
+- FeatureFile
+- Feature
+- FeaturePlacesFeatureField
+- FeaturePlacesFeatureFieldValue
+- FeatureFeaturetypeEnum
+- FeatureRuleFile
+- FeatureRule
+
+
+3.1.1
+-----
+
+Better type hints.
+
 3.1.0
 -----
 
 Added new tables for behavior pack blocks and terrain textures:
 
 - BpBlockFile
 - BpBlock
```

### Comparing `sqlite-bedrock-packs-3.1.0/src/sqlite_bedrock_packs.egg-info/SOURCES.txt` & `sqlite_bedrock_packs-3.2.0/src/sqlite_bedrock_packs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 src/sqlite_bedrock_packs/_db_behavior_pack.py
 src/sqlite_bedrock_packs/_db_bp_animation.py
 src/sqlite_bedrock_packs/_db_bp_animation_controller.py
 src/sqlite_bedrock_packs/_db_bp_block.py
 src/sqlite_bedrock_packs/_db_bp_item.py
 src/sqlite_bedrock_packs/_db_client_entity.py
 src/sqlite_bedrock_packs/_db_entity.py
+src/sqlite_bedrock_packs/_db_feature.py
+src/sqlite_bedrock_packs/_db_feature_rule.py
 src/sqlite_bedrock_packs/_db_geometry.py
 src/sqlite_bedrock_packs/_db_loot_table.py
 src/sqlite_bedrock_packs/_db_particle.py
 src/sqlite_bedrock_packs/_db_render_controller.py
 src/sqlite_bedrock_packs/_db_resource_pack.py
 src/sqlite_bedrock_packs/_db_rp_animation.py
 src/sqlite_bedrock_packs/_db_rp_animation_controller.py
@@ -34,8 +36,9 @@
 src/sqlite_bedrock_packs.egg-info/SOURCES.txt
 src/sqlite_bedrock_packs.egg-info/dependency_links.txt
 src/sqlite_bedrock_packs.egg-info/top_level.txt
 src/sqlite_bedrock_packs/better_json_tools/__init__.py
 src/sqlite_bedrock_packs/better_json_tools/compact_encoder.py
 src/sqlite_bedrock_packs/better_json_tools/json_walker.py
 src/sqlite_bedrock_packs/better_json_tools/jsonc.py
+src/sqlite_bedrock_packs/better_json_tools/py.typed
 tests/test_db.py
```

### Comparing `sqlite-bedrock-packs-3.1.0/tests/test_db.py` & `sqlite_bedrock_packs-3.2.0/tests/test_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import cast
 from pathlib import Path
 import re
 from sqlite_bedrock_packs import (
     Database, Left, EntityFile, RpAnimationControllerFile, build_easy_query)
 from sqlite_bedrock_packs.better_json_tools import load_jsonc
 
 
@@ -25,15 +26,17 @@
         raise Exception(
             f"Please configure your local '{secret_data_path.as_posix()}' "
             "file. The file should contain lists of resource packs and "
             "behavior packs in following format:\n"
             f"{PACK_PATHS_STRUCTURE}")
     packs_data = load_jsonc(secret_data_path)
     rp_paths = (packs_data / "rp_paths").data
+    rp_paths = cast(list[str], rp_paths)
     bp_paths = (packs_data / "bp_paths").data
+    bp_paths = cast(list[str], bp_paths)
     print(
         f'The SQLite database file will be created in:\n'
         f'\t{db_path.as_posix()}')
 
     db_path.unlink(missing_ok=True)
     db = Database.create(db_path)
     for rp_path in rp_paths:
```


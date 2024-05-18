# Comparing `tmp/rlgym-rocket-league-2.0.0a3.tar.gz` & `tmp/rlgym-rocket-league-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlgym-rocket-league-2.0.0a3.tar", last modified: Wed Aug 23 18:41:33 2023, max compression
+gzip compressed data, was "rlgym-rocket-league-2.0.0rc0.tar", last modified: Sat May 18 16:57:23 2024, max compression
```

## Comparing `rlgym-rocket-league-2.0.0a3.tar` & `rlgym-rocket-league-2.0.0rc0.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.744185 rlgym-rocket-league-2.0.0a3/
--rw-rw-rw-   0        0        0    10946 2021-03-04 22:29:53.000000 rlgym-rocket-league-2.0.0a3/LICENSE
--rw-rw-rw-   0        0        0       37 2023-08-19 16:59:10.000000 rlgym-rocket-league-2.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     2036 2023-08-23 18:41:33.740173 rlgym-rocket-league-2.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-08-19 21:03:59.000000 rlgym-rocket-league-2.0.0a3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.248225 rlgym-rocket-league-2.0.0a3/rlgym/
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.297221 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/
--rw-rw-rw-   0        0        0     1209 2023-08-19 17:20:02.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/README.md
--rw-rw-rw-   0        0        0       34 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.309221 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/action_parsers/
--rw-rw-rw-   0        0        0       93 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/action_parsers/__init__.py
--rw-rw-rw-   0        0        0     2472 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/action_parsers/lookup_table_action.py
--rw-rw-rw-   0        0        0     1263 2023-08-23 18:35:28.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/action_parsers/repeat_action.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.334220 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/
--rw-rw-rw-   0        0        0      137 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/__init__.py
--rw-rw-rw-   0        0        0     2787 2023-08-23 18:35:28.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/car.py
--rw-rw-rw-   0        0        0      287 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/game_config.py
--rw-rw-rw-   0        0        0     1389 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/game_state.py
--rw-rw-rw-   0        0        0     3710 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/physics_object.py
--rw-rw-rw-   0        0        0      157 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/utils.py
--rw-rw-rw-   0        0        0     2775 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/common_values.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.368220 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/
--rw-rw-rw-   0        0        0      274 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/__init__.py
--rw-rw-rw-   0        0        0      944 2023-08-23 18:35:28.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/all_condition.py
--rw-rw-rw-   0        0        0      944 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/any_condition.py
--rw-rw-rw-   0        0        0      473 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/goal_condition.py
--rw-rw-rw-   0        0        0     1052 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/no_touch_condition.py
--rw-rw-rw-   0        0        0      461 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/noop_condition.py
--rw-rw-rw-   0        0        0      862 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/timeout_condition.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.380222 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/
--rw-rw-rw-   0        0        0       37 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.470017 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/
--rw-rw-rw-   0        0        0       87 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/__init__.py
--rw-rw-rw-   0        0        0      582 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/communication_exception_handler.py
--rw-rw-rw-   0        0        0     5520 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/communication_handler.py
--rw-rw-rw-   0        0        0     2573 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/message.py
--rw-rw-rw-   0        0        0     2352 2023-08-23 18:35:28.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/game_engine.py
--rw-rw-rw-   0        0        0     5740 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/game_manager.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.497017 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/
--rw-rw-rw-   0        0        0      174 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/__init__.py
--rw-rw-rw-   0        0        0     6004 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/epic_launch.py
--rw-rw-rw-   0        0        0     1125 2023-08-16 18:09:50.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/install.py
--rw-rw-rw-   0        0        0     4790 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/launch.py
--rw-rw-rw-   0        0        0     1510 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/minimize.py
--rw-rw-rw-   0        0        0     1088 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/paging.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.524017 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/plugin/
--rw-rw-rw-   0        0        0   252928 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/plugin/RLGym.dll
--rwxrwxrwx   0        0        0    23040 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/plugin/RLMultiInjector.exe
--rw-rw-rw-   0        0        0     4316 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/math.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.540030 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/obs_builders/
--rw-rw-rw-   0        0        0       37 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/obs_builders/__init__.py
--rw-rw-rw-   0        0        0     4418 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/obs_builders/default_obs.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.558017 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/
--rw-rw-rw-   0        0        0      121 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/__init__.py
--rw-rw-rw-   0        0        0     1536 2023-08-23 18:35:28.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/combined_reward.py
--rw-rw-rw-   0        0        0      812 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/goal_reward.py
--rw-rw-rw-   0        0        0      728 2023-08-23 18:35:28.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/touch_reward.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.571028 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/
--rw-rw-rw-   0        0        0       94 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.255223 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.633017 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/
--rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_0.cmf
--rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_1.cmf
--rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_10.cmf
--rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_11.cmf
--rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_12.cmf
--rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_13.cmf
--rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_14.cmf
--rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_15.cmf
--rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_2.cmf
--rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_3.cmf
--rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_4.cmf
--rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_5.cmf
--rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_6.cmf
--rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_7.cmf
--rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_8.cmf
--rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_9.cmf
--rw-rw-rw-   0        0        0     2830 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/rlviser_renderer.py
--rw-rw-rw-   0        0        0     9856 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/rocketsim_engine.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.648017 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/state_mutators/
--rw-rw-rw-   0        0        0      151 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/state_mutators/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/state_mutators/fixed_team_size_mutator.py
--rw-rw-rw-   0        0        0     2141 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/state_mutators/kickoff_mutator.py
--rw-rw-rw-   0        0        0      401 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/state_mutators/mutator_sequence.py
--rw-rw-rw-   0        0        0     1212 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/version.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:41:33.737173 rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/
--rw-rw-rw-   0        0        0     2036 2023-08-23 18:41:33.000000 rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-08-23 18:41:33.000000 rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-23 18:41:33.000000 rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2023-08-23 18:41:33.000000 rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-23 18:41:33.000000 rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-23 18:41:33.745175 rlgym-rocket-league-2.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0     2455 2023-08-23 18:41:29.000000 rlgym-rocket-league-2.0.0a3/setup.json
--rw-rw-rw-   0        0        0      805 2023-08-23 18:04:36.000000 rlgym-rocket-league-2.0.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.654442 rlgym-rocket-league-2.0.0rc0/
+-rw-rw-rw-   0        0        0    10946 2021-03-04 22:29:53.000000 rlgym-rocket-league-2.0.0rc0/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-08-19 16:59:10.000000 rlgym-rocket-league-2.0.0rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2062 2024-05-18 16:57:23.653455 rlgym-rocket-league-2.0.0rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     1954 2023-12-03 17:45:55.000000 rlgym-rocket-league-2.0.0rc0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.530454 rlgym-rocket-league-2.0.0rc0/rlgym/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.551454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/
+-rw-rw-rw-   0        0        0     1209 2023-08-19 17:20:02.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/README.md
+-rw-rw-rw-   0        0        0       34 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.555454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/action_parsers/
+-rw-rw-rw-   0        0        0       93 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/action_parsers/__init__.py
+-rw-rw-rw-   0        0        0     2544 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/action_parsers/lookup_table_action.py
+-rw-rw-rw-   0        0        0     1501 2024-05-18 16:08:45.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/action_parsers/repeat_action.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.564454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/
+-rw-rw-rw-   0        0        0      137 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/__init__.py
+-rw-rw-rw-   0        0        0     3391 2024-02-25 13:34:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/car.py
+-rw-rw-rw-   0        0        0      287 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/game_config.py
+-rw-rw-rw-   0        0        0     1389 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/game_state.py
+-rw-rw-rw-   0        0        0     3710 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/physics_object.py
+-rw-rw-rw-   0        0        0      157 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/utils.py
+-rw-rw-rw-   0        0        0     3084 2024-02-25 13:34:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/common_values.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.574443 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/
+-rw-rw-rw-   0        0        0      274 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/__init__.py
+-rw-rw-rw-   0        0        0      975 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/all_condition.py
+-rw-rw-rw-   0        0        0      975 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/any_condition.py
+-rw-rw-rw-   0        0        0      496 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/goal_condition.py
+-rw-rw-rw-   0        0        0     1075 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/no_touch_condition.py
+-rw-rw-rw-   0        0        0      484 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/noop_condition.py
+-rw-rw-rw-   0        0        0      885 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/timeout_condition.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.578454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/
+-rw-rw-rw-   0        0        0       37 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.585454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/
+-rw-rw-rw-   0        0        0       87 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/communication_exception_handler.py
+-rw-rw-rw-   0        0        0     5520 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/communication_handler.py
+-rw-rw-rw-   0        0        0     2573 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/message.py
+-rw-rw-rw-   0        0        0     2352 2023-08-23 18:35:28.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/game_engine.py
+-rw-rw-rw-   0        0        0     5740 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/game_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.595454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/
+-rw-rw-rw-   0        0        0      174 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/__init__.py
+-rw-rw-rw-   0        0        0     6004 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/epic_launch.py
+-rw-rw-rw-   0        0        0     1125 2023-08-16 18:09:50.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/install.py
+-rw-rw-rw-   0        0        0     4790 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/launch.py
+-rw-rw-rw-   0        0        0     1510 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/minimize.py
+-rw-rw-rw-   0        0        0     1088 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/paging.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.600454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/plugin/
+-rw-rw-rw-   0        0        0   252928 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/plugin/RLGym.dll
+-rwxrwxrwx   0        0        0    23040 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/plugin/RLMultiInjector.exe
+-rw-rw-rw-   0        0        0     4316 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/math.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.604455 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/obs_builders/
+-rw-rw-rw-   0        0        0       37 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/obs_builders/__init__.py
+-rw-rw-rw-   0        0        0     4470 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/obs_builders/default_obs.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.610454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/
+-rw-rw-rw-   0        0        0      121 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/combined_reward.py
+-rw-rw-rw-   0        0        0      835 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/goal_reward.py
+-rw-rw-rw-   0        0        0      751 2024-05-18 16:07:54.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/touch_reward.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.612446 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/rlviser/
+-rw-rw-rw-   0        0        0       47 2024-04-13 13:29:38.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/rlviser/__init__.py
+-rw-rw-rw-   0        0        0     2845 2024-04-13 14:00:28.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/rlviser/rlviser_renderer.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.615454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/
+-rw-rw-rw-   0        0        0       47 2024-04-13 13:29:38.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.536442 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.637454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/
+-rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_0.cmf
+-rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_1.cmf
+-rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_10.cmf
+-rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_11.cmf
+-rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_12.cmf
+-rw-rw-rw-   0        0        0     2480 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_13.cmf
+-rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_14.cmf
+-rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_15.cmf
+-rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_2.cmf
+-rw-rw-rw-   0        0        0    16364 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_3.cmf
+-rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_4.cmf
+-rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_5.cmf
+-rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_6.cmf
+-rw-rw-rw-   0        0        0    18236 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_7.cmf
+-rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_8.cmf
+-rw-rw-rw-   0        0        0      416 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_9.cmf
+-rw-rw-rw-   0        0        0    10572 2024-04-14 14:57:18.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/rocketsim_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.644454 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/state_mutators/
+-rw-rw-rw-   0        0        0      151 2023-08-16 18:04:12.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/state_mutators/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/state_mutators/fixed_team_size_mutator.py
+-rw-rw-rw-   0        0        0     2141 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/state_mutators/kickoff_mutator.py
+-rw-rw-rw-   0        0        0      401 2023-08-23 18:35:27.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/state_mutators/mutator_sequence.py
+-rw-rw-rw-   0        0        0     1687 2024-05-18 16:37:43.000000 rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/version.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:57:23.651454 rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/
+-rw-rw-rw-   0        0        0     2062 2024-05-18 16:57:23.000000 rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3526 2024-05-18 16:57:23.000000 rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:57:23.000000 rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      246 2024-05-18 16:57:23.000000 rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-18 16:57:23.000000 rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:57:23.654442 rlgym-rocket-league-2.0.0rc0/setup.cfg
+-rw-rw-rw-   0        0        0     2486 2024-05-18 16:57:19.000000 rlgym-rocket-league-2.0.0rc0/setup.json
+-rw-rw-rw-   0        0        0      805 2023-08-23 18:04:36.000000 rlgym-rocket-league-2.0.0rc0/setup.py
```

### Comparing `rlgym-rocket-league-2.0.0a3/LICENSE` & `rlgym-rocket-league-2.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/PKG-INFO` & `rlgym-rocket-league-2.0.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rlgym-rocket-league
-Version: 2.0.0a3
+Version: 2.0.0rc0
 Summary: A python API that can be used to treat the game Rocket League as an Openai Gym-like environment for Reinforcement Learning projects.
 Home-page: https://rlgym.org
 Author: Lucas Emery and Matthew Allen
 Author-email: contact@rlgym.org
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/lucas-emery/rocket-league-gym
 Keywords: rocket-league,gym,reinforcement-learning,rlgym
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: sim
+Provides-Extra: rlviser
 Provides-Extra: game
 Provides-Extra: all
 License-File: LICENSE
 
 # The Rocket League Gym
 This is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.
```

### Comparing `rlgym-rocket-league-2.0.0a3/README.md` & `rlgym-rocket-league-2.0.0rc0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 Once the API is installed, you will need to enable the RLGym plugin from inside the Bakkesmod plugin manager. To do this, first launch the game, then press F2 to open the Bakkesmod menu. Navigate to the `plugins` tab and open the `Plugin Manager`. From there, scroll down until you find the RLGym plugin, and enable it. Close the game when this is done.
 
 
 ### Testing everything works
 RLGym is now installed! simply run ```example.py``` from our repo to ensure everything works.
 
 ## Dependency Management
-**Don't** specify this package as a dependency, this is an **instalation only** package.
+**DO NOT** specify this package as a dependency, this is an **installation only** package.
 
-You should depend directly on the package you're consuming and its corresponding extras, be it 
-`rlgym-rocket-league[sim]`, `rlgym-api` or any other in particular.
+You should depend directly on the package you're consuming and its corresponding extras, e.g.
+`rlgym-rocket-league[sim]`, `rlgym-api` or whichever of our libraries your project is using.
 
 ## Usage
 For tutorials and documentation, please visit our [Wiki](https://rlgym.org/).
 
 We also provide the base RLGym API in its own [standalone package](https://pypi.org/project/rlgym-api/) with no dependencies.
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/README.md` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/README.md`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/action_parsers/lookup_table_action.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/action_parsers/lookup_table_action.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Dict, Any
+from typing import Dict, Any, Tuple, List
 
 import numpy as np
 
 from rlgym.api import ActionParser, AgentID
 from rlgym.rocket_league.api import GameState
 
 
-class LookupTableAction(ActionParser[AgentID, np.ndarray, np.ndarray, GameState, int]):
+class LookupTableAction(ActionParser[AgentID, np.ndarray, np.ndarray, GameState, Tuple[str, int]]):
     """
     World-famous discrete action parser which uses a lookup table to reduce the number of possible actions from 1944 to 90
     """
 
     def __init__(self):
         super().__init__()
         self._lookup_table = self.make_lookup_table()
 
-    def get_action_space(self, agent: AgentID) -> int:
-        return len(self._lookup_table)
+    def get_action_space(self, agent: AgentID) -> Tuple[str, int]:
+        return 'discrete', len(self._lookup_table)
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         pass
 
     def parse_actions(self, actions: Dict[AgentID, np.ndarray], state: GameState, shared_info: Dict[str, Any]) -> Dict[AgentID, np.ndarray]:
         parsed_actions = {}
         for agent, action in actions.items():
             # Action can have shape (Ticks, 1) or (Ticks)
             assert len(action.shape) == 1 or (len(action.shape) == 2 and action.shape[1] == 1)
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/action_parsers/repeat_action.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/action_parsers/repeat_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from typing import Dict, Any
+from typing import Dict, Any, List
 
 import numpy as np
 
-from rlgym.api import ActionParser, SpaceType, AgentID
-from rlgym.rocket_league.api import GameState
+from rlgym.api import ActionParser, ActionType, StateType, ActionSpaceType, AgentID
 
 
-class RepeatAction(ActionParser[AgentID, np.ndarray, np.ndarray, GameState, SpaceType]):
+class RepeatAction(ActionParser[AgentID, ActionType, np.ndarray, StateType, ActionSpaceType]):
     """
     A simple wrapper to emulate tick skip
     """
 
     def __init__(self,
-                 parser: ActionParser[AgentID, np.ndarray, np.ndarray, GameState, SpaceType],
+                 parser: ActionParser[AgentID, ActionType, np.ndarray, StateType, ActionSpaceType],
                  repeats=8):
         super().__init__()
         self.parser = parser
         self.repeats = repeats
 
-    def get_action_space(self, agent: AgentID) -> SpaceType:
+    def get_action_space(self, agent: AgentID) -> ActionSpaceType:
         return self.parser.get_action_space(agent)
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
-        pass
+    def reset(self, agents: List[AgentID], initial_state: StateType, shared_info: Dict[str, Any]) -> None:
+        self.parser.reset(agents, initial_state, shared_info)
 
-    def parse_actions(self, actions: Dict[AgentID, np.ndarray], state: GameState, shared_info: Dict[str, Any]) -> Dict[AgentID, np.ndarray]:
+    def parse_actions(self, actions: Dict[AgentID, ActionType], state: StateType, shared_info: Dict[str, Any]) -> Dict[AgentID, np.ndarray]:
+        rlgym_actions = self.parser.parse_actions(actions, state, shared_info)
         repeat_actions = {}
-        for agent, action in actions.items():
-            # Action can have shape (ActionSpace)
-            assert len(action.shape) == 1
+        for agent, action in rlgym_actions.items():
+            if action.shape == (8,):
+                action = np.expand_dims(action, axis=0)
+            elif action.shape != (1, 8):
+                raise ValueError(f"Expected action to have shape (8,) or (1,8), got {action.shape}")
 
-            repeat_actions[agent] = np.expand_dims(action, axis=0).repeat(self.repeats, axis=0)
+            repeat_actions[agent] = action.repeat(self.repeats, axis=0)
 
-        return self.parser.parse_actions(repeat_actions, state, shared_info)
+        return repeat_actions
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/car.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/car.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 from dataclasses import dataclass
 from typing import Optional, Generic
 
 from rlgym.api import AgentID
-from ..common_values import DOUBLEJUMP_MAX_DELAY, FLIP_TORQUE_TIME
+from ..common_values import DOUBLEJUMP_MAX_DELAY, FLIP_TORQUE_TIME, BLUE_TEAM, ORANGE_TEAM
 from .physics_object import PhysicsObject
 from .utils import create_default_init
 
 
 @dataclass(init=False)
 class Car(Generic[AgentID]):
 
@@ -50,14 +50,34 @@
     _inverted_physics: PhysicsObject
 
     __slots__ = tuple(__annotations__)
 
     exec(create_default_init(__slots__))
 
     @property
+    def is_blue(self) -> bool:
+        return self.team_num == BLUE_TEAM
+
+    @property
+    def is_orange(self) -> bool:
+        return self.team_num == ORANGE_TEAM
+
+    @property
+    def is_demoed(self) -> bool:
+        return self.demo_respawn_timer > 0
+
+    @property
+    def is_boosting(self) -> bool:
+        return self.boost_active_time > 0
+
+    @property
+    def is_supersonic(self) -> bool:
+        return self.supersonic_time > 0
+
+    @property
     def can_flip(self) -> bool:
         return not self.has_double_jumped and not self.has_flipped and self.air_time_since_jump < DOUBLEJUMP_MAX_DELAY
 
     @property  # TODO This one isn't in rsim python yet, emulate with prop
     def is_flipping(self) -> bool:
         return self.has_flipped and self.flip_time < FLIP_TORQUE_TIME
 
@@ -67,11 +87,15 @@
             self.has_flipped = True
             if self.flip_time >= FLIP_TORQUE_TIME:
                 self.flip_time = 0
         else:
             self.flip_time = FLIP_TORQUE_TIME
 
     @property
+    def had_car_contact(self) -> bool:
+        return self.bump_victim_id is not None
+
+    @property
     def inverted_physics(self) -> PhysicsObject:
         if self._inverted_physics is None:
             self._inverted_physics = self.physics.inverted()
         return self._inverted_physics
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/game_state.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/game_state.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/api/physics_object.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/api/physics_object.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/common_values.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/common_values.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,15 +33,26 @@
 
 ORANGE_FIELD_BOTTOM_LEFT = (SIDE_WALL_X, BACK_WALL_Y, 0)
 BLUE_FIELD_BOTTOM_LEFT = (-SIDE_WALL_X, -BACK_WALL_Y, 0)
 
 ORANGE_FIELD_BOTTOM_RIGHT = (-SIDE_WALL_X, BACK_WALL_Y, 0)
 BLUE_FIELD_BOTTOM_RIGHT = (SIDE_WALL_X, -BACK_WALL_Y, 0)
 
-BALL_RADIUS = 92.75
+BALL_RADIUS = 91.25
+TICKS_PER_SECOND = 120
+CORNER_CATHETUS_LENGTH = 1152
+RAMP_HEIGHT = 256
+UNREAL_UNITS_PER_METER = 100
+SMALL_PAD_RECHARGE_SECONDS = 4
+BIG_PAD_RECHARGE_SECONDS = 10
+GRAVITY = 650  # uu/s^2
+BOOST_CONSUMPTION_RATE = 33.3  # per second
+CAR_MASS = 180
+BALL_MASS = 30
+BOOST_ACCELERATION = 991.666  # uu/s^2
 
 BALL_MAX_SPEED = 6000
 CAR_MAX_SPEED = 2300
 SUPERSONIC_THRESHOLD = 2200
 CAR_MAX_ANG_VEL = 5.5
 
 BLUE_TEAM = 0
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/all_condition.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/all_condition.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class AllCondition(DoneCondition[AgentID, GameState]):
 
     def __init__(self, *conditions: DoneCondition):
         self.conditions = tuple(conditions)
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         for condition in self.conditions:
-            condition.reset(initial_state, shared_info)
+            condition.reset(agents, initial_state, shared_info)
 
     def is_done(self, agents: List[AgentID], state: GameState, shared_info: Dict[str, Any]) -> Dict[AgentID, bool]:
         # TODO can we optimize this with numpy?
         combined_dones = {agent: False for agent in agents}
         for condition in self.conditions:
             dones = condition.is_done(agents, state, shared_info)
             for agent, done in dones.items():
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/any_condition.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/any_condition.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class AnyCondition(DoneCondition[AgentID, GameState]):
 
     def __init__(self, *conditions: DoneCondition):
         self.conditions = tuple(conditions)
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         for condition in self.conditions:
-            condition.reset(initial_state, shared_info)
+            condition.reset(agents, initial_state, shared_info)
 
     def is_done(self, agents: List[AgentID], state: GameState, shared_info: Dict[str, Any]) -> Dict[AgentID, bool]:
         # TODO can we optimize this with numpy?
         combined_dones = {agent: False for agent in agents}
         for condition in self.conditions:
             dones = condition.is_done(agents, state, shared_info)
             for agent, done in dones.items():
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/no_touch_condition.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/no_touch_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         """
         :param timeout: Timeout in seconds
         """
         self.timeout = timeout
         self.tick_rate = tick_rate
         self.last_touch_tick = None
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         self.last_touch_tick = initial_state.tick_count
 
     def is_done(self, agents: List[AgentID], state: GameState, shared_info: Dict[str, Any]) -> Dict[AgentID, bool]:
         if any(car.ball_touches > 0 for car in state.cars.values()):
             self.last_touch_tick = state.tick_count
             done = False
         else:
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/done_conditions/timeout_condition.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/done_conditions/timeout_condition.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,14 @@
         """
         :param timeout: Timeout in seconds
         """
         self.timeout = timeout
         self.tick_rate = tick_rate
         self.initial_tick = None
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         self.initial_tick = initial_state.tick_count
 
     def is_done(self, agents: List[AgentID], state: GameState, shared_info: Dict[str, Any]) -> Dict[AgentID, bool]:
         time_elapsed = (state.tick_count - self.initial_tick) * self.tick_rate
         done = time_elapsed >= self.timeout
         return {agent: done for agent in agents}
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/communication_exception_handler.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/communication_exception_handler.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/communication_handler.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/communication_handler.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/communication/message.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/communication/message.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/game_engine.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/game_engine.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/game_manager.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/game_manager.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/epic_launch.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/epic_launch.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/install.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/install.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/launch.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/launch.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/minimize.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/minimize.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/launch/paging.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/launch/paging.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/plugin/RLGym.dll` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/plugin/RLGym.dll`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/game/plugin/RLMultiInjector.exe` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/game/plugin/RLMultiInjector.exe`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/math.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/math.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/obs_builders/default_obs.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/obs_builders/default_obs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import math
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Tuple
 
 import numpy as np
 
 from rlgym.api import ObsBuilder, AgentID
 from rlgym.rocket_league.api import Car, GameState
 from rlgym.rocket_league.common_values import ORANGE_TEAM
 
 
-class DefaultObs(ObsBuilder[AgentID, np.ndarray, GameState, int]):
+class DefaultObs(ObsBuilder[AgentID, np.ndarray, GameState, Tuple[str, int]]):
 
     def __init__(self, zero_padding=3, pos_coef=1/2300, ang_coef=1/math.pi, lin_vel_coef=1/2300, ang_vel_coef=1/math.pi,
                  pad_timer_coef=1/10):
         """
         :param zero_padding: Number of max cars per team, if not None the obs will be zero padded
         :param pos_coef: Position normalization coefficient
         :param ang_coef: Rotation angle normalization coefficient
@@ -24,21 +24,21 @@
         self.POS_COEF = pos_coef
         self.ANG_COEF = ang_coef
         self.LIN_VEL_COEF = lin_vel_coef
         self.ANG_VEL_COEF = ang_vel_coef
         self.PAD_TIMER_COEF = pad_timer_coef
         self.zero_padding = zero_padding
 
-    def get_obs_space(self, agent: AgentID) -> int:
+    def get_obs_space(self, agent: AgentID) -> Tuple[str, int]:
         if self.zero_padding is not None:
-            return 52 + 20 * self.zero_padding * 2
+            return 'real', 52 + 20 * self.zero_padding * 2
         else:
-            return None  # Without zero padding this depends on the initial state, but we don't want to crash for now
+            return 'real', -1  # Without zero padding this depends on the initial state, but we don't want to crash for now
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         pass
 
     def build_obs(self, agents: List[AgentID], state: GameState, shared_info: Dict[str, Any]) -> Dict[AgentID, np.ndarray]:
         obs = {}
         for agent in agents:
             obs[agent] = self._build_obs(agent, state, shared_info)
 
@@ -112,10 +112,10 @@
             physics.forward,
             physics.up,
             physics.linear_velocity * self.LIN_VEL_COEF,
             physics.angular_velocity * self.ANG_VEL_COEF,
             [car.boost_amount,
              car.demo_respawn_timer,
              int(car.on_ground),
-             int(car.boost_active_time > 0),
-             int(car.supersonic_time > 0)]
+             int(car.is_boosting),
+             int(car.is_supersonic)]
         ])
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/combined_reward.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/combined_reward.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,17 +17,17 @@
                 r, w = value, 1.
             reward_fns.append(r)
             weights.append(w)
 
         self.reward_fns = tuple(reward_fns)
         self.weights = tuple(weights)
 
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         for reward_fn in self.reward_fns:
-            reward_fn.reset(initial_state, shared_info)
+            reward_fn.reset(agents, initial_state, shared_info)
 
     def get_rewards(self, agents: List[AgentID], state: GameState, is_terminated: Dict[AgentID, bool],
                     is_truncated: Dict[AgentID, bool], shared_info: Dict[str, Any]) -> Dict[AgentID, float]:
         # TODO optimize this double for loop with a numpy matrix?
         combined_rewards = {agent: 0. for agent in agents}
         for reward_fn, weight in zip(self.reward_fns, self.weights):
             rewards = reward_fn.get_rewards(agents, state, is_terminated, is_truncated, shared_info)
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/goal_reward.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/goal_reward.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Dict, Any
 
 from rlgym.api import RewardFunction, AgentID
 from rlgym.rocket_league.api import GameState
 
 
 class GoalReward(RewardFunction[AgentID, GameState, float]):
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         pass
 
     def get_rewards(self, agents: List[AgentID], state: GameState, is_terminated: Dict[AgentID, bool],
                     is_truncated: Dict[AgentID, bool], shared_info: Dict[str, Any]) -> Dict[AgentID, float]:
         return {agent: self._get_reward(agent, state) for agent in agents}
 
     def _get_reward(self, agent: AgentID, state: GameState) -> float:
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/reward_functions/touch_reward.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/reward_functions/touch_reward.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Dict, Any
 
 from rlgym.api import RewardFunction, AgentID
 from rlgym.rocket_league.api import GameState
 
 
 class TouchReward(RewardFunction[AgentID, GameState, float]):
-    def reset(self, initial_state: GameState, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: GameState, shared_info: Dict[str, Any]) -> None:
         pass
 
     def get_rewards(self, agents: List[AgentID], state: GameState, is_terminated: Dict[AgentID, bool],
                     is_truncated: Dict[AgentID, bool], shared_info: Dict[str, Any]) -> Dict[AgentID, float]:
         return {agent: self._get_reward(agent, state) for agent in agents}
 
     def _get_reward(self, agent: AgentID, state: GameState) -> float:
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_0.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_0.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_1.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_1.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_10.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_10.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_11.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_11.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_12.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_12.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_13.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_13.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_2.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_2.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_3.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_3.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_4.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_4.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_5.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_5.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_6.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_6.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_7.cmf` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/collision_meshes/soccar/mesh_7.cmf`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/rlviser_renderer.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/rlviser/rlviser_renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict
 
-import RocketSim as rsim
 import rlviser_py as rlviser
+import RocketSim as rsim
 
 from rlgym.api import Renderer
 from rlgym.rocket_league.api import Car, GameState
 from rlgym.rocket_league.common_values import BOOST_LOCATIONS
 
 
 class RLViserRenderer(Renderer[GameState]):
@@ -18,23 +18,24 @@
     def render(self, state: GameState, shared_info: Dict[str, Any]) -> Any:
         boost_pad_states = [bool(timer == 0) for timer in state.boost_pad_timers]
 
         ball = rsim.BallState()
         ball.pos = rsim.Vec(*state.ball.position)
         ball.vel = rsim.Vec(*state.ball.linear_velocity)
         ball.ang_vel = rsim.Vec(*state.ball.angular_velocity)
+        ball.rot_mat = rsim.RotMat(*state.ball.rotation_mtx.transpose().flatten())
 
         car_data = []
         for idx, car in enumerate(state.cars.values()):
             car_state = self._get_car_state(car)
-            car_data.append((idx, car.team_num, rsim.CarConfig(car.hitbox_type), car_state))
+            car_data.append((idx + 1, car.team_num, rsim.CarConfig(car.hitbox_type), car_state))
 
         self.packet_id += 1
-        rlviser.render(tick_count=self.packet_id, tick_rate=self.tick_rate, boost_pad_states=boost_pad_states,
-                       ball=ball, cars=car_data)
+        rlviser.render(tick_count=self.packet_id, tick_rate=self.tick_rate, game_mode=rsim.GameMode.SOCCAR,
+                       boost_pad_states=boost_pad_states, ball=ball, cars=car_data)
 
     def close(self):
         rlviser.quit()
 
     # I stole this from RocketSimEngine
     def _get_car_state(self, car: Car):
         car_state = rsim.CarState()
@@ -61,11 +62,8 @@
         car_state.flip_time = car.flip_time
         car_state.last_rel_dodge_torque = rsim.Vec(*car.flip_torque)
 
         car_state.is_auto_flipping = car.is_autoflipping
         car_state.auto_flip_timer = car.autoflip_timer
         car_state.auto_flip_torque_scale = car.autoflip_direction
 
-        if car.bump_victim_id is not None:
-            car_state.car_contact_id = car.bump_victim_id
-
         return car_state
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/sim/rocketsim_engine.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/sim/rocketsim_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import numpy as np
 import RocketSim as rsim
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 from rlgym.api import TransitionEngine, AgentID
 from rlgym.rocket_league.api import Car, GameConfig, GameState, PhysicsObject
 from rlgym.rocket_league.common_values import BOOST_LOCATIONS, BACK_WALL_Y, BALL_RADIUS
 
 
 class RocketSimEngine(TransitionEngine[AgentID, GameState, np.ndarray]):
@@ -19,14 +19,15 @@
             rsim.init(os.path.join(cur_dir, 'collision_meshes'))
         except Exception:
             pass
         self._state = None
         self._tick_count = None
         self._game_config = None
         self._cars: Dict[AgentID, rsim.Car] = {}
+        self._agent_ids: Dict[int, AgentID] = {}
         self._hitboxes: Dict[int, int] = {}
         self._touches: Dict[int, int] = {}
         self._arena = rsim.Arena(rsim.GameMode.SOCCAR)
         self._arena.set_ball_touch_callback(self._ball_touch_callback)
 
     @property
     def agents(self) -> List[AgentID]:
@@ -69,14 +70,15 @@
                 controls.boost = bool(action[step, 6])
                 controls.handbrake = bool(action[step, 7])
 
                 self._cars[agent_id].set_controls(controls)
 
             self._arena.step(1)
             self._tick_count += 1
+            #TODO call event listener
 
         return self._get_state()
 
     def set_state(self, desired_state: GameState, shared_info: Dict[str, Any]) -> GameState:
         self._tick_count = desired_state.tick_count
 
         config = rsim.MutatorConfig()
@@ -85,32 +87,41 @@
         self._arena.set_mutator_config(config)
         self._game_config = desired_state.config
 
         ball_state = rsim.BallState()
         ball_state.pos = rsim.Vec(*desired_state.ball.position)
         ball_state.vel = rsim.Vec(*desired_state.ball.linear_velocity)
         ball_state.ang_vel = rsim.Vec(*desired_state.ball.angular_velocity)
+        try:
+            ball_state.rot_mat = rsim.RotMat(*desired_state.ball.rotation_mtx.transpose().flatten())
+        except ValueError:
+            pass
         self._arena.ball.set_state(ball_state)
 
         #TODO reuse cars? We'd have to check the hitbox
         for car in self._arena.get_cars():
             self._arena.remove_car(car)
         self._cars.clear()
+        self._agent_ids.clear()
         self._hitboxes.clear()
         self._touches.clear()
 
         for agent_id, desired_car in desired_state.cars.items():
             config = rsim.CarConfig(desired_car.hitbox_type)
             config.dodge_deadzone = desired_state.config.dodge_deadzone
             car: rsim.Car = self._arena.add_car(desired_car.team_num, config)
             self._cars[agent_id] = car
+            self._agent_ids[car.id] = agent_id
             self._hitboxes[car.id] = desired_car.hitbox_type
             self._touches[car.id] = 0
 
-            self._set_car_state(car, desired_car)
+        # This loop looks dumb here but we need to create the cars before setting the state
+        #  so we know the full AgentID->RSimID mapping
+        for agent_id, desired_car in desired_state.cars.items():
+            self._set_car_state(self._cars[agent_id], desired_car)
 
         #TODO check if the order is correct, I think mtheall's bindings handle it internally
         for idx, pad in enumerate(self._arena.get_boost_pads()):
             pad_state = rsim.BoostPadState()
             pad_state.cooldown = desired_state.boost_pad_timers[idx]
             pad.set_state(pad_state)
 
@@ -122,14 +133,15 @@
         gs.config = self._game_config
 
         ball_state = self._arena.ball.get_state()
         gs.ball = PhysicsObject()
         gs.ball.position = ball_state.pos.as_numpy()
         gs.ball.linear_velocity = ball_state.vel.as_numpy()
         gs.ball.angular_velocity = ball_state.ang_vel.as_numpy()
+        gs.ball.rotation_mtx = np.ascontiguousarray(ball_state.rot_mat.as_numpy().reshape(3, 3).transpose())
 
         # Only works for soccar
         gs.goal_scored = abs(gs.ball.position[1]) > BACK_WALL_Y + BALL_RADIUS
 
         gs.cars = {}
         for agent_id, rsim_car in self._cars.items():
             car_state = rsim_car.get_state()
@@ -163,15 +175,15 @@
             car.flip_time = car_state.flip_time
             car.flip_torque = car_state.last_rel_dodge_torque.as_numpy()
 
             car.is_autoflipping = car_state.is_auto_flipping
             car.autoflip_timer = car_state.auto_flip_timer
             car.autoflip_direction = car_state.auto_flip_torque_scale
 
-            car.bump_victim_id = car_state.car_contact_id if car_state.car_contact_cooldown_timer > 0 else None
+            car.bump_victim_id = self._agent_ids[car_state.car_contact_id] if car_state.car_contact_cooldown_timer > 0 else None
             car.ball_touches = self._touches[rsim_car.id]
             self._touches[rsim_car.id] = 0
 
             gs.cars[agent_id] = car
 
         #TODO check if the order is correct, I think mtheall's bindings handle it internally
         gs.boost_pad_timers = np.empty(len(BOOST_LOCATIONS), dtype=np.float32)
@@ -208,15 +220,15 @@
         car_state.last_rel_dodge_torque = rsim.Vec(*desired_car.flip_torque)
 
         car_state.is_auto_flipping = desired_car.is_autoflipping
         car_state.auto_flip_timer = desired_car.autoflip_timer
         car_state.auto_flip_torque_scale = desired_car.autoflip_direction
 
         if desired_car.bump_victim_id is not None:
-            car_state.car_contact_id = desired_car.bump_victim_id
+            car_state.car_contact_id = self._cars[desired_car.bump_victim_id].id
             # Do we want to set the bump cooldown too?
 
         car.set_state(car_state)
 
     def _ball_touch_callback(self, arena: rsim.Arena, car: rsim.Car, data):
         self._touches[car.id] += 1
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/state_mutators/fixed_team_size_mutator.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/state_mutators/fixed_team_size_mutator.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/state_mutators/kickoff_mutator.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/state_mutators/kickoff_mutator.py`

 * *Files identical despite different names*

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym/rocket_league/version.py` & `rlgym-rocket-league-2.0.0rc0/rlgym/rocket_league/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,106 @@
 00000000: 0d0a 5f5f 7665 7273 696f 6e5f 5f20 3d20  ..__version__ = 
-00000010: 2732 2e30 2e30 2d61 6c70 6861 2d33 270d  '2.0.0-alpha-3'.
-00000020: 0a0d 0a0d 0a64 6566 2067 6574 5f63 7572  .....def get_cur
-00000030: 7265 6e74 5f72 656c 6561 7365 5f6e 6f74  rent_release_not
-00000040: 6573 2829 3a0d 0a20 2020 2069 6620 5f5f  es():..    if __
-00000050: 7665 7273 696f 6e5f 5f20 696e 2072 656c  version__ in rel
-00000060: 6561 7365 5f6e 6f74 6573 3a0d 0a20 2020  ease_notes:..   
-00000070: 2020 2020 2072 6574 7572 6e20 7265 6c65       return rele
-00000080: 6173 655f 6e6f 7465 735b 5f5f 7665 7273  ase_notes[__vers
-00000090: 696f 6e5f 5f5d 0d0a 2020 2020 7265 7475  ion__]..    retu
-000000a0: 726e 2027 270d 0a0d 0a0d 0a64 6566 2070  rn ''......def p
-000000b0: 7269 6e74 5f63 7572 7265 6e74 5f72 656c  rint_current_rel
-000000c0: 6561 7365 5f6e 6f74 6573 2829 3a0d 0a20  ease_notes():.. 
-000000d0: 2020 2070 7269 6e74 2866 2256 6572 7369     print(f"Versi
-000000e0: 6f6e 207b 5f5f 7665 7273 696f 6e5f 5f7d  on {__version__}
-000000f0: 2229 0d0a 2020 2020 7072 696e 7428 6765  ")..    print(ge
-00000100: 745f 6375 7272 656e 745f 7265 6c65 6173  t_current_releas
-00000110: 655f 6e6f 7465 7328 2929 0d0a 2020 2020  e_notes())..    
-00000120: 7072 696e 7428 2222 290d 0a0d 0a0d 0a72  print("")......r
-00000130: 656c 6561 7365 5f6e 6f74 6573 203d 207b  elease_notes = {
-00000140: 0d0a 2020 2020 2732 2e30 2e30 2d61 6c70  ..    '2.0.0-alp
-00000150: 6861 2d33 273a 0d0a 2020 2020 2222 220d  ha-3':..    """.
-00000160: 0a20 2020 202d 2054 6869 7320 7665 7273  .    - This vers
-00000170: 696f 6e20 636f 6e74 6169 6e73 206e 756d  ion contains num
-00000180: 6572 6f75 7320 756e 7465 7374 6564 2061  erous untested a
-00000190: 6e64 2062 7265 616b 696e 6720 6368 616e  nd breaking chan
-000001a0: 6765 732e 2052 756e 2061 7420 796f 7572  ges. Run at your
-000001b0: 206f 776e 2072 6973 6b2e 0d0a 2020 2020   own risk...    
-000001c0: 2d20 4164 6465 6420 7368 6172 6564 5f69  - Added shared_i
-000001d0: 6e66 6f20 7061 7261 6d20 746f 2054 7261  nfo param to Tra
-000001e0: 6e73 6974 696f 6e45 6e67 696e 6520 616e  nsitionEngine an
-000001f0: 6420 5265 6e64 6572 6572 0d0a 2020 2020  d Renderer..    
-00000200: 2d20 4669 7865 6420 5079 7468 6f6e 203c  - Fixed Python <
-00000210: 332e 3920 696e 7374 616c 6c0d 0a20 2020  3.9 install..   
-00000220: 202d 2055 7064 6174 6520 696d 706f 7274   - Update import
-00000230: 7320 746f 2072 6c67 796d 2e61 7069 0d0a  s to rlgym.api..
-00000240: 2020 2020 2d20 5265 6e61 6d65 2072 6c67      - Rename rlg
-00000250: 796d 2e72 6f63 6b65 745f 6c65 6167 7565  ym.rocket_league
-00000260: 2e65 6e67 696e 6520 746f 2072 6c67 796d  .engine to rlgym
-00000270: 2e72 6f63 6b65 745f 6c65 6167 7565 2e61  .rocket_league.a
-00000280: 7069 0d0a 2020 2020 2d20 496d 7072 6f76  pi..    - Improv
-00000290: 6520 6578 706f 7274 7320 736f 2069 6d70  e exports so imp
-000002a0: 6f72 7473 2061 7265 206d 6f72 6520 636f  orts are more co
-000002b0: 6e73 6f6c 6964 6174 6564 0d0a 2020 2020  nsolidated..    
-000002c0: 2222 222c 0d0a 2020 2020 2732 2e30 2e30  """,..    '2.0.0
-000002d0: 2d61 6c70 6861 2d32 273a 0d0a 2020 2020  -alpha-2':..    
-000002e0: 2222 220d 0a20 2020 202d 2054 6869 7320  """..    - This 
-000002f0: 7665 7273 696f 6e20 636f 6e74 6169 6e73  version contains
-00000300: 206e 756d 6572 6f75 7320 756e 7465 7374   numerous untest
-00000310: 6564 2061 6e64 2070 6f74 656e 7469 616c  ed and potential
-00000320: 6c79 2062 7265 616b 696e 6720 6368 616e  ly breaking chan
-00000330: 6765 732e 2052 756e 2061 7420 796f 7572  ges. Run at your
-00000340: 206f 776e 2072 6973 6b2e 0d0a 2020 2020   own risk...    
-00000350: 2d20 4669 7865 6420 726c 7669 7365 722d  - Fixed rlviser-
-00000360: 7079 2064 6570 656e 6465 6e63 7920 7665  py dependency ve
-00000370: 7273 696f 6e0d 0a20 2020 2022 2222 2c0d  rsion..    """,.
-00000380: 0a20 2020 2027 322e 302e 302d 616c 7068  .    '2.0.0-alph
-00000390: 612d 3127 3a0d 0a20 2020 2022 2222 0d0a  a-1':..    """..
-000003a0: 2020 2020 2d20 5468 6973 2076 6572 7369      - This versi
-000003b0: 6f6e 2063 6f6e 7461 696e 7320 6e75 6d65  on contains nume
-000003c0: 726f 7573 2075 6e74 6573 7465 6420 616e  rous untested an
-000003d0: 6420 706f 7465 6e74 6961 6c6c 7920 6272  d potentially br
-000003e0: 6561 6b69 6e67 2063 6861 6e67 6573 2e20  eaking changes. 
-000003f0: 5275 6e20 6174 2079 6f75 7220 6f77 6e20  Run at your own 
-00000400: 7269 736b 2e0d 0a20 2020 202d 204c 6966  risk...    - Lif
-00000410: 7465 6420 5079 7468 6f6e 203c 332e 3130  ted Python <3.10
-00000420: 2072 6573 7472 6963 7469 6f6e 0d0a 2020   restriction..  
-00000430: 2020 2222 222c 0d0a 2020 2020 2732 2e30    """,..    '2.0
-00000440: 2e30 2d61 6c70 6861 273a 0d0a 2020 2020  .0-alpha':..    
-00000450: 2222 220d 0a20 2020 202d 2054 6869 7320  """..    - This 
-00000460: 7665 7273 696f 6e20 636f 6e74 6169 6e73  version contains
-00000470: 206e 756d 6572 6f75 7320 756e 7465 7374   numerous untest
-00000480: 6564 2061 6e64 2062 7265 616b 696e 6720  ed and breaking 
-00000490: 6368 616e 6765 732e 2052 756e 2061 7420  changes. Run at 
-000004a0: 796f 7572 206f 776e 2072 6973 6b2e 0d0a  your own risk...
-000004b0: 2020 2020 2222 220d 0a7d 0d0a                """..}..
+00000010: 2732 2e30 2e30 2d72 6327 0d0a 0d0a 0d0a  '2.0.0-rc'......
+00000020: 6465 6620 6765 745f 6375 7272 656e 745f  def get_current_
+00000030: 7265 6c65 6173 655f 6e6f 7465 7328 293a  release_notes():
+00000040: 0d0a 2020 2020 6966 205f 5f76 6572 7369  ..    if __versi
+00000050: 6f6e 5f5f 2069 6e20 7265 6c65 6173 655f  on__ in release_
+00000060: 6e6f 7465 733a 0d0a 2020 2020 2020 2020  notes:..        
+00000070: 7265 7475 726e 2072 656c 6561 7365 5f6e  return release_n
+00000080: 6f74 6573 5b5f 5f76 6572 7369 6f6e 5f5f  otes[__version__
+00000090: 5d0d 0a20 2020 2072 6574 7572 6e20 2727  ]..    return ''
+000000a0: 0d0a 0d0a 0d0a 6465 6620 7072 696e 745f  ......def print_
+000000b0: 6375 7272 656e 745f 7265 6c65 6173 655f  current_release_
+000000c0: 6e6f 7465 7328 293a 0d0a 2020 2020 7072  notes():..    pr
+000000d0: 696e 7428 6622 5665 7273 696f 6e20 7b5f  int(f"Version {_
+000000e0: 5f76 6572 7369 6f6e 5f5f 7d22 290d 0a20  _version__}").. 
+000000f0: 2020 2070 7269 6e74 2867 6574 5f63 7572     print(get_cur
+00000100: 7265 6e74 5f72 656c 6561 7365 5f6e 6f74  rent_release_not
+00000110: 6573 2829 290d 0a20 2020 2070 7269 6e74  es())..    print
+00000120: 2822 2229 0d0a 0d0a 0d0a 7265 6c65 6173  ("")......releas
+00000130: 655f 6e6f 7465 7320 3d20 7b0d 0a20 2020  e_notes = {..   
+00000140: 2027 322e 302e 302d 7263 273a 0d0a 2020   '2.0.0-rc':..  
+00000150: 2020 2222 220d 0a20 2020 202d 2055 7064    """..    - Upd
+00000160: 6174 6564 2052 6f63 6b65 7453 696d 2061  ated RocketSim a
+00000170: 6e64 2052 4c56 6973 6572 2064 6570 656e  nd RLViser depen
+00000180: 6465 6e63 6965 7320 5b56 6972 785d 0d0a  dencies [Virx]..
+00000190: 2020 2020 2d20 4164 6465 6420 4261 6c6c      - Added Ball
+000001a0: 2052 6f74 4d74 7820 746f 2052 6f63 6b65   RotMtx to Rocke
+000001b0: 7453 696d 2065 6e67 696e 6520 616e 6420  tSim engine and 
+000001c0: 524c 5669 7365 7220 7265 6e64 6572 6572  RLViser renderer
+000001d0: 205b 5669 7278 5d0d 0a20 2020 202d 2046   [Virx]..    - F
+000001e0: 6978 6564 2062 756d 7020 7669 6374 696d  ixed bump victim
+000001f0: 2049 4420 696e 2052 6f63 6b65 7453 696d   ID in RocketSim
+00000200: 2065 6e67 696e 6520 5b4c 616d 705d 0d0a   engine [Lamp]..
+00000210: 2020 2020 2d20 4164 6465 6420 6d6f 7265      - Added more
+00000220: 2075 7365 6675 6c20 636f 6e73 7461 6e74   useful constant
+00000230: 7320 746f 2063 6f6d 6d6f 6e5f 7661 6c75  s to common_valu
+00000240: 6573 0d0a 2020 2020 2d20 5265 6d6f 7665  es..    - Remove
+00000250: 6420 524c 5669 7365 7220 6465 7065 6e64  d RLViser depend
+00000260: 656e 6379 2066 726f 6d20 7369 6d20 696e  ency from sim in
+00000270: 7374 616c 6c0d 0a20 2020 202d 2049 6d70  stall..    - Imp
+00000280: 726f 7665 6420 5265 7065 6174 4163 7469  roved RepeatActi
+00000290: 6f6e 2c20 6974 206e 6f77 2064 6f65 736e  on, it now doesn
+000002a0: 2774 2065 7870 6563 7420 796f 7572 2041  't expect your A
+000002b0: 6374 696f 6e50 6172 7365 7220 746f 2068  ctionParser to h
+000002c0: 616e 646c 6520 6d75 6c74 6970 6c65 2074  andle multiple t
+000002d0: 6963 6b73 0d0a 2020 2020 2d20 496d 7072  icks..    - Impr
+000002e0: 6f76 6564 2064 6566 6175 6c74 204f 6273  oved default Obs
+000002f0: 5370 6163 6520 616e 6420 4163 7469 6f6e  Space and Action
+00000300: 5370 6163 6520 6465 6669 6e69 7469 6f6e  Space definition
+00000310: 730d 0a20 2020 2022 2222 2c0d 0a20 2020  s..    """,..   
+00000320: 2027 322e 302e 302d 616c 7068 612d 3327   '2.0.0-alpha-3'
+00000330: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+00000340: 2d20 5468 6973 2076 6572 7369 6f6e 2063  - This version c
+00000350: 6f6e 7461 696e 7320 6e75 6d65 726f 7573  ontains numerous
+00000360: 2075 6e74 6573 7465 6420 616e 6420 6272   untested and br
+00000370: 6561 6b69 6e67 2063 6861 6e67 6573 2e20  eaking changes. 
+00000380: 5275 6e20 6174 2079 6f75 7220 6f77 6e20  Run at your own 
+00000390: 7269 736b 2e0d 0a20 2020 202d 2041 6464  risk...    - Add
+000003a0: 6564 2073 6861 7265 645f 696e 666f 2070  ed shared_info p
+000003b0: 6172 616d 2074 6f20 5472 616e 7369 7469  aram to Transiti
+000003c0: 6f6e 456e 6769 6e65 2061 6e64 2052 656e  onEngine and Ren
+000003d0: 6465 7265 720d 0a20 2020 202d 2046 6978  derer..    - Fix
+000003e0: 6564 2050 7974 686f 6e20 3c33 2e39 2069  ed Python <3.9 i
+000003f0: 6e73 7461 6c6c 0d0a 2020 2020 2d20 5570  nstall..    - Up
+00000400: 6461 7465 2069 6d70 6f72 7473 2074 6f20  date imports to 
+00000410: 726c 6779 6d2e 6170 690d 0a20 2020 202d  rlgym.api..    -
+00000420: 2052 656e 616d 6520 726c 6779 6d2e 726f   Rename rlgym.ro
+00000430: 636b 6574 5f6c 6561 6775 652e 656e 6769  cket_league.engi
+00000440: 6e65 2074 6f20 726c 6779 6d2e 726f 636b  ne to rlgym.rock
+00000450: 6574 5f6c 6561 6775 652e 6170 690d 0a20  et_league.api.. 
+00000460: 2020 202d 2049 6d70 726f 7665 2065 7870     - Improve exp
+00000470: 6f72 7473 2073 6f20 696d 706f 7274 7320  orts so imports 
+00000480: 6172 6520 6d6f 7265 2063 6f6e 736f 6c69  are more consoli
+00000490: 6461 7465 640d 0a20 2020 2022 2222 2c0d  dated..    """,.
+000004a0: 0a20 2020 2027 322e 302e 302d 616c 7068  .    '2.0.0-alph
+000004b0: 612d 3227 3a0d 0a20 2020 2022 2222 0d0a  a-2':..    """..
+000004c0: 2020 2020 2d20 5468 6973 2076 6572 7369      - This versi
+000004d0: 6f6e 2063 6f6e 7461 696e 7320 6e75 6d65  on contains nume
+000004e0: 726f 7573 2075 6e74 6573 7465 6420 616e  rous untested an
+000004f0: 6420 706f 7465 6e74 6961 6c6c 7920 6272  d potentially br
+00000500: 6561 6b69 6e67 2063 6861 6e67 6573 2e20  eaking changes. 
+00000510: 5275 6e20 6174 2079 6f75 7220 6f77 6e20  Run at your own 
+00000520: 7269 736b 2e0d 0a20 2020 202d 2046 6978  risk...    - Fix
+00000530: 6564 2072 6c76 6973 6572 2d70 7920 6465  ed rlviser-py de
+00000540: 7065 6e64 656e 6379 2076 6572 7369 6f6e  pendency version
+00000550: 0d0a 2020 2020 2222 222c 0d0a 2020 2020  ..    """,..    
+00000560: 2732 2e30 2e30 2d61 6c70 6861 2d31 273a  '2.0.0-alpha-1':
+00000570: 0d0a 2020 2020 2222 220d 0a20 2020 202d  ..    """..    -
+00000580: 2054 6869 7320 7665 7273 696f 6e20 636f   This version co
+00000590: 6e74 6169 6e73 206e 756d 6572 6f75 7320  ntains numerous 
+000005a0: 756e 7465 7374 6564 2061 6e64 2070 6f74  untested and pot
+000005b0: 656e 7469 616c 6c79 2062 7265 616b 696e  entially breakin
+000005c0: 6720 6368 616e 6765 732e 2052 756e 2061  g changes. Run a
+000005d0: 7420 796f 7572 206f 776e 2072 6973 6b2e  t your own risk.
+000005e0: 0d0a 2020 2020 2d20 4c69 6674 6564 2050  ..    - Lifted P
+000005f0: 7974 686f 6e20 3c33 2e31 3020 7265 7374  ython <3.10 rest
+00000600: 7269 6374 696f 6e0d 0a20 2020 2022 2222  riction..    """
+00000610: 2c0d 0a20 2020 2027 322e 302e 302d 616c  ,..    '2.0.0-al
+00000620: 7068 6127 3a0d 0a20 2020 2022 2222 0d0a  pha':..    """..
+00000630: 2020 2020 2d20 5468 6973 2076 6572 7369      - This versi
+00000640: 6f6e 2063 6f6e 7461 696e 7320 6e75 6d65  on contains nume
+00000650: 726f 7573 2075 6e74 6573 7465 6420 616e  rous untested an
+00000660: 6420 6272 6561 6b69 6e67 2063 6861 6e67  d breaking chang
+00000670: 6573 2e20 5275 6e20 6174 2079 6f75 7220  es. Run at your 
+00000680: 6f77 6e20 7269 736b 2e0d 0a20 2020 2022  own risk...    "
+00000690: 2222 0d0a 7d0d 0a                        ""..}..
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/PKG-INFO` & `rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rlgym-rocket-league
-Version: 2.0.0a3
+Version: 2.0.0rc0
 Summary: A python API that can be used to treat the game Rocket League as an Openai Gym-like environment for Reinforcement Learning projects.
 Home-page: https://rlgym.org
 Author: Lucas Emery and Matthew Allen
 Author-email: contact@rlgym.org
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/lucas-emery/rocket-league-gym
 Keywords: rocket-league,gym,reinforcement-learning,rlgym
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: sim
+Provides-Extra: rlviser
 Provides-Extra: game
 Provides-Extra: all
 License-File: LICENSE
 
 # The Rocket League Gym
 This is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.
```

### Comparing `rlgym-rocket-league-2.0.0a3/rlgym_rocket_league.egg-info/SOURCES.txt` & `rlgym-rocket-league-2.0.0rc0/rlgym_rocket_league.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,16 +41,17 @@
 rlgym/rocket_league/game/plugin/RLMultiInjector.exe
 rlgym/rocket_league/obs_builders/__init__.py
 rlgym/rocket_league/obs_builders/default_obs.py
 rlgym/rocket_league/reward_functions/__init__.py
 rlgym/rocket_league/reward_functions/combined_reward.py
 rlgym/rocket_league/reward_functions/goal_reward.py
 rlgym/rocket_league/reward_functions/touch_reward.py
+rlgym/rocket_league/rlviser/__init__.py
+rlgym/rocket_league/rlviser/rlviser_renderer.py
 rlgym/rocket_league/sim/__init__.py
-rlgym/rocket_league/sim/rlviser_renderer.py
 rlgym/rocket_league/sim/rocketsim_engine.py
 rlgym/rocket_league/sim/collision_meshes/soccar/mesh_0.cmf
 rlgym/rocket_league/sim/collision_meshes/soccar/mesh_1.cmf
 rlgym/rocket_league/sim/collision_meshes/soccar/mesh_10.cmf
 rlgym/rocket_league/sim/collision_meshes/soccar/mesh_11.cmf
 rlgym/rocket_league/sim/collision_meshes/soccar/mesh_12.cmf
 rlgym/rocket_league/sim/collision_meshes/soccar/mesh_13.cmf
```

### Comparing `rlgym-rocket-league-2.0.0a3/setup.json` & `rlgym-rocket-league-2.0.0rc0/setup.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8789021164021165%*

 * *Differences: {"'extras_require'": "{'sim': ['rocketsim >=2'], 'all': {insert: [(0, 'rocketsim >=2'), (1, "*

 * *                     "'rlviser-py ==0.6.*')], delete: [1, 0]}, 'rlviser': ['rlviser-py ==0.6.*', "*

 * *                     "'rocketsim >=2']}",*

 * * "'install_requires'": "{insert: [(0, 'rlgym-api >=2.0.0-rc,<3')], delete: [0]}",*

 * * "'packages'": "{insert: [(7, 'rlgym.rocket_league.rlviser')]}",*

 * * "'version'": "'2.0.0-rc'"}*

```diff
@@ -1,29 +1,32 @@
 {
     "description": "A python API that can be used to treat the game Rocket League as an Openai Gym-like environment for Reinforcement Learning projects.",
     "extras_require": {
         "all": [
-            "rocketsim >=1.2,<2",
-            "rlviser-py >=0.2.3,<0.3",
+            "rocketsim >=2",
+            "rlviser-py ==0.6.*",
             "pywin32 >=228",
             "pywinauto >=0.6.8,<0.7",
             "psutil >=5.8,<6"
         ],
         "game": [
             "pywin32 >=228",
             "pywinauto >=0.6.8,<0.7",
             "psutil >=5.8,<6"
         ],
+        "rlviser": [
+            "rlviser-py ==0.6.*",
+            "rocketsim >=2"
+        ],
         "sim": [
-            "rocketsim >=1.2,<2",
-            "rlviser-py >=0.2.3,<0.3"
+            "rocketsim >=2"
         ]
     },
     "install_requires": [
-        "rlgym-api >=2.0.0-alpha-1,<3",
+        "rlgym-api >=2.0.0-rc,<3",
         "numpy >=1.19,<2"
     ],
     "long_description": "# The Rocket League Gym\nThis is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.\n\n## Requirements\n* A Windows 10 PC\n* Rocket League (Both Steam and Epic are supported)\n* [Bakkesmod](https://www.bakkesmod.com)\n* The RLGym plugin for Bakkesmod (It's installed automatically by pip)\n* Python between versions 3.7 and 3.9 (3.10 not supported).\n\n## Installation\nInstall the library via pip:\n```\npip install rlgym-rocket-league[all]\n```\nOnce the API is installed, you will need to enable the RLGym plugin from inside the Bakkesmod plugin manager. To do this, first launch the game, then press F2 to open the Bakkesmod menu. Navigate to the `plugins` tab and open the `Plugin Manager`. From there, scroll down until you find the RLGym plugin, and enable it. Close the game when this is done.\n\nRLGym is now installed! simply run ```example.py``` from our repo to ensure everything works.\n\n## Usage\nFor tutorials and documentation, please visit our [Wiki](https://rlgym.org/).\n",
     "long_description_content_type": "text/markdown",
     "name": "rlgym-rocket-league",
     "package_data": {
         "rlgym.rocket_league": [
@@ -36,17 +39,18 @@
         "rlgym.rocket_league",
         "rlgym.rocket_league.action_parsers",
         "rlgym.rocket_league.api",
         "rlgym.rocket_league.done_conditions",
         "rlgym.rocket_league.game",
         "rlgym.rocket_league.obs_builders",
         "rlgym.rocket_league.reward_functions",
+        "rlgym.rocket_league.rlviser",
         "rlgym.rocket_league.sim",
         "rlgym.rocket_league.state_mutators",
         "rlgym.rocket_league.game.communication",
         "rlgym.rocket_league.game.launch",
         "rlgym.rocket_league.game.plugin",
         "rlgym.rocket_league.sim.collision_meshes",
         "rlgym.rocket_league.sim.collision_meshes.soccar"
     ],
-    "version": "2.0.0-alpha-3"
+    "version": "2.0.0-rc"
 }
```

### Comparing `rlgym-rocket-league-2.0.0a3/setup.py` & `rlgym-rocket-league-2.0.0rc0/setup.py`

 * *Files identical despite different names*


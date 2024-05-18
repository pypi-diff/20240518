# Comparing `tmp/rlgym-api-2.0.0a1.tar.gz` & `tmp/rlgym-api-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlgym-api-2.0.0a1.tar", last modified: Wed Aug 23 18:40:31 2023, max compression
+gzip compressed data, was "rlgym-api-2.0.0rc0.tar", last modified: Sat May 18 16:56:53 2024, max compression
```

## Comparing `rlgym-api-2.0.0a1.tar` & `rlgym-api-2.0.0rc0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-08-23 18:40:31.602864 rlgym-api-2.0.0a1/
--rw-rw-rw-   0        0        0    10946 2021-03-04 22:29:53.000000 rlgym-api-2.0.0a1/LICENSE
--rw-rw-rw-   0        0        0       37 2023-08-19 16:59:10.000000 rlgym-api-2.0.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     1126 2023-08-23 18:40:31.600853 rlgym-api-2.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-08-19 21:03:59.000000 rlgym-api-2.0.0a1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-23 18:40:31.442570 rlgym-api-2.0.0a1/rlgym/
-drwxrwxrwx   0        0        0        0 2023-08-23 18:40:31.486570 rlgym-api-2.0.0a1/rlgym/api/
--rw-rw-rw-   0        0        0      391 2023-08-19 17:20:02.000000 rlgym-api-2.0.0a1/rlgym/api/README.md
--rw-rw-rw-   0        0        0      106 2023-08-23 18:35:28.000000 rlgym-api-2.0.0a1/rlgym/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:40:31.533574 rlgym-api-2.0.0a1/rlgym/api/config/
--rw-rw-rw-   0        0        0      288 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/config/__init__.py
--rw-rw-rw-   0        0        0     2099 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/config/action_parser.py
--rw-rw-rw-   0        0        0     1469 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/config/done_condition.py
--rw-rw-rw-   0        0        0     2100 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/config/obs_builder.py
--rw-rw-rw-   0        0        0      405 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/config/renderer.py
--rw-rw-rw-   0        0        0     1682 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/config/reward_function.py
--rw-rw-rw-   0        0        0      715 2023-08-23 18:35:28.000000 rlgym-api-2.0.0a1/rlgym/api/config/state_mutator.py
--rw-rw-rw-   0        0        0     2076 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/config/transition_engine.py
--rw-rw-rw-   0        0        0     4661 2023-08-23 18:35:27.000000 rlgym-api-2.0.0a1/rlgym/api/rlgym.py
--rw-rw-rw-   0        0        0      278 2023-08-16 18:04:12.000000 rlgym-api-2.0.0a1/rlgym/api/typing.py
--rw-rw-rw-   0        0        0      792 2023-08-23 18:35:28.000000 rlgym-api-2.0.0a1/rlgym/api/version.py
-drwxrwxrwx   0        0        0        0 2023-08-23 18:40:31.597856 rlgym-api-2.0.0a1/rlgym_api.egg-info/
--rw-rw-rw-   0        0        0     1126 2023-08-23 18:40:31.000000 rlgym-api-2.0.0a1/rlgym_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-08-23 18:40:31.000000 rlgym-api-2.0.0a1/rlgym_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-23 18:40:31.000000 rlgym-api-2.0.0a1/rlgym_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-23 18:40:31.000000 rlgym-api-2.0.0a1/rlgym_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-23 18:40:31.602864 rlgym-api-2.0.0a1/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-08-23 18:40:23.000000 rlgym-api-2.0.0a1/setup.json
--rw-rw-rw-   0        0        0      805 2023-08-23 18:04:36.000000 rlgym-api-2.0.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:56:53.848097 rlgym-api-2.0.0rc0/
+-rw-rw-rw-   0        0        0    10946 2021-03-04 22:29:53.000000 rlgym-api-2.0.0rc0/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-08-19 16:59:10.000000 rlgym-api-2.0.0rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1127 2024-05-18 16:56:53.847107 rlgym-api-2.0.0rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     1954 2023-12-03 17:45:55.000000 rlgym-api-2.0.0rc0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:56:53.816096 rlgym-api-2.0.0rc0/rlgym/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:56:53.829107 rlgym-api-2.0.0rc0/rlgym/api/
+-rw-rw-rw-   0        0        0      391 2023-08-19 17:20:02.000000 rlgym-api-2.0.0rc0/rlgym/api/README.md
+-rw-rw-rw-   0        0        0      106 2023-08-23 18:35:28.000000 rlgym-api-2.0.0rc0/rlgym/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:56:53.840095 rlgym-api-2.0.0rc0/rlgym/api/config/
+-rw-rw-rw-   0        0        0      342 2024-04-14 14:39:21.000000 rlgym-api-2.0.0rc0/rlgym/api/config/__init__.py
+-rw-rw-rw-   0        0        0     2236 2024-05-18 15:55:37.000000 rlgym-api-2.0.0rc0/rlgym/api/config/action_parser.py
+-rw-rw-rw-   0        0        0     1580 2024-05-18 15:43:18.000000 rlgym-api-2.0.0rc0/rlgym/api/config/done_condition.py
+-rw-rw-rw-   0        0        0     2218 2024-05-18 15:43:18.000000 rlgym-api-2.0.0rc0/rlgym/api/config/obs_builder.py
+-rw-rw-rw-   0        0        0      405 2023-08-23 18:35:27.000000 rlgym-api-2.0.0rc0/rlgym/api/config/renderer.py
+-rw-rw-rw-   0        0        0     1793 2024-05-18 15:43:18.000000 rlgym-api-2.0.0rc0/rlgym/api/config/reward_function.py
+-rw-rw-rw-   0        0        0     1728 2024-05-18 15:55:37.000000 rlgym-api-2.0.0rc0/rlgym/api/config/shared_info_provider.py
+-rw-rw-rw-   0        0        0      715 2023-09-17 13:58:30.000000 rlgym-api-2.0.0rc0/rlgym/api/config/state_mutator.py
+-rw-rw-rw-   0        0        0     2076 2023-08-23 18:35:27.000000 rlgym-api-2.0.0rc0/rlgym/api/config/transition_engine.py
+-rw-rw-rw-   0        0        0     6108 2024-05-18 15:43:18.000000 rlgym-api-2.0.0rc0/rlgym/api/rlgym.py
+-rw-rw-rw-   0        0        0      330 2024-04-13 18:37:30.000000 rlgym-api-2.0.0rc0/rlgym/api/typing.py
+-rw-rw-rw-   0        0        0     1051 2024-05-18 16:37:43.000000 rlgym-api-2.0.0rc0/rlgym/api/version.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:56:53.846108 rlgym-api-2.0.0rc0/rlgym_api.egg-info/
+-rw-rw-rw-   0        0        0     1127 2024-05-18 16:56:53.000000 rlgym-api-2.0.0rc0/rlgym_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-18 16:56:53.000000 rlgym-api-2.0.0rc0/rlgym_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:56:53.000000 rlgym-api-2.0.0rc0/rlgym_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-18 16:56:53.000000 rlgym-api-2.0.0rc0/rlgym_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:56:53.848097 rlgym-api-2.0.0rc0/setup.cfg
+-rw-rw-rw-   0        0        0      735 2024-05-18 16:56:48.000000 rlgym-api-2.0.0rc0/setup.json
+-rw-rw-rw-   0        0        0      805 2023-08-23 18:04:36.000000 rlgym-api-2.0.0rc0/setup.py
```

### Comparing `rlgym-api-2.0.0a1/LICENSE` & `rlgym-api-2.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `rlgym-api-2.0.0a1/PKG-INFO` & `rlgym-api-2.0.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym-api
-Version: 2.0.0a1
+Version: 2.0.0rc0
 Summary: A python API with zero dependencies to create fully customizable environments for Reinforcement Learning projects.
 Home-page: https://rlgym.org
 Author: Lucas Emery and Matthew Allen
 Author-email: contact@rlgym.org
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/lucas-emery/rocket-league-gym
 Keywords: rocket-league,gym,reinforcement-learning,rlgym
```

### Comparing `rlgym-api-2.0.0a1/README.md` & `rlgym-api-2.0.0rc0/README.md`

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

### Comparing `rlgym-api-2.0.0a1/rlgym/api/config/action_parser.py` & `rlgym-api-2.0.0rc0/rlgym/api/config/action_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 The action parser.
 """
 from abc import abstractmethod
-from typing import Any, Dict, Generic
-from ..typing import AgentID, ActionType, EngineActionType, StateType, SpaceType
+from typing import Any, Dict, Generic, List
+from ..typing import AgentID, ActionType, EngineActionType, StateType, ActionSpaceType
 
 
-class ActionParser(Generic[AgentID, ActionType, EngineActionType, StateType, SpaceType]):
+class ActionParser(Generic[AgentID, ActionType, EngineActionType, StateType, ActionSpaceType]):
 
     @abstractmethod
-    def get_action_space(self, agent: AgentID) -> SpaceType:
+    def get_action_space(self, agent: AgentID) -> ActionSpaceType:
         """
         Function that returns the action space type. It will be called during the initialization of the environment.
 
         :return: The type of the action space
         """
         raise NotImplementedError
 
     @abstractmethod
-    def reset(self, initial_state: StateType, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: StateType, shared_info: Dict[str, Any]) -> None:
         """
         Function to be called each time the environment is reset.
 
+        :param agents: List of AgentIDs for which this ActionParser will receive actions
         :param initial_state: The initial state of the reset environment.
         :param shared_info: A dictionary with shared information across all config objects.
         """
         raise NotImplementedError
 
     @abstractmethod
     def parse_actions(self, actions: Dict[AgentID, ActionType], state: StateType, shared_info: Dict[str, Any]) -> Dict[AgentID, EngineActionType]:
```

### Comparing `rlgym-api-2.0.0a1/rlgym/api/config/done_condition.py` & `rlgym-api-2.0.0rc0/rlgym/api/config/done_condition.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from typing import Any, Dict, List, Generic
 from ..typing import AgentID, StateType
 
 
 class DoneCondition(Generic[AgentID, StateType]):
 
     @abstractmethod
-    def reset(self, initial_state: StateType, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: StateType, shared_info: Dict[str, Any]) -> None:
         """
         Function to be called each time the environment is reset.
 
+        :param agents: List of AgentIDs for which this DoneCondition will be evaluated
         :param initial_state: The initial state of the reset environment.
         :param shared_info: A dictionary with shared information across all config objects.
         """
         raise NotImplementedError
 
     @abstractmethod
     def is_done(self, agents: List[AgentID], state: StateType, shared_info: Dict[str, Any]) -> Dict[AgentID, bool]:
```

### Comparing `rlgym-api-2.0.0a1/rlgym/api/config/obs_builder.py` & `rlgym-api-2.0.0rc0/rlgym/api/config/obs_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 The observation builder.
 """
 from abc import abstractmethod
 from typing import Any, Dict, List, Generic
-from ..typing import AgentID, ObsType, StateType, SpaceType
+from ..typing import AgentID, ObsType, StateType, ObsSpaceType
 
 
-class ObsBuilder(Generic[AgentID, ObsType, StateType, SpaceType]):
+class ObsBuilder(Generic[AgentID, ObsType, StateType, ObsSpaceType]):
 
     @abstractmethod
-    def get_obs_space(self, agent: AgentID) -> SpaceType:
+    def get_obs_space(self, agent: AgentID) -> ObsSpaceType:
         """
         Function that returns the observation space type. It will be called during the initialization of the environment.
 
         :return: The type of the observation space
         """
         raise NotImplementedError
 
     @abstractmethod
-    def reset(self, initial_state: StateType, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: StateType, shared_info: Dict[str, Any]) -> None:
         """
         Function to be called each time the environment is reset. Note that this does not need to return anything,
         the environment will call `build_obs` automatically after reset, so the initial observation for a policy will be
         constructed in the same way as every other observation.
 
+        :param agents: List of AgentIDs for which this ObsBuilder will return an Obs
         :param initial_state: The initial game state of the reset environment.
         :param shared_info: A dictionary with shared information across all config objects.
         """
         raise NotImplementedError
 
     @abstractmethod
     def build_obs(self, agents: List[AgentID], state: StateType, shared_info: Dict[str, Any]) -> Dict[AgentID, ObsType]:
```

### Comparing `rlgym-api-2.0.0a1/rlgym/api/config/reward_function.py` & `rlgym-api-2.0.0rc0/rlgym/api/config/reward_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from typing import Any, Dict, List, Generic
 from ..typing import AgentID, RewardType, StateType
 
 
 class RewardFunction(Generic[AgentID, StateType, RewardType]):
 
     @abstractmethod
-    def reset(self, initial_state: StateType, shared_info: Dict[str, Any]) -> None:
+    def reset(self, agents: List[AgentID], initial_state: StateType, shared_info: Dict[str, Any]) -> None:
         """
         Function to be called each time the environment is reset. This is meant to enable users to design stateful reward
         functions that maintain information about the game throughout an episode to determine a reward.
 
+        :param agents: List of AgentIDs for which this RewardFunc will return a Reward
         :param initial_state: The initial state of the reset environment.
         :param shared_info: A dictionary with shared information across all config objects.
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_rewards(self, agents: List[AgentID], state: StateType, is_terminated: Dict[AgentID, bool], is_truncated: Dict[AgentID, bool], shared_info: Dict[str, Any]) -> Dict[AgentID, RewardType]:
```

### Comparing `rlgym-api-2.0.0a1/rlgym/api/config/state_mutator.py` & `rlgym-api-2.0.0rc0/rlgym/api/config/state_mutator.py`

 * *Files identical despite different names*

### Comparing `rlgym-api-2.0.0a1/rlgym/api/config/transition_engine.py` & `rlgym-api-2.0.0rc0/rlgym/api/config/transition_engine.py`

 * *Files identical despite different names*

### Comparing `rlgym-api-2.0.0a1/rlgym/api/rlgym.py` & `rlgym-api-2.0.0rc0/rlgym/api/rlgym.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
     The Rocket League gym environment.
 """
 from typing import Any, List, Dict, Tuple, Generic, Optional
+from .config import ActionParser, DoneCondition, ObsBuilder, RewardFunction, StateMutator, Renderer, TransitionEngine, SharedInfoProvider
+from .typing import AgentID, ObsType, ActionType, EngineActionType, RewardType, StateType, ObsSpaceType, ActionSpaceType
 
-from .config import ActionParser, DoneCondition, ObsBuilder, RewardFunction, StateMutator, Renderer, TransitionEngine
-from .typing import AgentID, ObsType, ActionType, EngineActionType, RewardType, StateType, SpaceType
 
-
-class RLGym(Generic[AgentID, ObsType, ActionType, EngineActionType, RewardType, StateType, SpaceType]):
+class RLGym(Generic[AgentID, ObsType, ActionType, EngineActionType, RewardType, StateType, ObsSpaceType, ActionSpaceType]):
     #TODO docs
 
     def __init__(self,
                  state_mutator: StateMutator[StateType],
-                 obs_builder: ObsBuilder[AgentID, ObsType, StateType, SpaceType],
-                 action_parser: ActionParser[AgentID, ActionType, EngineActionType, StateType, SpaceType],
+                 obs_builder: ObsBuilder[AgentID, ObsType, StateType, ObsSpaceType],
+                 action_parser: ActionParser[AgentID, ActionType, EngineActionType, StateType, ActionSpaceType],
                  reward_fn: RewardFunction[AgentID, StateType, RewardType],
-                 termination_cond: DoneCondition[AgentID, StateType],
-                 truncation_cond: DoneCondition[AgentID, StateType],
                  transition_engine: TransitionEngine[AgentID, StateType, EngineActionType],
-                 renderer: Optional[Renderer[StateType]]):
+                 termination_cond: Optional[DoneCondition[AgentID, StateType]] = None,
+                 truncation_cond: Optional[DoneCondition[AgentID, StateType]] = None,
+                 shared_info_provider: Optional[SharedInfoProvider[AgentID, StateType]] = None,
+                 renderer: Optional[Renderer[StateType]] = None):
         """
         TODO docs
         :param state_mutator:
         :param obs_builder:
         :param action_parser:
         :param reward_fn:
         :param termination_cond:
@@ -30,75 +30,90 @@
         :param transition_engine:
         :param renderer:
         """
         self.state_mutator = state_mutator
         self.obs_builder = obs_builder
         self.action_parser = action_parser
         self.reward_fn = reward_fn
+        self.transition_engine = transition_engine
         self.termination_cond = termination_cond
         self.truncation_cond = truncation_cond
-        self.transition_engine = transition_engine
         self.renderer = renderer
-        self.shared_info = {}
+        self.shared_info_provider = shared_info_provider
+        self.shared_info = shared_info_provider.create({}) if shared_info_provider is not None else {}
 
     @property
     def agents(self) -> List[AgentID]:
         return self.transition_engine.agents
 
     @property
-    def action_spaces(self) -> Dict[AgentID, SpaceType]:
+    def action_spaces(self) -> Dict[AgentID, ActionSpaceType]:
         spaces = {}
         for agent in self.agents:
             spaces[agent] = self.action_space(agent)
         return spaces
 
     @property
-    def observation_spaces(self) -> Dict[AgentID, SpaceType]:
+    def observation_spaces(self) -> Dict[AgentID, ObsSpaceType]:
         spaces = {}
         for agent in self.agents:
             spaces[agent] = self.observation_space(agent)
         return spaces
 
     @property
     def state(self) -> StateType:
         return self.transition_engine.state
 
     #TODO add snapshot property to all objects, save state and probably shared_info
 
-    def action_space(self, agent: AgentID) -> SpaceType:
+    def action_space(self, agent: AgentID) -> ActionSpaceType:
         return self.action_parser.get_action_space(agent)
 
-    def observation_space(self, agent: AgentID) -> SpaceType:
+    def observation_space(self, agent: AgentID) -> ObsSpaceType:
         return self.obs_builder.get_obs_space(agent)
 
     def set_state(self, desired_state: StateType) -> Dict[AgentID, ObsType]:
+        if self.shared_info_provider is not None:
+            self.shared_info = self.shared_info_provider.create(self.shared_info)
         state = self.transition_engine.set_state(desired_state, self.shared_info)
-
-        return self.obs_builder.build_obs(self.agents, state, self.shared_info)
+        agents = self.agents
+        if self.shared_info_provider is not None:
+            self.shared_info = self.shared_info_provider.set_state(agents, state, self.shared_info)
+        return self.obs_builder.build_obs(agents, state, self.shared_info)
 
     def reset(self) -> Dict[AgentID, ObsType]:
+        if self.shared_info_provider is not None:
+            self.shared_info = self.shared_info_provider.create(self.shared_info)
         desired_state = self.transition_engine.create_base_state()
         self.state_mutator.apply(desired_state, self.shared_info)
         state = self.transition_engine.set_state(desired_state, self.shared_info)
+        agents = self.agents
+        if self.shared_info_provider is not None:
+            self.shared_info = self.shared_info_provider.set_state(agents, state, self.shared_info)
+        self.obs_builder.reset(agents, state, self.shared_info)
+        self.action_parser.reset(agents, state, self.shared_info)
+        if self.termination_cond is not None:
+            self.termination_cond.reset(agents, state, self.shared_info)
+        if self.truncation_cond is not None:
+            self.truncation_cond.reset(agents, state, self.shared_info)
+        self.reward_fn.reset(agents, state, self.shared_info)
 
-        self.obs_builder.reset(state, self.shared_info)
-        self.action_parser.reset(state, self.shared_info)
-        self.termination_cond.reset(state, self.shared_info)
-        self.truncation_cond.reset(state, self.shared_info)
-        self.reward_fn.reset(state, self.shared_info)
-
-        return self.obs_builder.build_obs(self.agents, state, self.shared_info)
+        return self.obs_builder.build_obs(agents, state, self.shared_info)
 
     def step(self, actions: Dict[AgentID, ActionType]) -> Tuple[Dict[AgentID, ObsType], Dict[AgentID, RewardType], Dict[AgentID, bool], Dict[AgentID, bool]]:
         engine_actions = self.action_parser.parse_actions(actions, self.state, self.shared_info)
         new_state = self.transition_engine.step(engine_actions, self.shared_info)
         agents = self.agents
+        if self.shared_info_provider is not None:
+            self.shared_info = self.shared_info_provider.step(agents, new_state, self.shared_info)
         obs = self.obs_builder.build_obs(agents, new_state, self.shared_info)
-        is_terminated = self.termination_cond.is_done(agents, new_state, self.shared_info)
-        is_truncated = self.truncation_cond.is_done(agents, new_state, self.shared_info)
+        is_terminated = self.termination_cond.is_done(agents, new_state, self.shared_info) \
+            if self.termination_cond is not None else {agent: False for agent in agents}
+        is_truncated = self.truncation_cond.is_done(agents, new_state, self.shared_info) \
+            if self.truncation_cond is not None else {agent: False for agent in agents}
         rewards = self.reward_fn.get_rewards(agents, new_state, is_terminated, is_truncated, self.shared_info)
         return obs, rewards, is_terminated, is_truncated
 
     def render(self) -> Any:
         self.renderer.render(self.state, self.shared_info)
 
     def close(self) -> None:
```

### Comparing `rlgym-api-2.0.0a1/rlgym_api.egg-info/PKG-INFO` & `rlgym-api-2.0.0rc0/rlgym_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym-api
-Version: 2.0.0a1
+Version: 2.0.0rc0
 Summary: A python API with zero dependencies to create fully customizable environments for Reinforcement Learning projects.
 Home-page: https://rlgym.org
 Author: Lucas Emery and Matthew Allen
 Author-email: contact@rlgym.org
 License: Apache 2.0
 Project-URL: Source Code, https://github.com/lucas-emery/rocket-league-gym
 Keywords: rocket-league,gym,reinforcement-learning,rlgym
```

### Comparing `rlgym-api-2.0.0a1/rlgym_api.egg-info/SOURCES.txt` & `rlgym-api-2.0.0rc0/rlgym_api.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 rlgym/api/version.py
 rlgym/api/config/__init__.py
 rlgym/api/config/action_parser.py
 rlgym/api/config/done_condition.py
 rlgym/api/config/obs_builder.py
 rlgym/api/config/renderer.py
 rlgym/api/config/reward_function.py
+rlgym/api/config/shared_info_provider.py
 rlgym/api/config/state_mutator.py
 rlgym/api/config/transition_engine.py
 rlgym_api.egg-info/PKG-INFO
 rlgym_api.egg-info/SOURCES.txt
 rlgym_api.egg-info/dependency_links.txt
 rlgym_api.egg-info/top_level.txt
```

### Comparing `rlgym-api-2.0.0a1/setup.json` & `rlgym-api-2.0.0rc0/setup.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'version'": "'2.0.0-rc'"}*

```diff
@@ -8,9 +8,9 @@
             "README.md"
         ]
     },
     "packages": [
         "rlgym.api",
         "rlgym.api.config"
     ],
-    "version": "2.0.0-alpha-1"
+    "version": "2.0.0-rc"
 }
```

### Comparing `rlgym-api-2.0.0a1/setup.py` & `rlgym-api-2.0.0rc0/setup.py`

 * *Files identical despite different names*


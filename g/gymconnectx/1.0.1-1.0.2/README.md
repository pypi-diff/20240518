# Comparing `tmp/gymconnectx-1.0.1.tar.gz` & `tmp/gymconnectx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymconnectx-1.0.1.tar", last modified: Fri May 17 14:46:03 2024, max compression
+gzip compressed data, was "gymconnectx-1.0.2.tar", last modified: Fri May 17 16:54:00 2024, max compression
```

## Comparing `gymconnectx-1.0.1.tar` & `gymconnectx-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/gymconnectx/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/gymconnectx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/gymconnectx/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/gymconnectx/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25493 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/gymconnectx/envs/gymconnectxenv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/gymconnectx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:54:00.627990 gymconnectx-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 16:53:55.000000 gymconnectx-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-17 16:54:00.627990 gymconnectx-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-17 16:53:55.000000 gymconnectx-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:54:00.627990 gymconnectx-1.0.2/gymconnectx/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-17 16:53:55.000000 gymconnectx-1.0.2/gymconnectx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:54:00.627990 gymconnectx-1.0.2/gymconnectx/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 16:53:55.000000 gymconnectx-1.0.2/gymconnectx/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25373 2024-05-17 16:53:55.000000 gymconnectx-1.0.2/gymconnectx/envs/gymconnectxenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:54:00.627990 gymconnectx-1.0.2/gymconnectx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-17 16:54:00.000000 gymconnectx-1.0.2/gymconnectx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-17 16:54:00.000000 gymconnectx-1.0.2/gymconnectx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 16:54:00.000000 gymconnectx-1.0.2/gymconnectx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 16:54:00.000000 gymconnectx-1.0.2/gymconnectx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 16:54:00.000000 gymconnectx-1.0.2/gymconnectx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 16:53:55.000000 gymconnectx-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 16:54:00.627990 gymconnectx-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-17 16:53:55.000000 gymconnectx-1.0.2/setup.py
```

### Comparing `gymconnectx-1.0.1/LICENSE.md` & `gymconnectx-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.1/gymconnectx/envs/gymconnectxenv.py` & `gymconnectx-1.0.2/gymconnectx/envs/gymconnectxenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,18 +260,15 @@
 
         self.max_steps = max_steps
         self.current_step = 0
         self.is_done = False
 
         self.delay = delay
 
-        self.observation_space = Tuple([Box(low=0, high=1,
-                                            shape=(3, self.width, self.height),
-                                            dtype=np.int32)
-                                        for _ in range(2)])
+        self.observation_space = Box(low=0, high=255, shape=(height, width, 1), dtype=np.uint8)
         self.action_space = Tuple([Discrete(self.width) for _ in range(2)])
         self.state_space_size = (self.height * self.width) ** 3
 
         self.renderer = PyGameRenderEnv(self, square_size, avatar_player_1, avatar_player_2)
         self.reset()
 
     def step(self, movecol):
@@ -289,38 +286,38 @@
         Raises:
             IndexError: If the move is invalid (e.g., the column is full or out of bounds).
 
         This method updates the game state by inserting a chip into the chosen column, checks for a winner, updates the current
         player, and calculates the rewards based on the state of the game. It also updates the display through the renderer and
         prepares the info dictionary for the next player's move.
         """
-        if not (0 <= movecol <= self.width and self.board[movecol][self.height - 1] == -1):
+        if not (0 <= movecol < self.width and self.board[movecol][self.height - 1] == -1):
             raise IndexError(
                 f'Invalid move. tried to place a chip on column {movecol} which is already full. Valid moves are: {self.get_moves()}')
+
         row = self.height - 1
         while row >= 0 and self.board[movecol][row] == -1:
             row -= 1
-
         row += 1
 
         self.board[movecol][row] = self.current_player
         self.current_player = 1 - self.current_player
 
         self.winner, reward_vector = self.check_for_episode_termination(movecol, row)
 
-        info = {'legal_actions': self.get_moves(),
-                'next_player': self.current_player + 1}
-
-        reward_players = {'player_1': reward_vector[0],
-                          'player_2': reward_vector[1]}
-
+        info = {'legal_actions': self.get_moves(), 'next_player': self.current_player + 1}
+        reward_players = {'player_1': reward_vector[0], 'player_2': reward_vector[1]}
         self.is_done = self.winner is not None
         self.renderer.update_display()
 
-        return self.get_player_observations(), reward_players, self.is_done, info
+        obs = self.get_player_observations()
+        terminated = self.is_done
+        truncated = False
+
+        return obs, reward_players, terminated, truncated, info
 
     def reset(self) -> List[np.ndarray]:
         """
         Resets the game environment to its initial state. This method is typically called at the start of each new game.
 
         :return: A list of numpy arrays representing the initial observations of the game board for both players.
                      Each observation is an ndarray showing the current state of the board from the player's perspective.
```

### Comparing `gymconnectx-1.0.1/pyproject.toml` & `gymconnectx-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gymconnectx"
-version = "1.0.1"
+version = "1.0.2"
 description = "An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N."
 readme = "README.md"
 authors = [{ name = "Fauzi Sholichin" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```


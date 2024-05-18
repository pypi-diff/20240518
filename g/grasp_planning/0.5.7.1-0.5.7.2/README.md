# Comparing `tmp/grasp_planning-0.5.7.1.tar.gz` & `tmp/grasp_planning-0.5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.7.1.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.7.2.tar", max compression
```

## Comparing `grasp_planning-0.5.7.1.tar` & `grasp_planning-0.5.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1734 2024-05-16 09:02:48.947350 grasp_planning-0.5.7.1/README.md
--rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.7.1/grasp_planning/__init__.py
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.7.1/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.7.1/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.7.1/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.7.1/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.7.1/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.7.1/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.7.1/grasp_planning/constraints/orientation_constraint.py
--rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.7.1/grasp_planning/constraints/position_constraint.py
--rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.7.1/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.7.1/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.7.1/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     7732 2024-05-17 15:38:35.947749 grasp_planning-0.5.7.1/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.7.1/grasp_planning/solver/ik_optim.py
--rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.7.1/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      557 2024-05-17 15:45:28.754712 grasp_planning-0.5.7.1/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 grasp_planning-0.5.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1734 2024-05-16 09:02:48.947350 grasp_planning-0.5.7.2/README.md
+-rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.7.2/grasp_planning/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.7.2/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.7.2/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.7.2/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.7.2/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.7.2/grasp_planning/constraints/orientation_constraint.py
+-rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.7.2/grasp_planning/constraints/position_constraint.py
+-rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.7.2/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.7.2/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.7.2/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     7742 2024-05-17 19:31:19.299293 grasp_planning-0.5.7.2/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     6216 2024-05-18 19:54:55.776462 grasp_planning-0.5.7.2/grasp_planning/solver/ik_optim.py
+-rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.7.2/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      557 2024-05-18 20:02:58.529614 grasp_planning-0.5.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 grasp_planning-0.5.7.2/PKG-INFO
```

### Comparing `grasp_planning-0.5.7.1/README.md` & `grasp_planning-0.5.7.2/README.md`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.7.2/grasp_planning/constraints/collision_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.7.2/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/constraints/orientation_constraint.py` & `grasp_planning-0.5.7.2/grasp_planning/constraints/orientation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/constraints/position_constraint.py` & `grasp_planning-0.5.7.2/grasp_planning/constraints/position_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.7.2/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.7.2/grasp_planning/solver/gomp_planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import spatial_casadi as sc
 from scipy.spatial.transform import Rotation as R
 from grasp_planning.solver.robot_model import RobotKinematicModel
 from grasp_planning.cost.costs import SquaredAccCost
 from grasp_planning.constraints.constraints import *
 
 class GOMP():
-    def __init__(self, n_waypoints, urdf, theta=np.pi/4, roll_obj_grasp = np.pi, root_link='world', end_link='tool_frame') -> None:
+    def __init__(self, n_waypoints, urdf, theta=np.pi/4, pitch_obj_grasp = np.pi, root_link='world', end_link='tool_frame') -> None:
         # Init variables
         self.T_W_Grasp = None
         self.T_W_Obj = None
         self.T_Obj_Grasp = np.eye(4, dtype=float)
         
         # Kinematics
         self._robot_model = RobotKinematicModel(urdf, root_link, end_link)
         self.n_dofs = self._robot_model.n_dofs
         self.manipulation_frame_dim = 6
         self.x_dim = self.n_dofs
         self.n_waypoints = n_waypoints
         self.theta = theta
-        self.roll_obj_grasp = roll_obj_grasp
+        self.pitch_obj_grasp = pitch_obj_grasp
         
         # Optimization
         self.x = ca.SX.sym("x", self.x_dim, self.n_waypoints)
         self.x_init = None
         
         self._objective = None
         self.l_joint_limits, self.u_joint_limits = None, None
@@ -33,30 +33,30 @@
         self.param_grasp_ca = ca.SX.sym("param_grasp", 4, 4)
         self.param_obst_ca = ca.SX.sym("param_obst", 4, 4)
         self._collision_flag = False
         self.param_optim_ca = ca.vertcat()
         self.param_ca_list = []
 
 
-    def update_grasp_DOF(self, theta: float, degrees=True) -> None:
+    def update_grasp_DOF(self, theta: float, pitch_obj_grasp: float, degrees=True) -> None:
         """
         Object has to have z-axis aligned with the world frame
         """
         self.T_Obj_Grasp = np.eye(4, dtype=float)
         if degrees:
             self.theta = np.deg2rad(theta)
-            self.R_Obj_Grasp = R.from_euler('xyz', [0, np.rad2deg(self.roll_obj_grasp), 0.0], degrees=True).as_matrix()
+            self.pitch_obj_grasp = np.deg2rad(pitch_obj_grasp)
         else:
             self.theta = theta
-            self.R_Obj_Grasp = R.from_euler('xyz', [0, self.roll_obj_grasp, 0.0], degrees=False).as_matrix()
+            self.pitch_obj_grasp = pitch_obj_grasp
+
+        self.R_Obj_Grasp = R.from_euler('xyz', [0, self.pitch_obj_grasp, 0.0], degrees=False).as_matrix()
         self.T_Obj_Grasp[:3,:3] = self.R_Obj_Grasp
         self.T_W_Grasp = self.T_W_Obj @ self.T_Obj_Grasp
         
-        # print("T_W_Grasp\n", self.T_W_Grasp)
-
 
     def update_object_pose(self, T_W_Obj: np.array) -> None:
         """
         Update object and grasp poses
         """
         self.T_W_Obj = T_W_Obj
 
@@ -173,14 +173,14 @@
                                                 link_name=child_link,
                                                 r_link= r_link,
                                                 r_obst= r_obst,
                                                 tolerance=tolerance))
 
     def update_constraints_params(self, T_W_Obj, T_W_Obst=None):
         self.update_object_pose(T_W_Obj)
-        self.update_grasp_DOF(theta=self.theta, degrees=False)
+        self.update_grasp_DOF(theta=self.theta,  pitch_obj_grasp=self.pitch_obj_grasp, degrees=False)
 
         if self._collision_flag:
             self.params_optim_num = ca.vertcat(self.T_W_Grasp, T_W_Obst)
         else:
             self.params_optim_num = self.T_W_Grasp
```

### Comparing `grasp_planning-0.5.7.1/grasp_planning/solver/ik_optim.py` & `grasp_planning-0.5.7.2/grasp_planning/solver/ik_optim.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
         self.param_T_W_Ref = ca.SX.sym("param_grasp", 4, 4)
         self.param_obst_ca = ca.SX.sym("param_obst", 4, 4)
         self.param_optim_ca = ca.vertcat()
         self.param_ca_list = [self.param_T_W_Ref]
         self._collision_flag = False
 
-    def set_home_config(self, q):
-        self.q_home = q
+        self.param_ca_dict = dict()
+
 
     def set_init_guess(self, q):
         self.x_init = q
 
     def set_boundary_conditions(self):
         if self.l_joint_limits is None or self.u_joint_limits is None:
             # Reset joint limits
@@ -46,87 +46,114 @@
             joint_limits = self._robot_model.get_joint_pos_limits()
             self.l_joint_limits[:, 0] = joint_limits[:,0]
             self.u_joint_limits[:, 0] = joint_limits[:,1]
 
     
 
     def setup_problem(self, verbose=False):
-        # assert self.T_Obj_Grasp != None, "Grasp DOF is not set. Set additional degree of freedom around object."
-        # assert self.T_W_Obj != None, "Object pose is not set."
-        # 1. create decision variable
-        
-        # assert self.x_init != None, "Initial guess is missing. Set up one using `set_init_guess(q)`."
-
-        # Define objective function
-        cost = DistToHome(q_home=self.q_home,
-                          n_dofs=self.x_dim)
-        objective = cost.eval_cost(self.x)
-
+        # Read Constraints
         g, self.g_lb, self.g_ub = ca.vertcat(), ca.vertcat(), ca.vertcat()
         for g_term in self.g_list:
             gt, g_lb, g_ub = g_term.get_constraint()
             g = ca.vertcat(g, gt)
             self.g_lb = ca.vertcat(self.g_lb, g_lb)
             self.g_ub = ca.vertcat(self.g_ub, g_ub)
 
-        if self._collision_flag:
-            self.param_ca_list.append(self.param_obst_ca)
-
 
-        self.param_optim_ca = ca.vertcat(self.param_ca_list[0])
-        for i in range(1, len(self.param_ca_list)):
-            self.param_optim_ca = ca.vertcat(self.param_optim_ca, self.param_ca_list[i])
+        # Read Symbolic Paramaters
+        for i, param in enumerate(self.param_ca_dict):
+            if i == 0:
+                self._param_ca = self.param_ca_dict[param]["sym_param"]
+            else:
+                self._param_ca = ca.vertcat(self._param_ca, self.param_ca_dict[param]["sym_param"].reshape((-1,1)))
 
+        # Solver settings
         options = {}
         options["ipopt.acceptable_tol"] = 1e-3
         if not verbose:
             options["ipopt.print_level"] = 0
             options["print_time"] = 0
 
-        self.solver = ca.nlpsol('solver', 'ipopt', {'x': self.x, 'f': objective, 'g': g, 'p': self.param_optim_ca}, options)
+        # Define solver
+        self.solver = ca.nlpsol('solver', 'ipopt', {'x': self.x, 'f': self.objective.eval_cost(self.x), 'g': g, 'p': self._param_ca}, options)
     
 
         
     def solve(self):
+        # Read Symbolic Paramaters
+        for i, param in enumerate(self.param_ca_dict):
+            if i == 0:
+                self._param_num = self.param_ca_dict[param]["num_param"]
+            else:
+                self._param_num = ca.vertcat(self._param_num, self.param_ca_dict[param]["num_param"].reshape((-1,1), order='F'))
+
         result = self.solver(x0=self.x_init,
                              lbg=self.g_lb,
                              ubg=self.g_ub,
                              lbx=self.l_joint_limits.reshape((-1,1), order='F'),
                              ubx=self.u_joint_limits.reshape((-1,1), order='F'),
-                             p=self.params_optim_num)
+                             p=self._param_num)
 
         success_flag = self.solver.stats()["success"]
         success_msg = self.solver.stats()["return_status"]
         return  result['x'], success_flag
+    
 
+    def add_objective_function(self):
+        # Define parameter sym variable
+        name = "objective_param"
+        self.param_ca_dict[name] =  {
+            "sym_param" : ca.SX.sym(name, self.x_dim, 1),
+            "num_param" : np.zeros((self.x_dim, 1))
+            }
+        # Create objective function
+        self.objective = DistToHome(q_home=self.param_ca_dict[name]["sym_param"] ,
+                                    n_dofs=self.x_dim)
+      
     def add_position_constraint(self, tolerance=0.0):
+        # Define parameter sym variable
+        name = "position_g_param"
+        self.param_ca_dict[name] =  {
+            "sym_param" : ca.SX.sym(name, 4, 4),
+            "num_param" : np.eye(4)
+            }
+        # Create constraint
         self.g_list.append(PositionConstraint(robot=self._robot_model,
                                               q_ca=self.x,
-                                              paramca_T_W_Ref=self.param_T_W_Ref,
+                                              paramca_T_W_Ref=self.param_ca_dict[name]["sym_param"],
                                               tolerance=tolerance))
 
+
     def add_orientation_constraint(self, tolerance=0.0):
+        # Define parameter sym variable
+        name = "orientation_g_param"
+        self.param_ca_dict[name] =  {
+            "sym_param" : ca.SX.sym(name, 4, 4),
+            "num_param" : np.eye(4)
+            }
+        # Create constraint
         self.g_list.append(OrientationConstraint(robot=self._robot_model,
                                                  q_ca=self.x,
-                                                 paramca_T_W_Ref=self.param_T_W_Ref,
+                                                 paramca_T_W_Ref=self.param_ca_dict[name]["sym_param"],
                                                  tolerance=tolerance))
 
+
+
     
 
-    def add_collision_constraint(self, child_link, r_link=0.5, r_obst=0.2, tolerance=0.01):
-        self._collision_flag = True
-        self.g_list.append(CollisionConstraint(robot=self._robot_model,
-                                                q_ca=self.x,
-                                                waypoint_ID=0,
-                                                param_obst_ca=self.param_obst_ca,
-                                                link_name=child_link,
-                                                r_link= r_link,
-                                                r_obst= r_obst,
-                                                tolerance=tolerance))
-
-    def update_constraints_params(self, T_W_Ref, T_W_Obst=None):
-        self.T_W_Ref = T_W_Ref
-        if self._collision_flag:
-            self.params_optim_num = ca.vertcat(self.T_W_Ref, T_W_Obst)
-        else:
-            self.params_optim_num = self.T_W_Ref
+    def add_collision_constraint(self, name, link_names, r_link=0.5, r_obst=0.2, tolerance=0.01):
+        # Define parameter sym variable
+        self.param_ca_dict[name] =  {
+            "sym_param" : ca.SX.sym(name, 4, 4),
+            "num_param" : np.eye(4)
+            }
+        # Create constraint
+        for link in link_names:
+            self.g_list.append(CollisionConstraint(robot=self._robot_model,
+                                                    q_ca=self.x,
+                                                    waypoint_ID=0,
+                                                    param_obst_ca=self.param_ca_dict[name]["sym_param"],
+                                                    link_name=link,
+                                                    r_link= r_link,
+                                                    r_obst= r_obst,
+                                                    tolerance=tolerance))
```

### Comparing `grasp_planning-0.5.7.1/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.7.2/grasp_planning/solver/robot_model.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.1/pyproject.toml` & `grasp_planning-0.5.7.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grasp_planning"
-version = "0.5.7.1"
+version = "0.5.7.2"
 description = "\"Grasp and Motion Planning Python Package.\""
 authors = ["Tomas Merva <tmerva7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TomasMerva/gomp.git"
 repository = "https://github.com/TomasMerva/gomp.git"
```

### Comparing `grasp_planning-0.5.7.1/PKG-INFO` & `grasp_planning-0.5.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grasp_planning
-Version: 0.5.7.1
+Version: 0.5.7.2
 Summary: "Grasp and Motion Planning Python Package."
 Home-page: https://github.com/TomasMerva/gomp.git
 License: MIT
 Author: Tomas Merva
 Author-email: tmerva7@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
```


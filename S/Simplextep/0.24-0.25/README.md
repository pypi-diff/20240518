# Comparing `tmp/Simplextep-0.24-py3-none-any.whl.zip` & `tmp/Simplextep-0.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10060 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    40450 b- defN 24-May-16 08:42 Simplextep/Simplextep.py
+Zip file size: 10063 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    40450 b- defN 24-May-18 04:46 Simplextep/Simplextep.py
 -rw-rw-rw-  2.0 fat     1924 b- defN 24-May-16 08:43 Simplextep/__init__.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:43 Simplextep-0.24.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      316 b- defN 24-May-16 08:43 Simplextep-0.24.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:43 Simplextep-0.24.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-16 08:43 Simplextep-0.24.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      556 b- defN 24-May-16 08:43 Simplextep-0.24.dist-info/RECORD
-7 files, 44439 bytes uncompressed, 9076 bytes compressed:  79.6%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-18 04:48 Simplextep-0.25.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      316 b- defN 24-May-18 04:48 Simplextep-0.25.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 04:48 Simplextep-0.25.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-18 04:48 Simplextep-0.25.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      556 b- defN 24-May-18 04:48 Simplextep-0.25.dist-info/RECORD
+7 files, 44439 bytes uncompressed, 9079 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Simplextep/Simplextep.py
 Comment: 
 
 Filename: Simplextep/__init__.py
 Comment: 
 
-Filename: Simplextep-0.24.dist-info/LICENSE
+Filename: Simplextep-0.25.dist-info/LICENSE
 Comment: 
 
-Filename: Simplextep-0.24.dist-info/METADATA
+Filename: Simplextep-0.25.dist-info/METADATA
 Comment: 
 
-Filename: Simplextep-0.24.dist-info/WHEEL
+Filename: Simplextep-0.25.dist-info/WHEEL
 Comment: 
 
-Filename: Simplextep-0.24.dist-info/top_level.txt
+Filename: Simplextep-0.25.dist-info/top_level.txt
 Comment: 
 
-Filename: Simplextep-0.24.dist-info/RECORD
+Filename: Simplextep-0.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Simplextep/Simplextep.py

```diff
@@ -253,34 +253,34 @@
     def __str__(self, format_:str = "github"):
         columns =  ["Current Values"] + self.parameters
         data = pd.DataFrame(self.constraints, columns=columns)
         data["Basic Variables"] = self.label
         data_z = pd.DataFrame([self.objective_function], columns=columns)
         data_z["Basic Variables"] = f"-z"
 
-        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * "-"}" for _ in range(len(columns))])],
+        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * '-'}" for _ in range(len(columns))])],
                                 columns=columns)
-        data_empty["Basic Variables"] = f"{self.number_of_dash * "-"}"
+        data_empty["Basic Variables"] = f"{self.number_of_dash * '-'}"
 
         data = pd.concat((data, data_z, data_empty), ignore_index=True)
         self.data = data
 
         self.data.set_index("Basic Variables", inplace=True)
         return tabulate(self.data, headers="keys", tablefmt=format_, numalign="right", floatfmt=f".{self.decimal}f")
     
     def __repr__(self, format_:str = "github"):
         columns =  ["Current Values"] + self.parameters
         data = pd.DataFrame(self.constraints, columns=columns)
         data["Basic Variables"] = self.label
         data_z = pd.DataFrame([self.objective_function], columns=columns)
         data_z["Basic Variables"] = f"-z"
 
-        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * "-"}" for _ in range(len(columns))])],
+        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * '-'}" for _ in range(len(columns))])],
                                 columns=columns)
-        data_empty["Basic Variables"] = f"{self.number_of_dash * "-"}"
+        data_empty["Basic Variables"] = f"{self.number_of_dash * '-'}"
 
         data = pd.concat((data, data_z, data_empty), ignore_index=True)
         self.data = data
 
         self.data.set_index("Basic Variables", inplace=True)
         return tabulate(self.data, headers="keys", tablefmt=format_, numalign="right", floatfmt=f".{self.decimal}f")
 
@@ -542,17 +542,17 @@
         data["Basic Variables"] = labels
         data_z = pd.DataFrame([self.objective_function], columns=self.columns)
         data_z["Basic Variables"] = f"-z{self.iteration}"
         if self.two_phase and not self.two_phase_done:
             data_w = pd.DataFrame([self.minus_w], columns=self.columns)
             data_w["Basic Variables"] = f"-w{self.iteration}"
 
-        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * "-"}" for _ in range(len(self.columns))])],
+        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * '-'}" for _ in range(len(self.columns))])],
                                   columns=self.columns)
-        data_empty["Basic Variables"] = f"{self.number_of_dash * "-"}"
+        data_empty["Basic Variables"] = f"{self.number_of_dash * '-'}"
 
         self.iteration += 1
 
         if self.two_phase and not self.two_phase_done:
             data = pd.concat((data, data_z, data_w, data_empty), ignore_index=True)
         else:
             data = pd.concat((data, data_z, data_empty), ignore_index=True)
@@ -911,33 +911,33 @@
     def __str__(self, format_:str = "github"):
         columns =  ["Current Values"] + self.new_parameters
         data = pd.DataFrame(self.new_constraints, columns=columns)
         data["Basic Variables"] = ["s" for _ in range(len(self.new_equality))]
         data_z = pd.DataFrame([self.new_objective_function], columns=columns)
         data_z["Basic Variables"] = f"-z"
 
-        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * "-"}" for _ in range(len(columns))])],
+        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * '-'}" for _ in range(len(columns))])],
                                 columns=columns)
-        data_empty["Basic Variables"] = f"{self.number_of_dash * "-"}"
+        data_empty["Basic Variables"] = f"{self.number_of_dash * '-'}"
 
         data = pd.concat((data, data_z, data_empty), ignore_index=True)
         self.data = data
 
         self.data.set_index("Basic Variables", inplace=True)
         return tabulate(self.data, headers="keys", tablefmt=format_, numalign="right", floatfmt=f".{self.decimal}f")
     
     def __repr__(self, format_:str = "github"):
         columns =  ["Current Values"] + self.new_parameters
         data = pd.DataFrame(self.new_constraints, columns=columns)
         data["Basic Variables"] = ["s" for _ in range(len(self.new_equality))]
         data_z = pd.DataFrame([self.new_objective_function], columns=columns)
         data_z["Basic Variables"] = f"-z"
 
-        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * "-"}" for _ in range(len(columns))])],
+        data_empty = pd.DataFrame([np.array([f"{self.number_of_dash * '-'}" for _ in range(len(columns))])],
                                 columns=columns)
-        data_empty["Basic Variables"] = f"{self.number_of_dash * "-"}"
+        data_empty["Basic Variables"] = f"{self.number_of_dash * '-'}"
 
         data = pd.concat((data, data_z, data_empty), ignore_index=True)
         self.data = data
 
         self.data.set_index("Basic Variables", inplace=True)
         return tabulate(self.data, headers="keys", tablefmt=format_, numalign="right", floatfmt=f".{self.decimal}f")
```

## Comparing `Simplextep-0.24.dist-info/LICENSE` & `Simplextep-0.25.dist-info/LICENSE`

 * *Files identical despite different names*


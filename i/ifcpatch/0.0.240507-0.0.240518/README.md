# Comparing `tmp/ifcpatch-0.0.240507.tar.gz` & `tmp/ifcpatch-0.0.240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifcpatch-0.0.240507.tar", last modified: Tue May  7 13:37:59 2024, max compression
+gzip compressed data, was "ifcpatch-0.0.240518.tar", last modified: Sat May 18 00:59:30 2024, max compression
```

## Comparing `ifcpatch-0.0.240507.tar` & `ifcpatch-0.0.240518.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.213688 ifcpatch-0.0.240507/ifcpatch/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.217688 ifcpatch-0.0.240507/ifcpatch/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ConvertLengthUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ConvertNestToAggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ConvertPropertiesToQuantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/DowngradeIndexedPolyCurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ExtractElements.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ExtractPropertiesToSQLite.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixArchiCADToRevitDoorSwings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixArchiCADToRevitSpaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixRevitClassificationCodeTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixRevitTINs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/Ifc2Sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/MergeDuplicateTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/MergeProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/Migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/OffsetObjectPlacements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/OffsetStoreyElevations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/Optimise.py
--rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/PurgeData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RecycleNonRootedElements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RegenerateGlobalIds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RemoveRevitUniformatClassification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RemoveSiteRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ResetAbsoluteCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ResetSpatialElementLocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/SetRefElevation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/SetWorldCoordinateSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/SplitByBuildingStorey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/TessellateElements.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/ifcpatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 13:37:57.000000 ifcpatch-0.0.240507/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_ConvertLengthUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_ExtractElements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_MergeDuplicateTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_MergeProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_RegenerateGlobalIds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:59:30.254747 ifcpatch-0.0.240518/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-18 00:59:30.254747 ifcpatch-0.0.240518/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:59:30.246748 ifcpatch-0.0.240518/ifcpatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:59:30.254747 ifcpatch-0.0.240518/ifcpatch/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/ConvertLengthUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/ConvertNestToAggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/ConvertPropertiesToQuantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/DowngradeIndexedPolyCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/ExtractElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/ExtractPropertiesToSQLite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/FixArchiCADToRevitDoorSwings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/FixArchiCADToRevitSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/FixRevitClassificationCodeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/FixRevitTINs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/Ifc2Sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/MergeDuplicateTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/MergeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/Migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/OffsetObjectPlacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/OffsetStoreyElevations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/Optimise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/PurgeData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/RecycleNonRootedElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/RegenerateGlobalIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/RemoveRevitUniformatClassification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/RemoveSiteRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/ResetAbsoluteCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/ResetSpatialElementLocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/SetRefElevation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/SetWorldCoordinateSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/SplitByBuildingStorey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/TessellateElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/ifcpatch/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:59:30.254747 ifcpatch-0.0.240518/ifcpatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-18 00:59:30.000000 ifcpatch-0.0.240518/ifcpatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-18 00:59:30.000000 ifcpatch-0.0.240518/ifcpatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:59:30.000000 ifcpatch-0.0.240518/ifcpatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-18 00:59:30.000000 ifcpatch-0.0.240518/ifcpatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 00:59:30.000000 ifcpatch-0.0.240518/ifcpatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-18 00:59:28.000000 ifcpatch-0.0.240518/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:59:30.254747 ifcpatch-0.0.240518/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:59:30.254747 ifcpatch-0.0.240518/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/test/test_ConvertLengthUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/test/test_ExtractElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/test/test_MergeDuplicateTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/test/test_MergeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-18 00:59:24.000000 ifcpatch-0.0.240518/test/test_RegenerateGlobalIds.py
```

### Comparing `ifcpatch-0.0.240507/COPYING` & `ifcpatch-0.0.240518/COPYING`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/COPYING.LESSER` & `ifcpatch-0.0.240518/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/PKG-INFO` & `ifcpatch-0.0.240518/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifcpatch
-Version: 0.0.240507
+Version: 0.0.240518
 Summary: IFC patching utility
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifcpatch-0.0.240507/ifcpatch/__init__.py` & `ifcpatch-0.0.240518/ifcpatch/__init__.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/__main__.py` & `ifcpatch-0.0.240518/ifcpatch/__main__.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/ConvertLengthUnit.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/ConvertLengthUnit.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/ConvertNestToAggregate.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/ConvertNestToAggregate.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcPatch.  If not, see <http://www.gnu.org/licenses/>.
 
 import ifcopenshell
+import ifcopenshell.guid
 
 
 class Patcher:
     def __init__(self, src, file, logger):
         """Convert nesting relationships to aggregate relationships
 
         Some software like Revit won't load nested children elements because
```

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/ConvertPropertiesToQuantities.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/ConvertPropertiesToQuantities.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/DowngradeIndexedPolyCurve.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/DowngradeIndexedPolyCurve.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/ExtractElements.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/ExtractElements.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcPatch.  If not, see <http://www.gnu.org/licenses/>.
 
 import ifcopenshell
 import ifcopenshell.api
+import ifcopenshell.guid
 import ifcopenshell.util.selector
 from typing import Union
 from logging import Logger
 
 
 class Patcher:
     def __init__(self, src: str, file: ifcopenshell.file, logger: Logger, query: str = "IfcWall"):
```

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/ExtractPropertiesToSQLite.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/ExtractPropertiesToSQLite.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/FixArchiCADToRevitDoorSwings.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/FixArchiCADToRevitDoorSwings.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/FixArchiCADToRevitSpaces.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/FixArchiCADToRevitSpaces.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/FixRevitClassificationCodeTypes.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/FixRevitClassificationCodeTypes.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/FixRevitTINs.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/FixRevitTINs.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/Ifc2Sql.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/Ifc2Sql.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/MergeDuplicateTypes.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/MergeDuplicateTypes.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/MergeProject.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/MergeProject.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/Migrate.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/Migrate.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/OffsetObjectPlacements.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/OffsetObjectPlacements.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/OffsetStoreyElevations.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/OffsetStoreyElevations.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/Optimise.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/Optimise.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/PurgeData.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/PurgeData.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/RecycleNonRootedElements.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/RecycleNonRootedElements.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/RegenerateGlobalIds.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/RegenerateGlobalIds.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcPatch.  If not, see <http://www.gnu.org/licenses/>.
 
 import ifcopenshell
+import ifcopenshell.guid
 from logging import Logger
 
 
 class Patcher:
     def __init__(self, src: str, file: ifcopenshell.file, logger: Logger, only_duplicates=False):
         """Regenerate GlobalIds in an IFC model
```

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/RemoveRevitUniformatClassification.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/RemoveRevitUniformatClassification.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/RemoveSiteRepresentation.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/RemoveSiteRepresentation.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/ResetAbsoluteCoordinates.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/ResetAbsoluteCoordinates.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,37 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcPatch.  If not, see <http://www.gnu.org/licenses/>.
 
+import logging
+import numpy as np
+import numpy.typing as npt
+import ifcopenshell
+from typing import Literal, Optional, Union
+
 
 class Patcher:
-    def __init__(self, src, file, logger, mode="geometry", a=None, b=None, c=None, d=None):
+    def __init__(
+        self,
+        src: str,
+        file: ifcopenshell.file,
+        logger: logging.Logger,
+        mode: Literal[
+            "geometry",
+            "placement",
+            "both",
+        ] = "geometry",
+        a: Optional[float] = None,
+        b: Optional[float] = None,
+        c: Optional[float] = None,
+        d: Optional[float] = None,
+    ):
         """Reset any large coordinates to smaller coordinates based on a threshold
 
         If you find large coordinates in your model, the large coordinates may
         either by due to large coordinates in the object placement matrix of
         each object, or large coordinates in the geometry of each object.
 
         If it is the former (preferred), consult the OffsetObjectPlacements
@@ -147,15 +167,15 @@
                 self.logger.info(f"Resetting absolute coordinates by {point}")
             point.Coordinates = (
                 point.Coordinates[0] + offset_point[0],
                 point.Coordinates[1] + offset_point[1],
                 point.Coordinates[2] + offset_point[2],
             )
 
-    def is_point_far_away(self, point):
+    def is_point_far_away(self, point: Union[ifcopenshell.entity_instance, npt.NDArray[np.float64]]) -> bool:
         if hasattr(point, "Coordinates"):
             return (
                 abs(point.Coordinates[0]) > self.threshold
                 or abs(point.Coordinates[1]) > self.threshold
                 or abs(point.Coordinates[2]) > self.threshold
             )
         return abs(point[0]) > self.threshold or abs(point[1]) > self.threshold or abs(point[2]) > self.threshold
```

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/ResetSpatialElementLocations.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/ResetSpatialElementLocations.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/SetRefElevation.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/SetRefElevation.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/SetWorldCoordinateSystem.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/SetWorldCoordinateSystem.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/SplitByBuildingStorey.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/SplitByBuildingStorey.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/TessellateElements.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/TessellateElements.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch/recipes/__init__.py` & `ifcpatch-0.0.240518/ifcpatch/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/ifcpatch.egg-info/PKG-INFO` & `ifcpatch-0.0.240518/ifcpatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifcpatch
-Version: 0.0.240507
+Version: 0.0.240518
 Summary: IFC patching utility
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifcpatch-0.0.240507/ifcpatch.egg-info/SOURCES.txt` & `ifcpatch-0.0.240518/ifcpatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/pyproject.toml` & `ifcpatch-0.0.240518/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifcpatch"
-version = "0.0.240507"
+version = "0.0.240518"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC patching utility"
 readme = "README.md"
 keywords = ["IFC", "BIM"]
 classifiers = [
```

### Comparing `ifcpatch-0.0.240507/test/test_ConvertLengthUnit.py` & `ifcpatch-0.0.240518/test/test_ConvertLengthUnit.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/test/test_ExtractElements.py` & `ifcpatch-0.0.240518/test/test_ExtractElements.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/test/test_MergeDuplicateTypes.py` & `ifcpatch-0.0.240518/test/test_MergeDuplicateTypes.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/test/test_MergeProject.py` & `ifcpatch-0.0.240518/test/test_MergeProject.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240507/test/test_RegenerateGlobalIds.py` & `ifcpatch-0.0.240518/test/test_RegenerateGlobalIds.py`

 * *Files identical despite different names*


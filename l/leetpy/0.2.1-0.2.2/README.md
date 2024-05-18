# Comparing `tmp/leetpy-0.2.1.tar.gz` & `tmp/leetpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetpy-0.2.1.tar", last modified: Mon Apr  1 18:40:51 2024, max compression
+gzip compressed data, was "leetpy-0.2.2.tar", last modified: Sat May 18 16:15:04 2024, max compression
```

## Comparing `leetpy-0.2.1.tar` & `leetpy-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 18:40:51.854921 leetpy-0.2.1/
--rw-rw-rw-   0        0        0     1088 2024-02-27 09:00:16.000000 leetpy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4082 2024-04-01 18:40:51.853920 leetpy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2024-04-01 18:38:04.000000 leetpy-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 18:40:51.846920 leetpy-0.2.1/leetpy/
--rw-rw-rw-   0        0        0      374 2024-03-29 20:08:51.000000 leetpy-0.2.1/leetpy/__init__.py
--rw-rw-rw-   0        0        0     6820 2024-03-29 14:14:55.000000 leetpy-0.2.1/leetpy/_reingold_tilford_algorithm.py
--rw-rw-rw-   0        0        0     2672 2024-03-29 14:57:57.000000 leetpy-0.2.1/leetpy/array_1d.py
--rw-rw-rw-   0        0        0     4993 2024-03-30 08:21:13.000000 leetpy-0.2.1/leetpy/array_2d.py
--rw-rw-rw-   0        0        0    26791 2024-03-31 13:14:22.000000 leetpy-0.2.1/leetpy/binary_tree.py
--rw-rw-rw-   0        0        0     8553 2024-03-29 14:47:45.000000 leetpy-0.2.1/leetpy/linked_list.py
-drwxrwxrwx   0        0        0        0 2024-04-01 18:40:51.852920 leetpy-0.2.1/leetpy.egg-info/
--rw-rw-rw-   0        0        0     4082 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 18:40:51.854921 leetpy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1654 2024-04-01 18:39:32.000000 leetpy-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:15:04.427935 leetpy-0.2.2/
+-rw-rw-rw-   0        0        0     1088 2024-02-27 09:00:16.000000 leetpy-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4119 2024-05-18 16:15:04.427935 leetpy-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3419 2024-04-20 05:23:26.000000 leetpy-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:15:04.420936 leetpy-0.2.2/leetpy/
+-rw-rw-rw-   0        0        0      421 2024-04-16 20:00:25.000000 leetpy-0.2.2/leetpy/__init__.py
+-rw-rw-rw-   0        0        0     2627 2024-05-18 16:04:12.000000 leetpy-0.2.2/leetpy/_force_layout.py
+-rw-rw-rw-   0        0        0     6825 2024-04-02 06:05:58.000000 leetpy-0.2.2/leetpy/_reingold_tilford_algorithm.py
+-rw-rw-rw-   0        0        0     2672 2024-03-29 14:57:57.000000 leetpy-0.2.2/leetpy/array_1d.py
+-rw-rw-rw-   0        0        0     4993 2024-03-30 08:21:13.000000 leetpy-0.2.2/leetpy/array_2d.py
+-rw-rw-rw-   0        0        0    35263 2024-04-07 16:41:18.000000 leetpy-0.2.2/leetpy/binary_tree.py
+-rw-rw-rw-   0        0        0     9060 2024-04-02 14:13:37.000000 leetpy-0.2.2/leetpy/linked_list.py
+-rw-rw-rw-   0        0        0     6318 2024-05-18 16:07:41.000000 leetpy-0.2.2/leetpy/undirected_graph.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:15:04.426937 leetpy-0.2.2/leetpy.egg-info/
+-rw-rw-rw-   0        0        0     4119 2024-05-18 16:15:03.000000 leetpy-0.2.2/leetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-05-18 16:15:04.000000 leetpy-0.2.2/leetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:15:03.000000 leetpy-0.2.2/leetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-18 16:15:04.000000 leetpy-0.2.2/leetpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 16:15:04.000000 leetpy-0.2.2/leetpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 16:15:04.428934 leetpy-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2024-05-18 16:11:35.000000 leetpy-0.2.2/setup.py
```

### Comparing `leetpy-0.2.1/LICENSE` & `leetpy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.1/PKG-INFO` & `leetpy-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: You should solve DSA problems efficiently.
 Author: Aryan Pingle
 Author-email: realaryanpingle@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/aryanpingle/LeetPy
 Project-URL: Source, https://github.com/aryanpingle/LeetPy
 Project-URL: Download, https://pypi.org/project/leetpy/#files
@@ -75,18 +75,29 @@
     # Oh, and keep indentation to 2 spaces
     code += "\n" + BinaryTree.export_as_code(root, node_alias="CustomNode", indent=2)
 
 with open("testing.py", "w") as f:
     f.write(code)
 ```
 
-**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures. Here's a comprehensive list of examples:
+**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures. For a comprehensive list of usage examples, check out [/examples/README.md](./examples/README.md).
 
-|Example|Description|
-|---|---|
-|[Binary Tree Example 1](./examples/binary_tree/example_1.py)|Create a randomized binary tree with 20 nodes and visualize it.|
-|[Binary Tree Example 2](./examples/binary_tree/example_2.py)|Generate a file which contains code for creating randomized binary trees with some constraints (without dependending on the leetpy package).|
-|[Binary Tree Example 3](./examples/binary_tree/example_3.py)|Same as example 2, but with inlined generated code (reducing the number of generated lines).|
-|[Linked List Example 1](./examples/linked_list/example_1.py)|Create a randomized singly linked list with 20 nodes and visualize it.|
-|[Linked List Example 2](./examples/linked_list/example_2.py)|Create a randomized AND CYCLIC singly linked list with 20 UNIQUE nodes and visualize it.|
+## Development
+
+**`LeetPy`** has plans to support the following data structures:
+
+- [X] 1-D Arrays
+- [X] 2-D Arrays
+- [X] Binary Trees
+- [X] Singly Linked Lists
+- [ ] Doubly Linked Lists
+- [ ] Undirected Graphs (Weighted + Unweighted)
+- [ ] Directed Graphs (Weighted + Unweighted)
+
+All data structures have some common API's:
+
+- `create() -> structure` - To create the structure with random data and properties based on certain parameters
+- `export_as_code(structure) -> str` - To get an independent Python3 function that when called, returns the given data structure
+- `export_as_svg(structure) -> None` - To create an SVG file with a visualization of the given data structure
+- `print(structure) -> None` - To print a representation of the data structure to the terminal
```

### Comparing `leetpy-0.2.1/README.md` & `leetpy-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -56,16 +56,27 @@
     # Oh, and keep indentation to 2 spaces
     code += "\n" + BinaryTree.export_as_code(root, node_alias="CustomNode", indent=2)
 
 with open("testing.py", "w") as f:
     f.write(code)
 ```
 
-**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures. Here's a comprehensive list of examples:
+**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures. For a comprehensive list of usage examples, check out [/examples/README.md](./examples/README.md).
 
-|Example|Description|
-|---|---|
-|[Binary Tree Example 1](./examples/binary_tree/example_1.py)|Create a randomized binary tree with 20 nodes and visualize it.|
-|[Binary Tree Example 2](./examples/binary_tree/example_2.py)|Generate a file which contains code for creating randomized binary trees with some constraints (without dependending on the leetpy package).|
-|[Binary Tree Example 3](./examples/binary_tree/example_3.py)|Same as example 2, but with inlined generated code (reducing the number of generated lines).|
-|[Linked List Example 1](./examples/linked_list/example_1.py)|Create a randomized singly linked list with 20 nodes and visualize it.|
-|[Linked List Example 2](./examples/linked_list/example_2.py)|Create a randomized AND CYCLIC singly linked list with 20 UNIQUE nodes and visualize it.|
+## Development
+
+**`LeetPy`** has plans to support the following data structures:
+
+- [X] 1-D Arrays
+- [X] 2-D Arrays
+- [X] Binary Trees
+- [X] Singly Linked Lists
+- [ ] Doubly Linked Lists
+- [ ] Undirected Graphs (Weighted + Unweighted)
+- [ ] Directed Graphs (Weighted + Unweighted)
+
+All data structures have some common API's:
+
+- `create() -> structure` - To create the structure with random data and properties based on certain parameters
+- `export_as_code(structure) -> str` - To get an independent Python3 function that when called, returns the given data structure
+- `export_as_svg(structure) -> None` - To create an SVG file with a visualization of the given data structure
+- `print(structure) -> None` - To print a representation of the data structure to the terminal
```

### Comparing `leetpy-0.2.1/leetpy/_reingold_tilford_algorithm.py` & `leetpy-0.2.2/leetpy/_reingold_tilford_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,15 @@
     root: Optional[object],
     data_attr: str,
     left_attr: str,
     right_attr: str,
     minimum_separation: int = 3,
 ) -> Optional[TR_Node]:
     """
-    Create a deep copy of the given tree root with coordinates for each node on a 2-D plane.
+    Create a deep copy of the given tree root with coordinates for each node on a 2-D
+    plane.
     """
 
     TR_root = _TR_create_tree_copy(root, data_attr, left_attr, right_attr)
     TR_setup(TR_root, 0, TR_Extreme(), TR_Extreme(), minimum_separation)
     TR_petrify(TR_root, 0)
     return TR_root
```

### Comparing `leetpy-0.2.1/leetpy/array_1d.py` & `leetpy-0.2.2/leetpy/array_1d.py`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.1/leetpy/array_2d.py` & `leetpy-0.2.2/leetpy/array_2d.py`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.1/leetpy/binary_tree.py` & `leetpy-0.2.2/leetpy/binary_tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import deque
 import json
 import random
-from typing import Deque, Iterator, List, Optional, Set, TypedDict, TypeVar, Type
+import re as regex
 from rich import print as rich_print
+from typing import Deque, Iterator, List, Optional, Set, TypedDict, TypeVar, Type
 
 from ._reingold_tilford_algorithm import TR_create_drawing, TR_Node
 
 
 INT_MIN = -2147483648
 INT_MAX = 2147483647
 
@@ -14,14 +15,18 @@
 # Generic type for any object that represents a node in a binary tree
 NodeLike = TypeVar("NodeLike")
 """
 A generic type for any object that represents a node in a binary tree. It will have three
 unique attributes: for its data, for its left child and for its right child.
 """
 
+SupportsWrite = TypeVar("SupportsWrite")
+"""
+A generic type for any `.write()`-supporting file-like object."""
+
 
 class NodeConfig(TypedDict):
     """
     A 1:1 mapping of the three attributes of a binary tree node to the corresponding
     attribute names in a custom node object.
     """
 
@@ -183,15 +188,15 @@
             # Add the newly created node to the queue
             q.append(new_node)
             created_count += 1
 
             # If the parent isn't fully filled, add it to the queue
             if (
                 getattr(curr, config["left_attr"]) is None
-                or getattr(curr, config["left_attr"]) is None
+                or getattr(curr, config["right_attr"]) is None
             ):
                 # appendleft only matters when 'make_complete' is enabled
                 q.appendleft(curr)
 
         if make_bst:
             arr = [
                 getattr(node, config["data_attr"])
@@ -247,14 +252,59 @@
                 q.popleft()
 
             is_left = not is_left
 
         return root
 
     @staticmethod
+    def equals(
+        root1: Optional[NodeLike],
+        root2: Optional[NodeLike],
+        config1: NodeConfig = TreeNodeConfig,
+        config2: NodeConfig = TreeNodeConfig,
+    ) -> bool:
+        """
+        Check if the binary trees formed by two root nodes are equal in structure and
+        data.
+
+        Args:
+            root1: The root node of the first binary tree.
+            root2: The root node of the second binary tree.
+            config1: A dictionary that maps the three attributes of `TreeNode` to the
+                corresponding attribute names in `root1`. This is only needed if `root1`
+                is not an instance of `TreeNode`.
+            config2: A dictionary that maps the three attributes of `TreeNode` to the
+                corresponding attribute names in `root2`. This is only needed if `root2`
+                is not an instance of `TreeNode`.
+        """
+
+        if root1 is None and root2 is None:
+            return True
+
+        data1 = getattr(root1, config1["data_attr"])
+        data2 = getattr(root2, config2["data_attr"])
+        if data1 != data2:
+            return False
+
+        is_left_equal = BinaryTree.equals(
+            getattr(root1, config1["left_attr"]),
+            getattr(root2, config2["left_attr"]),
+            config1,
+            config2,
+        )
+        is_right_equal = BinaryTree.equals(
+            getattr(root1, config1["right_attr"]),
+            getattr(root2, config2["right_attr"]),
+            config1,
+            config2,
+        )
+
+        return is_left_equal and is_right_equal
+
+    @staticmethod
     def export_as_leetcode_array(
         root: Optional[NodeLike], config: NodeConfig = TreeNodeConfig
     ) -> str:
         """
         Generate a representation of the given rooted binary tree in Leetcode's testcase
         format.
 
@@ -378,17 +428,15 @@
                             f"{node_var}.{target_config['right_attr']} = {right_var}",
                             indent,
                         )
                     )
             else:
                 # Define this node
                 node_repr = get_node_repr(node, left_var, right_var)
-                code_lines.append(
-                    _indented(f"{node_var} = {node_repr}", indent)
-                )
+                code_lines.append(_indented(f"{node_var} = {node_repr}", indent))
 
             return node_var
 
         code_lines = []
         root_var = travel(root, code_lines)
         # Add a comment containing the array representation (for convenience)
         array_repr = BinaryTree.export_as_leetcode_array(root, source_config)
@@ -397,14 +445,163 @@
         code += "\n" + "\n".join(code_lines)
         # Return the root node
         code += "\n" + _indented(f"return {root_var}", indent)
 
         return code
 
     @staticmethod
+    def save_as_svg(
+        root: Optional[TreeNode],
+        fp: SupportsWrite,
+        node_color: str = "transparent",
+        stroke_color: str = "black",
+    ):
+        """
+        Save a visualization of the given binary tree as an SVG illustration.
+
+        Args:
+            fp: A file pointer (or any `.write()`-implementing object).
+            node_color: The background color of a node as a CSS-string.
+            stroke_color: The color of edges and node outlines as a CSS-string.
+        """
+        TR_root = TR_create_drawing(root, "val", "left", "right", minimum_separation=1)
+
+        # Find the minimum and maximum x and y coordinates (grid bounds)
+        x_bounds = [0, 0]
+        y_bounds = [0, 0]
+
+        def calculate_bounds(root: TR_Node):
+            if root is None:
+                return
+            x_bounds[0] = min(x_bounds[0], root.x_coord)
+            x_bounds[1] = max(x_bounds[1], root.x_coord)
+            y_bounds[0] = min(y_bounds[0], root.y_coord)
+            y_bounds[1] = max(y_bounds[1], root.y_coord)
+
+            calculate_bounds(root.left)
+            calculate_bounds(root.right)
+
+        calculate_bounds(TR_root)
+
+        ###################################
+        #         SVG Calculations        #
+        ###################################
+
+        # TODO: Create a utility module for SVG stuff
+
+        CELL_WIDTH = 100
+        CELL_HEIGHT = 2 * CELL_WIDTH  # Terminal char height = 2*width
+
+        SVG_VIEWBOX_LEFT = CELL_WIDTH * x_bounds[0]
+        SVG_VIEWBOX_RIGHT = CELL_WIDTH * (x_bounds[1] + 1)
+        SVG_VIEWBOX_UP = 0
+        SVG_VIEWBOX_DOWN = CELL_HEIGHT * (y_bounds[1] + 1)
+
+        SVG_WIDTH = SVG_VIEWBOX_RIGHT - SVG_VIEWBOX_LEFT
+        SVG_HEIGHT = SVG_VIEWBOX_DOWN - SVG_VIEWBOX_UP
+
+        NODE_RADIUS = min(CELL_WIDTH, CELL_HEIGHT) // 3
+        EDGE_STROKE_WIDTH = (2 * NODE_RADIUS) * 0.05
+        FONT_HEIGHT = NODE_RADIUS
+        CHAR_WIDTH = FONT_HEIGHT / 2
+
+        node_g = []  # A list of all SVGs that represent a node
+        node_mask_g = []  # Copies of node_g used for masking
+        text_g = []  # A list of all SVGs that represent a node's data
+        edge_g = []  # A list of all SVGs that represent an edge
+
+        def get_centered_text_svg(text: str, cx: int, cy: int) -> str:
+            baseline_x = cx - (CHAR_WIDTH) * (len(text) / 2)
+            baseline_y = cy + (FONT_HEIGHT / 2) * 0.8
+            return f"""
+            <text x="{baseline_x}" y="{baseline_y}" style="font-family: monospace;"
+            font-size="{FONT_HEIGHT}">{text}</text>
+            """
+
+        def add_node_svg(data: any, x_coord: int, y_coord: int):
+            cx = (x_coord * CELL_WIDTH) + (CELL_WIDTH / 2)
+            cy = (y_coord * CELL_HEIGHT) + (CELL_HEIGHT / 2)
+            node_g.append(
+                f"""
+                <ellipse cx="{cx}" cy="{cy}" rx="{NODE_RADIUS}" ry="{NODE_RADIUS}"
+                fill="{node_color}" stroke="{stroke_color}"
+                stroke-width="{EDGE_STROKE_WIDTH}">
+                </ellipse>
+                """
+            )
+            node_mask_g.append(
+                f"""
+                <ellipse cx="{cx}" cy="{cy}" rx="{NODE_RADIUS}" ry="{NODE_RADIUS}"
+                fill="black" stroke="black" stroke-width="{EDGE_STROKE_WIDTH}">
+                </ellipse>
+                """
+            )
+            text_g.append(get_centered_text_svg(str(data), cx, cy))
+
+        def add_edge_svg(x1: int, y1: int, x2: int, y2: int):
+            x1 = (x1 * CELL_WIDTH) + (CELL_WIDTH / 2)
+            x2 = (x2 * CELL_WIDTH) + (CELL_WIDTH / 2)
+            y1 = (y1 * CELL_HEIGHT) + (CELL_HEIGHT / 2)
+            y2 = (y2 * CELL_HEIGHT) + (CELL_HEIGHT / 2)
+            edge_g.append(
+                f"""
+                <line x1="{x1}" y1="{y1}" x2="{x2}" y2="{y2}" stroke="{stroke_color}"
+                stroke-width="{EDGE_STROKE_WIDTH}"></line>
+                """
+            )
+
+        def build_svg(node: TR_Node):
+            if node is None:
+                return
+
+            # Build edge svg's
+            if node.left is not None:
+                add_edge_svg(
+                    node.x_coord, node.y_coord, node.left.x_coord, node.left.y_coord
+                )
+            if node.right is not None:
+                add_edge_svg(
+                    node.x_coord, node.y_coord, node.right.x_coord, node.right.y_coord
+                )
+
+            # Build node svg
+            add_node_svg(node.val, node.x_coord, node.y_coord)
+
+            build_svg(node.left)
+            build_svg(node.right)
+
+        build_svg(TR_root)
+
+        # This is used for the node mask
+        background_rect_white = f"""
+        <rect x="{SVG_VIEWBOX_LEFT}" y="{SVG_VIEWBOX_UP}" width="{SVG_WIDTH}"
+        height="{SVG_HEIGHT}" fill="white"></rect>
+        """
+
+        code = f"""
+        <svg
+        version="1.1"
+        viewBox="{SVG_VIEWBOX_LEFT} {SVG_VIEWBOX_UP} {SVG_WIDTH} {SVG_HEIGHT}"
+        xmlns="http://www.w3.org/2000/svg">
+          <mask id="node-mask-group">
+            {background_rect_white}
+            {''.join(node_mask_g)}
+          </mask>
+          <g id="leetpy-bt-edges" mask="url(#node-mask-group)">{''.join(edge_g)}</g>
+          <g id="leetpy-bt-nodes">{''.join(node_g)}</g>
+          <g id="leetpy-bt-node-texts">{''.join(text_g)}</g>
+        </svg>
+        """
+
+        # Remove newlines and leading spaces in lines (for compression)
+        code = regex.sub(r"\s*(\n\s*)+", " ", code)
+
+        fp.write(code)
+
+    @staticmethod
     def get_depth(root: Optional[NodeLike], config: NodeConfig = TreeNodeConfig) -> int:
         """
         Returns the maximum depth/height of the given binary tree. For a single root node,
         the depth is 1.
 
         Args:
             config: A dictionary that maps the three attributes of `TreeNode` to the
@@ -420,14 +617,51 @@
             return 0
         return 1 + max(
             BinaryTree.get_depth(getattr(root, config["left_attr"]), config),
             BinaryTree.get_depth(getattr(root, config["right_attr"]), config),
         )
 
     @staticmethod
+    def get_max_width(
+        root: Optional[NodeLike], config: NodeConfig = TreeNodeConfig
+    ) -> int:
+        """
+        The maximum number of nodes at any level of the given binary tree.
+
+        Args:
+            config: A dictionary that maps the three attributes of `TreeNode` to the
+                corresponding attribute names in `root`. This is only needed if `root` is
+                not an instance of `TreeNode`.
+        """
+
+        assert not BinaryTree.is_cyclic(
+            root, config
+        ), "Cycle detected while traveling from the root"
+
+        if root is None:
+            return 0
+
+        widths = {}
+
+        def dfs(root: Optional[NodeLike], depth: int) -> None:
+            if root is None:
+                return
+
+            if not depth in widths:
+                widths[depth] = 0
+            widths[depth] += 1
+
+            dfs(getattr(root, config["left_attr"]), depth + 1)
+            dfs(getattr(root, config["right_attr"]), depth + 1)
+
+        dfs(root, 0)
+
+        return max(widths.values())
+
+    @staticmethod
     def is_binary_search_tree(
         root: Optional[NodeLike], config: NodeConfig = TreeNodeConfig
     ) -> bool:
         """
         Check if the given Binary Tree satisfies the properties of the Binary Search Tree
         data structure.
```

### Comparing `leetpy-0.2.1/leetpy/linked_list.py` & `leetpy-0.2.2/leetpy/linked_list.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     """A basic definition of a singly linked list's node."""
 
     def __init__(self, val: any = 0, next: Optional["ListNode"] = None):
         self.val = val
         self.next = next
 
 
+def _indented(s: str, spaces: int):
+    return " " * spaces + s
+
+
 class LinkedList:
     """
     Algorithms and utility functions related to the Singly Linked List data structure. All
     functions are static and stateless.
     """
 
     @staticmethod
@@ -87,15 +91,15 @@
         for value in array:
             head.next = ListNode(value)
             head = head.next
 
         return sentinel.next
 
     @staticmethod
-    def export_as_function(
+    def export_as_code(
         head: Optional[ListNode],
         indent: int = 4,
         function_name: str = "get_head",
         node_alias: str = "ListNode",
         type_hints: bool = True,
     ) -> str:
         """
@@ -109,56 +113,55 @@
                 "get_head")
             node_alias: The name of the class used to create a node for the linked list.
                 (default = "ListNode")
             type_hints: When enabled, the function code will have a Python3 return type
                 declaration for the given node_alias. (example: `-> Optional[ListNode]`)
         """
 
-        code__return_type = f" -> Optional[{node_alias}]" if type_hints else ""
-        code__func_signature = f"def {function_name}(){code__return_type}:"
+        code__return_type = ""
+        if type_hints:
+            code__return_type = " -> " + ("None" if head is None else node_alias)
+        code = f"def {function_name}(){code__return_type}:"
 
         if head is None:
-            return "\n".join([code__func_signature, " " * indent + "return None"])
+            # (in code) return None
+            code += "\n" + _indented("return None", indent)
+            return code
 
         def get_node_repr(node: Optional[ListNode]) -> str:
             if node is None:
                 return "None"
             return f"{node_alias}({node.val})"
 
         N = LinkedList.count_nodes(head)
 
-        code__func_body = []
-
         # Create the first node (index 0)
-        code__func_body.append(f"node_0 = {get_node_repr(head)}")
+        code += "\n" + _indented(f"node_0 = {get_node_repr(head)}", indent)
 
         node_to_index = {head: 0}
         for i in range(1, N):
             head = head.next
             # Create the new node
-            code__func_body.append(f"node_{i} = {get_node_repr(head)}")
+            code += "\n" + _indented(f"node_{i} = {get_node_repr(head)}", indent)
             node_to_index[head] = i
             # Justify its existence
-            code__func_body.append(f"node_{i-1}.next = node_{i}")
+            code += "\n" + _indented(f"node_{i-1}.next = node_{i}", indent)
 
         # head is now the last node
 
         # Create the cyclic reference, if any
         if LinkedList.is_cyclic(head):
-            code__func_body.append(f"# cyclic dependency")
-            code__func_body.append(f"node_{N-1}.next = node_{node_to_index[head.next]}")
+            code += "\n" + _indented(f"# cyclic dependency", indent)
+            code += "\n" + _indented(
+                f"node_{N-1}.next = node_{node_to_index[head.next]}", indent
+            )
 
-        code__func_body.append("return node_0")  # Return statement
+        code += "\n" + _indented("return node_0", indent)  # Return statement
 
-        return "\n".join(
-            [
-                code__func_signature,
-                *[" " * indent + line for line in code__func_body],
-            ]
-        )
+        return code
 
     @staticmethod
     def get(head: Optional[ListNode], n: int) -> Optional[ListNode]:
         """
         Get the n'th node in the given linked list (0-based indexing). Negative indices
         will return nodes from the end of the linked list.
 
@@ -220,14 +223,31 @@
                 rich_print("[cyan]↺ →[/]", end=" ")
             print(node.val, end=" ")
             if node.next is not None:
                 rich_print("[cyan]→[/]", end=" ")
         print()
 
     @staticmethod
+    def reverse(head: Optional[ListNode]) -> Optional[ListNode]:
+        """Reverse the given linked list and return the new head."""
+
+        assert not LinkedList.is_cyclic(head)
+
+        prev = None
+        current = head
+        while current is not None:
+            next = current.next
+            current.next = prev
+            prev = current
+            current = next
+        head = prev
+
+        return head
+
+    @staticmethod
     def search(head: Optional[ListNode], value: any) -> Optional[ListNode]:
         """
         Search for a node that contains the given value, and return the first match if
         any.
 
         NOTE: Cyclic references do not cause a problem.
         """
```

### Comparing `leetpy-0.2.1/leetpy.egg-info/PKG-INFO` & `leetpy-0.2.2/leetpy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: You should solve DSA problems efficiently.
 Author: Aryan Pingle
 Author-email: realaryanpingle@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/aryanpingle/LeetPy
 Project-URL: Source, https://github.com/aryanpingle/LeetPy
 Project-URL: Download, https://pypi.org/project/leetpy/#files
@@ -75,18 +75,29 @@
     # Oh, and keep indentation to 2 spaces
     code += "\n" + BinaryTree.export_as_code(root, node_alias="CustomNode", indent=2)
 
 with open("testing.py", "w") as f:
     f.write(code)
 ```
 
-**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures. Here's a comprehensive list of examples:
+**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures. For a comprehensive list of usage examples, check out [/examples/README.md](./examples/README.md).
 
-|Example|Description|
-|---|---|
-|[Binary Tree Example 1](./examples/binary_tree/example_1.py)|Create a randomized binary tree with 20 nodes and visualize it.|
-|[Binary Tree Example 2](./examples/binary_tree/example_2.py)|Generate a file which contains code for creating randomized binary trees with some constraints (without dependending on the leetpy package).|
-|[Binary Tree Example 3](./examples/binary_tree/example_3.py)|Same as example 2, but with inlined generated code (reducing the number of generated lines).|
-|[Linked List Example 1](./examples/linked_list/example_1.py)|Create a randomized singly linked list with 20 nodes and visualize it.|
-|[Linked List Example 2](./examples/linked_list/example_2.py)|Create a randomized AND CYCLIC singly linked list with 20 UNIQUE nodes and visualize it.|
+## Development
+
+**`LeetPy`** has plans to support the following data structures:
+
+- [X] 1-D Arrays
+- [X] 2-D Arrays
+- [X] Binary Trees
+- [X] Singly Linked Lists
+- [ ] Doubly Linked Lists
+- [ ] Undirected Graphs (Weighted + Unweighted)
+- [ ] Directed Graphs (Weighted + Unweighted)
+
+All data structures have some common API's:
+
+- `create() -> structure` - To create the structure with random data and properties based on certain parameters
+- `export_as_code(structure) -> str` - To get an independent Python3 function that when called, returns the given data structure
+- `export_as_svg(structure) -> None` - To create an SVG file with a visualization of the given data structure
+- `print(structure) -> None` - To print a representation of the data structure to the terminal
```

### Comparing `leetpy-0.2.1/setup.py` & `leetpy-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("version.txt", "r") as f:
     version = f.read()
 
-version = "0.2.1"
-
 # Validate the version name
 try:
     v = Version(version)
     rich_print(f"[bold cyan]{version}[/] [bold green]is a valid version name[/]")
 except:
     rich_print(f"[bold cyan]{version}[/] [bold red]is not a valid version name[/]")
     exit(1)
```


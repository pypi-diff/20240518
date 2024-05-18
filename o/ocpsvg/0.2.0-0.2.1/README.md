# Comparing `tmp/ocpsvg-0.2.0.tar.gz` & `tmp/ocpsvg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocpsvg-0.2.0.tar", last modified: Mon Dec  4 17:05:29 2023, max compression
+gzip compressed data, was "ocpsvg-0.2.1.tar", last modified: Sat May 18 12:44:07 2024, max compression
```

## Comparing `ocpsvg-0.2.0.tar` & `ocpsvg-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:29.785776 ocpsvg-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:29.777777 ocpsvg-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:29.781777 ocpsvg-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/.github/workflows/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-12-04 17:05:29.785776 ocpsvg-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:29.781777 ocpsvg-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/examples/svg-logo-hlr1.svg
--rw-r--r--   0 runner    (1001) docker     (127)    58091 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/examples/svg-logo-hlr2.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/examples/svg_tiger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:29.781777 ocpsvg-0.2.0/ocpsvg/
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/ocpsvg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/ocpsvg/hlr.py
--rw-r--r--   0 runner    (1001) docker     (127)    13896 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/ocpsvg/ocp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23878 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/ocpsvg/svg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:29.781777 ocpsvg-0.2.0/ocpsvg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-12-04 17:05:29.000000 ocpsvg-0.2.0/ocpsvg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-12-04 17:05:29.000000 ocpsvg-0.2.0/ocpsvg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 17:05:29.000000 ocpsvg-0.2.0/ocpsvg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-04 17:05:29.000000 ocpsvg-0.2.0/ocpsvg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-04 17:05:29.000000 ocpsvg-0.2.0/ocpsvg.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      511 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/readme-pypi.md
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 17:05:29.785776 ocpsvg-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:29.781777 ocpsvg-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/tests/ocp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/tests/test_hlr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/tests/test_ocp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23768 2023-12-04 17:05:19.000000 ocpsvg-0.2.0/tests/test_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:44:07.113419 ocpsvg-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:44:07.105419 ocpsvg-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:44:07.109419 ocpsvg-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/.github/workflows/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-18 12:44:07.113419 ocpsvg-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:44:07.109419 ocpsvg-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/examples/svg-logo-hlr1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    58091 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/examples/svg-logo-hlr2.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/examples/svg_tiger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:44:07.109419 ocpsvg-0.2.1/ocpsvg/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/ocpsvg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/ocpsvg/hlr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13896 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/ocpsvg/ocp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25438 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/ocpsvg/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:44:07.113419 ocpsvg-0.2.1/ocpsvg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-18 12:44:07.000000 ocpsvg-0.2.1/ocpsvg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-18 12:44:07.000000 ocpsvg-0.2.1/ocpsvg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:44:07.000000 ocpsvg-0.2.1/ocpsvg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 12:44:07.000000 ocpsvg-0.2.1/ocpsvg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 12:44:07.000000 ocpsvg-0.2.1/ocpsvg.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      511 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/readme-pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:44:07.113419 ocpsvg-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:44:07.113419 ocpsvg-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/tests/ocp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/tests/test_hlr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/tests/test_ocp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25256 2024-05-18 12:43:59.000000 ocpsvg-0.2.1/tests/test_svg.py
```

### Comparing `ocpsvg-0.2.0/.github/workflows/codecov.yaml` & `ocpsvg-0.2.1/.github/workflows/codecov.yaml`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/.github/workflows/publish.yaml` & `ocpsvg-0.2.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/.github/workflows/tests.yaml` & `ocpsvg-0.2.1/.github/workflows/tests.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: 
           - "3.9"
           - "3.10"
         os: 
-          - macos-latest
+          - macos-13
           - ubuntu-latest
           - windows-latest
 
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
```

### Comparing `ocpsvg-0.2.0/PKG-INFO` & `ocpsvg-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: ocpsvg
-Version: 0.2.0
+Version: 0.2.1
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: cadquery-ocp>=7.7.0
 Requires-Dist: svgpathtools<2,>=1.5.1
 Requires-Dist: svgelements<2,>=1.9.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # OCPSVG
```

### Comparing `ocpsvg-0.2.0/examples/svg-logo-hlr1.svg` & `ocpsvg-0.2.1/examples/svg-logo-hlr1.svg`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/examples/svg-logo-hlr2.svg` & `ocpsvg-0.2.1/examples/svg-logo-hlr2.svg`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/examples/svg_tiger.py` & `ocpsvg-0.2.1/examples/svg_tiger.py`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/ocpsvg/hlr.py` & `ocpsvg-0.2.1/ocpsvg/hlr.py`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/ocpsvg/ocp.py` & `ocpsvg-0.2.1/ocpsvg/ocp.py`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/ocpsvg/svg.py` & `ocpsvg-0.2.1/ocpsvg/svg.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from OCP.StdFail import StdFail_NotDone
 from OCP.TopoDS import TopoDS, TopoDS_Edge, TopoDS_Face, TopoDS_Shape, TopoDS_Wire
 
 from .ocp import (
     CurveOrAdaptor,
     InvalidWiresForFace,
     bezier_curve,
+    circle_curve,
     curve_and_adaptor,
     curve_to_beziers,
     curve_to_polyline,
     edge_from_curve,
     edge_to_curve,
     ellipse_curve,
     faces_from_wire_soup,
@@ -114,26 +115,24 @@
 @overload
 def import_svg_document(
     svg_file: Union[str, pathlib.Path, TextIO],
     *,
     flip_y: bool = True,
     ignore_visibility: bool = False,
     metadata: Optional[Callable[[ShapeElement, Sequence[ParentElement]], M]],
-) -> ItemsFromDocument[tuple[FaceOrWire, M]]:
-    ...
+) -> ItemsFromDocument[tuple[FaceOrWire, M]]: ...
 
 
 @overload
 def import_svg_document(
     svg_file: Union[str, pathlib.Path, TextIO],
     *,
     flip_y: bool = True,
     ignore_visibility: bool = False,
-) -> ItemsFromDocument[FaceOrWire]:
-    ...
+) -> ItemsFromDocument[FaceOrWire]: ...
 
 
 def import_svg_document(
     svg_file: Union[str, pathlib.Path, TextIO],
     *,
     flip_y: bool = True,
     ignore_visibility: bool = False,
@@ -277,14 +276,52 @@
     :yield: faces
     :raises SyntaxError:
     :raises ValueError:
     """
     return faces_from_wire_soup(wires_from_svg_path(path))
 
 
+def wires_from_svg_element(element: ShapeElement) -> Iterable[TopoDS_Wire]:
+    def check_unskewed_transform() -> Union[tuple[float, float, float], None]:
+        o = svgelements.Point(0, 0) * element.transform
+        x = svgelements.Point(1, 0) * element.transform
+        y = svgelements.Point(0, 1) * element.transform
+        is_skewed = abs(o.angle_to(y) - o.angle_to(x)) != pi / 2  # type: ignore
+        if not is_skewed:
+            return o.distance_to(x), o.distance_to(y), o.angle_to(x)  # type: ignore
+
+    element.reify()
+
+    if isinstance(element, (svgelements.Circle, svgelements.Ellipse)) and (
+        scale_and_angle := check_unskewed_transform()
+    ):
+        cx = float(element.cx)  # type: ignore
+        cy = float(element.cy)  # type: ignore
+        origin = svgelements.Point(cx, cy) * element.transform
+        center = gp_Pnt(origin.real, origin.imag, 0)  # type: ignore
+        scale_x, scale_y, angle = scale_and_angle
+        r1 = float(element.rx) * scale_x  # type: ignore
+        r2 = float(element.ry) * scale_y  # type: ignore
+        if r1 == r2:
+            curve = circle_curve(r1, center=center)
+        else:
+            curve = ellipse_curve(r1, r2, center=center, rotation=degrees(angle))
+        yield wire_from_continuous_edges((edge_from_curve(curve),))
+
+    elif path := svg_element_to_path(element):
+        yield from wires_from_svg_path(path)
+
+
+def svg_element_to_path(element: ShapeElement):
+    path = svgelements.Path(element)
+    if len(path):
+        path.reify()
+        return _svgelements_to_svgpathtools(path)
+
+
 def wires_from_svg_path(path: SvgPathLike) -> Iterable[TopoDS_Wire]:
     """Create wires from an SVG path.
 
     :param SvgPathLike path: input SVG path
     :yield: wires
     :raises SyntaxError:
     :raises ValueError:
@@ -619,26 +656,24 @@
 
 @overload
 def wires_from_svg_document(
     svg_file: Union[str, pathlib.Path, TextIO],
     metadata_factory: Callable[[ShapeElement, Sequence[ParentElement]], M],
     *,
     ignore_visibility: bool = False,
-) -> ItemsFromDocument[tuple[list[TopoDS_Wire], bool, M]]:
-    ...
+) -> ItemsFromDocument[tuple[list[TopoDS_Wire], bool, M]]: ...
 
 
 @overload
 def wires_from_svg_document(
     svg_file: Union[str, pathlib.Path, TextIO],
     metadata_factory: None,
     *,
     ignore_visibility: bool = False,
-) -> ItemsFromDocument[tuple[list[TopoDS_Wire], bool, None]]:
-    ...
+) -> ItemsFromDocument[tuple[list[TopoDS_Wire], bool, None]]: ...
 
 
 def wires_from_svg_document(
     svg_file: Union[str, pathlib.Path, TextIO],
     metadata_factory: Optional[Callable[[ShapeElement, Sequence[ParentElement]], M]],
     *,
     ignore_visibility: bool = False,
@@ -653,58 +688,54 @@
     def is_filled(element: ShapeElement):
         fill = element.fill
         return fill.value is not None  # type: ignore
 
     if callable(metadata_factory):
         wires = (
             (
-                list(wires_from_svg_path(path)),
+                list(wires_from_svg_element(source_element)),
                 is_filled(source_element),
                 metadata_factory(source_element, source_parents),
             )
-            for path, source_element, source_parents in elements
+            for source_element, source_parents in elements
         )
         return ItemsFromDocument(wires, elements.doc_info)
     else:
         wires = (
-            (list(wires_from_svg_path(path)), is_filled(source_element), None)
-            for path, source_element, _source_parents in elements
+            (
+                list(wires_from_svg_element(source_element)),
+                is_filled(source_element),
+                None,
+            )
+            for source_element, _source_parents in elements
         )
         return ItemsFromDocument(wires, elements.doc_info)
 
 
 def find_shapes_svg_in_document(
     svg_file: Union[str, pathlib.Path, TextIO],
     *,
     ignore_visibility: bool = False,
-) -> ItemsFromDocument[
-    tuple[svgpathtools.Path, ShapeElement, tuple[ParentElement, ...]]
-]:
-    def _svgelements_to_svgpathtools(svgelements_path: svgelements.Path):
-        """converting segments might be faster than re-parsing maybe?
-        but the representations are different (segments vs commands)
-        so exchanging via path spec is probably the safest bet."""
-
-        d_string = svgelements_path.d(relative=False)  # type: ignore
-        return svgpathtools.Path(d_string)
-
+) -> ItemsFromDocument[tuple[ShapeElement, tuple[ParentElement, ...]]]:
     def walk_svg_element(
         element: svgelements.SVGElement, parents: tuple[ParentElement, ...] = ()
     ) -> Iterator[tuple[ShapeElement, tuple[ParentElement, ...]]]:
         if isinstance(element, ShapeElement):
             yield element, parents
         elif isinstance(element, (svgelements.Group, svgelements.Use)):
             new_parents = *parents, element
             for child in element:  # type: ignore
                 yield from walk_svg_element(child, new_parents)  # type: ignore
 
     parsed_svg = svgelements.SVG.parse(  # type: ignore
-        resolve_path(svg_file)
-        if isinstance(svg_file, (str, pathlib.Path))
-        else svg_file,
+        (
+            resolve_path(svg_file)
+            if isinstance(svg_file, (str, pathlib.Path))
+            else svg_file
+        ),
         parse_display_none=ignore_visibility,
         ppi=25.4,  # inches to millimiters
     )
 
     def elements():
         for element, parents in walk_svg_element(parsed_svg):  # type: ignore
             if not ignore_visibility:
@@ -713,26 +744,35 @@
                     if visibility in ("hidden", "collapse"):  # type: ignore
                         continue
                 except (KeyError, AttributeError):
                     pass
 
             if isinstance(element, svgelements.Path):
                 if len(element):
-                    yield _svgelements_to_svgpathtools(element), element, parents
+                    yield element, parents
 
             elif isinstance(element, svgelements.Shape):
                 path = svgelements.Path(element)
                 if len(path):
                     path.reify()
-                    yield _svgelements_to_svgpathtools(path), element, parents
+                    yield element, parents
 
     doc_info = DocumentInfo(parsed_svg.width, parsed_svg.height)  # type: ignore
     return ItemsFromDocument(elements(), doc_info)
 
 
+def _svgelements_to_svgpathtools(svgelements_path: svgelements.Path):
+    """converting segments might be faster than re-parsing maybe?
+    but the representations are different (segments vs commands)
+    so exchanging via path spec is probably the safest bet."""
+
+    d_string = svgelements_path.d(relative=False)  # type: ignore
+    return svgpathtools.Path(d_string)
+
+
 def resolve_path(path: Union[pathlib.Path, str]) -> str:
     if not isinstance(path, pathlib.Path):
         path = pathlib.Path(path)
     return str(path.expanduser().resolve())
 
 
 def _path_from_SvgPathLike(path: SvgPathLike) -> svgpathtools.Path:
```

### Comparing `ocpsvg-0.2.0/ocpsvg.egg-info/PKG-INFO` & `ocpsvg-0.2.1/ocpsvg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: ocpsvg
-Version: 0.2.0
+Version: 0.2.1
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: cadquery-ocp>=7.7.0
 Requires-Dist: svgpathtools<2,>=1.5.1
 Requires-Dist: svgelements<2,>=1.9.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # OCPSVG
```

### Comparing `ocpsvg-0.2.0/ocpsvg.egg-info/SOURCES.txt` & `ocpsvg-0.2.1/ocpsvg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+LICENSE
 pyproject.toml
 readme-pypi.md
 readme.md
 .github/workflows/codecov.yaml
 .github/workflows/publish.yaml
 .github/workflows/tests.yaml
 examples/svg-logo-hlr1.svg
```

### Comparing `ocpsvg-0.2.0/readme.md` & `ocpsvg-0.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/tests/ocp.py` & `ocpsvg-0.2.1/tests/ocp.py`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/tests/test_hlr.py` & `ocpsvg-0.2.1/tests/test_hlr.py`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/tests/test_ocp.py` & `ocpsvg-0.2.1/tests/test_ocp.py`

 * *Files identical despite different names*

### Comparing `ocpsvg-0.2.0/tests/test_svg.py` & `ocpsvg-0.2.1/tests/test_svg.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from io import StringIO
 from math import pi
 from tempfile import NamedTemporaryFile
 from typing import Any, Sequence, Union
 
 import pytest
 import svgpathtools
-from OCP.Geom import Geom_Curve
+from OCP.Geom import Geom_Circle, Geom_Curve, Geom_Ellipse
 from OCP.GeomAbs import GeomAbs_CurveType
 from OCP.gp import gp_Vec
 from OCP.TopoDS import TopoDS, TopoDS_Face, TopoDS_Shape, TopoDS_Wire
 from pytest import approx, raises
 
 from ocpsvg.ocp import (
     bezier_curve,
@@ -33,14 +33,15 @@
     edge_to_svg_path,
     edges_from_svg_path,
     faces_from_svg_path,
     find_shapes_svg_in_document,
     format_svg,
     import_svg_document,
     polyline_to_svg_path,
+    svg_element_to_path,
     wire_to_svg_path,
     wires_from_svg_path,
 )
 
 from .ocp import face_area, face_normal
 from .test_ocp import XY, Pnt, as_Pnt, as_Pnts, as_tuple
 
@@ -638,15 +639,17 @@
     0.00794,-0.042334 0.023813,-0.05715 0.015875,-0.01587467 0.034925,-0.023812
     0.05715,-0.023812 0.022225,0 0.041275,0.00793733 0.05715,0.023812
     0.015875,0.01481667 0.023813,0.03386667 0.023813,0.05715 0,0.02328333
     -0.00794,0.04286267 -0.023813,0.058738 -0.015875,0.0158753
     -0.034925,0.0238127 -0.05715,0.023812 z"/>
     </svg>
     """
-    for path, _, _ in find_shapes_svg_in_document(StringIO(svg_src)):
+    for e, _ in find_shapes_svg_in_document(StringIO(svg_src)):
+        path = svg_element_to_path(e)
+        assert path
         for segment in path:
             assert not isinstance(segment, svgpathtools.Line)
 
 
 def test_fix_svgpathtools_closing_lines_str():
     """`svgpathtools` adds an extremenly short closing line segment to this path.
     We want it ignored when converting to edges."""
@@ -667,14 +670,66 @@
     )
     for wire in wires_from_svg_path(d):
         for edge in topoDS_iterator(wire):
             curve = edge_to_curve(TopoDS.Edge_s(edge))
             assert curve.GetType() != GeomAbs_CurveType.GeomAbs_Line
 
 
+@pytest.mark.parametrize(
+    "element, curve_type, center",
+    [
+        (
+            'circle r="40" cx="10" cy="5" transform="translate(10 0)"',
+            Geom_Circle,
+            (20, 5),
+        ),
+        (
+            'circle r="40" transform="translate(10 0) scale(2 1)"',
+            Geom_Ellipse,
+            (10, 0),
+        ),
+        (
+            'ellipse rx="40" ry="80" transform="scale(1 .5)"',
+            Geom_Circle,
+            (0, 0),
+        ),
+        (
+            'circle r="40" transform="rotate(90) translate(10 0)"',
+            Geom_Circle,
+            (0, 10),
+        ),
+    ],
+)
+def test_circles_and_ellipses(
+    element: str,
+    curve_type: Union[Geom_Circle, Geom_Ellipse],
+    center: tuple[float, float],
+):
+    svg_src = f"""
+    <svg xmlns="http://www.w3.org/2000/svg">
+        <{element} stroke="red" fill="none"/>
+    </svg>
+    """
+    buf = StringIO(svg_src)
+    imported = list(import_svg_document(buf))
+    assert len(imported) == 1
+    assert isinstance(imported[0], TopoDS_Wire)
+
+    curves = [
+        edge_to_curve(TopoDS.Edge_s(e)).Curve().Curve()
+        for e in topoDS_iterator(imported[0])
+    ]
+    assert len(curves) == 1
+    curve = curves[0]
+    assert type(curve) == curve_type
+    assert isinstance(curve, (Geom_Circle, Geom_Ellipse))
+    loc = curve.Axis().Location()
+    assert (loc.X(), loc.Y()) == approx(center)
+
+
 def nested_squares_path(count: int, x: float = 0, y: float = 0):
     def parts():
         for s in range(1, count + 1):
             yield f"M{x-s},{y-s} H{x+s} V{y+s} H{x-s} Z"
 
     return " ".join(parts())
```


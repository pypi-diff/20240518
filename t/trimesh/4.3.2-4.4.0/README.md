# Comparing `tmp/trimesh-4.3.2.tar.gz` & `tmp/trimesh-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimesh-4.3.2.tar", last modified: Mon Apr 29 23:29:15 2024, max compression
+gzip compressed data, was "trimesh-4.4.0.tar", last modified: Sat May 18 04:25:02 2024, max compression
```

## Comparing `trimesh-4.3.2.tar` & `trimesh-4.4.0.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.165613 trimesh-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-29 23:29:05.000000 trimesh-4.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-29 23:29:15.165613 trimesh-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-29 23:29:05.000000 trimesh-4.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-29 23:29:05.000000 trimesh-4.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:29:15.165613 trimesh-4.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.133612 trimesh-4.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_3dxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_3mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_adjacency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_convex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_crash.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_dae.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_except.py
--rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    41146 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_inertia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_integralmeancurvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_loaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_medial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_minimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_mutate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_normals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_path_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_path_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_scenegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_splines.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_texture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_unwrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_vertices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.145613 trimesh-4.3.2/trimesh/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   102599 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/convex.py
--rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.149613 trimesh-4.3.2/trimesh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17597 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/dae.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    68424 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/off.py
--rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/stl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/threedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/threemf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/xaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    30523 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.149613 trimesh-4.3.2/trimesh/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/path/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/path/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23095 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/svg_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)    26100 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    31112 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/ray/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/ray_pyembree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/ray_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/ray_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40277 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/creation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/resources/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/gltf2.schema.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.157612 trimesh-4.3.2/trimesh/resources/schema/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/box.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/capsule.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/cylinder.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/extrusion.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/primitive.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/scenegraph.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/sphere.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/transform.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/trimesh.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/wkt.polygon.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/urdf.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.157612 trimesh-4.3.2/trimesh/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/base.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/blender_boolean.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/blender_unwrap.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/dxf.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/path.svg
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/ply.json
--rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/viewer.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/units_to_inches.json
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.157612 trimesh-4.3.2/trimesh/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    74542 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21705 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    66702 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/windowed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29109 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/gloss.py
--rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh/voxel/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.979406 trimesh-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-18 04:24:54.000000 trimesh-4.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-05-18 04:25:02.979406 trimesh-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-05-18 04:24:54.000000 trimesh-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-18 04:24:54.000000 trimesh-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 04:25:02.979406 trimesh-4.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.951406 trimesh-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_3dxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_3mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41565 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_integralmeancurvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_medial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_normals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19045 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_path_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_path_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11093 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_scenegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18043 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_unwrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-18 04:24:54.000000 trimesh-4.4.0/tests/test_voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.955406 trimesh-4.4.0/trimesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102607 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20121 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45780 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.959406 trimesh-4.4.0/trimesh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17597 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70714 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/off.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/threedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/threemf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/xaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/exchange/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30723 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26160 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.959406 trimesh-4.4.0/trimesh/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/interfaces/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/interfaces/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/interfaces/gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.963406 trimesh-4.4.0/trimesh/path/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.963406 trimesh-4.4.0/trimesh/path/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/exchange/dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23099 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/exchange/svg_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43908 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/path/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19972 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33336 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.963406 trimesh-4.4.0/trimesh/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/ray/ray_pyembree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/ray/ray_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/ray/ray_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40277 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.967406 trimesh-4.4.0/trimesh/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/creation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.967406 trimesh-4.4.0/trimesh/resources/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/gltf2.schema.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.967406 trimesh-4.4.0/trimesh/resources/schema/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/box.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/capsule.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/cylinder.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/extrusion.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/primitive.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/scenegraph.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/sphere.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/transform.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/trimesh.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/primitive/wkt.polygon.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/schema/urdf.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.967406 trimesh-4.4.0/trimesh/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/templates/base.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/templates/blender_boolean.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/templates/blender_unwrap.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/templates/dxf.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/templates/path.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/templates/ply.json
+-rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/templates/viewer.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/resources/units_to_inches.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.971406 trimesh-4.4.0/trimesh/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/scene/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/scene/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/scene/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/scene/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74299 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21683 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66702 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.971406 trimesh-4.4.0/trimesh/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/viewer/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/viewer/trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/viewer/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30977 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/viewer/windowed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.971406 trimesh-4.4.0/trimesh/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/visual/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29111 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/visual/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/visual/gloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/visual/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/visual/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/visual/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.975406 trimesh-4.4.0/trimesh/voxel/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12525 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27695 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11765 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-18 04:24:54.000000 trimesh-4.4.0/trimesh/voxel/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 04:25:02.975406 trimesh-4.4.0/trimesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-05-18 04:25:02.000000 trimesh-4.4.0/trimesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-18 04:25:02.000000 trimesh-4.4.0/trimesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 04:25:02.000000 trimesh-4.4.0/trimesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-18 04:25:02.000000 trimesh-4.4.0/trimesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 04:25:02.000000 trimesh-4.4.0/trimesh.egg-info/top_level.txt
```

### Comparing `trimesh-4.3.2/LICENSE.md` & `trimesh-4.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/PKG-INFO` & `trimesh-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.3.2
+Version: 4.4.0
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,23 +75,23 @@
 Requires-Dist: cascadio; extra == "recommend"
 Requires-Dist: manifold3d>=2.3.0; extra == "recommend"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: pyright; extra == "test"
 Requires-Dist: ezdxf; extra == "test"
-Requires-Dist: gmsh>=4.12.1; extra == "test"
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: pymeshlab; extra == "test"
 Requires-Dist: pyinstrument; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: pytest-beartype; python_version >= "3.10" and extra == "test"
+Provides-Extra: deprecated
+Requires-Dist: gmsh==4.12.2; extra == "deprecated"
 Provides-Extra: all
-Requires-Dist: trimesh[easy,recommend,test]; extra == "all"
+Requires-Dist: trimesh[deprecated,easy,recommend,test]; extra == "all"
 
 [![trimesh](https://trimesh.org/_static/images/logotype-a.svg)](http://trimesh.org)
 
 -----------
 [![Github Actions](https://github.com/mikedh/trimesh/workflows/Release%20Trimesh/badge.svg)](https://github.com/mikedh/trimesh/actions) [![codecov](https://codecov.io/gh/mikedh/trimesh/branch/main/graph/badge.svg?token=4PVRQXyl2h)](https://codecov.io/gh/mikedh/trimesh)  [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/trimesh/trimesh?label=docker&sort=semver)](https://hub.docker.com/r/trimesh/trimesh/tags) [![PyPI version](https://badge.fury.io/py/trimesh.svg)](https://badge.fury.io/py/trimesh)
```

### Comparing `trimesh-4.3.2/README.md` & `trimesh-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/pyproject.toml` & `trimesh-4.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 61.0", "wheel"]
 
 [project]
 name = "trimesh"
 requires-python = ">=3.7"
-version = "4.3.2"
+version = "4.4.0"
 authors = [{name = "Michael Dawson-Haggerty", email = "mikedh@kerfed.com"}]
 license = {file = "LICENSE.md"}
 description = "Import, export, process, analyze and view triangular meshes."
 keywords = ["graphics", "mesh", "geometry", "3D"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -98,26 +98,28 @@
 # this is the list of everything that is ever added anywhere
 # mostly useful for getting our test coverage up
 test = [
     "pytest-cov",
     "coveralls",
     "pyright",
     "ezdxf",
-    "gmsh>=4.12.1",
     "pytest",
-    "pymeshlab",
+    #"pymeshlab",
     "pyinstrument",
     "matplotlib",
     "ruff",
     "pytest-beartype; python_version>='3.10'"
 ]
 
+# interfaces.gmsh will be dropped Jan 2025
+deprecated = ["gmsh==4.12.2"]
+
 # requires pip >= 21.2
 # https://hynek.me/articles/python-recursive-optional-dependencies/
-all = ["trimesh[easy,recommend,test]"]
+all = ["trimesh[easy,recommend,test,deprecated]"]
 
 [tool.ruff]
 target-version = "py37"
 line-length = 90
 
 
 # See https://github.com/charliermarsh/ruff#rules for error code definitions.
```

### Comparing `trimesh-4.3.2/tests/test_3dxml.py` & `trimesh-4.4.0/tests/test_3dxml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_3mf.py` & `trimesh-4.4.0/tests/test_3mf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_adjacency.py` & `trimesh-4.4.0/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_align.py` & `trimesh-4.4.0/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_arc.py` & `trimesh-4.4.0/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_base.py` & `trimesh-4.4.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_binvox.py` & `trimesh-4.4.0/tests/test_binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_boolean.py` & `trimesh-4.4.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_bounds.py` & `trimesh-4.4.0/tests/test_bounds.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,30 +113,30 @@
 
     def test_2D(self):
         for theta in g.np.linspace(0, g.np.pi * 2, 2000):
             # create some random rectangular-ish 2D points
             points = g.random((10, 2)) * [5, 1]
 
             # save the basic AABB of the points before rotation
-            rectangle_pre = points.ptp(axis=0)
+            rectangle_pre = g.np.ptp(points, axis=0)
 
             # rotate them by an increment
             TR = g.trimesh.transformations.planar_matrix(theta=theta)
             points = g.trimesh.transform_points(points, TR)
 
             # find the OBB of the points
             T, rectangle = g.trimesh.bounds.oriented_bounds_2D(points)
 
             # apply the calculated OBB
             oriented = g.trimesh.transform_points(points, T)
 
-            origin = oriented.min(axis=0) + oriented.ptp(axis=0) / 2.0
+            origin = oriented.min(axis=0) + g.np.ptp(oriented, axis=0) / 2.0
 
             # check to make sure the returned rectangle size is right
-            assert g.np.allclose(oriented.ptp(axis=0), rectangle)
+            assert g.np.allclose(g.np.ptp(oriented, axis=0), rectangle)
             # check to make sure the OBB consistently returns the
             # long axis in the same direction
             assert rectangle[0] > rectangle[1]
             # check to make sure result is actually returning an OBB
             assert g.np.allclose(origin, 0.0)
             # make sure OBB has less or same area as naive AABB
             assert g.np.prod(rectangle) <= g.np.prod(rectangle_pre)
@@ -195,15 +195,15 @@
         p = i.permutate.transform()
         assert p.symmetry == "radial"
 
         # find the bounding cylinder with this random transform
         r = p.bounding_cylinder
 
         # transformed height should match source mesh
-        assert g.np.isclose(i.vertices[:, 2].ptp(), r.primitive.height, rtol=1e-6)
+        assert g.np.isclose(g.np.ptp(i.vertices[:, 2]), r.primitive.height, rtol=1e-6)
         # slightly inflated cylinder should contain all
         # vertices of the source mesh
         assert r.buffer(0.01).contains(p.vertices).all()
 
     def test_obb_order(self):
         # make sure our sorting and transform flipping of
         # OBB extents are working by checking against a box
```

### Comparing `trimesh-4.3.2/tests/test_cache.py` & `trimesh-4.4.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_camera.py` & `trimesh-4.4.0/tests/test_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             fov = g.np.array([20, 50])
 
             # offset the points by a random amount
             offset = (g.random(3) - 0.5) * 100
             T = g.trimesh.scene.cameras.look_at(points + offset, fov)
 
             # check using trig
-            check = (points.ptp(axis=0)[:2] / 2.0) / g.np.tan(np.radians(fov / 2))
+            check = (np.ptp(points, axis=0)[:2] / 2.0) / g.np.tan(np.radians(fov / 2))
             check += points[:, 2].mean()
 
             # Z should be the same as maximum trig option
             assert np.linalg.inv(T)[2, 3] >= check.max()
 
         # just run to test other arguments
         # TODO(unknown): find the way to test it correctly
```

### Comparing `trimesh-4.3.2/tests/test_collision.py` & `trimesh-4.4.0/tests/test_collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_color.py` & `trimesh-4.4.0/tests/test_color.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def test_concatenate(self):
         a = g.get_mesh("ballA.off")
         b = g.get_mesh("ballB.off")
 
         a.visual.face_colors = [255, 0, 0]
         r = a + b
-        assert any(r.visual.face_colors.ptp(axis=0) > 1)
+        assert any(g.np.ptp(r.visual.face_colors, axis=0) > 1)
 
     def test_concatenate_empty_mesh(self):
         box = g.get_mesh("box.STL")
 
         mesh_fcolor = box.copy()
         mesh_fcolor.visual.face_colors = [255, 0, 0]
 
@@ -149,31 +149,31 @@
         Make sure cached smooth model is dumped if colors are changed
         """
         m = g.get_mesh("featuretype.STL")
 
         # will put smoothed mesh into visuals cache
         s = m.smooth_shaded
         # every color should be default color
-        assert s.visual.face_colors.ptp(axis=0).max() == 0
+        assert g.np.ptp(s.visual.face_colors, axis=0).max() == 0
 
         # set one face to a different color
         m.visual.face_colors[0] = [255, 0, 0, 255]
 
         # cache should be dumped yo
         s1 = m.smooth_shaded
-        assert s1.visual.face_colors.ptp(axis=0).max() != 0
+        assert g.np.ptp(s1.visual.face_colors, axis=0).max() != 0
 
         # do the same check on vertex color
         m = g.get_mesh("featuretype.STL")
         s = m.smooth_shaded
         # every color should be default color
-        assert s.visual.vertex_colors.ptp(axis=0).max() == 0
+        assert g.np.ptp(s.visual.vertex_colors, axis=0).max() == 0
         m.visual.vertex_colors[g.np.arange(10)] = [255, 0, 0, 255]
         s1 = m.smooth_shaded
-        assert s1.visual.face_colors.ptp(axis=0).max() != 0
+        assert g.np.ptp(s1.visual.face_colors, axis=0).max() != 0
 
     def test_vertex(self):
         m = g.get_mesh("torus.STL")
 
         m.visual.vertex_colors = [100, 100, 100, 255]
 
         assert len(m.visual.vertex_colors) == len(m.vertices)
```

### Comparing `trimesh-4.3.2/tests/test_convex.py` & `trimesh-4.4.0/tests/test_convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_copy.py` & `trimesh-4.4.0/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_crash.py` & `trimesh-4.4.0/tests/test_crash.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_creation.py` & `trimesh-4.4.0/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_curvature.py` & `trimesh-4.4.0/tests/test_curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_dae.py` & `trimesh-4.4.0/tests/test_dae.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         with g.TemporaryDirectory() as root:
             # export using a file path so it can auto-create
             # a FilePathResolver to write the stupid assets
             path = g.os.path.join(root, "duck.obj")
             s.export(path)
             # bring it back from outer space
             rec = g.trimesh.load(path, force="mesh")
-        assert rec.visual.uv.ptp(axis=0).ptp() > 1e-5
+        assert g.np.ptp(g.np.ptp(rec.visual.uv, axis=0)) > 1e-5
         assert s.visual.material.baseColorTexture.size == rec.visual.material.image.size
 
         conv = s.convert_units("inch")
         assert conv.units == "inch"
 
     def test_material_round(self):
         """
```

### Comparing `trimesh-4.3.2/tests/test_decomposition.py` & `trimesh-4.4.0/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_dxf.py` & `trimesh-4.4.0/tests/test_dxf.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
             # make sure all versions have consistent length
             assert g.np.allclose(L, L.mean(), rtol=0.01)
 
             # count the number of entities in the path
             # this should be the same for every version
             E = g.np.array([len(paths[i].entities) for i in group], dtype=g.np.int64)
-            assert E.ptp() == 0
+            assert g.np.ptp(E) == 0
 
     def test_bulge(self):
         """
         Test bulged polylines which are polylines with
         implicit arcs.
         """
         # get a drawing with bulged polylines
```

### Comparing `trimesh-4.3.2/tests/test_edges.py` & `trimesh-4.4.0/tests/test_edges.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_encoding.py` & `trimesh-4.4.0/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_except.py` & `trimesh-4.4.0/tests/test_except.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_export.py` & `trimesh-4.4.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_extrude.py` & `trimesh-4.4.0/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_facets.py` & `trimesh-4.4.0/tests/test_facets.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_fill.py` & `trimesh-4.4.0/tests/test_fill.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_geom.py` & `trimesh-4.4.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_gltf.py` & `trimesh-4.4.0/tests/test_gltf.py`

 * *Files 1% similar despite different names*

```diff
@@ -767,15 +767,15 @@
                 g.trimesh.load(
                     g.trimesh.util.wrap_as_stream(export), file_type="glb"
                 ).geometry.values()
             )
         )
         # original mesh should have vertex colors
         assert m.visual.kind == "face"
-        assert m.visual.vertex_colors.ptp(axis=0).ptp() > 0
+        assert g.np.ptp(g.np.ptp(m.visual.vertex_colors, axis=0)) > 0
         # vertex colors should have survived import-export
         assert g.np.allclose(m.visual.vertex_colors, r.visual.vertex_colors)
 
     def test_vertex_attrib(self):
         # test concatenation with texture
         m = g.get_mesh("fuze.obj")
 
@@ -1054,11 +1054,21 @@
                 ).geometry.values()
             )
         )
 
         # Check that the normals are still null
         assert g.np.allclose(reimported_mesh.vertex_normals[0], [0, 0, 0])
 
+    def test_no_indices(self):
+        # test mesh with no indices (faces should be generated correctly)
+        mesh = g.get_mesh("no_indices_3storybuilding.glb")
+        assert len(mesh.triangles) == 72
+
+        # the mesh is actually mode 5 with 4 vertices
+        # which as triangle strips would be 2 faces
+        mesh = g.get_mesh("Mesh_PrimitiveMode_04.gltf")
+        assert len(mesh.triangles) == 2
+
 
 if __name__ == "__main__":
     g.trimesh.util.attach_to_log()
     g.unittest.main()
```

### Comparing `trimesh-4.3.2/tests/test_gmsh.py` & `trimesh-4.4.0/tests/test_gmsh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_graph.py` & `trimesh-4.4.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_grouping.py` & `trimesh-4.4.0/tests/test_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,29 +211,29 @@
     def test_group_rows(self):
         a = g.np.arange(100) / 2.0
         b = g.np.tile(a, 3).reshape((-1, 3))
         c = g.np.vstack((b, b))
 
         gr = g.trimesh.grouping.group_rows(c)
         assert g.np.shape(gr) == (100, 2)
-        assert g.np.allclose(c[gr].ptp(axis=1), 0.0)
+        assert g.np.allclose(g.np.ptp(c[gr], axis=1), 0.0)
 
         gr = g.trimesh.grouping.group_rows(c, require_count=2)
         assert gr.shape == (100, 2)
-        assert g.np.allclose(c[gr].ptp(axis=1), 0.0)
+        assert g.np.allclose(g.np.ptp(c[gr], axis=1), 0.0)
 
         c = g.np.vstack((c, [1, 2, 3]))
         gr = g.trimesh.grouping.group_rows(c, require_count=2)
         grd = g.trimesh.grouping.group_rows(c)
         # should discard the single element
         assert gr.shape == (100, 2)
         # should get the single element correctly
         assert len(grd) == 101
         assert sum(1 for i in grd if len(i) == 2) == 100
-        assert g.np.allclose(c[gr].ptp(axis=1), 0.0)
+        assert g.np.allclose(g.np.ptp(c[gr], axis=1), 0.0)
 
     def test_group_vector(self):
         x = g.np.linspace(-100, 100, 100)
 
         vec = g.np.column_stack((x, g.np.ones(len(x)), g.np.zeros(len(x))))
         vec = g.trimesh.unitize(vec)
```

### Comparing `trimesh-4.3.2/tests/test_html.py` & `trimesh-4.4.0/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_identifier.py` & `trimesh-4.4.0/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_import.py` & `trimesh-4.4.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_inertia.py` & `trimesh-4.4.0/tests/test_inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_integralmeancurvature.py` & `trimesh-4.4.0/tests/test_integralmeancurvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_interval.py` & `trimesh-4.4.0/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_light.py` & `trimesh-4.4.0/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_loaded.py` & `trimesh-4.4.0/tests/test_loaded.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_medial.py` & `trimesh-4.4.0/tests/test_medial.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,13 +23,13 @@
                 *g.trimesh.path.polygons.medial_axis(poly)
             )
         )
         # should have returned a single tiny line
         # with midpoint at origin
         assert len(med.vertices) == 2
         assert len(med.entities) == 1
-        assert float(med.vertices.mean(axis=0).ptp()) < 1e-8
+        assert float(g.np.ptp(med.vertices.mean(axis=0))) < 1e-8
 
 
 if __name__ == "__main__":
     g.trimesh.util.attach_to_log()
     g.unittest.main()
```

### Comparing `trimesh-4.3.2/tests/test_merge.py` & `trimesh-4.4.0/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_mesh.py` & `trimesh-4.4.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_meta.py` & `trimesh-4.4.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_minimal.py` & `trimesh-4.4.0/tests/test_minimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def test_path_exc(self):
         # this should require *no deps*
         from trimesh.path import packing
 
         bounds, inserted = packing.rectangles_single([[1, 1], [2, 2]], size=[2, 4])
         assert inserted.all()
 
-        extents = bounds.reshape((-1, 2)).ptp(axis=0)
+        extents = np.ptp(bounds.reshape((-1, 2)), axis=0)
         assert np.allclose(extents, [2, 3])
         assert bounds.shape == (2, 2, 2)
         density = 5.0 / np.prod(extents)
         assert density > 0.833
 
     def test_load(self):
         # kinds of files we should be able to
```

### Comparing `trimesh-4.3.2/tests/test_mutate.py` & `trimesh-4.4.0/tests/test_mutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_normals.py` & `trimesh-4.4.0/tests/test_normals.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_nsphere.py` & `trimesh-4.4.0/tests/test_nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_obj.py` & `trimesh-4.4.0/tests/test_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         # if there is no texture image
         m = g.get_mesh("noimg.obj")
         assert m.visual.uv.shape == (len(m.vertices), 2)
         # make sure UV coordinates are in range 0.0 - 1.0
         assert m.visual.uv.max() < (1 + 1e-5)
         assert m.visual.uv.min() > -1e-5
         # check to make sure it's not all zeros
-        assert m.visual.uv.ptp() > 0.5
+        assert g.np.ptp(m.visual.uv) > 0.5
         rec = g.roundtrip(m.export(file_type="obj"), file_type="obj")
         assert g.np.isclose(m.area, rec.area)
 
     def test_trailing(self):
         # test files with texture and trailing slashes
         m = g.get_mesh("jacked.obj")
         assert len(m.visual.uv) == len(m.vertices)
@@ -44,15 +44,15 @@
         assert g.trimesh.util.is_shape(mesh.vertices, (-1, 3))
 
         # make sure groups are the right length
         # TODO: we do not support face groups now
         # assert len(mesh.metadata['face_groups']) == len(mesh.faces)
 
         # check to make sure there is signal not just zeros
-        # assert mesh.metadata['face_groups'].ptp() > 0
+        # assert g.np.ptp(mesh.metadata['face_groups']) > 0
 
     def test_obj_negative_indices(self):
         # a wavefront file with negative indices
         mesh = g.get_mesh("negative_indices.obj")
 
         # make sure some data got loaded
         assert g.trimesh.util.is_shape(mesh.faces, (12, 3))
```

### Comparing `trimesh-4.3.2/tests/test_off.py` & `trimesh-4.4.0/tests/test_off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_operators.py` & `trimesh-4.4.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_packing.py` & `trimesh-4.4.0/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_path_creation.py` & `trimesh-4.4.0/tests/test_path_creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_path_sample.py` & `trimesh-4.4.0/tests/test_path_sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_pathlib.py` & `trimesh-4.4.0/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_paths.py` & `trimesh-4.4.0/tests/test_paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -294,11 +294,31 @@
             assert g.trimesh.path.util.is_ccw(polygon.exterior.coords)
             # the interior should NOT be counterclockwise
             assert not g.trimesh.path.util.is_ccw(polygon.interiors[0].coords)
 
             # should be a valid Path2D
             g.check_path2D(planar)
 
+    def test_multiplane(self):
+        # check to make sure we're applying `tol_path.merge_digits` for line segments
+        vertices = g.np.array(
+            [
+                [19.402250931139097, -14.88787016674277, 64.0],
+                [20.03318396099334, -14.02738654377374, 64.0],
+                [19.402250931139097, -14.88787016674277, 0.0],
+                [20.03318396099334, -14.02738654377374, 0.0],
+                [21, -16.5, 32],
+            ]
+        )
+        faces = g.np.array(
+            [[1, 3, 0], [0, 3, 2], [1, 0, 4], [0, 2, 4], [3, 1, 4], [2, 3, 4]]
+        )
+        z_layer_centers = g.np.array([3, 3.0283334255218506])
+        m = g.trimesh.Trimesh(vertices, faces)
+        r = m.section_multiplane([0, 0, 0], [0, 0, 1], z_layer_centers)
+        assert len(r) == 2
+        assert all(i.is_closed for i in r)
+
 
 if __name__ == "__main__":
     g.trimesh.util.attach_to_log()
     g.unittest.main()
```

### Comparing `trimesh-4.3.2/tests/test_pbr.py` & `trimesh-4.4.0/tests/test_pbr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_permutate.py` & `trimesh-4.4.0/tests/test_permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_ply.py` & `trimesh-4.4.0/tests/test_ply.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
             # will raise if dtype string not valid
             g.np.dtype(d)
 
     def test_ply(self):
         m = g.get_mesh("machinist.XAML")
 
         assert m.visual.kind == "face"
-        assert m.visual.face_colors.ptp(axis=0).max() > 0
+        assert g.np.ptp(m.visual.face_colors, axis=0).max() > 0
 
         export = m.export(file_type="ply")
         reconstructed = g.roundtrip(export, file_type="ply")
 
         assert reconstructed.visual.kind == "face"
 
         assert g.np.allclose(reconstructed.visual.face_colors, m.visual.face_colors)
 
         m = g.get_mesh("reference.ply")
 
         assert m.visual.kind == "vertex"
-        assert m.visual.vertex_colors.ptp(axis=0).max() > 0
+        assert g.np.ptp(m.visual.vertex_colors, axis=0).max() > 0
 
         export = m.export(file_type="ply")
         reconstructed = g.roundtrip(export, file_type="ply")
         assert reconstructed.visual.kind == "vertex"
 
         assert g.np.allclose(reconstructed.visual.vertex_colors, m.visual.vertex_colors)
```

### Comparing `trimesh-4.3.2/tests/test_points.py` & `trimesh-4.4.0/tests/test_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 
         # make sure vertices and colors are new shape
         assert cloud.vertices.shape == new_shape
         assert len(cloud.colors) == new_shape[0]
         assert hash(cloud) != initial_hash
 
         # AABB volume should be same as points
-        assert g.np.isclose(cloud.bounding_box.volume, g.np.prod(points.ptp(axis=0)))
+        assert g.np.isclose(
+            cloud.bounding_box.volume, g.np.prod(g.np.ptp(points, axis=0))
+        )
 
         # will populate all bounding primitives
         assert cloud.bounding_primitive.volume > 0.0
         # ... except AABB (it uses OBB)
         assert cloud.bounding_box.volume > 0.0
 
         # check getitem and setitem
@@ -149,15 +151,15 @@
             clustered.append((group / 1000) + (index * 100))
         clustered = g.np.vstack(clustered)
 
         # run k- means clustering on our nicely separated data
         centroids, klabel = g.trimesh.points.k_means(points=clustered, k=cluster_count)
 
         # reshape to make sure all groups have the same index
-        variance = klabel.reshape((cluster_count, points_per_cluster)).ptp(axis=1)
+        variance = g.np.ptp(klabel.reshape((cluster_count, points_per_cluster)), axis=1)
 
         assert len(centroids) == cluster_count
         assert (variance == 0).all()
 
     def test_tsp(self):
         """
         Test our solution for visiting every point in order.
```

### Comparing `trimesh-4.3.2/tests/test_polygons.py` & `trimesh-4.4.0/tests/test_polygons.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         assert s.shape[1] == 2
         radius = (s**2).sum(axis=1).max()
         assert radius < (1.0 + 1e-8)
 
         # try getting OBB of samples
         _T, extents = g.trimesh.path.polygons.polygon_obb(s)
         # OBB of samples should be less than diameter of circle
-        diameter = g.np.reshape(p.bounds, (2, 2)).ptp(axis=0).max()
+        diameter = g.np.ptp(g.np.reshape(p.bounds, (2, 2)), axis=0).max()
         assert (extents <= diameter).all()
 
         # test sampling with multiple bodies
         for i in range(3):
             assert g.np.isclose(path.area, p.area * (i + 1))
             path = path + g.trimesh.load_path(g.Point([(i + 2) * 2, 0]).buffer(1.0))
             s = path.sample(count=count)
```

### Comparing `trimesh-4.3.2/tests/test_poses.py` & `trimesh-4.4.0/tests/test_poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_primitives.py` & `trimesh-4.4.0/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_proximity.py` & `trimesh-4.4.0/tests/test_proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_raster.py` & `trimesh-4.4.0/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_ray.py` & `trimesh-4.4.0/tests/test_ray.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             name = m.metadata["file_name"]
             hit_any.append(m.ray.intersects_any(**rays[name]))
             hit_loc.append(m.ray.intersects_location(**rays[name])[0])
             hit_id.append(m.ray.intersects_id(**rays[name]))
         hit_any = g.np.array(hit_any, dtype=g.np.int64)
 
         for i in g.trimesh.grouping.group(g.np.unique(names, return_inverse=True)[1]):
-            broken = hit_any[i].astype(g.np.int64).ptp(axis=0).sum()
+            broken = g.np.ptp(hit_any[i].astype(g.np.int64), axis=0).sum()
             assert broken == 0
 
     def test_rps(self):
         for use_embree in [True, False]:
             dimension = (10000, 3)
             sphere = g.get_mesh("unit_sphere.STL", use_embree=use_embree)
```

### Comparing `trimesh-4.3.2/tests/test_registration.py` & `trimesh-4.4.0/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_remesh.py` & `trimesh-4.4.0/tests/test_remesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                     m.triangles[idx], sub.vertices[vid]
                 )
                 # if face indexes are correct they will be on the triangle
                 # which means all barycentric coordinates are between 0.0-1.0
                 assert bary.max() < (1 + epsilon)
                 assert bary.min() > -epsilon
                 # make sure it's not all zeros
-                assert bary.ptp() > epsilon
+                assert g.np.ptp(bary) > epsilon
 
             v, f = g.trimesh.remesh.subdivide(vertices=m.vertices, faces=m.faces)
 
             max_edge = m.scale / 50
             v, f, idx = g.trimesh.remesh.subdivide_to_size(
                 vertices=m.vertices, faces=m.faces, max_edge=max_edge, return_index=True
             )
@@ -70,15 +70,15 @@
                 # find the barycentric coordinates
                 bary = g.trimesh.triangles.points_to_barycentric(m.triangles[idx], v[vid])
                 # if face indexes are correct they will be on the triangle
                 # which means all barycentric coordinates are between 0.0-1.0
                 assert bary.max() < (1 + epsilon)
                 assert bary.min() > -epsilon
                 # make sure it's not all zeros
-                assert bary.ptp() > epsilon
+                assert g.np.ptp(bary) > epsilon
 
             check = m.subdivide_to_size(
                 max_edge=m.extents.sum(), max_iter=1, return_index=False
             )
             assert check.faces.shape == m.faces.shape
 
     def test_sub(self):
@@ -197,16 +197,16 @@
 
         # original UV coordinates with faces
         ov = m.visual.uv[m.faces]
         # subdivided mesh faces
         sv = s.visual.uv[s.faces]
         # both subdivided and original should have faces
         # that don't vary wildly
-        assert ov.ptp(axis=1).mean(axis=0).max() < 0.1
-        assert sv.ptp(axis=1).mean(axis=0).max() < 0.1
+        assert g.np.ptp(ov, axis=1).mean(axis=0).max() < 0.1
+        assert g.np.ptp(sv, axis=1).mean(axis=0).max() < 0.1
 
         max_edge = m.scale / 50
         s = m.subdivide_to_size(max_edge=max_edge)
 
         # shouldn't have changed source mesh
         assert m.vertices.shape == shape
         # subdivided mesh should have more vertices
@@ -216,16 +216,16 @@
 
         # original UV coordinates with faces
         ov = m.visual.uv[m.faces]
         # subdivided mesh faces
         sv = s.visual.uv[s.faces]
         # both subdivided and original should have faces
         # that don't vary wildly
-        assert ov.ptp(axis=1).mean(axis=0).max() < 0.1
-        assert sv.ptp(axis=1).mean(axis=0).max() < 0.1
+        assert g.np.ptp(ov, axis=1).mean(axis=0).max() < 0.1
+        assert g.np.ptp(sv, axis=1).mean(axis=0).max() < 0.1
 
     def test_max_iter(self):
         m = g.trimesh.creation.box()
         try:
             m.subdivide_to_size(0.01, max_iter=1)
             raise BaseException("that shouldn't have worked!")
         except ValueError:
```

### Comparing `trimesh-4.3.2/tests/test_render.py` & `trimesh-4.4.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_repair.py` & `trimesh-4.4.0/tests/test_repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_repr.py` & `trimesh-4.4.0/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_resolvers.py` & `trimesh-4.4.0/tests/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_runlength.py` & `trimesh-4.4.0/tests/test_runlength.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_sample.py` & `trimesh-4.4.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_scene.py` & `trimesh-4.4.0/tests/test_scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 try:
     from . import generic as g
 except BaseException:
     import generic as g
 
 
 class SceneTests(g.unittest.TestCase):
@@ -98,14 +100,39 @@
                 s.rezero()
                 # if our cache dump was bad this will fail
                 assert g.np.allclose(s.centroid, 0, atol=1e-5)
 
                 # make sure explode doesn't crash
                 s.explode()
 
+    def test_cam_gltf(self):
+        # Test that the camera is stored and loaded successfully into a Scene from a gltf.
+        cam = g.trimesh.scene.cameras.Camera(fov=[60, 90], name="cam1")
+        box = g.trimesh.creation.box(extents=[1, 2, 3])
+        scene = g.trimesh.Scene(
+            geometry=[box],
+            camera=cam,
+            camera_transform=np.array(
+                [[0, 1, 0, -1], [1, 0, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]
+            ),
+        )
+        with g.TemporaryDirectory() as d:
+            # exports by path allow files to be written
+            path = g.os.path.join(d, "tmp.glb")
+            scene.export(path)
+            r = g.trimesh.load(path, force="scene")
+
+            # ensure no added nodes
+            assert set(r.graph.nodes) == {"world", "geometry_0", "cam1"}
+            # ensure same camera parameters and extrinsics
+            assert (r.camera_transform == scene.camera_transform).all()
+            assert r.camera.name == cam.name
+            assert (r.camera.fov == cam.fov).all()
+            assert r.camera.z_near == cam.z_near
+
     def test_scaling(self):
         # Test the scaling of scenes including unit conversion.
 
         scene = g.get_mesh("cycloidal.3DXML")
 
         hash_val = scene.__hash__()
         extents = scene.bounding_box_oriented.primitive.extents.copy()
```

### Comparing `trimesh-4.3.2/tests/test_scenegraph.py` & `trimesh-4.4.0/tests/test_scenegraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         forest = g.trimesh.scene.transforms.EnforcedForest()
         for k, v in edgelist.items():
             forest.add_edge(*k, **v)
 
         # generate a lot of random queries
         queries = g.np.random.choice(list(forest.nodes), 10000).reshape((-1, 2))
         # filter out any self-queries as networkx doesn't handle them
-        queries = queries[queries.ptp(axis=1) > 0]
+        queries = queries[g.np.ptp(queries, axis=1) > 0]
 
         # now run our shortest path algorithm in a profiler
         with g.Profiler() as P:
             ours = [forest.shortest_path(*q) for q in queries]
         # print this way to avoid a python2 syntax error
         g.log.debug(P.output_text())
```

### Comparing `trimesh-4.3.2/tests/test_section.py` & `trimesh-4.4.0/tests/test_section.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,16 +95,16 @@
                 # send Path2D back to 3D using the transform returned by
                 # section
                 back_3D = paths[index].to_3D(paths[index].metadata["to_3D"])
                 # move to parallel test plane
                 back_3D.apply_transform(base_inv)
 
                 # make sure all vertices have constant Z
-                assert back_3D.vertices[:, 2].ptp() < 1e-8
-                assert sections_3D[index].vertices[:, 2].ptp() < 1e-8
+                assert g.np.ptp(back_3D.vertices[:, 2]) < 1e-8
+                assert g.np.ptp(sections_3D[index].vertices[:, 2]) < 1e-8
 
                 # make sure reconstructed 3D section is at right height
                 assert g.np.isclose(
                     back_3D.vertices[:, 2].mean(),
                     sections_3D[index].vertices[:, 2].mean(),
                 )
```

### Comparing `trimesh-4.3.2/tests/test_segments.py` & `trimesh-4.4.0/tests/test_segments.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         n = segments.colinear_pairs(seg, length=epsilon)
         dots = [g.np.dot(*row) for row in unit[L]]
         assert (g.np.isclose(dots, 1.0) | g.np.isclose(dots, -1)).all()
 
         for pair in n:
             val = seg[pair]
             close = g.np.append(
-                (val[0] - val[1]).ptp(axis=1), (val[0] - val[1][::-1]).ptp(axis=1)
+                g.np.ptp(val[0] - val[1], axis=1), g.np.ptp(val[0] - val[1][::-1], axis=1)
             ).min()
             assert close < epsilon
 
     def test_extrude(self):
         from trimesh.path.segments import extrude
 
         # hand tuned segments
```

### Comparing `trimesh-4.3.2/tests/test_simplify.py` & `trimesh-4.4.0/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_smooth.py` & `trimesh-4.4.0/tests/test_smooth.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_smoothing.py` & `trimesh-4.4.0/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_splines.py` & `trimesh-4.4.0/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_step.py` & `trimesh-4.4.0/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_stl.py` & `trimesh-4.4.0/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_svg.py` & `trimesh-4.4.0/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_sweep.py` & `trimesh-4.4.0/tests/test_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     # a simple extrusion
     path = [[0, 0, 0], [0, 0, height]]
     # will be running asserts inside function
     b = sweep_polygon(circle, path)
 
     # should be a straight extrude along Z
-    expected = np.append(np.reshape(circle.bounds, (2, 2)).ptp(axis=0), height)
+    expected = np.append(np.ptp(np.reshape(circle.bounds, (2, 2)), axis=0), height)
     assert np.allclose(expected, b.extents)
 
     # should be well constructed
     assert b.is_volume
     # volume should correspond to expected cylinder area
     assert np.isclose(b.volume, circle.area * height)
```

### Comparing `trimesh-4.3.2/tests/test_texture.py` & `trimesh-4.4.0/tests/test_texture.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_thickness.py` & `trimesh-4.4.0/tests/test_thickness.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_trackball.py` & `trimesh-4.4.0/tests/test_trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_transformations.py` & `trimesh-4.4.0/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_triangles.py` & `trimesh-4.4.0/tests/test_triangles.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_units.py` & `trimesh-4.4.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_unwrap.py` & `trimesh-4.4.0/tests/test_unwrap.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_upstream.py` & `trimesh-4.4.0/tests/test_upstream.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_urdf.py` & `trimesh-4.4.0/tests/test_urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_util.py` & `trimesh-4.4.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_vector.py` & `trimesh-4.4.0/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_vertices.py` & `trimesh-4.4.0/tests/test_vertices.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_viewer.py` & `trimesh-4.4.0/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_visual.py` & `trimesh-4.4.0/tests/test_visual.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/tests/test_voxel.py` & `trimesh-4.4.0/tests/test_voxel.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         except ImportError:
             g.log.warning("no skimage, skipping marching cubes test")
             return
 
         # get some points on the surface of an icosahedron
         points = g.trimesh.creation.icosahedron().sample(1000)
         # make the pitch proportional to scale
-        pitch = points.ptp(axis=0).min() / 10
+        pitch = g.np.ptp(points, axis=0).min() / 10
         # run marching cubes
         mesh = g.trimesh.voxel.ops.points_to_marching_cubes(points=points, pitch=pitch)
 
         # mesh should have faces
         assert len(mesh.faces) > 0
         # mesh should be roughly centered
         assert (mesh.bounds[0] < -0.5).all()
```

### Comparing `trimesh-4.3.2/trimesh/__init__.py` & `trimesh-4.4.0/trimesh/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/base.py` & `trimesh-4.4.0/trimesh/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
         values = np.asanyarray(values, order="C", dtype=float64)
         # face normals need to correspond to faces
         if len(values) == 0 or values.shape != self.faces.shape:
             log.debug("face_normals incorrect shape, ignoring!")
             return
         # check if any values are larger than tol.merge
         # don't set the normals if they are all zero
-        ptp = values.ptp()
+        ptp = np.ptp(values)
         if not np.isfinite(ptp):
             log.debug("face_normals contain NaN, ignoring!")
             return
         if ptp < tol.merge:
             log.debug("face_normals all zero, ignoring!")
             return
 
@@ -499,15 +499,15 @@
         values : (len(self.vertices), 3) float
           Unit normal vectors for each vertex
         """
         if values is not None:
             values = np.asanyarray(values, order="C", dtype=float64)
             if values.shape == self.vertices.shape:
                 # check to see if they assigned all zeros
-                if values.ptp() < tol.merge:
+                if np.ptp(values) < tol.merge:
                     log.debug("vertex_normals are all zero!")
                 self._cache["vertex_normals"] = values
 
     @caching.cache_decorator
     def vertex_faces(self) -> NDArray[int64]:
         """
         A representation of the face indices that correspond to each vertex.
@@ -556,15 +556,15 @@
         extents : (3, ) float or None
           Array containing axis aligned [length, width, height]
           If mesh is empty returns None
         """
         # if mesh is empty return None
         if self.bounds is None:
             return None
-        extents = self.bounds.ptp(axis=0)
+        extents = np.ptp(self.bounds, axis=0)
 
         return extents
 
     @caching.cache_decorator
     def centroid(self) -> NDArray[float64]:
         """
         The point in space which is the average of the triangle
```

### Comparing `trimesh-4.3.2/trimesh/boolean.py` & `trimesh-4.4.0/trimesh/boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/bounds.py` & `trimesh-4.4.0/trimesh/bounds.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,37 +268,37 @@
         # however, we have reduced n with a convex hull and numpy dot products
         # are extremely fast so in practice this usually ends up being fine
         x = np.dot(edge_vectors, edge_vert[:, 0, :2].T)
         y = np.dot(perp_vectors, edge_vert[:, 0, :2].T)
         area = ((x.max(axis=1) - x.min(axis=1)) * (y.max(axis=1) - y.min(axis=1))).min()
 
         # the volume is 2D area plus the projected height
-        volume = area * projected[:, 2].ptp()
+        volume = area * np.ptp(projected[:, 2])
 
         # store this transform if it's better than one we've seen
         if volume < min_volume:
             min_volume = volume
             min_2D = to_2D
 
     # we know the minimum volume transform which should be the expensive
     # part so now we need to do the bookkeeping to find the box
     vert_ones = np.column_stack((vertices, np.ones(len(vertices)))).T
     projected = np.dot(min_2D, vert_ones).T[:, :3]
-    height = projected[:, 2].ptp()
+    height = np.ptp(projected[:, 2])
     rotation_2D, box = oriented_bounds_2D(projected[:, :2])
     min_extents = np.append(box, height)
     rotation_2D[:2, 2] = 0.0
     rotation_Z = transformations.planar_matrix_to_3D(rotation_2D)
 
     # combine the 2D OBB transformation with the 2D projection transform
     to_origin = np.dot(rotation_Z, min_2D)
 
     # transform points using our matrix to find the translation
     transformed = transformations.transform_points(vertices, to_origin)
-    box_center = transformed.min(axis=0) + transformed.ptp(axis=0) * 0.5
+    box_center = transformed.min(axis=0) + np.ptp(transformed, axis=0) * 0.5
     to_origin[:3, 3] = -box_center
 
     # return ordered 3D extents
     if ordered:
         # sort the three extents
         order = min_extents.argsort()
         # generate a matrix which will flip transform
@@ -370,15 +370,15 @@
             radius (float)
             height (float)
         else:
             volume (float)
         """
         to_2D = transformations.spherical_matrix(*spherical, axes="rxyz")
         projected = transformations.transform_points(hull, matrix=to_2D)
-        height = projected[:, 2].ptp()
+        height = np.ptp(projected[:, 2])
 
         try:
             center_2D, radius = nsphere.minimum_nsphere(projected[:, :2])
         except ValueError:
             return np.inf
 
         volume = np.pi * height * (radius**2)
@@ -401,15 +401,15 @@
             # convex hull should be watertight
             origin = obj.convex_hull.center_mass
         # will align symmetry axis with Z and move origin to zero
         to_2D = geometry.plane_transform(origin=origin, normal=obj.symmetry_axis)
         # transform vertices to plane to check
         on_plane = transformations.transform_points(obj.vertices, to_2D)
         # cylinder height is overall Z span
-        height = on_plane[:, 2].ptp()
+        height = np.ptp(on_plane[:, 2])
         # center mass is correct on plane, but position
         # along symmetry axis may be wrong so slide it
         slide = transformations.translation_matrix(
             [0, 0, (height / 2.0) - on_plane[:, 2].max()]
         )
         to_2D = np.dot(slide, to_2D)
         # radius is maximum radius
@@ -477,15 +477,15 @@
     transform : (4, 4) float
       Homogeneous transform moving extents to bounds
     """
     bounds = np.asanyarray(bounds, dtype=np.float64)
     if bounds.shape != (2, 3):
         raise ValueError("bounds must be (2, 3)")
 
-    extents = bounds.ptp(axis=0)
+    extents = np.ptp(bounds, axis=0)
     transform = np.eye(4)
     transform[:3, 3] = bounds.mean(axis=0)
 
     return extents, transform
 
 
 def corners(bounds):
```

### Comparing `trimesh-4.3.2/trimesh/caching.py` & `trimesh-4.4.0/trimesh/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,21 +182,21 @@
         during copies and certain types of slicing.
         """
 
         self._dirty_hash = True
         if isinstance(obj, type(self)):
             obj._dirty_hash = True
 
-    def __array_wrap__(self, out_arr, context=None):
+    def __array_wrap__(self, out_arr, context=None, *args, **kwargs):
         """
         Return a numpy scalar if array is 0d.
         See https://github.com/numpy/numpy/issues/5819
         """
         if out_arr.ndim:
-            return np.ndarray.__array_wrap__(self, out_arr, context)
+            return np.ndarray.__array_wrap__(self, out_arr, context, *args, **kwargs)
         # Match numpy's behavior and return a numpy dtype scalar
         return out_arr[()]
 
     @property
     def mutable(self):
         return self.flags["WRITEABLE"]
```

### Comparing `trimesh-4.3.2/trimesh/collision.py` & `trimesh-4.4.0/trimesh/collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/comparison.py` & `trimesh-4.4.0/trimesh/comparison.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/constants.py` & `trimesh-4.4.0/trimesh/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
 import numpy as np
 
-from .util import log, now
+from .util import decimal_to_digits, log, now
 
 
 @dataclass
 class ToleranceMesh:
     """
     ToleranceMesh objects hold tolerance information about meshes.
 
@@ -84,27 +84,31 @@
        When simplifying line segments to curves, what is the maximum
        angle the end sections can deviate from tangent that is
        acceptable.
     """
 
     zero: float = 1e-12
     merge: float = 1e-5
+
     planar: float = 1e-5
     seg_frac: float = 0.125
     seg_angle: float = float(np.radians(50))
     seg_angle_min: float = float(np.radians(1))
     seg_angle_frac: float = 0.5
     aspect_frac: float = 0.1
     radius_frac: float = 0.02
     radius_min: float = 1e-4
     radius_max: float = 50.0
     tangent: float = float(np.radians(20))
-
     strict: bool = False
 
+    @property
+    def merge_digits(self) -> int:
+        return decimal_to_digits(self.merge)
+
 
 @dataclass
 class ResolutionPath:
     """
     res.seg_frac : float
       When discretizing curves, what percentage of the drawing
       scale should we aim to make a single segment
```

### Comparing `trimesh-4.3.2/trimesh/convex.py` & `trimesh-4.4.0/trimesh/convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/creation.py` & `trimesh-4.4.0/trimesh/creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,15 +710,15 @@
     # resize cube based on passed extents
     if bounds is not None:
         if transform is not None or extents is not None:
             raise ValueError("`bounds` overrides `extents`/`transform`!")
         bounds = np.array(bounds, dtype=np.float64)
         if bounds.shape != (2, 3):
             raise ValueError("`bounds` must be (2, 3) float!")
-        extents = bounds.ptp(axis=0)
+        extents = np.ptp(bounds, axis=0)
         vertices *= extents
         vertices += bounds[0]
     elif extents is not None:
         extents = np.asanyarray(extents, dtype=np.float64)
         if extents.shape != (3,):
             raise ValueError("Extents must be (3,)!")
         vertices -= 0.5
```

### Comparing `trimesh-4.3.2/trimesh/curvature.py` & `trimesh-4.4.0/trimesh/curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/decomposition.py` & `trimesh-4.4.0/trimesh/decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exceptions.py` & `trimesh-4.4.0/trimesh/exceptions.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/binvox.py` & `trimesh-4.4.0/trimesh/exchange/binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/cascade.py` & `trimesh-4.4.0/trimesh/exchange/cascade.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/dae.py` & `trimesh-4.4.0/trimesh/exchange/dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/export.py` & `trimesh-4.4.0/trimesh/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/gltf.py` & `trimesh-4.4.0/trimesh/exchange/gltf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 from collections import OrderedDict, defaultdict, deque
 
 import numpy as np
 
 from .. import rendering, resources, transformations, util, visual
 from ..caching import hash_fast
 from ..constants import log, tol
-from ..typed import NDArray, Optional
-from ..util import unique_name
+from ..resolvers import Resolver, ZipResolver
+from ..scene.cameras import Camera
+from ..typed import Mapping, NDArray, Optional, Stream, Union
+from ..util import triangle_strips_to_faces, unique_name
 from ..visual.gloss import specular_to_pbr
 
 # magic numbers which have meaning in GLTF
 # most are uint32's of UTF-8 text
 _magic = {"gltf": 1179937895, "json": 1313821514, "bin": 5130562}
 
 # GLTF data type codes: little endian numpy dtypes
@@ -44,14 +46,17 @@
     "pbrMetallicRoughness": {
         "baseColorFactor": [1, 1, 1, 1],
         "metallicFactor": 0,
         "roughnessFactor": 0,
     }
 }
 
+# we can accept dict resolvers
+ResolverLike = Union[Resolver, Mapping]
+
 # GL geometry modes
 _GL_LINES = 1
 _GL_POINTS = 0
 _GL_TRIANGLES = 4
 _GL_STRIP = 5
 
 _EYE = np.eye(4)
@@ -257,19 +262,19 @@
     if tol.strict:
         validate(tree)
 
     return exported
 
 
 def load_gltf(
-    file_obj=None,
-    resolver=None,
-    ignore_broken=False,
-    merge_primitives=False,
-    skip_materials=False,
+    file_obj: Optional[Stream] = None,
+    resolver: Optional[ResolverLike] = None,
+    ignore_broken: bool = False,
+    merge_primitives: bool = False,
+    skip_materials: bool = False,
     **mesh_kwargs,
 ):
     """
     Load a GLTF file, which consists of a directory structure
     with multiple files.
 
     Parameters
@@ -332,19 +337,19 @@
         skip_materials=skip_materials,
         resolver=resolver,
     )
     return kwargs
 
 
 def load_glb(
-    file_obj,
-    resolver=None,
-    ignore_broken=False,
-    merge_primitives=False,
-    skip_materials=False,
+    file_obj: Stream,
+    resolver: Optional[ResolverLike] = None,
+    ignore_broken: bool = False,
+    merge_primitives: bool = False,
+    skip_materials: bool = False,
     **mesh_kwargs,
 ):
     """
     Load a GLTF file in the binary GLB format into a trimesh.Scene.
 
     Implemented from specification:
     https://github.com/KhronosGroup/glTF/tree/master/specification/2.0
@@ -440,14 +445,15 @@
     kwargs = _read_buffers(
         header=header,
         buffers=buffers,
         ignore_broken=ignore_broken,
         merge_primitives=merge_primitives,
         skip_materials=skip_materials,
         mesh_kwargs=mesh_kwargs,
+        resolver=resolver,
     )
 
     return kwargs
 
 
 def _uri_to_bytes(uri, resolver):
     """
@@ -1346,18 +1352,18 @@
     return materials
 
 
 def _read_buffers(
     header,
     buffers,
     mesh_kwargs,
-    ignore_broken=False,
-    merge_primitives=False,
-    skip_materials=False,
-    resolver=None,
+    resolver: Optional[ResolverLike],
+    ignore_broken: bool = False,
+    merge_primitives: bool = False,
+    skip_materials: bool = False,
 ):
     """
     Given binary data and a layout return the
     kwargs to create a scene object.
 
     Parameters
     -----------
@@ -1507,23 +1513,29 @@
                     # get vertices from accessors
                     kwargs["vertices"] = access[attr["POSITION"]]
                     # get faces from accessors
                     if "indices" in p:
                         if mode == _GL_STRIP:
                             # this is triangle strips
                             flat = access[p["indices"]].reshape(-1)
-                            kwargs["faces"] = util.triangle_strips_to_faces([flat])
+                            kwargs["faces"] = triangle_strips_to_faces([flat])
                         else:
                             kwargs["faces"] = access[p["indices"]].reshape((-1, 3))
                     else:
                         # indices are apparently optional and we are supposed to
                         # do the same thing as webGL drawArrays?
-                        kwargs["faces"] = np.arange(
-                            len(kwargs["vertices"]) * 3, dtype=np.int64
-                        ).reshape((-1, 3))
+                        if mode == _GL_STRIP:
+                            kwargs["faces"] = triangle_strips_to_faces(
+                                np.array([np.arange(len(kwargs["vertices"]))])
+                            )
+                        else:
+                            # GL_TRIANGLES
+                            kwargs["faces"] = np.arange(
+                                len(kwargs["vertices"]), dtype=np.int64
+                            ).reshape((-1, 3))
 
                     if "NORMAL" in attr:
                         # vertex normals are specified
                         kwargs["vertex_normals"] = access[attr["NORMAL"]]
                         # do we have UV coordinates
                     visuals = None
                     if "material" in p and not skip_materials:
@@ -1660,14 +1672,18 @@
     names[base_frame] = base_frame
 
     # visited, kwargs for scene.graph.update
     graph = deque()
     # unvisited, pairs of node indexes
     queue = deque()
 
+    # camera(s), if they exist
+    camera = None
+    camera_transform = None
+
     if "scene" in header:
         # specify the index of scenes if specified
         scene_index = header["scene"]
     else:
         # otherwise just use the first index
         scene_index = 0
 
@@ -1731,14 +1747,28 @@
             )
         if "scale" in child:
             # add scale to the matrix
             kwargs["matrix"] = np.dot(
                 kwargs["matrix"], np.diag(np.concatenate((child["scale"], [1.0])))
             )
 
+        # If a camera exists, create the camera and dont add the node to the graph
+        # TODO only process the first camera, ignore the rest
+        # TODO assumes the camera node is child of the world frame
+        # TODO will only read perspective camera
+        if "camera" in child and camera is None:
+            cam_idx = child["camera"]
+            try:
+                camera = _cam_from_gltf(header["cameras"][cam_idx])
+            except KeyError:
+                log.debug("GLTF camera is not fully-defined")
+            if camera:
+                camera_transform = kwargs["matrix"]
+            continue
+
         # treat node metadata similarly to mesh metadata
         if isinstance(child.get("extras"), dict):
             kwargs["metadata"] = child["extras"]
 
         # put any node extensions in a field of the metadata
         if "extensions" in child:
             if "metadata" not in kwargs:
@@ -1776,14 +1806,16 @@
 
     # kwargs for load_kwargs
     result = {
         "class": "Scene",
         "geometry": meshes,
         "graph": graph,
         "base_frame": base_frame,
+        "camera": camera,
+        "camera_transform": camera_transform,
     }
     try:
         # load any scene extras into scene.metadata
         # use a try except to avoid nested key checks
         result["metadata"] = header["scenes"][header["scene"]]["extras"]
     except BaseException:
         pass
@@ -1795,14 +1827,46 @@
         result["metadata"]["gltf_extensions"] = header["extensions"]
     except BaseException:
         pass
 
     return result
 
 
+def _cam_from_gltf(cam):
+    """
+    Convert a gltf perspective camera to trimesh.
+
+    The retrieved camera will have default resolution, since the gltf specification
+    does not contain it.
+
+    If the camera is not perspective will return None.
+    If the camera is perspective but is missing fields, will raise `KeyError`
+
+    Parameters
+    ------------
+    cam : dict
+      Camera represented as a dictionary according to glTF
+
+    Returns
+    -------------
+    camera : trimesh.scene.cameras.Camera
+      Trimesh camera object
+    """
+    if "perspective" not in cam:
+        return
+    name = cam.get("name")
+    znear = cam["perspective"]["znear"]
+    aspect_ratio = cam["perspective"]["aspectRatio"]
+    yfov = np.degrees(cam["perspective"]["yfov"])
+
+    fov = (aspect_ratio * yfov, yfov)
+
+    return Camera(name=name, fov=fov, z_near=znear)
+
+
 def _convert_camera(camera):
     """
     Convert a trimesh camera to a GLTF camera.
 
     Parameters
     ------------
     camera : trimesh.scene.cameras.Camera
@@ -2045,15 +2109,14 @@
     Returns
     ------------
     schema : dict
       A copy of the GLTF 2.0 schema without external references.
     """
     # replace references
     # get zip resolver to access referenced assets
-    from ..resolvers import ZipResolver
     from ..schemas import resolve
 
     # get a blob of a zip file including the GLTF 2.0 schema
     stream = resources.get_stream("schema/gltf2.schema.zip")
     # get the zip file as a dict keyed by file name
     archive = util.decompress(stream, "zip")
     # get a resolver object for accessing the schema
```

### Comparing `trimesh-4.3.2/trimesh/exchange/load.py` & `trimesh-4.4.0/trimesh/exchange/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,14 +409,20 @@
                 if isinstance(k, dict):
                     scene.graph.update(**k)
                 elif util.is_sequence(k) and len(k) == 3:
                     scene.graph.update(k[1], k[0], **k[2])
         else:
             scene = Scene(geometry)
 
+        # camera, if it exists
+        camera = kwargs.get("camera")
+        if camera:
+            scene.camera = camera
+            scene.camera_transform = kwargs.get("camera_transform")
+
         if "base_frame" in kwargs:
             scene.graph.base_frame = kwargs["base_frame"]
         metadata = kwargs.get("metadata")
         if isinstance(metadata, dict):
             scene.metadata.update(kwargs["metadata"])
         elif isinstance(metadata, str):
             # some ways someone might have encoded a string
```

### Comparing `trimesh-4.3.2/trimesh/exchange/misc.py` & `trimesh-4.4.0/trimesh/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/obj.py` & `trimesh-4.4.0/trimesh/exchange/obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/off.py` & `trimesh-4.4.0/trimesh/exchange/off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/ply.py` & `trimesh-4.4.0/trimesh/exchange/ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/stl.py` & `trimesh-4.4.0/trimesh/exchange/stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/threedxml.py` & `trimesh-4.4.0/trimesh/exchange/threedxml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/threemf.py` & `trimesh-4.4.0/trimesh/exchange/threemf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/urdf.py` & `trimesh-4.4.0/trimesh/exchange/urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/xaml.py` & `trimesh-4.4.0/trimesh/exchange/xaml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/exchange/xyz.py` & `trimesh-4.4.0/trimesh/exchange/xyz.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/geometry.py` & `trimesh-4.4.0/trimesh/geometry.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/graph.py` & `trimesh-4.4.0/trimesh/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,31 +277,35 @@
     """
     e_a = np.sort(faces_to_edges(faces_a), axis=1)
     e_b = np.sort(faces_to_edges(faces_b), axis=1)
     shared = grouping.boolean_rows(e_a, e_b, operation=np.intersect1d)
     return shared
 
 
-def facets(mesh, engine=None):
+def facets(mesh, engine=None, facet_threshold: Optional[Number] = None):
     """
     Find the list of parallel adjacent faces.
 
     Parameters
     -----------
-    mesh :  trimesh.Trimesh
+    mesh : trimesh.Trimesh
     engine : str
-       Which graph engine to use:
-       ('scipy', 'networkx')
+      Which graph engine to use:
+      ('scipy', 'networkx')
+    facet_threshold : float
+      Threshold for two facets to be considered coplanar
 
     Returns
     ---------
     facets : sequence of (n,) int
         Groups of face indexes of
         parallel adjacent faces.
     """
+    if facet_threshold is None:
+        facet_threshold = tol.facet_threshold
     # what is the radius of a circle that passes through the perpendicular
     # projection of the vector between the two non- shared vertices
     # onto the shared edge, with the face normal from the two adjacent faces
     radii = mesh.face_adjacency_radius
     # what is the span perpendicular to the shared edge
     span = mesh.face_adjacency_span
     # a very arbitrary formula for declaring two adjacent faces
@@ -310,15 +314,15 @@
     # a common failure mode is two faces that are very narrow with a slight
     # angle between them, so here we divide by the perpendicular span
     # to penalize very narrow faces, and then square it just for fun
     parallel = np.ones(len(radii), dtype=bool)
     # if span is zero we know faces are small/parallel
     nonzero = np.abs(span) > tol.zero
     # faces with a radii/span ratio larger than a threshold pass
-    parallel[nonzero] = (radii[nonzero] / span[nonzero]) ** 2 > tol.facet_threshold
+    parallel[nonzero] = (radii[nonzero] / span[nonzero]) ** 2 > facet_threshold
 
     # run connected components on the parallel faces to group them
     components = connected_components(
         mesh.face_adjacency[parallel],
         nodes=np.arange(len(mesh.faces)),
         min_len=2,
         engine=engine,
@@ -521,15 +525,15 @@
         edges_hash = grouping.hashable_rows(np.sort(edges, axis=1))
 
     # turn the (n,) traversal into (n-1, 2) edges
     trav_edge = np.column_stack((traversal[:-1], traversal[1:]))
     # hash each edge so we can compare to edge set
     trav_hash = grouping.hashable_rows(np.sort(trav_edge, axis=1))
     # check if each edge is contained in edge set
-    contained = np.in1d(trav_hash, edges_hash)
+    contained = np.isin(trav_hash, edges_hash)
 
     # exit early if every edge of traversal exists
     if contained.all():
         # just reshape one traversal
         split = [traversal]
     else:
         # find contiguous groups of contained edges
@@ -543,15 +547,15 @@
         # make sure elements of sequence are numpy arrays
         split[i] = np.asanyarray(split[i], dtype=np.int64)
         # don't close if its a single edge
         if len(t) <= 2:
             continue
         # make sure it's not already closed
         edge = np.sort([t[0], t[-1]])
-        if edge.ptp() == 0:
+        if np.ptp(edge) == 0:
             continue
         close = grouping.hashable_rows(edge.reshape((1, 2)))[0]
         # if we need the edge add it
         if close in edges_hash:
             split[i] = np.append(t, t[0]).astype(np.int64)
 
     return split
```

### Comparing `trimesh-4.3.2/trimesh/grouping.py` & `trimesh-4.4.0/trimesh/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 
         # if the data is within the range of our precision threshold
         if d_max < threshold and d_min > -threshold:
             # the resulting package
             hashable = np.zeros(len(as_int), dtype=np.uint64)
             # offset to the middle of the unsigned integer range
             # this array should contain only positive values
-            bitbang = (as_int + threshold).astype(np.uint64).T
+            bitbang = as_int.astype(np.uint64).T + threshold
             # loop through each column and bitwise xor to combine
             # make sure as_int is int64 otherwise bit offset won't work
             for offset, column in enumerate(bitbang):
                 # will modify hashable in place
                 np.bitwise_xor(hashable, column << (offset * precision), out=hashable)
             return hashable
```

### Comparing `trimesh-4.3.2/trimesh/inertia.py` & `trimesh-4.4.0/trimesh/inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/interfaces/blender.py` & `trimesh-4.4.0/trimesh/interfaces/blender.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/interfaces/generic.py` & `trimesh-4.4.0/trimesh/interfaces/generic.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/interfaces/gmsh.py` & `trimesh-4.4.0/trimesh/interfaces/gmsh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/intersections.py` & `trimesh-4.4.0/trimesh/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/interval.py` & `trimesh-4.4.0/trimesh/interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     b : (2, ) float
       Start and end of a 1D interval
 
     Returns
     --------------
     inter : (2, ) or (2, 2) float
       The unioned range from the two inputs,
-      if not `inter.ptp(axis=1)` will be zero.
+      if not np.ptp(`inter, axis=1)` will be zero.
     """
     a = np.array(a, dtype=np.float64)
     b = np.array(b, dtype=np.float64)
 
     # convert to vectorized form
     is_1D = a.shape == (2,)
     a = a.reshape((-1, 2))
```

### Comparing `trimesh-4.3.2/trimesh/nsphere.py` & `trimesh-4.4.0/trimesh/nsphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # the input complexity substantially and returns the same value
     points = convex.hull_points(obj)
 
     # we are scaling the mesh to a unit cube
     # this used to pass qhull_options 'QbB' to Voronoi however this had a bug somewhere
     # to avoid this we scale to a unit cube ourselves inside this function
     points_origin = points.min(axis=0)
-    points_scale = points.ptp(axis=0).min()
+    points_scale = np.ptp(points, axis=0).min()
     points = (points - points_origin) / points_scale
 
     # if all of the points are on an n-sphere already the voronoi
     # method will fail so we check a least squares fit before
     # bothering to compute the voronoi diagram
     fit_C, fit_R, fit_E = fit_nsphere(points)
     # return fit radius and center to global scale
@@ -165,15 +165,15 @@
     center_result, return_code = leastsq(residuals, guess, xtol=1e-8)
 
     if return_code not in [1, 2, 3, 4]:
         raise ValueError("Least square fit failed!")
 
     radii = util.row_norm(points - center_result)
     radius = radii.mean()
-    error = radii.ptp()
+    error = np.ptp(radii)
     return center_result, radius, error
 
 
 def is_nsphere(points):
     """
     Check if a list of points is an nsphere.
```

### Comparing `trimesh-4.3.2/trimesh/parent.py` & `trimesh-4.4.0/trimesh/parent.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/arc.py` & `trimesh-4.4.0/trimesh/path/arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/creation.py` & `trimesh-4.4.0/trimesh/path/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/curve.py` & `trimesh-4.4.0/trimesh/path/curve.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/entities.py` & `trimesh-4.4.0/trimesh/path/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
           Index of vertices
         """
         return self.points[0]
 
     @origin.setter
     def origin(self, value):
         value = int(value)
-        if not hasattr(self, "points") or self.points.ptp() == 0:
+        if not hasattr(self, "points") or np.ptp(self.points) == 0:
             self.points = np.ones(3, dtype=np.int64) * value
         else:
             self.points[0] = value
 
     @property
     def vector(self):
         """
```

### Comparing `trimesh-4.3.2/trimesh/path/exchange/dxf.py` & `trimesh-4.4.0/trimesh/path/exchange/dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/exchange/export.py` & `trimesh-4.4.0/trimesh/path/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/exchange/load.py` & `trimesh-4.4.0/trimesh/path/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/exchange/misc.py` & `trimesh-4.4.0/trimesh/path/exchange/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 from ... import graph, grouping, util
+from ...constants import tol_path
 from ..entities import Arc, Line
 
 
 def dict_to_path(as_dict):
     """
     Turn a pure dict into a dict containing entity objects that
     can be sent directly to a Path constructor.
@@ -58,15 +59,15 @@
         return result
     elif util.is_shape(lines, (-1, 2, (2, 3))):
         # case where we have line segments in 2D or 3D
         dimension = lines.shape[-1]
         # convert lines to even number of (n, dimension) points
         lines = lines.reshape((-1, dimension))
         # merge duplicate vertices
-        unique, inverse = grouping.unique_rows(lines)
+        unique, inverse = grouping.unique_rows(lines, digits=tol_path.merge_digits)
         # use scipy edges_to_path to skip creating
         # a bajillion individual line entities which
         # will be super slow vs. fewer polyline entities
         return edges_to_path(edges=inverse.reshape((-1, 2)), vertices=lines[unique])
     else:
         raise ValueError("Lines must be (n,(2|3)) or (n,2,(2|3))")
     return result
```

### Comparing `trimesh-4.3.2/trimesh/path/exchange/svg_io.py` & `trimesh-4.4.0/trimesh/path/exchange/svg_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,15 @@
                         ]
                         for a in chunk
                     ],
                     dtype=np.float64,
                 )
                 # all arcs share the same center radius and rotation
                 closed = False
-                if verts[:, 4:].ptp(axis=0).mean() < 1e-3:
+                if np.ptp(verts[:, 4:], axis=0).mean() < 1e-3:
                     start, end = verts[:, :2], verts[:, 2:4]
                     # if every end point matches the start point of a new
                     # arc that means this is really a closed circle made
                     # up of multiple arc segments
                     closed = util.allclose(start, np.roll(end, 1, axis=0))
                 if closed:
                     # hot-patch a closed arc flag
```

### Comparing `trimesh-4.3.2/trimesh/path/intersections.py` & `trimesh-4.4.0/trimesh/path/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/packing.py` & `trimesh-4.4.0/trimesh/path/packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             # reorder with permutations
             order = np.random.permutation(order)
 
     if size is None:
         # if no bounds are passed start it with the size of a large
         # rectangle exactly which will require re-rooting for
         # subsequent insertions
-        root_bounds = [[0.0] * dimension, extents[extents.ptp(axis=1).argmax()]]
+        root_bounds = [[0.0] * dimension, extents[np.ptp(extents, axis=1).argmax()]]
     else:
         # restrict the bounds to passed size and disallow re-rooting
         root_bounds = [[0.0] * dimension, size]
 
     # the current root node to insert each rectangle
     root = RectangleBin(bounds=root_bounds)
 
@@ -226,15 +226,15 @@
 
         if inserted is None and size is None:
             # we failed to insert into children
             # so we need to create a new parent
             # get the size of the current root node
             bounds = root.bounds
             # current extents
-            current = bounds.ptp(axis=0)
+            current = np.ptp(bounds, axis=0)
 
             # pick the direction which has the least hyper-volume.
             best = np.inf
             for roll in range(len(current)):
                 stack = np.array([current, _roll(rectangle, roll)])
                 # we are going to combine two hyper-rect
                 # so we have `dim` choices on ways to split
@@ -276,15 +276,15 @@
             new_root = RectangleBin([bounds[0], new_max])
             # this node has children so it is occupied
             new_root.occupied = True
             # create a bin for both bounds
             new_root.child = [RectangleBin(bounds_ori), RectangleBin(bounds_ins)]
 
             # insert the original sheet into the new tree
-            root_offset = new_root.child[0].insert(bounds.ptp(axis=0), rotate=rotate)
+            root_offset = new_root.child[0].insert(np.ptp(bounds, axis=0), rotate=rotate)
             # we sized the cells so original tree would fit
             assert root_offset is not None
 
             # existing inserts need to be moved
             if not allclose(root_offset[0][0], 0.0):
                 offset[consume] += root_offset[0][0]
 
@@ -473,15 +473,15 @@
         # run a single insertion order
         # don't shuffle the first run, shuffle subsequent runs
         bounds, insert = rectangles_single(
             extents=extents, size=size, shuffle=(i != 0), rotate=rotate, random=random
         )
 
         count = insert.sum()
-        extents_all = bounds.reshape((-1, dim)).ptp(axis=0)
+        extents_all = np.ptp(bounds.reshape((-1, dim)), axis=0)
 
         if quanta is not None:
             # compute the density using an upsized quanta
             extents = np.ceil(extents_all / quanta) * quanta
 
         # calculate the packing density
         density = area[insert].sum() / np.prod(extents_all)
@@ -556,15 +556,15 @@
             seed=seed,
             spacing=spacing,
         )
         # really should have inserted all the rect
         assert insert.all()
         # re-index bounds back to original indexes
         bounds = bounds[inverse]
-        assert np.allclose(bounds.ptp(axis=1), [i.size for i in images])
+        assert np.allclose(np.ptp(bounds, axis=1), [i.size for i in images])
     else:
         # use the number of pixels as the rectangle size
         bounds, insert = rectangles(
             extents=[i.size for i in images],
             rotate=False,
             iterations=iterations,
             seed=seed,
@@ -576,15 +576,15 @@
     if spacing is None:
         spacing = 0
     else:
         spacing = int(spacing)
 
     # offsets should be integer multiple of pizels
     offset = bounds[:, 0].round().astype(int)
-    extents = bounds.reshape((-1, 2)).ptp(axis=0) + (spacing * 2)
+    extents = np.ptp(bounds.reshape((-1, 2)), axis=0) + (spacing * 2)
     size = extents.round().astype(int)
     if power_resize:
         # round up all dimensions to powers of 2
         size = (2 ** np.ceil(np.log2(size))).astype(np.int64)
 
     if mode is None:
         # get the mode of every input image
@@ -715,15 +715,15 @@
     """
     if len(bounds) != len(extents):
         raise ValueError("`bounds` must match `extents`")
     if len(extents) == 0:
         return []
 
     # find the size of the AABB of the passed bounds
-    passed = bounds.ptp(axis=1)
+    passed = np.ptp(bounds, axis=1)
     # zeroth index is 2D, `1` is 3D
     dimension = passed.shape[1]
 
     # store the resulting transformation matrices
     result = np.tile(np.eye(dimension + 1), (len(bounds), 1, 1))
 
     # a lookup table for rotations for rolling cuboiods
@@ -755,15 +755,15 @@
     # rectangular rotation involves rolling
     for roll in range(extents.shape[1]):
         # find all the passed bounding boxes represented by
         # rolling the original extents by this amount
         rolled = np.roll(extents, roll, axis=1)
         # check to see if the rolled original extents
         # match the requested bounding box
-        ok = (passed - rolled).ptp(axis=1) < _TOL_ZERO
+        ok = np.ptp((passed - rolled), axis=1) < _TOL_ZERO
         if not ok.any():
             continue
 
         # the base rotation for this
         mat = lookup[dimension - 2][roll]
         # the lower corner of the AABB plus the rolled extent
         offset = np.tile(np.eye(dimension + 1), (ok.sum(), 1, 1))
```

### Comparing `trimesh-4.3.2/trimesh/path/path.py` & `trimesh-4.4.0/trimesh/path/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         The size of the axis aligned bounding box.
 
         Returns
         ---------
         extents : (dimension,) float
           Edge length of AABB
         """
-        return self.bounds.ptp(axis=0)
+        return np.ptp(self.bounds, axis=0)
 
     def convert_units(self, desired: str, guess: bool = False):
         """
         Convert the units of the current drawing in place.
 
         Parameters
         -----------
@@ -829,15 +829,15 @@
 
         # transform all vertices to 2D plane
         flat = tf.transform_points(self.vertices, to_2D)
 
         # Z values of vertices which are referenced
         heights = flat[referenced][:, 2]
         # points are not on a plane because Z varies
-        if heights.ptp() > tol.planar:
+        if np.ptp(heights) > tol.planar:
             # since Z is inconsistent set height to zero
             height = 0.0
             if check:
                 raise ValueError("points are not flat!")
         else:
             # if the points were planar store the height
             height = heights.mean()
```

### Comparing `trimesh-4.3.2/trimesh/path/polygons.py` & `trimesh-4.4.0/trimesh/path/polygons.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,15 +390,15 @@
       on the polygon's medial axis
     vertices : (m, 2) float
       Vertex positions in space
     """
     # a circle will have a single point medial axis
     if len(polygon.interiors) == 0:
         # what is the approximate scale of the polygon
-        scale = np.reshape(polygon.bounds, (2, 2)).ptp(axis=0).max()
+        scale = np.ptp(np.reshape(polygon.bounds, (2, 2)), axis=0).max()
         # a (center, radius, error) tuple
         fit = fit_circle_check(polygon.exterior.coords, scale=scale)
         # is this polygon in fact a circle
         if fit is not None:
             # return an edge that has the center as the midpoint
             epsilon = np.clip(fit["radius"] / 500, 1e-5, np.inf)
             vertices = np.array(
@@ -409,15 +409,15 @@
             edges = np.array([[0, 1]], dtype=np.int64)
             return edges, vertices
 
     from scipy.spatial import Voronoi
     from shapely import vectorized
 
     if resolution is None:
-        resolution = np.reshape(polygon.bounds, (2, 2)).ptp(axis=0).max() / 100
+        resolution = np.ptp(np.reshape(polygon.bounds, (2, 2)), axis=0).max() / 100
 
     # get evenly spaced points on the polygons boundaries
     samples = resample_boundaries(polygon=polygon, resolution=resolution, clip=clip)
     # stack the boundary into a (m,2) float array
     samples = stack_boundaries(samples)
     # create the voronoi diagram on 2D points
     voronoi = Voronoi(samples)
@@ -438,15 +438,15 @@
     # mask voronoi vertices
     vertices = voronoi.vertices[contained]
     # re-index edges
     edges_final = mask[edges]
 
     if tol.strict:
         # make sure we didn't screw up indexes
-        assert (vertices[edges_final] - voronoi.vertices[edges]).ptp() < 1e-5
+        assert np.ptp(vertices[edges_final] - voronoi.vertices[edges]) < 1e-5
 
     return edges_final, vertices
 
 
 def identifier(polygon: Polygon) -> NDArray[float64]:
     """
     Return a vector containing values representative of
@@ -515,15 +515,15 @@
       Source geometry
 
     Returns
     ------------
     scale : float
       Length of AABB diagonal
     """
-    extents = np.reshape(polygon.bounds, (2, 2)).ptp(axis=0)
+    extents = np.ptp(np.reshape(polygon.bounds, (2, 2)), axis=0)
     scale = (extents**2).sum() ** 0.5
 
     return scale
 
 
 def paths_to_polygons(paths, scale=None):
     """
@@ -585,15 +585,15 @@
       where n <= count
     """
     # do batch point-in-polygon queries
     from shapely import vectorized
 
     # get size of bounding box
     bounds = np.reshape(polygon.bounds, (2, 2))
-    extents = bounds.ptp(axis=0)
+    extents = np.ptp(bounds, axis=0)
 
     # how many points to check per loop iteration
     per_loop = int(count * factor)
 
     # start with some rejection sampling
     points = bounds[0] + extents * np.random.random((per_loop, 2))
     # do the point in polygon test and append resulting hits
@@ -659,15 +659,15 @@
         basic = basic.geoms[np.argmax([i.area for i in basic.geoms])]
 
     # check perimeter of result against original perimeter
     if basic.is_valid and np.isclose(basic.length, polygon.length, rtol=rtol):
         return basic
 
     if scale is None:
-        distance = 0.002 * np.reshape(polygon.bounds, (2, 2)).ptp(axis=0).mean()
+        distance = 0.002 * np.ptp(np.reshape(polygon.bounds, (2, 2)), axis=0).mean()
     else:
         distance = 0.002 * scale
 
     # if there are no interiors, we can work with just the exterior
     # ring, which is often more reliable
     if len(polygon.interiors) == 0:
         # try buffering the exterior of the polygon
@@ -830,15 +830,15 @@
 
     padding = 0.0
     if apad is not None:
         # set padding by absolute value
         padding += float(apad)
     if rpad is not None:
         # get the 2D scale as the longest side of the AABB
-        scale = vertices_2D.ptp(axis=0).max()
+        scale = np.ptp(vertices_2D, axis=0).max()
         # apply the scale-relative padding
         padding += float(rpad) * scale
 
     # some types of errors will lead to a bajillion disconnected
     # regions and the union will take forever to fail
     # so exit here early
     if len(polygons) > max_regions:
```

### Comparing `trimesh-4.3.2/trimesh/path/raster.py` & `trimesh-4.4.0/trimesh/path/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     # check inputs
     pitch = np.asanyarray(pitch, dtype=np.float64)
     origin = np.asanyarray(origin, dtype=np.float64)
 
     # if resolution is None make it larger than path
     if resolution is None:
-        span = np.vstack((path.bounds, origin)).ptp(axis=0)
+        span = np.ptp(np.vstack((path.bounds, origin)), axis=0)
         resolution = np.ceil(span / pitch) + 2
     # get resolution as a (2,) int tuple
     resolution = np.asanyarray(resolution, dtype=np.int64)
     resolution = tuple(resolution.tolist())
 
     # convert all discrete paths to pixel space
     discrete = [((i - origin) / pitch).round().astype(np.int64) for i in path.discrete]
```

### Comparing `trimesh-4.3.2/trimesh/path/repair.py` & `trimesh-4.4.0/trimesh/path/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/segments.py` & `trimesh-4.4.0/trimesh/path/segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/simplify.py` & `trimesh-4.4.0/trimesh/path/simplify.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     scale = float(scale)
 
     # can only be a circle if the first and last point are the
     # same (AKA is a closed path)
     if np.linalg.norm(points[0] - points[-1]) > tol.merge:
         return None
 
-    box = points.ptp(axis=0)
+    box = np.ptp(points, axis=0)
     # the bounding box size of the points
     # check aspect ratio as an early exit if the path is not a circle
     aspect = np.divide(*box)
     if np.abs(aspect - 1.0) > tol.aspect_frac:
         return None
 
     # fit a circle with tolerance checks
```

### Comparing `trimesh-4.3.2/trimesh/path/traversal.py` & `trimesh-4.4.0/trimesh/path/traversal.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/path/util.py` & `trimesh-4.4.0/trimesh/path/util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/permutate.py` & `trimesh-4.4.0/trimesh/permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/points.py` & `trimesh-4.4.0/trimesh/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,15 +554,15 @@
         The size of the axis aligned bounds
 
         Returns
         ------------
         extents : (3,) float
           Edge length of axis aligned bounding box
         """
-        return self.bounds.ptp(axis=0)
+        return np.ptp(self.bounds, axis=0)
 
     @property
     def centroid(self):
         """
         The mean vertex position
 
         Returns
```

### Comparing `trimesh-4.3.2/trimesh/poses.py` & `trimesh-4.4.0/trimesh/poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/primitives.py` & `trimesh-4.4.0/trimesh/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -720,15 +720,15 @@
                 raise ValueError(
                     "if `bounds` is passed `extents` and `transform` must not be!"
                 )
             bounds = np.array(bounds, dtype=np.float64)
             if bounds.shape != (2, 3):
                 raise ValueError("`bounds` must be (2, 3) float")
             # create extents from AABB
-            extents = bounds.ptp(axis=0)
+            extents = np.ptp(bounds, axis=0)
             # translate to the center of the box
             transform = np.eye(4)
             transform[:3, 3] = bounds[0] + extents / 2.0
 
         self.primitive = PrimitiveAttributes(
             self,
             defaults=defaults,
```

### Comparing `trimesh-4.3.2/trimesh/proximity.py` & `trimesh-4.4.0/trimesh/proximity.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     # the first candidate is the best result for unambiguous cases
     result_close = query_close[idxs[:, 0]]
     result_tid = two_candidates[:, 0]
     result_distance = two_dists[:, 0]
 
     # however: same closest point on two different faces
     # find the best one and correct triangle ids if necessary
-    check_distance = two_dists.ptp(axis=1) < tol.merge
+    check_distance = np.ptp(two_dists, axis=1) < tol.merge
     check_magnitude = np.all(np.abs(two_dists) > tol.merge, axis=1)
 
     # mask results where corrections may be apply
     c_mask = np.bitwise_and(check_distance, check_magnitude)
 
     # get two face normals for the candidate points
     normals = mesh.face_normals[two_candidates[c_mask]]
```

### Comparing `trimesh-4.3.2/trimesh/ray/ray_pyembree.py` & `trimesh-4.4.0/trimesh/ray/ray_pyembree.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/ray/ray_triangle.py` & `trimesh-4.4.0/trimesh/ray/ray_triangle.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/ray/ray_util.py` & `trimesh-4.4.0/trimesh/ray/ray_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/registration.py` & `trimesh-4.4.0/trimesh/registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/remesh.py` & `trimesh-4.4.0/trimesh/remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/rendering.py` & `trimesh-4.4.0/trimesh/rendering.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/repair.py` & `trimesh-4.4.0/trimesh/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resolvers.py` & `trimesh-4.4.0/trimesh/resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/__init__.py` & `trimesh-4.4.0/trimesh/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/creation.json` & `trimesh-4.4.0/trimesh/resources/creation.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/gltf2.schema.zip` & `trimesh-4.4.0/trimesh/resources/schema/gltf2.schema.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/primitive/box.schema.json` & `trimesh-4.4.0/trimesh/resources/schema/primitive/box.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/primitive/capsule.schema.json` & `trimesh-4.4.0/trimesh/resources/schema/primitive/capsule.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/primitive/cylinder.schema.json` & `trimesh-4.4.0/trimesh/resources/schema/primitive/cylinder.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/primitive/extrusion.schema.json` & `trimesh-4.4.0/trimesh/resources/schema/primitive/extrusion.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/primitive/scenegraph.schema.json` & `trimesh-4.4.0/trimesh/resources/schema/primitive/scenegraph.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/primitive/sphere.schema.json` & `trimesh-4.4.0/trimesh/resources/schema/primitive/sphere.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/primitive/trimesh.schema.json` & `trimesh-4.4.0/trimesh/resources/schema/primitive/trimesh.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/schema/urdf.xsd` & `trimesh-4.4.0/trimesh/resources/schema/urdf.xsd`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/templates/blender_boolean.py.tmpl` & `trimesh-4.4.0/trimesh/resources/templates/blender_boolean.py.tmpl`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/templates/blender_unwrap.py.template` & `trimesh-4.4.0/trimesh/resources/templates/blender_unwrap.py.template`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/templates/dxf.json` & `trimesh-4.4.0/trimesh/resources/templates/dxf.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/templates/viewer.zip` & `trimesh-4.4.0/trimesh/resources/templates/viewer.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/resources/units_to_inches.json` & `trimesh-4.4.0/trimesh/resources/units_to_inches.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/sample.py` & `trimesh-4.4.0/trimesh/sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/scene/cameras.py` & `trimesh-4.4.0/trimesh/scene/cameras.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
     # Transform points to camera frame (just use the rotation part)
     rinv = rotation[:3, :3].T
     points_c = rinv.dot(points.T).T
 
     if center is None:
         # Find the center of the points' AABB in camera frame
-        center_c = points_c.min(axis=0) + 0.5 * points_c.ptp(axis=0)
+        center_c = points_c.min(axis=0) + 0.5 * np.ptp(points_c, axis=0)
     else:
         # Transform center to camera frame
         center_c = rinv.dot(center)
 
     # Re-center the points around the camera-frame origin
     points_c -= center_c
```

### Comparing `trimesh-4.3.2/trimesh/scene/lighting.py` & `trimesh-4.4.0/trimesh/scene/lighting.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/scene/scene.py` & `trimesh-4.4.0/trimesh/scene/scene.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/scene/transforms.py` & `trimesh-4.4.0/trimesh/scene/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/schemas.py` & `trimesh-4.4.0/trimesh/schemas.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/smoothing.py` & `trimesh-4.4.0/trimesh/smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/transformations.py` & `trimesh-4.4.0/trimesh/transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
 def identity_matrix():
     """Return 4x4 identity/unit matrix.
 
     >>> I = identity_matrix()
     >>> np.allclose(I, np.dot(I, I))
     True
-    >>> np.sum(I), np.trace(I)
+    >>> float(np.sum(I)), float(np.trace(I))
     (4.0, 4.0)
     >>> np.allclose(I, np.identity(4))
     True
 
     """
     return np.identity(4)
 
@@ -251,15 +251,15 @@
 
     >>> v0 = np.random.random(3) - 0.5
     >>> v1 = translation_from_matrix(translation_matrix(v0))
     >>> np.allclose(v0, v1)
     True
 
     """
-    return np.array(matrix, copy=False)[:3, 3].copy()
+    return np.asarray(matrix)[:3, 3].copy()
 
 
 def reflection_matrix(point, normal):
     """Return matrix to mirror at plane defined by point and normal vector.
 
     >>> v0 = np.random.random(4) - 0.5
     >>> v0[3] = 1.
@@ -292,15 +292,15 @@
     >>> M0 = reflection_matrix(v0, v1)
     >>> point, normal = reflection_from_matrix(M0)
     >>> M1 = reflection_matrix(point, normal)
     >>> is_same_transform(M0, M1)
     True
 
     """
-    M = np.array(matrix, dtype=np.float64, copy=False)
+    M = np.asarray(matrix, dtype=np.float64)
     # normal: unit eigenvector corresponding to eigenvalue -1
     w, V = np.linalg.eig(M[:3, :3])
     i = np.where(abs(np.real(w) + 1.0) < 1e-8)[0]
     if not len(i):
         raise ValueError("no unit eigenvector corresponding to eigenvalue -1")
     normal = np.real(V[:, i[0]]).squeeze()
     # point: any unit eigenvector corresponding to eigenvalue 1
@@ -380,15 +380,15 @@
             [direction[2], 0.0, -direction[0]],
             [-direction[1], direction[0], 0.0],
         ]
     )
 
     # if point is specified, rotation is not around origin
     if point is not None:
-        point = np.array(point[:3], dtype=np.float64, copy=False)
+        point = np.asarray(point[:3], dtype=np.float64)
         M[:3, 3] = point - np.dot(M[:3, :3], point)
 
     # return symbolic angles as sympy Matrix objects
     if symbolic:
         return sp.Matrix(M)
 
     return M
@@ -403,15 +403,15 @@
     >>> R0 = rotation_matrix(angle, direc, point)
     >>> angle, direc, point = rotation_from_matrix(R0)
     >>> R1 = rotation_matrix(angle, direc, point)
     >>> is_same_transform(R0, R1)
     True
 
     """
-    R = np.array(matrix, dtype=np.float64, copy=False)
+    R = np.asarray(matrix, dtype=np.float64)
     R33 = R[:3, :3]
     # direction: unit eigenvector of R33 corresponding to eigenvalue of 1
     w, W = np.linalg.eig(R33.T)
     i = np.where(abs(np.real(w) - 1.0) < 1e-8)[0]
     if not len(i):
         raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
     direction = np.real(W[:, i[-1]]).squeeze()
@@ -482,15 +482,15 @@
     >>> S0 = scale_matrix(factor, origin, direct)
     >>> factor, origin, direction = scale_from_matrix(S0)
     >>> S1 = scale_matrix(factor, origin, direction)
     >>> is_same_transform(S0, S1)
     True
 
     """
-    M = np.array(matrix, dtype=np.float64, copy=False)
+    M = np.asarray(matrix, dtype=np.float64)
     M33 = M[:3, :3]
     factor = np.trace(M33) - 2.0
     try:
         # direction: unit eigenvector corresponding to eigenvalue factor
         w, V = np.linalg.eig(M33)
         i = np.where(abs(np.real(w) - factor) < 1e-8)[0][0]
         direction = np.real(V[:, i]).squeeze()
@@ -537,32 +537,32 @@
     >>> np.allclose(v1[1], v0[1])
     True
     >>> np.allclose(v1[0], 3-v1[1])
     True
 
     """
     M = np.identity(4)
-    point = np.array(point[:3], dtype=np.float64, copy=False)
+    point = np.asarray(point[:3], dtype=np.float64)
     normal = unit_vector(normal[:3])
     if perspective is not None:
         # perspective projection
-        perspective = np.array(perspective[:3], dtype=np.float64, copy=False)
+        perspective = np.asarray(perspective[:3], dtype=np.float64)
         M[0, 0] = M[1, 1] = M[2, 2] = np.dot(perspective - point, normal)
         M[:3, :3] -= np.outer(perspective, normal)
         if pseudo:
             # preserve relative depth
             M[:3, :3] -= np.outer(normal, normal)
             M[:3, 3] = np.dot(point, normal) * (perspective + normal)
         else:
             M[:3, 3] = np.dot(point, normal) * perspective
         M[3, :3] = -normal
         M[3, 3] = np.dot(perspective, normal)
     elif direction is not None:
         # parallel projection
-        direction = np.array(direction[:3], dtype=np.float64, copy=False)
+        direction = np.asarray(direction[:3], dtype=np.float64)
         scale = np.dot(direction, normal)
         M[:3, :3] -= np.outer(direction, normal) / scale
         M[:3, 3] = direction * (np.dot(point, normal) / scale)
     else:
         # orthogonal projection
         M[:3, :3] -= np.outer(normal, normal)
         M[:3, 3] = np.dot(point, normal) * normal
@@ -597,15 +597,15 @@
     >>> P0 = projection_matrix(point, normal, perspective=persp, pseudo=True)
     >>> result = projection_from_matrix(P0, pseudo=True)
     >>> P1 = projection_matrix(*result)
     >>> is_same_transform(P0, P1)
     True
 
     """
-    M = np.array(matrix, dtype=np.float64, copy=False)
+    M = np.asarray(matrix, dtype=np.float64)
     M33 = M[:3, :3]
     w, V = np.linalg.eig(M)
     i = np.where(abs(np.real(w) - 1.0) < 1e-8)[0]
     if not pseudo and len(i):
         # point: any eigenvector corresponding to eigenvalue 1
         point = np.real(V[:, i[-1]]).squeeze()
         point /= point[3]
@@ -742,15 +742,15 @@
     >>> S0 = shear_matrix(angle, direct, point, normal)
     >>> angle, direct, point, normal = shear_from_matrix(S0)
     >>> S1 = shear_matrix(angle, direct, point, normal)
     >>> is_same_transform(S0, S1)
     True
 
     """
-    M = np.array(matrix, dtype=np.float64, copy=False)
+    M = np.asarray(matrix, dtype=np.float64)
     M33 = M[:3, :3]
     # normal: cross independent eigenvectors corresponding to the eigenvalue 1
     w, V = np.linalg.eig(M33)
 
     i = np.where(abs(np.real(w) - 1.0) < 1e-4)[0]
     if len(i) < 2:
         raise ValueError(f"no two linear independent eigenvectors found {w}")
@@ -797,24 +797,24 @@
     >>> T0 = translation_matrix([1, 2, 3])
     >>> scale, shear, angles, trans, persp = decompose_matrix(T0)
     >>> T1 = translation_matrix(trans)
     >>> np.allclose(T0, T1)
     True
     >>> S = scale_matrix(0.123)
     >>> scale, shear, angles, trans, persp = decompose_matrix(S)
-    >>> scale[0]
-    0.123
+    >>> bool(np.isclose(scale[0], 0.123))
+    True
     >>> R0 = euler_matrix(1, 2, 3)
     >>> scale, shear, angles, trans, persp = decompose_matrix(R0)
     >>> R1 = euler_matrix(*angles)
     >>> np.allclose(R0, R1)
     True
 
     """
-    M = np.array(matrix, dtype=np.float64, copy=True).T
+    M = np.array(matrix, dtype=np.float64).T
     if abs(M[3, 3]) < _EPS:
         raise ValueError("M[3, 3] is zero")
     M /= M[3, 3]
     P = M.copy()
     P[:, 3] = 0.0, 0.0, 0.0, 1.0
     if not np.linalg.det(P):
         raise ValueError("matrix is singular")
@@ -978,16 +978,16 @@
     >>> v0[:3] += np.random.normal(0, 1e-8, 300).reshape(3, -1)
     >>> M = affine_matrix_from_points(v0[:3], v1[:3])
     >>> check = np.allclose(v1, np.dot(M, v0))
 
     More examples in superimposition_matrix()
 
     """
-    v0 = np.array(v0, dtype=np.float64, copy=True)
-    v1 = np.array(v1, dtype=np.float64, copy=True)
+    v0 = np.array(v0, dtype=np.float64)
+    v1 = np.array(v1, dtype=np.float64)
 
     ndims = v0.shape[0]
     if ndims < 2 or v0.shape[1] < ndims or v0.shape != v1.shape:
         raise ValueError("input arrays are of wrong shape or type")
 
     # move centroids to origin
     t0 = -np.mean(v0, axis=1)
@@ -1093,16 +1093,16 @@
     >>> v = np.empty((4, 100, 3))
     >>> v[:, :, 0] = v0
     >>> M = superimposition_matrix(v0, v1, scale=True, usesvd=False)
     >>> np.allclose(v1, np.dot(M, v[:, :, 0]))
     True
 
     """
-    v0 = np.array(v0, dtype=np.float64, copy=False)[:3]
-    v1 = np.array(v1, dtype=np.float64, copy=False)[:3]
+    v0 = np.asarray(v0, dtype=np.float64)[:3]
+    v1 = np.asarray(v1, dtype=np.float64)[:3]
     return affine_matrix_from_points(v0, v1, shear=False, scale=scale, usesvd=usesvd)
 
 
 def euler_matrix(ai, aj, ak, axes="sxyz"):
     """Return homogeneous rotation matrix from Euler angles and axis sequence.
 
     ai, aj, ak : Euler's roll, pitch and yaw angles
@@ -1199,15 +1199,15 @@
         _TUPLE2AXES[axes]  # validation
         firstaxis, parity, repetition, frame = axes
 
     i = firstaxis
     j = _NEXT_AXIS[i + parity]
     k = _NEXT_AXIS[i - parity + 1]
 
-    M = np.array(matrix, dtype=np.float64, copy=False)[:3, :3]
+    M = np.asarray(matrix, dtype=np.float64)[:3, :3]
     if repetition:
         sy = np.sqrt(M[i, j] * M[i, j] + M[i, k] * M[i, k])
         if sy > _EPS:
             ax = np.arctan2(M[i, j], M[i, k])
             ay = np.arctan2(sy, M[i, i])
             az = np.arctan2(M[j, i], -M[k, i])
         else:
@@ -1331,15 +1331,15 @@
     True
     >>> M = quaternion_matrix([[1, 0, 0, 0],[0, 1, 0, 0]])
     >>> np.allclose(M, np.array([np.identity(4), np.diag([1, -1, -1, 1])]))
     True
 
 
     """
-    q = np.array(quaternion, dtype=np.float64, copy=True).reshape((-1, 4))
+    q = np.array(quaternion, dtype=np.float64).reshape((-1, 4))
     n = np.einsum("ij,ij->i", q, q)
     # how many entries do we have
     num_qs = len(n)
     identities = n < _EPS
     q[~identities, :] *= np.sqrt(2.0 / n[~identities, None])
     q = np.einsum("ij,ik->ikj", q, q)
 
@@ -1398,15 +1398,15 @@
     True
     >>> R = euler_matrix(0.0, 0.0, np.pi/2.0)
     >>> is_same_quaternion(quaternion_from_matrix(R, isprecise=False),
     ...                    quaternion_from_matrix(R, isprecise=True))
     True
 
     """
-    M = np.array(matrix, dtype=np.float64, copy=False)[:4, :4]
+    M = np.asarray(matrix, dtype=np.float64)[:4, :4]
     if isprecise:
         q = np.empty((4,))
         t = np.trace(M)
         if t > M[3, 3]:
             q[0] = t
             q[3] = M[1, 0] - M[0, 1]
             q[2] = M[0, 2] - M[2, 0]
@@ -1478,29 +1478,29 @@
 
     >>> q0 = random_quaternion()
     >>> q1 = quaternion_conjugate(q0)
     >>> q1[0] == q0[0] and all(q1[1:] == -q0[1:])
     True
 
     """
-    q = np.array(quaternion, dtype=np.float64, copy=True)
+    q = np.array(quaternion, dtype=np.float64)
     np.negative(q[1:], q[1:])
     return q
 
 
 def quaternion_inverse(quaternion):
     """Return inverse of quaternion.
 
     >>> q0 = random_quaternion()
     >>> q1 = quaternion_inverse(q0)
     >>> np.allclose(quaternion_multiply(q0, q1), [1, 0, 0, 0])
     True
 
     """
-    q = np.array(quaternion, dtype=np.float64, copy=True)
+    q = np.array(quaternion, dtype=np.float64)
     np.negative(q[1:], q[1:])
     return q / np.dot(q, q)
 
 
 def quaternion_real(quaternion):
     """Return real part of quaternion.
 
@@ -1514,15 +1514,15 @@
 def quaternion_imag(quaternion):
     """Return imaginary part of quaternion.
 
     >>> quaternion_imag([3, 0, 1, 2])
     array([0., 1., 2.])
 
     """
-    return np.array(quaternion[1:4], dtype=np.float64, copy=True)
+    return np.array(quaternion[1:4], dtype=np.float64)
 
 
 def quaternion_slerp(quat0, quat1, fraction, spin=0, shortestpath=True):
     """Return spherical linear interpolation between two quaternions.
 
     >>> q0 = random_quaternion()
     >>> q1 = random_quaternion()
@@ -1739,31 +1739,31 @@
         return np.array([v0 / n, v1 / n, 0.0])
     else:
         return np.array([v0, v1, np.sqrt(1.0 - n)])
 
 
 def arcball_constrain_to_axis(point, axis):
     """Return sphere point perpendicular to axis."""
-    v = np.array(point, dtype=np.float64, copy=True)
-    a = np.array(axis, dtype=np.float64, copy=True)
+    v = np.array(point, dtype=np.float64)
+    a = np.array(axis, dtype=np.float64)
     v -= a * np.dot(a, v)  # on plane
     n = vector_norm(v)
     if n > _EPS:
         if v[2] < 0.0:
             np.negative(v, v)
         v /= n
         return v
     if a[2] == 1.0:
         return np.array([1.0, 0.0, 0.0])
     return unit_vector([-a[1], a[0], 0.0])
 
 
 def arcball_nearest_axis(point, axes):
     """Return axis, which arc is nearest to point."""
-    point = np.array(point, dtype=np.float64, copy=False)
+    point = np.asarray(point, dtype=np.float64)
     nearest = None
     mx = -1.0
     for axis in axes:
         t = np.dot(arcball_constrain_to_axis(point, axis), point)
         if t > mx:
             nearest = axis
             mx = t
@@ -1822,21 +1822,21 @@
     >>> np.allclose(n, np.sqrt(np.sum(v*v, axis=1)))
     True
     >>> v = np.random.rand(5, 4, 3)
     >>> n = np.empty((5, 3))
     >>> vector_norm(v, axis=1, out=n)
     >>> np.allclose(n, np.sqrt(np.sum(v*v, axis=1)))
     True
-    >>> vector_norm([])
+    >>> float(vector_norm([]))
     0.0
-    >>> vector_norm([1])
+    >>> float(vector_norm([1]))
     1.0
 
     """
-    data = np.array(data, dtype=np.float64, copy=True)
+    data = np.array(data, dtype=np.float64)
     if out is None:
         if data.ndim == 1:
             return np.sqrt(np.dot(data, data))
         data *= data
         out = np.atleast_1d(np.sum(data, axis=axis))
         np.sqrt(out, out)
         return out
@@ -1864,45 +1864,45 @@
     True
     >>> v1 = np.empty((5, 4, 3))
     >>> unit_vector(v0, axis=1, out=v1)
     >>> np.allclose(v1, v2)
     True
     >>> list(unit_vector([]))
     []
-    >>> list(unit_vector([1]))
+    >>> [float(i) for i in unit_vector([1])]
     [1.0]
 
     """
     if out is None:
-        data = np.array(data, dtype=np.float64, copy=True)
+        data = np.array(data, dtype=np.float64)
         if data.ndim == 1:
             data /= np.sqrt(np.dot(data, data))
             return data
     else:
         if out is not data:
-            out[:] = np.array(data, copy=False)
+            out[:] = np.asarray(data)
         data = out
     length = np.atleast_1d(np.sum(data * data, axis))
     np.sqrt(length, length)
     if axis is not None:
         length = np.expand_dims(length, axis)
     data /= length
     if out is None:
         return data
 
 
 def random_vector(size):
     """Return array of random doubles in the half-open interval [0.0, 1.0).
 
     >>> v = random_vector(10000)
-    >>> np.all(v >= 0) and np.all(v < 1)
+    >>> bool(np.all(v >= 0) and np.all(v < 1))
     True
     >>> v0 = random_vector(10)
     >>> v1 = random_vector(10)
-    >>> np.any(v0 == v1)
+    >>> bool(np.any(v0 == v1))
     False
 
     """
     return np.random.random(size)
 
 
 def vector_product(v0, v1, axis=0):
@@ -1946,16 +1946,16 @@
     >>> v0 = [[2, 0, 0], [2, 0, 0], [0, 2, 0], [2, 0, 0]]
     >>> v1 = [[0, 3, 0], [0, 0, 3], [0, 0, 3], [3, 3, 3]]
     >>> a = angle_between_vectors(v0, v1, axis=1)
     >>> np.allclose(a, [1.5708, 1.5708, 1.5708, 0.95532])
     True
 
     """
-    v0 = np.array(v0, dtype=np.float64, copy=False)
-    v1 = np.array(v1, dtype=np.float64, copy=False)
+    v0 = np.asarray(v0, dtype=np.float64)
+    v1 = np.asarray(v1, dtype=np.float64)
     dot = np.sum(v0 * v1, axis=axis)
     dot /= vector_norm(v0, axis=axis) * vector_norm(v1, axis=axis)
 
     # clip off floating point error to avoid `nan` in the arccos`
     dot = np.clip(dot, -1.0, 1.0)
     return np.arccos(dot if directed else np.fabs(dot))
 
@@ -1997,17 +1997,17 @@
 
     >>> is_same_transform(np.identity(4), np.identity(4))
     True
     >>> is_same_transform(np.identity(4), random_rotation_matrix())
     False
 
     """
-    matrix0 = np.array(matrix0, dtype=np.float64, copy=True)
+    matrix0 = np.array(matrix0, dtype=np.float64)
     matrix0 /= matrix0[3, 3]
-    matrix1 = np.array(matrix1, dtype=np.float64, copy=True)
+    matrix1 = np.array(matrix1, dtype=np.float64)
     matrix1 /= matrix1[3, 3]
     return np.allclose(matrix0, matrix1)
 
 
 def is_same_quaternion(q0, q1):
     """Return True if two quaternions are equal."""
     q0 = np.array(q0)
@@ -2247,21 +2247,21 @@
 
     matrix = np.asanyarray(matrix, dtype=np.float64)
 
     if matrix.shape != (4, 4):
         return False
 
     # make sure last row has no scaling
-    if (matrix[-1] - [0, 0, 0, 1]).ptp() > epsilon:
+    if np.ptp(matrix[-1] - [0, 0, 0, 1]) > epsilon:
         return False
 
     # check dot product of rotation against transpose
     check = np.dot(matrix[:3, :3], matrix[:3, :3].T) - _IDENTITY[:3, :3]
 
-    return check.ptp() < epsilon
+    return np.ptp(check) < epsilon
 
 
 def scale_and_translate(scale=None, translate=None):
     """
     Optimized version of `compose_matrix` for just
     scaling then translating.
```

### Comparing `trimesh-4.3.2/trimesh/triangles.py` & `trimesh-4.4.0/trimesh/triangles.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,17 +331,15 @@
     Returns
     ----------
     aligned : (n,) bool
       Are normals aligned with triangles
     """
     triangles = np.asanyarray(triangles, dtype=np.float64)
     if not util.is_shape(triangles, (-1, 3, 3), allow_zeros=True):
-        raise ValueError(
-            f"triangles must have shape (n, 3, 3), got {triangles.shape!s}"
-        )
+        raise ValueError(f"triangles must have shape (n, 3, 3), got {triangles.shape!s}")
     normals_compare = np.asanyarray(normals_compare, dtype=np.float64)
 
     calculated, valid = normals(triangles)
     if normals_compare.shape == (3,):
         # single comparison vector case
         difference = np.dot(calculated, normals_compare)
     else:
```

### Comparing `trimesh-4.3.2/trimesh/typed.py` & `trimesh-4.4.0/trimesh/typed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from io import BytesIO, StringIO
 from pathlib import Path
 from sys import version_info
 from typing import (
     IO,
     Any,
     BinaryIO,
+    Mapping,
     Optional,
     TextIO,
     Union,
 )
 
 from numpy import float64, floating, int64, integer, unsignedinteger
 
@@ -54,8 +55,9 @@
     "Number",
     "Optional",
     "Sequence",
     "Stream",
     "Tuple",
     "float64",
     "int64",
+    "Mapping",
 ]
```

### Comparing `trimesh-4.3.2/trimesh/units.py` & `trimesh-4.4.0/trimesh/units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/util.py` & `trimesh-4.4.0/trimesh/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -2230,15 +2230,15 @@
       Acceptable distance between `a` and `b` to be "close"
 
     Returns
     -----------
     bool indicating if all elements are within `atol`.
     """
     #
-    return float((a - b).ptp()) < atol
+    return float(np.ptp(a - b)) < atol
 
 
 class FunctionRegistry(Mapping):
     """
     Non-overwritable mapping of string keys to functions.
 
     This allows external packages to register additional implementations
```

### Comparing `trimesh-4.3.2/trimesh/version.py` & `trimesh-4.4.0/trimesh/version.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/viewer/__init__.py` & `trimesh-4.4.0/trimesh/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/viewer/notebook.py` & `trimesh-4.4.0/trimesh/viewer/notebook.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/viewer/trackball.py` & `trimesh-4.4.0/trimesh/viewer/trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/viewer/widget.py` & `trimesh-4.4.0/trimesh/viewer/widget.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/viewer/windowed.py` & `trimesh-4.4.0/trimesh/viewer/windowed.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,17 +558,17 @@
                 # create a grid marker
                 from ..path.creation import grid
 
                 bounds = self.scene.bounds
                 center = bounds.mean(axis=0)
                 # set the grid to the lowest Z position
                 # also offset by the scale to avoid interference
-                center[2] = bounds[0][2] - (bounds[:, 2].ptp() / 100)
+                center[2] = bounds[0][2] - (np.ptp(bounds[:, 2]) / 100)
                 # choose the side length by maximum XY length
-                side = bounds.ptp(axis=0)[:2].max()
+                side = np.ptp(bounds, axis=0)[:2].max()
                 # create an axis marker sized relative to the scene
                 grid_mesh = grid(side=side, count=4, transform=translation_matrix(center))
                 # convert the path to vertexlist args
                 args = rendering.convert_to_vertexlist(grid_mesh)
                 # create ordered args for a vertex list
                 self._grid = self.batch.add_indexed(*args)
             except BaseException:
```

### Comparing `trimesh-4.3.2/trimesh/visual/__init__.py` & `trimesh-4.4.0/trimesh/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/visual/base.py` & `trimesh-4.4.0/trimesh/visual/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/visual/color.py` & `trimesh-4.4.0/trimesh/visual/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,15 +829,15 @@
         from matplotlib.pyplot import get_cmap
 
         cmap = get_cmap(color_map)
 
     # make input always float
     values = np.asanyarray(values, dtype=np.float64).ravel()
     # scale values to 0.0 - 1.0 and get colors
-    colors = cmap((values - values.min()) / values.ptp())
+    colors = cmap((values - values.min()) / np.ptp(values))
     # convert to 0-255 RGBA
     rgba = to_rgba(colors, dtype=dtype)
 
     return rgba
 
 
 def uv_to_color(uv, image):
```

### Comparing `trimesh-4.3.2/trimesh/visual/gloss.py` & `trimesh-4.4.0/trimesh/visual/gloss.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/visual/material.py` & `trimesh-4.4.0/trimesh/visual/material.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/visual/objects.py` & `trimesh-4.4.0/trimesh/visual/objects.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/visual/texture.py` & `trimesh-4.4.0/trimesh/visual/texture.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh/voxel/base.py` & `trimesh-4.4.0/trimesh/voxel/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,15 @@
     @encoding.setter
     def encoding(self, encoding):
         if isinstance(encoding, np.ndarray):
             encoding = DenseEncoding(encoding)
         elif not isinstance(encoding, Encoding):
             raise ValueError(f"encoding must be an Encoding, got {encoding!s}")
         if len(encoding.shape) != 3:
-            raise ValueError(
-                f"encoding must be rank 3, got shape {encoding.shape!s}"
-            )
+            raise ValueError(f"encoding must be rank 3, got shape {encoding.shape!s}")
         if encoding.dtype != bool:
             raise ValueError(f"encoding must be binary, got {encoding.dtype}")
         self._data["encoding"] = encoding
 
     @property
     def transform(self):
         """4x4 homogeneous transformation matrix."""
```

### Comparing `trimesh-4.3.2/trimesh/voxel/creation.py` & `trimesh-4.4.0/trimesh/voxel/creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,19 +140,16 @@
         regions, n = ndimage.label(~voxels)
         distance = ndimage.distance_transform_cdt(~voxels)
         representatives = [
             np.unravel_index((distance * (regions == i)).argmax(), distance.shape)
             for i in range(1, n + 1)
         ]
         contains = mesh.contains(np.asarray(representatives) * pitch + local_origin)
-
         where = np.where(contains)[0] + 1
-        # use in1d vs isin for older numpy versions
-        internal = np.in1d(regions.flatten(), where).reshape(regions.shape)
-
+        internal = np.isin(regions.flatten(), where).reshape(regions.shape)
         voxels = np.logical_or(voxels, internal)
 
     return base.VoxelGrid(voxels, tr.translation_matrix(local_origin))
 
 
 @log_time
 def voxelize_ray(mesh, pitch, per_cell=None):
```

### Comparing `trimesh-4.3.2/trimesh/voxel/encoding.py` & `trimesh-4.4.0/trimesh/voxel/encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -811,17 +811,15 @@
     Lazily transposed encoding
 
     Dense equivalent is `np.transpose`
     """
 
     def __init__(self, base_encoding, perm):
         if not isinstance(base_encoding, Encoding):
-            raise ValueError(
-                f"base_encoding must be an Encoding, got {base_encoding!s}"
-            )
+            raise ValueError(f"base_encoding must be an Encoding, got {base_encoding!s}")
         if len(base_encoding.shape) != len(perm):
             raise ValueError(
                 "base_encoding has %d ndims - cannot transpose with perm %s"
                 % (base_encoding.ndims, str(perm))
             )
         super().__init__(base_encoding)
         perm = np.array(perm, dtype=np.int64)
```

### Comparing `trimesh-4.3.2/trimesh/voxel/morphology.py` & `trimesh-4.4.0/trimesh/voxel/morphology.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,27 @@
 
 def _dense(encoding, rank=None):
     if isinstance(encoding, np.ndarray):
         dense = encoding
     elif isinstance(encoding, enc.Encoding):
         dense = encoding.dense
     else:
-        raise ValueError(
-            f"encoding must be np.ndarray or Encoding, got {encoding!s}"
-        )
+        raise ValueError(f"encoding must be np.ndarray or Encoding, got {encoding!s}")
     if rank:
         _assert_rank(dense, rank)
     return dense
 
 
 def _sparse_indices(encoding, rank=None):
     if isinstance(encoding, np.ndarray):
         sparse_indices = encoding
     elif isinstance(encoding, enc.Encoding):
         sparse_indices = encoding.sparse_indices
     else:
-        raise ValueError(
-            f"encoding must be np.ndarray or Encoding, got {encoding!s}"
-        )
+        raise ValueError(f"encoding must be np.ndarray or Encoding, got {encoding!s}")
 
     _assert_sparse_rank(sparse_indices, 3)
     return sparse_indices
 
 
 def _assert_rank(value, rank):
     if len(value.shape) != rank:
```

### Comparing `trimesh-4.3.2/trimesh/voxel/ops.py` & `trimesh-4.4.0/trimesh/voxel/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     # 3D sparse arrays, using wrapped scipy.sparse
     # pip install sparse
     import sparse
 
     # find the bounding box of both arrays
     extrema = np.array([a.min(axis=0), a.max(axis=0), b.min(axis=0), b.max(axis=0)])
     origin = extrema.min(axis=0) - 1
-    size = tuple(extrema.ptp(axis=0) + 2)
+    size = tuple(np.ptp(extrema, axis=0) + 2)
 
     # put nearby voxel arrays into same shape sparse array
     sp_a = sparse.COO((a - origin).T, data=np.ones(len(a), dtype=bool), shape=size)
     sp_b = sparse.COO((b - origin).T, data=np.ones(len(b), dtype=bool), shape=size)
 
     # apply the logical operation
     # get a sparse matrix out
```

### Comparing `trimesh-4.3.2/trimesh/voxel/runlength.py` & `trimesh-4.4.0/trimesh/voxel/runlength.py`

 * *Files 1% similar despite different names*

```diff
@@ -612,28 +612,28 @@
     indices = []
     values = []
     it = iter(rle_data)
     index = 0
     try:
         while True:
             value = next(it)
-            counts = next(it)
+            counts = int(next(it))
             end = index + counts
             if value:
                 indices.append(np.arange(index, end, dtype=np.int64))
                 values.append(np.repeat(value, counts))
             index = end
     except StopIteration:
         pass
     if len(indices) == 0:
         assert len(values) == 0
         return indices, values
 
     indices = np.concatenate(indices)
-    values = np.concatenate(values)
+    values = np.concatenate(values, dtype=rle_data.dtype)
     return indices, values
 
 
 def brle_to_sparse(brle_data, dtype=np.int64):
     ends = np.cumsum(brle_data)
     indices = [np.arange(s, e, dtype=dtype) for s, e in zip(ends[::2], ends[1::2])]
     return np.concatenate(indices)
```

### Comparing `trimesh-4.3.2/trimesh/voxel/transforms.py` & `trimesh-4.4.0/trimesh/voxel/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.2/trimesh.egg-info/PKG-INFO` & `trimesh-4.4.0/trimesh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.3.2
+Version: 4.4.0
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,23 +75,23 @@
 Requires-Dist: cascadio; extra == "recommend"
 Requires-Dist: manifold3d>=2.3.0; extra == "recommend"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: pyright; extra == "test"
 Requires-Dist: ezdxf; extra == "test"
-Requires-Dist: gmsh>=4.12.1; extra == "test"
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: pymeshlab; extra == "test"
 Requires-Dist: pyinstrument; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: pytest-beartype; python_version >= "3.10" and extra == "test"
+Provides-Extra: deprecated
+Requires-Dist: gmsh==4.12.2; extra == "deprecated"
 Provides-Extra: all
-Requires-Dist: trimesh[easy,recommend,test]; extra == "all"
+Requires-Dist: trimesh[deprecated,easy,recommend,test]; extra == "all"
 
 [![trimesh](https://trimesh.org/_static/images/logotype-a.svg)](http://trimesh.org)
 
 -----------
 [![Github Actions](https://github.com/mikedh/trimesh/workflows/Release%20Trimesh/badge.svg)](https://github.com/mikedh/trimesh/actions) [![codecov](https://codecov.io/gh/mikedh/trimesh/branch/main/graph/badge.svg?token=4PVRQXyl2h)](https://codecov.io/gh/mikedh/trimesh)  [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/trimesh/trimesh?label=docker&sort=semver)](https://hub.docker.com/r/trimesh/trimesh/tags) [![PyPI version](https://badge.fury.io/py/trimesh.svg)](https://badge.fury.io/py/trimesh)
```

### Comparing `trimesh-4.3.2/trimesh.egg-info/SOURCES.txt` & `trimesh-4.4.0/trimesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*


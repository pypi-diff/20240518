# Comparing `tmp/whitecanvas-0.2.6.tar.gz` & `tmp/whitecanvas-0.3.0.tar.gz`

## Comparing `whitecanvas-0.2.6.tar` & `whitecanvas-0.3.0.tar`

### file list

```diff
@@ -1,240 +1,268 @@
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/mkdocs.yml
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.github/workflows/test.yml
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/index.md
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/quick_start.md
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/_scripts/_hooks.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/_scripts/_screenshots.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/canvas.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/core.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/tools.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/types.md
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/basics.md
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/grid.md
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/index.md
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/inset_second.md
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/joint_grid.md
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/legend.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/namespaces.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/native_objects.md
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/aggregation.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/cat_cat.md
--rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/cat_num.md
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/index.md
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/num_num.md
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/stacking.md
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/canvas_events.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/index.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/layer_events.md
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/mouse_events.md
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/distribution.md
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/face_layers.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/index.md
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/layer_groups.md
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/lines.md
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/markers.md
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/mouse.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/texts.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/tools/index.md
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/tools/selection.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/boxplot_with_outliers.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/curve_fit.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/draw_with_mouse.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/fit_layer.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/heatmap_with_text.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/image_profile.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/integral.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/joint_grid.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/layer_clicked_event.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/line_with_error.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/line_with_spans.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/lines.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/markers_hover_text.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/markers_multicolor.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/markers_with_legend.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/plotly_in_qt.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/raincloud_plot.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/show_image_on_pick.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/stack_bars.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/superplot.py
--rw-r--r--   0        0        0    93685 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/curve_fit.png
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/heatmap.png
--rw-r--r--   0        0        0   205151 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/jointgrid.png
--rw-r--r--   0        0        0    45190 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/raincloud.png
--rw-r--r--   0        0        0    41392 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/superplot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/_utils.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_canvas.py
--rw-r--r--   0        0        0    11908 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_categorical.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_grouping.py
--rw-r--r--   0        0        0    12476 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_layers.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_logics.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_plt.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_theme.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_tools.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/__init__.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/_axis.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/_exceptions.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/_signal.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/animation.py
--rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/core.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/__init__.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_app.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_instance.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_not_implemented.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_window/__init__.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_window/_qt.py
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_window/_tk.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/__init__.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/_base.py
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/_labels.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/_legend.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/band.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/bars.py
--rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/canvas.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/image.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/line.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/markers.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/text.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/__init__.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_base.py
--rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_labels.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_legend.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/band.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/bars.py
--rw-r--r--   0        0        0    15742 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/canvas.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/image.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/line.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/markers.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/text.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/__init__.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/_base.py
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/canvas.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/layers.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/__init__.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/_base.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/_labels.py
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/_legend.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/band.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/bars.py
--rw-r--r--   0        0        0    13248 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/canvas.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/image.py
--rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/line.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/markers.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/text.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/__init__.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_base.py
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_labels.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_legend.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_qt_utils.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/band.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/bars.py
--rw-r--r--   0        0        0    15158 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/canvas.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/image.py
--rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/line.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/markers.py
--rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/text.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/_gridlines.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/_label.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/band.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/bars.py
--rw-r--r--   0        0        0    12258 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/canvas.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/image.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/line.py
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/markers.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/text.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/__init__.py
--rw-r--r--   0        0        0    69749 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_base.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_between.py
--rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_dims.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_fit.py
--rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_grid.py
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_imageref.py
--rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_joint.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_linker.py
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_namespaces.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_palette.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_stacked.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/layerlist.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/__init__.py
--rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_base.py
--rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_both_cat.py
--rw-r--r--   0        0        0    18971 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_feature_cat.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_joint_cat.py
--rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_one_cat.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_stacked_cat.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/__init__.py
--rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_base.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_legend.py
--rw-r--r--   0        0        0    36394 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_mixin.py
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_ndim.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_sizehint.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_text_utils.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/__init__.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/band.py
--rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/bars.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/errorbars.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/image.py
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/inf_curve.py
--rw-r--r--   0        0        0    23189 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/line.py
--rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/markers.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/rects.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/rug.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/spans.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/text.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/_cat_utils.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/_collections.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/_offsets.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/band_collection.py
--rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/boxplot.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/colorbar.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/graph.py
--rw-r--r--   0        0        0    25093 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/labeled.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_band.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_collection.py
--rw-r--r--   0        0        0    14529 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_fill.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_markers.py
--rw-r--r--   0        0        0    16196 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/marker_collection.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/stemplot.py
--rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/textinfo.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/__init__.py
--rw-r--r--   0        0        0    41141 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_box_like.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_dataframe.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_df_compat.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_jitter.py
--rw-r--r--   0        0        0    33317 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_marker_like.py
--rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_plans.py
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_shared.py
--rw-r--r--   0        0        0    14768 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_stackable.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/plot/__init__.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/plot/_canvases.py
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/plot/_methods.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/protocols/__init__.py
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/protocols/canvas_protocol.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/protocols/layer_protocols.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/theme/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/theme/_api.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/theme/_dataclasses.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/tools/__init__.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/tools/_polygon_utils.py
--rw-r--r--   0        0        0    24164 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/tools/_selection.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_alias.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_enums.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_mouse.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_tuples.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/__init__.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/collections.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/hist.py
--rw-r--r--   0        0        0    14353 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/kde.py
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/normalize.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/type_check.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/LICENSE
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/README.md
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/index.md
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/quick_start.md
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/_scripts/_hooks.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/_scripts/_screenshots.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/api/canvas.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/api/core.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/api/tools.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/api/types.md
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/basics.md
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/grid.md
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/index.md
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/inset_second.md
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/joint_grid.md
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/legend.md
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/namespaces.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/canvas/native_objects.md
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/categorical/aggregation.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/categorical/cat_cat.md
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/categorical/cat_num.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/categorical/index.md
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/categorical/num_num.md
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/categorical/stacking.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/events/canvas_events.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/events/index.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/events/layer_events.md
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/events/mouse_events.md
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/distribution.md
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/face_layers.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/index.md
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/layer_groups.md
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/lines.md
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/markers.md
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/mouse.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/layers/texts.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/tools/index.md
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/docs/tools/selection.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/boxplot_with_outliers.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/curve_fit.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/draw_with_mouse.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/fit_layer.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/heatmap_with_text.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/image_profile.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/integral.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/joint_grid.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/layer_clicked_event.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/line_with_error.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/line_with_spans.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/lines.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/markers_hover_text.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/markers_multicolor.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/markers_with_legend.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/plotly_in_qt.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/raincloud_plot.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/show_image_on_pick.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/stack_bars.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/examples/superplot.py
+-rw-r--r--   0        0        0    93685 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/images/curve_fit.png
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/images/heatmap.png
+-rw-r--r--   0        0        0   205151 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/images/jointgrid.png
+-rw-r--r--   0        0        0    45190 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/images/raincloud.png
+-rw-r--r--   0        0        0    41392 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/images/superplot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/_utils.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0    14332 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_canvas.py
+-rw-r--r--   0        0        0    11908 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_categorical.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_grouping.py
+-rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_layers.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_logics.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_plt.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_theme.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/tests/test_tools.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/__init__.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/_axis.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/_exceptions.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/_signal.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/animation.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/core.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/__init__.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/_app.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/_instance.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/_not_implemented.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/_window/__init__.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/_window/_qt.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/_window/_tk.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/__init__.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/_base.py
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/_labels.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/_legend.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/band.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/bars.py
+-rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/canvas.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/image.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/line.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/markers.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/bokeh/text.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/__init__.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/_base.py
+-rw-r--r--   0        0        0     8132 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/_labels.py
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/_legend.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/band.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/bars.py
+-rw-r--r--   0        0        0    16120 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/canvas.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/image.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/line.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/markers.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/text.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/vectors.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/components3d/__init__.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/components3d/canvas.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/components3d/line.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/components3d/markers.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/components3d/mesh.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/matplotlib/components3d/vectors3d.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/mock/__init__.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/mock/_base.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/mock/canvas.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/mock/layers.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/__init__.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/_base.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/_labels.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/_legend.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/band.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/bars.py
+-rw-r--r--   0        0        0    13475 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/canvas.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/image.py
+-rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/line.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/markers.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/text.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/components3d/__init__.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/components3d/canvas.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/components3d/line.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/components3d/markers.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/plotly/components3d/mesh.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/__init__.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_base.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_labels.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_legend.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_qt_utils.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/band.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/bars.py
+-rw-r--r--   0        0        0    15158 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/canvas.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/image.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/line.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/markers.py
+-rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/text.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/vectors.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/_gridlines.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/_label.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/band.py
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/bars.py
+-rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/canvas.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/image.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/line.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/markers.py
+-rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/text.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/components3d/__init__.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/components3d/axis.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/components3d/canvas.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/components3d/line.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/components3d/markers.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/backend/vispy/components3d/mesh.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/__init__.py
+-rw-r--r--   0        0        0    73609 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_base.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_between.py
+-rw-r--r--   0        0        0    18135 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_dims.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_fit.py
+-rw-r--r--   0        0        0    15308 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_grid.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_imageref.py
+-rw-r--r--   0        0        0    22066 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_joint.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_linker.py
+-rw-r--r--   0        0        0    15101 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_namespaces.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_palette.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/_stacked.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/layerlist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/canvas3d/__init__.py
+-rw-r--r--   0        0        0    22006 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/canvas3d/_base.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/dataframe/__init__.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_base.py
+-rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_both_cat.py
+-rw-r--r--   0        0        0    18971 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_feature_cat.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_joint_cat.py
+-rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_one_cat.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_stacked_cat.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/__init__.py
+-rw-r--r--   0        0        0    11178 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_base.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_legend.py
+-rw-r--r--   0        0        0    36589 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_mixin.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_ndim.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_sizehint.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_text_utils.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/__init__.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/band.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/bars.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/errorbars.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/image.py
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/inf_curve.py
+-rw-r--r--   0        0        0    23189 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/line.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/markers.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/rects.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/rug.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/spans.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/text.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/_primitive/vectors.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/_cat_utils.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/_collections.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/_offsets.py
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/band_collection.py
+-rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/boxplot.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/colorbar.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/graph.py
+-rw-r--r--   0        0        0    25093 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/labeled.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/line_band.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/line_collection.py
+-rw-r--r--   0        0        0    14529 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/line_fill.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/line_markers.py
+-rw-r--r--   0        0        0    16196 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/marker_collection.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/stemplot.py
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/group/textinfo.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/layer3d/__init__.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/layer3d/_base.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/layer3d/line.py
+-rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/layer3d/markers.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/layer3d/mesh.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/layer3d/vectors.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/__init__.py
+-rw-r--r--   0        0        0    41141 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_box_like.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_dataframe.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_df_compat.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_jitter.py
+-rw-r--r--   0        0        0    33317 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_marker_like.py
+-rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_plans.py
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_shared.py
+-rw-r--r--   0        0        0    14768 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/layers/tabular/_stackable.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/plot/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/plot/_canvases.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/plot/_methods.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/protocols/__init__.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/protocols/canvas_protocol.py
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/protocols/layer_protocols.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/theme/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/theme/_api.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/theme/_dataclasses.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/tools/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/tools/_polygon_utils.py
+-rw-r--r--   0        0        0    24164 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/tools/_selection.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/types/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/types/_alias.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/types/_enums.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/types/_mouse.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/types/_tuples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/utils/__init__.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/utils/collections.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/utils/hist.py
+-rw-r--r--   0        0        0    14353 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/utils/kde.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/utils/normalize.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/whitecanvas/utils/type_check.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/README.md
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 whitecanvas-0.3.0/PKG-INFO
```

### Comparing `whitecanvas-0.2.6/.pre-commit-config.yaml` & `whitecanvas-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/mkdocs.yml` & `whitecanvas-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/.github/workflows/docs.yml` & `whitecanvas-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/.github/workflows/test.yml` & `whitecanvas-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/index.md` & `whitecanvas-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/quick_start.md` & `whitecanvas-0.3.0/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/_scripts/_hooks.py` & `whitecanvas-0.3.0/docs/_scripts/_hooks.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/_scripts/_screenshots.py` & `whitecanvas-0.3.0/docs/_scripts/_screenshots.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/canvas/basics.md` & `whitecanvas-0.3.0/docs/canvas/basics.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/canvas/grid.md` & `whitecanvas-0.3.0/docs/canvas/grid.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/canvas/inset_second.md` & `whitecanvas-0.3.0/docs/canvas/inset_second.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/canvas/joint_grid.md` & `whitecanvas-0.3.0/docs/canvas/joint_grid.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/canvas/legend.md` & `whitecanvas-0.3.0/docs/canvas/legend.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/canvas/namespaces.md` & `whitecanvas-0.3.0/docs/canvas/namespaces.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/canvas/native_objects.md` & `whitecanvas-0.3.0/docs/canvas/native_objects.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/categorical/aggregation.md` & `whitecanvas-0.3.0/docs/categorical/aggregation.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/categorical/cat_cat.md` & `whitecanvas-0.3.0/docs/categorical/cat_cat.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/categorical/cat_num.md` & `whitecanvas-0.3.0/docs/categorical/cat_num.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/categorical/index.md` & `whitecanvas-0.3.0/docs/categorical/index.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/categorical/num_num.md` & `whitecanvas-0.3.0/docs/categorical/num_num.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/categorical/stacking.md` & `whitecanvas-0.3.0/docs/categorical/stacking.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/events/index.md` & `whitecanvas-0.3.0/docs/events/index.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/events/mouse_events.md` & `whitecanvas-0.3.0/docs/events/mouse_events.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/layers/distribution.md` & `whitecanvas-0.3.0/docs/layers/distribution.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/layers/face_layers.md` & `whitecanvas-0.3.0/docs/layers/face_layers.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/layers/layer_groups.md` & `whitecanvas-0.3.0/docs/layers/layer_groups.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/layers/lines.md` & `whitecanvas-0.3.0/docs/layers/lines.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/layers/markers.md` & `whitecanvas-0.3.0/docs/layers/markers.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/layers/mouse.md` & `whitecanvas-0.3.0/docs/layers/mouse.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/layers/texts.md` & `whitecanvas-0.3.0/docs/layers/texts.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/docs/tools/selection.md` & `whitecanvas-0.3.0/docs/tools/selection.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/curve_fit.py` & `whitecanvas-0.3.0/examples/curve_fit.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/draw_with_mouse.py` & `whitecanvas-0.3.0/examples/draw_with_mouse.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/fit_layer.py` & `whitecanvas-0.3.0/examples/fit_layer.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/image_profile.py` & `whitecanvas-0.3.0/examples/image_profile.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/joint_grid.py` & `whitecanvas-0.3.0/examples/joint_grid.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/layer_clicked_event.py` & `whitecanvas-0.3.0/examples/layer_clicked_event.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/line_with_error.py` & `whitecanvas-0.3.0/examples/line_with_error.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/line_with_spans.py` & `whitecanvas-0.3.0/examples/line_with_spans.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/markers_hover_text.py` & `whitecanvas-0.3.0/examples/markers_hover_text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/markers_multicolor.py` & `whitecanvas-0.3.0/examples/markers_multicolor.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/raincloud_plot.py` & `whitecanvas-0.3.0/examples/raincloud_plot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/show_image_on_pick.py` & `whitecanvas-0.3.0/examples/show_image_on_pick.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/examples/superplot.py` & `whitecanvas-0.3.0/examples/superplot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/images/curve_fit.png` & `whitecanvas-0.3.0/images/curve_fit.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/images/heatmap.png` & `whitecanvas-0.3.0/images/heatmap.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/images/jointgrid.png` & `whitecanvas-0.3.0/images/jointgrid.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/images/raincloud.png` & `whitecanvas-0.3.0/images/raincloud.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/images/superplot.png` & `whitecanvas-0.3.0/images/superplot.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/tests/_utils.py` & `whitecanvas-0.3.0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/tests/conftest.py` & `whitecanvas-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/tests/test_canvas.py` & `whitecanvas-0.3.0/tests/test_canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import tempfile
 import numpy as np
 from numpy.testing import assert_allclose
 
 import pytest
 import whitecanvas as wc
-from whitecanvas import new_canvas, wrap_canvas
+from whitecanvas import new_canvas, wrap_canvas, new_canvas_3d
 from whitecanvas.types import Point, MouseEvent
 
 from ._utils import assert_color_equal, filter_warning
 
 
 def test_namespaces(backend: str):
     canvas = new_canvas(backend=backend)
@@ -370,7 +370,21 @@
             yield
         history.append("release")
 
     canvas.mouse.emulate_drag([(1, 1), (1, 2), (1, 3)], button="left")
     assert history == []
     canvas.mouse.emulate_drag([(1, 1), (1, 2), (1, 3)], button="right")
     assert history == ["press", "move", "move", "release"]
+
+def test_canvas_3d(backend: str):
+    if backend not in ("matplotlib", "vispy", "plotly"):
+        pytest.skip(f"{backend} does not support 3d")
+    canvas = new_canvas_3d(backend=backend)
+    if backend != "vispy":
+        canvas.update_axes(visible=True, color="gray")
+        canvas.update_font(size=13, color="pink", family="Arial")
+    canvas.update_labels(title="Title", x="X", y="Y", z="Z")
+    canvas.add_line([0, 1, 2], [0, 1, 2], [0, 1, 2])
+    canvas.add_markers([0, 1, 2], [0, 1, 2], [0, 1, 2])
+    if backend == "matplotlib":
+        canvas.add_vectors([0, 1, 2], [0, 1, 2], [0, 0, 0], [0, 1, 2], [0, 1, 2], [1, 1, 1])
+    canvas.add_surface(np.array([[2,3,2], [3,2,3]]))
```

### Comparing `whitecanvas-0.2.6/tests/test_categorical.py` & `whitecanvas-0.3.0/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/tests/test_grouping.py` & `whitecanvas-0.3.0/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/tests/test_layers.py` & `whitecanvas-0.3.0/tests/test_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,7 +381,25 @@
     layer.data
     assert layer.ndata == 2
     layer.data = [5, 10, 18, 30]
     layer.data = [[5, 10, 18, 30], [15, 20, 18, 21]]
     layer.rects
     layer.as_edge_only()
     layer.with_hover_template("x={left:.2f}, y={bottom:.2f}")
+
+
+def test_vectors(backend: str):
+    if backend not in ("matplotlib", "pyqtgraph", "mock"):
+        pytest.skip(f"Vectors not supported by {backend}")
+    canvas = new_canvas(backend=backend)
+    layer = canvas.add_vectors(np.arange(10), np.zeros(10), np.ones(10), np.zeros(10))
+    layer.data
+    assert_allclose(layer.data.x, np.arange(10))
+    assert_allclose(layer.data.y, np.zeros(10))
+    assert_allclose(layer.data.vx, np.ones(10))
+    assert_allclose(layer.data.vy, np.zeros(10))
+    layer.data = np.arange(10) * 2, np.zeros(10), np.ones(10), np.zeros(10)
+    assert_allclose(layer.data.x, np.arange(10) * 2)
+    layer.color
+    layer.color = [1.0, 0.0, 0.0, 1.0]
+    layer.width = 3
+    layer.style = ":"
```

### Comparing `whitecanvas-0.2.6/tests/test_logics.py` & `whitecanvas-0.3.0/tests/test_logics.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/tests/test_theme.py` & `whitecanvas-0.3.0/tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/tests/test_tools.py` & `whitecanvas-0.3.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/_axis.py` & `whitecanvas-0.3.0/whitecanvas/_axis.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/_signal.py` & `whitecanvas-0.3.0/whitecanvas/_signal.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/animation.py` & `whitecanvas-0.3.0/whitecanvas/animation.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/core.py` & `whitecanvas-0.3.0/whitecanvas/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,30 @@
     _grid.add_canvas(0, 0, palette=palette)
     cvs = SingleCanvas(_grid)
     if size is not None:
         cvs.size = size
     return cvs
 
 
+def new_canvas_3d(
+    backend: Backend | str | None = None,
+    *,
+    size: tuple[int, int] | None = None,
+    palette: str | ColormapType | None = None,
+):
+    from whitecanvas.canvas.canvas3d._base import SingleCanvas3D
+
+    _grid = CanvasGrid([1], [1], backend=backend)
+    _grid.add_canvas_3d(0, 0, palette=palette)
+    cvs = SingleCanvas3D(_grid)
+    if size is not None:
+        cvs.size = size
+    return cvs
+
+
 def new_grid(
     rows: int | Sequence[int] = 1,
     cols: int | Sequence[int] = 1,
     *,
     size: tuple[int, int] | None = None,
     backend: Backend | str | None = None,
 ) -> CanvasGrid:
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/_app.py` & `whitecanvas-0.3.0/whitecanvas/backend/_app.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/_instance.py` & `whitecanvas-0.3.0/whitecanvas/backend/_instance.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,14 +68,25 @@
     def get(self, attr: str):
         """Get an object from the current backend."""
         out = getattr(self._mod, attr, None)
         if out is None:
             raise RuntimeError(f"Backend {self._name!r} does not implement {attr!r}")
         return out
 
+    def get_submodule(self, attr: str):
+        """Get a submodule from the current backend."""
+        import importlib
+
+        if self.is_dummy():
+            return _dummy_backend_module
+        out = importlib.import_module(f"whitecanvas.backend.{self._name}.{attr}")
+        if out is None:
+            raise RuntimeError(f"Backend {self._name!r} does not implement {attr!r}")
+        return out
+
     def is_dummy(self) -> bool:
         """True is the backend is a dummy backend."""
         return self.name.startswith(".")
 
 
 class DummyObject:
     def __init__(self, *args, **kwargs):
@@ -83,15 +94,15 @@
 
 
 class DummyBackendModule:
     def __init__(self):
         self.Canvas = DummyObject
 
     def __getattr__(self, key):
-        raise RuntimeError(f"Cannot install {key!r} before finishing layouting.")
+        return DummyObject
 
 
 _dummy_backend_module = DummyBackendModule()
 
 
 @contextmanager
 def patch_dummy_backend():
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/_not_implemented.py` & `whitecanvas-0.3.0/whitecanvas/backend/_not_implemented.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import numpy as np
+
 from whitecanvas.types import Hatch, LineStyle
 
 
 def edge_style():
     def _getter(self):
         return getattr(self, "__edge_style_value", LineStyle.SOLID)
 
@@ -23,29 +25,51 @@
         if isinstance(value, LineStyle):
             value = [value] * self._plt_get_ndata()
         setattr(self, "__edge_style_value", value)
 
     return _getter, _setter
 
 
-def face_pattern():
+def edge_width():
+    def _getter(self):
+        return getattr(self, "__edge_width_value", 1.0)
+
+    def _setter(self, value: float):
+        setattr(self, "__edge_width_value", value)
+
+    return _getter, _setter
+
+
+def edge_color():
+    def _getter(self):
+        return getattr(
+            self, "__edge_color_value", np.array([0, 0, 0, 255], dtype=np.float32)
+        )
+
+    def _setter(self, value: float):
+        setattr(self, "__edge_color_value", value)
+
+    return _getter, _setter
+
+
+def face_hatch():
     def _getter(self):
-        return getattr(self, "__face_pattern_value", Hatch.SOLID)
+        return getattr(self, "__face_hatch_value", Hatch.SOLID)
 
     def _setter(self, value: Hatch):
-        setattr(self, "__face_pattern_value", value)
+        setattr(self, "__face_hatch_value", value)
 
     return _getter, _setter
 
 
-def face_patterns():
+def face_hatches():
     def _getter(self):
         return getattr(
-            self, "__face_pattern_value", [Hatch.SOLID] * self._plt_get_ndata()
+            self, "__face_hatch_value", [Hatch.SOLID] * self._plt_get_ndata()
         )
 
     def _setter(self, value: Hatch | list[Hatch]):
         if isinstance(value, Hatch):
             value = [value] * self._plt_get_ndata()
-        setattr(self, "__face_pattern_value", value)
+        setattr(self, "__face_hatch_value", value)
 
     return _getter, _setter
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/_window/__init__.py` & `whitecanvas-0.3.0/whitecanvas/backend/_window/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/_window/_qt.py` & `whitecanvas-0.3.0/whitecanvas/backend/_window/_qt.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/_window/_tk.py` & `whitecanvas-0.3.0/whitecanvas/backend/_window/_tk.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/_base.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/_labels.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/_labels.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/_legend.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/band.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/bars.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/bars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/canvas.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/canvas.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/image.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/line.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/markers.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/bokeh/text.py` & `whitecanvas-0.3.0/whitecanvas/backend/bokeh/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_base.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,20 @@
     def _plt_set_visible(self, visible):
         self.set_visible(visible)
 
     def _plt_set_zorder(self, zorder: int):
         self.set_zorder(zorder)
 
 
+class FakeAxes:
+    def __init__(self):
+        self.transData = None
+        self.transAxes = None
+
+
 def symbol_to_path(symbol: Symbol):
     marker_obj = mmarkers.MarkerStyle(symbol.value)
     return marker_obj.get_path().transformed(marker_obj.get_transform())
 
 
 OVERLAY_ZORDER = 10000
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_labels.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/_labels.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from matplotlib import pyplot as plt
 from matplotlib.ticker import AutoLocator, AutoMinorLocator
 
 from whitecanvas.types import LineStyle
 
 if TYPE_CHECKING:
+    from matplotlib import axis as mpl_axis
+    from matplotlib import text as mpl_text
+
     from whitecanvas.backend.matplotlib.canvas import Canvas
 
 
 class SupportsText:
     def __init__(self, canvas: Canvas):
         self._canvas = weakref.ref(canvas)
         self._text = ""
@@ -73,256 +76,170 @@
     def _plt_set_fontfamily(self, font):
         d = self._fontdict.copy()
         d["family"] = font
         self._canvas()._axes.set_title(self._text, fontdict=d)
         self._fontdict = d
 
 
-class XLabel(SupportsText):
+class MplLabel(SupportsText):
+    def __init__(self, canvas: Canvas, name: str):
+        super().__init__(canvas)
+        self._axis_name = name
+
+    def _set_label(self, text: str, fontdict: dict[str, str] = {}):
+        fname = f"set_{self._axis_name}label"
+        getattr(self._canvas()._axes, fname)(text, fontdict)
+
     def _plt_get_text(self) -> str:
-        return self._canvas()._axes.get_xlabel()
+        return getattr(self._canvas()._axes, f"get_{self._axis_name}label")()
 
     def _plt_set_text(self, text: str):
-        self._canvas()._axes.set_xlabel(text, self._fontdict)
+        self._set_label(text, self._fontdict)
         self._text = text
 
     def _plt_set_color(self, color):
         d = self._fontdict.copy()
         d["color"] = color
-        self._canvas()._axes.set_xlabel(self._text, fontdict=d)
+        self._set_label(self._text, fontdict=d)
         self._fontdict = d
 
     def _plt_get_visible(self) -> bool:
         return bool(self._canvas()._axes.get_xlabel())
 
     def _plt_set_visible(self, visible: bool):
         if visible:
-            self._canvas()._axes.set_xlabel(self._text, fontdict=self._fontdict)
+            self._set_label(self._text, fontdict=self._fontdict)
         else:
-            self._canvas()._axes.set_xlabel("")
+            self._set_label("")
 
     def _plt_set_size(self, size: str):
         d = self._fontdict.copy()
         d["fontsize"] = size
-        self._canvas()._axes.set_xlabel(self._text, fontdict=d)
+        self._set_label(self._text, fontdict=d)
         self._fontdict = d
 
     def _plt_set_fontfamily(self, font):
         d = self._fontdict.copy()
         d["family"] = font
-        self._canvas()._axes.set_xlabel(self._text, fontdict=d)
-        self._fontdict = d
-
-
-class YLabel(SupportsText):
-    def _plt_get_text(self) -> str:
-        return self._canvas()._axes.get_ylabel()
-
-    def _plt_set_text(self, text: str):
-        self._canvas()._axes.set_ylabel(text, self._fontdict)
-        self._text = text
-
-    def _plt_set_color(self, color):
-        d = self._fontdict.copy()
-        d["color"] = color
-        self._canvas()._axes.set_ylabel(self._text, fontdict=d)
+        self._set_label(self._text, fontdict=d)
         self._fontdict = d
 
-    def _plt_get_visible(self) -> bool:
-        return bool(self._canvas()._axes.get_ylabel())
 
-    def _plt_set_visible(self, visible: bool):
-        if visible:
-            self._canvas()._axes.set_ylabel(self._text, fontdict=self._fontdict)
-        else:
-            self._canvas()._axes.set_ylabel("")
+class MplTicks(SupportsText):
+    def __init__(self, canvas: Canvas, name: str):
+        super().__init__(canvas)
+        self._axis_name = name
 
-    def _plt_set_size(self, size: str):
-        d = self._fontdict.copy()
-        d["fontsize"] = size
-        self._canvas()._axes.set_ylabel(self._text, fontdict=d)
-        self._fontdict = d
+    def _get_tick_labels(self) -> list[mpl_text.Text]:
+        axes = self._canvas()._axes
+        return getattr(axes, f"get_{self._axis_name}ticklabels")()
 
-    def _plt_set_fontfamily(self, font):
-        d = self._fontdict.copy()
-        d["family"] = font
-        self._canvas()._axes.set_ylabel(self._text, fontdict=d)
-        self._fontdict = d
+    def _get_ticks(self) -> list[float]:
+        axes = self._canvas()._axes
+        return getattr(axes, f"get_{self._axis_name}ticks")()
 
+    def _set_ticks(self, ticks: list[float]):
+        axes = self._canvas()._axes
+        getattr(axes, f"set_{self._axis_name}ticks")(ticks)
 
-class XTicks(SupportsText):
     def _plt_get_tick_labels(self) -> tuple[list[float], list[str]]:
-        axes = self._canvas()._axes
-        return axes.get_xticks(), [x.get_text() for x in axes.get_xticklabels()]
+        return self._get_ticks(), [x.get_text() for x in self._get_tick_labels()]
 
     def _plt_override_labels(self, pos: list[float], labels: list[str]):
-        self._canvas()._axes.set_xticks(pos, labels)
+        axes = self._canvas()._axes
+        getattr(axes, f"set_{self._axis_name}ticks")(pos, labels)
 
     def _plt_reset_override(self):
         # FIXME: This is not a perfect solution. It will update the x-axis scale.
-        self._canvas()._axes.get_xaxis().clear()
+        axis = getattr(self._canvas()._axes, f"get_{self._axis_name}axis")()
+        axis.clear()
 
     def _plt_set_color(self, color):
         d = self._fontdict.copy()
         d["color"] = color
-        for x in self._canvas()._axes.get_xticklabels():
+        for x in self._get_tick_labels():
             x.set_color(color)
         self._fontdict = d
 
     def _plt_get_visible(self) -> bool:
-        return self._canvas()._axes.get_xticklines()[0].get_visible()
+        ticklines = getattr(self._canvas()._axes, f"get_{self._axis_name}ticklines")()
+        return ticklines[0].get_visible()
 
     def _plt_set_visible(self, visible: bool):
         axes = self._canvas()._axes
-        for tick in axes.get_xticklines():
+        for tick in getattr(axes, f"get_{self._axis_name}ticklines")():
             tick.set_visible(visible)
-        for text in axes.get_xticklabels():
+        for text in self._get_tick_labels():
             text.set_visible(visible)
 
     def _plt_set_size(self, size: str):
         d = self._fontdict.copy()
         d["fontsize"] = size
-        for x in self._canvas()._axes.get_xticklabels():
+        for x in self._get_tick_labels():
             x.set_fontsize(size)
         self._fontdict = d
 
     def _plt_set_fontfamily(self, font):
         d = self._fontdict.copy()
         d["family"] = font
-        for x in self._canvas()._axes.get_xticklabels():
+        for x in self._get_tick_labels():
             x.set_fontfamily(font)
         self._fontdict = d
 
     def _plt_get_text_rotation(self) -> float:
-        return self._canvas()._axes.get_xticklabels()[0].get_rotation()
+        return self._get_tick_labels()[0].get_rotation()
 
     def _plt_set_text_rotation(self, rotation: float):
-        for x in self._canvas()._axes.get_xticklabels():
+        for x in self._get_tick_labels():
             x.set_rotation(rotation)
 
 
-class YTicks(SupportsText):
-    def _plt_get_tick_labels(self) -> tuple[list[float], list[str]]:
-        axes = self._canvas()._axes
-        return axes.get_yticks(), [x.get_text() for x in axes.get_yticklabels()]
-
-    def _plt_override_labels(self, pos: list[float], labels: list[str]):
-        self._canvas()._axes.set_yticks(pos, labels)
-
-    def _plt_reset_override(self):
-        self._canvas()._axes.get_yaxis().clear()
-
-    def _plt_set_color(self, color):
-        d = self._fontdict.copy()
-        d["color"] = color
-        for x in self._canvas()._axes.get_yticklabels():
-            x.set_color(color)
-        self._fontdict = d
-
-    def _plt_get_visible(self) -> bool:
-        return self._canvas()._axes.get_yticklines()[0].get_visible()
-
-    def _plt_set_visible(self, visible: bool):
-        axes = self._canvas()._axes
-        for tick in axes.get_yticklines():
-            tick.set_visible(visible)
-        for text in axes.get_yticklabels():
-            text.set_visible(visible)
-
-    def _plt_set_size(self, size: str):
-        d = self._fontdict.copy()
-        d["fontsize"] = size
-        for x in self._canvas()._axes.get_yticklabels():
-            x.set_fontsize(size)
-        self._fontdict = d
-
-    def _plt_set_fontfamily(self, font):
-        d = self._fontdict.copy()
-        d["family"] = font
-        for x in self._canvas()._axes.get_yticklabels():
-            x.set_fontfamily(font)
-        self._fontdict = d
-
-
-class AxisBase:
-    def __init__(self, canvas: Canvas):
-        self._canvas = weakref.ref(canvas)
-
-
-class XAxis(AxisBase):
-    def __init__(self, canvas: Canvas):
+class MplAxis:
+    def __init__(self, canvas: Canvas, name: str):
         self._canvas = weakref.ref(canvas)
+        self._axis_name = name
 
     def _plt_get_limits(self) -> tuple[float, float]:
         axes = self._canvas()._axes
-        x0, x1 = axes.get_xlim()
-        if axes.xaxis_inverted():
+        x0, x1 = getattr(axes, f"get_{self._axis_name}lim")()
+        if getattr(axes, f"{self._axis_name}axis_inverted")():
             return x1, x0
         else:
             return x0, x1
 
     def _plt_set_limits(self, limits: tuple[float, float]):
         axes = self._canvas()._axes
-        if axes.xaxis_inverted():
+        if getattr(axes, f"{self._axis_name}axis_inverted")():
             limits = limits[::-1]
-        axes.set_xlim(*limits)
-
-    def _plt_get_color(self):
-        return self._canvas()._axes.xaxis.get_tick_params()["color"]
+        getattr(axes, f"set_{self._axis_name}lim")(*limits)
 
-    def _plt_set_color(self, color):
-        ax = self._canvas()._axes
-        color = tuple(color)
-        ax.xaxis.set_tick_params(color=color, labelcolor=color)
-        ax.spines["bottom"].set_color(color)
-
-    def _plt_flip(self):
-        self._canvas()._axes.invert_xaxis()
-
-    def _plt_set_grid_state(self, visible: bool, color, width: float, style: LineStyle):
-        self._canvas()._axes.xaxis.grid(
-            visible,
-            which="major",
-            color=color,
-            linestyle=style.value,
-            linewidth=width,
-        )
-
-
-class YAxis(AxisBase):
-    def __init__(self, canvas: Canvas):
-        self._canvas = weakref.ref(canvas)
-
-    def _plt_get_limits(self) -> tuple[float, float]:
-        axes = self._canvas()._axes
-        y0, y1 = axes.get_ylim()
-        if axes.yaxis_inverted():
-            return y1, y0
-        else:
-            return y0, y1
-
-    def _plt_set_limits(self, limits: tuple[float, float]):
-        axes = self._canvas()._axes
-        if axes.yaxis_inverted():
-            limits = limits[::-1]
-        axes.set_ylim(*limits)
+    def _get_mpl_axis(self) -> mpl_axis.Axis:
+        return getattr(self._canvas()._axes, f"{self._axis_name}axis")
 
     def _plt_get_color(self):
-        return self._canvas()._axes.yaxis.get_tick_params()["color"]
+        return self._get_mpl_axis().get_tick_params()["color"]
 
     def _plt_set_color(self, color):
-        ax = self._canvas()._axes
+        ax = self._get_mpl_axis()
         color = tuple(color)
-        ax.yaxis.set_tick_params(color=color, labelcolor=color)
-        ax.spines["left"].set_color(color)
+        ax.set_tick_params(color=color, labelcolor=color)
+        if hasattr(ax, "line"):  # 3D
+            ax.line.set_color(color)
+        else:
+            if self._axis_name == "x":
+                self._canvas()._axes.spines["bottom"].set_color(color)
+            else:
+                self._canvas()._axes.spines["left"].set_color(color)
 
     def _plt_flip(self):
-        self._canvas()._axes.invert_yaxis()
+        axis = self._get_mpl_axis()
+        axis.set_inverted(not axis.get_inverted())
 
     def _plt_set_grid_state(self, visible: bool, color, width: float, style: LineStyle):
-        self._canvas()._axes.yaxis.grid(
+        axis = self._get_mpl_axis()
+        axis.grid(
             visible,
             which="major",
             color=color,
             linestyle=style.value,
             linewidth=width,
         )
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_legend.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/_legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,17 @@
     )  # fmt: skip
 
 
 @make_sample_item.register
 def _(item: _leg.ErrorLegendItem):
     line_2d = Line2D([], [], color="#00000000")
     caps = Line2D([], [], color=item.color, linewidth=item.width)
-    barlines = Line2D(
-        [], [], color=item.color, linewidth=item.width, linestyle=item.style.value
-    )  # fmt: skip
+    barlines = LineCollection(
+        [], color=item.color, linewidth=item.width, linestyle=item.style.value
+    )
     return ErrorbarContainer((line_2d, (caps,), [barlines]), has_yerr=True)
 
 
 @make_sample_item.register
 def _(item: _leg.LineErrorLegendItem):
     line_2d = make_sample_item(item.line)
     caps, barlines, has_xerr, has_yerr = _norm_xyerr(item.xerr, item.yerr)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/band.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/bars.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/bars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/canvas.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,33 +4,26 @@
 from timeit import default_timer
 from typing import Callable
 
 import matplotlib as mpl
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.artist import Artist
-from matplotlib.backend_bases import (
-    MouseButton as mplMouseButton,
-)
-from matplotlib.backend_bases import (
-    MouseEvent as mplMouseEvent,
-)
+from matplotlib.backend_bases import MouseButton as mplMouseButton
+from matplotlib.backend_bases import MouseEvent as mplMouseEvent
 from matplotlib.collections import Collection
 from matplotlib.lines import Line2D
 
 from whitecanvas import protocols
 from whitecanvas.backend.matplotlib._base import MplLayer, MplMouseEventsMixin
 from whitecanvas.backend.matplotlib._labels import (
+    MplAxis,
+    MplLabel,
+    MplTicks,
     Title,
-    XAxis,
-    XLabel,
-    XTicks,
-    YAxis,
-    YLabel,
-    YTicks,
 )
 from whitecanvas.backend.matplotlib._legend import make_sample_item
 from whitecanvas.backend.matplotlib.bars import Bars
 from whitecanvas.backend.matplotlib.image import Image as whitecanvasImage
 from whitecanvas.backend.matplotlib.text import Texts as whitecanvasText
 from whitecanvas.layers._legend import LegendItem, LegendItemCollection
 from whitecanvas.types import (
@@ -43,21 +36,21 @@
 )
 
 
 @protocols.check_protocol(protocols.CanvasProtocol)
 class Canvas:
     def __init__(self, ax: plt.Axes):
         self._axes = ax
-        self._xaxis = XAxis(self)
-        self._yaxis = YAxis(self)
+        self._xaxis = MplAxis(self, "x")
+        self._yaxis = MplAxis(self, "y")
         self._title = Title(self)
-        self._xlabel = XLabel(self)
-        self._ylabel = YLabel(self)
-        self._xticks = XTicks(self)
-        self._yticks = YTicks(self)
+        self._xlabel = MplLabel(self, "x")
+        self._ylabel = MplLabel(self, "y")
+        self._xticks = MplTicks(self, "x")
+        self._yticks = MplTicks(self, "y")
         ax.set_axisbelow(True)  # grid lines below other layers
         self._annot = ax.annotate(
             text="", xy=(0, 0), xytext=(20, -20), textcoords="data",
             bbox={"fc": np.array([1.0, 1.0, 1.0, 0.67])},
             fontproperties={"size": 14, "family": "Arial"},
             clip_on=False, zorder=10000,
         )  # fmt: skip
@@ -387,14 +380,23 @@
     def _plt_add_canvas(self, row: int, col: int, rowspan: int, colspan: int) -> Canvas:
         r1 = row + rowspan
         c1 = col + colspan
         axes = self._fig.add_subplot(self._gridspec[row:r1, col:c1])
         axes.set_facecolor(self._fig.get_facecolor())
         return Canvas(axes)
 
+    def _plt_add_canvas_3d(self, row: int, col: int, rowspan: int, colspan: int):
+        from whitecanvas.backend.matplotlib.components3d import Canvas3D
+
+        r1 = row + rowspan
+        c1 = col + colspan
+        axes = self._fig.add_subplot(self._gridspec[row:r1, col:c1], projection="3d")
+        axes.set_facecolor(self._fig.get_facecolor())
+        return Canvas3D(axes)
+
     def _plt_get_visible(self) -> bool:
         return self._fig.get_visible()
 
     def _plt_show(self):
         # TODO: show the inline plot again
         self._fig.show(warn=False)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/image.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/line.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/markers.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/text.py` & `whitecanvas-0.3.0/whitecanvas/backend/matplotlib/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/mock/_base.py` & `whitecanvas-0.3.0/whitecanvas/backend/mock/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/mock/canvas.py` & `whitecanvas-0.3.0/whitecanvas/backend/mock/canvas.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/mock/layers.py` & `whitecanvas-0.3.0/whitecanvas/backend/mock/layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import numpy as np
 from cmap import Colormap
+from numpy.typing import NDArray
 
 from whitecanvas import protocols
 from whitecanvas.backend.mock._base import (
     BaseMockLayer,
     MockHasData,
     MockHasEdges,
     MockHasFaces,
@@ -210,7 +211,31 @@
         self._rotation = rotation
 
     def _plt_get_text_fontfamily(self) -> str:
         return self._fontfamily
 
     def _plt_set_text_fontfamily(self, family: str):
         self._fontfamily = family
+
+
+@protocols.check_protocol(protocols.VectorsProtocol)
+class Vectors(MockHasData, MockHasEdges):
+    def __init__(self, x0, dx, y0, dy):
+        super().__init__((x0, dx, y0, dy))
+
+    def _plt_get_ndata(self) -> int:
+        return self._plt_get_data()[0].size
+
+    def _plt_get_edge_color(self) -> NDArray[np.float32]:
+        if not hasattr(self, "_edge_color"):
+            ndata = self._plt_get_ndata()
+            self._edge_color = np.zeros((ndata, 4), dtype=np.float32)
+        return self._edge_color
+
+    def _plt_set_edge_color(self, color: NDArray[np.float32]):
+        self._edge_color = as_color_array(color, self._plt_get_ndata())
+
+    def _plt_get_antialias(self) -> bool:
+        return self._antialias
+
+    def _plt_set_antialias(self, antialias: bool):
+        self._antialias = antialias
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/_base.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/_labels.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/_labels.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         self._axis = axis
 
     def _get_title(self):
         layout = self._canvas()._subplot_layout()
         return getattr(layout, self._axis).title
 
 
+class AxisLabel3D(AxisLabel):
+    def _get_title(self):
+        layout = self._canvas()._subplot_layout()
+        return getattr(layout.scene, self._axis).title
+
+
 class Axis(_CanvasComponent):
     def __init__(self, canvas: Canvas, axis: str):
         super().__init__(canvas)
         self._axis = axis
 
     @property
     def name(self) -> str:
@@ -120,14 +126,19 @@
     def _plt_set_grid_state(self, visible: bool, color, width: float, style: LineStyle):
         axis = self._plt_get_axis()
         axis.showgrid = visible
         axis.gridcolor = rgba_str_color(color)
         axis.gridwidth = width
 
 
+class Axis3D(Axis):
+    def _plt_get_axis(self):
+        return getattr(self._canvas()._subplot_layout().scene, self._axis)
+
+
 class Ticks(_CanvasComponent):
     def __init__(self, canvas: Canvas, axis: str):
         super().__init__(canvas)
         self._axis = axis
         self._visible = True
 
     def _plt_get_axis(self):
@@ -174,7 +185,13 @@
         self._plt_get_axis().tickfont.color = rgba_str_color(color)
 
     def _plt_get_text_rotation(self) -> float:
         return -self._plt_get_axis().tickangle
 
     def _plt_set_text_rotation(self, angle: float):
         self._plt_get_axis().tickangle = -angle
+
+
+class Ticks3D(Ticks):
+    def _plt_get_axis(self):
+        layout = self._canvas()._subplot_layout()
+        return getattr(layout.scene, self._axis)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/_legend.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/band.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/band.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import numpy as np
 from plotly import graph_objects as go
 
-from whitecanvas.backend._not_implemented import face_pattern
+from whitecanvas.backend._not_implemented import face_hatch
 from whitecanvas.backend.plotly._base import (
     PlotlyHoverableLayer,
     from_plotly_linestyle,
     to_plotly_linestyle,
 )
 from whitecanvas.protocols import BandProtocol, check_protocol
 from whitecanvas.types import LineStyle, Orientation
@@ -77,15 +77,15 @@
 
     def _plt_get_face_color(self):
         return arr_color(self._props["fillcolor"])
 
     def _plt_set_face_color(self, color):
         self._props["fillcolor"] = rgba_str_color(color)
 
-    _plt_get_face_hatch, _plt_set_face_hatch = face_pattern()
+    _plt_get_face_hatch, _plt_set_face_hatch = face_hatch()
 
     def _plt_get_edge_color(self):
         return arr_color(self._props["line"]["color"])
 
     def _plt_set_edge_color(self, color):
         self._props["line"]["color"] = rgba_str_color(color)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/bars.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/bars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/canvas.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,14 +385,19 @@
         self._widths = widths
 
     def _plt_add_canvas(self, row: int, col: int, rowspan: int, colspan: int) -> Canvas:
         if rowspan > 1 or colspan > 1:
             raise NotImplementedError("Plotly backend does not support rowspan/colspan")
         return Canvas(self._figs, row=row, col=col, app=self._app)
 
+    def _plt_add_canvas_3d(self, row: int, col: int, rowspan: int, colspan: int):
+        from whitecanvas.backend.plotly.components3d import Canvas3D
+
+        return Canvas3D(self._figs, row=row, col=col, app=self._app)
+
     def _plt_show(self):
         if self._app in ("qt", "wx", "tk"):
             return NotImplemented
         if self._app == "notebook" and "IPython" in sys.modules:
             from IPython import get_ipython
             from IPython.display import display
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/image.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/line.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/markers.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             return np.empty((0, 4), dtype=np.float32)
         return np.stack([arr_color(c) for c in color], axis=0)
 
     def _plt_set_face_color(self, color: NDArray[np.float32]):
         color = as_color_array(color, self._plt_get_ndata())
         self._props["marker"]["color"] = [rgba_str_color(c) for c in color]
 
-    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_patterns()
+    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_hatches()
 
     def _plt_get_symbol(self) -> Symbol:
         return from_plotly_marker_symbol(self._props["marker"]["symbol"])
 
     def _plt_set_symbol(self, symbol: Symbol):
         self._props["marker"]["symbol"] = to_plotly_marker_symbol(symbol)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/plotly/text.py` & `whitecanvas-0.3.0/whitecanvas/backend/plotly/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_base.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_labels.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_labels.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_legend.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_qt_utils.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/_qt_utils.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/band.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/bars.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/bars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/canvas.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/canvas.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/image.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import numpy as np
 import pyqtgraph as pg
 from cmap import Colormap
 from qtpy.QtGui import QTransform
 
 from whitecanvas.backend.pyqtgraph._base import PyQtLayer
-from whitecanvas.backend.pyqtgraph._qt_utils import array_to_qcolor
 from whitecanvas.protocols import ImageProtocol, check_protocol
 
 
 @check_protocol(ImageProtocol)
 class Image(pg.ImageItem, PyQtLayer):
     def __init__(self, data: np.ndarray):
         super().__init__(np.swapaxes(data, 0, 1))
@@ -24,18 +23,15 @@
         self.setImage(np.swapaxes(data, 0, 1))
 
     def _plt_get_colormap(self) -> Colormap:
         return self._cmap
 
     def _plt_set_colormap(self, cmap: Colormap):
         self._cmap = cmap
-        stops = cmap.color_stops
-        colors = [array_to_qcolor(col) for col in stops.color_array]
-        pg_cmap = pg.ColorMap(stops.stops, colors)
-        self.setColorMap(pg_cmap)
+        self.setColorMap(cmap.to_pyqtgraph())
 
     def _plt_get_clim(self) -> tuple[float, float]:
         low, high = self.getLevels()
         return low, high
 
     def _plt_set_clim(self, clim: tuple[float, float]):
         self.setLevels(clim)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/line.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,19 +104,19 @@
 
 @check_protocol(MultiLineProtocol)
 class MultiLine(pg.ItemGroup, PyQtLayer):
     clicked = QtCore.Signal(list)
 
     def __init__(self, data: list[NDArray[np.floating]]):
         super().__init__()
-        pen = QtGui.QPen(QtGui.QColor(255, 255, 255))
-        pen.setCosmetic(True)
         self._lines: list[pg.PlotCurveItem] = []
         self._qpens: list[QtGui.QPen] = []
         for i, seg in enumerate(data):
+            pen = QtGui.QPen(QtGui.QColor(255, 255, 255))
+            pen.setCosmetic(True)
             item = pg.PlotCurveItem(
                 seg[:, 0], seg[:, 1], pen=pen, antialias=True, clickable=True
             )
             item.sigClicked.connect(self._clicked_cb(i))
             self.addItem(item)
             self._lines.append(item)
             self._qpens.append(pen)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/markers.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/text.py` & `whitecanvas-0.3.0/whitecanvas/backend/pyqtgraph/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/_gridlines.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/_gridlines.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/_label.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/_label.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/band.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/band.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     ##### HasFace protocol #####
     def _plt_get_face_color(self) -> NDArray[np.float32]:
         return np.array(self.color, dtype=np.float32)
 
     def _plt_set_face_color(self, color: NDArray[np.float32]):
         self.color = color
 
-    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_pattern()
+    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_hatch()
 
     ##### HasEdges protocol #####
     def _plt_get_edge_color(self) -> NDArray[np.float32]:
         return np.array(self.border_color, dtype=np.float32)
 
     def _plt_set_edge_color(self, color: NDArray[np.float32]):
         self.border_color = color
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/bars.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/bars.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         return np.stack(colors, axis=0)
 
     def _plt_set_face_color(self, color: NDArray[np.float32]):
         color = as_color_array(color, size=self._plt_get_ndata())
         for rect, c in zip(self._rectangles, color):
             rect.color = c
 
-    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_patterns()
+    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_hatches()
 
     ##### HasEdges protocol #####
     def _plt_get_edge_color(self) -> NDArray[np.float32]:
         colors = []
         for rect in self._rectangles:
             colors.append(rect.border_color)
         return np.stack(colors, axis=0)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/canvas.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,24 +233,37 @@
             vispy_use(_APP_NAMES.get(app, app))
         self._scene = SceneCanvasExt(keys="interactive")
         self._grid: Grid = self._scene.central_widget.add_grid()
         self._scene.create_native()
         self._heights = heights
         self._widths = widths
 
-    def _plt_add_canvas(self, row: int, col: int, rowspan: int, colspan: int):
+    def _calc_rc_and_span(self, row: int, col: int, rowspan: int, colspan: int):
         rspan = sum(self._heights[row : row + rowspan])
         cspan = sum(self._widths[col : col + colspan])
         r = sum(self._heights[:row])
         c = sum(self._widths[:col])
-        viewbox: ViewBox = self._grid.add_view(r, c, rspan, cspan)
+        return r, c, rspan, cspan
+
+    def _plt_add_canvas(self, row: int, col: int, rowspan: int, colspan: int):
+        view_pos = self._calc_rc_and_span(row, col, rowspan, colspan)
+        viewbox: ViewBox = self._grid.add_view(*view_pos)
         canvas = Canvas(viewbox)
         canvas._set_scene_ref(self._scene)
         return canvas
 
+    def _plt_add_canvas_3d(self, row: int, col: int, rowspan: int, colspan: int):
+        from whitecanvas.backend.vispy.components3d import Canvas3D
+
+        view_pos = self._calc_rc_and_span(row, col, rowspan, colspan)
+        viewbox: ViewBox = self._grid.add_view(*view_pos)
+        canvas = Canvas3D(viewbox)
+        # canvas._set_scene_ref(self._scene)
+        return canvas
+
     def _plt_get_background_color(self):
         return self._scene.bgcolor.rgba
 
     def _plt_set_background_color(self, color):
         self._scene.bgcolor = color
 
     def _plt_screenshot(self) -> NDArray[np.uint8]:
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/image.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/line.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/markers.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             size=self._plt_get_symbol_size(),
             edge_width=self._plt_get_edge_width(),
             face_color=color,
             edge_color=self._plt_get_edge_color(),
             symbol=self.symbol,
         )
 
-    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_patterns()
+    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_hatches()
 
     ##### HasEdges protocol #####
     def _plt_get_edge_color(self) -> NDArray[np.float32]:
         return self._data["a_fg_color"]
 
     def _plt_set_edge_color(self, color: NDArray[np.float32]):
         color = as_color_array(color, self._plt_get_ndata())
```

### Comparing `whitecanvas-0.2.6/whitecanvas/backend/vispy/text.py` & `whitecanvas-0.3.0/whitecanvas/backend/vispy/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     def _plt_get_face_color(self):
         return np.zeros((self._plt_get_ndata(), 4))
 
     def _plt_set_face_color(self, color):
         pass
 
-    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_patterns()
+    _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_hatches()
 
     def _plt_get_edge_color(self):
         return np.zeros((self._plt_get_ndata(), 4))
 
     def _plt_set_edge_color(self, color):
         pass
```

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_base.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,32 +66,164 @@
 
 
 class CanvasEvents(SignalGroup):
     lims = Signal(Rect)
     drawn = Signal()
 
 
-class CanvasBase(ABC):
-    """Base class for any canvas object."""
-
+class CanvasNDBase(ABC):
     title = _ns.TitleNamespace()
     x = _ns.XAxisNamespace()
     y = _ns.YAxisNamespace()
-    dims = Dims()
     layers = _ll.LayerList()
-    overlays = _ll.LayerList()
-    mouse = _ns.MouseNamespace()
     events: CanvasEvents
 
     def __init__(self, palette: ColormapType | None = None):
         if palette is None:
             palette = theme.get_theme().palette
-        self._color_palette = ColorPalette(palette)
         self.events = CanvasEvents()
+        self._color_palette = ColorPalette(palette)
         self._is_grouping = False
+
+    @abstractmethod
+    def _get_backend(self) -> Backend:
+        """Return the backend."""
+
+    @abstractmethod
+    def _canvas(self) -> protocols.CanvasProtocol:
+        """Return the canvas object."""
+
+    @abstractmethod
+    def _autoscale_for_layer(self, layer: _l.Layer):
+        """Autoscale the canvas for the given layer."""
+
+    def _draw_canvas(self):
+        self._canvas()._plt_draw()
+        self.events.drawn.emit()
+
+    def _coerce_name(self, name: str | None, default: str = "data") -> str:
+        if name is None:
+            basename = default
+            name = f"{default}-0"
+        else:
+            basename = name
+        i = 0
+        _exists = {layer.name for layer in self.layers}
+        while name in _exists:
+            name = f"{basename}-{i}"
+            i += 1
+        return name
+
+    def _cb_inserted(self, idx: int, layer: _l.Layer):
+        if self._is_grouping:
+            # this happens when the grouped layer is inserted
+            layer._connect_canvas(self)
+            return
+
+        _canvas = self._canvas()
+        for l in _iter_layers(layer):
+            _canvas._plt_add_layer(l._backend)
+            l._connect_canvas(self)
+
+        if isinstance(layer, _l.LayerWrapper):
+            # TODO: check if connecting LayerGroup is necessary
+            layer._connect_canvas(self)
+        # autoscale
+        self._autoscale_for_layer(layer)
+        self._cb_reordered()
+
+    def _cb_reordered(self):
+        layer_backends = []
+        for layer in self.layers:
+            if isinstance(layer, _l.PrimitiveLayer):
+                layer_backends.append(layer._backend)
+            elif isinstance(layer, _l.LayerGroup):
+                for child in layer.iter_primitive():
+                    layer_backends.append(child._backend)
+            elif isinstance(layer, _l.LayerWrapper):
+                for child in _iter_layers(layer):
+                    layer_backends.append(child._backend)
+            else:
+                raise RuntimeError(f"type {type(layer)} not expected")
+        self._canvas()._plt_reorder_layers(layer_backends)
+
+    def _cb_removed(self, idx: int, layer: _l.Layer):
+        if self._is_grouping:
+            return
+        _canvas = self._canvas()
+        for l in _iter_layers(layer):
+            _canvas._plt_remove_layer(l._backend)
+            l._disconnect_canvas(self)
+
+    def _cb_layer_grouped(self, group: _l.LayerGroup):
+        indices: list[int] = []  # layers to remove
+        not_found: list[_l.PrimitiveLayer] = []  # primitive layers to add
+        id_exists = set(map(id, self.layers.iter_primitives()))
+        for layer in group.iter_children():
+            try:
+                idx = self.layers.index(layer)
+                indices.append(idx)
+            except ValueError:
+                not_found.extend(_iter_layers(layer))
+        if not indices:
+            return
+        self._is_grouping = True
+        try:
+            for idx in reversed(indices):
+                # remove from the layer list since it is directly grouped
+                self.layers.pop(idx)
+            self.layers.append(group)
+            _canvas = self._canvas()
+            for child in not_found:
+                if id(child) in id_exists:
+                    # skip since it is already in the canvas
+                    continue
+                child._connect_canvas(self)
+                _canvas._plt_add_layer(child._backend)
+        finally:
+            self._is_grouping = False
+        self._cb_reordered()
+        self._autoscale_for_layer(group)
+
+    def _generate_colors(self, color: ColorType | None) -> Color:
+        if color is None:
+            color = self._color_palette.next()
+        return color
+
+    @property
+    def autoscale_enabled(self) -> bool:
+        """Return whether autoscale is enabled."""
+        return self._autoscale_enabled
+
+    @autoscale_enabled.setter
+    def autoscale_enabled(self, enabled: bool):
+        if not isinstance(enabled, bool):
+            raise TypeError(f"Expected a bool, got {type(enabled)}.")
+        self._autoscale_enabled = enabled
+
+    @contextmanager
+    def autoscale_context(self, enabled: bool):
+        """Context manager to temporarily change the autoscale state."""
+        _was_enabled = self.autoscale_enabled
+        self.autoscale_enabled = enabled
+        try:
+            yield
+        finally:
+            self.autoscale_enabled = _was_enabled
+
+
+class CanvasBase(CanvasNDBase):
+    """Base class for any canvas object."""
+
+    dims = Dims()
+    overlays = _ll.LayerList()
+    mouse = _ns.MouseNamespace()
+
+    def __init__(self, palette: ColormapType | None = None):
+        super().__init__(palette)
         self._autoscale_enabled = True
         if not self._get_backend().is_dummy():
             self._init_canvas()
 
     def _init_canvas(self):
         # default colors and font
         _t = theme.get_theme()
@@ -177,47 +309,14 @@
             "`canvas.mouse.double_clicked` instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.mouse.clicked
 
     @property
-    def autoscale_enabled(self) -> bool:
-        """Return whether autoscale is enabled."""
-        return self._autoscale_enabled
-
-    @autoscale_enabled.setter
-    def autoscale_enabled(self, enabled: bool):
-        if not isinstance(enabled, bool):
-            raise TypeError(f"Expected a bool, got {type(enabled)}.")
-        self._autoscale_enabled = enabled
-
-    @contextmanager
-    def autoscale_context(self, enabled: bool):
-        """Context manager to temporarily change the autoscale state."""
-        _was_enabled = self.autoscale_enabled
-        self.autoscale_enabled = enabled
-        try:
-            yield
-        finally:
-            self.autoscale_enabled = _was_enabled
-
-    @abstractmethod
-    def _get_backend(self) -> Backend:
-        """Return the backend."""
-
-    @abstractmethod
-    def _canvas(self) -> protocols.CanvasProtocol:
-        """Return the canvas object."""
-
-    def _draw_canvas(self):
-        self._canvas()._plt_draw()
-        self.events.drawn.emit()
-
-    @property
     def native(self) -> Any:
         """Return the native canvas object."""
         return self._canvas()._plt_get_native()
 
     @property
     def aspect_ratio(self) -> float | None:
         """Aspect ratio of the canvas (None if not locked)."""
@@ -389,27 +488,34 @@
         with self.events.lims.blocked():
             self.x.lim = xmin, xmax
             self.y.lim = ymin, ymax
         self.events.lims.emit(Rect(xmin, xmax, ymin, ymax))
 
     def update_axes(
         self,
-        visible: bool = _void,
-        color: ColorType | None = _void,
+        *,
+        visible: bool | None = None,
+        color: ColorType | None = None,
     ):
-        if visible is not _void:
-            self.x.ticks.visible = visible
-            self.y.ticks.visible = visible
-        if color is not _void:
-            self.x.color = color
-            self.x.ticks.color = color
-            self.x.label.color = color
-            self.y.color = color
-            self.y.ticks.color = color
-            self.y.label.color = color
+        """
+        Update axes appearance.
+
+        Parameters
+        ----------
+        visible : bool, optional
+            Whether to show the axes.
+        color : color-like, optional
+            Color of the axes.
+        """
+        if visible is not None:
+            self.x.ticks.visible = self.y.ticks.visible = visible
+        if color is not None:
+            self.x.color = self.y.color = color
+            self.x.ticks.color = self.y.ticks.color = color
+            self.x.label.color = self.y.label.color = color
         return self
 
     def update_labels(
         self,
         title: str | None = None,
         x: str | None = None,
         y: str | None = None,
@@ -429,37 +535,37 @@
         if y is not None:
             self.y.label.text = y
             self.y.label.visible = True
         return self
 
     def update_font(
         self,
-        size: float | _Void = _void,
-        color: ColorType | _Void = _void,
-        family: str | _Void = _void,
+        size: float | None = None,
+        color: ColorType | None = None,
+        family: str | None = None,
     ) -> Self:
         """
         Update all the fonts, including the title, x/y labels and x/y tick labels.
 
         Parameters
         ----------
         size : float, optional
             New font size.
         color : color-like, optional
             New font color.
         family : str, optional
             New font family.
         """
-        if size is not _void:
+        if size is not None:
             self.title.size = self.x.label.size = self.y.label.size = size
             self.x.ticks.size = self.y.ticks.size = size
-        if family is not _void:
+        if family is not None:
             self.title.family = self.x.label.family = self.y.label.family = family
             self.x.ticks.family = self.y.ticks.family = family
-        if color is not _void:
+        if color is not None:
             self.title.color = self.x.label.color = self.y.label.color = color
             self.x.ticks.color = self.y.ticks.color = color
         return self
 
     def cat(
         self,
         data: _DF,
@@ -767,15 +873,15 @@
 
         Returns
         -------
         Line
             The line layer.
         """
         xdata, ydata = normalize_xy(*args)
-        name = self._coerce_name(_l.Line, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         width = theme._default("line.width", width)
         style = theme._default("line.style", style)
         layer = _l.Line(
             xdata, ydata, name=name, color=color, width=width, style=style,
             alpha=alpha, antialias=antialias, backend=self._get_backend(),
         )  # fmt: skip
@@ -832,15 +938,15 @@
 
         Returns
         -------
         Markers
             The markers layer.
         """
         xdata, ydata = normalize_xy(*args)
-        name = self._coerce_name(_l.Markers, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         symbol = theme._default("markers.symbol", symbol)
         size = theme._default("markers.size", size)
         hatch = theme._default("markers.hatch", hatch)
         layer = _l.Markers(
             xdata, ydata, name=name, symbol=symbol, size=size, color=color,
             alpha=alpha, hatch=hatch, backend=self._get_backend(),
@@ -907,15 +1013,15 @@
             The bars layer.
         """
         center, height = normalize_xy(*args)
         if bottom is not None:
             bottom = as_array_1d(bottom)
             if bottom.shape != height.shape:
                 raise ValueError("Expected bottom to have the same shape as height")
-        name = self._coerce_name(_l.Bars, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         extent = theme._default("bars.extent", extent)
         hatch = theme._default("bars.hatch", hatch)
         layer = _l.Bars(
             center, height, bottom, extent=extent, name=name, orient=orient,
             color=color, alpha=alpha, hatch=hatch, backend=self._get_backend(),
         )  # fmt: skip
@@ -963,15 +1069,15 @@
             Color of the bars.
 
         Returns
         -------
         Bars
             The bars layer that represents the histogram.
         """
-        name = self._coerce_name("histogram", name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         width = theme._default("line.width", width)
         style = theme._default("line.style", style)
         layer = _lg.Histogram.from_array(
             data, bins=bins, limits=limits, shape=shape, kind=kind, name=name,
             color=color, width=width, style=style, orient=orient,
             backend=self._get_backend(),
@@ -1037,15 +1143,15 @@
         coords: ArrayLike,
         *,
         name=None,
         color: ColorType | None = None,
         alpha: float = 1.0,
         hatch: str | Hatch | None = None,
     ) -> _l.Rects[_mixin.ConstFace, _mixin.ConstEdge]:
-        name = self._coerce_name(_l.Rects, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         hatch = theme._default("bars.hatch", hatch)
         layer = _l.Rects(
             coords, name=name, color=color, alpha=alpha, hatch=hatch,
             backend=self._get_backend()
         )  # fmt: skip
         return self.add_layer(layer)
@@ -1087,15 +1193,15 @@
             Antialiasing of the line.
 
         Returns
         -------
         Line
             The line layer that represents the CDF.
         """
-        name = self._coerce_name("histogram", name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         width = theme._default("line.width", width)
         style = theme._default("line.style", style)
         layer = _l.Line.build_cdf(
             data, orient=orient, name=name, color=color, width=width, style=style,
             alpha=alpha, antialias=antialias, backend=self._get_backend(),
         )  # fmt: skip
@@ -1138,22 +1244,81 @@
             Pattern of the bar faces.
 
         Returns
         -------
         Spans
             The spans layer.
         """
-        name = self._coerce_name("histogram", name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         layer = _l.Spans(
             spans, name=name, orient=orient, color=color, alpha=alpha,
             hatch=hatch, backend=self._get_backend(),
         )  # fmt: skip
         return self.add_layer(layer)
 
+    def add_vectors(
+        self,
+        x: ArrayLike1D,
+        y: ArrayLike1D,
+        vx: ArrayLike1D,
+        vy: ArrayLike1D,
+        *,
+        name: str | None = None,
+        color: ColorType | None = None,
+        width: float | None = None,
+        style: LineStyle | str | None = None,
+        alpha: float = 1.0,
+        antialias: bool = True,
+    ) -> _l.Vectors:
+        """
+        Add a vector field to the canvas.
+
+        >>> canvas.add_vectors(x, y, vx, vy)
+
+        Parameters
+        ----------
+        x : array-like
+            X coordinates of the vectors.
+        y : array-like
+            Y coordinates of the vectors.
+        vx : array-like
+            X components of the vectors.
+        vy : array-like
+            Y components of the vectors.
+        name : str, optional
+            Name of the layer.
+        color : color-like, optional
+            Color of the bars.
+        width : float, optional
+            Line width. Use the theme default if not specified.
+        style : str or LineStyle, optional
+            Line style. Use the theme default if not specified.
+        alpha : float, default 1.0
+            Alpha channel of the line.
+        antialias : bool, default True
+            Antialiasing of the line.
+
+        Returns
+        -------
+        Vectors
+            The vectors layer.
+        """
+        name = self._coerce_name(name)
+        color = self._generate_colors(color)
+        width = theme._default("line.width", width)
+        style = theme._default("line.style", style)
+        layer = _l.Vectors(
+            as_array_1d(x, dtype=np.float32), as_array_1d(y, dtype=np.float32),
+            as_array_1d(vx, dtype=np.float32), as_array_1d(vy, dtype=np.float32),
+            name=name, color=color, width=width, style=style,
+            alpha=alpha, antialias=antialias, backend=self._get_backend(),
+        )  # fmt: skip
+        return self.add_layer(layer)
+
     def add_infline(
         self,
         pos: tuple[float, float] = (0, 0),
         angle: float = 0.0,
         *,
         name: str | None = None,
         color: ColorType | None = None,
@@ -1190,15 +1355,15 @@
             Antialiasing of the line.
 
         Returns
         -------
         InfLine
             The infline layer.
         """
-        name = self._coerce_name(_l.InfLine, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         width = theme._default("line.width", width)
         style = theme._default("line.style", style)
         layer = _l.InfLine(
             pos, angle, name=name, color=color, alpha=alpha,
             width=width, style=style, antialias=antialias,
             backend=self._get_backend(),
@@ -1244,15 +1409,15 @@
             Antialiasing of the line.
 
         Returns
         -------
         InfCurve
             The infcurve layer.
         """
-        name = self._coerce_name(_l.InfCurve, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         width = theme._default("line.width", width)
         style = theme._default("line.style", style)
         layer = _l.InfCurve(
             model, bounds=bounds, name=name, color=color, width=width, alpha=alpha,
             style=style, antialias=antialias, backend=self._get_backend(),
         )  # fmt: skip
@@ -1376,15 +1541,15 @@
             Hatch of the band face.
 
         Returns
         -------
         Band
             The band layer.
         """
-        name = self._coerce_name(_l.Band, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         layer = _l.Band(
             xdata, ylow, yhigh, name=name, orient=orient, color=color,
             alpha=alpha, hatch=hatch, backend=self._get_backend(),
         )  # fmt: skip
         return self.add_layer(layer)
 
@@ -1433,15 +1598,15 @@
             Size of the caps of the error indicators
 
         Returns
         -------
         Errorbars
             The errorbars layer.
         """
-        name = self._coerce_name(_l.Errorbars, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         width = theme._default("line.width", width)
         style = theme._default("line.style", style)
         layer = _l.Errorbars(
             xdata, ylow, yhigh, name=name, color=color, width=width,
             style=style, antialias=antialias, capsize=capsize, alpha=alpha,
             orient=orient, backend=self._get_backend(),
@@ -1498,15 +1663,15 @@
             Antialiasing of the line.
 
         Returns
         -------
         Rug
             The rug layer.
         """
-        name = self._coerce_name(_l.Errorbars, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         layer = _l.Rug(
             events, low=low, high=high, name=name, color=color, alpha=alpha,
             width=width, style=style, antialias=antialias, orient=orient,
             backend=self._get_backend(),
         )  # fmt: skip
         return self.add_layer(layer)
@@ -1546,15 +1711,15 @@
             Line style of the outline.
 
         Returns
         -------
         Kde
             The KDE layer.
         """
-        name = self._coerce_name(_lg.Kde, name)
+        name = self._coerce_name(name)
         color = self._generate_colors(color)
         width = theme._default("line.width", width)
         style = theme._default("line.style", style)
 
         layer = _lg.Kde.from_array(
             data, bottom=bottom, scale=1, band_width=band_width, name=name,
             orient=orient, color=color, width=width, style=style,
@@ -1777,28 +1942,14 @@
         """
         if more_layers:
             if not isinstance(layers, _l.Layer):
                 raise TypeError("No overload matches the arguments")
             layers = [layers, *more_layers]
         return _lg.LayerTuple(layers, name=name)
 
-    def _coerce_name(self, layer_type: type[_l.Layer] | str, name: str | None) -> str:
-        if name is None:
-            if isinstance(layer_type, str):
-                name = layer_type
-            else:
-                name = layer_type.__name__.lower()
-        basename = name
-        i = 0
-        _exists = {layer.name for layer in self.layers}
-        while name in _exists:
-            name = f"{basename}-{i}"
-            i += 1
-        return name
-
     def _autoscale_for_layer(
         self,
         layer: _l.Layer,
         pad_rel: float | None = None,
         maybe_empty: bool = True,
     ):
         """This function will be called when a layer is inserted to the canvas."""
@@ -1847,32 +1998,14 @@
                 or not layer._ATTACH_TO_AXIS
                 or getattr(layer, "orient", None) is not Orientation.VERTICAL
             ):
                 ymin -= dy
             ymax += dy
         self.lims = xmin, xmax, ymin, ymax
 
-    def _cb_inserted(self, idx: int, layer: _l.Layer):
-        if self._is_grouping:
-            # this happens when the grouped layer is inserted
-            layer._connect_canvas(self)
-            return
-
-        _canvas = self._canvas()
-        for l in _iter_layers(layer):
-            _canvas._plt_add_layer(l._backend)
-            l._connect_canvas(self)
-
-        if isinstance(layer, _l.LayerWrapper):
-            # TODO: check if connecting LayerGroup is necessary
-            layer._connect_canvas(self)
-        # autoscale
-        self._autoscale_for_layer(layer)
-        self._cb_reordered()
-
     def _cb_overlay_inserted(self, idx: int, layer: _l.Layer):
         _canvas = self._canvas()
         fn = self._get_backend().get("as_overlay")
         for l in _iter_layers(layer):
             _canvas._plt_add_layer(l._backend)
             fn(l._backend, _canvas)
             l._connect_canvas(self)
@@ -1886,29 +2019,14 @@
         if self._is_grouping:
             return
         _canvas = self._canvas()
         for l in _iter_layers(layer):
             _canvas._plt_remove_layer(l._backend)
             l._disconnect_canvas(self)
 
-    def _cb_reordered(self):
-        layer_backends = []
-        for layer in self.layers:
-            if isinstance(layer, _l.PrimitiveLayer):
-                layer_backends.append(layer._backend)
-            elif isinstance(layer, _l.LayerGroup):
-                for child in layer.iter_primitive():
-                    layer_backends.append(child._backend)
-            elif isinstance(layer, _l.LayerWrapper):
-                for child in _iter_layers(layer):
-                    layer_backends.append(child._backend)
-            else:
-                raise RuntimeError(f"type {type(layer)} not expected")
-        self._canvas()._plt_reorder_layers(layer_backends)
-
     def _cb_layer_grouped(self, group: _l.LayerGroup):
         indices: list[int] = []  # layers to remove
         not_found: list[_l.PrimitiveLayer] = []  # primitive layers to add
         id_exists = set(map(id, self.layers.iter_primitives()))
         for layer in group.iter_children():
             try:
                 idx = self.layers.index(layer)
```

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_between.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_between.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_dims.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_dims.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,20 +68,18 @@
 
     @property
     def names(self) -> list[str]:
         """Names of the dimensions."""
         return [a.name for a in self._axes]
 
     @overload
-    def axis(self, name: str) -> DimAxis:
-        ...
+    def axis(self, name: str) -> DimAxis: ...
 
     @overload
-    def axis(self, name: str, *, default: _T) -> DimAxis | _T:
-        ...
+    def axis(self, name: str, *, default: _T) -> DimAxis | _T: ...
 
     def axis(self, name, *, default=_default):
         """Get the axis by name."""
         for a in self._axes:
             if a.name == name:
                 return a
         if default is _default:
@@ -90,28 +88,24 @@
 
     @property
     def indices(self) -> dict[str, SupportsIndex]:
         """Current indices for each dimension."""
         return {a.name: a.value() for a in self._axes}
 
     @overload
-    def set_indices(self, arg: dict[str, SupportsIndex]):
-        ...
+    def set_indices(self, arg: dict[str, SupportsIndex]): ...
 
     @overload
-    def set_indices(self, arg: Sequence[SupportsIndex]):
-        ...
+    def set_indices(self, arg: Sequence[SupportsIndex]): ...
 
     @overload
-    def set_indices(self, arg: SupportsIndex):
-        ...
+    def set_indices(self, arg: SupportsIndex): ...
 
     @overload
-    def set_indices(self, **kwargs: SupportsIndex):
-        ...
+    def set_indices(self, **kwargs: SupportsIndex): ...
 
     def set_indices(self, arg=None, **kwargs: Any):
         """
         Set current indices and update the canvas.
 
         Either of the following forms are allowed:
         >>> canvas.dims.set_indices(axis_0=3, axis_1=4)
@@ -344,15 +338,15 @@
 
         Returns
         -------
         XYLayerStack
             Layer stack of a line layer.
         """
         canvas = self._get_canvas()
-        name = canvas._coerce_name(_l.Line, name)
+        name = canvas._coerce_name(name)
         color = canvas._generate_colors(color)
         stack = _ndl.XYLayerStack.from_layer_class(
             _l.Line, xdata, ydata, name=name, color=color, width=width, style=style,
             alpha=alpha, antialias=antialias, backend=canvas._get_backend(),
         )  # fmt: skip
         return self._add_layer(stack)
 
@@ -364,15 +358,15 @@
         name: str | None = None,
         color: ColorType | None = None,
         hatch: str | Hatch = Hatch.SOLID,
         symbol: str | Symbol = Symbol.CIRCLE,
         size: float = 5.0,
     ) -> _ndl.XYLayerStack:
         canvas = self._get_canvas()
-        name = canvas._coerce_name(_l.Markers, name)
+        name = canvas._coerce_name(name)
         color = canvas._generate_colors(color)
         stack = _ndl.XYLayerStack.from_layer_class(
             _l.Markers, xdata, ydata, name=name, color=color, hatch=hatch,
             symbol=symbol, size=size, backend=canvas._get_backend(),
         )  # fmt: skip
         return self._add_layer(stack)
 
@@ -401,15 +395,15 @@
 
         Returns
         -------
         XYYLayerStack
             Layer stack of a band layer.
         """
         canvas = self._get_canvas()
-        name = canvas._coerce_name(_l.Band, name)
+        name = canvas._coerce_name(name)
         color = canvas._generate_colors(color)
         stack = _ndl.XYYLayerStack.from_layer_class(
             _l.Band, xdata, ylow, yhigh, name=name, color=color, hatch=hatch,
             alpha=alpha, backend=canvas._get_backend(),
         )  # fmt: skip
         return self._add_layer(stack)
 
@@ -441,15 +435,15 @@
 
         Returns
         -------
         XYYLayerStack
             Layer stack of an errorbars layer.
         """
         canvas = self._get_canvas()
-        name = canvas._coerce_name(_l.Errorbars, name)
+        name = canvas._coerce_name(name)
         color = canvas._generate_colors(color)
         stack = _ndl.XYYLayerStack.from_layer_class(
             _l.Errorbars, xdata, ylow, yhigh, name=name, orient=orient, color=color,
             width=width, style=style, antialias=antialias, capsize=capsize,
             backend=canvas._get_backend(),
         )  # fmt: skip
         return self._add_layer(stack)
@@ -478,15 +472,15 @@
 
         Returns
         -------
         YLayerStack
             Layer stack of a rug layer.
         """
         canvas = self._get_canvas()
-        name = canvas._coerce_name(_l.Rug, name)
+        name = canvas._coerce_name(name)
         color = canvas._generate_colors(color)
         stack = _ndl.YLayerStack.from_layer_class(
             _l.Rug, events, low=low, high=high, name=name, orient=orient,
             color=color,  width=width,  style=style, antialias=antialias,
             alpha=alpha, backend=canvas._get_backend(),
         )  # fmt: skip
         return self._add_layer(stack)
@@ -518,15 +512,15 @@
 
         Returns
         -------
         TextLayerStack
             Layer stack of text layers.
         """
         canvas = self._get_canvas()
-        name = canvas._coerce_name(_l.Texts, name)
+        name = canvas._coerce_name(name)
         stack = _ndl.TextLayerStack.from_layer_class(
             _l.Texts, xdata, ydata, string, name=name, color=color, size=size,
             rotation=rotation, anchor=anchor, family=family,
             backend=canvas._get_backend(),
         )  # fmt: skip
         return self._add_layer(stack)
 
@@ -554,15 +548,15 @@
 
         Returns
         -------
         ImageLayerStack
             Layer stack of image layers.
         """
         canvas = self._get_canvas()
-        name = canvas._coerce_name(_l.Image, name)
+        name = canvas._coerce_name(name)
         stack = _ndl.ImageLayerStack.from_layer_class(
             _l.Image, image, name=name, cmap=cmap, clim=clim, rgb=rgb,
             backend=canvas._get_backend(),
         )  # fmt: skip
         self._add_layer(stack)
 
         if flip_canvas and not canvas.y.flipped:
```

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_fit.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_fit.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_grid.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,48 @@
         if self._x_linked:
             self._x_linker_ref.link(canvas.x)
         if self._y_linked:
             self._y_linker_ref.link(canvas.y)
         canvas.events.drawn.connect(self.events.drawn.emit, unique=True, max_args=None)
         return canvas
 
+    def add_canvas_3d(
+        self,
+        row: int,
+        col: int,
+        rowspan: int = 1,
+        colspan: int = 1,
+        *,
+        palette: str | None = None,
+    ):
+        """Add a canvas to the grid at the given position"""
+        from whitecanvas.canvas.canvas3d._base import Canvas3D
+
+        for idx, item in np.ndenumerate(self._canvas_array[row, col]):
+            if item is not None:
+                raise ValueError(f"Canvas already exists at {idx}")
+        backend_canvas = self._backend_object._plt_add_canvas_3d(
+            row, col, rowspan, colspan
+        )
+        canvas = self._canvas_array[row, col] = Canvas3D.from_backend(
+            backend_canvas,
+            backend=self._backend,
+            palette=palette,
+        )
+        # Now backend axes/viewbox are created, we can install mouse events
+        # canvas._install_mouse_events()
+
+        # link axes if needed
+        if self._x_linked:
+            self._x_linker_ref.link(canvas.x)
+        if self._y_linked:
+            self._y_linker_ref.link(canvas.y)
+        canvas.events.drawn.connect(self.events.drawn.emit, unique=True, max_args=None)
+        return canvas
+
     def _iter_add_canvas(self, **kwargs) -> Iterator[Canvas]:
         for row in range(len(self._heights)):
             for col in range(len(self._widths)):
                 yield self.add_canvas(row, col, **kwargs)
 
     def _iter_canvas(self) -> Iterator[tuple[tuple[int, int], Canvas]]:
         yielded: set[int] = set()
```

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_imageref.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_imageref.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_joint.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_joint.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         """Create a joint categorical canvas."""
         from whitecanvas.canvas.dataframe import JointCatPlotter
 
         return JointCatPlotter(self, data, x, y, update_labels=update_labels)
 
     def _link_marginal_to_main(self, layer: _l.Layer, main: _l.Layer) -> None:
         # TODO: this is not the only thing to be done
-        main.events.visible.connect_setattr(layer, "visible")
+        main.events.visible.connect_setattr(layer, "visible", maxargs=1)
 
     def add_legend(
         self,
         layers: Sequence[str | _l.Layer] | None = None,
         location: Location | LocationStr = "top_right",
         *,
         title: str | None = None,
@@ -441,39 +441,36 @@
     @abstractmethod
     def add_layer_for_markers(
         self,
         data: ArrayLike1D,
         color: ColorType,
         hatch: Hatch = Hatch.SOLID,
         backend: str | Backend | None = None,
-    ) -> _l.Layer:
-        ...
+    ) -> _l.Layer: ...
 
     @abstractmethod
     def add_layer_for_cat_markers(
         self,
         df: DataFrameWrapper[_DF],
         value: str,
         color: NStr | None = None,
         hatch: NStr | None = None,
         backend: str | Backend | None = None,
-    ) -> _l.Layer:
-        ...
+    ) -> _l.Layer: ...
 
     @abstractmethod
     def add_layer_for_cat_hist2d(
         self,
         df: DataFrameWrapper[_DF],
         value: str,
         color: str | None = None,
         bins: HistBinType | tuple[HistBinType, HistBinType] = "auto",
         limits: tuple[float, float] | None = None,
         backend: str | Backend | None = None,
-    ) -> _l.Layer:
-        ...
+    ) -> _l.Layer: ...
 
 
 class MarginalHistPlotter(MarginalPlotter):
     def __init__(
         self,
         orient: OrientationLike,
         bins: HistBinType = "auto",
```

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_linker.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_linker.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_namespaces.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_namespaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,18 @@
         l = self._canvas_ref()
         if l is None:
             raise ReferenceDeletedError("Canvas has been deleted.")
         elif l is _no_canvas:
             raise TypeError("No canvas is associated with the class itself.")
         return l._canvas()
 
+    def _draw_canvas(self):
+        if canvas := self._canvas_ref():
+            canvas._draw_canvas()
+
     def __repr__(self) -> str:
         cname = type(self).__name__
         l = self._canvas_ref()
         if l is None:
             return f"<{cname} of deleted canvas>"
         elif l is _no_canvas:
             return f"<{cname}>"
@@ -259,14 +263,19 @@
 
 
 class YTickNamespace(_TicksNamespace):
     def _get_object(self):
         return self._get_canvas()._plt_get_yticks()
 
 
+class ZTickNamespace(_TicksNamespace):
+    def _get_object(self):
+        return self._get_canvas()._plt_get_zticks()
+
+
 class TitleNamespace(_TextLabelNamespace):
     def _get_object(self):
         return self._get_canvas()._plt_get_title()
 
 
 class XLabelNamespace(_TextLabelNamespace):
     def _get_object(self):
@@ -274,14 +283,19 @@
 
 
 class YLabelNamespace(_TextLabelNamespace):
     def _get_object(self):
         return self._get_canvas()._plt_get_ylabel()
 
 
+class ZLabelNamespace(_TextLabelNamespace):
+    def _get_object(self):
+        return self._get_canvas()._plt_get_zlabel()
+
+
 class AxisNamespace(Namespace):
     events: AxisSignals
     _attrs = ("lim", "color", "flipped")
 
     def __init__(self, canvas: CanvasBase | None = None):
         super().__init__(canvas)
         self.events = AxisSignals()
@@ -316,14 +330,15 @@
     def color(self):
         """Color of the axis."""
         return self._get_object()._plt_get_color()
 
     @color.setter
     def color(self, color):
         self._get_object()._plt_set_color(np.array(Color(color)))
+        self._draw_canvas()
 
     @property
     def flipped(self) -> bool:
         """Return true if the axis is flipped."""
         return self._flipped
 
     @flipped.setter
@@ -359,14 +374,22 @@
     label = YLabelNamespace()
     ticks = YTickNamespace()
 
     def _get_object(self):
         return self._get_canvas()._plt_get_yaxis()
 
 
+class ZAxisNamespace(AxisNamespace):
+    label = ZLabelNamespace()
+    ticks = ZTickNamespace()
+
+    def _get_object(self):
+        return self._get_canvas()._plt_get_zaxis()
+
+
 class MouseNamespace(AxisNamespace):
     """Namespace that contains the mouse events."""
 
     clicked = MouseSignal(object)
     """Signal emitted when a mouse button is clicked."""
 
     moved = MouseMoveSignal()
```

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_palette.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_palette.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/_stacked.py` & `whitecanvas-0.3.0/whitecanvas/canvas/_stacked.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/layerlist.py` & `whitecanvas-0.3.0/whitecanvas/canvas/layerlist.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_base.py` & `whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_both_cat.py` & `whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_both_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_feature_cat.py` & `whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_feature_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_joint_cat.py` & `whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_joint_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_one_cat.py` & `whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_one_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_stacked_cat.py` & `whitecanvas-0.3.0/whitecanvas/canvas/dataframe/_stacked_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/__init__.py` & `whitecanvas-0.3.0/whitecanvas/layers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Line,
     Markers,
     MultiLine,
     Rects,
     Rug,
     Spans,
     Texts,
+    Vectors,
 )
 
 __all__ = [
     "Layer",
     "PrimitiveLayer",
     "DataBoundLayer",
     "LayerGroup",
@@ -38,8 +39,9 @@
     "Band",
     "Rug",
     "InfLine",
     "InfCurve",
     "Texts",
     "Rects",
     "Image",
+    "Vectors",
 ]
```

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_base.py` & `whitecanvas-0.3.0/whitecanvas/layers/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import weakref
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Generic, Iterable, Iterator, TypeVar
 
 import numpy as np
 from numpy.typing import NDArray
 from psygnal import Signal, SignalGroup
 
 from whitecanvas.backend import Backend
@@ -25,31 +25,36 @@
 class LayerEvents(SignalGroup):
     data = Signal(check_nargs_on_connect=False)  # (data)
     name = Signal(str)
     visible = Signal(bool)
     _layer_grouped = Signal(object)  # (group)
 
 
+def _no_ref() -> None:
+    return None
+
+
 class Layer(ABC):
     events: LayerEvents
     _events_class: type[LayerEvents]
     _ATTACH_TO_AXIS = False
     _NO_PADDING_NEEDED = False
 
     def __init__(self, name: str | None = None):
         if not hasattr(self.__class__, "_events_class"):
             self.events = LayerEvents()
         else:
             self.events = self.__class__._events_class()
         self._name = name if name is not None else self.__class__.__name__
         self._x_hint = self._y_hint = None
         self._group_layer_ref: weakref.ReferenceType[LayerGroup] | None = None
-        self._canvas_ref = lambda: None
+        self._canvas_ref = _no_ref
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def visible(self) -> bool:
         """Return true if the layer is visible"""
 
     @visible.setter
     def visible(self, visible: bool):
         """Set the visibility of the layer"""
 
@@ -74,15 +79,15 @@
         self.events.connect(canvas._draw_canvas, unique=True, max_args=0)
         self._canvas_ref = weakref.ref(canvas)
 
     def _disconnect_canvas(self, canvas: CanvasBase):
         """If needed, do something when layer is removed from a canvas."""
         self.events._layer_grouped.disconnect(canvas._cb_layer_grouped)
         self.events.disconnect(canvas._draw_canvas)
-        self._canvas_ref = lambda: None
+        self._canvas_ref = _no_ref
 
     def _canvas(self) -> CanvasBase:
         canvas = self._canvas_ref()
         if canvas is None:
             raise ValueError("Layer is not in any canvas.")
         return canvas
 
@@ -103,15 +108,15 @@
 
 
 class PrimitiveLayer(Layer, Generic[_P]):
     """Layers that are composed of a single component."""
 
     _backend: _P
     _backend_name: str
-    _backend_class_name = None
+    _backend_class_name: str | None = None
 
     @property
     def visible(self) -> bool:
         """Return true if the layer is visible"""
         return self._backend._plt_get_visible()
 
     @visible.setter
@@ -119,16 +124,23 @@
         """Set the visibility of the layer"""
         self._backend._plt_set_visible(visible)
         self.events.visible.emit(visible)
 
     def _create_backend(self, backend: Backend, *args) -> _P:
         """Create a backend object."""
         if self._backend_class_name is not None:
-            self._backend_name = backend.name
-            return backend.get(self._backend_class_name)(*args)
+            if "." not in self._backend_class_name:
+                backend_cls_name = self._backend_class_name
+                self._backend_name = backend.name
+                return backend.get(backend_cls_name)(*args)
+            else:
+                _mod, _cls = self._backend_class_name.rsplit(".")
+                backend_cls = getattr(backend.get_submodule(_mod), _cls)
+                self._backend_name = backend.name
+                return backend_cls(*args)
         for mro in reversed(type(self).__mro__):
             name = mro.__name__
             if (
                 issubclass(mro, PrimitiveLayer)
                 and mro is not PrimitiveLayer
                 and backend.has(name)
             ):
@@ -188,23 +200,22 @@
             raise ValueError(
                 "Expected text to have the same size as the data, "
                 f"got {len(texts)} and {self.ndata}"
             )
         self._backend._plt_set_hover_text(texts)
         return self
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def ndata(self) -> int:
         """Number of data points."""
 
 
 class LayerGroup(Layer):
-    """
-    A group of layers that will be treated as a single layer in the canvas.
-    """
+    """A group of layers that will be treated as a single layer in the canvas."""
 
     def __init__(self, name: str | None = None):
         super().__init__(name)
         self._visible = True
 
     @abstractmethod
     def iter_children(self) -> Iterator[Layer]:
```

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_legend.py` & `whitecanvas-0.3.0/whitecanvas/layers/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_mixin.py` & `whitecanvas-0.3.0/whitecanvas/layers/_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     Any,
     Generic,
     Iterable,
     Iterator,
@@ -86,48 +86,55 @@
 
 
 class FaceNamespace(LayerNamespace[PrimitiveLayer[_lp.HasFaces]]):
     _properties = ("color", "hatch")
     events: FaceEvents
     _events_class = FaceEvents
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def color(self) -> NDArray[np.floating]:
         raise NotImplementedError
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def hatch(self) -> Hatch | EnumArray[Hatch]:
         raise NotImplementedError
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def alpha(self) -> float | NDArray[np.floating]:
         raise NotImplementedError
 
     @abstractmethod
     def update(self, color=None, hatch=None, alpha=1.0): ...
 
 
 class EdgeNamespace(LayerNamespace[PrimitiveLayer[_lp.HasEdges]]):
     _properties = ("color", "style", "width")
     events: EdgeEvents
     _events_class = EdgeEvents
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def color(self) -> NDArray[np.floating]:
         raise NotImplementedError
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def width(self) -> float | NDArray[np.floating]:
         raise NotImplementedError
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def style(self) -> LineStyle | EnumArray[LineStyle]:
         raise NotImplementedError
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def alpha(self) -> float | NDArray[np.floating]:
         raise NotImplementedError
 
     @abstractmethod
     def update(self, color=None, width=None, style=None, alpha=1.0): ...
 
 
@@ -217,14 +224,17 @@
     def _as_legend_info(self):
         if self.color.size == 0:
             return _legend.EmptyLegendItem()
         color = self.color[0]
         hatch = self.hatch[0]
         return _legend.FaceInfo(color, hatch)
 
+    def _ndata(self) -> int:
+        return self._layer.ndata
+
     @property
     def alpha(self) -> float:
         return self.color[:, 3]
 
     @alpha.setter
     def alpha(self, value):
         color = self.color.copy()
@@ -255,14 +265,17 @@
         if self.color.size == 0:
             return _legend.EmptyLegendItem()
         color = self.color[0]
         width = self.width[0]
         style = self.style[0]
         return _legend.EdgeInfo(color, width, style)
 
+    def _ndata(self) -> int:
+        return self._layer.ndata
+
     @property
     def alpha(self) -> float:
         return self.color[:, 3]
 
     @alpha.setter
     def alpha(self, value):
         color = self.color.copy()
@@ -462,16 +475,16 @@
     @property
     def color(self) -> NDArray[np.floating]:
         """Face color of the bar."""
         return self._layer._backend._plt_get_face_color()
 
     @color.setter
     def color(self, color):
-        col = as_color_array(color, self._layer.ndata)
-        if self._layer.ndata > 0:
+        col = as_color_array(color, self._ndata())
+        if self._ndata() > 0:
             self._layer._backend._plt_set_face_color(col)
         self.events.color.emit(col)
 
     @property
     def hatch(self) -> EnumArray[Hatch]:
         """Face fill hatches."""
         return np.asarray(self._layer._backend._plt_get_face_hatch(), dtype=object)
@@ -480,49 +493,49 @@
     def hatch(self, hatch: str | Hatch | Iterable[str | Hatch]):
         if isinstance(hatch, str):
             hatch = Hatch(hatch)
         elif isinstance(hatch, Hatch):
             pass
         else:
             hatch = [Hatch(p) for p in hatch]
-        if self._layer.ndata > 0:
+        if self._ndata() > 0:
             self._layer._backend._plt_set_face_hatch(hatch)
         self.events.hatch.emit(hatch)
 
 
 class MultiEdge(MultiPropertyEdgeBase):
     @property
     def color(self) -> NDArray[np.floating]:
         """Edge color of the bar."""
         return self._layer._backend._plt_get_edge_color()
 
     @color.setter
     def color(self, color):
-        col = as_color_array(color, self._layer.ndata)
-        if self._layer.ndata > 0:
+        col = as_color_array(color, self._ndata())
+        if self._ndata() > 0:
             self._layer._backend._plt_set_edge_color(col)
         self.events.color.emit(col)
 
     @property
     def width(self) -> NDArray[np.floating]:
         """Edge widths."""
         return self._layer._backend._plt_get_edge_width()
 
     @width.setter
     def width(self, width: float | Iterable[float]):
         if not is_real_number(width):
             width = np.asarray(width, dtype=np.float32)
-            if width.shape != (self._layer.ndata,):
+            if width.shape != (self._ndata(),):
                 raise ValueError(
                     "Width must be a scalar or an array of length "
-                    f"{self._layer.ndata}, got {width.shape!r}"
+                    f"{self._ndata()}, got {width.shape!r}"
                 )
         else:
             width = float(width)
-        if self._layer.ndata > 0:
+        if self._ndata() > 0:
             self._layer._backend._plt_set_edge_width(width)
         self.events.width.emit(width)
 
     @property
     def style(self) -> EnumArray[LineStyle]:
         """Edge styles."""
         return np.asarray(self._layer._backend._plt_get_edge_style(), dtype=object)
@@ -531,15 +544,15 @@
     def style(self, style: str | LineStyle | Iterable[str | LineStyle]):
         if isinstance(style, str):
             style = LineStyle(style)
         elif isinstance(style, LineStyle):
             pass
         else:
             style = [LineStyle(s) for s in style]
-        if self._layer.ndata > 0:
+        if self._ndata() > 0:
             self._layer._backend._plt_set_edge_style(style)
         self.events.style.emit(style)
 
 
 _NFace = TypeVar("_NFace", bound=FaceNamespace)
 _NEdge = TypeVar("_NEdge", bound=EdgeNamespace)
 
@@ -865,19 +878,21 @@
 
 
 class FontNamespace(LayerNamespace[PrimitiveLayer[_lp.HasText]]):
     _properties = ("color", "size", "family")
     events: FontEvents
     _events_class = FontEvents
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def color(self):
         raise NotImplementedError
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def size(self):
         raise NotImplementedError
 
     @property
     def family(self):
         return self._layer._backend._plt_get_text_fontfamily()
```

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_ndim.py` & `whitecanvas-0.3.0/whitecanvas/layers/_ndim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """LayerStack represents a stack of layers for n-D visualization."""
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar
 
 import numpy as np
 from numpy.typing import NDArray
 from typing_extensions import Concatenate, ParamSpec
 
 from whitecanvas.layers import _primitive
@@ -208,15 +208,16 @@
 class Slicable(ABC, Generic[_T]):
     """A class that can generate sliced data."""
 
     @abstractmethod
     def slice_at(self, index: tuple[int, ...]) -> _T:
         """Get the sliced data at the given index."""
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def shape(self) -> tuple[int, ...]:
         """The shape of the data."""
 
     @property
     def ndim(self) -> int:
         """The number of dimensions of the data."""
         return len(self.shape)
@@ -260,16 +261,15 @@
 
 
 # TODO: multidimensional stripplot etc.
 class TableArray(Slicable[NDArray[np.number]]):
     def __init__(self, obj: dict[Any, dict[str, NDArray[np.number]]]):
         self._obj = obj
 
-    def slice_at(self, index: tuple[int, ...]):
-        ...
+    def slice_at(self, index: tuple[int, ...]): ...
 
 
 class StackedArray(Slicable[_T]):
     """A stacked Slicable objects."""
 
     def __init__(
         self,
```

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_sizehint.py` & `whitecanvas-0.3.0/whitecanvas/layers/_sizehint.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,7 +43,30 @@
     ypad = (ymax - ymin) * ypad_rel
     y_minmax = ymin - ypad, ymax + ypad
     if orient.is_vertical:
         _x_hint, _y_hint = x_minmax, y_minmax
     else:
         _x_hint, _y_hint = y_minmax, x_minmax
     return _x_hint, _y_hint
+
+
+def xyz_size_hint(
+    x: NDArray[np.number],
+    y: NDArray[np.number],
+    z: NDArray[np.number],
+    xpad_rel: float = 0.0,
+    ypad_rel: float = 0.0,
+    zpad_rel: float = 0.0,
+) -> tuple[_Hint, _Hint, _Hint]:
+    if x.size == 0:
+        return None, None, None
+    xmin, xmax = x.min(), x.max()
+    ymin, ymax = y.min(), y.max()
+    zmin, zmax = z.min(), z.max()
+    xpad = (xmax - xmin) * xpad_rel
+    ypad = (ymax - ymin) * ypad_rel
+    zpad = (zmax - zmin) * zpad_rel
+    x_minmax = x.min() - xpad, x.max() + xpad
+    y_minmax = y.min() - ypad, y.max() + ypad
+    z_minmax = z.min() - zpad, z.max() + zpad
+    _x_hint, _y_hint, _z_hint = x_minmax, y_minmax, z_minmax
+    return _x_hint, _y_hint, _z_hint
```

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_text_utils.py` & `whitecanvas-0.3.0/whitecanvas/layers/_text_utils.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/__init__.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from whitecanvas.layers._primitive.inf_curve import InfCurve, InfLine
 from whitecanvas.layers._primitive.line import Line, MultiLine
 from whitecanvas.layers._primitive.markers import Markers
 from whitecanvas.layers._primitive.rects import Rects
 from whitecanvas.layers._primitive.rug import Rug
 from whitecanvas.layers._primitive.spans import Spans
 from whitecanvas.layers._primitive.text import Texts
+from whitecanvas.layers._primitive.vectors import Vectors
 
 __all__ = [
     "Line",
     "MultiLine",
     "Bars",
     "Markers",
     "Band",
@@ -20,8 +21,9 @@
     "Errorbars",
     "Rug",
     "InfLine",
     "InfCurve",
     "Texts",
     "Image",
     "Rects",
+    "Vectors",
 ]
```

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/band.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/bars.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/bars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/errorbars.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/errorbars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/image.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/inf_curve.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/inf_curve.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/line.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/markers.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/rects.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/rects.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/rug.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/rug.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/spans.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/spans.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/_primitive/text.py` & `whitecanvas-0.3.0/whitecanvas/layers/_primitive/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/__init__.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/_collections.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/_collections.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/_offsets.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/_offsets.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/band_collection.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/band_collection.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/boxplot.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/boxplot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/colorbar.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/colorbar.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/graph.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/graph.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/labeled.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/labeled.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/line_band.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/line_band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/line_collection.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/line_collection.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/line_fill.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/line_fill.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/line_markers.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/line_markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/marker_collection.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/marker_collection.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/stemplot.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/stemplot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/group/textinfo.py` & `whitecanvas-0.3.0/whitecanvas/layers/group/textinfo.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/__init__.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_box_like.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_box_like.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_dataframe.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_dataframe.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_df_compat.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_df_compat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_jitter.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_jitter.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_marker_like.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_marker_like.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_plans.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_plans.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_shared.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_shared.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/layers/tabular/_stackable.py` & `whitecanvas-0.3.0/whitecanvas/layers/tabular/_stackable.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/plot/_canvases.py` & `whitecanvas-0.3.0/whitecanvas/plot/_canvases.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from whitecanvas.backend import Backend
-from whitecanvas.canvas import Canvas, CanvasGrid
+from whitecanvas.canvas import Canvas, CanvasGrid, SingleCanvas
 from whitecanvas.core import new_canvas, new_grid
 
 
 def current_grid() -> CanvasGrid:
     """Return the current canvas grid."""
     grid = CanvasGrid._CURRENT_INSTANCE
     if grid is None:
@@ -17,20 +17,34 @@
     """Return the current canvas."""
     canvas = Canvas._CURRENT_INSTANCE
     if canvas is None:
         canvas = new_canvas()
     return canvas
 
 
-def show(block: bool = False):
+def show(block: bool = False, flush: bool = True):
     """Show the current canvas."""
     current_grid().show(block=block)
+    if flush:
+        Canvas._CURRENT_INSTANCE = None
 
 
 def subplots(
     nrows: int = 1,
     ncols: int = 1,
-    *,
-    backend: Backend | str | None = None,
 ) -> CanvasGrid:
     """Create a new grid of subplots."""
-    return new_grid(nrows, ncols, backend=backend).fill()
+    return new_grid(nrows, ncols).fill()
+
+
+def figure(
+    *,
+    size: tuple[float, float] | None = None,
+    palette: str | None = None,
+) -> SingleCanvas:
+    """Create a new grid of subplots."""
+    return new_canvas(size=size, palette=palette)
+
+
+def use(backend: str):
+    """Set the backend to use."""
+    return Backend(backend)  # update default
```

### Comparing `whitecanvas-0.2.6/whitecanvas/protocols/__init__.py` & `whitecanvas-0.3.0/whitecanvas/protocols/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,30 @@
     CanvasGridProtocol,
     CanvasProtocol,
     HasVisibility,
     TextLabelProtocol,
     TicksProtocol,
 )
 from whitecanvas.protocols.layer_protocols import (
-    ArrowProtocol,
     BandProtocol,
     BarProtocol,
     BaseProtocol,
     ErrorbarProtocol,
     ImageProtocol,
     LineProtocol,
     MarkersProtocol,
+    MeshProtocol,
     MultiLineProtocol,
     RangeDataProtocol,
     TextProtocol,
+    VectorsProtocol,
 )
 
 __all__ = [
-    "ArrowProtocol",
+    "VectorsProtocol",
     "BaseProtocol",
     "LineProtocol",
     "MultiLineProtocol",
     "MarkersProtocol",
     "BarProtocol",
     "BandProtocol",
     "ErrorbarProtocol",
@@ -36,14 +37,15 @@
     "RangeDataProtocol",
     "CanvasProtocol",
     "CanvasGridProtocol",
     "HasVisibility",
     "TextLabelProtocol",
     "TicksProtocol",
     "AxisProtocol",
+    "MeshProtocol",
 ]
 
 _C = TypeVar("_C")
 
 
 def check_protocol(p: "type[BaseProtocol]") -> Callable[[_C], _C]:
     def _inner(c):
```

### Comparing `whitecanvas-0.2.6/whitecanvas/protocols/canvas_protocol.py` & `whitecanvas-0.3.0/whitecanvas/protocols/canvas_protocol.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/protocols/layer_protocols.py` & `whitecanvas-0.3.0/whitecanvas/protocols/layer_protocols.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any, Callable, Protocol, runtime_checkable
 
 import numpy as np
 from cmap import Colormap
 from numpy.typing import NDArray
 
-from whitecanvas.types import Alignment, Hatch, LineStyle, Orientation, Symbol
+from whitecanvas.types import Alignment, Hatch, LineStyle, MeshData, Orientation, Symbol
 
 Array1D = NDArray[np.number]
 
 
 @runtime_checkable
 class BaseProtocol(Protocol):
     def _plt_get_visible(self) -> bool:
@@ -264,20 +264,47 @@
 
 @runtime_checkable
 class TextProtocol(HasText, HasEdges, HasFaces, Protocol):
     pass
 
 
 @runtime_checkable
-class ArrowProtocol(HasEdges, Protocol):
-    def _plt_get_arrow_size(self) -> float:
-        """Return the arrow size."""
+class VectorsProtocol(XXYYDataProtocol, HasEdges, Protocol):
+    def _plt_get_antialias(self) -> bool:
+        """Return the anti alias."""
+
+    def _plt_set_antialias(self, antialias: bool):
+        """Set the anti alias."""
+
+
+@runtime_checkable
+class MeshProtocol(BaseProtocol, HasFaces, HasEdges, Protocol):
+    def _plt_get_data(self) -> MeshData:
+        """Return the mesh data."""
+
+    def _plt_set_data(self, data: MeshData):
+        """Set the mesh data."""
+
+    def _plt_get_face_color(self) -> NDArray[np.float32]:
+        """Return the face color."""
+
+    def _plt_set_face_color(self, color: NDArray[np.float32]):
+        """Set the face color."""
 
-    def _plt_set_arrow_size(self, size: float):
-        """Set the arrow size."""
+    def _plt_get_edge_color(self) -> NDArray[np.float32]:
+        """Return the edge color."""
+
+    def _plt_set_edge_color(self, color: NDArray[np.float32]):
+        """Set the edge color."""
+
+    def _plt_get_edge_width(self) -> float:
+        """Return the edge width."""
+
+    def _plt_set_edge_width(self, width: float):
+        """Set the edge width."""
 
 
 @runtime_checkable
 class ImageProtocol(BaseProtocol, Protocol):
     def _plt_get_data(self) -> NDArray[np.number]:
         """Return the image data."""
```

### Comparing `whitecanvas-0.2.6/whitecanvas/theme/_api.py` & `whitecanvas-0.3.0/whitecanvas/theme/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
-from typing import Generator
+from typing import Any, Generator
 
 from whitecanvas.theme._dataclasses import DARK_THEME, LIGHT_THEME, Theme
 
 _EXISTING_THEMES = {
     "light": LIGHT_THEME,
     "dark": DARK_THEME,
 }
@@ -23,15 +23,15 @@
     if isinstance(name, Theme):
         return name
     if name is None:
         return _DEFAULT_THEME
     return _EXISTING_THEMES[name]
 
 
-def _default(attr: str, value):
+def _default(attr: str, value) -> Any:
     if value is not None:
         return value
     out = _DEFAULT_THEME
     for a in attr.split("."):
         out = getattr(out, a)
     return out
```

### Comparing `whitecanvas-0.2.6/whitecanvas/theme/_dataclasses.py` & `whitecanvas-0.3.0/whitecanvas/theme/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/tools/_polygon_utils.py` & `whitecanvas-0.3.0/whitecanvas/tools/_polygon_utils.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/tools/_selection.py` & `whitecanvas-0.3.0/whitecanvas/tools/_selection.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/types/__init__.py` & `whitecanvas-0.3.0/whitecanvas/types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,24 @@
     MouseEventType,
     Orientation,
     OrientationLike,
     Origin,
     Symbol,
 )
 from whitecanvas.types._mouse import MouseEvent, Point
-from whitecanvas.types._tuples import Rect, XYData, XYTextData, XYYData
+from whitecanvas.types._tuples import (
+    MeshData,
+    Rect,
+    XYData,
+    XYTextData,
+    XYVectorData,
+    XYYData,
+    XYZData,
+    XYZVectorData,
+)
 
 __all__ = [
     "ColorType",
     "ColormapType",
     "ArrayLike1D",
     "LineStyle",
     "Location",
@@ -46,10 +55,14 @@
     "MouseEvent",
     "Point",
     "MouseEventType",
     "Alignment",
     "XYData",
     "XYYData",
     "XYTextData",
+    "XYZData",
+    "XYVectorData",
+    "XYZVectorData",
     "Rect",
+    "MeshData",
     "_Void",
 ]
```

### Comparing `whitecanvas-0.2.6/whitecanvas/types/_alias.py` & `whitecanvas-0.3.0/whitecanvas/types/_alias.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/types/_enums.py` & `whitecanvas-0.3.0/whitecanvas/types/_enums.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/types/_mouse.py` & `whitecanvas-0.3.0/whitecanvas/types/_mouse.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/types/_tuples.py` & `whitecanvas-0.3.0/whitecanvas/types/_tuples.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,14 +43,51 @@
 
 class XYTextData(NamedTuple):
     x: NDArray[np.floating]
     y: NDArray[np.floating]
     text: NDArray[np.object_]
 
 
+class XYZData(NamedTuple):
+    """
+    Tuple of x, y, and z array.
+
+    Used for data of Surface etc.
+    """
+
+    x: NDArray[np.floating]
+    y: NDArray[np.floating]
+    z: NDArray[np.floating]
+
+    def stack(self) -> NDArray[np.floating]:
+        """Data as a stacked (N, 3) array."""
+        return np.stack([self.x, self.y, self.z], axis=1)
+
+
+class XYVectorData(NamedTuple):
+    x: NDArray[np.floating]
+    y: NDArray[np.floating]
+    vx: NDArray[np.floating]
+    vy: NDArray[np.floating]
+
+
+class XYZVectorData(NamedTuple):
+    x: NDArray[np.floating]
+    y: NDArray[np.floating]
+    z: NDArray[np.floating]
+    vx: NDArray[np.floating]
+    vy: NDArray[np.floating]
+    vz: NDArray[np.floating]
+
+
+class MeshData(NamedTuple):
+    vertices: NDArray[np.floating]
+    faces: NDArray[np.intp]
+
+
 class Rect(NamedTuple):
     """Rectangular range in left, right, bottom, top order."""
 
     left: float
     right: float
     bottom: float
     top: float
```

### Comparing `whitecanvas-0.2.6/whitecanvas/utils/collections.py` & `whitecanvas-0.3.0/whitecanvas/utils/collections.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/utils/hist.py` & `whitecanvas-0.3.0/whitecanvas/utils/hist.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/utils/kde.py` & `whitecanvas-0.3.0/whitecanvas/utils/kde.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/whitecanvas/utils/normalize.py` & `whitecanvas-0.3.0/whitecanvas/utils/normalize.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any, Mapping
 
 import numpy as np
 from cmap import Color
 from numpy.typing import ArrayLike, NDArray
 
-from whitecanvas.types import XYData
+from whitecanvas.types import XYData, XYZData
 from whitecanvas.utils import type_check as _tc
 
 
 def as_array_1d(x: ArrayLike, dtype=None) -> NDArray[np.number]:
     """Normalize the input as a 1D array."""
     x = np.asarray(x, dtype=dtype)
     if x.ndim != 1:
@@ -52,14 +52,46 @@
                 f"got {xdata.size} and {ydata.size}"
             )
     else:
         raise TypeError(f"Expected 1 or 2 positional arguments, got {len(args)}")
     return xdata, ydata
 
 
+def normalize_xyz(
+    *args,
+) -> tuple[NDArray[np.number], NDArray[np.number], NDArray[np.number]]:
+    """Normalize the input as three 1D array with the same shape."""
+    if len(args) == 1:
+        if isinstance(args[0], XYZData):
+            return args[0].x, args[0].y, args[0].z
+        arr = np.asarray(args[0])
+        if arr.dtype.kind not in "iuf":
+            raise ValueError(f"Input {args[0]!r} did not return a numeric array")
+        if arr.ndim == 2 and arr.shape[1] == 3:
+            xdata = arr[:, 0]
+            ydata = arr[:, 1]
+            zdata = arr[:, 2]
+        else:
+            raise ValueError(
+                f"Expected 1D array or 2D array with shape (N, 3), got {arr.shape}"
+            )
+    elif len(args) == 3:
+        xdata = as_array_1d(args[0])
+        ydata = as_array_1d(args[1])
+        zdata = as_array_1d(args[2])
+        if xdata.size != ydata.size != zdata.size:
+            raise ValueError(
+                "Expected xdata, ydata, and zdata to have the same size, "
+                f"got {xdata.size}, {ydata.size}, and {zdata.size}"
+            )
+    else:
+        raise TypeError(f"Expected 1 or 3 positional arguments, got {len(args)}")
+    return xdata, ydata, zdata
+
+
 def arr_color(color) -> np.ndarray:
     """Normalize a color input to a 4-element float array."""
     try:
         c = Color(color)
     except Exception:
         raise ValueError(f"Invalid input for a color: {color!r}") from None
     return np.array(c.rgba, dtype=np.float32)
@@ -100,17 +132,21 @@
             return np.stack([arr_color(each) for each in color], axis=0)
         elif color.shape in [(3,), (4,)]:
             col = arr_color(color)
             return np.repeat(col[np.newaxis, :], size, axis=0)
         elif color.shape in [(size, 3), (size, 4)]:
             return color
         else:
+            if isinstance(color, np.ndarray):
+                color_repr = f"ndarray of shape={color.shape} and dtype={color.dtype}"
+            else:
+                color_repr = repr(color)
             raise ValueError(
                 f"Color array must have shape (3,), (4,), (N={size}, 3), or (N={size},"
-                f" 4) but got\n{color!r}"
+                f" 4) but got {color_repr}."
             )
     try:
         arr = np.array(color)
     except ValueError as e:
         if str(e).startswith("setting an array element with a sequence"):
             # this happens when ["red", [0.0, 1.0, 0.0, 1.0]] is given
             color_normed = np.stack(
```

### Comparing `whitecanvas-0.2.6/whitecanvas/utils/type_check.py` & `whitecanvas-0.3.0/whitecanvas/utils/type_check.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/.gitignore` & `whitecanvas-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/LICENSE` & `whitecanvas-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/README.md` & `whitecanvas-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.6/pyproject.toml` & `whitecanvas-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,17 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "typing_extensions>=4.5.0",
   "numpy>=1.23.2",
   "psygnal>=0.9.4,!=0.10.0",
-  "cmap>=0.1.2",
+  "cmap>=0.2.0",
 ]
 
-
 [project.optional-dependencies]
 matplotlib = [
   "matplotlib>=3.4.3,!=3.8.0",
 ]
 
 pyqtgraph = [
   "pyqtgraph>=0.13.3",
```

### Comparing `whitecanvas-0.2.6/PKG-INFO` & `whitecanvas-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: whitecanvas
-Version: 0.2.6
+Version: 0.3.0
 Summary: A type safe and backend independent plotting library for Python.
 Project-URL: Documentation, https://github.com/hanjinliu/whitecanvas#readme
 Project-URL: Issues, https://github.com/hanjinliu/whitecanvas/issues
 Project-URL: Source, https://github.com/hanjinliu/whitecanvas
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
@@ -41,15 +41,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
-Requires-Dist: cmap>=0.1.2
+Requires-Dist: cmap>=0.2.0
 Requires-Dist: numpy>=1.23.2
 Requires-Dist: psygnal!=0.10.0,>=0.9.4
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: bokeh
 Requires-Dist: bokeh>=3.3.1; extra == 'bokeh'
 Provides-Extra: docs
 Requires-Dist: imageio>=2.9.0; extra == 'docs'
```


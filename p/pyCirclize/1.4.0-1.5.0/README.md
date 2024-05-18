# Comparing `tmp/pycirclize-1.4.0.tar.gz` & `tmp/pycirclize-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycirclize-1.4.0.tar", max compression
+gzip compressed data, was "pycirclize-1.5.0.tar", max compression
```

## Comparing `pycirclize-1.4.0.tar` & `pycirclize-1.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1062 2024-04-01 13:00:56.095008 pycirclize-1.4.0/LICENSE
--rw-r--r--   0        0        0     9304 2024-04-01 13:00:56.095008 pycirclize-1.4.0/README.md
--rw-r--r--   0        0        0     2088 2024-04-01 13:00:56.239009 pycirclize-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       89 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/__init__.py
--rw-r--r--   0        0        0    45398 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/circos.py
--rw-r--r--   0        0        0     3078 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/config.py
--rw-r--r--   0        0        0      337 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/__init__.py
--rw-r--r--   0        0        0     1684 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/bed.py
--rw-r--r--   0        0        0    15407 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/genbank.py
--rw-r--r--   0        0        0    17077 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/gff.py
--rw-r--r--   0        0        0     8157 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/matrix.py
--rw-r--r--   0        0        0     6182 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/table.py
--rw-r--r--   0        0        0    16391 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/patches.py
--rw-r--r--   0        0        0    16891 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/sector.py
--rw-r--r--   0        0        0    52377 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/track.py
--rw-r--r--   0        0        0    25330 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/tree.py
--rw-r--r--   0        0        0      533 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/__init__.py
--rw-r--r--   0        0        0     7829 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/dataset.py
--rw-r--r--   0        0        0     9955 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/images/python_logo.png
--rw-r--r--   0        0        0      565 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/alphabet.nwk
--rw-r--r--   0        0        0     7112 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/large_example.nwk
--rw-r--r--   0        0        0      778 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/medium_example.nwk
--rw-r--r--   0        0        0      227 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/small_example.nwk
--rw-r--r--   0        0        0     3870 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/helper.py
--rw-r--r--   0        0        0     2314 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/plot.py
--rw-r--r--   0        0        0        0 2024-04-01 13:00:56.239009 pycirclize-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     2601 2024-04-01 13:00:56.239009 pycirclize-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-01 13:00:56.239009 pycirclize-1.4.0/tests/parser/__init__.py
--rw-r--r--   0        0        0     2639 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_genbank.py
--rw-r--r--   0        0        0     1827 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_gff.py
--rw-r--r--   0        0        0     4351 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_matrix.py
--rw-r--r--   0        0        0     3700 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_table.py
--rw-r--r--   0        0        0     2765 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_circos.py
--rw-r--r--   0        0        0    25147 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_plot.py
--rw-r--r--   0        0        0     2887 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_sector.py
--rw-r--r--   0        0        0      988 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_track.py
--rw-r--r--   0        0        0      755 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
--rw-r--r--   0        0        0    30808 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
--rw-r--r--   0        0        0   283582 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
--rw-r--r--   0        0        0   148834 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
--rw-r--r--   0        0        0    36204 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff
--rw-r--r--   0        0        0   580710 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
--rw-r--r--   0        0        0    58530 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
--rw-r--r--   0        0        0    57946 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz
--rw-r--r--   0        0        0        0 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/utils/test_dataset.py
--rw-r--r--   0        0        0     1839 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/utils/test_helper.py
--rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 pycirclize-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-18 05:08:28.097730 pycirclize-1.5.0/LICENSE
+-rw-r--r--   0        0        0     9304 2024-05-18 05:08:28.101730 pycirclize-1.5.0/README.md
+-rw-r--r--   0        0        0     2088 2024-05-18 05:08:28.245730 pycirclize-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/__init__.py
+-rw-r--r--   0        0        0    46248 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/circos.py
+-rw-r--r--   0        0        0     3078 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/config.py
+-rw-r--r--   0        0        0      337 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/__init__.py
+-rw-r--r--   0        0        0     1684 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/bed.py
+-rw-r--r--   0        0        0    16026 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/genbank.py
+-rw-r--r--   0        0        0    17540 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/gff.py
+-rw-r--r--   0        0        0     8157 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/matrix.py
+-rw-r--r--   0        0        0     6182 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/table.py
+-rw-r--r--   0        0        0    16391 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/patches.py
+-rw-r--r--   0        0        0    17309 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/sector.py
+-rw-r--r--   0        0        0    52377 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/track.py
+-rw-r--r--   0        0        0    25330 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/tree.py
+-rw-r--r--   0        0        0      533 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/__init__.py
+-rw-r--r--   0        0        0     7829 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/dataset.py
+-rw-r--r--   0        0        0     9955 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/images/python_logo.png
+-rw-r--r--   0        0        0      565 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/alphabet.nwk
+-rw-r--r--   0        0        0     7112 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/large_example.nwk
+-rw-r--r--   0        0        0      778 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/medium_example.nwk
+-rw-r--r--   0        0        0      227 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/small_example.nwk
+-rw-r--r--   0        0        0     3870 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/helper.py
+-rw-r--r--   0        0        0     2314 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/plot.py
+-rw-r--r--   0        0        0        0 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     2601 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/parser/__init__.py
+-rw-r--r--   0        0        0     2639 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/parser/test_genbank.py
+-rw-r--r--   0        0        0     1827 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/parser/test_gff.py
+-rw-r--r--   0        0        0     4351 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/parser/test_matrix.py
+-rw-r--r--   0        0        0     3700 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/parser/test_table.py
+-rw-r--r--   0        0        0     2962 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_circos.py
+-rw-r--r--   0        0        0    25203 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_plot.py
+-rw-r--r--   0        0        0     2885 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_sector.py
+-rw-r--r--   0        0        0      988 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_track.py
+-rw-r--r--   0        0        0      755 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
+-rw-r--r--   0        0        0    30808 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
+-rw-r--r--   0        0        0   283582 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
+-rw-r--r--   0        0        0   148834 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
+-rw-r--r--   0        0        0    36204 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/prokaryote/enterobacteria_phage.gff
+-rw-r--r--   0        0        0   580710 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
+-rw-r--r--   0        0        0    58530 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
+-rw-r--r--   0        0        0    57946 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz
+-rw-r--r--   0        0        0        0 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/utils/test_dataset.py
+-rw-r--r--   0        0        0     1839 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/utils/test_helper.py
+-rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 pycirclize-1.5.0/PKG-INFO
```

### Comparing `pycirclize-1.4.0/LICENSE` & `pycirclize-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/README.md` & `pycirclize-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/pyproject.toml` & `pycirclize-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyCirclize"
-version = "1.4.0"
+version = "1.5.0"
 description = "Circular visualization in Python"
 authors = ["moshi4"]
 license = "MIT"
 homepage = "https://moshi4.github.io/pyCirclize/"
 repository = "https://github.com/moshi4/pyCirclize/"
 readme = "README.md"
 keywords = [
```

### Comparing `pycirclize-1.4.0/src/pycirclize/circos.py` & `pycirclize-1.5.0/src/pycirclize/circos.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,45 +36,41 @@
 
 
 class Circos:
     """Circos Visualization Class"""
 
     def __init__(
         self,
-        sectors: Mapping[str, int | float],
+        sectors: Mapping[str, int | float | tuple[float, float]],
         start: float = 0,
         end: float = 360,
         *,
         space: float | list[float] = 0,
         endspace: bool = True,
-        sector2start_pos: Mapping[str, int | float] | None = None,
         sector2clockwise: dict[str, bool] | None = None,
         show_axis_for_debug: bool = False,
     ):
         """
         Parameters
         ----------
-        sectors : Mapping[str, int | float]
-            Sector name & size dict
+        sectors : Mapping[str, int | float | tuple[float, float]]
+            Sector name & size (or range) dict
         start : float, optional
             Plot start degree (`-360 <= start < end <= 360`)
         end : float, optional
             Plot end degree (`-360 <= start < end <= 360`)
         space : float | list[float], optional
             Space degree(s) between sector
         endspace : bool, optional
             If True, insert space after the end sector
-        sector2start_pos : Mapping[str, int | float] | None, optional
-            Sector name & start position dict. By default, `start_pos=0`.
         sector2clockwise : dict[str, bool] | None, optional
             Sector name & clockwise bool dict. By default, `clockwise=True`.
         show_axis_for_debug : bool, optional
             Show axis for position check debugging (Developer option)
         """
-        sector2start_pos = {} if sector2start_pos is None else sector2start_pos
         sector2clockwise = {} if sector2clockwise is None else sector2clockwise
 
         # Check start-end degree range
         self._check_degree_range(start, end)
 
         # Calculate sector region & add sector
         whole_deg_size = end - start
@@ -96,27 +92,29 @@
                 Too large sector space size is set!!
                 Circos Degree Size = {whole_deg_size} ({start} - {end})
                 Total Sector Space Size = {space_deg_size}
                 List of Sector Space Size = {space_list}
                 """
             )[1:-1]
             raise ValueError(err_msg)
-        sector_total_size = sum(sectors.values())
+
+        sector2range = self._to_sector2range(sectors)
+        sector_total_size = sum([max(r) - min(r) for r in sector2range.values()])
 
         rad_pos = math.radians(start)
         self._sectors: list[Sector] = []
-        for idx, (sector_name, sector_size) in enumerate(sectors.items()):
+        for idx, (sector_name, sector_range) in enumerate(sector2range.items()):
+            sector_size = max(sector_range) - min(sector_range)
             sector_size_ratio = sector_size / sector_total_size
             deg_size = whole_deg_size_without_space * sector_size_ratio
             rad_size = math.radians(deg_size)
             rad_lim = (rad_pos, rad_pos + rad_size)
             rad_pos += rad_size + math.radians(space_list[idx])
-            start_pos = sector2start_pos.get(sector_name, 0)
             clockwise = sector2clockwise.get(sector_name, True)
-            sector = Sector(sector_name, sector_size, rad_lim, start_pos, clockwise)
+            sector = Sector(sector_name, sector_range, rad_lim, clockwise)
             self._sectors.append(sector)
 
         self._deg_lim = (start, end)
         self._rad_lim = (math.radians(start), math.radians(end))
         self._patches: list[Patch] = []
         self._plot_funcs: list[Callable[[PolarAxes], None]] = []
         self._ax: PolarAxes | None = None
@@ -176,14 +174,15 @@
     ############################################################
 
     @staticmethod
     def radar_chart(
         table: str | Path | pd.DataFrame | RadarTable,
         *,
         r_lim: tuple[float, float] = (0, 100),
+        vmin: float = 0,
         vmax: float = 100,
         fill: bool = True,
         marker_size: int = 0,
         bg_color: str | None = "#eeeeee80",
         circular: bool = False,
         cmap: str | dict[str, str] = "Set2",
         show_grid_label: bool = True,
@@ -199,14 +198,16 @@
 
         Parameters
         ----------
         table : str | Path | pd.DataFrame | RadarTable
             Table file or Table dataframe or RadarTable instance
         r_lim : tuple[float, float], optional
             Radar chart radius limit region (0 - 100)
+        vmin : float, optional
+            Min value
         vmax : float, optional
             Max value
         fill : bool, optional
             If True, fill color of radar chart.
         marker_size : int, optional
             Marker size
         bg_color : str | None, optional
@@ -240,14 +241,18 @@
             Handler function takes each row(index) name of table as an argument.
 
         Returns
         -------
         circos : Circos
             Circos instance initialized for radar chart
         """
+        if not vmin < vmax:
+            raise ValueError(f"vmax must be larger than vmin ({vmin=}, {vmax=})")
+        size = vmax - vmin
+
         # Setup default properties
         grid_line_kws = {} if grid_line_kws is None else deepcopy(grid_line_kws)
         for k, v in dict(color="grey", ls="dashed", lw=0.5).items():
             grid_line_kws.setdefault(k, v)
 
         grid_label_kws = {} if grid_label_kws is None else deepcopy(grid_label_kws)
         for k, v in dict(color="dimgrey", size=10, ha="left", va="top").items():
@@ -265,50 +270,52 @@
             track.fill_between(x, [vmax] * len(x), arc=circular, color=bg_color)
 
         # Plot grid line
         if grid_interval_ratio:
             if not 0 < grid_interval_ratio <= 1.0:
                 raise ValueError(f"{grid_interval_ratio=} is invalid.")
             # Plot horizontal grid line & label
-            stop, step = vmax + (vmax / 1000), vmax * grid_interval_ratio
-            for v in np.arange(0, stop, step):
-                track.line(x, [v] * len(x), vmax=vmax, arc=circular, **grid_line_kws)
+            stop, step = vmax + (size / 1000), size * grid_interval_ratio
+            for v in np.arange(vmin, stop, step):
+                y = [v] * len(x)
+                track.line(x, y, vmin=vmin, vmax=vmax, arc=circular, **grid_line_kws)
                 if show_grid_label:
-                    r = track._y_to_r(v, 0, vmax)
+                    r = track._y_to_r(v, vmin, vmax)
                     # Format grid label
                     if grid_label_formatter:
                         text = grid_label_formatter(v)
                     else:
                         v = float(f"{v:.9f}")  # Correct rounding error
                         text = f"{v:.0f}" if math.isclose(int(v), float(v)) else str(v)
                     track.text(text, 0, r, **grid_label_kws)
             # Plot vertical grid line
             for p in x[:-1]:
-                track.line([p, p], [0, vmax], vmax=vmax, **grid_line_kws)
+                track.line([p, p], [vmin, vmax], vmin=vmin, vmax=vmax, **grid_line_kws)
 
         # Plot radar charts
         if isinstance(cmap, str):
             row_name2color = radar_table.get_row_name2color(cmap)
         else:
             row_name2color = cmap
         for row_name, values in radar_table.row_name2values.items():
             y = values + [values[0]]
             color = row_name2color[row_name]
             line_kws = line_kws_handler(row_name) if line_kws_handler else {}
             line_kws.setdefault("lw", 1.0)
             line_kws.setdefault("label", row_name)
-            track.line(x, y, vmax=vmax, arc=False, color=color, **line_kws)
+            track.line(x, y, vmin=vmin, vmax=vmax, arc=False, color=color, **line_kws)
             if marker_size > 0:
                 marker_kws = marker_kws_handler(row_name) if marker_kws_handler else {}
                 marker_kws.setdefault("marker", "o")
                 marker_kws.setdefault("zorder", 2)
                 marker_kws.update(s=marker_size**2)
-                track.scatter(x, y, vmax=vmax, color=color, **marker_kws)
+                track.scatter(x, y, vmin=vmin, vmax=vmax, color=color, **marker_kws)
             if fill:
-                track.fill_between(x, y, vmax=vmax, arc=False, color=color, alpha=0.5)
+                fill_kws = dict(arc=False, color=color, alpha=0.5)
+                track.fill_between(x, y, y2=vmin, vmin=vmin, vmax=vmax, **fill_kws)  # type:ignore
 
         # Plot column names
         for idx, col_name in enumerate(radar_table.col_names):
             deg = 360 * (idx / sector.size)
             label_kws = label_kws_handler(col_name) if label_kws_handler else {}
             label_kws.setdefault("size", 12)
             if math.isclose(deg, 0):
@@ -573,23 +580,21 @@
 
         Returns
         -------
         circos : Circos
             Circos instance initialized from BED file
         """
         records = Bed(bed_file).records
-        sectors = {rec.chr: rec.size for rec in records}
-        sector2start_pos = {rec.chr: rec.start for rec in records}
+        sectors = {rec.chr: (rec.start, rec.end) for rec in records}
         return Circos(
             sectors,
             start,
             end,
             space=space,
             endspace=endspace,
-            sector2start_pos=sector2start_pos,
             sector2clockwise=sector2clockwise,
         )
 
     def add_cytoband_tracks(
         self,
         r_lim: tuple[float, float],
         cytoband_file: str | Path,
@@ -1094,14 +1099,31 @@
             err_msg = "start-end must be "
             err_msg += f"'{min_deg} <= start < end <= {max_deg}' ({start=}, {end=})"
             raise ValueError(err_msg)
         if end - start > max_deg:
             err_msg = f"'end - start' must be less than {max_deg} ({start=}, {end=})"
             raise ValueError(err_msg)
 
+    def _to_sector2range(
+        self,
+        sectors: Mapping[str, int | float | tuple[float, float]],
+    ) -> dict[str, tuple[float, float]]:
+        """Convert sectors to sector2range"""
+        sector2range: dict[str, tuple[float, float]] = {}
+        for name, value in sectors.items():
+            if isinstance(value, (tuple, list)):
+                sector_start, sector_end = value
+                if not sector_start < sector_end:
+                    err_msg = f"{sector_end=} must be larger than {sector_start=}."
+                    raise ValueError(err_msg)
+                sector2range[name] = (sector_start, sector_end)
+            else:
+                sector2range[name] = (0, value)
+        return sector2range
+
     def _initialize_figure(
         self,
         figsize: tuple[float, float] = (8, 8),
         dpi: int = 100,
     ) -> tuple[Figure, PolarAxes]:
         """Initialize figure
```

### Comparing `pycirclize-1.4.0/src/pycirclize/config.py` & `pycirclize-1.5.0/src/pycirclize/config.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/parser/bed.py` & `pycirclize-1.5.0/src/pycirclize/parser/bed.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/parser/genbank.py` & `pycirclize-1.5.0/src/pycirclize/parser/genbank.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 import bz2
 import gzip
 import warnings
 import zipfile
 from collections import defaultdict
 from io import StringIO, TextIOWrapper
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import numpy as np
 from Bio import SeqIO, SeqUtils
 from Bio.SeqFeature import Seq, SeqFeature, SimpleLocation
 from Bio.SeqRecord import SeqRecord
 
+if TYPE_CHECKING:
+    from numpy.typing import NDArray
+
 
 class Genbank:
     """Genbank Parser Class"""
 
     def __init__(
         self,
         gbk_source: str | Path | TextIOWrapper | list[SeqRecord],
@@ -52,19 +56,22 @@
             if gbk_file.suffix in (".gz", ".bz2", ".zip"):
                 self._name = gbk_file.with_suffix("").with_suffix("").name
             else:
                 self._name = gbk_file.with_suffix("").name
         elif isinstance(self._gbk_source, (StringIO, TextIOWrapper)):
             self._name = self._records[0].name
         else:
-            raise NotImplementedError("Failed to get name.")
+            raise ValueError("Failed to get genbank name.")
 
         if min_range or max_range:
             warnings.warn("min_range & max_range is no longer used in Genbank parser.")
 
+        if len(self.records) == 0:
+            raise ValueError(f"Failed to parse {gbk_source} as Genbank file.")
+
     ############################################################
     # Property
     ############################################################
 
     @property
     def name(self) -> str:
         """Name"""
@@ -123,29 +130,29 @@
 
     def calc_gc_skew(
         self,
         window_size: int | None = None,
         step_size: int | None = None,
         *,
         seq: str | None = None,
-    ) -> tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[NDArray[np.int64], NDArray[np.float64]]:
         """Calculate GC skew in sliding window
 
         Parameters
         ----------
         window_size : int | None, optional
             Window size (Default: `genome_size / 500`)
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
         seq : str | None, optional
             Sequence for GCskew calculation (Default: `self.genome_seq`)
 
         Returns
         -------
-        gc_skew_result_tuple : tuple[np.ndarray, np.ndarray]
+        gc_skew_result_tuple : tuple[NDArray[np.int64], NDArray[np.float64]]
             Position list & GC skew list
         """
         pos_list, gc_skew_list = [], []
         seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
@@ -164,37 +171,40 @@
             c = subseq.count("C") + subseq.count("c")
             try:
                 skew = (g - c) / float(g + c)
             except ZeroDivisionError:
                 skew = 0.0
             gc_skew_list.append(skew)
 
-        return (np.array(pos_list), np.array(gc_skew_list))
+        pos_list = np.array(pos_list).astype(np.int64)
+        gc_skew_list = np.array(gc_skew_list).astype(np.float64)
+
+        return pos_list, gc_skew_list
 
     def calc_gc_content(
         self,
         window_size: int | None = None,
         step_size: int | None = None,
         *,
         seq: str | None = None,
-    ) -> tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[NDArray[np.int64], NDArray[np.float64]]:
         """Calculate GC content in sliding window
 
         Parameters
         ----------
         window_size : int | None, optional
             Window size (Default: `genome_size / 500`)
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
         seq : str | None, optional
             Sequence for GC content calculation (Default: `self.genome_seq`)
 
         Returns
         -------
-        gc_content_result_tuple : tuple[np.ndarray, np.ndarray]
+        gc_content_result_tuple : tuple[NDArray[np.int64], NDArray[np.float64]]
             Position list & GC content list
         """
         pos_list, gc_content_list = [], []
         seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
@@ -208,15 +218,18 @@
             window_start_pos = 0 if window_start_pos < 0 else window_start_pos
             window_end_pos = len(seq) if window_end_pos > len(seq) else window_end_pos
 
             subseq = seq[window_start_pos:window_end_pos]
             gc_content = SeqUtils.gc_fraction(subseq) * 100
             gc_content_list.append(gc_content)
 
-        return (np.array(pos_list), np.array(gc_content_list))
+        pos_list = np.array(pos_list).astype(np.int64)
+        gc_content_list = np.array(gc_content_list).astype(np.float64)
+
+        return pos_list, gc_content_list
 
     def get_seqid2seq(self) -> dict[str, str]:
         """Get seqid & complete/contig/scaffold genome sequence dict
 
         Returns
         -------
         seqid2seq : dict[str, int]
@@ -232,38 +245,41 @@
         seqid2size : dict[str, int]
             seqid & genome size dict
         """
         return {seqid: len(seq) for seqid, seq in self.get_seqid2seq().items()}
 
     def get_seqid2features(
         self,
-        feature_type: str | None = "CDS",
+        feature_type: str | list[str] | None = "CDS",
         target_strand: int | None = None,
     ) -> dict[str, list[SeqFeature]]:
         """Get seqid & features in target seqid genome dict
 
         Parameters
         ----------
-        feature_type : str | None, optional
+        feature_type : str | list[str] | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
             If None, extract regardless of feature type.
         target_strand : int | None, optional
             Extract target strand. If None, extract regardless of strand.
 
         Returns
         -------
         seqid2features : dict[str, list[SeqFeature]]
             seqid & features dict
         """
+        if isinstance(feature_type, str):
+            feature_type = [feature_type]
+
         seqid2features = defaultdict(list)
         for rec in self.records:
             feature: SeqFeature
             for feature in rec.features:
                 strand = feature.location.strand
-                if feature_type is not None and feature.type != feature_type:
+                if feature_type is not None and feature.type not in feature_type:
                     continue
                 if target_strand is not None and strand != target_strand:
                     continue
                 # Exclude feature which straddle genome start position
                 if self._is_straddle_feature(feature):
                     continue
                 start = int(feature.location.start)  # type: ignore
@@ -275,23 +291,24 @@
                         qualifiers=feature.qualifiers,
                     ),
                 )
         return seqid2features
 
     def extract_features(
         self,
-        feature_type: str | None = "CDS",
+        feature_type: str | list[str] | None = "CDS",
+        *,
         target_strand: int | None = None,
         target_range: tuple[int, int] | None = None,
     ) -> list[SeqFeature]:
         """Extract features (only first record)
 
         Parameters
         ----------
-        feature_type : str | None, optional
+        feature_type : str | list[str] | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
             If None, extract regardless of feature type.
         target_strand : int | None, optional
             Extract target strand. If None, extract regardless of strand.
         target_range : tuple[int, int] | None, optional
             Extract target range. If None, extract regardless of range.
```

### Comparing `pycirclize-1.4.0/src/pycirclize/parser/gff.py` & `pycirclize-1.5.0/src/pycirclize/parser/gff.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,55 +120,63 @@
         seqid2size : dict[str, int]
             seqid & genome size dict
         """
         return self._seqid2size
 
     def get_seqid2features(
         self,
-        feature_type: str | None = "CDS",
+        feature_type: str | list[str] | None = "CDS",
         target_strand: int | None = None,
     ) -> dict[str, list[SeqFeature]]:
         """Get seqid & features in target seqid genome dict
 
         Parameters
         ----------
-        feature_type : str | None, optional
+        feature_type : str | list[str] | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
             If None, extract regardless of feature type.
         target_strand : int | None, optional
             Extract target strand. If None, extract regardless of strand.
 
         Returns
         -------
         seqid2features : dict[str, list[SeqFeature]]
             seqid & features dict
         """
+        if isinstance(feature_type, str):
+            feature_type = [feature_type]
+
         gff_records = GffRecord.filter_records(
             self.all_records,
             feature_type=feature_type,
             target_strand=target_strand,
         )
         seqid2features: dict[str, list[SeqFeature]] = {}
         for seqid in self.seqid_list:
             seqid2features[seqid] = []
         for rec in gff_records:
             seqid2features[rec.seqid].append(rec.to_seq_feature())
         return seqid2features
 
     def extract_features(
         self,
-        feature_type: str | None = "CDS",
+        feature_type: str | list[str] | None = "CDS",
+        *,
         target_strand: int | None = None,
         target_range: tuple[int, int] | None = None,
     ) -> list[SeqFeature]:
         """Extract features
 
+        If `target_seqid` is specified when the Gff instance initialized,
+        then the features of the target seqid are extracted.
+        Otherwise, extract the features of the seqid in the first row.
+
         Parameters
         ----------
-        feature_type : str | None, optional
+        feature_type : str | list[str] | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
             If None, extract regardless of feature type.
         target_strand : int | None, optional
             Extract target strand. If None, extract regardless of strand.
         target_range : tuple[int, int] | None, optional
             Extract target range. If None, extract regardless of range.
 
@@ -200,15 +208,15 @@
         features : list[SeqFeature]
             Feature list
         """
         # Extract exon features by mRNA-exon relation
         parent_id = None
         parent_id2record: dict[str, GffRecord] = {}
         parent_id2exons: dict[str, list[GffRecord]] = defaultdict(list)
-        for rec in self._records:
+        for rec in self.records:
             if rec.type == feature_type:
                 parent_id = rec.attrs.get("ID", [None])[0]
                 if parent_id is None:
                     continue
                 parent_id2record[parent_id] = rec
             if rec.type == "exon":
                 if parent_id is not None and parent_id == rec.attrs["Parent"][0]:
@@ -479,39 +487,42 @@
         gff_elms[8] = attr_dict
 
         return GffRecord(*gff_elms)
 
     @staticmethod
     def filter_records(
         gff_records: list[GffRecord],
-        feature_type: str | None = "CDS",
+        feature_type: str | list[str] | None = "CDS",
         target_strand: int | None = None,
         target_range: tuple[int, int] | None = None,
     ) -> list[GffRecord]:
         """Filter GFF records by feature_type, strand, range
 
         Parameters
         ----------
         gff_records : list[GffRecord]
             GFF records to be filterd
-        feature_type : str | None, optional
+        feature_type : str | list[str] | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...). If None, no filter.
         target_strand : int | None, optional
             Target strand. If None, no filter.
         target_range : tuple[int, int] | None, optional
             Target range. If None, no filter.
 
         Returns
         -------
         filter_gff_records : list[SeqFeature]
             Filtered GFF records
         """
+        if isinstance(feature_type, str):
+            feature_type = [feature_type]
+
         filter_gff_records = []
         for rec in gff_records:
-            if feature_type is not None and rec.type != feature_type:
+            if feature_type is not None and rec.type not in feature_type:
                 continue
             if target_strand is not None and rec.strand != target_strand:
                 continue
             if target_range is not None:
                 min_range, max_range = min(target_range), max(target_range)
                 if not min_range <= rec.start <= rec.end <= max_range:
                     continue
```

### Comparing `pycirclize-1.4.0/src/pycirclize/parser/matrix.py` & `pycirclize-1.5.0/src/pycirclize/parser/matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/parser/table.py` & `pycirclize-1.5.0/src/pycirclize/parser/table.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/patches.py` & `pycirclize-1.5.0/src/pycirclize/patches.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/sector.py` & `pycirclize-1.5.0/src/pycirclize/sector.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,37 +22,39 @@
 
 class Sector:
     """Circos Sector Class"""
 
     def __init__(
         self,
         name: str,
-        size: float,
+        size: float | tuple[float, float],
         rad_lim: tuple[float, float],
-        start_pos: float = 0,
         clockwise: bool = True,
     ):
         """
         Parameters
         ----------
         name : str
             Sector name
-        size : float
-            Sector size
+        size : float | tuple[float, float]
+            Sector size (or range)
         rad_lim : tuple[float, float]
             Sector radian limit region
-        start_pos : float, optional
-            Sector start position
         clockwise : bool, optional
             Sector coordinate direction (clockwise or anti-clockwise).
         """
         self._name = name
-        self._size = size
+        if isinstance(size, (tuple, list)):
+            start, end = size[0], size[1]
+        else:
+            start, end = 0, size
+        self._start = start
+        self._end = end
+        self._size = end - start
         self._rad_lim = rad_lim
-        self._start_pos = start_pos
         self._clockwise = clockwise
         self._tracks: list[Track] = []
 
         # Plot data and functions
         self._patches: list[Patch] = []
         self._plot_funcs: list[Callable[[PolarAxes], None]] = []
 
@@ -69,20 +71,20 @@
     def size(self) -> float:
         """Sector size (x coordinate)"""
         return self._size
 
     @property
     def start(self) -> float:
         """Sector start position (x coordinate)"""
-        return self._start_pos
+        return self._start
 
     @property
     def end(self) -> float:
         """Sector end position (x coordinate)"""
-        return self._start_pos + self._size
+        return self._end
 
     @property
     def center(self) -> float:
         """Sector center position (x coordinate)"""
         return (self.start + self.end) / 2
 
     @property
@@ -203,17 +205,24 @@
             Ignore x coordinate range error
 
         Returns
         -------
         rad : float
             Radian coordinate
         """
-        if not self.start <= x <= self.end and not ignore_range_error:
-            err_msg = f"{x=} is invalid range of '{self.name}' sector.\n{self}"
-            raise ValueError(err_msg)
+        # Check target x is in valid sector range
+        if not ignore_range_error:
+            # Apply relative torelance value to sector range to avoid
+            # unexpected invalid range error due to rounding errors (Issue #27, #67)
+            rel_tol = 1e-14
+            min_range, max_range = self.start - rel_tol, self.end + rel_tol
+            if not min_range <= x <= max_range:
+                err_msg = f"{x=} is invalid range of '{self.name}' sector.\n{self}"
+                raise ValueError(err_msg)
+
         if not self.clockwise:
             x = (self.start + self.end) - x
         size_ratio = self.rad_size / self.size
         x_from_start = x - self.start
         rad_from_start = x_from_start * size_ratio
         rad = min(self.rad_lim) + rad_from_start
         return rad
```

### Comparing `pycirclize-1.4.0/src/pycirclize/track.py` & `pycirclize-1.5.0/src/pycirclize/track.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/tree.py` & `pycirclize-1.5.0/src/pycirclize/tree.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/__init__.py` & `pycirclize-1.5.0/src/pycirclize/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/dataset.py` & `pycirclize-1.5.0/src/pycirclize/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/example_data/images/python_logo.png` & `pycirclize-1.5.0/src/pycirclize/utils/example_data/images/python_logo.png`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/alphabet.nwk` & `pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/alphabet.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/large_example.nwk` & `pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/large_example.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/medium_example.nwk` & `pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/medium_example.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/helper.py` & `pycirclize-1.5.0/src/pycirclize/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/src/pycirclize/utils/plot.py` & `pycirclize-1.5.0/src/pycirclize/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/conftest.py` & `pycirclize-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/parser/test_genbank.py` & `pycirclize-1.5.0/tests/parser/test_genbank.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/parser/test_gff.py` & `pycirclize-1.5.0/tests/parser/test_gff.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/parser/test_matrix.py` & `pycirclize-1.5.0/tests/parser/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/parser/test_table.py` & `pycirclize-1.5.0/tests/parser/test_table.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/test_circos.py` & `pycirclize-1.5.0/tests/test_circos.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 def test_circos_init():
     """Test circos initialization"""
     circos = Circos({"A": 10, "B": 20, "C": 15})
     assert [s.name for s in circos.sectors] == ["A", "B", "C"]
     assert [s.size for s in circos.sectors] == [10, 20, 15]
 
+    circos = Circos(dict(D=10, E=(10, 20), F=(30, 50), G=100))
+    assert [s.name for s in circos.sectors] == ["D", "E", "F", "G"]
+    assert [s.size for s in circos.sectors] == [10, 10, 20, 100]
+
 
 @pytest.mark.parametrize(
     "start, end",
     [
         (-10, 360),  # End - Start > 360
         (0, -90),  # Start > End
         (-400, -200),  # Start < -360
```

### Comparing `pycirclize-1.4.0/tests/test_plot.py` & `pycirclize-1.5.0/tests/test_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -690,18 +690,18 @@
     outer_track = sector.add_track((98, 100))
     outer_track.axis(fc="lightgrey")
     outer_track.xticks_by_interval(5000, label_formatter=lambda v: f"{v / 1000:.0f} Kb")
     outer_track.xticks_by_interval(1000, tick_length=1, show_label=False)
     # Plot forward & reverse CDS genomic features
     cds_track = sector.add_track((90, 95))
     cds_track.genomic_features(
-        gbk.extract_features("CDS", 1), plotstyle="arrow", fc="salmon"
+        gbk.extract_features("CDS", target_strand=1), plotstyle="arrow", fc="salmon"
     )
     cds_track.genomic_features(
-        gbk.extract_features("CDS", -1), plotstyle="arrow", fc="skyblue"
+        gbk.extract_features("CDS", target_strand=-1), plotstyle="arrow", fc="skyblue"
     )
 
     circos.savefig(fig_outfile)
     assert fig_outfile.exists()
 
 
 def test_track_genomic_features_gff_plot(
@@ -723,15 +723,15 @@
     outer_track = sector.add_track((98, 100))
     outer_track.axis(fc="lightgrey")
     outer_track.xticks_by_interval(5000, label_formatter=lambda v: f"{v / 1000:.0f} Kb")
     outer_track.xticks_by_interval(1000, tick_length=1, show_label=False)
     # Plot forward & reverse CDS genomic features
     cds_track = sector.add_track((90, 95))
     cds_track.genomic_features(
-        gff.extract_features("CDS", 1), plotstyle="arrow", fc="salmon"
+        gff.extract_features("CDS", target_strand=1), plotstyle="arrow", fc="salmon"
     )
     cds_track.genomic_features(
-        gff.extract_features("CDS", -1), plotstyle="arrow", fc="skyblue"
+        gff.extract_features("CDS", target_strand=-1), plotstyle="arrow", fc="skyblue"
     )
 
     circos.savefig(fig_outfile)
     assert fig_outfile.exists()
```

### Comparing `pycirclize-1.4.0/tests/test_sector.py` & `pycirclize-1.5.0/tests/test_sector.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def sector() -> Sector:
     """Sector test fixture"""
     return Sector("test", 1000, (0, math.pi))
 
 
 def test_property():
     """Test sector property"""
-    # Case1: start_pos = 0 (Default)
+    # Case1: Set int size
     name, size, rad_lim = "test", 1000, (0, math.pi)
     sector_case1 = Sector(name, size, rad_lim)
     assert sector_case1.name == name
     assert sector_case1.size == size
     assert sector_case1.start == 0
     assert sector_case1.end == size
     assert sector_case1.center == 500
@@ -26,20 +26,20 @@
     assert sector_case1.rad_lim == rad_lim
     assert sector_case1.deg_size == 180
     assert sector_case1.deg_lim == (0, 180)
     assert sector_case1.tracks == []
     assert sector_case1.patches == []
     assert sector_case1.plot_funcs == []
 
-    # Case2: start_pos != 0
-    name, size, rad_lim, start_pos = "test", 1000, (0, math.pi), 100
-    sector_case2 = Sector(name, size, rad_lim, start_pos)
-    assert sector_case2.size == size
-    assert sector_case2.start == start_pos
-    assert sector_case2.end == start_pos + size
+    # Case2: Set tuple[float, float] range
+    name, range, rad_lim = "test", (100, 1100), (0, math.pi)
+    sector_case2 = Sector(name, range, rad_lim)
+    assert sector_case2.size == range[1] - range[0]
+    assert sector_case2.start == range[0]
+    assert sector_case2.end == range[1]
     assert sector_case2.center == 600
 
 
 def test_add_track(sector: Sector):
     """Test add_track()"""
     sector.add_track((90, 100), name="Test01")
     sector.add_track((80, 90))
@@ -69,25 +69,25 @@
     sector.add_track((90, 100))
     sector.add_track((50, 70))
     assert sector.get_lowest_r() == 50
 
 
 def test_x_to_pad():
     """Test `x_to_pad()`"""
-    # Case1: start_pos = 0
+    # Case1: Set int size
     sector = Sector("test", 1000, (0, math.pi))
     assert sector.x_to_rad(0) == 0
     assert sector.x_to_rad(250) == math.pi / 4
     assert sector.x_to_rad(500) == math.pi / 2
     assert sector.x_to_rad(1000) == math.pi
     with pytest.raises(ValueError):
         sector.x_to_rad(sector.end + 1)
 
-    # Case2: start_pos != 0
-    sector = Sector("test", 1000, (0, math.pi), start_pos=100)
+    # Case2: Set tuple[float, float] range
+    sector = Sector("test", (100, 1100), (0, math.pi))
     assert sector.x_to_rad(350) == math.pi / 4
     assert sector.x_to_rad(600) == math.pi / 2
     assert sector.x_to_rad(1100) == math.pi
     with pytest.raises(ValueError):
         assert sector.x_to_rad(0) == 0
     with pytest.raises(ValueError):
         sector.x_to_rad(sector.end + 1)
```

### Comparing `pycirclize-1.4.0/tests/test_track.py` & `pycirclize-1.5.0/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed` & `pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_chr.bed`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv` & `pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv` & `pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk` & `pycirclize-1.5.0/tests/testdata/prokaryote/enterobacteria_phage.gbk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff` & `pycirclize-1.5.0/tests/testdata/prokaryote/enterobacteria_phage.gff`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz` & `pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz` & `pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz` & `pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/utils/test_dataset.py` & `pycirclize-1.5.0/tests/utils/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/tests/utils/test_helper.py` & `pycirclize-1.5.0/tests/utils/test_helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.4.0/PKG-INFO` & `pycirclize-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCirclize
-Version: 1.4.0
+Version: 1.5.0
 Summary: Circular visualization in Python
 Home-page: https://moshi4.github.io/pyCirclize/
 License: MIT
 Keywords: matplotlib,visualization,bioinformatics,circos,chord-diagram
 Author: moshi4
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
```


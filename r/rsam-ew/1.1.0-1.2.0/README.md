# Comparing `tmp/rsam_ew-1.1.0.tar.gz` & `tmp/rsam_ew-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsam_ew-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rsam_ew-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rsam_ew-1.1.0.tar` & `rsam_ew-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1085 2024-05-08 08:08:12.548040 rsam_ew-1.1.0/LICENSE
--rw-r--r--   0        0        0       47 2024-05-11 08:31:09.928735 rsam_ew-1.1.0/README.md
--rw-r--r--   0        0        0      973 2024-05-13 12:37:32.445568 rsam_ew-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      328 2024-05-13 12:10:52.060571 rsam_ew-1.1.0/src/rsam_ew/__init__.py
--rw-r--r--   0        0        0     7824 2024-05-13 12:36:56.273134 rsam_ew-1.1.0/src/rsam_ew/rsam.py
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 rsam_ew-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-08 08:08:12.548040 rsam_ew-1.2.0/LICENSE
+-rw-r--r--   0        0        0       47 2024-05-11 08:31:09.928735 rsam_ew-1.2.0/README.md
+-rw-r--r--   0        0        0      973 2024-05-18 05:42:15.204296 rsam_ew-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      328 2024-05-13 12:10:52.060571 rsam_ew-1.2.0/src/rsam_ew/__init__.py
+-rw-r--r--   0        0        0     7983 2024-05-18 05:47:02.195415 rsam_ew-1.2.0/src/rsam_ew/rsam.py
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 rsam_ew-1.2.0/PKG-INFO
```

### Comparing `rsam_ew-1.1.0/LICENSE` & `rsam_ew-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsam_ew-1.1.0/pyproject.toml` & `rsam_ew-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name =  "rsam-ew"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
     {name = "Martanto", email = "martanto@live.com"},
 ]
 description = "Plot RSAM from earthworm files"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["seismic", "volcano", "seiscomp", "volcanology", "seismology", "magma indonesia"]
```

### Comparing `rsam_ew-1.1.0/src/rsam_ew/rsam.py` & `rsam_ew-1.2.0/src/rsam_ew/rsam.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'Okt': 'Oct',
     'Des': 'Dec',
 }
 
 
 class RsamEW:
     def __init__(self, zip_file_location: str, station: str, channel: str, network: str = None, location: str = None,
-                 wildcard: str = '.dat', delimiter=',', combine_data: bool = False, current_dir: str = None,
+                 wildcard: str = '.DAT', delimiter=',', combine_data: bool = False, current_dir: str = None,
                  input_dir: str = None):
 
         if current_dir is None:
             current_dir = os.getcwd()
         self.current_dir = current_dir
 
         if input_dir is None:
@@ -36,14 +36,16 @@
         self.channel = channel
 
         self.nslc = f'{self.network}.{self.station}.{self.location}.{self.channel}'
 
         self.output_dir, self.figures_dir, self.rsam_dir = self.check_directory(os.getcwd())
         self.extract_dir = self.extract_dir()
         self.filename: str = Path(zip_file_location).stem
+
+        zip_file_location = os.path.join(current_dir, zip_file_location)
         self.files: list = self.get_files(zip_file_location, wildcard, delimiter)
 
         if combine_data is True:
             self.combine_csvs(self.files)
 
     def check_directory(self, current_dir: str = None) -> Tuple[str, str, str]:
 
@@ -174,27 +176,28 @@
         print(f'✅ RSAM file saved at {save_path}')
         return df
 
     def plot_ax(self, ax: plt.Axes, df: pd.DataFrame, smoothing: str = '1d', interval_day: int = 1,
                 y_min: float = 0, y_max: float = None) -> plt.Axes:
 
         ax.scatter(df.index, df['value'], c='k', alpha=0.3, s=10, label='10 minutes')
-        ax.plot(df.index, df[smoothing], c='red', label='1 day', alpha=1)
+        ax.plot(df.index, df[smoothing], c='red', label=smoothing, alpha=1)
 
         ax.set_xlabel('Datetime', fontsize=12)
         ax.xaxis.set_major_locator(mdates.DayLocator(interval=interval_day))
         ax.xaxis.set_major_formatter(mdates.DateFormatter('%Y-%m-%d'))
         ax.set_ylim(y_min, y_max)
         ax.set_xlim(df.first_valid_index(), df.last_valid_index())
         ax.legend(loc='upper right', fontsize='8', ncol=4)
 
         return ax
 
-    def plot(self, start_date: str, end_date: str, title: str = None, smoothing: str = '1d', width: int = 12, height: int = 9,
-             interval_day: int = 1, y_min: float = 0, y_max: float = None, save: bool = True):
+    def plot(self, start_date: str, end_date: str, title: str = None, smoothing: str = '1d', width: int = 12,
+             height: int = 9, interval_day: int = 1, y_min: float = 0, y_max: float = None, show_gridline: bool = True,
+             save: bool = True):
         dates: DatetimeIndex = pd.date_range(start_date, end_date, freq="D")
 
         df = self.get_df(dates)
         df[smoothing] = df['value'].rolling(smoothing, center=True).median()
 
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(width, height),
                                layout="constrained", sharex=True)
@@ -207,15 +210,16 @@
 
         ax = self.plot_ax(ax, df=df, smoothing=smoothing, interval_day=interval_day,
                           y_min=y_min, y_max=y_max)
 
         ax.set_title('{} \n Periode {} - {}'.format(title, start_date, end_date), fontsize=14)
 
         plt.xticks(rotation=45)
-        plt.grid(visible=True, which='both')
+        if show_gridline is True:
+            plt.grid(visible=True, which='both')
 
         if save:
             save_path = os.path.join(self.figures_dir, f'rsam_{self.nslc}_{start_date}_{end_date}_{smoothing}.png')
             fig.savefig(save_path, dpi=300)
             print(f'📈 RSAM Graphics saved to {save_path}')
 
         return fig
```

### Comparing `rsam_ew-1.1.0/PKG-INFO` & `rsam_ew-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsam-ew
-Version: 1.1.0
+Version: 1.2.0
 Summary: Plot RSAM from earthworm files
 Keywords: seismic,volcano,seiscomp,volcanology,seismology,magma indonesia
 Author-email: Martanto <martanto@live.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/beats_swing-0.1.3.tar.gz` & `tmp/beats_swing-0.1.4.tar.gz`

## Comparing `beats_swing-0.1.3.tar` & `beats_swing-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 beats_swing-0.1.3/DEVELOPMENT.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.1.3/Makefile
--rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.1.3/pylintrc
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.1.3/test_requirements.txt
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.github/workflows/build_release.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/explorer.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/first_pass.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/librosa_explorer.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/mess_around_w_librosa.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 beats_swing-0.1.3/scripts/score.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/__init__.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/cli.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/constants.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/filtering.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/shared_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/api.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/librosa.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/trivial.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 beats_swing-0.1.3/src/beats/estimators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/beats/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/beats/test_cli.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.1.3/tests/beats/test_smoke.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.1.3/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 beats_swing-0.1.3/README.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 beats_swing-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 beats_swing-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 beats_swing-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 beats_swing-0.1.4/DEVELOPMENT.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 beats_swing-0.1.4/Makefile
+-rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 beats_swing-0.1.4/pylintrc
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 beats_swing-0.1.4/test_requirements.txt
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 beats_swing-0.1.4/.github/workflows/build_release.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 beats_swing-0.1.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 beats_swing-0.1.4/scripts/explorer.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 beats_swing-0.1.4/scripts/first_pass.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 beats_swing-0.1.4/scripts/librosa_explorer.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 beats_swing-0.1.4/scripts/mess_around_w_librosa.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 beats_swing-0.1.4/scripts/score.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/cli.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/constants.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/filtering.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/shared_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/estimators/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/estimators/api.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/estimators/librosa.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/estimators/transformed.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/estimators/trivial.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 beats_swing-0.1.4/src/beats/estimators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beats_swing-0.1.4/tests/beats/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 beats_swing-0.1.4/tests/beats/test_cli.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 beats_swing-0.1.4/tests/beats/test_smoke.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 beats_swing-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 beats_swing-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 beats_swing-0.1.4/README.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 beats_swing-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 beats_swing-0.1.4/PKG-INFO
```

### Comparing `beats_swing-0.1.3/.pre-commit-config.yaml` & `beats_swing-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/DEVELOPMENT.md` & `beats_swing-0.1.4/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/Makefile` & `beats_swing-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/pylintrc` & `beats_swing-0.1.4/pylintrc`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/test_requirements.txt` & `beats_swing-0.1.4/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/.github/workflows/build_release.yml` & `beats_swing-0.1.4/.github/workflows/build_release.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/.github/workflows/tests.yml` & `beats_swing-0.1.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/scripts/explorer.py` & `beats_swing-0.1.4/scripts/explorer.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/scripts/first_pass.py` & `beats_swing-0.1.4/scripts/first_pass.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/scripts/librosa_explorer.py` & `beats_swing-0.1.4/scripts/librosa_explorer.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/scripts/mess_around_w_librosa.py` & `beats_swing-0.1.4/scripts/mess_around_w_librosa.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/scripts/score.py` & `beats_swing-0.1.4/scripts/score.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,56 +12,65 @@
 
 REQUIREMENTS:
   * the song names have to start with the true tempo,
     for example, `"056_my_slow_song.mp3"`.
 """
 
 import dataclasses
+import functools
 import hashlib
 from pathlib import Path
 from typing import Sequence
 from typing import Tuple
 
 import librosa
 import mlflow
 import mlflow.tracking.fluent as mltrack
 import numpy as np
 import plotly.express as px
 
 from beats.estimators.api import Estimator
 from beats.estimators.librosa import Librosav1
 from beats.estimators.librosa import Librosav2
+from beats.estimators.transformed import Transformed
+from beats.estimators.transformed import cut
 from beats.estimators.trivial import Zero
 from beats.estimators.utils import Metrics
 from beats.estimators.utils import score
 from beats.shared_types import SamplingRate
 from beats.shared_types import Song
 from beats.shared_types import Tempo
 from beats.shared_types import Vector
 
 
+@functools.lru_cache
 def song_from_file(
     audio_file: Path,
-) -> Tuple[Song, SamplingRate, Tempo]:  # TODO: cache?
+) -> Tuple[Song, SamplingRate, Tempo]:
     y, fs = librosa.load(str(audio_file), sr=None)
     # tempo should be encoded as the first 3 characters of the file name;
     # 50 is encoded as 050
     ground_truth_tempo = int(audio_file.name[0:3])
     return Song(y), SamplingRate(fs), Tempo(ground_truth_tempo)
 
 
 MLFLOW_DIR = Path(__file__).parent.parent / "mlflow"
 MP3_DIR = Path(__file__).parent.parent / "data"
 
+BIG_CUT = functools.partial(cut, start_proportion=0.2, end_proportion=0.8)
 ESTIMATORS: Sequence[Estimator] = [
     Zero(),
     Librosav1(),
     Librosav2(),
+    Transformed(transform=cut, estimator=Librosav1()),
+    Transformed(transform=cut, estimator=Librosav2()),
+    Transformed(transform=BIG_CUT, estimator=Librosav1()),
+    Transformed(transform=BIG_CUT, estimator=Librosav2()),
 ]
-DATASET = [f for f in MP3_DIR.iterdir() if f.suffix in [".mp3", ".m4a"]]
+DATASET = [f for f in MP3_DIR.rglob("*") if f.suffix in [".mp3", ".m4a"]]
 SONGS: Sequence[Tuple[Song, SamplingRate, Tempo]] = [song_from_file(d) for d in DATASET]
 
 
 def store(metrics: Metrics, estimator: Estimator, dataset: Sequence[Path]) -> None:
     """Store metrics to the mlflow instance"""
     for k, v in dataclasses.asdict(metrics).items():
         if isinstance(v, (int, float)):
@@ -78,16 +87,18 @@
     for k, v in estimator.params().items():
         mltrack.log_param(k, v)
 
     df = metrics.all_df
     df["name"] = [d.name for d in dataset]
     mltrack.log_table(metrics.all_df, "details.json")
 
+    df["abs_err"] = df["error"].abs()
     mltrack.log_figure(
-        px.scatter(df, x="true", y="pred", hover_data="name"), "true_vs_pred.html"
+        px.scatter(df, x="true", y="pred", hover_data="name", color="abs_err"),
+        "true_vs_pred.html",
     )
 
 
 def pipeline() -> None:
     mlflow.set_tracking_uri(f"file://{MLFLOW_DIR}")
     mltrack.set_experiment("tempo-tracking")
```

### Comparing `beats_swing-0.1.3/src/beats/cli.py` & `beats_swing-0.1.4/src/beats/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from typing import Tuple
 
 import librosa
 
 from beats.constants import SUPPORTED_FORMATS
 from beats.estimators.librosa import Librosav2
+from beats.estimators.transformed import Transformed, cut
 from beats.shared_types import SamplingRate
 from beats.shared_types import Song
 from beats.shared_types import Tempo
 
 
 @dataclasses.dataclass
 class Args:
@@ -50,15 +51,15 @@
     y, fs = librosa.load(str(audio_file), sr=None)
     return Song(y), SamplingRate(fs)
 
 
 def estimate_tempo(audio_file: Path) -> Tempo:
     """Estimate the tempo of a song at the specified file."""
     song, fs = _song_from_file(audio_file)
-    tempo = Librosav2().tempo(song, fs)
+    tempo = Transformed(transform=cut, estimator=Librosav2()).tempo(song, fs)
     return tempo
 
 
 def main() -> None:
     """Print the estimated tempo to stdout."""
     args = _parse_args()
     tempo = estimate_tempo(args.music_file)
```

### Comparing `beats_swing-0.1.3/src/beats/filtering.py` & `beats_swing-0.1.4/src/beats/filtering.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/src/beats/estimators/api.py` & `beats_swing-0.1.4/src/beats/estimators/api.py`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/src/beats/estimators/librosa.py` & `beats_swing-0.1.4/src/beats/estimators/librosa.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,96 @@
 """Librosa-based tempo estimators."""
 
 from typing import Mapping
 
 import librosa
+import numpy as np
+from librosa import onset
 
 from beats.estimators.api import Estimator
 from beats.shared_types import SamplingRate
 from beats.shared_types import Song
 from beats.shared_types import Tempo
 
 
 class Librosav1(Estimator):
     """Tempo estimator using `librosa.beat.beat_track`."""
 
-    def __init__(self, start_bpm: float = 120.0, tightness: float = 100.0):
+    def __init__(self, start_bpm: float = 120.0, max_tempo: float = 350.0):
         self._start_bpm = start_bpm
-        self._tightness = tightness
+        self._max_tempo = max_tempo
 
     def tempo(self, song: Song, fs: SamplingRate) -> Tempo:
-        tempo, _ = librosa.beat.beat_track(
-            y=song, sr=fs, start_bpm=self._start_bpm, tightness=self._tightness
+        onset_envelope = onset.onset_strength(
+            y=song,
+            sr=fs,
+            hop_length=512,
+            aggregate=np.median,
+            # constants from librosa.beat.beat_track
+        )
+        tempo = float(
+            librosa.beat.tempo(
+                y=song,
+                sr=fs,
+                start_bpm=self._start_bpm,
+                max_tempo=self._max_tempo,
+                onset_envelope=onset_envelope,
+            )
         )
         return Tempo(float(tempo))
 
     def params(self) -> Mapping[str, str | float | int]:
         return {
             "start_bpm": self._start_bpm,
-            "tightness": self._tightness,
+            "max_tempo": self._max_tempo,
         }
 
 
 class Librosav2(Estimator):
     """Tempo estimator using `librosa.beat.beat_track`.
     It takes the initial guess of the tempo and seeds another search with it.
     We retain the higher guess out of the two.
 
     This approach seems to be surprisingly good at picking out harmonics.
     """
 
-    def __init__(self, start_bpm: float = 120.0, tightness: float = 100.0):
+    def __init__(self, start_bpm: float = 120.0, max_tempo: float = 350.0):
         self._start_bpm = start_bpm
-        self._tightness = tightness
+        self._max_tempo = max_tempo
 
     def tempo(self, song: Song, fs: SamplingRate) -> Tempo:
-        tempo, _ = librosa.beat.beat_track(
-            y=song, sr=fs, start_bpm=self._start_bpm, tightness=self._tightness
+        onset_envelope = onset.onset_strength(
+            y=song,
+            sr=fs,
+            hop_length=512,
+            aggregate=np.median,
+            # constants from librosa.beat.beat_track
+        )
+        tempo = float(
+            librosa.beat.tempo(
+                y=song,
+                sr=fs,
+                start_bpm=self._start_bpm,
+                max_tempo=self._max_tempo,
+                onset_envelope=onset_envelope,
+            )
         )
-        tempo2, _ = librosa.beat.beat_track(
-            y=song, sr=fs, start_bpm=float(tempo) * 2, tightness=self._tightness
+
+        tempo2 = float(
+            librosa.beat.tempo(
+                y=song,
+                sr=fs,
+                start_bpm=float(tempo) * 2,
+                max_tempo=self._max_tempo,
+                onset_envelope=onset_envelope,
+            )
         )
         if tempo2 >= 1.8 * tempo:
-            return Tempo(float(tempo2))
+            return Tempo(tempo2)
         else:
-            return Tempo(float(tempo))
+            return Tempo(tempo)
 
     def params(self) -> Mapping[str, str | float | int]:
         return {
             "start_bpm": self._start_bpm,
-            "tightness": self._tightness,
+            "max_tempo": self._max_tempo,
         }
```

### Comparing `beats_swing-0.1.3/src/beats/estimators/utils.py` & `beats_swing-0.1.4/src/beats/estimators/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class Metrics:
     """A container with various performance metrics."""
 
     mean_squared_error: float
     root_mean_squared_error: float
     mean_absolute_error: float
     r_squared: float
+    num_off_by_5: int
 
     all_df: pd.DataFrame
 
 
 def score(predictions: Vector, ground_truth: Vector) -> Metrics:
     df = pd.DataFrame({"pred": predictions, "true": ground_truth})
 
@@ -28,8 +29,9 @@
     mse = float(np.square(df["error"].values).mean())
     return Metrics(
         mean_squared_error=mse,
         root_mean_squared_error=float(np.sqrt(mse)),
         mean_absolute_error=float(abs(df["error"].mean())),
         r_squared=r2_score(df["pred"], df["true"]),
         all_df=df,
+        num_off_by_5=len(df[df["error"].abs() > 5]),
     )
```

### Comparing `beats_swing-0.1.3/.gitignore` & `beats_swing-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/LICENSE.txt` & `beats_swing-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/README.md` & `beats_swing-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `beats_swing-0.1.3/pyproject.toml` & `beats_swing-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "beats_swing"
-version = "0.1.3"
+version = "0.1.4"
 description = "Determine the tempo of an mp3 song. Tweaked for swing music."
 authors = [
     {name = "Elvijs Sarkans", email = "elvijs.sarkans@gmail.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `beats_swing-0.1.3/PKG-INFO` & `beats_swing-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beats_swing
-Version: 0.1.3
+Version: 0.1.4
 Summary: Determine the tempo of an mp3 song. Tweaked for swing music.
 Project-URL: repository, https://github.com/elvijs/beats
 Project-URL: homepage, https://github.com/elvijs/beats
 Project-URL: issues, https://github.com/elvijs/beats/issues
 Author-email: Elvijs Sarkans <elvijs.sarkans@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
```


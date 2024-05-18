# Comparing `tmp/time_split-0.2.1.tar.gz` & `tmp/time_split-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_split-0.2.1.tar", max compression
+gzip compressed data, was "time_split-0.3.0.tar", max compression
```

## Comparing `time_split-0.2.1.tar` & `time_split-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1077 2024-04-20 17:44:39.846115 time_split-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     3248 2024-04-20 17:44:39.846115 time_split-0.2.1/README.md
--rw-r--r--   0        0        0     4772 2024-04-20 17:44:39.850115 time_split-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      342 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/__init__.py
--rw-r--r--   0        0        0      351 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_backend/__init__.py
--rw-r--r--   0        0        0      496 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_backend/_datetime_index_like.py
--rw-r--r--   0        0        0     4932 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_backend/_limits.py
--rw-r--r--   0        0        0     2220 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_backend/_process_available.py
--rw-r--r--   0        0        0     2666 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_backend/_schedule.py
--rw-r--r--   0        0        0     3744 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_backend/_span.py
--rw-r--r--   0        0        0     5712 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_backend/_splitter.py
--rw-r--r--   0        0        0     1560 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_docstrings.py
--rw-r--r--   0        0        0      261 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_frontend/__init__.py
--rw-r--r--   0        0        0    11750 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_frontend/_plot.py
--rw-r--r--   0        0        0     5087 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_frontend/_progress.py
--rw-r--r--   0        0        0     1089 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_frontend/_split.py
--rw-r--r--   0        0        0     3001 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_frontend/_to_string.py
--rw-r--r--   0        0        0     2163 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_frontend/_weight.py
--rw-r--r--   0        0        0      420 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/_support.py
--rw-r--r--   0        0        0       62 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/__init__.py
--rw-r--r--   0        0        0      953 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/_log_progress.py
--rw-r--r--   0        0        0     1808 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/pandas/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/pandas/_impl.py
--rw-r--r--   0        0        0     2424 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/polars/__init__.py
--rw-r--r--   0        0        0     1867 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/polars/_impl.py
--rw-r--r--   0        0        0      131 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/sklearn/__init__.py
--rw-r--r--   0        0        0     5711 2024-04-20 17:44:39.850115 time_split-0.2.1/src/time_split/integration/sklearn/_impl.py
--rw-r--r--   0        0        0     3001 2024-04-20 17:44:39.854115 time_split-0.2.1/src/time_split/integration/split_data.py
--rw-r--r--   0        0        0        0 2024-04-20 17:44:39.854115 time_split-0.2.1/src/time_split/py.typed
--rw-r--r--   0        0        0     6333 2024-04-20 17:44:39.854115 time_split-0.2.1/src/time_split/settings.py
--rw-r--r--   0        0        0      652 2024-04-20 17:44:39.854115 time_split-0.2.1/src/time_split/support/__init__.py
--rw-r--r--   0        0        0      250 2024-04-20 17:44:39.854115 time_split-0.2.1/src/time_split/support/types.py
--rw-r--r--   0        0        0     2218 2024-04-20 17:44:39.854115 time_split-0.2.1/src/time_split/types.py
--rw-r--r--   0        0        0     4600 1970-01-01 00:00:00.000000 time_split-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-18 18:13:13.983766 time_split-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     3248 2024-05-18 18:13:13.983766 time_split-0.3.0/README.md
+-rw-r--r--   0        0        0     4789 2024-05-18 18:13:13.987766 time_split-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      342 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_backend/__init__.py
+-rw-r--r--   0        0        0      496 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_backend/_datetime_index_like.py
+-rw-r--r--   0        0        0     4932 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_backend/_limits.py
+-rw-r--r--   0        0        0     2220 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_backend/_process_available.py
+-rw-r--r--   0        0        0     2666 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_backend/_schedule.py
+-rw-r--r--   0        0        0     3744 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_backend/_span.py
+-rw-r--r--   0        0        0     5712 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_backend/_splitter.py
+-rw-r--r--   0        0        0     1560 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_docstrings.py
+-rw-r--r--   0        0        0      321 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_frontend/__init__.py
+-rw-r--r--   0        0        0    11750 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_frontend/_plot.py
+-rw-r--r--   0        0        0    10370 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_frontend/_progress.py
+-rw-r--r--   0        0        0     1089 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_frontend/_split.py
+-rw-r--r--   0        0        0     3001 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_frontend/_to_string.py
+-rw-r--r--   0        0        0     2163 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_frontend/_weight.py
+-rw-r--r--   0        0        0      420 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/_support.py
+-rw-r--r--   0        0        0       62 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/__init__.py
+-rw-r--r--   0        0        0      993 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/_log_progress.py
+-rw-r--r--   0        0        0     3019 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/base.py
+-rw-r--r--   0        0        0     1808 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/pandas/__init__.py
+-rw-r--r--   0        0        0     2778 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/pandas/_impl.py
+-rw-r--r--   0        0        0     2424 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/polars/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/polars/_impl.py
+-rw-r--r--   0        0        0      131 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/sklearn/__init__.py
+-rw-r--r--   0        0        0     5741 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/integration/sklearn/_impl.py
+-rw-r--r--   0        0        0        0 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/py.typed
+-rw-r--r--   0        0        0     6459 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/settings.py
+-rw-r--r--   0        0        0      712 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/support/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/support/types.py
+-rw-r--r--   0        0        0     3660 2024-05-18 18:13:13.991766 time_split-0.3.0/src/time_split/types.py
+-rw-r--r--   0        0        0     4600 1970-01-01 00:00:00.000000 time_split-0.3.0/PKG-INFO
```

### Comparing `time_split-0.2.1/LICENSE.md` & `time_split-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/README.md` & `time_split-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/pyproject.toml` & `time_split-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "time-split"
-version = "0.2.1"
+version = "0.3.0"
 description = "Time-based k-fold validation splits for heterogeneous data."
 authors = ["Richard Sundqvist <richard.sundqvist@live.se>"]
 
 readme = "README.md"
 homepage = "https://github.com/rsundqvist/time-split"
 repository = "https://github.com/rsundqvist/time-split"
 documentation = "https://time-split.readthedocs.io"
@@ -42,26 +42,26 @@
 
 [tool.poetry.extras]
 plotting = ["matplotlib", "seaborn"]
 
 [tool.poetry.group.manual-extras.dependencies]
 # Extras that must be available for docs + tests go here. Doc/test-only deps go in their respective groups.
 croniter = "^2.0.3"
-pyarrow = "^15.0.2"
+pyarrow = ">=15.0.2,<17.0.0"
 polars = { version = "^0.20.19", extras = ["pandas"] }
 
 [tool.poetry.group.docs]
 [tool.poetry.group.docs.dependencies]
 # duplicate object warnings for sphinx>=4
 # description: https://github.com/astropy/astropy/issues/11723
 # https://github.com/astropy/astropy/pull/12270
 sphinx = "^7.2.6"
-sphinx-gallery = "^0.15.0"
+sphinx-gallery = "^0.16.0"
 pydata-sphinx-theme = "^0.15.2"
-myst-parser = "^2.0.0"
+myst-parser = ">=2,<4"
 nbsphinx = "^0.9.3"
 ipython = "^8.23.0"
 
 [tool.poetry.group.notebooks]
 optional = true
 [tool.poetry.group.notebooks.dependencies]
 jupyterlab = "^4"
@@ -76,20 +76,20 @@
 pytest-cov = "^5.0.0"
 
 scikit-learn = "^1.4.2"
 # TODO Unpin.
 # dask.datasets.timeseries() warns:
 #     UserWarning: dask_expr does not support the DataFrameIOFunction protocol for column projection
 # on dask == 2024.3.1
-dask = { version = "==2024.4.1", extras = ["dataframe"] }
+dask = { version = "==2024.5.0", extras = ["dataframe"] }
 
 [tool.poetry.group.devops.dependencies]
 invoke = "^2.2.0"
 mypy = "^1.9.0"
-ruff = "^0.3.7"
+ruff = ">=0.3.7,<0.5.0"
 
 safety = "^3.1.0"
 codespell = "^2.2.6"
 bump2version = "^1.0.1"
 
 [tool.ruff]
 line-length = 120
```

### Comparing `time_split-0.2.1/src/time_split/_backend/_limits.py` & `time_split-0.3.0/src/time_split/_backend/_limits.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_backend/_process_available.py` & `time_split-0.3.0/src/time_split/_backend/_process_available.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_backend/_schedule.py` & `time_split-0.3.0/src/time_split/_backend/_schedule.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_backend/_span.py` & `time_split-0.3.0/src/time_split/_backend/_span.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_backend/_splitter.py` & `time_split-0.3.0/src/time_split/_backend/_splitter.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_docstrings.py` & `time_split-0.3.0/src/time_split/_docstrings.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_frontend/_plot.py` & `time_split-0.3.0/src/time_split/_frontend/_plot.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_frontend/_split.py` & `time_split-0.3.0/src/time_split/_frontend/_split.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_frontend/_to_string.py` & `time_split-0.3.0/src/time_split/_frontend/_to_string.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/_frontend/_weight.py` & `time_split-0.3.0/src/time_split/_frontend/_weight.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/integration/_log_progress.py` & `time_split-0.3.0/src/time_split/integration/_log_progress.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 from collections.abc import Iterable
-from typing import Any, Union
+from typing import Any
 
 from .. import log_split_progress
 from .._docstrings import add_docstrings
-from ..types import DatetimeSplitBounds, DatetimeSplits
+from ..types import DatetimeSplitBounds, DatetimeSplits, LogSplitProgressKwargs, MetricsType
 
-LogProgressArg = Union[str, bool, dict[str, Any], logging.Logger, logging.LoggerAdapter]  # type: ignore[type-arg]
+LogProgressArg = str | bool | logging.Logger | logging.LoggerAdapter[Any] | LogSplitProgressKwargs[MetricsType]
 
 add_docstrings(log_progress="Controls logging of fold progress. See :func:`~.log_split_progress` for details.")
 
 
 def handle_log_progress_arg(
-    log_progress: LogProgressArg, *, splits: DatetimeSplits
+    log_progress: LogProgressArg[MetricsType], *, splits: DatetimeSplits
 ) -> Iterable[DatetimeSplitBounds] | None:
     """Wrapper function for integrations."""
     if log_progress is True:
         return log_split_progress(splits)
     elif isinstance(log_progress, (str, logging.Logger, logging.LoggerAdapter)):
         return log_split_progress(splits, logger=log_progress)
     elif isinstance(log_progress, dict):
```

### Comparing `time_split-0.2.1/src/time_split/integration/pandas/__init__.py` & `time_split-0.3.0/src/time_split/integration/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/integration/pandas/_impl.py` & `time_split-0.3.0/src/time_split/integration/pandas/_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from datetime import date, datetime
 from typing import Generic, TypeVar, Unpack
 
 from pandas import DataFrame, DatetimeIndex, Series, Timestamp
 from rics.misc import tname
 
 from ..._docstrings import docs
-from ...types import DatetimeIndexSplitterKwargs
+from ...types import DatetimeIndexSplitterKwargs, MetricsType
 from .._log_progress import LogProgressArg
-from ..split_data import DatetimeSplit, split_data
+from ..base import DatetimeSplit, split_data
 
 PandasT = TypeVar("PandasT", Series, DataFrame)
 """A splittable pandas type."""
 
 
 @docs
 def split_pandas(
     data: PandasT,
     time_column: Hashable = None,
     *,
-    log_progress: LogProgressArg = False,
+    log_progress: LogProgressArg[MetricsType] = False,
     **kwargs: Unpack[DatetimeIndexSplitterKwargs],
 ) -> Iterable[DatetimeSplit[PandasT]]:
     """Split a pandas type.
 
     This function splits indexed data (i.e. ``Series`` and ``DataFrame``), not the index itself. Use
     :func:`time_split.split` for pandas ``Index`` types, setting ``available=data.index``.
```

### Comparing `time_split-0.2.1/src/time_split/integration/polars/__init__.py` & `time_split-0.3.0/src/time_split/integration/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `time_split-0.2.1/src/time_split/integration/polars/_impl.py` & `time_split-0.3.0/src/time_split/integration/polars/_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from datetime import date, datetime
 from typing import Unpack
 
 from polars import DataFrame, Series
 from rics.misc import tname
 
 from ..._docstrings import docs
-from ...types import DatetimeIndexSplitterKwargs
+from ...types import DatetimeIndexSplitterKwargs, MetricsType
 from .._log_progress import LogProgressArg
-from ..split_data import DatetimeSplit, split_data
+from ..base import DatetimeSplit, split_data
 
 
 @docs
 def split_polars(
     data: DataFrame,
     time_column: str,
     *,
-    log_progress: LogProgressArg = False,
+    log_progress: LogProgressArg[MetricsType] = False,
     **kwargs: Unpack[DatetimeIndexSplitterKwargs],
 ) -> Iterable[DatetimeSplit[DataFrame]]:
     """Split a polars frame.
 
     Args:
         data: A ``polars.DataFrame``.
         time_column: A column to split on.
```

### Comparing `time_split-0.2.1/src/time_split/integration/sklearn/_impl.py` & `time_split-0.3.0/src/time_split/integration/sklearn/_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ..._backend import DatetimeIndexSplitter
 from ..._docstrings import docs
 from ...types import (
     DatetimeIterable,
     DatetimeSplits,
     DatetimeTypes,
     Flex,
+    MetricsType,
     Schedule,
     Span,
 )
 from .._log_progress import LogProgressArg, handle_log_progress_arg
 
 try:
     from sklearn.model_selection import BaseCrossValidator  # type: ignore[import-untyped]
@@ -56,15 +57,15 @@
         schedule: Schedule,
         *,
         before: Span = "7d",
         after: Span = 1,
         n_splits: int = 0,
         flex: Flex = "auto",
         step: int = 1,
-        log_progress: LogProgressArg = False,
+        log_progress: LogProgressArg[MetricsType] = False,
         verify_xy: bool = True,
     ) -> None:
         super().__init__()
         self._splitter = DatetimeIndexSplitter(
             schedule,
             before=before,
             after=after,
```

### Comparing `time_split-0.2.1/src/time_split/integration/split_data.py` & `time_split-0.3.0/src/time_split/integration/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return self.bounds.mid
 
 
 @_docs
 def split_data(
     data: DataT,
     *,
-    log_progress: _log_progress.LogProgressArg = False,
+    log_progress: _log_progress.LogProgressArg[_tst.MetricsType] = False,
     as_available: DataAsAvailableFn[DataT],
     select: DataSelectFn[DataT],
     **kwargs: _t.Unpack[_tst.DatetimeIndexSplitterKwargs],
 ) -> _t.Iterable[DatetimeSplit[DataT]]:
     """Base implementation for splitting integrated `data` types.
 
     The required ``as_available`` and ``select`` callables provided perform the actual integration.
```

### Comparing `time_split-0.2.1/src/time_split/settings.py` & `time_split-0.3.0/src/time_split/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,19 +109,18 @@
 
     .. code-block:: python
        :caption: Sample output.
 
        '2021-12-30' <= [schedule: '2022-01-04' (Tuesday)] < '2022-01-04 18:00:00'
     """
 
-    SECONDS_FORMATTER: str | _t.Callable[[float], str] = "rics.performance.format_seconds"
-    """A callable ``(seconds) -> formatted_seconds``.
+    SECONDS_FORMATTER: _t.Callable[[float], str] | None = None
+    """A callable ``(seconds) -> formatted_seconds``. Use :func:`rics.performance.format_seconds` if ``None``.
 
-    Both ``seconds`` and ``formatted_seconds`` will be available to the :attr:`END_MESSAGE` message. If a string is
-    given, the actual callable will be resolved using :func:`rics.misc.get_by_full_name`.
+    Both ``seconds`` and ``formatted_seconds`` will be available to the :attr:`END_MESSAGE` message.
     """
 
     START_MESSAGE: str = "Begin fold {n}/{n_splits}: {fold}."
     """Message indicating that the current fold has been yielded to the user.
 
     Has access to all keys from the previous section, as well as:
 
@@ -152,14 +151,17 @@
     """
 
     AUTO_DATE_FORMAT = "%Y-%m-%d"
     """Short-form timestamp format_spec used by ``<key>.auto``."""
     AUTO_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
     """Long-form timestamp format_spec used by ``<key>.auto``."""
 
+    FORMAT_METRICS: _tst.FormatMetrics[_t.Any] | None = None
+    """A callable ``(end_message, metrics) -> str``. Use the :func:`default formatter <.support.default_metrics_formatter>` if ``None``."""
+
 
 class misc:  # noqa: N801
     """Miscellaneous settings that don't fit in any other namespace."""
 
     snap_to_end: bool = True
     """Controls alignment of timedelta-based splits.
```

### Comparing `time_split-0.2.1/src/time_split/support/__init__.py` & `time_split-0.3.0/src/time_split/support/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,17 @@
    Not part of the stable API.
 
 This module may change without notice. Stick to the top-level :mod:`time_split`-module, or lock down your
 dependencies if you need to use the ``support`` module.
 """
 
 from .._backend import DatetimeIndexSplitter, expand_limits, process_available
-from .._frontend import fold_weight, to_string
+from .._frontend import default_metrics_formatter, fold_weight, to_string
 
 __all__ = [
     "DatetimeIndexSplitter",
     "expand_limits",
     "process_available",
+    "default_metrics_formatter",
     "fold_weight",
     "to_string",
 ]
```

### Comparing `time_split-0.2.1/PKG-INFO` & `time_split-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-split
-Version: 0.2.1
+Version: 0.3.0
 Summary: Time-based k-fold validation splits for heterogeneous data.
 Home-page: https://github.com/rsundqvist/time-split
 Author: Richard Sundqvist
 Author-email: richard.sundqvist@live.se
 Requires-Python: >=3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


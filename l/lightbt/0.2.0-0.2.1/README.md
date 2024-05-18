# Comparing `tmp/lightbt-0.2.0.tar.gz` & `tmp/lightbt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Users\Kan\Documents\GitHub\LightBT\dist\.tmp-m0t7x80w\lightbt-0.2.0.tar", last modified: Wed Aug 23 13:07:49 2023, max compression
+gzip compressed data, was "D:\Users\Kan\Documents\GitHub\LightBT\dist\.tmp-uxukx6zp\lightbt-0.2.1.tar", last modified: Sun Oct  1 12:41:47 2023, max compression
```

## Comparing `lightbt-0.2.0.tar` & `lightbt-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-23 13:07:49.691857 lightbt-0.2.0/
--rw-rw-rw-   0        0        0     1083 2023-08-12 11:48:10.000000 lightbt-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     5724 2023-08-23 13:07:49.690855 lightbt-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5376 2023-08-23 11:48:30.000000 lightbt-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-23 13:07:49.600144 lightbt-0.2.0/lightbt/
--rw-rw-rw-   0        0        0       70 2023-08-13 12:05:50.000000 lightbt-0.2.0/lightbt/__init__.py
--rw-rw-rw-   0        0        0       23 2023-08-23 12:36:14.000000 lightbt-0.2.0/lightbt/_version.py
--rw-rw-rw-   0        0        0    10185 2023-08-23 11:48:30.000000 lightbt-0.2.0/lightbt/base.py
--rw-rw-rw-   0        0        0     1294 2023-08-18 16:07:26.000000 lightbt-0.2.0/lightbt/callbacks.py
--rw-rw-rw-   0        0        0     5989 2023-08-23 12:36:14.000000 lightbt-0.2.0/lightbt/enums.py
--rw-rw-rw-   0        0        0    17009 2023-08-23 09:12:29.000000 lightbt-0.2.0/lightbt/portfolio.py
--rw-rw-rw-   0        0        0    15317 2023-08-18 15:32:01.000000 lightbt-0.2.0/lightbt/position.py
--rw-rw-rw-   0        0        0     4317 2023-08-23 08:59:41.000000 lightbt-0.2.0/lightbt/signals.py
--rw-rw-rw-   0        0        0     9606 2023-08-23 12:42:04.000000 lightbt-0.2.0/lightbt/stats.py
--rw-rw-rw-   0        0        0     2009 2023-08-23 12:56:26.000000 lightbt-0.2.0/lightbt/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-23 13:07:49.686857 lightbt-0.2.0/lightbt.egg-info/
--rw-rw-rw-   0        0        0     5724 2023-08-23 13:07:49.000000 lightbt-0.2.0/lightbt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-08-23 13:07:49.000000 lightbt-0.2.0/lightbt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-23 13:07:49.000000 lightbt-0.2.0/lightbt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-23 13:07:49.000000 lightbt-0.2.0/lightbt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-23 13:07:49.000000 lightbt-0.2.0/lightbt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      613 2023-08-18 09:28:51.000000 lightbt-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-23 13:07:49.692857 lightbt-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-07-31 04:54:16.000000 lightbt-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-01 12:41:47.492049 lightbt-0.2.1/
+-rw-rw-rw-   0        0        0     1083 2023-08-12 11:48:10.000000 lightbt-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5754 2023-10-01 12:41:47.492049 lightbt-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5376 2023-08-23 11:48:30.000000 lightbt-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-10-01 12:41:47.476420 lightbt-0.2.1/lightbt/
+-rw-rw-rw-   0        0        0       70 2023-08-13 12:05:50.000000 lightbt-0.2.1/lightbt/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-10-01 11:52:34.000000 lightbt-0.2.1/lightbt/_version.py
+-rw-rw-rw-   0        0        0    10194 2023-10-01 11:46:48.000000 lightbt-0.2.1/lightbt/base.py
+-rw-rw-rw-   0        0        0     1294 2023-08-18 16:07:26.000000 lightbt-0.2.1/lightbt/callbacks.py
+-rw-rw-rw-   0        0        0     6241 2023-10-01 11:52:34.000000 lightbt-0.2.1/lightbt/enums.py
+-rw-rw-rw-   0        0        0    17739 2023-10-01 11:46:48.000000 lightbt-0.2.1/lightbt/portfolio.py
+-rw-rw-rw-   0        0        0    15317 2023-08-18 15:32:01.000000 lightbt-0.2.1/lightbt/position.py
+-rw-rw-rw-   0        0        0     5091 2023-10-01 12:30:05.000000 lightbt-0.2.1/lightbt/signals.py
+-rw-rw-rw-   0        0        0     9606 2023-08-23 12:42:04.000000 lightbt-0.2.1/lightbt/stats.py
+-rw-rw-rw-   0        0        0     2009 2023-08-23 12:56:26.000000 lightbt-0.2.1/lightbt/utils.py
+drwxrwxrwx   0        0        0        0 2023-10-01 12:41:47.492049 lightbt-0.2.1/lightbt.egg-info/
+-rw-rw-rw-   0        0        0     5754 2023-10-01 12:41:47.000000 lightbt-0.2.1/lightbt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-10-01 12:41:47.000000 lightbt-0.2.1/lightbt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-01 12:41:47.000000 lightbt-0.2.1/lightbt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-10-01 12:41:47.000000 lightbt-0.2.1/lightbt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-10-01 12:41:47.000000 lightbt-0.2.1/lightbt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      613 2023-08-18 09:28:51.000000 lightbt-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-10-01 12:41:47.492049 lightbt-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-07-31 04:54:16.000000 lightbt-0.2.1/setup.py
```

### Comparing `lightbt-0.2.0/LICENSE` & `lightbt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightbt-0.2.0/PKG-INFO` & `lightbt-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lightbt
-Version: 0.2.0
+Version: 0.2.1
 Summary: lightweight backtester
 Author-email: wukan <wu-kan@163.com>
 License: BSD-3-Clause
 Keywords: backtest
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numba>=0.57.1
 
 # LightBT
 轻量级回测工具
 
 ## 注意
 每种工具都有其适合的应用场景。遇到需要快速评测大批量参数或因子的场景，我们只要相对准确。所以使用对数收益累加更合适
```

### Comparing `lightbt-0.2.0/README.md` & `lightbt-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lightbt-0.2.0/lightbt/base.py` & `lightbt-0.2.1/lightbt/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self.mapping_asset_int = {}
         self.mapping_int_asset = {}
         self.conf: pd.DataFrame = pd.DataFrame()
 
     def reset(self):
         """重置。不需要再次`setup`，只需要重新跑一次`run_`即可"""
         self.pf.reset()
-        # 入金
+        # 入初始资金
         self.deposit(self._init_cash)
 
     def setup(self, df: pd.DataFrame) -> None:
         """映射资产，配置合约乘数和保证金率
 
         同名的会进行替换
```

### Comparing `lightbt-0.2.0/lightbt/callbacks.py` & `lightbt-0.2.1/lightbt/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightbt-0.2.0/lightbt/enums.py` & `lightbt-0.2.1/lightbt/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,22 @@
     Percent: int = 4
     # 目标数量和方向
     TargetAmount: int = 5
     # 目标市值和方向
     TargetValue: int = 6
     # 目标保证金和方向
     TargetMargin: int = 7
-    # 目标市值占比
+    # 目标市值百分比。size绝对值之和范围[0,1]
     TargetPercentValue: int = 8
-    # 目标保证金占比
-    TargetPercentMargin: int = 9
+    # 目标市值比例。size值可能为1.5:1:-1等
+    TargetScaleValue: int = 9
+    # 目标保证金百分比。size绝对值之和范围[0,1]
+    TargetPercentMargin: int = 10
+    # 目标保证金比例。size值可能为1.5:1:-1等
+    TargetScaleMargin: int = 11
 
 
 SizeType = SizeTypeT()
 
 # 绩效统计。为减少内存，使用float32
 performance_dt = np.dtype([
     ('date', np.int64),  # 日期时间
```

### Comparing `lightbt-0.2.0/lightbt/portfolio.py` & `lightbt-0.2.1/lightbt/portfolio.py`

 * *Files 5% similar despite different names*

```diff
@@ -251,17 +251,19 @@
         qty: float
 
         Returns
         -------
         bool
 
         """
-        if qty <= 0.0:
-            # 数量不合法，返回。可用于刷新行情但不产生交易记录
-            return False
+        # convert_size时已经过滤了不合法的数量，所以这里注释了
+
+        # if qty <= 0.0:
+        #     # 数量不合法，返回。可用于刷新行情但不产生交易记录
+        #     return False
 
         pos: Position = self._positions[asset]
         # 成交价所对应的市值和手续费
         value = pos.calc_value(fill_price, qty)
         commission = pos.calc_commission(is_buy, is_open, value, qty)
         if is_open:
             # 可开手数检查
@@ -294,19 +296,33 @@
         # asset不能出现重复
         _rs: np.ndarray = self._position_records[asset]
         margin_ratio: np.ndarray = _rs['margin_ratio']
         amount: np.ndarray = _rs['amount']
         mult: np.ndarray = _rs['mult']
 
         # 以下的操作size为nan时最终还是nan, 所以可以用来标记只更新最新价
+        if size_type == SizeType.TargetScaleMargin:
+            size = size / np.nansum(np.abs(size))
+            _equity: float = self.Equity
+            size = _equity * size / margin_ratio
+            size_type = SizeType.TargetValue
         if size_type == SizeType.TargetPercentMargin:
             # 总权益转分别使用保证金再转市值
             _equity: float = self.Equity * np.nansum(np.abs(size))
             size = _equity * size / margin_ratio
             size_type = SizeType.TargetValue
+        if size_type == SizeType.TargetScaleValue:
+            size = size / np.nansum(np.abs(size))
+            _equity: float = self.Equity
+            _ratio: float = np.nansum((np.abs(size) * margin_ratio))
+            if _ratio == 0:
+                size = _equity * size
+            else:
+                size = _equity / _ratio * size
+            size_type = SizeType.TargetValue
         if size_type == SizeType.TargetPercentValue:
             # 总权益除保证金率占比，得到总市值，然后得到分别市值
             _equity: float = self.Equity * np.nansum(np.abs(size))
             _ratio: float = np.nansum((np.abs(size) * margin_ratio))
             if _ratio == 0:
                 size = _equity * size
             else:
```

### Comparing `lightbt-0.2.0/lightbt/position.py` & `lightbt-0.2.1/lightbt/position.py`

 * *Files identical despite different names*

### Comparing `lightbt-0.2.0/lightbt/signals.py` & `lightbt-0.2.1/lightbt/signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -147,10 +147,39 @@
 
     """
     # 全体数据排序，并复制
     df = df.sort_values(by=['date'])
 
     # 按日期标记，每段的最后一条标记为True。一定要提前排序
     date_0 = df['date'].dt.date
-    df['date_diff'] = date_0 != date_0.shift(-1)
+    df['date_diff'] = date_0 != date_0.shift(-1, fill_value=0)
+
+    return df
+
+
+def orders_weekly(df: pd.DataFrame) -> pd.DataFrame:
+    """
+
+    Parameters
+    ----------
+    df
+
+    Returns
+    -------
+    pd.DataFrame
+        1. 已经按时间进行了排序。sort_values
+        2. 添加了日期标记，用于触发内部的绩效快照
+
+    Notes
+    -----
+    有多处修改了数据，所以需要`copy`。`sort_values`隐含了`copy`
+
+    """
+    # 全体数据排序，并复制
+    df = df.sort_values(by=['date'])
+
+    # 按日期标记，每段的最后一条标记为True。一定要提前排序
+    date_0 = df['date'].dt.isocalendar().week
+    # week的范围是1~52，所以可以fill_value写0 或>52的值
+    df['date_diff'] = date_0 != date_0.shift(-1, fill_value=99)
 
     return df
```

### Comparing `lightbt-0.2.0/lightbt/stats.py` & `lightbt-0.2.1/lightbt/stats.py`

 * *Files identical despite different names*

### Comparing `lightbt-0.2.0/lightbt/utils.py` & `lightbt-0.2.1/lightbt/utils.py`

 * *Files identical despite different names*

### Comparing `lightbt-0.2.0/lightbt.egg-info/PKG-INFO` & `lightbt-0.2.1/lightbt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lightbt
-Version: 0.2.0
+Version: 0.2.1
 Summary: lightweight backtester
 Author-email: wukan <wu-kan@163.com>
 License: BSD-3-Clause
 Keywords: backtest
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numba>=0.57.1
 
 # LightBT
 轻量级回测工具
 
 ## 注意
 每种工具都有其适合的应用场景。遇到需要快速评测大批量参数或因子的场景，我们只要相对准确。所以使用对数收益累加更合适
```

### Comparing `lightbt-0.2.0/pyproject.toml` & `lightbt-0.2.1/pyproject.toml`

 * *Files identical despite different names*


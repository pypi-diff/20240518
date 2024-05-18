# Comparing `tmp/goto_conversion-0.3.0.tar.gz` & `tmp/goto_conversion-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goto_conversion-0.3.0.tar", last modified: Thu May  2 09:49:03 2024, max compression
+gzip compressed data, was "goto_conversion-0.3.1.tar", last modified: Sat May 18 04:44:30 2024, max compression
```

## Comparing `goto_conversion-0.3.0.tar` & `goto_conversion-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.291061 goto_conversion-0.3.0/
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1073 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/LICENSE.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)     6895 2024-05-02 09:49:03.290870 goto_conversion-0.3.0/PKG-INFO
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     6348 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/README.md
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)      614 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/pyproject.toml
--rw-r--r--   0 gotoukaijin   (501) staff       (20)       38 2024-05-02 09:49:03.291103 goto_conversion-0.3.0/setup.cfg
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.289043 goto_conversion-0.3.0/src/
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.289740 goto_conversion-0.3.0/src/goto_conversion/
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1639 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/src/goto_conversion/__init__.py
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.290626 goto_conversion-0.3.0/src/goto_conversion.egg-info/
--rw-r--r--   0 gotoukaijin   (501) staff       (20)     6895 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/PKG-INFO
--rw-r--r--   0 gotoukaijin   (501) staff       (20)      240 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/SOURCES.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/dependency_links.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)       16 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/top_level.txt
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-18 04:44:30.782471 goto_conversion-0.3.1/
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1073 2024-05-18 04:42:42.000000 goto_conversion-0.3.1/LICENSE.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)     6435 2024-05-18 04:44:30.782281 goto_conversion-0.3.1/PKG-INFO
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     5888 2024-05-18 04:42:42.000000 goto_conversion-0.3.1/README.md
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)      614 2024-05-18 04:42:42.000000 goto_conversion-0.3.1/pyproject.toml
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)       38 2024-05-18 04:44:30.782520 goto_conversion-0.3.1/setup.cfg
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-18 04:44:30.780713 goto_conversion-0.3.1/src/
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-18 04:44:30.781288 goto_conversion-0.3.1/src/goto_conversion/
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1639 2024-05-18 04:42:42.000000 goto_conversion-0.3.1/src/goto_conversion/__init__.py
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-18 04:44:30.782024 goto_conversion-0.3.1/src/goto_conversion.egg-info/
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)     6435 2024-05-18 04:44:30.000000 goto_conversion-0.3.1/src/goto_conversion.egg-info/PKG-INFO
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)      240 2024-05-18 04:44:30.000000 goto_conversion-0.3.1/src/goto_conversion.egg-info/SOURCES.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2024-05-18 04:44:30.000000 goto_conversion-0.3.1/src/goto_conversion.egg-info/dependency_links.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)       16 2024-05-18 04:44:30.000000 goto_conversion-0.3.1/src/goto_conversion.egg-info/top_level.txt
```

### Comparing `goto_conversion-0.3.0/LICENSE.txt` & `goto_conversion-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goto_conversion-0.3.0/PKG-INFO` & `goto_conversion-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goto_conversion
-Version: 0.3.0
+Version: 0.3.1
 Summary: Gambling Odds To Outcome probabilities Conversion (goto_conversion)
 Author: Kaito Goto
 Project-URL: Homepage, https://github.com/gotoConversion/goto_conversion
 Project-URL: Bug Tracker, https://github.com/gotoConversion/goto_conversion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,31 +18,26 @@
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
 Our proposed method, **G**ambling **O**dds **T**o **O**utcome probabilities **Conversion** (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
 
 The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
 
-Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
+Furthermore, our table of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
 
 The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
 
-# Citations (not limited to, unofficial)
+# goto_conversion was leveraged by:
 
-[Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
-
-[Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
-
-[Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
-
-[Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
-
-[1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
-
-[15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+- [Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
+- [Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
+- [1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+- [15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+- [Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+- [Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -76,22 +71,18 @@
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/PseudoCode.png?raw=true)
 
 # Experiment Results
 
 Brier Score was mainly used to evaluate the accuracy of the probabilities implied by each conversion method. The Brier Score is essentially the mean squared error of the probabilities relative to the ground truth. Ranked Probability Score (RPS) was additionally used to evaluate the probabilities for football betting odds because the outcome is ordinal (home win, draw and away win). RPS is essentially the Brier Score on the cumulative probabilities.
 
-The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
+The experiment results table below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers under both Brier Score and RPS. Kaggle notebook to reproduce the table below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
 
-The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets. `goto_conversion` outperforms all other conversion methods for both win and place betting markets. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds).
-
-![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/RacingExperiment.png?raw=true)
-
 # References
 
 <a id="1">[1]</a> 
 [H. S. Shin, “Prices of State Contingent Claims with Insider
 traders, and the Favorite-Longshot Bias”. The Economic
 Journal, 1992, 102, pp. 426-435.](https://doi.org/10.2307/2234526)
```

### Comparing `goto_conversion-0.3.0/README.md` & `goto_conversion-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,31 +4,26 @@
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
 Our proposed method, **G**ambling **O**dds **T**o **O**utcome probabilities **Conversion** (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
 
 The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
 
-Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
+Furthermore, our table of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
 
 The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
 
-# Citations (not limited to, unofficial)
+# goto_conversion was leveraged by:
 
-[Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
-
-[Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
-
-[Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
-
-[Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
-
-[1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
-
-[15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+- [Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
+- [Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
+- [1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+- [15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+- [Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+- [Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -62,22 +57,18 @@
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/PseudoCode.png?raw=true)
 
 # Experiment Results
 
 Brier Score was mainly used to evaluate the accuracy of the probabilities implied by each conversion method. The Brier Score is essentially the mean squared error of the probabilities relative to the ground truth. Ranked Probability Score (RPS) was additionally used to evaluate the probabilities for football betting odds because the outcome is ordinal (home win, draw and away win). RPS is essentially the Brier Score on the cumulative probabilities.
 
-The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
+The experiment results table below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers under both Brier Score and RPS. Kaggle notebook to reproduce the table below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
 
-The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets. `goto_conversion` outperforms all other conversion methods for both win and place betting markets. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds).
-
-![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/RacingExperiment.png?raw=true)
-
 # References
 
 <a id="1">[1]</a> 
 [H. S. Shin, “Prices of State Contingent Claims with Insider
 traders, and the Favorite-Longshot Bias”. The Economic
 Journal, 1992, 102, pp. 426-435.](https://doi.org/10.2307/2234526)
```

### Comparing `goto_conversion-0.3.0/pyproject.toml` & `goto_conversion-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "goto_conversion"
-version = "0.3.0"
+version = "0.3.1"
 authors = [{ name = 'Kaito Goto' },]
 description = "Gambling Odds To Outcome probabilities Conversion (goto_conversion)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `goto_conversion-0.3.0/src/goto_conversion/__init__.py` & `goto_conversion-0.3.1/src/goto_conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `goto_conversion-0.3.0/src/goto_conversion.egg-info/PKG-INFO` & `goto_conversion-0.3.1/src/goto_conversion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goto_conversion
-Version: 0.3.0
+Version: 0.3.1
 Summary: Gambling Odds To Outcome probabilities Conversion (goto_conversion)
 Author: Kaito Goto
 Project-URL: Homepage, https://github.com/gotoConversion/goto_conversion
 Project-URL: Bug Tracker, https://github.com/gotoConversion/goto_conversion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,31 +18,26 @@
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
 Our proposed method, **G**ambling **O**dds **T**o **O**utcome probabilities **Conversion** (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
 
 The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
 
-Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
+Furthermore, our table of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
 
 The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
 
-# Citations (not limited to, unofficial)
+# goto_conversion was leveraged by:
 
-[Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
-
-[Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
-
-[Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
-
-[Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
-
-[1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
-
-[15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+- [Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
+- [Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
+- [1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+- [15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+- [Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+- [Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -76,22 +71,18 @@
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/PseudoCode.png?raw=true)
 
 # Experiment Results
 
 Brier Score was mainly used to evaluate the accuracy of the probabilities implied by each conversion method. The Brier Score is essentially the mean squared error of the probabilities relative to the ground truth. Ranked Probability Score (RPS) was additionally used to evaluate the probabilities for football betting odds because the outcome is ordinal (home win, draw and away win). RPS is essentially the Brier Score on the cumulative probabilities.
 
-The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
+The experiment results table below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers under both Brier Score and RPS. Kaggle notebook to reproduce the table below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
 
-The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets. `goto_conversion` outperforms all other conversion methods for both win and place betting markets. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds).
-
-![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/RacingExperiment.png?raw=true)
-
 # References
 
 <a id="1">[1]</a> 
 [H. S. Shin, “Prices of State Contingent Claims with Insider
 traders, and the Favorite-Longshot Bias”. The Economic
 Journal, 1992, 102, pp. 426-435.](https://doi.org/10.2307/2234526)
```


# Comparing `tmp/byteforge_coinmarketcap-1.4.tar.gz` & `tmp/byteforge_coinmarketcap-1.5.tar.gz`

## Comparing `byteforge_coinmarketcap-1.4.tar` & `byteforge_coinmarketcap-1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/MANIFEST
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/__init__.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/types/__init__.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/types/token_state.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/common.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/latest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/key/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/key/info.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v2/cryptocurrency/quotes/historical.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/doc/coinmarketcap.png
--rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/doc/coinmarketcap_original.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/tests/__init__.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/tests/test_coinmarketcap.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/.gitignore
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/LICENSE
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/README.md
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/pyproject.toml
--rw-r--r--   0        0        0    25988 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/MANIFEST
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/__init__.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/types/__init__.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/types/token_state.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/v1/cryptocurrency/listings/common.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/v1/cryptocurrency/listings/latest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/v1/key/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/v1/key/info.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/coinmarketcap/v2/cryptocurrency/quotes/historical.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/doc/coinmarketcap.png
+-rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/doc/coinmarketcap_original.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/tests/__init__.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/tests/test_coinmarketcap.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/.gitignore
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/LICENSE
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/README.md
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/pyproject.toml
+-rw-r--r--   0        0        0    26224 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.5/PKG-INFO
```

### Comparing `byteforge_coinmarketcap-1.4/coinmarketcap/core.py` & `byteforge_coinmarketcap-1.5/coinmarketcap/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional, List
 
 from .types.token_state import TokenState, Quote
 from .v2.cryptocurrency.quotes.historical import _quotes_historical_v2
 from .v1.cryptocurrency.listings.latest import _listings_latest
 from .v1.cryptocurrency.listings.common import SortOption, AuxFields, SortDir, FilterOptions
 from .v1.key.info import _key_info
-from .v1.key.info import _calls_left_today
+from .v1.key.info import _safe_daily_call_limit
 
 class Market(object):
 
 	_session = None
 	_caching_session = None
 	_debug_mode = False
 	_api_key = None
@@ -113,23 +113,23 @@
 					convert: List[str] = ['USD'],
 					aux_fields: AuxFields = None, 
 					filters: FilterOptions = None) -> List[TokenState]:
 		
 		return _listings_latest(self, sort_by, sort_dir, start, limit, convert, aux_fields, filters)
 	
 
-	def calls_left_today(self):
+	def safe_daily_call_limit(self):
 		"""
 		Calculates how many API calls are left for today, based on the service plan's monthly call limit.
 
 		This function takes the user's API call limit and subtracts the number of calls used to date,
 		providing a simple ratio to estimate daily available calls until the reset date. Note that 
 		this is an approximation based on equal usage each day until the reset.
 
 		Parameters:
 			market (Market): An instance of the Market class, which handles the API communications.
 
 		Returns:
 			int: Approximate number of API calls left for the current day, based on daily usage 
 				till the reset date and a monthly limit.
 		"""		
-		return _calls_left_today(self)
+		return _safe_daily_call_limit(self)
```

### Comparing `byteforge_coinmarketcap-1.4/coinmarketcap/types/token_state.py` & `byteforge_coinmarketcap-1.5/coinmarketcap/types/token_state.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/common.py` & `byteforge_coinmarketcap-1.5/coinmarketcap/v1/cryptocurrency/listings/common.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/latest.py` & `byteforge_coinmarketcap-1.5/coinmarketcap/v1/cryptocurrency/listings/latest.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/coinmarketcap/v1/key/info.py` & `byteforge_coinmarketcap-1.5/coinmarketcap/v1/key/info.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,37 +14,36 @@
     Returns:
         dict: A dictionary containing detailed key configuration information such as API limits.
     """
     dct_response = market._request('v1/key/info', ignore_cache=True)
     return dct_response['data']
 
 
-def _calls_left_today(market):
+def _safe_daily_call_limit(market):
     """
-    Calculates how many API calls are left for today, based on the service plan's monthly call limit.
+    Calculates the safe number of API calls that can be made per day, based on the remaining quota and time until the reset.
 
-    This function takes the user's API call limit and subtracts the number of calls used to date,
-    providing a simple ratio to estimate daily available calls until the reset date. Note that 
-    this is an approximation based on equal usage each day until the reset.
+    This function estimates the daily call limit by dividing the remaining quota by the number of days left until the quota reset.
+    The estimation is based on equal usage allocation each day until the reset date.
 
     Parameters:
         market (Market): An instance of the Market class, which handles the API communications.
 
     Returns:
-        int: Approximate number of API calls left for the current day, based on daily usage 
-             till the reset date and a monthly limit.
+        int: Approximate number of API calls that can be safely made per day, based on remaining monthly quota
+             and days until the quota reset.
     """
     dct_response = market._request('v1/key/info', no_cache=True)
     quota_reset_dt = parser.parse(dct_response['data']['plan']['credit_limit_monthly_reset_timestamp'])
     monthly_calls_remaining = dct_response['data']['usage']['current_month']['credits_left']
-    
-    # Ensure the current datetime is timezone-aware with UTC timezone  
+
+    # Ensure the current datetime is timezone-aware with UTC timezone
     now_datetime = datetime.now(timezone.utc)
 
-    # Calculate the timedelta  
+    # Calculate the timedelta
     time_difference = quota_reset_dt - now_datetime
 
-    # Extract the number of days as an integer  
+    # Extract the number of days as an integer
     number_of_days = time_difference.days
 
     # Convert daily calls calculation into an integer
     return int(monthly_calls_remaining / number_of_days) if number_of_days > 0 else 0  # Added safety for division
```

### Comparing `byteforge_coinmarketcap-1.4/coinmarketcap/v2/cryptocurrency/quotes/historical.py` & `byteforge_coinmarketcap-1.5/coinmarketcap/v2/cryptocurrency/quotes/historical.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/doc/coinmarketcap.png` & `byteforge_coinmarketcap-1.5/doc/coinmarketcap.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/doc/coinmarketcap_original.png` & `byteforge_coinmarketcap-1.5/doc/coinmarketcap_original.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/tests/test_coinmarketcap.py` & `byteforge_coinmarketcap-1.5/tests/test_coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/LICENSE` & `byteforge_coinmarketcap-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.4/README.md` & `byteforge_coinmarketcap-1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
 ### Example Usage
 
 ```python
 from byteforge_coinmarketcap import Market
 from datetime import datetime
 
-market = Market(api_key='your_api_key')
+coinmarketcap = Market(api_key='your_api_key')
 
 historical_quotes = coinmarketcap.quotes_historical(
     ticker='BTC',
     timestamp_start=1709269200,
     timestamp_end=1710046800,
     interval='daily',
     convert=['USD', 'EUR']
@@ -250,28 +250,28 @@
 Please ensure to select the interval that best matches your data analysis needs.
 
 
 To include the new `calls_left_today` routine in your existing project documentation, add a section that explains its purpose, usage, and example code on how to call it. Below is a suggested format for including this information in your README:
 
 ## Monitoring API Usage
 
-As you utilize the API, it's important to manage the number of requests to stay within your plan's limits. The `calls_left_today` function provides an easy way to monitor your daily API usage against your monthly limits.
+As you utilize the API, it's important to manage the number of requests to stay within your plan's limits. The `safe_daily_call_limit` function provides an easy way to verify your daily API limits against your monthly call budget.
 
 ### Purpose
 
-The `calls_left_today` method estimates the number of API calls you can still make for the current day without exceeding your monthly limit. This is crucial for applications that need to manage request rates or distribute API calls evenly throughout a billing period.
+The `safe_daily_call_limit` method estimates the number of API calls you can make during the current day without exceeding your monthly limit. This is crucial for applications that need to manage request rates or distribute API calls evenly throughout a billing period.
 
 ### Usage
 
-2. **Call the `calls_left_today` Method**:
-   Use the `calls_left_today` method to find out how many more API calls you can make today.
+2. **Call the `safe_daily_call_limit` Method**:
+   Use the `safe_daily_call_limit` method to find out how many API calls you can safely make per day without exhausting your quota.  It's up to you to store a counter for this and track your daily usage.  The SDK call is stateless and just uses some simple math to determine this value.
 
 ```python
-remaining_calls = market.calls_left_today()
-print(f"You have {remaining_calls} API calls left for today.")
+safe_calls_per_day = coinmarkectap.safe_daily_call_limit()
+print(f"You can safely make {safe_calls_per_day} calls per day.")
 ```
 
 ### Note
 
 - **Accuracy**: Please note that this function provides an approximation. If your daily API call volume varies significantly, consider implementing more detailed tracking mechanisms.
 - **Reset Timing**: Be aware of your API subscription details, especially when the monthly call count resets, as this will affect the calculations.
```

### Comparing `byteforge_coinmarketcap-1.4/pyproject.toml` & `byteforge_coinmarketcap-1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "byteforge-coinmarketcap"
-version = "1.4"
+version = "1.5"
 description = "Python SDK for the coinmarketcap.com API."
 readme = "README.md"
 license = { file="LICENSE" }
 keywords = ["cryptocurrency", "API", "coinmarketcap", "BTC", "Bitcoin", "LTC", "Litecoin", "XRP", "Ripple", "ETH", "Ethereum"]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `byteforge_coinmarketcap-1.4/PKG-INFO` & `byteforge_coinmarketcap-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: byteforge-coinmarketcap
-Version: 1.4
+Version: 1.5
 Summary: Python SDK for the coinmarketcap.com API.
 Project-URL: Homepage, https://github.com/jmazzahacks/byteforge-coinmarketcap/
 Project-URL: Issues, https://github.com/jmazzahacks/byteforge-coinmarketcap/issues
 Author: Jason Byteforgia
 License:                              Apache License
                                Version 2.0, January 2004
                             http://www.apache.org/licenses/
@@ -416,15 +416,15 @@
 
 ### Example Usage
 
 ```python
 from byteforge_coinmarketcap import Market
 from datetime import datetime
 
-market = Market(api_key='your_api_key')
+coinmarketcap = Market(api_key='your_api_key')
 
 historical_quotes = coinmarketcap.quotes_historical(
     ticker='BTC',
     timestamp_start=1709269200,
     timestamp_end=1710046800,
     interval='daily',
     convert=['USD', 'EUR']
@@ -469,28 +469,28 @@
 Please ensure to select the interval that best matches your data analysis needs.
 
 
 To include the new `calls_left_today` routine in your existing project documentation, add a section that explains its purpose, usage, and example code on how to call it. Below is a suggested format for including this information in your README:
 
 ## Monitoring API Usage
 
-As you utilize the API, it's important to manage the number of requests to stay within your plan's limits. The `calls_left_today` function provides an easy way to monitor your daily API usage against your monthly limits.
+As you utilize the API, it's important to manage the number of requests to stay within your plan's limits. The `safe_daily_call_limit` function provides an easy way to verify your daily API limits against your monthly call budget.
 
 ### Purpose
 
-The `calls_left_today` method estimates the number of API calls you can still make for the current day without exceeding your monthly limit. This is crucial for applications that need to manage request rates or distribute API calls evenly throughout a billing period.
+The `safe_daily_call_limit` method estimates the number of API calls you can make during the current day without exceeding your monthly limit. This is crucial for applications that need to manage request rates or distribute API calls evenly throughout a billing period.
 
 ### Usage
 
-2. **Call the `calls_left_today` Method**:
-   Use the `calls_left_today` method to find out how many more API calls you can make today.
+2. **Call the `safe_daily_call_limit` Method**:
+   Use the `safe_daily_call_limit` method to find out how many API calls you can safely make per day without exhausting your quota.  It's up to you to store a counter for this and track your daily usage.  The SDK call is stateless and just uses some simple math to determine this value.
 
 ```python
-remaining_calls = market.calls_left_today()
-print(f"You have {remaining_calls} API calls left for today.")
+safe_calls_per_day = coinmarkectap.safe_daily_call_limit()
+print(f"You can safely make {safe_calls_per_day} calls per day.")
 ```
 
 ### Note
 
 - **Accuracy**: Please note that this function provides an approximation. If your daily API call volume varies significantly, consider implementing more detailed tracking mechanisms.
 - **Reset Timing**: Be aware of your API subscription details, especially when the monthly call count resets, as this will affect the calculations.
```


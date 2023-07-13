# Comparing `tmp/crypto-screening-2.8.4.tar.gz` & `tmp/crypto-screening-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.8.4.tar", last modified: Thu Jul 13 01:43:01 2023, max compression
+gzip compressed data, was "crypto-screening-3.0.0.tar", last modified: Thu Jul 13 15:41:24 2023, max compression
```

## Comparing `crypto-screening-2.8.4.tar` & `crypto-screening-3.0.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.454387 crypto-screening-2.8.4/
--rw-rw-rw-   0        0        0       98 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-13 01:43:01.454387 crypto-screening-2.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.4/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.4/build.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.422187 crypto-screening-2.8.4/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.443824 crypto-screening-2.8.4/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.4/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.4/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    39266 2023-07-12 23:07:59.000000 crypto-screening-2.8.4/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21275 2023-07-12 23:36:53.000000 crypto-screening-2.8.4/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19359 2023-07-12 23:37:04.000000 crypto-screening-2.8.4/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.4/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.4/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.4/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.4/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.4/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.445824 crypto-screening-2.8.4/crypto_screening/market/
--rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.4/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.448852 crypto-screening-2.8.4/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.453882 crypto-screening-2.8.4/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32677 2023-07-13 01:20:24.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.4/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.4/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.4/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.4/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.438792 crypto-screening-2.8.4/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 01:43:01.454387 crypto-screening-2.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-13 01:42:55.000000 crypto-screening-2.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:41:24.690907 crypto-screening-3.0.0/
+-rw-rw-rw-   0        0        0       98 2023-07-13 15:41:22.000000 crypto-screening-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-13 15:41:24.689903 crypto-screening-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-3.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-3.0.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:41:24.598130 crypto-screening-3.0.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-13 15:41:24.653162 crypto-screening-3.0.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-3.0.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-3.0.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    39266 2023-07-12 23:07:59.000000 crypto-screening-3.0.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21275 2023-07-12 23:36:53.000000 crypto-screening-3.0.0/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19359 2023-07-12 23:37:04.000000 crypto-screening-3.0.0/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-3.0.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-3.0.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    13639 2023-07-13 15:21:10.000000 crypto-screening-3.0.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-3.0.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-3.0.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:41:24.663163 crypto-screening-3.0.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-3.0.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:41:24.685432 crypto-screening-3.0.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-3.0.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-3.0.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-3.0.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-3.0.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:41:24.688399 crypto-screening-3.0.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-3.0.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    18442 2023-07-13 14:37:22.000000 crypto-screening-3.0.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3251 2023-07-13 13:32:20.000000 crypto-screening-3.0.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    30412 2023-07-13 15:36:47.000000 crypto-screening-3.0.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    14109 2023-07-13 13:54:09.000000 crypto-screening-3.0.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    14866 2023-07-13 13:45:46.000000 crypto-screening-3.0.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-3.0.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-3.0.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-3.0.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-3.0.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:41:24.615159 crypto-screening-3.0.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-13 15:41:24.000000 crypto-screening-3.0.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-13 15:41:24.000000 crypto-screening-3.0.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 15:41:24.000000 crypto-screening-3.0.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-13 15:41:24.000000 crypto-screening-3.0.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-13 15:41:24.000000 crypto-screening-3.0.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-13 15:41:22.000000 crypto-screening-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-3.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-3.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 15:41:24.690907 crypto-screening-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-13 15:36:47.000000 crypto-screening-3.0.0/setup.py
```

### Comparing `crypto-screening-2.8.4/PKG-INFO` & `crypto-screening-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.4
+Version: 3.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.4/README.md` & `crypto-screening-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/build.py` & `crypto-screening-3.0.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/collect/assets.py` & `crypto-screening-3.0.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/collect/exchanges.py` & `crypto-screening-3.0.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/collect/market.py` & `crypto-screening-3.0.0/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/collect/ohlcv.py` & `crypto-screening-3.0.0/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/collect/orderbook.py` & `crypto-screening-3.0.0/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/collect/screeners.py` & `crypto-screening-3.0.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/collect/symbols.py` & `crypto-screening-3.0.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/dataset.py` & `crypto-screening-3.0.0/crypto_screening/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from typing import (
     Union, Optional, Tuple, Iterable,
     Any, Callable, Dict, List
 )
 
 import pandas as pd
 
+from crypto_screening.interval import interval_to_total_time
+
 __all__ = [
     "row_to_dataset",
     "save_dataset",
     "load_dataset",
     "update_dataset",
     "split_dataset",
     "strip_dataset",
@@ -38,15 +40,16 @@
     "prepare_saving_location",
     "BIDS_VOLUME",
     "ASKS_VOLUME",
     "CSV_EXTENSION",
     "JSON_EXTENSION",
     "DEFAULT_EXTENSION",
     "BASE_VOLUME",
-    "QUOTE_VOLUME"
+    "QUOTE_VOLUME",
+    "bid_ask_to_ohlcv"
 ]
 
 OPEN = "Open"
 CLOSE = "Close"
 HIGH = "High"
 LOW = "Low"
 VOLUME = "Volume"
@@ -477,8 +480,37 @@
         if (
             (validation is None) or
             (callable(validation) and validation(dataset[column]))
         ):
             return dataset[column]
         # end if
     # end for
-# end find_column
+# end find_column
+
+def bid_ask_to_ohlcv(dataset: pd.DataFrame, interval: str) -> pd.DataFrame:
+    """
+    Converts the BID/ASK spread dataset into a OHLCV dataset.
+
+    :param dataset: The source data.
+    :param interval: The interval for the new dataset.
+
+    :return: The returned dataset.
+    """
+
+    interval_total_time = interval_to_total_time(interval)
+    interval_total_minutes = (
+            interval_total_time.total_seconds() // 60
+    )
+    adjuster = f'{interval_total_minutes}Min'
+
+    ohlcv_dataset: pd.DataFrame = (
+        dataset[BIDS].resample(adjuster).ohlc()
+    )
+    ohlcv_dataset.columns = [OPEN, HIGH, LOW, CLOSE]
+    volume: pd.DataFrame = (
+        dataset[BIDS_VOLUME].resample(adjuster).ohlc()
+    )
+    volume.columns = [OPEN, HIGH, LOW, CLOSE]
+    ohlcv_dataset[VOLUME] = volume[CLOSE]
+
+    return ohlcv_dataset
+# end bid_ask_to_ohlcv
```

### Comparing `crypto-screening-2.8.4/crypto_screening/interval.py` & `crypto-screening-3.0.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/market/dynamic.py` & `crypto-screening-3.0.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/market/foundation/data.py` & `crypto-screening-3.0.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/market/foundation/protocols.py` & `crypto-screening-3.0.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/market/foundation/state.py` & `crypto-screening-3.0.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/market/foundation/waiting.py` & `crypto-screening-3.0.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/market/screeners/base.py` & `crypto-screening-3.0.0/crypto_screening/market/screeners/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # base.py
 
 import datetime as dt
 import time
 from typing import (
-    Optional, Union, Dict, Iterable, Any, List
+    Optional, Union, Dict, Iterable, Any, List, Callable
 )
 
 import pandas as pd
 
-from represent import Modifiers
+from represent import Modifiers, represent
 
 from multithreading import Caller, multi_threaded_call
 
-from crypto_screening.dataset import save_dataset, load_dataset
+from cryptofeed.defines import L2_BOOK
+
+from crypto_screening.process import find_string_value
+from crypto_screening.dataset import save_dataset, load_dataset, DATE_TIME
 from crypto_screening.symbols import Separator
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.market.foundation.state import WaitingState
 from crypto_screening.market.foundation.waiting import (
     base_wait_for_initialization, base_wait_for_dynamic_initialization,
     base_wait_for_dynamic_update, base_wait_for_update
 )
 from crypto_screening.market.foundation.data import DataCollector
-from crypto_screening.market.screeners.recorder import (
-    MarketRecorder, create_market_dataframe
-)
 
 __all__ = [
     "BaseScreener",
     "BaseMultiScreener",
     "structure_screeners_datasets",
-    "structure_screener_datasets"
+    "structure_screener_datasets",
+    "create_market_dataframe",
+    "MarketRecorder",
+    "validate_market"
 ]
 
 class BaseScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
@@ -52,14 +55,17 @@
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
+
+    - market:
+        The dataset of the market data.
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.append("market")
 
     __slots__ = "symbol", "exchange", "market"
 
@@ -238,14 +244,203 @@
             end = time.time()
 
             time.sleep(max([delay - (end - start), 1]))
         # end while
     # end saving_loop
 # end BaseScreener
 
+def create_market_dataframe(columns: Optional[Iterable[str]] = None) -> pd.DataFrame:
+    """
+    Creates a dataframe for the order book data.
+
+    :param columns: The dataset columns.
+
+    :return: The dataframe.
+    """
+
+    market = pd.DataFrame(
+        {column: [] for column in columns or []}, index=[]
+    )
+    market.index.name = DATE_TIME
+
+    return market
+# end create_market_dataframe
+
+RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
+
+Market = Dict[str, Dict[str, Any]]
+
+def validate_market(data: Any) -> Market:
+    """
+    Validates the data.
+
+    :param data: The data to validate.
+
+    :return: The valid data.
+    """
+
+    try:
+        if not isinstance(data, dict):
+            raise ValueError
+        # end if
+
+        for exchange, values in data.items():
+            if not (
+                isinstance(exchange, str) and
+                (
+                    isinstance(values, dict) and
+                    all(
+                        isinstance(symbol, str)
+                        for symbol, _ in values.items()
+                    )
+                )
+            ):
+                raise ValueError
+            # end if
+        # end for
+
+    except (TypeError, ValueError):
+        raise ValueError(
+            f"Data must be of type {Market}, not: {data}."
+        )
+    # end try
+
+    return data
+# end validate_market
+
+@represent
+class MarketRecorder:
+    """
+    A class to represent a crypto data feed recorder.
+    This object passes the record method to the handler object to record
+    the data fetched by the handler.
+
+    Parameters:
+
+    - market:
+        The market structure of the data to store the fetched data in.
+        This structure is a dictionary with exchange names as keys
+        and dictionaries as values, where their keys are symbols,
+        and their values are the dataframes to record the data.
+
+    >>> from crypto_screening.market.screeners.base import MarketRecorder
+    >>>
+    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
+    >>>
+    >>> recorder = MarketRecorder(data=market)
+
+    """
+
+    __modifiers__ = Modifiers()
+    __modifiers__.hidden.append("market")
+
+    __slots__ = "market",
+
+    def __init__(self, market: Market) -> None:
+        """
+        Defines the class attributes.
+
+        :param market: The object to fill with the crypto feed record.
+        """
+
+        self.market = self.validate_market(data=market)
+    # end __init__
+
+    def parameters(self) -> RecorderParameters:
+        """
+        Returns the order book parameters.
+
+        :return: The order book parameters.
+        """
+
+        return dict(
+            channels=[L2_BOOK],
+            callbacks={L2_BOOK: self.record},
+            max_depth=1
+        )
+    # end parameters
+
+    @staticmethod
+    def validate_market(data: Any) -> Market:
+        """
+        Validates the data.
+
+        :param data: The data to validate.
+
+        :return: The valid data.
+        """
+
+        return validate_market(data=data)
+    # end validate_market
+
+    def structure(self) -> Dict[str, List[str]]:
+        """
+        Returns the structure of the market data.
+
+        :return: The structure of the market.
+        """
+
+        return {
+            exchange: list(symbols.keys())
+            for exchange, symbols in self.market.items()
+        }
+    # end structure
+
+    def data(self, exchange: str, symbol: str) -> Any:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+
+        :return: The dataset of the spread data.
+        """
+
+        exchange = find_string_value(
+            value=exchange, values=self.market.keys()
+        )
+
+        validate_exchange(
+            exchange=exchange,
+            exchanges=self.market.keys(),
+            provider=self
+        )
+
+        validate_symbol(
+            symbol=symbol,
+            exchange=exchange,
+            exchanges=self.market.keys(),
+            symbols=self.market[exchange],
+            provider=self
+        )
+
+        return self.market[exchange][symbol]
+    # end data
+
+    def in_market(self, exchange: str, symbol: str) -> bool:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+
+        :return: The dataset of the spread data.
+        """
+
+        try:
+            self.data(exchange=exchange, symbol=symbol)
+
+            return True
+
+        except ValueError:
+            return False
+        # end try
+    # end in_market
+# end MarketRecorder
+
 class BaseMultiScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
@@ -267,16 +462,16 @@
 
     screeners: List[BaseScreener]
 
     __slots__ = 'recorder', 'screeners'
 
     def __init__(
             self,
+            recorder: MarketRecorder,
             screeners: Optional[Iterable[BaseScreener]] = None,
-            recorder: Optional[MarketRecorder] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None
     ) -> None:
         """
         Defines the class attributes.
 
@@ -285,17 +480,15 @@
         :param cancel: The cancel time for the loops.
         """
 
         super().__init__(location=location, cancel=cancel, delay=delay)
 
         self.screeners = list(screeners or [])
 
-        self.recorder = recorder or MarketRecorder(
-            market=structure_screener_datasets(screeners=self.screeners)
-        )
+        self.recorder = recorder
     # end __init__
 
     @property
     def market(self) -> Dict[str, Dict[str, pd.DataFrame]]:
         """
         Returns the market to hold the recorder data.
```

### Comparing `crypto-screening-2.8.4/crypto_screening/market/screeners/container.py` & `crypto-screening-3.0.0/crypto_screening/market/screeners/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Iterable, List
 
 from represent import Modifiers
 
 from crypto_screening.market.screeners.base import (
     BaseScreener, structure_screener_datasets
 )
-from crypto_screening.market.screeners.recorder import MarketRecorder
+from crypto_screening.market.screeners.base import MarketRecorder
 
 class ScreenersContainer(MarketRecorder):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
```

### Comparing `crypto-screening-2.8.4/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-3.0.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1079 +1,966 @@
 # ohlcv.py
 
-import time
-import asyncio
-import warnings
 import datetime as dt
 from typing import (
-    Optional, Union, Dict, Iterable, Any, List
+    Dict, Optional, Iterable, Any, Union, List
 )
 
 import pandas as pd
-import numpy as np
-
-import ccxt
-import ccxt.pro as ccxtpro
-import ccxt.async_support as async_ccxt
 
 from represent import Modifiers
 
-from multithreading import Caller, multi_threaded_call
+from cryptofeed import FeedHandler
+from cryptofeed.types import OrderBook
 
+from crypto_screening.interval import interval_to_total_time
 from crypto_screening.dataset import (
-    OPEN, HIGH, LOW, CLOSE, VOLUME, BIDS, ASKS,
-    DATE_TIME, OHLCV_COLUMNS, ASKS_VOLUME, BIDS_VOLUME
+    OHLCV_COLUMNS, OPEN, HIGH, LOW, CLOSE, VOLUME,
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
 )
-from crypto_screening.interval import interval_to_total_time
+from crypto_screening.symbols import adjust_symbol
+from crypto_screening.market.screeners.base import (
+    BaseScreener, structure_screener_datasets
+)
+from crypto_screening.market.screeners.recorder import MarketScreener
 from crypto_screening.market.screeners.base import (
-    BaseMultiScreener, structure_screener_datasets, BaseScreener
+    create_market_dataframe, MarketRecorder, validate_market
 )
-from crypto_screening.market.screeners.recorder import (
-    MarketRecorder, create_market_dataframe
+from crypto_screening.market.screeners.orderbook import (
+    create_orderbook_dataframe, OrderbookScreener,
+    OrderbookMarketScreener, create_orderbook_market
 )
+from crypto_screening.process import find_string_value
 
 __all__ = [
+    "OHLCVMarketScreener",
+    "OHLCVMarketRecorder",
     "OHLCVScreener",
-    "MarketOHLCVScreener",
-    "market_ohlcv_recorder",
-    "MarketOHLCVRecorder",
-    "market_ohlcv_screener",
     "create_ohlcv_market",
-    "create_ohlcv_dataframe"
+    "ohlcv_market_screener",
+    "ohlcv_market_recorder",
+    "create_ohlcv_dataframe",
+    "validate_intervals",
+    "structure_screener_intervals",
+    "datasets_to_intervals_datasets",
+    "validate_ohlcv_market",
+    "create_ohlcv_market_recorder_initializers",
+    "structure_screeners_intervals"
 ]
 
-def configure_exchange(
-        exchange: str,
-        pro: Optional[bool] = True,
-        options: Optional[Dict[str, Any]] = None
-) -> async_ccxt.Exchange:
-    """
-    Validates the exchange source value.
+OHLCVMarket = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
+Market = Dict[str, Dict[str, Any]]
+Intervals = Dict[str, Dict[str, Iterable[str]]]
+Indexes = Dict[str, Dict[str, Dict[str, int]]]
 
-    :param exchange: The name of the exchange platform.
-    :param pro: The value for the pro interface.
-    :param options: The ccxt options.
+def create_ohlcv_dataframe() -> pd.DataFrame:
+    """
+    Creates a dataframe for the order book data.
 
-    :return: The validates source.
+    :return: The dataframe.
     """
 
-    if exchange.lower() == "coinbase":
-        exchange = "coinbasepro"
-    # end if
+    return create_market_dataframe(
+        columns=OHLCVMarketRecorder.COLUMNS
+    )
+# end create_ohlcv_dataframe
 
-    try:
-        exchange_service = getattr(
-            (ccxtpro if pro else async_ccxt), exchange
-        )(options)
+def datasets_to_intervals_datasets(
+        data: Dict[str, Iterable[str]],
+        interval: Optional[str] = None
+) -> Dict[str, Dict[str, List[str]]]:
+    """
+    Creates the dataframes of the market data.
 
-    except AttributeError:
-        raise ValueError(f"Unrecognized exchange name: {exchange}.")
-        # end try
+    :param data: The market data.
+    :param interval: The interval for the structure.
 
-    if not (
-        hasattr(exchange_service, "watch_tickers") or
-        hasattr(exchange_service, "fetch_tickers")
-    ):
-        raise ValueError(
-            f"Exchange {exchange_service} must have at least one of the "
-            f"methods 'fetch_tickers', or 'watch_tickers'."
-        )
-        # end if
-    # end if
+    :return: The dataframes of the market data.
+    """
+
+    interval = interval or OHLCVScreener.INTERVAL
 
-    return exchange_service
-# end configure_exchange
+    return {
+        exchange.lower(): {
+            symbol.upper(): [interval]
+            for symbol in symbols
+        } for exchange, symbols in data.items()
+    }
+# end datasets_to_intervals_datasets
 
 class OHLCVScreener(BaseScreener):
     """
-    A class to represent a live asset data builder.
+    A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
-    You can also use it to build real time datasets of Open
-    High Low Close Volume, with Bids and Asks.
-
     Parameters:
 
     - symbol:
         The symbol of an asset to screen.
 
     - exchange:
         The name of the exchange platform to screen data from.
 
-    - locaion:
+    - location:
         The saving location for the saved data of the screener.
 
-    - interval:
-        The interval for the time between data points in the dataset.
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
 
-    - screener:
-        The screener object to connect to for creating the dataset.
-
-    - length:
-        An initial dataset length to start with.
-
-    - pro:
-        The value to use the pro interface.
-
-    - options:
-        The ccxt options for the backend screening process.
+    - interval:
+        The interval for the data structure of OHLCV.
 
-    - cencel:
-        The time to cancel screening process after no new data is fetched.
+    - market:
+        The dataset of the market data as OHLCV.
 
-    >>> from crypto_screening.market.screeners import OHLCVScreener
-    >>>
-    >>> screener = OHLCVScreener(
-    >>>     symbol="BTC/USD", exchange="binance"
-    >>> )
-    >>>
-    >>> screener.run(wait=True)
-    >>>
-    >>> print(screener.market.iloc[-1].splitlines()[0])
-    >>>
-    >>> while True:
-    >>>     screener.wait_for_update()
-    >>>
-    >>>     print(screener.market.iloc[-1].splitlines()[-1])
+    - base_market:
+        The dataset of the market data as BID/ASK spread.
     """
 
-    __modifiers__ = Modifiers(**BaseScreener.__modifiers__)
-    __modifiers__.excluded.append('task')
-
-    __slots__ = "interval", "pro", "options", "task"
-
     INTERVAL = "1m"
 
-    PRO = False
-
-    OPTIONS = {}
-
-    LENGTH = 0
-
-    COLUMNS = (
-        OPEN, HIGH, LOW, CLOSE, VOLUME,
-        ASKS, BIDS, ASKS_VOLUME, BIDS_VOLUME
-    )
-
     def __init__(
             self,
             symbol: str,
             exchange: str,
             interval: Optional[str] = None,
-            pro: Optional[bool] = True,
-            data: Optional[pd.DataFrame] = None,
-            length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
             location: Optional[str] = None,
-            options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            market: Optional[pd.DataFrame] = None,
+            base_market: Optional[pd.DataFrame] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param symbol: The symbol of the asset.
         :param exchange: The exchange to get source data from.
-        :param interval: The interval for the data.
-        :param data: The base dataset of the asset to add to.
-        :param length: The length of the base dataset.
         :param location: The saving location for the data.
         :param delay: The delay for the process.
-        :param pro: The value for the pro interface.
-        :param options: The ccxt options.
-        :param cancel: The time to cancel the waiting.
+        :param cancel: The cancel time for the loops.
+        :param market: The data for the market.
+        :param base_market: The base market dataset.
         """
 
         super().__init__(
-            symbol=symbol, exchange=exchange, delay=delay,
-            location=location, cancel=cancel
+            symbol=symbol, exchange=exchange, location=location,
+            cancel=cancel, delay=delay, market=market
         )
 
-        if pro is None:
-            pro = self.PRO
-        # end if
-
-        if length is None:
-            length = self.LENGTH
-        # end if
-
-        self.pro = pro
         self.interval = interval or self.INTERVAL
-        self.options = options or {}
-
-        self.task = None
 
-        self.market = self.validate_data(data, length=length)
+        self.base_market = base_market
     # end __init__
 
-    def __getstate__(self) -> Dict[str, Any]:
-        """
-        Returns the data of the object.
-
-        :return: The state of the object.
+    def dataset_path(self, location: Optional[str] = None) -> str:
         """
+        Creates the path to the saving file for the screener object.
 
-        data = super().__getstate__()
+        :param location: The saving location of the dataset.
 
-        data["task"] = None
+        :return: The saving path for the dataset.
+        """
 
-        return data
-    # end __getstate__
+        return (
+            super().dataset_path(location=location).
+            replace(".csv", f"-{self.interval}.csv")
+        )
+    # end dataset_path
 
-    def validate_data(self, data: Any, length: Optional[int]) -> pd.DataFrame:
+    def orderbook_screener(self) -> OrderbookScreener:
         """
-        Validates the asset data value.
-
-        :param data: The asset data.
-        :param length: The length of the data to add.
+        Creates the orderbook screener object.
 
-        :return: The validates source.
+        :return: The orderbook screener.
         """
 
-        if not all(
-            hasattr(self, name) for name in ["exchange", "interval"]
-        ):
-            raise AttributeError(
-                "Source and interval attributes must be defined "
-                "before attempting to validate the data parameter data."
-            )
-        # end if
+        return OrderbookScreener(
+            symbol=self.symbol, exchange=self.exchange, location=self.location,
+            cancel=self.cancel, delay=self.delay, market=self.base_market
+        )
+    # end orderbook_screener
+# end OHLCVScreener
 
-        if (
-            (data is None) and
-            (
-                (length is None) or
-                (length == 0) or
-                (length is False) or
-                (
-                    isinstance(length, int) and
-                    not (0 < length <= 500)
-                )
-            )
-        ):
-            data = pd.DataFrame(
-                {column: [] for column in self.COLUMNS},
-                index=[]
-            )
+def validate_intervals(data: Any) -> Intervals:
+    """
+    Validates the data.
 
-        elif (data is None) and (isinstance(length, int)):
-            if 0 < length <= 500:
-                try:
-                    exchange = getattr(ccxt, self.exchange)(self.options)
-
-                    data = self.data_to_dataset(
-                        exchange.fetch_ohlcv(
-                            symbol=self.symbol,
-                            timeframe=self.interval,
-                            limit=length
-                        )
-                    )
+    :param data: The data to validate.
+
+    :return: The valid data.
+    """
 
-                except Exception as e:
-                    warnings.warn(str(e))
+    try:
+        if not isinstance(data, dict):
+            raise ValueError
+        # end if
 
-                    data = pd.DataFrame(
-                        {column: [] for column in self.COLUMNS},
-                        index=[]
+        for exchange, symbols in data.items():
+            if not (
+                isinstance(exchange, str) and
+                (
+                    isinstance(symbols, dict) and
+                    all(
+                        all(isinstance(interval, str) for interval in intervals)
+                        for symbol, intervals in symbols.items()
                     )
-                # end try
-
-            else:
-                raise ValueError(
-                    f"Length must be a positive int between "
-                    f"{1} and {500} when data is not defined, "
-                    f"not: {length}."
                 )
+            ):
+                raise ValueError
             # end if
-        # end if
-
-        return data
-    # end validate_data
-
-    def data_to_dataset(self, data: Iterable[Iterable]) -> pd.DataFrame:
-        """
-        Adjusts the dataset to an asset Open, High, Low, Close, Bids, Asks, Volume dataset.
-
-        :param data: The data to adjust.
+        # end for
 
-        :return: The asset dataset.
-        """
+    except (TypeError, ValueError):
+        raise ValueError(
+            f"Data must be of type {Intervals}, not: {data}."
+        )
+    # end try
 
-        data = pd.DataFrame(data)
+    return data
+# end validate_intervals
 
-        index_column_name = list(data.columns)[0]
+def validate_ohlcv_market(data: Any) -> OHLCVMarket:
+    """
+    Validates the data.
 
-        data.index = pd.to_datetime(data[index_column_name], unit="ms")
-        del data[index_column_name]
-        data.index.name = DATE_TIME
-        data.columns = list(OHLCV_COLUMNS)
+    :param data: The data to validate.
 
-        if len(self.market) == 0:
-            asks = [np.nan] * len(data)
-            bids = [np.nan] * len(data)
+    :return: The valid data.
+    """
 
-        else:
-            asks = (
-                self.market[ASKS].iloc
-                [-len(data):].values[:]
-            )
-            bids = (
-                self.market[BIDS].iloc
-                [-len(data):].values[:]
-            )
+    try:
+        if not isinstance(data, dict):
+            raise ValueError
         # end if
 
-        if ASKS in data:
-            data[ASKS].values[:] = asks
-
-        else:
-            data[ASKS] = asks
-        # end if
+        for exchange, symbols in data.items():
+            if not (
+                isinstance(exchange, str) and
+                (
+                    isinstance(symbols, dict) and
+                    all(
+                        all(
+                            isinstance(interval, str) and
+                            isinstance(dataset, pd.DataFrame)
+                            for interval, dataset in intervals.items()
+                        )
+                        for symbol, intervals in symbols.items()
+                    )
+                )
+            ):
+                raise ValueError
+            # end if
+        # end for
 
-        if BIDS in data:
-            data[BIDS].values[:] = bids
+    except (TypeError, ValueError):
+        raise ValueError(
+            f"Data must be of type {OHLCVMarket}, not: {data}."
+        )
+    # end try
 
-        else:
-            data[BIDS] = bids
-        # end if
+    return data
+# end validate_ohlcv_market
 
-        return data[list(self.COLUMNS)]
-    # end data_to_dataset
+def create_ohlcv_market(data: Intervals) -> Dict[str, Dict[str, Dict[str, pd.DataFrame]]]:
+    """
+    Creates the dataframes of the market data.
 
-    def dataset_path(self, location: Optional[str] = None) -> str:
-        """
-        Creates the path to the saving file for the screener object.
+    :param data: The market data.
 
-        :param location: The saving location of the dataset.
+    :return: The dataframes of the market data.
+    """
 
-        :return: The saving path for the dataset.
-        """
+    return {
+        exchange.lower(): {
+            symbol.upper(): {
+                interval: create_ohlcv_dataframe()
+                for interval in intervals
+            }
+            for symbol, intervals in symbols.items()
+        } for exchange, symbols in data.items()
+    }
+# end create_ohlcv_market
 
-        return super().dataset_path(location=location).replace(
-            '.csv', f'_{self.interval}.csv'
-        )
-    # end dataset_path
+def create_ohlcv_market_recorder_initializers(
+        intervals: Optional[Intervals] = None,
+        market: Optional[Market] = None,
+        ohlcv_market: Optional[OHLCVMarket] = None
+) -> Dict[str, Union[Market, OHLCVMarket, Intervals]]:
+    """
+    Defines the class attributes.
 
-    async def async_get_market(self) -> Dict[str, float]:
-        """
-        Gets the market data.
+    :param market: The object to fill with the crypto feed record.
+    :param intervals: The intervals for the datasets.
+    :param ohlcv_market: The OHLCV market structure.
 
-        :return: The bids and asks.
-        """
+    :return: The valid data.
+    """
 
-        exchange = configure_exchange(
-            exchange=self.exchange.lower(), pro=self.pro,
-            options=self.options
+    if (ohlcv_market, market, intervals) == (None, None, None):
+        raise ValueError(
+            f"No data given to initialize {OHLCVMarketRecorder}"
         )
+    # end if
 
-        method = None
+    if (ohlcv_market is not None) and (intervals is None):
+        validate_ohlcv_market(ohlcv_market)
 
-        if hasattr(exchange, "fetch_tickers"):
-            method = exchange.fetch_tickers
+        intervals: Dict[str, Dict[str, List[str]]] = {}
 
-        elif hasattr(exchange, "watch_tickers"):
-            method = exchange.watch_tickers
-        # end if
+        for exchange, symbols in ohlcv_market.items():
+            for symbol, symbol_intervals in symbols.items():
+                for interval in symbol_intervals:
+                    (
+                        intervals.
+                        setdefault(exchange, {}).
+                        setdefault(symbol, []).
+                        append(interval)
+                    )
+                # end for
+            # end for
+        # end for
+    # end if
 
-        data = await method(symbols=[self.symbol])
-        data: Dict[str, Union[float, Dict[str, float]]]
+    if (market is not None) and (intervals is None):
+        validate_market(market)
 
-        if self.symbol in data:
-            data = data[self.symbol]
-        # end if
+        intervals: Dict[str, Dict[str, List[str]]] = {}
 
-        data[ASKS.lower()] = data.get("ask")
-        data[BIDS.lower()] = data.get("bid")
-        data[ASKS_VOLUME.lower()] = data.get("askVolume")
-        data[BIDS_VOLUME.lower()] = data.get("bidVolume")
-        saved_volume = data.get("volume", data.get('baseVolume'))
+        for exchange, symbols in market.items():
+            for symbol in symbols:
+                (
+                    intervals.
+                    setdefault(exchange, {}).
+                    setdefault(symbol, []).
+                    append(OHLCVMarketRecorder.INTERVAL)
+                )
+            # end for
+        # end for
+    # end if
 
-        if 'info' in data and VOLUME.lower() in data['info']:
-            saved_volume = float(data['info'][VOLUME.lower()])
-        # end if
+    if (ohlcv_market is None) and intervals:
+        validate_intervals(intervals)
 
-        data = {
-            key: (
-                float(data[key.lower()]) if
-                isinstance(data[key.lower()], str) else
-                data[key.lower()]
-            ) for key in self.COLUMNS if key.lower() in data
-        }
+        ohlcv_market = create_ohlcv_market(data=intervals)
+    # end if
 
-        try:
-            ohlcv = await exchange.fetch_ohlcv(
-                self.symbol, timeframe='1m', limit=1
-            )
+    if (market is None) and (ohlcv_market is not None):
+        validate_ohlcv_market(ohlcv_market)
 
-            ohlcv = {
-                column: float(value) for column, value in
-                zip(OHLCV_COLUMNS, ohlcv[0][1:])
-            }
+        market: Market = {}
 
-            data.update(ohlcv)
+        for exchange, symbols in ohlcv_market.items():
+            for symbol, symbol_intervals in symbols.items():
+                (
+                    market.
+                    setdefault(exchange, {}).
+                    setdefault(symbol, create_orderbook_dataframe())
+                )
+            # end for
+        # end for
+    # end if
 
-        except Exception as e:
-            warnings.warn(f"{type(e).__name__}: {e}")
-        # end try
+    return dict(
+        market=market,
+        ohlcv_market=ohlcv_market,
+        intervals=intervals
+    )
+# end create_ohlcv_market_recorder_initializers
 
-        data.setdefault(VOLUME, saved_volume)
+class OHLCVMarketRecorder(MarketRecorder):
+    """
+    A class to represent a crypto data feed recorder.
+    This object passes the record method to the handler object to record
+    the data fetched by the handler.
 
-        await exchange.close()
+    Parameters:
 
-        return data
-    # end async_get_market
+    - market:
+        The market structure of the data to store the fetched data in.
+        This structure is a dictionary with exchange names as keys
+        and dictionaries as values, where their keys are symbols,
+        and their values are the dataframes to record the data.
 
-    async def async_update_market(self) -> None:
-        """Updates the market data."""
+    - intervals:
+        The structure to set a specific interval to the dataset
+        of each symbol in each exchange, matching the market data.
 
-        data = await self.async_get_market()
+    >>> from crypto_screening.market.screeners import ohlcv_market_recorder
+    >>>
+    >>> market = {'binance': ['BTC/USDT'], 'bittrex': {'1m': 'ETH/USDT'}}
+    >>>
+    >>> recorder = ohlcv_market_recorder(data=market)
+    """
 
-        self.market.loc[dt.datetime.now()] = data
-    # end async_update_market
+    __modifiers__ = Modifiers(**MarketRecorder.__modifiers__)
+    __modifiers__.hidden.extend(["intervals", "ohlcv_market"])
 
-    def update_market(self) -> None:
-        """Updates the market data."""
+    __slots__ = "_index", "ohlcv_market", "intervals"
 
-        asyncio.run(self.async_update_market())
-    # end update_market
+    COLUMNS = OHLCV_COLUMNS
+    INTERVAL = OHLCVScreener.INTERVAL
 
-    def get_market(self) -> Dict[str, float]:
+    def __init__(
+            self,
+            intervals: Optional[Intervals] = None,
+            market: Optional[Market] = None,
+            ohlcv_market: Optional[OHLCVMarket] = None
+    ) -> None:
         """
-        Gets the market data.
+        Defines the class attributes.
 
-        :return: The market data.
+        :param market: The object to fill with the crypto feed record.
+        :param intervals: The intervals for the datasets.
+        :param ohlcv_market: The OHLCV market structure.
         """
 
-        return asyncio.run(self.async_get_market())
-    # end get_market
-
-    async def async_run_loop(self) -> None:
-        """Runs the processes of price screening."""
+        data = create_ohlcv_market_recorder_initializers(
+            market=market, ohlcv_market=ohlcv_market, intervals=intervals
+        )
 
-        self._screening = True
+        market = data["market"]
+        intervals = data["intervals"]
+        ohlcv_market = data["ohlcv_market"]
 
-        delay = interval_to_total_time(self.interval).seconds
+        super().__init__(market=market)
 
-        while self.screening:
-            start = time.time()
+        self.intervals = self.validate_intervals(intervals)
+        self.ohlcv_market = self.validate_market(ohlcv_market)
 
-            try:
-                await self.async_update_market()
+        self._index: Indexes = {}
+    # end __init__
 
-            except Exception as e:
-                warnings.warn(f"{type(e).__name__}: {e}")
-            # end try
+    @staticmethod
+    def validate_ohlcv_market(data: Any) -> OHLCVMarket:
+        """
+        Validates the data.
 
-            end = time.time()
+        :param data: The data to validate.
 
-            if delay:
-                time.sleep(max([delay - (end - start), 0]))
-            # end if
-        # end while
-    # end async_run
+        :return: The valid data.
+        """
 
-    def screening_loop(self) -> None:
-        """Runs the process of the price screening."""
+        return validate_ohlcv_market(data=data)
+    # end validate_ohlcv_market
 
-        task = self.async_run_loop()
+    @staticmethod
+    def validate_intervals(data: Any) -> Intervals:
+        """
+        Validates the data.
 
-        loop = asyncio.new_event_loop()
+        :param data: The data to validate.
 
-        self.task = loop.create_task(task)
+        :return: The valid data.
+        """
 
-        if not loop.is_running():
-            loop.run_forever()
-        # end if
-    # end screening_loop
+        return validate_intervals(data=data)
+    # end validate_market
 
-    def stop(self) -> None:
-        """Stops the screening process."""
+    def ohlcv(self, exchange: str, symbol: str, interval: str) -> pd.DataFrame:
+        """
+        Returns the market data of the symbol from the exchange.
 
-        super().stop()
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+        :param interval: The interval for the dataset.
 
-        if self.task is not None:
-            self.task.cancel()
-        # end if
-    # end stop
-# end OHLCVScreener
+        :return: The dataset of the spread data.
+        """
 
-class MarketOHLCVRecorder(MarketRecorder):
-    """
-    A class to represent a crypto data feed recorder.
-    This object passes the record method to the handler object to record
-    the data fetched by the handler.
+        self.data(exchange=exchange, symbol=symbol)
 
-    Parameters:
+        intervals = self.ohlcv_market[exchange][symbol]
 
-    - market:
-        The market structure of the data to store the fetched data in.
-        This structure is a dictionary with exchange names as keys
-        and dictionaries as values, where their keys are symbols,
-        and their values are the dataframes to record the data.
+        interval = find_string_value(value=interval, values=intervals)
 
-    >>> from crypto_screening.market.screeners import market_ohlcv_recorder
-    >>>
-    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
-    >>>
-    >>> recorder = market_ohlcv_recorder(data=market)
-    """
+        if interval not in intervals:
+            raise ValueError(
+                f"'{interval}' is not a valid "
+                f"interval for the symbol '{symbol}' of '{exchange}' exchange. "
+                f"Valid symbols: {', '.join(intervals.keys() or [])} for {self}."
+            )
+        # end if
 
-    COLUMNS = OHLCVScreener.COLUMNS
+        return intervals[interval]
+    # end ohlcv
 
-    def ohlcv(self, exchange: str, symbol: str) -> pd.DataFrame:
+    def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source name of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.data(exchange=exchange, symbol=symbol)
-    # end ohlcv
+    # end orderbook
+
+    async def record(self, data: OrderBook, timestamp: float) -> None:
+        """
+        Records the data from the crypto feed into the dataset.
+
+        :param data: The data from the exchange.
+        :param timestamp: The time of the request.
+        """
+
+        exchange = find_string_value(
+            value=data.exchange, values=self.market.keys()
+        )
+        symbol = find_string_value(
+            value=adjust_symbol(symbol=data.symbol),
+            values=exchange
+        )
+
+        spread_dataset = (
+            self.market.
+            setdefault(exchange, {}).
+            setdefault(symbol, create_orderbook_dataframe())
+        )
+
+        bids = data.book.bids.to_list()
+        asks = data.book.asks.to_list()
+
+        try:
+            current_index = dt.datetime.fromtimestamp(timestamp)
+
+            spread_dataset.loc[current_index] = {
+                BIDS: float(bids[0][0]),
+                ASKS: float(asks[0][0]),
+                BIDS_VOLUME: float(bids[0][1]),
+                ASKS_VOLUME: float(asks[0][1])
+            }
+
+        except IndexError:
+            return
+        # end try
+
+        for interval, ohlcv_dataset in (
+            self.ohlcv_market[exchange][symbol].items()
+        ):
+            dataset_index = (
+                self._index.
+                setdefault(exchange, {}).
+                setdefault(symbol, {}).
+                setdefault(interval, 0)
+            )
+
+            span: dt.timedelta = (
+                spread_dataset.index[-1] -
+                spread_dataset.index[dataset_index]
+            )
+
+            interval_total_time = interval_to_total_time(interval)
+
+            if (span >= interval_total_time) or (dataset_index == 0):
+                interval_total_minutes = (
+                    interval_total_time.total_seconds() // 60
+                )
+                adjuster = f'{interval_total_minutes}Min'
+
+                dataset: pd.DataFrame = (
+                    spread_dataset[BIDS].resample(adjuster).ohlc()
+                )
+                dataset.columns = [OPEN, HIGH, LOW, CLOSE]
+                volume: pd.DataFrame = (
+                    spread_dataset[BIDS_VOLUME].resample(adjuster).ohlc()
+                )
+                volume.columns = [OPEN, HIGH, LOW, CLOSE]
+                dataset[VOLUME] = volume[CLOSE]
+
+                for index, row in dataset.iterrows():
+                    ohlcv_dataset.loc[index] = row
+                # end for
+
+                self._index[exchange][symbol][interval] += 1
+            # end for
+        # end if
+    # end record
 # end MarketOHLCVRecorder
 
-def create_ohlcv_dataframe() -> pd.DataFrame:
+def structure_screener_intervals(
+        screeners: Iterable[OHLCVScreener]
+) -> Dict[str, Dict[str, List[str]]]:
     """
-    Creates a dataframe for the order book data.
+    Structures the screener objects by exchanges and symbols
 
-    :return: The dataframe.
+    :param screeners: The screeners to structure.
+
+    :return: The structure of the screeners.
     """
 
-    return create_market_dataframe(
-        columns=MarketOHLCVRecorder.COLUMNS
-    )
-# end create_orderbook_dataframe
+    structure: Dict[str, Dict[str, List[str]]] = {}
 
-def create_ohlcv_market(data: Dict[str, Iterable[str]]) -> Dict[str, Dict[str, pd.DataFrame]]:
-    """
-    Creates the dataframes of the market data.
+    for screener in screeners:
+        (
+            structure.
+            setdefault(screener.exchange, {}).
+            setdefault(screener.symbol, []).
+            append(screener.interval)
+        )
+    # end for
 
-    :param data: The market data.
+    return structure
+# end structure_screener_intervals
 
-    :return: The dataframes of the market data.
+def structure_screeners_intervals(
+        screeners: Iterable[OHLCVScreener]
+) -> OHLCVMarket:
     """
+    Structures the screener objects by exchanges and symbols
 
-    return {
-        exchange.lower(): {
-            symbol.upper(): create_ohlcv_dataframe()
-            for symbol in data[exchange]
-        } for exchange in data
-    }
-# end create_ohlcv_market
+    :param screeners: The screeners to structure.
 
-def market_ohlcv_recorder(data: Dict[str, Iterable[str]]) -> MarketOHLCVRecorder:
+    :return: The structure of the screeners.
     """
-    Creates the market recorder object for the data.
 
-    :param data: The market data.
+    structure = {}
 
-    :return: The market recorder object.
-    """
+    for screener in screeners:
+        (
+            structure.
+            setdefault(screener.exchange, {}).
+            setdefault(screener.symbol, {}).
+            setdefault(screener.interval, screeners)
+        )
+    # end for
 
-    return MarketOHLCVRecorder(
-        market=create_ohlcv_market(data=data)
-    )
-# end market_ohlcv_recorder
+    return structure
+# end structure_screeners_intervals
 
-class MarketOHLCVScreener(BaseMultiScreener):
+class OHLCVMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
     Parameters:
 
-    - exchanges:
-        The data of exchanges and their symbols to screen.
+    - screeners:
+        The screeners to connect to the market screener.
 
-    - interval:
-        The interval for the time between data points in the dataset.
+    - intervals:
+        The structure to set a specific interval to the dataset
+        of each symbol in each exchange, matching the market data.
 
-    - delay:
-        The delay to wait between each data fetching.
-
-    - length:
-        An initial dataset length to start with.
-
-    - locaion:
+    - location:
         The saving location for the saved data of the screener.
 
-    - pro:
-        The value to use the pro interface.
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
+
+    - delay:
+        The delay to wait between each data fetching.
 
-    - options:
-        The ccxt options for the backend screening process.
+    - handler:
+        The handler object to handle the data feed.
 
-    - cencel:
-        The time to cancel screening process after no new data is fetched.
+    - recorder:
+        The recorder object to record the data of the market from the feed.
 
-    >>> from crypto_screening.market.screeners import MarketOHLCVScreener
+    >>> from crypto_screening.market.screeners import orderbook_market_screener
     >>>
-    >>> screener = MarketOHLCVScreener(
-    >>>     data={
-    >>>         "binance": ["BTC/USDT", "AAVE/EUR"],
-    >>>         "bittrex": ["GRT/USD", "BTC/USD"]
-    >>>     }
-    >>> )
+    >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> screener.run(wait=True)
+    >>> screener = orderbook_market_screener(data=structure)
+    >>> screener.run()
     """
 
-    __slots__ = "interval", "pro", "options", "task", "exchanges", "length"
-
-    INTERVAL = OHLCVScreener.INTERVAL
-
-    PRO = OHLCVScreener.PRO
+    screeners: List[Union[OHLCVScreener, OrderbookScreener]]
+    recorder: OHLCVMarketRecorder
 
-    OPTIONS = OHLCVScreener.OPTIONS
-
-    LENGTH = OHLCVScreener.LENGTH
-    CANCEL = OHLCVScreener.CANCEL
-
-    COLUMNS = OHLCVScreener.COLUMNS
-
-    screeners: List[OHLCVScreener]
+    COLUMNS = OHLCVMarketRecorder.COLUMNS
+    INTERVAL = OHLCVMarketRecorder.INTERVAL
 
     def __init__(
             self,
-            interval: Optional[str] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            length: Optional[Union[int, bool]] = None,
+            intervals: Optional[Intervals] = None,
+            market: Optional[Market] = None,
+            ohlcv_market: Optional[OHLCVMarket] = None,
+            screeners: Optional[Iterable[Union[OHLCVScreener, OrderbookScreener]]] = None,
             location: Optional[str] = None,
-            pro: Optional[bool] = None,
-            options: Optional[Dict[str, Any]] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
-            screeners: Optional[Iterable[OHLCVScreener]] = None,
-            recorder: Optional[MarketRecorder] = None
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            refresh: Optional[Union[float, dt.timedelta, bool]] = None,
+            limited: Optional[bool] = None,
+            handler: Optional[FeedHandler] = None,
+            amount: Optional[int] = None,
+            recorder: Optional[OHLCVMarketRecorder] = None
     ) -> None:
         """
-        Defines the class attributes.
+        Creates the class attributes.
 
-        :param interval: The interval of the data to load.
-        :param pro: The value to use the pro interface.
         :param location: The saving location for the data.
-        :param delay: The delay between each data fetching request.
-        :param length: The length of the data to get in each request.
-        :param options: The ccxt options.
-        :param cancel: The time it takes to cancel a non-updating screener.
-        :param screeners: The create_screeners for the multi-screener object.
+        :param intervals: The intervals for the datasets.
+        :param delay: The delay for the process.
+        :param cancel: The cancel time for the loops.
+        :param limited: The value to limit the screeners to active only.
+        :param refresh: The refresh time for rerunning.
+        :param handler: The handler object for the market data.
+        :param amount: The maximum amount of symbols for each feed.
         :param recorder: The recorder object for recording the data.
         """
 
+        screeners = screeners or []
+
+        data = create_ohlcv_market_recorder_initializers(
+            market=market or structure_screener_datasets(screeners=screeners),
+            intervals=intervals or structure_screener_intervals(screeners=screeners),
+            ohlcv_market=ohlcv_market,
+        )
+
+        market = data["market"]
+        intervals = data["intervals"]
+        ohlcv_market = data["ohlcv_market"]
+
         super().__init__(
-            delay=delay, cancel=cancel,
-            location=location, recorder=recorder or MarketOHLCVRecorder(
-                market=structure_screener_datasets(screeners=screeners)
-            )
+            location=location, cancel=cancel,
+            delay=delay, recorder=recorder or OHLCVMarketRecorder(
+                market=market, intervals=intervals, ohlcv_market=ohlcv_market
+            ),
+            screeners=screeners, handler=handler, limited=limited,
+            amount=amount, refresh=refresh
         )
 
-        if pro is None:
-            pro = self.PRO
-        # end if
+        self.screeners[:] = self.screeners or []
+        self.screeners.extend(self.create_ohlcv_screeners())
+        self.screeners.extend(self.create_orderbook_screeners())
+    # end __init__
 
-        if length is None:
-            length = self.LENGTH
-        # end if
+    @property
+    def orderbook_screeners(self) -> List[OrderbookScreener]:
+        """
+        Returns a list of all the order-book screeners.
 
-        self.options = options or self.OPTIONS
-        self.interval = interval or self.INTERVAL
-        self.pro = pro
-        self.length = length
+        :return: The order-book screeners.
+        """
+
+        return [
+            screener for screener in self.screeners
+            if isinstance(screener, OrderbookScreener)
+        ]
+    # end orderbook_screeners
+
+    @property
+    def ohlcv_screeners(self) -> List[OHLCVScreener]:
+        """
+        Returns a list of all the ohlcv screeners.
+
+        :return: The ohlcv screeners.
+        """
 
-        self.screeners[:] = list(screeners or []) or self.create_screeners()
-    # end Screener
+        return [
+            screener for screener in self.screeners
+            if isinstance(screener, OHLCVScreener)
+        ]
+    # end ohlcv_screeners
 
-    def create_screener(
+    def create_ohlcv_screener(
             self,
             symbol: str,
             exchange: str,
-            pro: Optional[bool] = True,
-            length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
+            interval: Optional[str] = None,
             location: Optional[str] = None,
-            options: Optional[Dict[str, Any]] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             container: Optional[Dict[str, Dict[str, OHLCVScreener]]] = None
     ) -> OHLCVScreener:
         """
-        Creates the screener and inserts it into the container.
+        Defines the class attributes.
 
-        :param container: The container to contain the new screener.
-        :param symbol: The symbol of the screener.
-        :param exchange: The source of the data.
-        :param pro: The value to use the pro interface.
+        :param symbol: The symbol of the asset.
+        :param exchange: The exchange to get source data from.
         :param location: The saving location for the data.
-        :param delay: The delay between each data fetching request.
-        :param length: The length of the data to get in each request.
-        :param options: The ccxt options.
-        :param cancel: The time it takes to cancel a non-updating screener.
+        :param cancel: The time to cancel the waiting.
+        :param delay: The delay for the process.
+        :param container: The container to contain the new screener.
+        :param interval: The interval for the dataset.
         """
 
-        if container is None:
-            container = {}
-        # end if
-
-        if pro is None:
-            pro = self.pro
+        if interval is None:
+            interval = self.INTERVAL
         # end if
 
-        if length is None:
-            length = self.length
+        if container is None:
+            container = {}
         # end if
 
         if cancel is None:
             cancel = self.cancel
         # end if
 
         if delay is None:
             delay = self.delay
         # end if
 
-        container.setdefault(exchange, {})[symbol] = OHLCVScreener(
-            symbol=symbol, exchange=exchange,
-            options=options, interval=self.interval,
-            pro=pro, delay=delay, length=length,
-            location=location or self.location, cancel=cancel
+        screener = OHLCVScreener(
+            symbol=symbol, exchange=exchange, delay=delay,
+            location=location, cancel=cancel, market=(
+                self.recorder.ohlcv(
+                    exchange=exchange, symbol=symbol, interval=interval
+                )
+                if self.in_market(symbol=symbol, exchange=exchange)
+                else None
+            ),
+            base_market=(
+                self.recorder.orderbook(exchange=exchange, symbol=symbol)
+                if self.in_market(symbol=symbol, exchange=exchange)
+                else None
+            )
         )
 
-        return container[exchange][symbol]
-    # end create_screener
+        container.setdefault(exchange, {})[symbol] = screener
+
+        return screener
+    # end create_ohlcv_screener
 
-    def _create_screener(
+    def create_ohlcv_screeners(
             self,
-            symbol: str,
-            exchange: str,
-            pro: Optional[bool] = True,
-            length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
+            interval: Optional[str] = None,
+            intervals: Optional[Intervals] = None,
             location: Optional[str] = None,
-            options: Optional[Dict[str, Any]] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, Optional[OHLCVScreener]]]] = None,
-    ) -> OHLCVScreener:
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            container: Optional[Dict[str, Dict[str, OHLCVScreener]]] = None
+    ) -> List[OHLCVScreener]:
         """
-        Creates the screener and inserts it into the container.
+        Defines the class attributes.
 
-        :param container: The container to contain the new screener.
-        :param symbol: The symbol of the screener.
-        :param exchange: The source of the data.
-        :param pro: The value to use the pro interface.
+        :param interval: The interval for the dataset.
+        :param intervals: The intervals for the screeners.
         :param location: The saving location for the data.
-        :param delay: The delay between each data fetching request.
-        :param length: The length of the data to get in each request.
-        :param options: The ccxt options.
-        :param cancel: The time it takes to cancel a non-updating screener.
+        :param cancel: The time to cancel the waiting.
+        :param delay: The delay for the process.
+        :param container: The container to contain the new screeners.
         """
 
-        if container is None:
-            container = {}
-        # end if
+        screeners = []
 
         try:
-            return self.create_screener(
-                symbol=symbol, exchange=exchange,
-                container=container, pro=pro, length=length,
-                delay=delay, location=location,
-                options=options, cancel=cancel
-            )
+            validate_intervals(intervals)
 
-        except ValueError as e:
-            warnings.warn(str(e))
+            valid = True
 
-            container.setdefault(exchange, {})[symbol] = None
+        except ValueError:
+            valid = False
         # end try
-    # end _create_screener
-
-    def _create_screeners(
-            self,
-            symbols: Iterable[str],
-            exchange: str,
-            pro: Optional[bool] = True,
-            length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            location: Optional[str] = None,
-            options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, Optional[OHLCVScreener]]]] = None,
-            wait: Optional[bool] = True
-    ) -> Dict[str, Optional[OHLCVScreener]]:
-        """
-        Creates the screener and inserts it into the container.
-
-        :param container: The container to contain the new screener.
-        :param symbols: The symbol of the screener.
-        :param exchange: The source of the data.
-        :param wait: The value to wait for the creation of the screeners.
-        :param pro: The value to use the pro interface.
-        :param location: The saving location for the data.
-        :param delay: The delay between each data fetching request.
-        :param length: The length of the data to get in each request.
-        :param options: The ccxt options.
-        :param cancel: The time it takes to cancel a non-updating screener.
-        """
-
-        if container is None:
-            container = {}
-        # end if
-
-        symbols = list(symbols)
-
-        callers = []
-
-        for symbol in symbols:
-            callers.append(
-                Caller(
-                    target=self._create_screener,
-                    kwargs=dict(
-                        container=container,
-                        symbol=symbol, exchange=exchange,
-                        pro=pro, length=length,
-                        delay=delay, location=location,
-                        options=options, cancel=cancel
-                    )
-                )
-            )
-        # end for
-
-        multi_threaded_call(callers=callers, wait=wait)
-
-        return container
-    # end _create_screeners
 
-    def create_screeners(
-            self,
-            pro: Optional[bool] = True,
-            length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            location: Optional[str] = None,
-            options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-    ) -> List[OHLCVScreener]:
-        """
-        Initializes the create_screeners.
+        for exchange in self.market:
+            for symbol in self.market[exchange]:
+                if valid:
+                    interval = intervals[exchange][symbol]
+                # end if
 
-        :param pro: The value to use the pro interface.
-        :param location: The saving location for the data.
-        :param delay: The delay between each data fetching request.
-        :param length: The length of the data to get in each request.
-        :param options: The ccxt options.
-        :param cancel: The time it takes to cancel a non-updating screener.
-
-        :return: The created screener objects.
-        """
-
-        market: Dict[str, Dict[str, OHLCVScreener]] = {}
-
-        callers = []
-
-        for exchange, symbols in self.recorder.structure().items():
-            market.setdefault(exchange, {})
-
-            callers.append(
-                Caller(
-                    target=self._create_screeners,
-                    kwargs=dict(
-                        container=market, symbols=symbols,
-                        exchange=exchange, wait=False,
-                        pro=pro, length=length,
-                        delay=delay, location=location,
-                        options=options, cancel=cancel
+                screeners.append(
+                    self.create_ohlcv_screener(
+                        symbol=symbol, exchange=exchange, delay=delay,
+                        location=location, cancel=cancel,
+                        container=container, interval=interval
                     )
                 )
-            )
-        # end for
-
-        screeners = []
-
-        for exchange, symbols in market.items():
-            for symbol, screener in symbols.items():
-                if isinstance(screener, OHLCVScreener):
-                    screeners.append(screener)
-                # end if
             # end for
         # end for
 
         return screeners
-    # end create_screeners
-
-    def ohlcv(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source name of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        return self.recorder.ohlcv(exchange=exchange, symbol=symbol)
-    # end ohlcv
-
-    async def async_get_market(self) -> Dict[str, Dict[str, Dict[str, float]]]:
-        """
-        Gets the market data.
+    # end create_ohlcv_screeners
 
-        :return: The market data.
-        """
-
-        market = {exchange: {} for exchange in self.exchanges}
-
-        for screener in self.screeners:
-            market[screener.exchange][screener.symbol] = (
-                await screener.async_get_market()
-            )
-        # end for
-
-        return market
-    # end async_get_market
-
-    async def async_update_market(self) -> None:
-        """Updates the market data."""
-
-        for screener in self.screeners:
-            await screener.async_update_market()
-        # end for
-    # end async_update_market
-
-    def update_market(self) -> None:
-        """Updates the market data."""
-
-        asyncio.run(self.async_update_market())
-    # end update_market
-
-    def get_market(self) -> Dict[str, Dict[str, Dict[str, float]]]:
-        """
-        Gets the market data.
-
-        :return: The market data.
-        """
-
-        return asyncio.run(self.async_get_market())
-    # end get_market
-
-    def stop(self) -> None:
-        """Stops the screening process."""
-
-        super().stop()
-
-        for screener in self.screeners:
-            screener.stop()
-        # end for
-    # end stop
-
-    def terminate(self) -> None:
-        """Stops the screening process."""
-
-        super().terminate()
-
-        for screener in self.screeners:
-            screener.terminate()
-        # end for
-    # end terminate
-
-    def start_screening(
-            self,
-            save: Optional[bool] = True,
-            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> None:
-        """
-        Starts the screening process.
-
-        :param save: The value to save the data.
-        :param timeout: The valur to add a timeout to the process.
-        """
-
-        if self.screening:
-            warnings.warn(f"Screening process of {self} is already running.")
+    create_orderbook_screener = OrderbookMarketScreener.create_orderbook_screener
+    create_orderbook_screeners = OrderbookMarketScreener.create_orderbook_screeners
+# end MarketOHLCVRecorder
 
-            return
-        # end if
+def ohlcv_market_recorder(
+        data: Union[Intervals, Dict[str, Iterable[str]]],
+        interval: Optional[str] = None
+) -> OHLCVMarketRecorder:
+    """
+    Creates the market recorder object for the data.
 
-        for screener in self.screeners:
-            screener.run(
-                timeout=timeout, wait=False,
-                block=False, save=save
-            )
-        # end for
-    # end start_screening
+    :param data: The market data.
+    :param interval: The interval for the structure.
 
-    def run(
-            self,
-            screen: Optional[bool] = True,
-            save: Optional[bool] = True,
-            block: Optional[bool] = False,
-            update: Optional[bool] = True,
-            wait: Optional[Union[bool, float, dt.timedelta, dt.datetime]] = False,
-            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> None:
-        """
-        Runs the process of the price screening.
+    :return: The market recorder object.
+    """
 
-        :param screen: The value to start the screening.
-        :param save: The value to save the data.
-        :param wait: The value to wait after starting to run the process.
-        :param block: The value to block the execution.
-        :param update: The value to update the screeners.
-        :param timeout: The valur to add a timeout to the process.
-        """
+    try:
+        intervals = validate_ohlcv_market(data)
 
-        if screen:
-            self.start_screening(save=save, timeout=timeout)
-        # end if
+    except ValueError:
+        validate_market(data)
 
-        super().run(
-            screen=False, save=False, block=block,
-            update=update, wait=wait, timeout=timeout
+        intervals = datasets_to_intervals_datasets(
+            data=data, interval=interval
         )
-    # end run
-# end MarketOHLCVScreener
+    # end try
 
-Market = Dict[str, Dict[str, pd.DataFrame]]
+    return OHLCVMarketRecorder(intervals=intervals, market=data)
+# end ohlcv_market_recorder
 
-def market_ohlcv_screener(
-        data: Dict[str, Iterable[str]],
-        interval: Optional[str] = None,
-        delay: Optional[Union[float, dt.timedelta]] = None,
-        length: Optional[Union[int, bool]] = None,
+def ohlcv_market_screener(
+        data: Union[Intervals, Dict[str, Iterable[str]]],
+        intervals: Optional[Intervals] = None,
+        market: Optional[Market] = None,
+        ohlcv_market: Optional[OHLCVMarket] = None,
         location: Optional[str] = None,
-        pro: Optional[bool] = None,
-        options: Optional[Dict[str, Any]] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
-        market: Optional[Market] = None,
-        recorder: Optional[MarketOHLCVRecorder] = None,
-) -> MarketOHLCVScreener:
+        delay: Optional[Union[float, dt.timedelta]] = None,
+        limited: Optional[bool] = None,
+        handler: Optional[FeedHandler] = None,
+        amount: Optional[int] = None,
+        refresh: Optional[Union[float, dt.timedelta, bool]] = None,
+        recorder: Optional[OHLCVMarketRecorder] = None,
+        fixed: Optional[bool] = True,
+        separator: Optional[str] = None,
+        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
+) -> OHLCVMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
+    :param handler: The handler object for the market data.
+    :param limited: The value to limit the screeners to active only.
+    :param parameters: The parameters for the exchanges.
     :param market: The object to fill with the crypto feed record.
+    :param intervals: The intervals for the datasets.
+    :param ohlcv_market: The OHLCV market structure.
+    :param fixed: The value for fixed parameters to all exchanges.
+    :param refresh: The refresh time for rerunning.
+    :param amount: The maximum amount of symbols for each feed.
+    :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
-    :param interval: The interval of the data to load.
-    :param pro: The value to use the pro interface.
     :param location: The saving location for the data.
-    :param delay: The delay between each data fetching request.
-    :param length: The length of the data to get in each request.
-    :param options: The ccxt options.
-    :param cancel: The time it takes to cancel a non-updating screener.
+    :param delay: The delay for the process.
+    :param cancel: The cancel time for the loops.
 
     :return: The market screener object.
     """
 
-    screener = MarketOHLCVScreener(
-        recorder=recorder or MarketOHLCVRecorder(
-            market=market or create_ohlcv_market(data=data)
+    try:
+        intervals = validate_intervals(data)
+
+    except ValueError:
+        market = create_orderbook_market(data)
+    # end try
+
+    screener = OHLCVMarketScreener(
+        recorder=recorder or OHLCVMarketRecorder(
+            market=market, ohlcv_market=ohlcv_market, intervals=intervals
         ),
-        location=location, cancel=cancel, delay=delay,
-        options=options, pro=pro, interval=interval, length=length
+        handler=handler, location=location, amount=amount,
+        cancel=cancel, delay=delay, limited=limited, refresh=refresh
+    )
+
+    screener.add_feeds(
+        data=screener.recorder.structure(), fixed=fixed,
+        separator=separator, parameters=parameters
     )
 
     return screener
-# end market_orderbook_recorder
+# end orderbook_market_recorder
```

### Comparing `crypto-screening-2.8.4/crypto_screening/market/waiting.py` & `crypto-screening-3.0.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/process.py` & `crypto-screening-3.0.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/symbols.py` & `crypto-screening-3.0.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening/validate.py` & `crypto-screening-3.0.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-3.0.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.4
+Version: 3.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.4/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-3.0.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.4/pyproject.toml` & `crypto-screening-3.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.8.4'
+version = '3.0.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.8.4/setup.py` & `crypto-screening-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.8.4',
+        version='3.0.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```


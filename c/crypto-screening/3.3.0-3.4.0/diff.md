# Comparing `tmp/crypto-screening-3.3.0.tar.gz` & `tmp/crypto-screening-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-3.3.0.tar", last modified: Thu Jul 13 18:26:25 2023, max compression
+gzip compressed data, was "crypto-screening-3.4.0.tar", last modified: Thu Jul 13 18:46:44 2023, max compression
```

## Comparing `crypto-screening-3.3.0.tar` & `crypto-screening-3.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:25.666912 crypto-screening-3.3.0/
--rw-rw-rw-   0        0        0       98 2023-07-13 18:26:25.000000 crypto-screening-3.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-13 18:26:25.665910 crypto-screening-3.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-3.3.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-3.3.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:25.638173 crypto-screening-3.3.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:25.655381 crypto-screening-3.3.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-3.3.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-3.3.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    43277 2023-07-13 18:16:12.000000 crypto-screening-3.3.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21191 2023-07-13 17:18:17.000000 crypto-screening-3.3.0/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19312 2023-07-13 17:18:17.000000 crypto-screening-3.3.0/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-3.3.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-3.3.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    13639 2023-07-13 15:21:10.000000 crypto-screening-3.3.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-3.3.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-3.3.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:25.656381 crypto-screening-3.3.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    10473 2023-07-13 18:26:10.000000 crypto-screening-3.3.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:25.659890 crypto-screening-3.3.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-3.3.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-3.3.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-3.3.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-3.3.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:25.664910 crypto-screening-3.3.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-3.3.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    18442 2023-07-13 14:37:22.000000 crypto-screening-3.3.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     5832 2023-07-13 18:26:10.000000 crypto-screening-3.3.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    30311 2023-07-13 17:42:52.000000 crypto-screening-3.3.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    14109 2023-07-13 13:54:09.000000 crypto-screening-3.3.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    14866 2023-07-13 13:45:46.000000 crypto-screening-3.3.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-3.3.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-3.3.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-3.3.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-3.3.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:25.649874 crypto-screening-3.3.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-13 18:26:25.000000 crypto-screening-3.3.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-13 18:26:25.000000 crypto-screening-3.3.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 18:26:25.000000 crypto-screening-3.3.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-13 18:26:25.000000 crypto-screening-3.3.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-13 18:26:25.000000 crypto-screening-3.3.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-13 18:26:25.000000 crypto-screening-3.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-3.3.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-3.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 18:26:25.666912 crypto-screening-3.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-13 18:26:21.000000 crypto-screening-3.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:46:44.679355 crypto-screening-3.4.0/
+-rw-rw-rw-   0        0        0       98 2023-07-13 18:46:44.000000 crypto-screening-3.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-13 18:46:44.678354 crypto-screening-3.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-3.4.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-3.4.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:46:44.655355 crypto-screening-3.4.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-13 18:46:44.669354 crypto-screening-3.4.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-3.4.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-3.4.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    43277 2023-07-13 18:16:12.000000 crypto-screening-3.4.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21191 2023-07-13 17:18:17.000000 crypto-screening-3.4.0/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19312 2023-07-13 17:18:17.000000 crypto-screening-3.4.0/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-3.4.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-3.4.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    13639 2023-07-13 15:21:10.000000 crypto-screening-3.4.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-3.4.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-3.4.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:46:44.670355 crypto-screening-3.4.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10933 2023-07-13 18:45:57.000000 crypto-screening-3.4.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:46:44.673355 crypto-screening-3.4.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-3.4.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-3.4.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-3.4.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-3.4.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:46:44.677356 crypto-screening-3.4.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-3.4.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    18442 2023-07-13 14:37:22.000000 crypto-screening-3.4.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     7012 2023-07-13 18:45:57.000000 crypto-screening-3.4.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    30311 2023-07-13 17:42:52.000000 crypto-screening-3.4.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    14109 2023-07-13 13:54:09.000000 crypto-screening-3.4.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    14866 2023-07-13 13:45:46.000000 crypto-screening-3.4.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-3.4.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-3.4.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-3.4.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-3.4.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:46:44.664355 crypto-screening-3.4.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-13 18:46:44.000000 crypto-screening-3.4.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-13 18:46:44.000000 crypto-screening-3.4.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:46:44.000000 crypto-screening-3.4.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-13 18:46:44.000000 crypto-screening-3.4.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-13 18:46:44.000000 crypto-screening-3.4.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-13 18:46:44.000000 crypto-screening-3.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-3.4.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-3.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 18:46:44.679355 crypto-screening-3.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-13 18:46:36.000000 crypto-screening-3.4.0/setup.py
```

### Comparing `crypto-screening-3.3.0/PKG-INFO` & `crypto-screening-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 3.3.0
+Version: 3.4.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-3.3.0/README.md` & `crypto-screening-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/build.py` & `crypto-screening-3.4.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/collect/assets.py` & `crypto-screening-3.4.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/collect/exchanges.py` & `crypto-screening-3.4.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/collect/market.py` & `crypto-screening-3.4.0/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/collect/ohlcv.py` & `crypto-screening-3.4.0/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/collect/orderbook.py` & `crypto-screening-3.4.0/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/collect/screeners.py` & `crypto-screening-3.4.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/collect/symbols.py` & `crypto-screening-3.4.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/dataset.py` & `crypto-screening-3.4.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/interval.py` & `crypto-screening-3.4.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/dynamic.py` & `crypto-screening-3.4.0/crypto_screening/market/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional, Iterable, List, Union, Dict
 
 from represent import Modifiers
 
 import pandas as pd
 
 from crypto_screening.collect.screeners import exchanges_symbols_screeners
+from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.collect.orderbook import (
     assets_orderbook_market_state, symbols_orderbook_market_state,
     SymbolsOrderbookMarketState, AssetsOrderbookMarketState
 )
 from crypto_screening.collect.ohlcv import (
     assets_ohlcv_market_state, symbols_ohlcv_market_state,
     SymbolsOHLCVMarketState, AssetsOHLCVMarketState
@@ -85,21 +86,37 @@
         :param exchange: The exchange name.
         :param symbol: The ticker name.
         :param length: The length of the data.
 
         :return: The data.
         """
 
-        screener = self.find_orderbook_screener(
-            exchange=exchange, symbol=symbol
-        )
+        try:
+            screener = self.find_orderbook_screener(
+                exchange=exchange, symbol=symbol
+            )
 
-        length = min(length or 0, len(screener.market))
+            market = screener.market
 
-        return screener.market.iloc[-length:]
+        except ValueError:
+            screener = self.find_screener(
+                exchange=exchange, symbol=symbol
+            )
+
+            if isinstance(screener, OHLCVScreener):
+                market = screener.base_market
+
+            else:
+                market = screener.market
+            # end if
+        # end try
+
+        length = min(length or 0, len(market))
+
+        return market.iloc[-length:]
     # end find_orderbook_dataset
 
     def find_datasets(
             self,
             exchange: str,
             symbol: str,
             length: Optional[int] = None
```

### Comparing `crypto-screening-3.3.0/crypto_screening/market/foundation/data.py` & `crypto-screening-3.4.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-3.4.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/foundation/state.py` & `crypto-screening-3.4.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-3.4.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/screeners/base.py` & `crypto-screening-3.4.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/screeners/container.py` & `crypto-screening-3.4.0/crypto_screening/market/screeners/container.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,29 +62,50 @@
 
         :return: The data.
         """
 
         if not self.in_market(exchange=exchange, symbol=symbol):
             raise ValueError(
                 f"Screener object for symbol - {symbol} and "
-                f"exchange - {exchange} cannot be found in {self}."
+                f"exchange - {exchange} cannot be found in {repr(self)}."
             )
         # end if
 
         screeners = []
 
         for screener in self.screeners:
             if (screener.exchange == exchange) and (screener.symbol == symbol):
                 screeners.append(screener)
             # end if
         # end for
 
         return screeners
     # end find_screeners
 
+    def orderbook_screener_in_market(self, exchange: str, symbol: str) -> bool:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        try:
+            self.find_orderbook_screener(
+                exchange=exchange, symbol=symbol
+            )
+
+            return True
+
+        except ValueError:
+            return False
+    # end orderbook_screener_in_market
+
     def find_orderbook_screener(self, exchange: str, symbol: str) -> OrderbookScreener:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
 
@@ -99,15 +120,15 @@
             ):
                 return screener
             # end if
         # end for
 
         raise ValueError(
             f"Orderbook Screener object for symbol - {symbol} and "
-            f"exchange - {exchange} cannot be found in {self}."
+            f"exchange - {exchange} cannot be found in {repr(self)}."
         )
     # end find_orderbook_screener
 
     def find_orderbook_screeners(self, exchange: str, symbol: str) -> List[OrderbookScreener]:
         """
         Returns the data by according to the parameters.
 
@@ -128,14 +149,38 @@
                 screeners.append(screener)
             # end if
         # end for
 
         return screeners
     # end find_orderbook_screener
 
+    def ohlcv_screener_in_market(
+            self, exchange: str, symbol: str, interval: str
+    ) -> bool:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+        :param interval: The interval for the dataset.
+
+        :return: The data.
+        """
+
+        try:
+            self.find_ohlcv_screener(
+                exchange=exchange, symbol=symbol, interval=interval
+            )
+
+            return True
+
+        except ValueError:
+            return False
+    # end ohlcv_screener_in_market
+
     def find_ohlcv_screener(
             self, exchange: str, symbol: str, interval: str
     ) -> OHLCVScreener:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
@@ -154,15 +199,15 @@
             ):
                 return screener
             # end if
         # end for
 
         raise ValueError(
             f"OHLCV Screener object for symbol - {symbol} and "
-            f"exchange - {exchange} cannot be found in {self}."
+            f"exchange - {exchange} cannot be found in {repr(self)}."
         )
     # end find_screeners
 
     def find_ohlcv_screeners(
             self, exchange: str, symbol: str, interval: str
     ) -> List[OHLCVScreener]:
         """
```

### Comparing `crypto-screening-3.3.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-3.4.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-3.4.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-3.4.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/market/waiting.py` & `crypto-screening-3.4.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/process.py` & `crypto-screening-3.4.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/symbols.py` & `crypto-screening-3.4.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening/validate.py` & `crypto-screening-3.4.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-3.4.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 3.3.0
+Version: 3.4.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-3.3.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-3.4.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.3.0/pyproject.toml` & `crypto-screening-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '3.3.0'
+version = '3.4.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-3.3.0/setup.py` & `crypto-screening-3.4.0/setup.py`

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
-        version='3.3.0',
+        version='3.4.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```


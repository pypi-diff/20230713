# Comparing `tmp/crypto-screening-2.7.1.tar.gz` & `tmp/crypto-screening-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.7.1.tar", last modified: Wed Jul 12 05:52:16 2023, max compression
+gzip compressed data, was "crypto-screening-2.8.0.tar", last modified: Wed Jul 12 22:52:38 2023, max compression
```

## Comparing `crypto-screening-2.7.1.tar` & `crypto-screening-2.8.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.295759 crypto-screening-2.7.1/
--rw-rw-rw-   0        0        0       98 2023-07-12 05:52:15.000000 crypto-screening-2.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-12 05:52:16.295759 crypto-screening-2.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.7.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.7.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.272786 crypto-screening-2.7.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.285745 crypto-screening-2.7.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.7.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.7.1/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    54885 2023-07-12 05:52:05.000000 crypto-screening-2.7.1/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.7.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.7.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.7.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.7.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.7.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.287745 crypto-screening-2.7.1/crypto_screening/market/
--rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.7.1/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.290252 crypto-screening-2.7.1/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.294813 crypto-screening-2.7.1/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.7.1/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.7.1/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.7.1/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.7.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.282235 crypto-screening-2.7.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-12 05:52:15.000000 crypto-screening-2.7.1/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.7.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.7.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 05:52:16.295759 crypto-screening-2.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-12 05:52:12.000000 crypto-screening-2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.123528 crypto-screening-2.8.0/
+-rw-rw-rw-   0        0        0       98 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-12 22:52:38.123528 crypto-screening-2.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.029834 crypto-screening-2.8.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.067431 crypto-screening-2.8.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    39228 2023-07-12 22:48:08.000000 crypto-screening-2.8.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21241 2023-07-12 22:49:02.000000 crypto-screening-2.8.0/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19325 2023-07-12 22:49:02.000000 crypto-screening-2.8.0/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.068439 crypto-screening-2.8.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.085409 crypto-screening-2.8.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.122557 crypto-screening-2.8.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.042835 crypto-screening-2.8.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 22:52:38.124529 crypto-screening-2.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-12 22:52:23.000000 crypto-screening-2.8.0/setup.py
```

### Comparing `crypto-screening-2.7.1/PKG-INFO` & `crypto-screening-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.7.1
+Version: 2.8.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.7.1/README.md` & `crypto-screening-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/build.py` & `crypto-screening-2.8.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/collect/assets.py` & `crypto-screening-2.8.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/collect/exchanges.py` & `crypto-screening-2.8.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/collect/market.py` & `crypto-screening-2.8.0/crypto_screening/collect/market.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,63 +12,57 @@
 from represent import represent, Modifiers
 
 import numpy as np
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
-from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, dataset_to_json
-)
+from crypto_screening.dataset import dataset_to_json
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
 from crypto_screening.collect.screeners import (
     find_screeners, screeners_to_assets_datasets,
     screeners_to_symbols_datasets
 )
-from crypto_screening.market.screeners.orderbook import (
-    create_orderbook_dataframe
-)
 
 __all__ = [
     "validate_assets_market_state_prices_symbol",
     "assets_market_price",
     "is_symbol_in_assets_market_prices",
     "symbols_market_prices",
-    "symbols_market_state",
     "symbols_market_price",
-    "merge_assets_market_states",
-    "merge_symbols_market_states",
     "assets_market_prices",
     "validate_symbols_market_state_prices_symbol",
-    "assets_market_state",
-    "AssetsMarketState",
-    "SymbolsMarketState",
     "is_exchange_in_market_prices",
     "is_symbol_in_symbols_market_prices",
-    "symbol_market_prices_to_assets_market_prices",
-    "symbols_market_state_to_assets_market_state",
-    "assets_market_state_to_symbols_market_state",
-    "assets_market_prices_to_symbol_market_prices",
+    "symbol_to_assets_market_prices",
+    "assets_to_symbol_market_prices",
     "assets_market_dataset_to_symbols_market_datasets",
-    "symbols_market_dataset_to_assets_market_datasets",
+    "symbols_to_assets_market_datasets",
     "symbols_screeners",
     "symbols_market_datasets_to_symbols_screeners",
     "assets_screeners",
     "assets_market_datasets_to_assets_screeners",
-    "assets_market_data_to_symbols_market_data",
+    "assets_to_symbols_market_data",
     "add_symbols_data_to_screeners",
     "add_assets_data_to_screeners",
-    "symbols_market_data_to_assets_market_data",
+    "symbols_to_assets_market_data",
     "merge_symbols_market_data",
     "merge_assets_market_data",
     "dataset_to_data",
     "symbols_datasets_to_symbols_data",
     "assets_datasets_to_assets_data",
     "screeners_to_symbols_data",
-    "screeners_to_assets_data"
+    "screeners_to_assets_data",
+    "MarketBase",
+    "assets_market_data",
+    "symbols_market_data",
+    "assets_market_state",
+    "symbols_market_state",
+    "merge_assets_market_states",
+    "merge_symbols_market_states"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 def is_exchange_in_market_prices(
         exchange: str,
@@ -284,193 +278,14 @@
     )
 
     data = list(prices[exchange][symbol])
 
     return data[-1][0], float(data[-1][-1])
 # end symbols_market_price
 
-@define(repr=False)
-@represent
-class AssetsMarketBase(metaclass=ABCMeta):
-    """
-    A class to represent the current market state.
-
-    This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
-
-    attributes:
-
-    - screeners:
-        The screener objects to collect the prices of the assets.
-    """
-
-    screeners: Iterable[BaseScreener]
-
-    __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=["screeners"])
-
-    def __hash__(self) -> int:
-        """
-        Returns the hash of the object.
-
-        :return: The hash of the object.
-        """
-
-        return id(self)
-    # end __hash__
-
-    def in_bids_prices(
-            self,
-            exchange: str,
-            symbol: str,
-            separator: Optional[str] = None
-    ) -> bool:
-        """
-        Checks if the symbol is in the prices' data.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to search.
-        :param separator: The separator of the assets.
-
-        :return: The validation value.
-        """
-
-        return is_symbol_in_assets_market_prices(
-            exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.bids
-        )
-    # end in_bids_prices
-
-    def in_asks_prices(
-            self,
-            exchange: str,
-            symbol: str,
-            separator: Optional[str] = None
-    ) -> bool:
-        """
-        Checks if the symbol is in the prices' data.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to search.
-        :param separator: The separator of the assets.
-
-        :return: The validation value.
-        """
-
-        return is_symbol_in_assets_market_prices(
-            exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.asks
-        )
-    # end in_asks_prices
-
-    def in_prices(
-            self,
-            exchange: str,
-            symbol: str,
-            separator: Optional[str] = None
-    ) -> bool:
-        """
-        Checks if the symbol is in the prices' data.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to search.
-        :param separator: The separator of the assets.
-
-        :return: The validation value.
-        """
-
-        return (
-            self.in_bids_prices(
-                exchange=exchange, symbol=symbol,
-                separator=separator
-            )
-            and
-            self.in_asks_prices(
-                exchange=exchange, symbol=symbol,
-                separator=separator
-            )
-        )
-    # end in_prices
-# end AssetsMarketBase
-
-@define(repr=False)
-@represent
-class SymbolsMarketBase(metaclass=ABCMeta):
-    """
-    A class to represent the current market state.
-
-    This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
-
-    attributes:
-
-    - screeners:
-        The screener objects to collect the prices of the assets.
-    """
-
-    screeners: Iterable[BaseScreener]
-
-    __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=["screeners"])
-
-    def __hash__(self) -> int:
-        """
-        Returns the hash of the object.
-
-        :return: The hash of the object.
-        """
-
-        return id(self)
-    # end __hash__
-
-    def in_bids_prices(self, exchange: str, symbol: str) -> bool:
-        """
-        Checks if the symbol is in the prices' data.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to search.
-
-        :return: The validation value.
-        """
-
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.bids
-        )
-    # end in_bids_prices
-
-    def in_asks_prices(self, exchange: str, symbol: str) -> bool:
-        """
-        Checks if the symbol is in the prices' data.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to search.
-
-        :return: The validation value.
-        """
-
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.asks
-        )
-    # end in_asks_prices
-
-    def in_prices(self, exchange: str, symbol: str) -> bool:
-        """
-        Checks if the symbol is in the prices' data.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to search.
-
-        :return: The validation value.
-        """
-
-        return (
-            self.in_bids_prices(exchange=exchange, symbol=symbol) and
-            self.in_asks_prices(exchange=exchange, symbol=symbol)
-        )
-    # end in_prices
-# end SymbolsMarketBase
-
 def symbols_market_prices(
         exchange: str,
         symbol: str,
         prices: SymbolsPrices,
         provider: Optional[Any] = None
 ) -> List[Tuple[dt.datetime, float]]:
     """
@@ -488,218 +303,14 @@
         exchange=exchange, symbol=symbol,
         prices=prices, provider=provider
     )
 
     return [(time, float(value)) for time, value in prices[exchange][symbol]]
 # end symbols_market_prices
 
-AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
-AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
-
-@define(repr=False)
-@represent
-class AssetsMarketState(AssetsMarketBase):
-    """
-    A class to represent the current market state.
-
-    This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
-
-    attributes:
-
-    - screeners:
-        The screener objects to collect the prices of the assets.
-
-    - bids:
-        The bids prices of the assets.
-
-    - asks:
-        The asks prices of the assets.
-
-    - bids_volume:
-        The bids volume prices of the assets.
-
-    - asks_volume:
-        The asks volume prices of the assets.
-
-    >>> from crypto_screening.collect.market import AssetsMarketState
-    >>>
-    >>> state = assets_market_state(...)
-    """
-
-    bids: AssetsPrices
-    asks: AssetsPrices
-    bids_volume: AssetsPrices
-    asks_volume: AssetsPrices
-
-    __modifiers__: ClassVar[Modifiers] = Modifiers(
-        **AssetsMarketBase.__modifiers__
-    )
-    __modifiers__.excluded.extend(["bids", "asks", "bids_volume", "asks_volume"])
-
-    def bid(
-            self, exchange: str, symbol: str, separator: Optional[str] = None
-    ) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the bid price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its bid price.
-        :param separator: The separator of the assets.
-
-        :return: The bid price for the symbol.
-        """
-
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.bids,
-            separator=separator, provider=self
-        )
-    # end bid
-
-    def ask(
-            self, exchange: str, symbol: str, separator: Optional[str] = None
-    ) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the ask price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its ask price.
-        :param separator: The separator of the assets.
-
-        :return: The ask price for the symbol.
-        """
-
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.asks,
-            separator=separator, provider=self
-        )
-    # end ask
-
-    def bid_volume(
-            self, exchange: str, symbol: str, separator: Optional[str] = None
-    ) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the bid price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its bid price.
-        :param separator: The separator of the assets.
-
-        :return: The bid price for the symbol.
-        """
-
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.bids_volume,
-            separator=separator, provider=self
-        )
-    # end bid_volume
-
-    def ask_volume(
-            self, exchange: str, symbol: str, separator: Optional[str] = None
-    ) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the ask price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its ask price.
-        :param separator: The separator of the assets.
-
-        :return: The ask price for the symbol.
-        """
-
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.asks_volume,
-            separator=separator, provider=self
-        )
-    # end ask_volume
-
-    def data(self) -> AssetsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        datasets: Dict[str, Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]]] = {}
-
-        for key, data in zip(
-            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
-            (self.bids, self.asks, self.bids_volume, self.asks_volume)
-        ):
-            for exchange, bases in data.items():
-                for base, quotes in bases.items():
-                    for quote, prices in quotes.items():
-                        for i, (time, price) in enumerate(prices):
-                            try:
-                                if isinstance(time, str):
-                                    time = dt.datetime.fromisoformat(time)
-
-                                elif isinstance(time, int):
-                                    time = dt.datetime.fromtimestamp(time)
-
-                            except (Type, ValueError):
-                                pass
-                            # end try
-
-                            (
-                                datasets.
-                                setdefault(exchange, {}).
-                                setdefault(base, {}).
-                                setdefault(quote, {}).
-                                setdefault(time, {})
-                            )[key] = price
-                        # end for
-                # end for
-            # end for
-        # end for
-
-        new_datasets: AssetsMarketData = {}
-
-        for exchange, bases in datasets.items():
-            for base, quotes in bases.items():
-                for quote, prices in quotes.items():
-                    (
-                        new_datasets.
-                        setdefault(exchange, {}).
-                        setdefault(base, {})
-                    )[quote] = sorted(
-                        list(prices.items()), key=lambda pair: pair[0]
-                    )
-                # end for
-            # end for
-        # end for
-
-        return new_datasets
-    # end data
-
-    def datasets(self) -> AssetsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: AssetsMarketDatasets = {}
-
-        for exchange, bases in self.data().items():
-            for base, quotes in bases.items():
-                for quote, rows in quotes.items():
-                    dataset = create_orderbook_dataframe()
-
-                    for time, row in rows:
-                        dataset.loc[time] = row
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        return datasets
-# end assets_market_state_to_datasets
-# end AssetsMarketStates
-
 def assets_market_prices(
         exchange: str,
         symbol: str,
         prices: AssetsPrices,
         separator: Optional[str] = None,
         provider: Optional[Any] = None
 ) -> List[Tuple[dt.datetime, float]]:
@@ -721,87 +332,46 @@
     )
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
     return [(time, float(value)) for time, value in prices[exchange][base][quote]]
 # end assets_market_prices
 
-def assets_market_state(
-        screeners: Optional[Iterable[BaseScreener]] = None,
-        separator: Optional[str] = None,
-        length: Optional[int] = None,
-        adjust: Optional[bool] = True
-) -> AssetsMarketState:
+@define(repr=False)
+@represent
+class MarketBase(metaclass=ABCMeta):
     """
-    Fetches the prices and relations between the assets.
-
-    :param screeners: The price screeners.
-    :param separator: The separator of the assets.
-    :param length: The length of the prices.
-    :param adjust: The value to adjust the length of the sequences.
+    A class to represent the current market state.
 
-    :return: The prices of the assets.
-    """
+    This object contains the state of the market, as Close,
+    bids and asks prices of specific assets, gathered from the network.
 
-    bids: AssetsPrices = {}
-    asks: AssetsPrices = {}
-    bids_volume: AssetsPrices = {}
-    asks_volume: AssetsPrices = {}
+    attributes:
 
-    if (length is None) and (not adjust):
-        length = min([len(screener.market) for screener in screeners])
-    # end if
+    - screeners:
+        The screener objects to collect the prices of the assets.
+    """
 
-    for screener in screeners:
-        if adjust and (length is None):
-            length = len(screener.market)
+    screeners: Iterable[BaseScreener]
 
-        elif adjust:
-            length = min([len(screener.market), length])
-        # end if
+    __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=["screeners"])
 
-        if length > len(screener.market):
-            raise ValueError(
-                f"Data of '{screener.exchange}' "
-                f"symbol in '{screener.symbol}' exchange "
-                f"is not long enough for the requested length: {length}. "
-                f"Consider using the 'adjust' parameter as {True}, "
-                f"to adjust to the actual length of the data."
-            )
-        # end if
+    def __hash__(self) -> int:
+        """
+        Returns the hash of the object.
 
-        base, quote = symbol_to_parts(
-            symbol=screener.symbol, separator=separator
-        )
+        :return: The hash of the object.
+        """
 
-        for key, data in zip(
-            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
-            (bids, asks, bids_volume, asks_volume)
-        ):
-            (
-                data.
-                setdefault(screener.exchange, {}).
-                setdefault(base, {}).
-                setdefault(
-                    quote,
-                    list(
-                        zip(
-                            list(screener.market.index[-length:]),
-                            list(screener.market[key][-length:])
-                        )
-                    )
-                )
-            )
-    # end for
+        return id(self)
+    # end __hash__
+# end OrderbookMarketBase
 
-    return AssetsMarketState(
-        screeners=screeners, bids=bids, asks=asks,
-        bids_volume=bids_volume, asks_volume=asks_volume
-    )
-# end assets_market_state
+AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
+AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
 def dataset_to_data(dataset: pd.DataFrame) -> List[Tuple[dt.datetime, Dict[str, float]]]:
     """
     Converts the dataset into the data of the rows.
@@ -889,389 +459,14 @@
     """
 
     return symbols_datasets_to_symbols_data(
         screeners_to_symbols_datasets(screeners=screeners)
     )
 # end screeners_to_symbols_data
 
-@define(repr=False)
-@represent
-class SymbolsMarketState(SymbolsMarketBase):
-    """
-    A class to represent the current market state.
-
-    This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
-
-    attributes:
-
-    - screeners:
-        The screener objects to collect the prices of the assets.
-
-    - prices:
-        The close price of the assets.
-
-    - bids:
-        The bids prices of the assets.
-
-    - asks:
-        The asks prices of the assets.
-
-    - bids_volume:
-        The bids volume prices of the assets.
-
-    - asks_volume:
-        The asks volume prices of the assets.
-
-    >>> from crypto_screening.collect.market import AssetsMarketState
-    >>>
-    >>> state = assets_market_state(...)
-    """
-
-    bids: SymbolsPrices
-    asks: SymbolsPrices
-    bids_volume: SymbolsPrices
-    asks_volume: SymbolsPrices
-
-    __modifiers__: ClassVar[Modifiers] = Modifiers(
-        **AssetsMarketBase.__modifiers__
-    )
-    __modifiers__.excluded.extend(["bids", "asks", "bids_volume", "asks_volume"])
-
-    def bid(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the bid price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its bid price.
-
-        :return: The bid price for the symbol.
-        """
-
-        return symbols_market_prices(
-            exchange=exchange, symbol=symbol,
-            prices=self.bids, provider=self
-        )
-    # end bid
-
-    def ask(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the ask price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its ask price.
-
-        :return: The ask price for the symbol.
-        """
-
-        return symbols_market_prices(
-            exchange=exchange, symbol=symbol,
-            prices=self.asks, provider=self
-        )
-    # end ask
-
-    def bid_volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the bid price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its bid price.
-
-        :return: The bid price for the symbol.
-        """
-
-        return symbols_market_prices(
-            exchange=exchange, symbol=symbol,
-            prices=self.bids_volume, provider=self
-        )
-    # end bid_volume
-
-    def ask_volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
-        """
-        Returns the ask price for the symbol.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol to find its ask price.
-
-        :return: The ask price for the symbol.
-        """
-
-        return symbols_market_prices(
-            exchange=exchange, symbol=symbol,
-            prices=self.asks_volume, provider=self
-        )
-    # end ask_volume
-
-    def data(self) -> SymbolsMarketData:
-        """
-        Returns the structured data of the state.
-
-        :return: The data of the state.
-        """
-
-        datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]] = {}
-
-        for key, data in zip(
-            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
-            (self.bids, self.asks, self.bids_volume, self.asks_volume)
-        ):
-            for exchange, symbols in data.items():
-                for symbol, prices in symbols.items():
-                    for i, (time, price) in enumerate(prices):
-                        try:
-                            if isinstance(time, str):
-                                time = dt.datetime.fromisoformat(time)
-
-                            elif isinstance(time, int):
-                                time = dt.datetime.fromtimestamp(time)
-
-                        except (Type, ValueError):
-                            pass
-                        # end try
-
-                        (
-                            datasets.
-                            setdefault(exchange, {}).
-                            setdefault(symbol, {}).
-                            setdefault(time, {})
-                        )[key] = price
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        new_datasets: SymbolsMarketData = {}
-
-        for exchange, symbols in datasets.items():
-            for symbol, prices in symbols.copy().items():
-                new_datasets.setdefault(exchange, {})[symbol] = sorted(
-                    list(prices.items()), key=lambda pair: pair[0]
-                )
-            # end for
-        # end for
-
-        return new_datasets
-    # end data
-
-    def datasets(self) -> SymbolsMarketDatasets:
-        """
-        Rebuilds the dataset from the market state.
-
-        :return: The dataset of the state data.
-        """
-
-        datasets: SymbolsMarketDatasets = {}
-
-        for exchange, symbols in self.data().items():
-            for symbol, rows in symbols.items():
-                dataset = create_orderbook_dataframe()
-
-                for time, row in rows:
-                    dataset.loc[time] = row
-                # end for
-            # end for
-        # end for
-
-        return datasets
-# end symbols_market_state_to_datasets
-# end SymbolsMarketStates
-
-def symbols_market_state(
-        screeners: Optional[Iterable[BaseScreener]] = None,
-        length: Optional[int] = None,
-        adjust: Optional[bool] = True
-) -> SymbolsMarketState:
-    """
-    Fetches the prices and relations between the assets.
-
-    :param screeners: The price screeners.
-    :param length: The length of the prices.
-    :param adjust: The value to adjust the length of the sequences.
-
-    :return: The prices of the assets.
-    """
-
-    bids: SymbolsPrices = {}
-    asks: SymbolsPrices = {}
-    bids_volume: SymbolsPrices = {}
-    asks_volume: SymbolsPrices = {}
-
-    if (length is None) and (not adjust):
-        length = min([len(screener.market) for screener in screeners])
-    # end if
-
-    for screener in screeners:
-        if adjust and (length is None):
-            length = len(screener.market)
-
-        elif adjust:
-            length = min([len(screener.market), length])
-        # end if
-
-        if length > len(screener.market):
-            raise ValueError(
-                f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
-                f"is not long enough for the requested length: {length}. "
-                f"Consider using the 'adjust' parameter as {True}, "
-                f"to adjust to the actual length of the data."
-            )
-        # end if
-
-        for key, data in zip(
-            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
-            (bids, asks, bids_volume, asks_volume)
-        ):
-            (
-                data.
-                setdefault(screener.exchange, {}).
-                setdefault(
-                    screener.symbol,
-                    list(
-                        zip(
-                            list(screener.market.index[-length:]),
-                            list(screener.market[key][-length:])
-                        )
-                    )
-                )
-            )
-        # end for
-    # end for
-
-    return SymbolsMarketState(
-        screeners=screeners, bids=bids, asks=asks,
-        bids_volume=bids_volume, asks_volume=asks_volume
-    )
-# end symbols_market_state
-
-def merge_symbols_market_states(
-        *states: SymbolsMarketState, sort: Optional[bool] = True
-) -> SymbolsMarketState:
-    """
-    Concatenates the states of the market.
-
-    :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
-
-    :return: The states object.
-    """
-
-    bids: SymbolsPrices = {}
-    asks: SymbolsPrices = {}
-    bids_volume: SymbolsPrices = {}
-    asks_volume: SymbolsPrices = {}
-
-    for state in states:
-        for key, (state_data, data) in zip(
-            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
-            (
-                (state.bids, bids),
-                (state.asks, asks),
-                (state.bids_volume, bids_volume),
-                (state.asks_volume, asks_volume)
-            )
-        ):
-            for exchange, symbols in state_data.items():
-                for symbol, prices in symbols.items():
-                    (
-                        data.setdefault(exchange, {}).
-                        setdefault(symbol, []).
-                        extend(prices)
-                    )
-                # end for
-            # end for
-        # end for
-    # end for
-
-    screeners = []
-
-    if sort:
-        for prices_data in (bids, asks, bids_volume, asks_volume):
-            for exchange, symbols in prices_data.items():
-                for symbol, prices in symbols.items():
-                    prices.sort(key=lambda pair: pair[0])
-                # end for
-            # end for
-        # end for
-    # end if
-
-    for state in states:
-        screeners.extend(state.screeners)
-    # end for
-
-    return SymbolsMarketState(
-        screeners=set(screeners), bids=bids, asks=asks,
-        bids_volume=bids_volume, asks_volume=asks_volume
-    )
-# end merge_symbols_market_states
-
-def merge_assets_market_states(
-        *states: AssetsMarketState, sort: Optional[bool] = True
-) -> AssetsMarketState:
-    """
-    Concatenates the states of the market.
-
-    :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
-
-    :return: The states object.
-    """
-
-    bids: AssetsPrices = {}
-    asks: AssetsPrices = {}
-    bids_volume: AssetsPrices = {}
-    asks_volume: AssetsPrices = {}
-
-    for state in states:
-        for key, (state_data, data) in zip(
-            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
-            (
-                (state.bids, bids),
-                (state.asks, asks),
-                (state.bids_volume, bids_volume),
-                (state.asks_volume, asks_volume)
-            )
-        ):
-            for exchange, symbols in state_data.items():
-                for base, quotes in symbols.items():
-                    for quote, prices in quotes.items():
-                        (
-                            data.setdefault(exchange, {}).
-                            setdefault(base, {}).
-                            setdefault(quote, []).
-                            extend(prices)
-                        )
-                # end for
-            # end for
-        # end for
-    # end for
-
-    if sort:
-        for prices_data in (bids, asks, bids_volume, asks_volume):
-            for exchange, bases in prices_data.items():
-                for base, quotes in bases.items():
-                    for quote, prices in quotes.items():
-                        prices.sort(key=lambda pair: pair[0])
-                    # end for
-                # end for
-            # end for
-        # end for
-    # end if
-
-    screeners = []
-
-    for state in states:
-        screeners.extend(state.screeners)
-    # end for
-
-    return AssetsMarketState(
-        screeners=set(screeners), bids=bids, asks=asks,
-        bids_volume=bids_volume, asks_volume=asks_volume
-    )
-# end merge_assets_market_states
-
 def merge_symbols_market_data(
         *data: SymbolsMarketData, sort: Optional[bool] = True
 ) -> SymbolsMarketData:
     """
     Concatenates the states of the market.
 
     :param data: The states to concatenate.
@@ -1299,15 +494,15 @@
             for symbol, prices in symbols.items():
                 prices.sort(key=lambda pair: pair[0])
             # end for
         # end for
     # end if
 
     return new_data
-# end merge_symbols_market_states
+# end merge_symbols_ohlcv_market_states
 
 def merge_assets_market_data(
         *data: AssetsMarketData, sort: Optional[bool] = True
 ) -> AssetsMarketData:
     """
     Concatenates the states of the market.
 
@@ -1340,17 +535,17 @@
                     prices.sort(key=lambda pair: pair[0])
                 # end for
             # end for
         # end for
     # end if
 
     return new_data
-# end merge_assets_market_states
+# end merge_assets_ohlcv_market_states
 
-def symbols_market_dataset_to_assets_market_datasets(
+def symbols_to_assets_market_datasets(
         datasets: SymbolsMarketDatasets, separator: Optional[str] = None
 ) -> AssetsMarketDatasets:
     """
     Converts the datasets structure from symbols to assets.
 
     :param datasets: The datasets to convert.
     :param separator: The separator for the symbols.
@@ -1369,15 +564,15 @@
                 setdefault(base, {}).
                 setdefault(quote, dataset)
             )
         # end for
     # end for
 
     return assets_datasets
-# end symbols_market_dataset_to_assets_market_datasets
+# end symbols_to_assets_market_datasets
 
 def assets_market_dataset_to_symbols_market_datasets(
         datasets: AssetsMarketDatasets, separator: Optional[str] = None
 ) -> SymbolsMarketDatasets:
     """
     Converts the datasets structure from assets to symbols.
 
@@ -1400,15 +595,15 @@
                 )
         # end for
     # end for
 
     return symbols_datasets
 # end assets_market_dataset_to_symbols_market_datasets
 
-def assets_market_prices_to_symbol_market_prices(
+def assets_to_symbol_market_prices(
         prices: AssetsPrices, separator: Optional[str] = None
 ) -> SymbolsPrices:
     """
     Converts an assets market prices into a symbols market prices.
 
     :param prices: The source prices.
     :param separator: The separator for the symbols.
@@ -1431,46 +626,17 @@
                     ).append((time, price))
                 # end for
             # end for
         # end for
     # end for
 
     return symbols_prices
-# end assets_market_prices_to_symbol_market_prices
+# end assets_to_symbol_market_prices
 
-def assets_market_state_to_symbols_market_state(
-        state: AssetsMarketState,
-        separator: Optional[str] = None
-) -> SymbolsMarketState:
-    """
-    Converts an assets market state into a symbols market state.
-
-    :param state: The source state.
-    :param separator: The separator for the symbols.
-
-    :return: The results state.
-    """
-
-    return SymbolsMarketState(
-        bids=assets_market_prices_to_symbol_market_prices(
-            state.bids, separator=separator
-        ),
-        asks=assets_market_prices_to_symbol_market_prices(
-            state.asks, separator=separator
-        ),
-        bids_volume=assets_market_prices_to_symbol_market_prices(
-            state.bids_volume, separator=separator
-        ),
-        asks_volume=assets_market_prices_to_symbol_market_prices(
-            state.asks_volume, separator=separator
-        )
-    )
-# end assets_market_state_to_symbols_market_state
-
-def symbol_market_prices_to_assets_market_prices(
+def symbol_to_assets_market_prices(
         prices: SymbolsPrices, separator: Optional[str] = None
 ) -> AssetsPrices:
     """
     Converts a symbols market prices into an assets market prices.
 
     :param prices: The source prices.
     :param separator: The separator for the symbols.
@@ -1492,46 +658,17 @@
                     setdefault(quote, [])
                 ).append((time, price))
             # end for
         # end for
     # end for
 
     return assets_prices
-# end symbol_market_prices_to_assets_market_prices
-
-def symbols_market_state_to_assets_market_state(
-        state: SymbolsMarketState,
-        separator: Optional[str] = None
-) -> AssetsMarketState:
-    """
-    Converts a symbols market state into an assets market state.
+# end symbol_to_assets_market_prices
 
-    :param state: The source state.
-    :param separator: The separator for the symbols.
-
-    :return: The results state.
-    """
-
-    return AssetsMarketState(
-        bids=symbol_market_prices_to_assets_market_prices(
-            state.bids, separator=separator
-        ),
-        asks=symbol_market_prices_to_assets_market_prices(
-            state.asks, separator=separator
-        ),
-        bids_volume=symbol_market_prices_to_assets_market_prices(
-            state.bids_volume, separator=separator
-        ),
-        asks_volume=symbol_market_prices_to_assets_market_prices(
-            state.asks_volume, separator=separator
-        )
-    )
-# end symbols_market_state_to_assets_market_state
-
-def assets_market_data_to_symbols_market_data(
+def assets_to_symbols_market_data(
         data: AssetsMarketData,
         separator: Optional[str] = None
 ) -> SymbolsMarketData:
     """
     Converts the structure of the market data from assets to symbols.
 
     :param data: The data to convert.
@@ -1552,17 +689,17 @@
                     setdefault(exchange, {}).
                     setdefault(symbol, data)
                 )
             # end for
     # end for
 
     return symbols_data
-# end assets_market_data_to_symbols_market_data
+# end assets_to_symbols_market_data
 
-def symbols_market_data_to_assets_market_data(
+def symbols_to_assets_market_data(
         data: SymbolsMarketData,
         separator: Optional[str] = None
 ) -> AssetsMarketData:
     """
     Converts the structure of the market data from assets to symbols.
 
     :param data: The data to convert.
@@ -1584,15 +721,15 @@
                 setdefault(quote, data)
             )
             # end for
         # end for
     # end for
 
     return assets_data
-# end assets_market_data_to_symbols_market_data
+# end assets_to_symbols_market_data
 
 _ST = TypeVar("_ST", Type[BaseScreener], Type[OrderbookScreener])
 
 AssetsScreeners = Dict[str, Dict[str, Dict[str, Union[BaseScreener, _ST]]]]
 
 def assets_market_datasets_to_assets_screeners(
         datasets: AssetsMarketDatasets,
@@ -1789,11 +926,349 @@
     :param screeners: The screeners to update.
     :param data: The new data to add to the screeners.
     :param adjust: The value to adjust with screeners that are not found.
     """
 
     return add_symbols_data_to_screeners(
         screeners=screeners,
-        data=assets_market_data_to_symbols_market_data(data=data),
+        data=assets_to_symbols_market_data(data=data),
         adjust=adjust
     )
-# end add_assets_data_to_screeners
+# end add_assets_data_to_screeners
+
+def assets_market_data(
+        columns: Dict[str, str],
+        prices: Optional[Dict[str, AssetsPrices]] = None
+) -> AssetsMarketData:
+    """
+    Returns the structured data of the state.
+
+    :param prices: The prices for the data collection.
+    :param columns: The columns for the data.
+
+    :return: The data of the state.
+    """
+
+    prices = prices or {name: {} for name in columns}
+
+    datasets: Dict[str, Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]]] = {}
+
+    for name in columns:
+        for exchange, bases in prices[name].items():
+            for base, quotes in bases.items():
+                for quote, prices in quotes.items():
+                    for i, (time, price) in enumerate(prices):
+                        try:
+                            if isinstance(time, str):
+                                time = dt.datetime.fromisoformat(time)
+
+                            elif isinstance(time, int):
+                                time = dt.datetime.fromtimestamp(time)
+                            # end if
+
+                        except (Type, ValueError):
+                            pass
+                        # end try
+
+                        (
+                            datasets.
+                            setdefault(exchange, {}).
+                            setdefault(base, {}).
+                            setdefault(quote, {}).
+                            setdefault(time, {})
+                        )[columns[name]] = price
+                    # end for
+            # end for
+        # end for
+    # end for
+
+    new_datasets: AssetsMarketData = {}
+
+    for exchange, bases in datasets.items():
+        for base, quotes in bases.items():
+            for quote, prices in quotes.items():
+                (
+                    new_datasets.
+                    setdefault(exchange, {}).
+                    setdefault(base, {})
+                )[quote] = sorted(
+                    list(prices.items()), key=lambda pair: pair[0]
+                )
+            # end for
+        # end for
+    # end for
+
+    return new_datasets
+# end assets_market_data
+
+def symbols_market_data(
+        columns: Dict[str, str],
+        prices: Optional[Dict[str, SymbolsPrices]] = None
+) -> SymbolsMarketData:
+    """
+    Returns the structured data of the state.
+
+    :param prices: The prices for the data collection.
+    :param columns: The columns for the data.
+
+    :return: The data of the state.
+    """
+
+    datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]] = {}
+
+    for name in columns:
+        for exchange, symbols in prices[name].items():
+            for symbol, prices in symbols.items():
+                for i, (time, price) in enumerate(prices):
+                    try:
+                        if isinstance(time, str):
+                            time = dt.datetime.fromisoformat(time)
+
+                        elif isinstance(time, int):
+                            time = dt.datetime.fromtimestamp(time)
+
+                    except (Type, ValueError):
+                        pass
+                    # end try
+
+                    (
+                        datasets.
+                        setdefault(exchange, {}).
+                        setdefault(symbol, {}).
+                        setdefault(time, {})
+                    )[columns[name]] = price
+                # end for
+            # end for
+        # end for
+    # end for
+
+    new_datasets: SymbolsMarketData = {}
+
+    for exchange, symbols in datasets.items():
+        for symbol, prices in symbols.copy().items():
+            new_datasets.setdefault(exchange, {})[symbol] = sorted(
+                list(prices.items()), key=lambda pair: pair[0]
+            )
+        # end for
+    # end for
+
+    return new_datasets
+# end symbols_market_data
+
+def assets_market_state(
+        columns: Dict[str, str],
+        prices: Optional[Dict[str, AssetsPrices]] = None,
+        screeners: Optional[Iterable[BaseScreener]] = None,
+        separator: Optional[str] = None,
+        length: Optional[int] = None,
+        adjust: Optional[bool] = True
+) -> Dict[str, AssetsPrices]:
+    """
+    Fetches the prices and relations between the assets.
+
+    :param prices: The prices for the data collection.
+    :param columns: The columns for the data.
+    :param screeners: The price screeners.
+    :param separator: The separator of the assets.
+    :param length: The length of the prices.
+    :param adjust: The value to adjust the length of the sequences.
+
+    :return: The prices of the assets.
+    """
+
+    prices = prices or {name: {} for name in columns}
+
+    if (length is None) and (not adjust):
+        length = min([len(screener.market) for screener in screeners])
+    # end if
+
+    for screener in screeners:
+        if adjust and (length is None):
+            length = len(screener.market)
+
+        elif adjust:
+            length = min([len(screener.market), length])
+        # end if
+
+        if length > len(screener.market):
+            raise ValueError(
+                f"Data of '{screener.exchange}' "
+                f"symbol in '{screener.symbol}' exchange "
+                f"is not long enough for the requested length: {length}. "
+                f"Consider using the 'adjust' parameter as {True}, "
+                f"to adjust to the actual length of the data."
+            )
+        # end if
+
+        base, quote = symbol_to_parts(
+            symbol=screener.symbol, separator=separator
+        )
+
+        for name in zip(columns, prices):
+            (
+                prices[name].
+                setdefault(screener.exchange, {}).
+                setdefault(base, {}).
+                setdefault(
+                    quote,
+                    list(
+                        zip(
+                            list(screener.market.index[-length:]),
+                            list(screener.market[columns[name]][-length:])
+                        )
+                    )
+                )
+            )
+    # end for
+
+    return prices
+# end assets_market_state
+
+def symbols_market_state(
+        columns: Dict[str, str],
+        prices: Optional[Dict[str, SymbolsPrices]] = None,
+        screeners: Optional[Iterable[BaseScreener]] = None,
+        length: Optional[int] = None,
+        adjust: Optional[bool] = True
+) -> Dict[str, SymbolsPrices]:
+    """
+    Fetches the prices and relations between the assets.
+
+    :param prices: The prices for the data collection.
+    :param columns: The columns for the data.
+    :param screeners: The price screeners.
+    :param length: The length of the prices.
+    :param adjust: The value to adjust the length of the sequences.
+
+    :return: The prices of the assets.
+    """
+
+    prices = prices or {name: {} for name in columns}
+
+    if (length is None) and (not adjust):
+        length = min([len(screener.market) for screener in screeners])
+    # end if
+
+    for screener in screeners:
+        if adjust and (length is None):
+            length = len(screener.market)
+
+        elif adjust:
+            length = min([len(screener.market), length])
+        # end if
+
+        if length > len(screener.market):
+            raise ValueError(
+                f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
+                f"is not long enough for the requested length: {length}. "
+                f"Consider using the 'adjust' parameter as {True}, "
+                f"to adjust to the actual length of the data."
+            )
+        # end if
+
+        for name in zip(columns, prices):
+            (
+                prices[name].
+                setdefault(screener.exchange, {}).
+                setdefault(
+                    screener.symbol,
+                    list(
+                        zip(
+                            list(screener.market.index[-length:]),
+                            list(screener.market[columns[name]][-length:])
+                        )
+                    )
+                )
+            )
+        # end for
+    # end for
+
+    return prices
+# end symbols_market_state
+
+def merge_assets_market_states(
+        *states: MarketBase,
+        prices: Dict[str, AssetsPrices],
+        sort: Optional[bool] = True
+) -> Dict[str, AssetsPrices]:
+    """
+    Concatenates the states of the market.
+
+    :param prices: The prices for the data collection.
+    :param states: The states to concatenate.
+    :param sort: The value to sort the prices by the time.
+
+    :return: The states object.
+    """
+
+    for state in states:
+        for name in prices:
+            for exchange, bases in getattr(state, name).items():
+                for base, quotes in bases.items():
+                    for quote, quote_prices in quotes.items():
+                        (
+                            prices[name].setdefault(exchange, {}).
+                            setdefault(base, {}).
+                            setdefault(quote, []).
+                            extend(quote_prices)
+                        )
+                # end for
+            # end for
+        # end for
+    # end for
+
+    if sort:
+        for prices_data in prices.values():
+            for exchange, bases in prices_data.items():
+                for base, quotes in bases.items():
+                    for quote_prices in quotes.values():
+                        quote_prices.sort(key=lambda pair: pair[0])
+                    # end for
+                # end for
+            # end for
+        # end for
+    # end if
+
+    return prices
+# end merge_assets_market_states
+
+def merge_symbols_market_states(
+        *states: MarketBase,
+        prices: Dict[str, SymbolsPrices],
+        sort: Optional[bool] = True
+) -> Dict[str, SymbolsPrices]:
+    """
+    Concatenates the states of the market.
+
+    :param prices: The prices for the data collection.
+    :param states: The states to concatenate.
+    :param sort: The value to sort the prices by the time.
+
+    :return: The states object.
+    """
+
+    for state in states:
+        for name in prices:
+            for exchange, symbols in getattr(state, name).items():
+                for symbol, symbol_prices in symbols.items():
+                    (
+                        prices[name].setdefault(exchange, {}).
+                        setdefault(symbol, []).
+                        extend(symbol_prices)
+                    )
+                # end for
+            # end for
+        # end for
+    # end for
+
+    if sort:
+        for prices_data in prices.values():
+            for exchange, symbols in prices_data.items():
+                for symbol_prices in symbols.values():
+                    symbol_prices.sort(key=lambda pair: pair[0])
+                # end for
+            # end for
+        # end for
+    # end if
+
+    return prices
+# end merge_symbols_market_states
```

### Comparing `crypto-screening-2.7.1/crypto_screening/collect/screeners.py` & `crypto-screening-2.8.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/collect/symbols.py` & `crypto-screening-2.8.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/dataset.py` & `crypto-screening-2.8.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/interval.py` & `crypto-screening-2.8.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/foundation/data.py` & `crypto-screening-2.8.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.8.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/foundation/state.py` & `crypto-screening-2.8.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.8.0/crypto_screening/market/foundation/waiting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # waiting.py
 
 import datetime as dt
 import time
 from typing import (
-    Optional, Union, Iterable, Callable
+    Optional, Union, Iterable, Callable, Any
 )
 
 from crypto_screening.market.foundation.state import WaitingState
 from crypto_screening.market.foundation.data import DataCollector
-from crypto_screening.market.foundation.protocols import (
-    BaseScreenerProtocol
-)
+
 __all__ = [
     "base_wait_for_update",
     "base_wait_for_initialization",
     "base_wait_for_dynamic_update",
     "base_wait_for_dynamic_initialization"
 ]
 
-Gatherer = Callable[[Iterable[DataCollector]], Iterable[BaseScreenerProtocol]]
+Gatherer = Callable[[Iterable[Any]], Iterable[Any]]
 
 def base_wait_for_dynamic_initialization(
         screeners: Iterable[DataCollector],
         stop: Optional[bool] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
         gatherer: Optional[Gatherer] = None
```

### Comparing `crypto-screening-2.7.1/crypto_screening/market/screeners/base.py` & `crypto-screening-2.8.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/screeners/container.py` & `crypto-screening-2.8.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.8.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.8.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.8.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/market/waiting.py` & `crypto-screening-2.8.0/crypto_screening/market/waiting.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import datetime as dt
 from typing import (
     Optional, Union, Iterable
 )
 
 from crypto_screening.collect.screeners import gather_screeners
 from crypto_screening.market.screeners import BaseScreener, BaseMultiScreener
+from crypto_screening.market.foundation.state import WaitingState
 from crypto_screening.market.foundation.waiting import (
     base_wait_for_update, base_wait_for_dynamic_initialization,
-    base_wait_for_initialization, base_wait_for_dynamic_update,
-    WaitingState
+    base_wait_for_initialization, base_wait_for_dynamic_update
 )
 
 __all__ = [
     "wait_for_dynamic_initialization",
     "wait_for_update",
     "wait_for_initialization",
     "wait_for_dynamic_update",
```

### Comparing `crypto-screening-2.7.1/crypto_screening/process.py` & `crypto-screening-2.8.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/symbols.py` & `crypto-screening-2.8.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening/validate.py` & `crypto-screening-2.8.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.8.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.7.1
+Version: 2.8.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.7.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.8.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 crypto_screening.egg-info/SOURCES.txt
 crypto_screening.egg-info/dependency_links.txt
 crypto_screening.egg-info/requires.txt
 crypto_screening.egg-info/top_level.txt
 crypto_screening/collect/assets.py
 crypto_screening/collect/exchanges.py
 crypto_screening/collect/market.py
+crypto_screening/collect/ohlcv.py
+crypto_screening/collect/orderbook.py
 crypto_screening/collect/screeners.py
 crypto_screening/collect/symbols.py
 crypto_screening/market/dynamic.py
 crypto_screening/market/waiting.py
 crypto_screening/market/foundation/data.py
 crypto_screening/market/foundation/protocols.py
 crypto_screening/market/foundation/state.py
```

### Comparing `crypto-screening-2.7.1/pyproject.toml` & `crypto-screening-2.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.7.1'
+version = '2.8.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.7.1/setup.py` & `crypto-screening-2.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.7.1',
+        version='2.8.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```


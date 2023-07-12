# Comparing `tmp/crypto-screening-2.8.1.tar.gz` & `tmp/crypto-screening-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.8.1.tar", last modified: Wed Jul 12 23:01:52 2023, max compression
+gzip compressed data, was "crypto-screening-2.8.2.tar", last modified: Wed Jul 12 23:08:04 2023, max compression
```

## Comparing `crypto-screening-2.8.1.tar` & `crypto-screening-2.8.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.832545 crypto-screening-2.8.1/
--rw-rw-rw-   0        0        0       98 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-12 23:01:52.832545 crypto-screening-2.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.803423 crypto-screening-2.8.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.822529 crypto-screening-2.8.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.1/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    39202 2023-07-12 23:01:36.000000 crypto-screening-2.8.1/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21241 2023-07-12 22:49:02.000000 crypto-screening-2.8.1/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19325 2023-07-12 22:49:02.000000 crypto-screening-2.8.1/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.824529 crypto-screening-2.8.1/crypto_screening/market/
--rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.1/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.827037 crypto-screening-2.8.1/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.831597 crypto-screening-2.8.1/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.1/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.1/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.1/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.817502 crypto-screening-2.8.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 23:01:52.832545 crypto-screening-2.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-12 23:01:43.000000 crypto-screening-2.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:08:04.124922 crypto-screening-2.8.2/
+-rw-rw-rw-   0        0        0       98 2023-07-12 23:08:03.000000 crypto-screening-2.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-12 23:08:04.124922 crypto-screening-2.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.2/build.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:08:04.098769 crypto-screening-2.8.2/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-12 23:08:04.116145 crypto-screening-2.8.2/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.2/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.2/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    39266 2023-07-12 23:07:59.000000 crypto-screening-2.8.2/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21241 2023-07-12 22:49:02.000000 crypto-screening-2.8.2/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19325 2023-07-12 22:49:02.000000 crypto-screening-2.8.2/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.2/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.2/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.2/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:08:04.117145 crypto-screening-2.8.2/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.2/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:08:04.119169 crypto-screening-2.8.2/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.2/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.2/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.2/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.2/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:08:04.123913 crypto-screening-2.8.2/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.2/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.2/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.2/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.8.2/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.2/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.2/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.2/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.2/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.2/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.2/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:08:04.111240 crypto-screening-2.8.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-12 23:08:04.000000 crypto-screening-2.8.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-12 23:08:04.000000 crypto-screening-2.8.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:08:04.000000 crypto-screening-2.8.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-12 23:08:04.000000 crypto-screening-2.8.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-12 23:08:04.000000 crypto-screening-2.8.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-12 23:08:03.000000 crypto-screening-2.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 23:08:04.125922 crypto-screening-2.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-12 23:07:59.000000 crypto-screening-2.8.2/setup.py
```

### Comparing `crypto-screening-2.8.1/PKG-INFO` & `crypto-screening-2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.1
+Version: 2.8.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.1/README.md` & `crypto-screening-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/build.py` & `crypto-screening-2.8.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/collect/assets.py` & `crypto-screening-2.8.2/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/collect/exchanges.py` & `crypto-screening-2.8.2/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/collect/market.py` & `crypto-screening-2.8.2/crypto_screening/collect/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -951,16 +951,16 @@
     prices = prices or {name: {} for name in columns}
 
     datasets: Dict[str, Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]]] = {}
 
     for name in columns:
         for exchange, bases in prices[name].items():
             for base, quotes in bases.items():
-                for quote, prices in quotes.items():
-                    for i, (time, price) in enumerate(prices):
+                for quote, symbols_prices in quotes.items():
+                    for i, (time, price) in enumerate(symbols_prices):
                         try:
                             if isinstance(time, str):
                                 time = dt.datetime.fromisoformat(time)
 
                             elif isinstance(time, int):
                                 time = dt.datetime.fromtimestamp(time)
                             # end if
@@ -981,21 +981,21 @@
         # end for
     # end for
 
     new_datasets: AssetsMarketData = {}
 
     for exchange, bases in datasets.items():
         for base, quotes in bases.items():
-            for quote, prices in quotes.items():
+            for quote, symbols_prices in quotes.items():
                 (
                     new_datasets.
                     setdefault(exchange, {}).
                     setdefault(base, {})
                 )[quote] = sorted(
-                    list(prices.items()), key=lambda pair: pair[0]
+                    list(symbols_prices.items()), key=lambda pair: pair[0]
                 )
             # end for
         # end for
     # end for
 
     return new_datasets
 # end assets_market_data
@@ -1013,16 +1013,16 @@
     :return: The data of the state.
     """
 
     datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]] = {}
 
     for name in columns:
         for exchange, symbols in prices[name].items():
-            for symbol, prices in symbols.items():
-                for i, (time, price) in enumerate(prices):
+            for symbol, symbols_prices in symbols.items():
+                for i, (time, price) in enumerate(symbols_prices):
                     try:
                         if isinstance(time, str):
                             time = dt.datetime.fromisoformat(time)
 
                         elif isinstance(time, int):
                             time = dt.datetime.fromtimestamp(time)
 
@@ -1040,17 +1040,17 @@
             # end for
         # end for
     # end for
 
     new_datasets: SymbolsMarketData = {}
 
     for exchange, symbols in datasets.items():
-        for symbol, prices in symbols.copy().items():
+        for symbol, symbols_prices in symbols.copy().items():
             new_datasets.setdefault(exchange, {})[symbol] = sorted(
-                list(prices.items()), key=lambda pair: pair[0]
+                list(symbols_prices.items()), key=lambda pair: pair[0]
             )
         # end for
     # end for
 
     return new_datasets
 # end symbols_market_data
```

### Comparing `crypto-screening-2.8.1/crypto_screening/collect/ohlcv.py` & `crypto-screening-2.8.2/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/collect/orderbook.py` & `crypto-screening-2.8.2/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/collect/screeners.py` & `crypto-screening-2.8.2/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/collect/symbols.py` & `crypto-screening-2.8.2/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/dataset.py` & `crypto-screening-2.8.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/interval.py` & `crypto-screening-2.8.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/dynamic.py` & `crypto-screening-2.8.2/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/foundation/data.py` & `crypto-screening-2.8.2/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.8.2/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/foundation/state.py` & `crypto-screening-2.8.2/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.8.2/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/screeners/base.py` & `crypto-screening-2.8.2/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/screeners/container.py` & `crypto-screening-2.8.2/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.8.2/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.8.2/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.8.2/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/market/waiting.py` & `crypto-screening-2.8.2/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/process.py` & `crypto-screening-2.8.2/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/symbols.py` & `crypto-screening-2.8.2/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening/validate.py` & `crypto-screening-2.8.2/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.8.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.1
+Version: 2.8.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.8.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.1/pyproject.toml` & `crypto-screening-2.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.8.1'
+version = '2.8.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.8.1/setup.py` & `crypto-screening-2.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.8.1',
+        version='2.8.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```


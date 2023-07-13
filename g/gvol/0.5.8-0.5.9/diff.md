# Comparing `tmp/gvol-0.5.8.tar.gz` & `tmp/gvol-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvol-0.5.8.tar", max compression
+gzip compressed data, was "gvol-0.5.9.tar", max compression
```

## Comparing `gvol-0.5.8.tar` & `gvol-0.5.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1132 2023-07-12 07:52:55.074125 gvol-0.5.8/README.md
--rw-r--r--   0        0        0       86 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/__init__.py
--rw-r--r--   0        0        0    55510 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/client.py
--rw-r--r--   0        0        0    36960 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/queries.py
--rw-r--r--   0        0        0     1766 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/types.py
--rw-r--r--   0        0        0     1411 2023-07-12 07:52:55.078125 gvol-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gvol-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-07-13 09:24:07.767249 gvol-0.5.9/README.md
+-rw-r--r--   0        0        0       86 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/__init__.py
+-rw-r--r--   0        0        0    55510 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/client.py
+-rw-r--r--   0        0        0    36973 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/queries.py
+-rw-r--r--   0        0        0     1766 2023-07-13 09:24:07.767249 gvol-0.5.9/gvol/types.py
+-rw-r--r--   0        0        0     1411 2023-07-13 09:24:07.767249 gvol-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gvol-0.5.9/PKG-INFO
```

### Comparing `gvol-0.5.8/README.md` & `gvol-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `gvol-0.5.8/gvol/client.py` & `gvol-0.5.9/gvol/client.py`

 * *Files identical despite different names*

### Comparing `gvol-0.5.8/gvol/queries.py` & `gvol-0.5.9/gvol/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1384,17 +1384,17 @@
 options_cumulative_net_volumes = """
 query NetVolumeGvolDirection($tradeType: TradeTypeEnum, $days: Float, $symbol: SymbolEnumType, $exchange: ExchangeEnumType, $showActiveExpirations: Boolean)
  {genericNetVolumeGvolDirection(symbol: $symbol, tradeType: $tradeType, days: $days, exchange: $exchange, showActiveExpirations: $showActiveExpirations) 
  {date strike cumulative indexPrice}}
 """
 
 options_cumulative_net_volumes_hist = """
-query HistoricalNetVolumeApi($symbol: SymbolEnumType, $dateStart: String, $dateEnd: String $exchange: ExchangeEnumType, $trade: TradeEnumType, $showActiveExpirations: Boolean)
-{HistoricalNetVolumeApi(symbol: $symbol, dateStart: $dateStart, dateEnd: $dateEnd exchange: $exchange, trade: $trade, showActiveExpirations: $showActiveExpirations) 
-{date strike cumulative cumulativeGamma cumulativeVega cumulativeDelta indexPrice} }
+query HistoricalNetVolumeApi($symbol: SymbolEnumType, $dateStart: String, $dateEnd: String $exchange: ExchangeEnumType, $tradeType: TradeEnumType, $showActiveExpirations: Boolean)
+{ HistoricalNetVolumeApi(symbol: $symbol, dateStart: $dateStart, dateEnd: $dateEnd exchange: $exchange, tradeType: $tradeType, showActiveExpirations: $showActiveExpirations)
+{date strike cumulative cumulativeGamma cumulativeVega cumulativeDelta indexPrice } }
 """
 
 options_cumulative_net_positioning = """
 query NetPositioning( $symbol: SymbolEnumType, $exchange: ExchangeEnumType, $dateStart: String) 
 {genericNetPositioningGvolDirection(symbol: $symbol, exchange: $exchange, dateStart: $dateStart) 
 { date
    strike
```

### Comparing `gvol-0.5.8/gvol/types.py` & `gvol-0.5.9/gvol/types.py`

 * *Files identical despite different names*

### Comparing `gvol-0.5.8/pyproject.toml` & `gvol-0.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gvol"
-version = "0.5.8"
+version = "0.5.9"
 description = "GVol is a Python library to access the GVol API"
 authors = ["Denys Halenok <denys.halenok@gmail.com>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/genesis-volatility/gvol-py"
 repository = "https://github.com/genesis-volatility/gvol-py"
```

### Comparing `gvol-0.5.8/PKG-INFO` & `gvol-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvol
-Version: 0.5.8
+Version: 0.5.9
 Summary: GVol is a Python library to access the GVol API
 Home-page: https://github.com/genesis-volatility/gvol-py
 Author: Denys Halenok
 Author-email: denys.halenok@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```


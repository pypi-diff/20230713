# Comparing `tmp/PyQuantKit-0.2.0a0.tar.gz` & `tmp/PyQuantKit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQuantKit-0.2.0a0.tar", last modified: Mon Jan 30 10:01:33 2023, max compression
+gzip compressed data, was "PyQuantKit-0.2.1.tar", last modified: Thu Jul 13 08:03:30 2023, max compression
```

## Comparing `PyQuantKit-0.2.0a0.tar` & `PyQuantKit-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-01-30 10:01:33.507729 PyQuantKit-0.2.0a0/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-01-25 08:58:13.000000 PyQuantKit-0.2.0a0/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      588 2023-01-30 10:01:33.492544 PyQuantKit-0.2.0a0/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-01-30 10:01:32.938308 PyQuantKit-0.2.0a0/PyQuantKit/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    35885 2023-01-25 08:58:13.000000 PyQuantKit-0.2.0a0/PyQuantKit/ConsoleUtils.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    68097 2023-01-25 08:58:13.000000 PyQuantKit-0.2.0a0/PyQuantKit/MarketUtils.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    16240 2023-01-25 08:58:13.000000 PyQuantKit-0.2.0a0/PyQuantKit/TechnicalAnalysis.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    19504 2023-01-25 08:58:13.000000 PyQuantKit-0.2.0a0/PyQuantKit/TradeUtils.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7923 2023-01-30 09:56:07.000000 PyQuantKit-0.2.0a0/PyQuantKit/_FinanceDecimal.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2937 2023-01-30 09:57:41.000000 PyQuantKit-0.2.0a0/PyQuantKit/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-01-30 10:01:33.407695 PyQuantKit-0.2.0a0/PyQuantKit.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      588 2023-01-30 10:01:31.000000 PyQuantKit-0.2.0a0/PyQuantKit.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      358 2023-01-30 10:01:32.000000 PyQuantKit-0.2.0a0/PyQuantKit.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-01-30 10:01:31.000000 PyQuantKit-0.2.0a0/PyQuantKit.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2023-01-30 10:01:31.000000 PyQuantKit-0.2.0a0/PyQuantKit.egg-info/requires.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-01-30 10:01:31.000000 PyQuantKit-0.2.0a0/PyQuantKit.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       53 2023-01-25 08:58:13.000000 PyQuantKit-0.2.0a0/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-01-30 10:01:33.511224 PyQuantKit-0.2.0a0/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1491 2023-01-25 08:58:13.000000 PyQuantKit-0.2.0a0/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:03:30.224429 PyQuantKit-0.2.1/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-07-13 06:36:49.000000 PyQuantKit-0.2.1/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      561 2023-07-13 08:03:30.217441 PyQuantKit-0.2.1/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:03:29.932804 PyQuantKit-0.2.1/PyQuantKit/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    35885 2023-07-13 06:36:49.000000 PyQuantKit-0.2.1/PyQuantKit/ConsoleUtils.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    68097 2023-07-13 06:36:49.000000 PyQuantKit-0.2.1/PyQuantKit/MarketUtils.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    16240 2023-07-13 06:36:49.000000 PyQuantKit-0.2.1/PyQuantKit/TechnicalAnalysis.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    19551 2023-07-13 06:44:45.000000 PyQuantKit-0.2.1/PyQuantKit/TradeUtils.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7923 2023-07-13 06:36:49.000000 PyQuantKit-0.2.1/PyQuantKit/_FinanceDecimal.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2935 2023-07-13 07:21:59.000000 PyQuantKit-0.2.1/PyQuantKit/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:03:30.159310 PyQuantKit-0.2.1/PyQuantKit.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      561 2023-07-13 08:03:25.000000 PyQuantKit-0.2.1/PyQuantKit.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      358 2023-07-13 08:03:27.000000 PyQuantKit-0.2.1/PyQuantKit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-07-13 08:03:25.000000 PyQuantKit-0.2.1/PyQuantKit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2023-07-13 08:03:25.000000 PyQuantKit-0.2.1/PyQuantKit.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-07-13 08:03:25.000000 PyQuantKit-0.2.1/PyQuantKit.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       53 2023-07-13 06:36:49.000000 PyQuantKit-0.2.1/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-07-13 08:03:30.227391 PyQuantKit-0.2.1/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1491 2023-07-13 06:36:49.000000 PyQuantKit-0.2.1/setup.py
```

### Comparing `PyQuantKit-0.2.0a0/LICENSE` & `PyQuantKit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.0a0/PyQuantKit/ConsoleUtils.py` & `PyQuantKit-0.2.1/PyQuantKit/ConsoleUtils.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.0a0/PyQuantKit/MarketUtils.py` & `PyQuantKit-0.2.1/PyQuantKit/MarketUtils.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.0a0/PyQuantKit/TechnicalAnalysis.py` & `PyQuantKit-0.2.1/PyQuantKit/TechnicalAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.0a0/PyQuantKit/TradeUtils.py` & `PyQuantKit-0.2.1/PyQuantKit/TradeUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,42 +73,43 @@
 class TradeReport(object):
     def __init__(
             self, *,
             ticker: str,
             side: int | float | str | TransactionSide,
             volume: float,
             notional: float,
-            trade_time: datetime.datetime,
             order_id: str,
+            timestamp: float = None,
+            trade_time: datetime.datetime = None,
             price: float = None,
             trade_id: str = None,
             multiplier: float = 1,
             fee: float = .0
     ):
         """
         store trade report data
         :param ticker: ticker (symbol) of the given asset (stock, future, option, crypto and etc.)
         :param side: TransactionSide should be the same as TradeInstruction
         :param volume: Traded volume (the number of shares, contracts or crypto, etc.)
         :param notional: Traded notional (the amount of money) or premium of the option
-        :param trade_time: datetime.datetime when trade was matched
+        :param timestamp: Timestamp when trade was matched
         :param order_id: the id of its TradeInstruction
         :param price: the traded price. NOTED: trade price does not necessarily equal notional / volume. For example, currency swap, crypto swap (future) and debt
         :param trade_id: the id of itself
         :param multiplier: multiplier for contract or option
         :param fee: transition fee of this trade
         """
         assert volume >= 0, 'Trade volume must not be negative'
 
         self.__ticker = str(ticker)
         self.__side = TransactionSide(side)
         self.__price = price
         self.__volume = volume
         self.__notional = notional
-        self.__trade_time = trade_time
+        self.__timestamp = trade_time.timestamp() if timestamp is None else timestamp
         self.__order_id = str(order_id)
         self.__trade_id = str(trade_id) if trade_id is not None else str(uuid.uuid4())
         self.__multiplier = float(multiplier)
         self.__fee = fee
 
     def __repr__(self):
         return '<TradeReport>{}'.format({key: item.name if key == 'side' else item for key, item in self.__dict__.items()})
@@ -168,15 +169,15 @@
     def to_json(self, fmt: str = 'str') -> str | dict:
         json_dict = {
             'ticker': self.__ticker,
             'side': self.__side.name,
             'price': self.__price,
             'volume': self.__volume,
             'notional': self.__notional,
-            'trade_time': self.__trade_time.timestamp(),
+            'timestamp': self.__timestamp,
             'order_id': self.__order_id,
             'trade_id': self.__trade_id,
             'multiplier': self.__multiplier,
             'fee': self.__fee,
         }
 
         if fmt == 'dict':
@@ -186,15 +187,15 @@
 
     def copy(self, **kwargs):
         new_trade = self.__class__(
             ticker=kwargs.pop('ticker', self.__ticker),
             side=kwargs.pop('side', self.__side),
             volume=kwargs.pop('volume', self.__volume),
             notional=kwargs.pop('notional', self.__notional),
-            trade_time=kwargs.pop('trade_time', self.__trade_time),
+            timestamp=kwargs.pop('timestamp', self.__timestamp),
             order_id=kwargs.pop('order_id', None),
             price=kwargs.pop('price', self.__price),
             trade_id=kwargs.pop('trade_id', f'{self.__trade_id}.copy'),
             multiplier=kwargs.pop('multiplier', self.__multiplier),
             fee=kwargs.pop('fee', self.__fee)
         )
 
@@ -209,15 +210,15 @@
 
         self = cls(
             ticker=json_dict['ticker'],
             side=TransactionSide(json_dict['side']),
             volume=json_dict['volume'],
             price=json_dict['price'],
             notional=json_dict['notional'],
-            trade_time=datetime.datetime.fromtimestamp(json_dict['trade_time']),
+            timestamp=json_dict['timestamp'],
             order_id=json_dict['order_id'],
             trade_id=json_dict['trade_id'],
             multiplier=json_dict['multiplier'],
             fee=json_dict['fee'],
         )
 
         return self
@@ -225,15 +226,15 @@
     @staticmethod
     def from_trade(trade_data: TradeData, order_id: str, trade_id: str = None) -> TradeReport:
         report = TradeReport(
             ticker=trade_data.ticker,
             side=trade_data.side,
             volume=trade_data.volume,
             notional=trade_data.notional,
-            trade_time=trade_data.trade_time,
+            timestamp=trade_data.timestamp,
             order_id=order_id,
             trade_id=trade_id
         )
         return report
 
     @property
     def multiplier(self) -> float:
@@ -266,19 +267,19 @@
         elif self.__volume == 0:
             return .0
         else:
             return self.__notional / self.__volume / self.__multiplier
 
     @property
     def trade_time(self) -> datetime.datetime:
-        return self.__trade_time
+        return datetime.datetime.fromtimestamp(self.__timestamp)
 
     @property
     def timestamp(self):
-        return self.__trade_time.timestamp()
+        return self.__timestamp
 
     @property
     def order_id(self) -> str:
         return self.__order_id
 
     @property
     def trade_id(self) -> str:
```

### Comparing `PyQuantKit-0.2.0a0/PyQuantKit/_FinanceDecimal.py` & `PyQuantKit-0.2.1/PyQuantKit/_FinanceDecimal.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.0a0/PyQuantKit/__init__.py` & `PyQuantKit-0.2.1/PyQuantKit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = '0.2.0.a'
+__version__ = '0.2.1'
 
 import logging
 import sys
 import time
 
 LOGGER: logging.Logger | None = None
 LOG_LEVEL = logging.INFO
```

### Comparing `PyQuantKit-0.2.0a0/setup.py` & `PyQuantKit-0.2.1/setup.py`

 * *Files identical despite different names*


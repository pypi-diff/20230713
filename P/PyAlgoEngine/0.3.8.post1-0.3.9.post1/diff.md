# Comparing `tmp/PyAlgoEngine-0.3.8.post1.tar.gz` & `tmp/PyAlgoEngine-0.3.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAlgoEngine-0.3.8.post1.tar", last modified: Tue Jul 11 08:35:44 2023, max compression
+gzip compressed data, was "PyAlgoEngine-0.3.9.post1.tar", last modified: Thu Jul 13 08:02:28 2023, max compression
```

## Comparing `PyAlgoEngine-0.3.8.post1.tar` & `PyAlgoEngine-0.3.9.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 08:35:44.097739 PyAlgoEngine-0.3.8.post1/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 08:35:42.018439 PyAlgoEngine-0.3.8.post1/AlgoEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 08:35:42.737139 PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31104 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/AlgoEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1465 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/EventEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    32307 2023-07-11 05:55:16.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/MarketEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    79235 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/TradeEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3653 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 08:35:43.233955 PyAlgoEngine-0.3.8.post1/AlgoEngine/Strategies/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1814 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Strategies/BackTest.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    14977 2023-07-11 08:34:21.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Strategies/_StrategyEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1738 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/Strategies/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      432 2023-07-11 08:34:54.000000 PyAlgoEngine-0.3.8.post1/AlgoEngine/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      521 2023-07-11 08:35:44.081411 PyAlgoEngine-0.3.8.post1/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 08:35:43.944029 PyAlgoEngine-0.3.8.post1/PyAlgoEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      521 2023-07-11 08:35:31.000000 PyAlgoEngine-0.3.8.post1/PyAlgoEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      499 2023-07-11 08:35:35.000000 PyAlgoEngine-0.3.8.post1/PyAlgoEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-07-11 08:35:31.000000 PyAlgoEngine-0.3.8.post1/PyAlgoEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       57 2023-07-11 08:35:31.000000 PyAlgoEngine-0.3.8.post1/PyAlgoEngine.egg-info/requires.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-07-11 08:35:31.000000 PyAlgoEngine-0.3.8.post1/PyAlgoEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       42 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-07-11 08:35:44.104812 PyAlgoEngine-0.3.8.post1/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1528 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8.post1/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:02:28.835953 PyAlgoEngine-0.3.9.post1/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:02:27.742215 PyAlgoEngine-0.3.9.post1/AlgoEngine/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:02:28.185423 PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31104 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/AlgoEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1465 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/EventEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    32307 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/MarketEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    80159 2023-07-13 07:54:27.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/TradeEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3653 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:02:28.421032 PyAlgoEngine-0.3.9.post1/AlgoEngine/Strategies/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1814 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Strategies/BackTest.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    14957 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Strategies/_StrategyEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1738 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/Strategies/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      432 2023-07-13 08:01:55.000000 PyAlgoEngine-0.3.9.post1/AlgoEngine/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      521 2023-07-13 08:02:28.826061 PyAlgoEngine-0.3.9.post1/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-13 08:02:28.751186 PyAlgoEngine-0.3.9.post1/PyAlgoEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      521 2023-07-13 08:02:21.000000 PyAlgoEngine-0.3.9.post1/PyAlgoEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      499 2023-07-13 08:02:23.000000 PyAlgoEngine-0.3.9.post1/PyAlgoEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-07-13 08:02:21.000000 PyAlgoEngine-0.3.9.post1/PyAlgoEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       57 2023-07-13 08:02:21.000000 PyAlgoEngine-0.3.9.post1/PyAlgoEngine.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-07-13 08:02:21.000000 PyAlgoEngine-0.3.9.post1/PyAlgoEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       42 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-07-13 08:02:28.838201 PyAlgoEngine-0.3.9.post1/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1528 2023-07-13 06:42:19.000000 PyAlgoEngine-0.3.9.post1/setup.py
```

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/AlgoEngine.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/AlgoEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/EventEngine.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/EventEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/MarketEngine.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/MarketEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/TradeEngine.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/TradeEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,39 @@
         if algo is None:
             return 0
 
         result = algo.on_filled(report=report, **kwargs)
         self._update_status()
         return result
 
+    def add_exposure(self, ticker: str, volume: float, notional: float, side: TransactionSide, timestamp: float):
+        """
+        this is a method to add dummy algo and fills it.
+
+        the method provides an easy way to amend exposure
+        """
+
+        algo = self.algo_registry.to_algo(name=self.algo_registry.passive)(
+            handler=self,
+            ticker=ticker,
+            side=side,
+            target_volume=volume,
+            dma=None,
+        )
+        self.algos[algo.algo_id] = algo
+
+        order = TradeInstruction(ticker=ticker, order_id=f'Dummy.{uuid.uuid4().hex}', volume=volume, side=side)
+        report = TradeReport(ticker=ticker, volume=volume, notional=notional, side=side, timestamp=timestamp, order_id=order.order_id)
+        order.fill(report)
+        algo.status = algo.Status.done
+        algo.order[order.order_id] = order
+        self._update_status()
+
+        return report
+
     def on_canceled(self, order_id: str, **kwargs):
         algo = self.reversed_order_mapping.get(order_id)
 
         if algo is None:
             return 0
 
         result = algo.on_canceled(order_id=order_id, **kwargs)
```

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Engine/__init__.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Engine/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Strategies/BackTest.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Strategies/BackTest.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Strategies/_StrategyEngine.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Strategies/_StrategyEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,62 +87,62 @@
             self._on_eod.remove(kwargs['on_eod'])
 
         if 'on_bod' in kwargs:
             self._on_bod.remove(kwargs['on_bod'])
 
     def add_handler_safe(self, **kwargs):
         if 'on_market_data' in kwargs:
-            if (handler := kwargs['on_market_data']) in self._on_market_data:
+            if handler := kwargs['on_market_data'] in self._on_market_data:
                 LOGGER.warning(f'on_market_data handler {handler} already registered, skipped!')
             else:
                 self._on_market_data.append(handler)
 
         if 'on_report' in kwargs:
-            if (handler := kwargs['on_report']) in self._on_report:
+            if handler := kwargs['on_report'] in self._on_report:
                 LOGGER.warning(f'on_report handler {handler} already registered, skipped!')
             else:
                 self._on_report.append(handler)
 
         if 'on_order' in kwargs:
-            if (handler := kwargs['on_order']) in self._on_order:
+            if handler := kwargs['on_order'] in self._on_order:
                 LOGGER.warning(f'on_order handler {handler} already registered, skipped!')
             else:
                 self._on_order.append(handler)
 
         if 'on_eod' in kwargs:
-            if (handler := kwargs['on_eod']) in self._on_eod:
+            if handler := kwargs['on_eod'] in self._on_eod:
                 LOGGER.warning(f'on_eod handler {handler} already registered, skipped!')
             else:
                 self._on_eod.append(handler)
 
         if 'on_bod' in kwargs:
-            if (handler := kwargs['on_bod']) in self._on_bod:
+            if handler := kwargs['on_bod'] in self._on_bod:
                 LOGGER.warning(f'on_bod handler {handler} already registered, skipped!')
             else:
                 self._on_bod.append(handler)
 
     def remove_handler_safe(self, **kwargs):
         if 'on_market_data' in kwargs:
-            if (handler := kwargs['on_market_data']) in self._on_market_data:
+            if handler := kwargs['on_market_data'] in self._on_market_data:
                 self._on_market_data.remove(handler)
 
         if 'on_report' in kwargs:
-            if (handler := kwargs['on_report']) in self._on_report:
+            if handler := kwargs['on_report'] in self._on_report:
                 self._on_report.remove(handler)
 
         if 'on_order' in kwargs:
-            if (handler := kwargs['on_order']) in self._on_order:
+            if handler := kwargs['on_order'] in self._on_order:
                 self._on_order.remove(handler)
 
         if 'on_eod' in kwargs:
-            if (handler := kwargs['on_eod']) in self._on_eod:
+            if handler := kwargs['on_eod'] in self._on_eod:
                 self._on_eod.remove(handler)
 
         if 'on_bod' in kwargs:
-            if (handler := kwargs['on_bod']) in self._on_bod:
+            if handler := kwargs['on_bod'] in self._on_bod:
                 self._on_bod.remove(handler)
 
     def attach_strategy(self, strategy: object):
         if callable(handler := getattr(strategy, 'on_market_data', None)):
             self._on_market_data.append(handler)
 
         if callable(handler := getattr(strategy, 'on_report', None)):
```

### Comparing `PyAlgoEngine-0.3.8.post1/AlgoEngine/Strategies/__init__.py` & `PyAlgoEngine-0.3.9.post1/AlgoEngine/Strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.8.post1/LICENSE` & `PyAlgoEngine-0.3.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.8.post1/PKG-INFO` & `PyAlgoEngine-0.3.9.post1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.8.post1
+Version: 0.3.9.post1
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `PyAlgoEngine-0.3.8.post1/PyAlgoEngine.egg-info/PKG-INFO` & `PyAlgoEngine-0.3.9.post1/PyAlgoEngine.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.8.post1
+Version: 0.3.9.post1
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `PyAlgoEngine-0.3.8.post1/setup.py` & `PyAlgoEngine-0.3.9.post1/setup.py`

 * *Files identical despite different names*


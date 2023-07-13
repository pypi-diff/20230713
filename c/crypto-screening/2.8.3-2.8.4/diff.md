# Comparing `tmp/crypto-screening-2.8.3.tar.gz` & `tmp/crypto-screening-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.8.3.tar", last modified: Wed Jul 12 23:37:14 2023, max compression
+gzip compressed data, was "crypto-screening-2.8.4.tar", last modified: Thu Jul 13 01:43:01 2023, max compression
```

## Comparing `crypto-screening-2.8.3.tar` & `crypto-screening-2.8.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 23:37:14.873614 crypto-screening-2.8.3/
--rw-rw-rw-   0        0        0       98 2023-07-12 23:37:14.000000 crypto-screening-2.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-12 23:37:14.873614 crypto-screening-2.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:37:14.842796 crypto-screening-2.8.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-12 23:37:14.862911 crypto-screening-2.8.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.3/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    39266 2023-07-12 23:07:59.000000 crypto-screening-2.8.3/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21275 2023-07-12 23:36:53.000000 crypto-screening-2.8.3/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19359 2023-07-12 23:37:04.000000 crypto-screening-2.8.3/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:37:14.863942 crypto-screening-2.8.3/crypto_screening/market/
--rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.3/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:37:14.867514 crypto-screening-2.8.3/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.3/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.3/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.3/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.3/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:37:14.872589 crypto-screening-2.8.3/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.3/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.3/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.3/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.8.3/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.3/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.3/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.3/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.3/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.3/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:37:14.857372 crypto-screening-2.8.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-12 23:37:14.000000 crypto-screening-2.8.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-12 23:37:14.000000 crypto-screening-2.8.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 23:37:14.000000 crypto-screening-2.8.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-12 23:37:14.000000 crypto-screening-2.8.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-12 23:37:14.000000 crypto-screening-2.8.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-12 23:37:14.000000 crypto-screening-2.8.3/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 23:37:14.873614 crypto-screening-2.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-12 23:37:11.000000 crypto-screening-2.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.454387 crypto-screening-2.8.4/
+-rw-rw-rw-   0        0        0       98 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-13 01:43:01.454387 crypto-screening-2.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.4/build.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.422187 crypto-screening-2.8.4/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.443824 crypto-screening-2.8.4/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.4/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.4/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    39266 2023-07-12 23:07:59.000000 crypto-screening-2.8.4/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21275 2023-07-12 23:36:53.000000 crypto-screening-2.8.4/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19359 2023-07-12 23:37:04.000000 crypto-screening-2.8.4/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.4/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.4/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.4/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.4/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.4/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.445824 crypto-screening-2.8.4/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.4/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.448852 crypto-screening-2.8.4/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.4/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.453882 crypto-screening-2.8.4/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32677 2023-07-13 01:20:24.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.4/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.4/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.4/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.4/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.4/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:43:01.438792 crypto-screening-2.8.4/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-13 01:43:01.000000 crypto-screening-2.8.4/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 01:43:01.454387 crypto-screening-2.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-13 01:42:55.000000 crypto-screening-2.8.4/setup.py
```

### Comparing `crypto-screening-2.8.3/PKG-INFO` & `crypto-screening-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.3
+Version: 2.8.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.3/README.md` & `crypto-screening-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/build.py` & `crypto-screening-2.8.4/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/collect/assets.py` & `crypto-screening-2.8.4/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/collect/exchanges.py` & `crypto-screening-2.8.4/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/collect/market.py` & `crypto-screening-2.8.4/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/collect/ohlcv.py` & `crypto-screening-2.8.4/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/collect/orderbook.py` & `crypto-screening-2.8.4/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/collect/screeners.py` & `crypto-screening-2.8.4/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/collect/symbols.py` & `crypto-screening-2.8.4/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/dataset.py` & `crypto-screening-2.8.4/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/interval.py` & `crypto-screening-2.8.4/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/dynamic.py` & `crypto-screening-2.8.4/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/foundation/data.py` & `crypto-screening-2.8.4/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.8.4/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/foundation/state.py` & `crypto-screening-2.8.4/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.8.4/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/screeners/base.py` & `crypto-screening-2.8.4/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/screeners/container.py` & `crypto-screening-2.8.4/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.8.4/crypto_screening/market/screeners/ohlcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -784,15 +784,15 @@
                 delay=delay, location=location,
                 options=options, cancel=cancel
             )
 
         except ValueError as e:
             warnings.warn(str(e))
 
-            container[symbol] = None
+            container.setdefault(exchange, {})[symbol] = None
         # end try
     # end _create_screener
 
     def _create_screeners(
             self,
             symbols: Iterable[str],
             exchange: str,
@@ -887,25 +887,20 @@
                         delay=delay, location=location,
                         options=options, cancel=cancel
                     )
                 )
             )
         # end for
 
-        multi_threaded_call(callers=callers)
-
         screeners = []
 
-        for exchange in market.values():
-            for symbol, screener in exchange.copy().items():
+        for exchange, symbols in market.items():
+            for symbol, screener in symbols.items():
                 if isinstance(screener, OHLCVScreener):
                     screeners.append(screener)
-
-                else:
-                    exchange.pop(symbol)
                 # end if
             # end for
         # end for
 
         return screeners
     # end create_screeners
```

### Comparing `crypto-screening-2.8.3/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.8.4/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.8.4/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/market/waiting.py` & `crypto-screening-2.8.4/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/process.py` & `crypto-screening-2.8.4/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/symbols.py` & `crypto-screening-2.8.4/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening/validate.py` & `crypto-screening-2.8.4/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.8.4/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.3
+Version: 2.8.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.8.4/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.3/pyproject.toml` & `crypto-screening-2.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.8.3'
+version = '2.8.4'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.8.3/setup.py` & `crypto-screening-2.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.8.3',
+        version='2.8.4',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```


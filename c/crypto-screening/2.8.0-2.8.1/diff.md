# Comparing `tmp/crypto-screening-2.8.0.tar.gz` & `tmp/crypto-screening-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.8.0.tar", last modified: Wed Jul 12 22:52:38 2023, max compression
+gzip compressed data, was "crypto-screening-2.8.1.tar", last modified: Wed Jul 12 23:01:52 2023, max compression
```

## Comparing `crypto-screening-2.8.0.tar` & `crypto-screening-2.8.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.123528 crypto-screening-2.8.0/
--rw-rw-rw-   0        0        0       98 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-12 22:52:38.123528 crypto-screening-2.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.029834 crypto-screening-2.8.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.067431 crypto-screening-2.8.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    39228 2023-07-12 22:48:08.000000 crypto-screening-2.8.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21241 2023-07-12 22:49:02.000000 crypto-screening-2.8.0/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19325 2023-07-12 22:49:02.000000 crypto-screening-2.8.0/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.068439 crypto-screening-2.8.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.085409 crypto-screening-2.8.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.122557 crypto-screening-2.8.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:52:38.042835 crypto-screening-2.8.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-12 22:52:37.000000 crypto-screening-2.8.0/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 22:52:38.124529 crypto-screening-2.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-12 22:52:23.000000 crypto-screening-2.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.832545 crypto-screening-2.8.1/
+-rw-rw-rw-   0        0        0       98 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-12 23:01:52.832545 crypto-screening-2.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.8.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.8.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.803423 crypto-screening-2.8.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.822529 crypto-screening-2.8.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.8.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.8.1/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    39202 2023-07-12 23:01:36.000000 crypto-screening-2.8.1/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21241 2023-07-12 22:49:02.000000 crypto-screening-2.8.1/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19325 2023-07-12 22:49:02.000000 crypto-screening-2.8.1/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.8.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.8.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.8.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.8.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.8.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.824529 crypto-screening-2.8.1/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10285 2023-07-12 22:22:15.000000 crypto-screening-2.8.1/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.827037 crypto-screening-2.8.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-2.8.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.831597 crypto-screening-2.8.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.8.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-2.8.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.8.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.8.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.8.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:01:52.817502 crypto-screening-2.8.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-12 23:01:52.000000 crypto-screening-2.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.8.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.8.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 23:01:52.832545 crypto-screening-2.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-12 23:01:43.000000 crypto-screening-2.8.1/setup.py
```

### Comparing `crypto-screening-2.8.0/PKG-INFO` & `crypto-screening-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.0
+Version: 2.8.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.0/README.md` & `crypto-screening-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/build.py` & `crypto-screening-2.8.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/collect/assets.py` & `crypto-screening-2.8.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/collect/exchanges.py` & `crypto-screening-2.8.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/collect/market.py` & `crypto-screening-2.8.1/crypto_screening/collect/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -1099,15 +1099,15 @@
             )
         # end if
 
         base, quote = symbol_to_parts(
             symbol=screener.symbol, separator=separator
         )
 
-        for name in zip(columns, prices):
+        for name in columns:
             (
                 prices[name].
                 setdefault(screener.exchange, {}).
                 setdefault(base, {}).
                 setdefault(
                     quote,
                     list(
@@ -1161,15 +1161,15 @@
                 f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
                 f"is not long enough for the requested length: {length}. "
                 f"Consider using the 'adjust' parameter as {True}, "
                 f"to adjust to the actual length of the data."
             )
         # end if
 
-        for name in zip(columns, prices):
+        for name in columns:
             (
                 prices[name].
                 setdefault(screener.exchange, {}).
                 setdefault(
                     screener.symbol,
                     list(
                         zip(
```

### Comparing `crypto-screening-2.8.0/crypto_screening/collect/ohlcv.py` & `crypto-screening-2.8.1/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/collect/orderbook.py` & `crypto-screening-2.8.1/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/collect/screeners.py` & `crypto-screening-2.8.1/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/collect/symbols.py` & `crypto-screening-2.8.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/dataset.py` & `crypto-screening-2.8.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/interval.py` & `crypto-screening-2.8.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/dynamic.py` & `crypto-screening-2.8.1/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/foundation/data.py` & `crypto-screening-2.8.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.8.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/foundation/state.py` & `crypto-screening-2.8.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.8.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/screeners/base.py` & `crypto-screening-2.8.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/screeners/container.py` & `crypto-screening-2.8.1/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.8.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.8.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.8.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/market/waiting.py` & `crypto-screening-2.8.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/process.py` & `crypto-screening-2.8.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/symbols.py` & `crypto-screening-2.8.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening/validate.py` & `crypto-screening-2.8.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.8.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.8.0
+Version: 2.8.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.8.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.8.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.8.0/pyproject.toml` & `crypto-screening-2.8.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.8.0'
+version = '2.8.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.8.0/setup.py` & `crypto-screening-2.8.1/setup.py`

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
-        version='2.8.0',
+        version='2.8.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```


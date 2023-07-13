# Comparing `tmp/yfinance-0.2.7.tar.gz` & `tmp/yfinance-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfinance-0.2.7.tar", last modified: Thu Jan 26 17:04:18 2023, max compression
+gzip compressed data, was "yfinance-0.2.9.tar", last modified: Thu Jan 26 22:22:36 2023, max compression
```

## Comparing `yfinance-0.2.7.tar` & `yfinance-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:04:18.163169 yfinance-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-26 17:04:02.000000 yfinance-0.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-26 17:04:02.000000 yfinance-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-01-26 17:04:18.163169 yfinance-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-01-26 17:04:02.000000 yfinance-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-26 17:04:18.163169 yfinance-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-01-26 17:04:02.000000 yfinance-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:04:18.163169 yfinance-0.2.7/yfinance/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63482 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:04:18.163169 yfinance-0.2.7/yfinance/scrapers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/scrapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/scrapers/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/scrapers/fundamentals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/scrapers/holders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/scrapers/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/tickers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34999 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-26 17:04:02.000000 yfinance-0.2.7/yfinance/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:04:18.163169 yfinance-0.2.7/yfinance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-01-26 17:04:18.000000 yfinance-0.2.7/yfinance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-26 17:04:18.000000 yfinance-0.2.7/yfinance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 17:04:18.000000 yfinance-0.2.7/yfinance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-26 17:04:18.000000 yfinance-0.2.7/yfinance.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-26 17:04:18.000000 yfinance-0.2.7/yfinance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-26 17:04:18.000000 yfinance-0.2.7/yfinance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:22:36.465235 yfinance-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-26 22:22:19.000000 yfinance-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-26 22:22:19.000000 yfinance-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-01-26 22:22:36.465235 yfinance-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-01-26 22:22:19.000000 yfinance-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-26 22:22:36.465235 yfinance-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-01-26 22:22:19.000000 yfinance-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:22:36.465235 yfinance-0.2.9/yfinance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65348 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:22:36.465235 yfinance-0.2.9/yfinance/scrapers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/scrapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/scrapers/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/scrapers/fundamentals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/scrapers/holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/scrapers/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34999 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-26 22:22:19.000000 yfinance-0.2.9/yfinance/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:22:36.465235 yfinance-0.2.9/yfinance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-01-26 22:22:36.000000 yfinance-0.2.9/yfinance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-26 22:22:36.000000 yfinance-0.2.9/yfinance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 22:22:36.000000 yfinance-0.2.9/yfinance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-26 22:22:36.000000 yfinance-0.2.9/yfinance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-26 22:22:36.000000 yfinance-0.2.9/yfinance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-26 22:22:36.000000 yfinance-0.2.9/yfinance.egg-info/top_level.txt
```

### Comparing `yfinance-0.2.7/LICENSE.txt` & `yfinance-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/PKG-INFO` & `yfinance-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance
-Version: 0.2.7
+Version: 0.2.9
 Summary: Download market data from Yahoo! Finance API
 Home-page: https://github.com/ranaroussi/yfinance
 Author: Ran Aroussi
 Author-email: ran@aroussi.com
 License: Apache
 Keywords: pandas,yahoo finance,pandas datareader
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yfinance Version: 0.2.7 Summary: Download market
+Metadata-Version: 2.1 Name: yfinance Version: 0.2.9 Summary: Download market
 data from Yahoo! Finance API Home-page: https://github.com/ranaroussi/yfinance
 Author: Ran Aroussi Author-email: ran@aroussi.com License: Apache Keywords:
 pandas,yahoo finance,pandas datareader Platform: any Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Topic :: Office/Business :: Financial Classifier: Topic
 :: Office/Business :: Financial :: Investment Classifier: Topic :: Scientific/
```

### Comparing `yfinance-0.2.7/README.md` & `yfinance-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/setup.py` & `yfinance-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/__init__.py` & `yfinance-0.2.9/yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/base.py` & `yfinance-0.2.9/yfinance/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         self._day_high = None
         self._day_low = None
         self._last_price = None
         self._last_volume = None
 
         self._prev_close = None
 
+        self._reg_prev_close = None
+
         self._50d_day_average = None
         self._200d_day_average = None
         self._year_high = None
         self._year_low = None
         self._year_change = None
 
         self._10d_avg_vol = None
@@ -85,20 +87,25 @@
         # attrs = utils.attributes(self)
         # return attrs.keys()
         # utils.attributes is calling each method, bad!
         # Have to hardcode
         keys = ["currency", "exchange", "timezone"]
         keys += ["shares", "market_cap"]
         keys += ["last_price", "previous_close", "open", "day_high", "day_low"]
+        keys += ["regular_market_previous_close"]
         keys += ["last_volume"]
         keys += ["fifty_day_average", "two_hundred_day_average", "ten_day_average_volume", "three_month_average_volume"]
         keys += ["year_high", "year_low", "year_change"]
         return keys
     def items(self):
         return [(k,self[k]) for k in self.keys()]
+    def get(self, key, default=None):
+        if key in self.keys():
+            return self[key]
+        return default
     def __getitem__(self, k):
         if not isinstance(k, str):
             raise KeyError(f"key must be a string")
         if not k in self.keys():
             raise KeyError(f"'{k}' not valid key. Examine 'FastInfo.keys()'")
         return getattr(self, k)
     def __contains__(self, k):
@@ -107,31 +114,35 @@
         return iter(self.keys())
 
     def __str__(self):
         return "lazy-loading dict with keys = " + str(self.keys())
     def __repr__(self):
         return self.__str__()
 
+    def toJSON(self, indent=4):
+        d = {k:self[k] for k in self.keys()}
+        return _json.dumps({k:self[k] for k in self.keys()}, indent=indent)
+
     def _get_1y_prices(self, fullDaysOnly=False):
         if self._prices_1y is None:
-            self._prices_1y = self._tkr.history(period="380d", auto_adjust=False)
+            self._prices_1y = self._tkr.history(period="380d", auto_adjust=False, debug=False)
             self._md = self._tkr.get_history_metadata()
             try:
                 ctp = self._md["currentTradingPeriod"]
                 self._today_open = pd.to_datetime(ctp["regular"]["start"], unit='s', utc=True).tz_convert(self.timezone)
                 self._today_close = pd.to_datetime(ctp["regular"]["end"], unit='s', utc=True).tz_convert(self.timezone)
                 self._today_midnight = self._today_close.ceil("D")
             except:
                 self._today_open = None
                 self._today_close = None
                 self._today_midnight = None
                 raise
 
         if self._prices_1y.empty:
-            return self.self._prices_1y
+            return self._prices_1y
 
         dt1 = self._prices_1y.index[-1]
         if fullDaysOnly and self._exchange_open_now():
             # Exclude today
             dt1 -= utils._interval_to_timedelta("1h")
         dt0 = dt1 - utils._interval_to_timedelta("1y") + utils._interval_to_timedelta("1d")
         return self._prices_1y.loc[dt0:dt1]
@@ -195,183 +206,219 @@
         return self._timezone
 
     @property
     def shares(self):
         if self._shares is not None:
             return self._shares
 
-        try:
-            shares = self._tkr.get_shares_full(start=pd.Timestamp.utcnow().date()-pd.Timedelta(days=548))
-        except Exception as e:
-            if "did not return share count" in str(e):
-                shares = None
-            else:
-                raise
+        shares = self._tkr.get_shares_full(start=pd.Timestamp.utcnow().date()-pd.Timedelta(days=548))
         if shares is None:
             # Requesting 18 months failed, so fallback to shares which should include last year
             shares = self._tkr.get_shares()
-        if shares is None:
-            raise Exception(f"{self._tkr.ticker}: Cannot retrieve share count")
-        if isinstance(shares, pd.DataFrame):
-            shares = shares[shares.columns[0]]
-        self._shares = shares.iloc[-1]
+        if shares is not None:
+            if isinstance(shares, pd.DataFrame):
+                shares = shares[shares.columns[0]]
+            self._shares = int(shares.iloc[-1])
         return self._shares
 
     @property
     def last_price(self):
         if self._last_price is not None:
             return self._last_price
-        # self._last_price = self._get_exchange_metadata()["regularMarketPrice"]
         prices = self._get_1y_prices()
-        self._last_price = _np.nan if prices.empty else prices["Close"].iloc[-1]
+        if prices.empty:
+            self._last_price = self._get_exchange_metadata()["regularMarketPrice"]
+        else:
+            self._last_price = float(prices["Close"].iloc[-1])
         return self._last_price
 
     @property
     def previous_close(self):
         if self._prev_close is not None:
             return self._prev_close
         prices = self._get_1y_prices()
-        self._prev_close = _np.nan if prices.empty else prices["Close"].iloc[-2]
+        if prices.empty:
+            # Very few symbols have previousClose despite no 
+            # no trading data. E.g. 'QCSTIX'.
+            # So fallback to original info[] if available.
+            self._tkr.info  # trigger fetch
+            if "previousClose" in self._tkr._quote._retired_info:
+                self._prev_close = self._tkr._quote._retired_info["previousClose"]
+        else:
+            self._prev_close = float(prices["Close"].iloc[-2])
         return self._prev_close
 
     @property
+    def regular_market_previous_close(self):
+        if self._reg_prev_close is not None:
+            return self._reg_prev_close
+        prices = self._get_1y_prices()
+        if prices.empty:
+            # Very few symbols have regularMarketPreviousClose despite no 
+            # no trading data. E.g. 'QCSTIX'.
+            # So fallback to original info[] if available.
+            self._tkr.info  # trigger fetch
+            if "regularMarketPreviousClose" in self._tkr._quote._retired_info:
+                self._reg_prev_close = self._tkr._quote._retired_info["regularMarketPreviousClose"]
+        else:
+            self._reg_prev_close = float(prices["Close"].iloc[-2])
+        return self._reg_prev_close
+
+    @property
     def open(self):
         if self._open is not None:
             return self._open
         prices = self._get_1y_prices()
-        self._open = _np.nan if prices.empty else prices["Open"].iloc[-1]
+        self._open = None if prices.empty else float(prices["Open"].iloc[-1])
         return self._open
 
     @property
     def day_high(self):
         if self._day_high is not None:
             return self._day_high
         prices = self._get_1y_prices()
-        self._day_high = _np.nan if prices.empty else prices["High"].iloc[-1]
+        self._day_high = None if prices.empty else float(prices["High"].iloc[-1])
         return self._day_high
 
     @property
     def day_low(self):
         if self._day_low is not None:
             return self._day_low
         prices = self._get_1y_prices()
-        self._day_low = _np.nan if prices.empty else prices["Low"].iloc[-1]
+        self._day_low = None if prices.empty else float(prices["Low"].iloc[-1])
         return self._day_low
 
     @property
     def last_volume(self):
         if self._last_volume is not None:
             return self._last_volume
         prices = self._get_1y_prices()
-        self._last_volume = 0 if prices.empty else prices["Volume"].iloc[-1]
+        self._last_volume = None if prices.empty else int(prices["Volume"].iloc[-1])
         return self._last_volume
 
     @property
     def fifty_day_average(self):
         if self._50d_day_average is not None:
             return self._50d_day_average
 
         prices = self._get_1y_prices(fullDaysOnly=True)
         if prices.empty:
-            self._50d_day_average = _np.nan
+            self._50d_day_average = None
         else:
             n = prices.shape[0]
             a = n-50
             b = n
             if a < 0:
                 a = 0
-            self._50d_day_average = prices["Close"].iloc[a:b].mean()
+            self._50d_day_average = float(prices["Close"].iloc[a:b].mean())
 
         return self._50d_day_average
 
     @property
     def two_hundred_day_average(self):
         if self._200d_day_average is not None:
             return self._200d_day_average
 
         prices = self._get_1y_prices(fullDaysOnly=True)
         if prices.empty:
-            self._200d_day_average = _np.nan
+            self._200d_day_average = None
         else:
             n = prices.shape[0]
             a = n-200
             b = n
             if a < 0:
                 a = 0
 
-            self._200d_day_average = prices["Close"].iloc[a:b].mean()
+            self._200d_day_average = float(prices["Close"].iloc[a:b].mean())
 
         return self._200d_day_average
 
     @property
     def ten_day_average_volume(self):
         if self._10d_avg_vol is not None:
             return self._10d_avg_vol
 
         prices = self._get_1y_prices(fullDaysOnly=True)
         if prices.empty:
-            self._10d_avg_vol = 0
+            self._10d_avg_vol = None
         else:
             n = prices.shape[0]
             a = n-10
             b = n
             if a < 0:
                 a = 0
-            self._10d_avg_vol = prices["Volume"].iloc[a:b].mean()
+            self._10d_avg_vol = int(prices["Volume"].iloc[a:b].mean())
 
         return self._10d_avg_vol
 
     @property
     def three_month_average_volume(self):
         if self._3mo_avg_vol is not None:
             return self._3mo_avg_vol
 
         prices = self._get_1y_prices(fullDaysOnly=True)
         if prices.empty:
-            self._3mo_avg_vol = 0
+            self._3mo_avg_vol = None
         else:
             dt1 = prices.index[-1]
             dt0 = dt1 - utils._interval_to_timedelta("3mo") + utils._interval_to_timedelta("1d")
-            self._3mo_avg_vol = prices.loc[dt0:dt1, "Volume"].mean()
+            self._3mo_avg_vol = int(prices.loc[dt0:dt1, "Volume"].mean())
 
         return self._3mo_avg_vol
 
     @property
     def year_high(self):
         if self._year_high is not None:
             return self._year_high
 
         prices = self._get_1y_prices(fullDaysOnly=True)
-        self._year_high = prices["High"].max()
+        self._year_high = float(prices["High"].max())
         return self._year_high
 
     @property
     def year_low(self):
         if self._year_low is not None:
             return self._year_low
 
         prices = self._get_1y_prices(fullDaysOnly=True)
-        self._year_low = prices["Low"].min()
+        self._year_low = float(prices["Low"].min())
         return self._year_low
 
     @property
     def year_change(self):
         if self._year_change is not None:
             return self._year_change
 
         prices = self._get_1y_prices(fullDaysOnly=True)
         self._year_change = (prices["Close"].iloc[-1] - prices["Close"].iloc[0]) / prices["Close"].iloc[0]
+        self._year_change = float(self._year_change)
         return self._year_change
 
     @property
     def market_cap(self):
         if self._mcap is not None:
             return self._mcap
 
-        self._mcap = self.shares * self.last_price
+        try:
+            shares = self.shares
+        except Exception as e:
+            if "Cannot retrieve share count" in str(e):
+                shares = None
+            else:
+                raise
+
+        if shares is None:
+            # Very few symbols have marketCap despite no share count.
+            # E.g. 'BTC-USD'
+            # So fallback to original info[] if available.
+            self._tkr.info
+            if "marketCap" in self._tkr._quote._retired_info:
+                self._mcap = self._tkr._quote._retired_info["marketCap"]
+        else:
+            self._mcap = float(shares * self.last_price)
         return self._mcap
 
 
 class TickerBase:
     def __init__(self, ticker, session=None):
         self.ticker = ticker.upper()
         self.session = session
@@ -1491,15 +1538,15 @@
             fail = False
         if fail:
             print(f"{self.ticker}: Yahoo web request for share count failed")
             return None
 
         shares_data = json_data["timeseries"]["result"]
         if not "shares_out" in shares_data[0]:
-            raise Exception(f"{self.ticker}: Yahoo did not return share count in date range {start} -> {end}")
+            return None
         try:
             df = _pd.Series(shares_data[0]["shares_out"], index=_pd.to_datetime(shares_data[0]["timestamp"], unit="s"))
         except Exception as e:
             print(f"{self.ticker}: Failed to parse shares count data: "+str(e))
             return None
 
         df.index = df.index.tz_localize(tz)
```

### Comparing `yfinance-0.2.7/yfinance/data.py` & `yfinance-0.2.9/yfinance/data.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/multi.py` & `yfinance-0.2.9/yfinance/multi.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/scrapers/analysis.py` & `yfinance-0.2.9/yfinance/scrapers/analysis.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/scrapers/fundamentals.py` & `yfinance-0.2.9/yfinance/scrapers/fundamentals.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/scrapers/holders.py` & `yfinance-0.2.9/yfinance/scrapers/holders.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/scrapers/quote.py` & `yfinance-0.2.9/yfinance/scrapers/quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 info_retired_keys_price.update({"regularMarket"+s for s in ["DayHigh", "DayLow", "Open", "PreviousClose", "Price", "Volume"]})
 info_retired_keys_price.update({"fiftyTwoWeekLow", "fiftyTwoWeekHigh", "fiftyTwoWeekChange", "fiftyDayAverage", "twoHundredDayAverage"})
 info_retired_keys_price.update({"averageDailyVolume10Day", "averageVolume10days", "averageVolume"})
 info_retired_keys_exchange = {"currency", "exchange", "exchangeTimezoneName", "exchangeTimezoneShortName"}
 info_retired_keys_marketCap = {"marketCap"}
 info_retired_keys_symbol = {"symbol"}
 info_retired_keys = info_retired_keys_price | info_retired_keys_exchange | info_retired_keys_marketCap | info_retired_keys_symbol
-#
-info_retired_keys = []
 
 
 PRUNE_INFO = True
 # PRUNE_INFO = False
 
 
 from collections.abc import MutableMapping
@@ -42,24 +40,24 @@
         return self.info.__repr__()
 
     def __contains__(self, k):
         return k in self.info.keys()
 
     def __getitem__(self, k):
         if k in info_retired_keys_price:
-            print(f"Price data removed from info. Use Ticker.fast_info or history() instead")
+            print(f"Price data removed from info (key='{k}'). Use Ticker.fast_info or history() instead")
             return None
         elif k in info_retired_keys_exchange:
-            print(f"Exchange data removed from info. Use Ticker.fast_info or Ticker.get_history_metadata() instead")
+            print(f"Exchange data removed from info (key='{k}'). Use Ticker.fast_info or Ticker.get_history_metadata() instead")
             return None
         elif k in info_retired_keys_marketCap:
-            print(f"Market cap removed from info. Use Ticker.fast_info instead")
+            print(f"Market cap removed from info (key='{k}'). Use Ticker.fast_info instead")
             return None
         elif k in info_retired_keys_symbol:
-            print(f"Symbol removed from info. You know this already")
+            print(f"Symbol removed from info (key='{k}'). You know this already")
             return None
         return self.info[self._keytransform(k)]
 
     def __setitem__(self, k, value):
         self.info[self._keytransform(k)] = value
 
     def __delitem__(self, k):
@@ -79,14 +77,15 @@
 class Quote:
 
     def __init__(self, data: TickerData, proxy=None):
         self._data = data
         self.proxy = proxy
 
         self._info = None
+        self._retired_info = None
         self._sustainability = None
         self._recommendations = None
         self._calendar = None
 
         self._already_scraped = False
         self._already_scraped_complementary = False
 
@@ -197,18 +196,22 @@
                     '://')[1].split('/')[0].replace('www.', '')
                 self._info['logo_url'] = 'https://logo.clearbit.com/%s' % domain
         except Exception:
             pass
 
         # Delete redundant info[] keys, because values can be accessed faster
         # elsewhere - e.g. price keys. Hope is reduces Yahoo spam effect.
-        if PRUNE_INFO:
-            for k in info_retired_keys:
-                if k in self._info:
+        # But record the dropped keys, because in rare cases they are needed.
+        self._retired_info = {}
+        for k in info_retired_keys:
+            if k in self._info:
+                self._retired_info[k] = self._info[k]
+                if PRUNE_INFO:
                     del self._info[k]
+        if PRUNE_INFO:
             # InfoDictWrapper will explain how to access above data elsewhere
             self._info = InfoDictWrapper(self._info)
 
         # events
         try:
             cal = pd.DataFrame(quote_summary_store['calendarEvents']['earnings'])
             cal['earningsDate'] = pd.to_datetime(
```

### Comparing `yfinance-0.2.7/yfinance/shared.py` & `yfinance-0.2.9/yfinance/shared.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/ticker.py` & `yfinance-0.2.9/yfinance/ticker.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/tickers.py` & `yfinance-0.2.9/yfinance/tickers.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance/utils.py` & `yfinance-0.2.9/yfinance/utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-0.2.7/yfinance.egg-info/PKG-INFO` & `yfinance-0.2.9/yfinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance
-Version: 0.2.7
+Version: 0.2.9
 Summary: Download market data from Yahoo! Finance API
 Home-page: https://github.com/ranaroussi/yfinance
 Author: Ran Aroussi
 Author-email: ran@aroussi.com
 License: Apache
 Keywords: pandas,yahoo finance,pandas datareader
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yfinance Version: 0.2.7 Summary: Download market
+Metadata-Version: 2.1 Name: yfinance Version: 0.2.9 Summary: Download market
 data from Yahoo! Finance API Home-page: https://github.com/ranaroussi/yfinance
 Author: Ran Aroussi Author-email: ran@aroussi.com License: Apache Keywords:
 pandas,yahoo finance,pandas datareader Platform: any Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Topic :: Office/Business :: Financial Classifier: Topic
 :: Office/Business :: Financial :: Investment Classifier: Topic :: Scientific/
```

### Comparing `yfinance-0.2.7/yfinance.egg-info/SOURCES.txt` & `yfinance-0.2.9/yfinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*


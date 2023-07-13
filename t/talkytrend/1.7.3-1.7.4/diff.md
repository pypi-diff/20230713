# Comparing `tmp/talkytrend-1.7.3.tar.gz` & `tmp/talkytrend-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.7.3.tar", max compression
+gzip compressed data, was "talkytrend-1.7.4.tar", max compression
```

## Comparing `talkytrend-1.7.3.tar` & `talkytrend-1.7.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-12 13:59:39.697182 talkytrend-1.7.3/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-12 13:59:39.697182 talkytrend-1.7.3/README.md
--rw-r--r--   0        0        0     2476 2023-07-12 13:59:40.517257 talkytrend-1.7.3/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-12 13:59:40.517257 talkytrend-1.7.3/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-12 13:59:39.697182 talkytrend-1.7.3/talkytrend/config.py
--rw-r--r--   0        0        0     2232 2023-07-12 13:59:39.697182 talkytrend-1.7.3/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     7304 2023-07-12 13:59:39.697182 talkytrend-1.7.3/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 20:43:38.458302 talkytrend-1.7.4/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-13 20:43:38.458302 talkytrend-1.7.4/README.md
+-rw-r--r--   0        0        0     2476 2023-07-13 20:43:39.286323 talkytrend-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-13 20:43:39.290323 talkytrend-1.7.4/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-13 20:43:38.458302 talkytrend-1.7.4/talkytrend/config.py
+-rw-r--r--   0        0        0     2285 2023-07-13 20:43:38.458302 talkytrend-1.7.4/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     7304 2023-07-13 20:43:38.458302 talkytrend-1.7.4/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.4/PKG-INFO
```

### Comparing `talkytrend-1.7.3/LICENSE` & `talkytrend-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.3/README.md` & `talkytrend-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.3/pyproject.toml` & `talkytrend-1.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.7.3"
+version = "1.7.4"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.7.3/talkytrend/config.py` & `talkytrend-1.7.4/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.3/talkytrend/default_settings.toml` & `talkytrend-1.7.4/talkytrend/default_settings.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,21 @@
     # { id ="GOLD",exchange="TVC",screener="cfd", interval = "4h"},
     # { id ="USOIL",exchange="FX",screener="cfd", interval = "4h"},
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
     #use https://tvdb.brianthe.dev/ to get details
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
-fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
+fomc_decision_date = ["2023-09-20","2023-11-01","2023-12-13"]
 enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&max=2&apikey="
 news_api_key = ""
 enable_feed = true
-news_feed="http://feeds.feedburner.com/zerohedge/feed"
+#news_feed="http://feeds.feedburner.com/zerohedge/feed"
+news_feed="https://www.financialjuice.com/feed.ashx?xy=rss"
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 
 
 
 [testing]
 VALUE = "On Testing"
 talkytrend_enabled = true
@@ -55,9 +56,9 @@
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
 enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
 enable_feed = true
-news_feed="http://feeds.feedburner.com/zerohedge/feed"
+news_feed="https://www.financialjuice.com/feed.ashx?xy=rss"
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
```

### Comparing `talkytrend-1.7.3/talkytrend/main.py` & `talkytrend-1.7.4/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.3/PKG-INFO` & `talkytrend-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.7.3
+Version: 1.7.4
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.7.3 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.7.4 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```


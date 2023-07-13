# Comparing `tmp/ohlcv-plus-2.0.2.tar.gz` & `tmp/ohlcv-plus-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohlcv-plus-2.0.2.tar", last modified: Sat Jun 17 18:25:16 2023, max compression
+gzip compressed data, was "ohlcv-plus-2.0.3.tar", last modified: Thu Jul 13 14:19:52 2023, max compression
```

## Comparing `ohlcv-plus-2.0.2.tar` & `ohlcv-plus-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 18:25:16.574954 ohlcv-plus-2.0.2/
--rwxrwxrwx   0 root         (0) root         (0)     1062 2023-06-17 04:52:02.000000 ohlcv-plus-2.0.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1620 2023-06-17 18:25:16.575047 ohlcv-plus-2.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1312 2023-06-17 17:50:46.000000 ohlcv-plus-2.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 18:25:16.573308 ohlcv-plus-2.0.2/ohlcv/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.2/ohlcv/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-17 18:23:00.000000 ohlcv-plus-2.0.2/ohlcv/ohlcv.py
--rwxrwxrwx   0 root         (0) root         (0)     1649 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.2/ohlcv/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 18:25:16.574717 ohlcv-plus-2.0.2/ohlcv_plus.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1620 2023-06-17 18:25:16.000000 ohlcv-plus-2.0.2/ohlcv_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      253 2023-06-17 18:25:16.000000 ohlcv-plus-2.0.2/ohlcv_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-17 18:25:16.000000 ohlcv-plus-2.0.2/ohlcv_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-06-17 18:25:16.000000 ohlcv-plus-2.0.2/ohlcv_plus.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-17 18:25:16.000000 ohlcv-plus-2.0.2/ohlcv_plus.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-17 18:25:16.575577 ohlcv-plus-2.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      614 2023-06-17 18:25:05.000000 ohlcv-plus-2.0.2/setup.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-07-13 14:19:52.767477 ohlcv-plus-2.0.3/
+-rw-rw-r--   0 x         (1000) x         (1000)     1062 2023-07-13 03:45:08.000000 ohlcv-plus-2.0.3/LICENSE
+-rw-rw-r--   0 x         (1000) x         (1000)     1620 2023-07-13 14:19:52.767477 ohlcv-plus-2.0.3/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)     1312 2023-07-13 03:45:08.000000 ohlcv-plus-2.0.3/README.md
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-07-13 14:19:52.766477 ohlcv-plus-2.0.3/ohlcv/
+-rw-rw-r--   0 x         (1000) x         (1000)       34 2023-07-13 03:45:08.000000 ohlcv-plus-2.0.3/ohlcv/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)    15540 2023-07-13 14:16:08.000000 ohlcv-plus-2.0.3/ohlcv/ohlcv.py
+-rw-rw-r--   0 x         (1000) x         (1000)     1649 2023-07-13 03:45:08.000000 ohlcv-plus-2.0.3/ohlcv/utils.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-07-13 14:19:52.767477 ohlcv-plus-2.0.3/ohlcv_plus.egg-info/
+-rw-rw-r--   0 x         (1000) x         (1000)     1620 2023-07-13 14:19:52.000000 ohlcv-plus-2.0.3/ohlcv_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)      253 2023-07-13 14:19:52.000000 ohlcv-plus-2.0.3/ohlcv_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        1 2023-07-13 14:19:52.000000 ohlcv-plus-2.0.3/ohlcv_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 x         (1000) x         (1000)       32 2023-07-13 14:19:52.000000 ohlcv-plus-2.0.3/ohlcv_plus.egg-info/requires.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        6 2023-07-13 14:19:52.000000 ohlcv-plus-2.0.3/ohlcv_plus.egg-info/top_level.txt
+-rw-rw-r--   0 x         (1000) x         (1000)       79 2023-07-13 14:19:52.767477 ohlcv-plus-2.0.3/setup.cfg
+-rw-rw-r--   0 x         (1000) x         (1000)      614 2023-07-13 14:16:08.000000 ohlcv-plus-2.0.3/setup.py
```

### Comparing `ohlcv-plus-2.0.2/LICENSE` & `ohlcv-plus-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ohlcv-plus-2.0.2/PKG-INFO` & `ohlcv-plus-2.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohlcv-plus
-Version: 2.0.2
+Version: 2.0.3
 Summary: Crypto OHLCV data downloader.
 Home-page: https://github.com/Shaft-3796/OHLCV-Plus
 Download-URL: https://github.com/Shaft-3796/OHLCV-Plus/archive/refs/tags/2.0.0.tar.gz
 Author: Shaft
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ohlcv-plus-2.0.2/README.md` & `ohlcv-plus-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ohlcv-plus-2.0.2/ohlcv/ohlcv.py` & `ohlcv-plus-2.0.3/ohlcv/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,28 @@
 
         if verbose:
             print(Fore.CYAN, f"Aggregating {len(requests)} dataframe for a total of {limit} candles. This might take "
                              f"some time.", Fore.RESET)
         df = pd.concat([responses[i][0] for i in range(len(requests))], ignore_index=True).iloc[:-1].iloc[:limit]
         df = df.drop_duplicates(subset=['timestamp'])
         df = df.reset_index(drop=True)
+        if verbose:
+            print(Fore.CYAN, f"Verifying data integrity.", Fore.RESET)
+        ic = 0
+        for i in range(1, len(df)):
+            if df['timestamp'].iloc[i] - df['timestamp'].iloc[i - 1] != tf:
+                # Check the number of missing candles
+                missing = int((df['timestamp'].iloc[i] - df['timestamp'].iloc[i - 1]) / tf)
+                ic += missing
+
+        if ic > 0 and verbose:
+            msg = f"WARNING: Integrity check failed:\n  {ic} candles were detected as missing, this is most likely " \
+                  f"not a download issue but rather an exchange issue, some exchanges do not provide data for " \
+                  f"downtimes or other reasons."
+            print(Fore.YELLOW, msg, Fore.RESET)
         return df
 
     def update(self, dataframe: pd.DataFrame, market: str, timeframe: str, verbose: bool = True, workers: int = 100):
         """
         Update an existing dataframe with new data.
         :param dataframe: the dataframe to update.
         :param market: the market as a string e.g. 'BTC/USDT', this market must be available on the exchange.
```

### Comparing `ohlcv-plus-2.0.2/ohlcv/utils.py` & `ohlcv-plus-2.0.3/ohlcv/utils.py`

 * *Files identical despite different names*

### Comparing `ohlcv-plus-2.0.2/ohlcv_plus.egg-info/PKG-INFO` & `ohlcv-plus-2.0.3/ohlcv_plus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohlcv-plus
-Version: 2.0.2
+Version: 2.0.3
 Summary: Crypto OHLCV data downloader.
 Home-page: https://github.com/Shaft-3796/OHLCV-Plus
 Download-URL: https://github.com/Shaft-3796/OHLCV-Plus/archive/refs/tags/2.0.0.tar.gz
 Author: Shaft
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ohlcv-plus-2.0.2/setup.py` & `ohlcv-plus-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='ohlcv-plus',
-      version='2.0.2',
+      version='2.0.3',
       description='Crypto OHLCV data downloader.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Shaft',
       url='https://github.com/Shaft-3796/OHLCV-Plus',
       download_url='https://github.com/Shaft-3796/OHLCV-Plus/archive/refs/tags/2.0.0.tar.gz',
       packages=['ohlcv'],
```


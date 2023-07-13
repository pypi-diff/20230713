# Comparing `tmp/cf_clearance-0.30.0.tar.gz` & `tmp/cf_clearance-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_clearance-0.30.0.tar", last modified: Thu Jul 13 03:40:21 2023, max compression
+gzip compressed data, was "cf_clearance-0.30.1.tar", last modified: Thu Jul 13 04:03:26 2023, max compression
```

## Comparing `cf_clearance-0.30.0.tar` & `cf_clearance-0.30.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11343 2023-06-16 09:27:03.281672 cf_clearance-0.30.0/LICENSE
--rw-r--r--   0        0        0     6115 2023-07-13 03:27:14.858331 cf_clearance-0.30.0/README.md
--rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.30.0/cf_clearance/.DS_Store
--rw-r--r--   0        0        0      335 2023-07-13 03:38:20.275438 cf_clearance-0.30.0/cf_clearance/__init__.py
--rw-r--r--   0        0        0      118 2023-06-07 07:53:29.052052 cf_clearance-0.30.0/cf_clearance/errors.py
--rw-r--r--   0        0        0     1268 2023-06-07 07:53:29.052342 cf_clearance-0.30.0/cf_clearance/js/canvas.fingerprinting.js
--rw-r--r--   0        0        0     1846 2023-06-07 07:53:29.052624 cf_clearance-0.30.0/cf_clearance/js/chrome.global.js
--rw-r--r--   0        0        0     5662 2023-06-07 07:53:29.052917 cf_clearance-0.30.0/cf_clearance/js/chrome.plugin.js
--rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.30.0/cf_clearance/js/chrome.runtime.js
--rw-r--r--   0        0        0       74 2023-06-07 07:53:29.053074 cf_clearance-0.30.0/cf_clearance/js/emulate.touch.js
--rw-r--r--   0        0        0     1083 2023-06-07 07:53:29.053302 cf_clearance-0.30.0/cf_clearance/js/navigator.permissions.js
--rw-r--r--   0        0        0      489 2023-06-07 07:53:29.053552 cf_clearance-0.30.0/cf_clearance/js/navigator.webdriver.js
--rw-r--r--   0        0        0     2223 2023-07-13 03:27:14.858659 cf_clearance-0.30.0/cf_clearance/retry.py
--rw-r--r--   0        0        0     3677 2023-07-13 02:29:58.161925 cf_clearance-0.30.0/cf_clearance/stealth.py
--rw-r--r--   0        0        0     1006 2023-07-13 03:40:21.054674 cf_clearance-0.30.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.30.0/tests/__init__.py
--rw-r--r--   0        0        0     1816 2023-07-13 03:27:14.859270 cf_clearance-0.30.0/tests/test_async_cf.py
--rw-r--r--   0        0        0      715 2023-06-07 07:53:29.055195 cf_clearance-0.30.0/tests/test_common.py
--rw-r--r--   0        0        0     1361 2023-07-13 03:27:14.859553 cf_clearance-0.30.0/tests/test_cron_challenge.py
--rw-r--r--   0        0        0     1671 2023-07-13 03:27:14.859795 cf_clearance-0.30.0/tests/test_sync_cf.py
--rw-r--r--   0        0        0     6916 1970-01-01 00:00:00.000000 cf_clearance-0.30.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-16 09:27:03.281672 cf_clearance-0.30.1/LICENSE
+-rw-r--r--   0        0        0     6117 2023-07-13 03:42:57.357841 cf_clearance-0.30.1/README.md
+-rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.30.1/cf_clearance/.DS_Store
+-rw-r--r--   0        0        0      336 2023-07-13 03:41:27.148526 cf_clearance-0.30.1/cf_clearance/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-07 07:53:29.052052 cf_clearance-0.30.1/cf_clearance/errors.py
+-rw-r--r--   0        0        0     1268 2023-06-07 07:53:29.052342 cf_clearance-0.30.1/cf_clearance/js/canvas.fingerprinting.js
+-rw-r--r--   0        0        0     1846 2023-06-07 07:53:29.052624 cf_clearance-0.30.1/cf_clearance/js/chrome.global.js
+-rw-r--r--   0        0        0     5662 2023-06-07 07:53:29.052917 cf_clearance-0.30.1/cf_clearance/js/chrome.plugin.js
+-rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.30.1/cf_clearance/js/chrome.runtime.js
+-rw-r--r--   0        0        0       74 2023-06-07 07:53:29.053074 cf_clearance-0.30.1/cf_clearance/js/emulate.touch.js
+-rw-r--r--   0        0        0     1083 2023-06-07 07:53:29.053302 cf_clearance-0.30.1/cf_clearance/js/navigator.permissions.js
+-rw-r--r--   0        0        0      489 2023-06-07 07:53:29.053552 cf_clearance-0.30.1/cf_clearance/js/navigator.webdriver.js
+-rw-r--r--   0        0        0     2285 2023-07-13 04:01:31.970692 cf_clearance-0.30.1/cf_clearance/retry.py
+-rw-r--r--   0        0        0     3677 2023-07-13 02:29:58.161925 cf_clearance-0.30.1/cf_clearance/stealth.py
+-rw-r--r--   0        0        0     1006 2023-07-13 04:03:26.339413 cf_clearance-0.30.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.30.1/tests/__init__.py
+-rw-r--r--   0        0        0     1816 2023-07-13 03:27:14.859270 cf_clearance-0.30.1/tests/test_async_cf.py
+-rw-r--r--   0        0        0      715 2023-06-07 07:53:29.055195 cf_clearance-0.30.1/tests/test_common.py
+-rw-r--r--   0        0        0     1020 2023-07-13 04:01:41.773088 cf_clearance-0.30.1/tests/test_cron_challenge.py
+-rw-r--r--   0        0        0     1671 2023-07-13 03:27:14.859795 cf_clearance-0.30.1/tests/test_sync_cf.py
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 cf_clearance-0.30.1/PKG-INFO
```

### Comparing `cf_clearance-0.30.0/LICENSE` & `cf_clearance-0.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/README.md` & `cf_clearance-0.30.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 import requests
 
 proxy = "socks5://localhost:7890"
 resp = requests.post("http://localhost:8000/challenge",
                      json={"proxy": {"server": proxy}, "timeout": 20,
                            "url": "https://nowsecure.nl"})
 data = resp.json()
-# In some cases, the cloudflare challenge will not be triggered, so when cf in the return parameter is true, it means that the challenge has been encountered.
+# In some cases, the cloudflare challenge will not be triggered,
+# so when cf in the return parameter is true, it means that the challenge has been encountered.
 if data.get("success") and data.get("cf"):
     ua = data.get("user_agent")
     cf_clearance_value = data.get("cookies").get("cf_clearance")
     # use cf_clearance, must be same IP and UA
     headers = {"user-agent": ua}
     cookies = {"cf_clearance": cf_clearance_value}
     res = requests.get('https://nowsecure.nl', proxies={
```

### Comparing `cf_clearance-0.30.0/cf_clearance/.DS_Store` & `cf_clearance-0.30.1/cf_clearance/.DS_Store`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/cf_clearance/js/canvas.fingerprinting.js` & `cf_clearance-0.30.1/cf_clearance/js/canvas.fingerprinting.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/cf_clearance/js/chrome.global.js` & `cf_clearance-0.30.1/cf_clearance/js/chrome.global.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/cf_clearance/js/chrome.plugin.js` & `cf_clearance-0.30.1/cf_clearance/js/chrome.plugin.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/cf_clearance/js/chrome.runtime.js` & `cf_clearance-0.30.1/cf_clearance/js/chrome.runtime.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/cf_clearance/js/navigator.permissions.js` & `cf_clearance-0.30.1/cf_clearance/js/navigator.permissions.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/cf_clearance/retry.py` & `cf_clearance-0.30.1/cf_clearance/retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from playwright.async_api import Page as AsyncPage
 from playwright.sync_api import Page as SyncPage
 
 
 async def async_cf_retry(page: AsyncPage, tries: int = 10) -> Tuple[bool, bool]:
     success = False
     cf = True
+    user_tries = tries
     while tries > 0:
         await page.wait_for_timeout(1500)
         try:
             success = False if await page.query_selector("#challenge-form") else True
             if success:
                 break
             simple_challenge = await page.query_selector(
@@ -26,22 +27,23 @@
                         "xpath=//input[@type='checkbox']"
                     )
                     if click:
                         await click.click()
         except Error:
             success = False
         tries -= 1
-    if tries == 10:
+    if tries == user_tries:
         cf = False
     return success, cf
 
 
 def sync_cf_retry(page: SyncPage, tries: int = 10) -> Tuple[bool, bool]:
     success = False
     cf = True
+    user_tries = tries
     while tries > 0:
         page.wait_for_timeout(1500)
         try:
             success = False if page.query_selector("#challenge-form") else True
             if success:
                 break
             simple_challenge = page.query_selector(
@@ -55,10 +57,10 @@
                         "xpath=//input[@type='checkbox']"
                     )
                     if click:
                         click.click()
         except Error:
             success = False
         tries -= 1
-    if tries == 10:
+    if tries == user_tries:
         cf = False
     return success, cf
```

### Comparing `cf_clearance-0.30.0/cf_clearance/stealth.py` & `cf_clearance-0.30.1/cf_clearance/stealth.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/pyproject.toml` & `cf_clearance-0.30.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cf_clearance"
-version = "0.30.0"
+version = "0.30.1"
 description = "Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with the cf_clearance, make sure you use the same IP and UA as when you got it."
 authors = [
     { name = "vvanglro", email = "vvanglro@gmail.com" },
 ]
 dependencies = [
     "playwright",
 ]
```

### Comparing `cf_clearance-0.30.0/tests/test_async_cf.py` & `cf_clearance-0.30.1/tests/test_async_cf.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/tests/test_common.py` & `cf_clearance-0.30.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/tests/test_sync_cf.py` & `cf_clearance-0.30.1/tests/test_sync_cf.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.30.0/PKG-INFO` & `cf_clearance-0.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_clearance
-Version: 0.30.0
+Version: 0.30.1
 Summary: Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with the cf_clearance, make sure you use the same IP and UA as when you got it.
 Author-Email: vvanglro <vvanglro@gmail.com>
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -56,15 +56,16 @@
 import requests
 
 proxy = "socks5://localhost:7890"
 resp = requests.post("http://localhost:8000/challenge",
                      json={"proxy": {"server": proxy}, "timeout": 20,
                            "url": "https://nowsecure.nl"})
 data = resp.json()
-# In some cases, the cloudflare challenge will not be triggered, so when cf in the return parameter is true, it means that the challenge has been encountered.
+# In some cases, the cloudflare challenge will not be triggered,
+# so when cf in the return parameter is true, it means that the challenge has been encountered.
 if data.get("success") and data.get("cf"):
     ua = data.get("user_agent")
     cf_clearance_value = data.get("cookies").get("cf_clearance")
     # use cf_clearance, must be same IP and UA
     headers = {"user-agent": ua}
     cookies = {"cf_clearance": cf_clearance_value}
     res = requests.get('https://nowsecure.nl', proxies={
```


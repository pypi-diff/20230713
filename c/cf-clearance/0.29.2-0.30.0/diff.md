# Comparing `tmp/cf_clearance-0.29.2.tar.gz` & `tmp/cf_clearance-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_clearance-0.29.2.tar", last modified: Fri Jun  9 04:16:31 2023, max compression
+gzip compressed data, was "cf_clearance-0.30.0.tar", last modified: Thu Jul 13 03:40:21 2023, max compression
```

## Comparing `cf_clearance-0.29.2.tar` & `cf_clearance-0.30.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2022-05-30 06:44:14.187456 cf_clearance-0.29.2/LICENSE
--rw-r--r--   0        0        0     5689 2023-06-07 07:53:29.051659 cf_clearance-0.29.2/README.md
--rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.29.2/cf_clearance/.DS_Store
--rw-r--r--   0        0        0      281 2023-06-09 04:15:48.860878 cf_clearance-0.29.2/cf_clearance/__init__.py
--rw-r--r--   0        0        0      118 2023-06-07 07:53:29.052052 cf_clearance-0.29.2/cf_clearance/errors.py
--rw-r--r--   0        0        0     1268 2023-06-07 07:53:29.052342 cf_clearance-0.29.2/cf_clearance/js/canvas.fingerprinting.js
--rw-r--r--   0        0        0     1846 2023-06-07 07:53:29.052624 cf_clearance-0.29.2/cf_clearance/js/chrome.global.js
--rw-r--r--   0        0        0     5662 2023-06-07 07:53:29.052917 cf_clearance-0.29.2/cf_clearance/js/chrome.plugin.js
--rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.29.2/cf_clearance/js/chrome.runtime.js
--rw-r--r--   0        0        0       74 2023-06-07 07:53:29.053074 cf_clearance-0.29.2/cf_clearance/js/emulate.touch.js
--rw-r--r--   0        0        0     1083 2023-06-07 07:53:29.053302 cf_clearance-0.29.2/cf_clearance/js/navigator.permissions.js
--rw-r--r--   0        0        0      489 2023-06-07 07:53:29.053552 cf_clearance-0.29.2/cf_clearance/js/navigator.webdriver.js
--rw-r--r--   0        0        0     2058 2023-06-07 07:53:29.053700 cf_clearance-0.29.2/cf_clearance/retry.py
--rw-r--r--   0        0        0     3678 2023-06-07 07:53:29.053841 cf_clearance-0.29.2/cf_clearance/stealth.py
--rw-r--r--   0        0        0     1060 2023-06-09 04:16:31.938178 cf_clearance-0.29.2/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.29.2/tests/__init__.py
--rw-r--r--   0        0        0     1805 2023-06-07 07:53:29.055046 cf_clearance-0.29.2/tests/test_async_cf.py
--rw-r--r--   0        0        0      715 2023-06-07 07:53:29.055195 cf_clearance-0.29.2/tests/test_common.py
--rw-r--r--   0        0        0      838 2023-06-07 07:53:29.055295 cf_clearance-0.29.2/tests/test_cron_challenge.py
--rw-r--r--   0        0        0     1660 2023-06-07 07:53:29.055526 cf_clearance-0.29.2/tests/test_sync_cf.py
--rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 cf_clearance-0.29.2/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-16 09:27:03.281672 cf_clearance-0.30.0/LICENSE
+-rw-r--r--   0        0        0     6115 2023-07-13 03:27:14.858331 cf_clearance-0.30.0/README.md
+-rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.30.0/cf_clearance/.DS_Store
+-rw-r--r--   0        0        0      335 2023-07-13 03:38:20.275438 cf_clearance-0.30.0/cf_clearance/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-07 07:53:29.052052 cf_clearance-0.30.0/cf_clearance/errors.py
+-rw-r--r--   0        0        0     1268 2023-06-07 07:53:29.052342 cf_clearance-0.30.0/cf_clearance/js/canvas.fingerprinting.js
+-rw-r--r--   0        0        0     1846 2023-06-07 07:53:29.052624 cf_clearance-0.30.0/cf_clearance/js/chrome.global.js
+-rw-r--r--   0        0        0     5662 2023-06-07 07:53:29.052917 cf_clearance-0.30.0/cf_clearance/js/chrome.plugin.js
+-rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.30.0/cf_clearance/js/chrome.runtime.js
+-rw-r--r--   0        0        0       74 2023-06-07 07:53:29.053074 cf_clearance-0.30.0/cf_clearance/js/emulate.touch.js
+-rw-r--r--   0        0        0     1083 2023-06-07 07:53:29.053302 cf_clearance-0.30.0/cf_clearance/js/navigator.permissions.js
+-rw-r--r--   0        0        0      489 2023-06-07 07:53:29.053552 cf_clearance-0.30.0/cf_clearance/js/navigator.webdriver.js
+-rw-r--r--   0        0        0     2223 2023-07-13 03:27:14.858659 cf_clearance-0.30.0/cf_clearance/retry.py
+-rw-r--r--   0        0        0     3677 2023-07-13 02:29:58.161925 cf_clearance-0.30.0/cf_clearance/stealth.py
+-rw-r--r--   0        0        0     1006 2023-07-13 03:40:21.054674 cf_clearance-0.30.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.30.0/tests/__init__.py
+-rw-r--r--   0        0        0     1816 2023-07-13 03:27:14.859270 cf_clearance-0.30.0/tests/test_async_cf.py
+-rw-r--r--   0        0        0      715 2023-06-07 07:53:29.055195 cf_clearance-0.30.0/tests/test_common.py
+-rw-r--r--   0        0        0     1361 2023-07-13 03:27:14.859553 cf_clearance-0.30.0/tests/test_cron_challenge.py
+-rw-r--r--   0        0        0     1671 2023-07-13 03:27:14.859795 cf_clearance-0.30.0/tests/test_sync_cf.py
+-rw-r--r--   0        0        0     6916 1970-01-01 00:00:00.000000 cf_clearance-0.30.0/PKG-INFO
```

### Comparing `cf_clearance-0.29.2/LICENSE` & `cf_clearance-0.30.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2021-2023 vvanglro
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cf_clearance-0.29.2/README.md` & `cf_clearance-0.30.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,19 @@
 ```python
 import requests
 
 proxy = "socks5://localhost:7890"
 resp = requests.post("http://localhost:8000/challenge",
                      json={"proxy": {"server": proxy}, "timeout": 20,
                            "url": "https://nowsecure.nl"})
-if resp.json().get("success"):
-    ua = resp.json().get("user_agent")
-    cf_clearance_value = resp.json().get("cookies").get("cf_clearance")
+data = resp.json()
+# In some cases, the cloudflare challenge will not be triggered, so when cf in the return parameter is true, it means that the challenge has been encountered.
+if data.get("success") and data.get("cf"):
+    ua = data.get("user_agent")
+    cf_clearance_value = data.get("cookies").get("cf_clearance")
     # use cf_clearance, must be same IP and UA
     headers = {"user-agent": ua}
     cookies = {"cf_clearance": cf_clearance_value}
     res = requests.get('https://nowsecure.nl', proxies={
         "all": proxy
     }, headers=headers, cookies=cookies)
     if '<title>Just a moment...</title>' not in res.text:
@@ -89,25 +91,28 @@
     print("cf challenge fail")
 # get cf_clearance
 with sync_playwright() as p:
     browser = p.chromium.launch(headless=False, proxy={"server": "socks5://localhost:7890"})
     page = browser.new_page()
     sync_stealth(page, pure=True)
     page.goto('https://nowsecure.nl')
-    res = sync_cf_retry(page)
-    if res:
-        cookies = page.context.cookies()
-        for cookie in cookies:
-            if cookie.get('name') == 'cf_clearance':
-                cf_clearance_value = cookie.get('value')
-                print(cf_clearance_value)
-        ua = page.evaluate('() => {return navigator.userAgent}')
-        print(ua)
+    res, cf = sync_cf_retry(page)
+    if cf:
+        if res:
+            cookies = page.context.cookies()
+            for cookie in cookies:
+                if cookie.get('name') == 'cf_clearance':
+                    cf_clearance_value = cookie.get('value')
+                    print(cf_clearance_value)
+            ua = page.evaluate('() => {return navigator.userAgent}')
+            print(ua)
+        else:
+            print("cf challenge fail")
     else:
-        print("cf challenge fail")
+        print("No cloudflare challenges encountered")
     browser.close()
 # use cf_clearance, must be same IP and UA
 headers = {"user-agent": ua}
 cookies = {"cf_clearance": cf_clearance_value}
 res = requests.get('https://nowsecure.nl', proxies=proxies, headers=headers, cookies=cookies)
 if '<title>Just a moment...</title>' not in res.text:
     print("cf challenge success")
@@ -132,25 +137,28 @@
         print("cf challenge fail")
     # get cf_clearance
     async with async_playwright() as p:
         browser = await p.chromium.launch(headless=False, proxy={"server": "socks5://localhost:7890"})
         page = await browser.new_page()
         await async_stealth(page, pure=True)
         await page.goto('https://nowsecure.nl')
-        res = await async_cf_retry(page)
-        if res:
-            cookies = await page.context.cookies()
-            for cookie in cookies:
-                if cookie.get('name') == 'cf_clearance':
-                    cf_clearance_value = cookie.get('value')
-                    print(cf_clearance_value)
-            ua = await page.evaluate('() => {return navigator.userAgent}')
-            print(ua)
+        res, cf = await async_cf_retry(page)
+        if cf:
+            if res:
+                cookies = await page.context.cookies()
+                for cookie in cookies:
+                    if cookie.get('name') == 'cf_clearance':
+                        cf_clearance_value = cookie.get('value')
+                        print(cf_clearance_value)
+                ua = await page.evaluate('() => {return navigator.userAgent}')
+                print(ua)
+            else:
+                print("cf challenge fail")
         else:
-            print("cf challenge fail")
+            print("No cloudflare challenges encountered")
         await browser.close()
     # use cf_clearance, must be same IP and UA
     headers = {"user-agent": ua}
     cookies = {"cf_clearance": cf_clearance_value}
     res = requests.get('https://nowsecure.nl', proxies=proxies, headers=headers, cookies=cookies)
     if '<title>Just a moment...</title>' not in res.text:
         print("cf challenge success")
```

### Comparing `cf_clearance-0.29.2/cf_clearance/.DS_Store` & `cf_clearance-0.30.0/cf_clearance/.DS_Store`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.2/cf_clearance/js/canvas.fingerprinting.js` & `cf_clearance-0.30.0/cf_clearance/js/canvas.fingerprinting.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.2/cf_clearance/js/chrome.global.js` & `cf_clearance-0.30.0/cf_clearance/js/chrome.global.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.2/cf_clearance/js/chrome.plugin.js` & `cf_clearance-0.30.0/cf_clearance/js/chrome.plugin.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.2/cf_clearance/js/chrome.runtime.js` & `cf_clearance-0.30.0/cf_clearance/js/chrome.runtime.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.2/cf_clearance/js/navigator.permissions.js` & `cf_clearance-0.30.0/cf_clearance/js/navigator.permissions.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.2/cf_clearance/retry.py` & `cf_clearance-0.30.0/cf_clearance/retry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
+from typing import Tuple
+
 from playwright.async_api import Error
 from playwright.async_api import Page as AsyncPage
 from playwright.sync_api import Page as SyncPage
 
 
-async def async_cf_retry(page: AsyncPage, tries: int = 10) -> bool:
+async def async_cf_retry(page: AsyncPage, tries: int = 10) -> Tuple[bool, bool]:
     success = False
+    cf = True
     while tries > 0:
         await page.wait_for_timeout(1500)
         try:
             success = False if await page.query_selector("#challenge-form") else True
             if success:
                 break
             simple_challenge = await page.query_selector(
@@ -23,19 +26,22 @@
                         "xpath=//input[@type='checkbox']"
                     )
                     if click:
                         await click.click()
         except Error:
             success = False
         tries -= 1
-    return success
+    if tries == 10:
+        cf = False
+    return success, cf
 
 
-def sync_cf_retry(page: SyncPage, tries: int = 10) -> bool:
+def sync_cf_retry(page: SyncPage, tries: int = 10) -> Tuple[bool, bool]:
     success = False
+    cf = True
     while tries > 0:
         page.wait_for_timeout(1500)
         try:
             success = False if page.query_selector("#challenge-form") else True
             if success:
                 break
             simple_challenge = page.query_selector(
@@ -49,9 +55,10 @@
                         "xpath=//input[@type='checkbox']"
                     )
                     if click:
                         click.click()
         except Error:
             success = False
         tries -= 1
-
-    return success
+    if tries == 10:
+        cf = False
+    return success, cf
```

### Comparing `cf_clearance-0.29.2/cf_clearance/stealth.py` & `cf_clearance-0.30.0/cf_clearance/stealth.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     navigator_permissions: bool = True
     navigator_webdriver: bool = True
     chrome_runtime: bool = True
     chrome_plugin: bool = True
 
     @property
     def enabled_scripts(self):
-
         if self.chrome_fp:
             yield SCRIPTS["chrome_fp"]
         if self.chrome_global:
             yield SCRIPTS["chrome_global"]
         if self.chrome_touch:
             yield SCRIPTS["chrome_touch"]
         if self.navigator_permissions:
```

### Comparing `cf_clearance-0.29.2/pyproject.toml` & `cf_clearance-0.30.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [project]
 name = "cf_clearance"
-version = "0.29.2"
+version = "0.30.0"
 description = "Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with the cf_clearance, make sure you use the same IP and UA as when you got it."
 authors = [
     { name = "vvanglro", email = "vvanglro@gmail.com" },
 ]
 dependencies = [
-    "playwright>=1.34.0",
+    "playwright",
 ]
-requires-python = ">=3.7,<4"
+requires-python = ">=3.8,<4"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.license]
@@ -30,12 +29,12 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pre-commit>=2.21.0",
+    "pre-commit>=3.3.3",
 ]
 
 [tool.ruff]
 line-length = 120
```

### Comparing `cf_clearance-0.29.2/tests/test_async_cf.py` & `cf_clearance-0.30.0/tests/test_async_cf.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
                 "--start-maximized",
             ],
         )
         content = await browser.new_context(no_viewport=True)
         page = await content.new_page()
         await async_stealth(page, pure=True)
         await page.goto("https://nowsecure.nl")
-        res = await async_cf_retry(page)
+        res, cf = await async_cf_retry(page)
         ua = None
         cf_clearance_value = None
-        if res:
+        if res and cf:
             cookies = await page.context.cookies()
             for cookie in cookies:
                 if cookie.get("name") == "cf_clearance":
                     cf_clearance_value = cookie.get("value")
             ua = await page.evaluate("() => {return navigator.userAgent}")
         else:
             logging.info("cf challenge fail")
```

### Comparing `cf_clearance-0.29.2/tests/test_common.py` & `cf_clearance-0.30.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.2/tests/test_cron_challenge.py` & `cf_clearance-0.30.0/tests/test_cron_challenge.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 from playwright.async_api import async_playwright
 
 from cf_clearance import async_cf_retry, async_stealth
 
 
 async def test_cf_challenge(url: str):
     async with async_playwright() as p:
-        browser = await p.chromium.launch(headless=False)
+        browser = await p.chromium.launch(
+            headless=False,
+            args=[
+                "--disable-gpu",
+                "--no-sandbox",
+                "--disable-dev-shm-usage",
+                "--no-first-run",
+                "--no-service-autorun",
+                "--no-default-browser-check",
+                "--password-store=basic",
+                "--start-maximized",
+            ],
+        )
         context = await browser.new_context()
         page = await context.new_page()
         await async_stealth(page, pure=True)
         await page.goto(url)
-        res = await async_cf_retry(page)
-        if res:
-            cookies = await page.context.cookies()
-            for cookie in cookies:
-                if cookie.get("name") == "cf_clearance":
-                    cf_clearance_value = cookie.get("value")
-        assert cf_clearance_value
+        res, cf = await async_cf_retry(page)
+        if cf:
+            if res:
+                cookies = await page.context.cookies()
+                for cookie in cookies:
+                    if cookie.get("name") == "cf_clearance":
+                        cf_clearance_value = cookie.get("value")
+                assert cf_clearance_value
+            else:
+                raise
+        else:
+            print("No cloudflare challenges encountered")
         await browser.close()
 
 
 if __name__ == "__main__":
     import asyncio
 
     asyncio.run(test_cf_challenge("https://nowsecure.nl"))
```

### Comparing `cf_clearance-0.29.2/tests/test_sync_cf.py` & `cf_clearance-0.30.0/tests/test_sync_cf.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
                 "--start-maximized",
             ],
         )
         content = browser.new_context(no_viewport=True)
         page = content.new_page()
         sync_stealth(page, pure=True)
         page.goto("https://nowsecure.nl")
-        res = sync_cf_retry(page)
+        res, cf = sync_cf_retry(page)
         ua = None
         cf_clearance_value = None
-        if res:
+        if res and cf:
             cookies = page.context.cookies()
             for cookie in cookies:
                 if cookie.get("name") == "cf_clearance":
                     cf_clearance_value = cookie.get("value")
             ua = page.evaluate("() => {return navigator.userAgent}")
         else:
             logging.info("cf challenge fail")
```

### Comparing `cf_clearance-0.29.2/PKG-INFO` & `cf_clearance-0.30.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: cf-clearance
-Version: 0.29.2
+Name: cf_clearance
+Version: 0.30.0
 Summary: Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with the cf_clearance, make sure you use the same IP and UA as when you got it.
 Author-Email: vvanglro <vvanglro@gmail.com>
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://github.com/vvanglro/cf_clearance
 Project-URL: Repository, https://github.com/vvanglro/cf_clearance
-Requires-Python: <4,>=3.7
-Requires-Dist: playwright>=1.34.0
+Requires-Python: <4,>=3.8
+Requires-Dist: playwright
 Description-Content-Type: text/markdown
 
 # cf-clearance
 
 [![OSCS Status](https://www.oscs1024.com/platform/badge/vvanglro/cf_clearance.svg?size=small)](https://www.oscs1024.com/project/vvanglro/cf_clearance?ref=badge_small)
 [![Package version](https://img.shields.io/pypi/v/cf_clearance?color=%2334D058&label=pypi%20package)](https://pypi.python.org/pypi/cf_clearance)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cf_clearance.svg?color=%2334D058)](https://pypi.python.org/pypi/cf_clearance)
@@ -56,17 +55,19 @@
 ```python
 import requests
 
 proxy = "socks5://localhost:7890"
 resp = requests.post("http://localhost:8000/challenge",
                      json={"proxy": {"server": proxy}, "timeout": 20,
                            "url": "https://nowsecure.nl"})
-if resp.json().get("success"):
-    ua = resp.json().get("user_agent")
-    cf_clearance_value = resp.json().get("cookies").get("cf_clearance")
+data = resp.json()
+# In some cases, the cloudflare challenge will not be triggered, so when cf in the return parameter is true, it means that the challenge has been encountered.
+if data.get("success") and data.get("cf"):
+    ua = data.get("user_agent")
+    cf_clearance_value = data.get("cookies").get("cf_clearance")
     # use cf_clearance, must be same IP and UA
     headers = {"user-agent": ua}
     cookies = {"cf_clearance": cf_clearance_value}
     res = requests.get('https://nowsecure.nl', proxies={
         "all": proxy
     }, headers=headers, cookies=cookies)
     if '<title>Just a moment...</title>' not in res.text:
@@ -107,25 +108,28 @@
     print("cf challenge fail")
 # get cf_clearance
 with sync_playwright() as p:
     browser = p.chromium.launch(headless=False, proxy={"server": "socks5://localhost:7890"})
     page = browser.new_page()
     sync_stealth(page, pure=True)
     page.goto('https://nowsecure.nl')
-    res = sync_cf_retry(page)
-    if res:
-        cookies = page.context.cookies()
-        for cookie in cookies:
-            if cookie.get('name') == 'cf_clearance':
-                cf_clearance_value = cookie.get('value')
-                print(cf_clearance_value)
-        ua = page.evaluate('() => {return navigator.userAgent}')
-        print(ua)
+    res, cf = sync_cf_retry(page)
+    if cf:
+        if res:
+            cookies = page.context.cookies()
+            for cookie in cookies:
+                if cookie.get('name') == 'cf_clearance':
+                    cf_clearance_value = cookie.get('value')
+                    print(cf_clearance_value)
+            ua = page.evaluate('() => {return navigator.userAgent}')
+            print(ua)
+        else:
+            print("cf challenge fail")
     else:
-        print("cf challenge fail")
+        print("No cloudflare challenges encountered")
     browser.close()
 # use cf_clearance, must be same IP and UA
 headers = {"user-agent": ua}
 cookies = {"cf_clearance": cf_clearance_value}
 res = requests.get('https://nowsecure.nl', proxies=proxies, headers=headers, cookies=cookies)
 if '<title>Just a moment...</title>' not in res.text:
     print("cf challenge success")
@@ -150,25 +154,28 @@
         print("cf challenge fail")
     # get cf_clearance
     async with async_playwright() as p:
         browser = await p.chromium.launch(headless=False, proxy={"server": "socks5://localhost:7890"})
         page = await browser.new_page()
         await async_stealth(page, pure=True)
         await page.goto('https://nowsecure.nl')
-        res = await async_cf_retry(page)
-        if res:
-            cookies = await page.context.cookies()
-            for cookie in cookies:
-                if cookie.get('name') == 'cf_clearance':
-                    cf_clearance_value = cookie.get('value')
-                    print(cf_clearance_value)
-            ua = await page.evaluate('() => {return navigator.userAgent}')
-            print(ua)
+        res, cf = await async_cf_retry(page)
+        if cf:
+            if res:
+                cookies = await page.context.cookies()
+                for cookie in cookies:
+                    if cookie.get('name') == 'cf_clearance':
+                        cf_clearance_value = cookie.get('value')
+                        print(cf_clearance_value)
+                ua = await page.evaluate('() => {return navigator.userAgent}')
+                print(ua)
+            else:
+                print("cf challenge fail")
         else:
-            print("cf challenge fail")
+            print("No cloudflare challenges encountered")
         await browser.close()
     # use cf_clearance, must be same IP and UA
     headers = {"user-agent": ua}
     cookies = {"cf_clearance": cf_clearance_value}
     res = requests.get('https://nowsecure.nl', proxies=proxies, headers=headers, cookies=cookies)
     if '<title>Just a moment...</title>' not in res.text:
         print("cf challenge success")
```


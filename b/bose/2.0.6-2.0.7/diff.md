# Comparing `tmp/bose-2.0.6.tar.gz` & `tmp/bose-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-2.0.6.tar", last modified: Thu Jul  6 12:05:39 2023, max compression
+gzip compressed data, was "bose-2.0.7.tar", last modified: Thu Jul 13 15:37:04 2023, max compression
```

## Comparing `bose-2.0.6.tar` & `bose-2.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:05:39.350177 bose-2.0.6/
--rw-rw-rw-   0        0        0    14120 2023-07-06 12:05:39.389114 bose-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    10357 2023-07-06 11:59:35.580609 bose-2.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 12:05:39.350177 bose-2.0.6/bose/
--rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.6/bose/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.6/bose/account_generator.py
--rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.6/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.6/bose/base_data.py
--rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.6/bose/base_task.py
--rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.6/bose/beep_utils.py
--rw-rw-rw-   0        0        0    10372 2023-07-06 11:45:35.506166 bose-2.0.6/bose/bose_driver.py
--rw-rw-rw-   0        0        0    10384 2023-07-06 11:56:35.717259 bose-2.0.6/bose/bose_undetected_driver.py
--rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.6/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.6/bose/download_driver.py
--rw-rw-rw-   0        0        0      993 2023-07-06 10:42:02.261172 bose-2.0.6/bose/ip_utils.py
--rw-rw-rw-   0        0        0     2995 2023-07-01 18:25:25.812969 bose-2.0.6/bose/launch_tasks.py
--rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.6/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.6/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.6/bose/opponent.py
--rw-rw-rw-   0        0        0     2558 2023-07-05 08:58:01.580924 bose-2.0.6/bose/output.py
--rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.6/bose/profile.py
--rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.6/bose/schedule_utils.py
--rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.6/bose/task_config.py
--rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.6/bose/task_info.py
--rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.6/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.6/bose/user_agent.py
--rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.6/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.6/bose/wait.py
--rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.6/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-07-06 12:00:05.333647 bose-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:37:04.916600 bose-2.0.7/
+-rw-rw-rw-   0        0        0    14120 2023-07-13 15:37:04.916600 bose-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10357 2023-07-06 11:59:35.580609 bose-2.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-13 15:37:04.916600 bose-2.0.7/bose/
+-rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.7/bose/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.7/bose/account_generator.py
+-rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.7/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.7/bose/base_data.py
+-rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.7/bose/base_task.py
+-rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.7/bose/beep_utils.py
+-rw-rw-rw-   0        0        0    10586 2023-07-13 15:33:35.445633 bose-2.0.7/bose/bose_driver.py
+-rw-rw-rw-   0        0        0    10384 2023-07-06 11:56:35.717259 bose-2.0.7/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.7/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.7/bose/download_driver.py
+-rw-rw-rw-   0        0        0      993 2023-07-06 10:42:02.261172 bose-2.0.7/bose/ip_utils.py
+-rw-rw-rw-   0        0        0     3040 2023-07-09 14:30:45.891095 bose-2.0.7/bose/launch_tasks.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.7/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.7/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.7/bose/opponent.py
+-rw-rw-rw-   0        0        0     3130 2023-07-11 16:45:26.788592 bose-2.0.7/bose/output.py
+-rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.7/bose/profile.py
+-rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.7/bose/schedule_utils.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.7/bose/task_config.py
+-rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.7/bose/task_info.py
+-rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.7/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.7/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.7/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.7/bose/wait.py
+-rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.7/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-07-13 15:36:43.101330 bose-2.0.7/setup.py
```

### Comparing `bose-2.0.6/PKG-INFO` & `bose-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 2.0.6
+Version: 2.0.7
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-2.0.6/README.rst` & `bose-2.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/account_generator.py` & `bose-2.0.7/bose/account_generator.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/analytics.py` & `bose-2.0.7/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/base_data.py` & `bose-2.0.7/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/base_task.py` & `bose-2.0.7/bose/base_task.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/bose_driver.py` & `bose-2.0.7/bose/bose_undetected_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import traceback
-from datetime import datetime
-from selenium import webdriver
+from undetected_chromedriver import Chrome
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 import random
 from time import sleep
 from .beep_utils import beep_input
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
 from .utils import relative_path, sleep_for_n_seconds, sleep_forever
+from datetime import datetime
 
 
-class BoseDriver(webdriver.Chrome):
+class BoseUndetectedDriver(Chrome):
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
```

### Comparing `bose-2.0.6/bose/bose_undetected_driver.py` & `bose-2.0.7/bose/bose_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import traceback
-from undetected_chromedriver import Chrome
+from datetime import datetime
+from selenium import webdriver
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 import random
 from time import sleep
 from .beep_utils import beep_input
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
 from .utils import relative_path, sleep_for_n_seconds, sleep_forever
-from datetime import datetime
 
 
-class BoseUndetectedDriver(Chrome):
+class BoseDriver(webdriver.Chrome):
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
@@ -124,25 +124,27 @@
         except:
             return None
 
     def scroll_site(self):
         self.execute_script(""" 
 window.scrollBy(0, 10000);
 """)
+        
+    def can_element_be_scrolled(self, element):
+        # <=3 is a fix to handle floating point numbers
+        result = not (self.execute_script(
+            "return Math.abs(arguments[0].scrollTop - (arguments[0].scrollHeight - arguments[0].offsetHeight)) <= 3", element))
+        return result
 
     def scroll_element(self, element):
-
-        did_element_scroll = self.execute_script(
-            "return Math.round(arguments[0].scrollTop) === Math.round(Math.round(arguments[0].scrollHeight) - Math.round(arguments[0].offsetHeight))", element)
-
-        if did_element_scroll:
-            return False
-        else:
+        if self.can_element_be_scrolled(element):
             self.execute_script("arguments[0].scrollBy(0, 10000)", element)
             return True
+        else:
+            return False
 
     def get_cookies_dict(self):
         all_cookies = self.get_cookies()
         cookies_dict = {}
         for cookie in all_cookies:
             cookies_dict[cookie['name']] = cookie['value']
         return cookies_dict
@@ -265,14 +267,19 @@
         if raise_exception:
             raise Exception(f"Page {target} not found")
         return False
 
 
     def save_screenshot(self, filename=datetime.now().strftime('%Y-%m-%d_%H-%M-%S') + ".png"):
         try:
+
+
+            if not filename.endswith(".png"):
+                filename = filename + ".png"
+
             saving_screenshot_at = relative_path(
                 f'{self.task_path}/{filename}', 0)
             self.get_screenshot_as_file(
                 saving_screenshot_at)
         except:
             traceback.print_exc()
             print('Failed to save screenshot')
```

### Comparing `bose-2.0.6/bose/create_driver.py` & `bose-2.0.7/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/download_driver.py` & `bose-2.0.7/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/ip_utils.py` & `bose-2.0.7/bose/ip_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/launch_tasks.py` & `bose-2.0.7/bose/launch_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 
 def launch_tasks(*tasks):
     for Task in tasks: 
         print('Task Started')
 
         task  = Task()
         task_config = task.get_task_config()
+        data = task.get_data()
+        if type(data) is not list:
+            data = [data]
 
         should_first_beep = len(tasks) > 1
 
-        if task_config.prompt_to_close_browser: 
-            prompt_message = f"Kindly close other browsers where {task_config.target_website} is open to prevent detection from {task_config.target_website} and press enter to continue..."
-            beep_input(prompt_message, task_config.beep and should_first_beep)
-
-        if task_config.change_ip: 
-            prompt_change_ip(task_config.beep and should_first_beep)
+        if len(data) > 0:
+            if task_config.prompt_to_close_browser: 
+                prompt_message = f"Kindly close other browsers where {task_config.target_website} is open to prevent detection from {task_config.target_website} and press enter to continue..."
+                beep_input(prompt_message, task_config.beep and should_first_beep)
 
-        data = task.get_data()
+            if task_config.change_ip: 
+                prompt_change_ip(task_config.beep and should_first_beep)
         
-        if type(data) is not list:
-            data = [data]
         
         schedules = task.schedule(data)
 
         output = []
         for index in range(len(data)):
             current_data = data[index]
             delay = schedules[index]['delay']
```

### Comparing `bose-2.0.6/bose/local_storage.py` & `bose-2.0.7/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/local_storage_driver.py` & `bose-2.0.7/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/output.py` & `bose-2.0.7/bose/output.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import csv
-from .utils import relative_path, write_json, read_json
+from .utils import relative_path, write_json, read_json, write_html
 
 class Output:
 
     def read_json(filename):
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
@@ -76,8 +76,31 @@
             # Save the image in the output directory
             path = f'{output_dir}/{filename}'
             with open(relative_path(
                 path, 0), "wb") as f:
                 f.write(response.content)
         else:
             print("Failed to download the image.")
-            return path
+            return path
+        
+    def write_html(data, filename):
+        if not filename.startswith("output/"):
+            filename = "output/" +  filename
+
+        if not filename.endswith(".html"):
+            filename = filename + ".html"
+
+        write_html(data, filename)
+        print(f"View written HTML file at {filename}")
+
+
+
+    def write_file(data, filename):
+        if not filename.startswith("output/"):
+            filename = "output/" +  filename
+
+
+        write_html(data, filename)
+        print(f"View written file at {filename}")
+
+
+
```

### Comparing `bose-2.0.6/bose/profile.py` & `bose-2.0.7/bose/profile.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/schedule_utils.py` & `bose-2.0.7/bose/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/task_info.py` & `bose-2.0.7/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/temp_mail.py` & `bose-2.0.7/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/user_agent.py` & `bose-2.0.7/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/utils.py` & `bose-2.0.7/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/bose/window_size.py` & `bose-2.0.7/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.6/setup.py` & `bose-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     except:
       return None
     
             
 setup(
     name='bose',
     packages=['bose'],
-    version='2.0.6',
+    version='2.0.7',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/",
         "Source": "https://github.com/omkarcloud/bose",
         "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
```


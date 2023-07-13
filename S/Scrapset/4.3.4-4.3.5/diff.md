# Comparing `tmp/Scrapset-4.3.4.tar.gz` & `tmp/Scrapset-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-4.3.4.tar", last modified: Thu Jul 13 18:23:00 2023, max compression
+gzip compressed data, was "Scrapset-4.3.5.tar", last modified: Thu Jul 13 18:27:52 2023, max compression
```

## Comparing `Scrapset-4.3.4.tar` & `Scrapset-4.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 18:23:00.850549 Scrapset-4.3.4/
--rw-rw-rw-   0        0        0     4648 2023-07-13 18:23:00.851551 Scrapset-4.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 18:23:00.836472 Scrapset-4.3.4/Scrapset/
--rw-rw-rw-   0        0        0    10290 2023-07-13 18:21:12.000000 Scrapset-4.3.4/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       61 2023-07-13 16:57:26.000000 Scrapset-4.3.4/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:23:00.849457 Scrapset-4.3.4/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.3.4/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-13 18:23:00.852865 Scrapset-4.3.4/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-07-13 18:22:49.000000 Scrapset-4.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:27:52.862599 Scrapset-4.3.5/
+-rw-rw-rw-   0        0        0     4648 2023-07-13 18:27:52.862599 Scrapset-4.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 18:27:52.855623 Scrapset-4.3.5/Scrapset/
+-rw-rw-rw-   0        0        0    10284 2023-07-13 18:25:37.000000 Scrapset-4.3.5/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       61 2023-07-13 16:57:26.000000 Scrapset-4.3.5/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:27:52.861395 Scrapset-4.3.5/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 18:27:52.000000 Scrapset-4.3.5/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.3.5/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-13 18:27:52.862599 Scrapset-4.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-07-13 18:27:05.000000 Scrapset-4.3.5/setup.py
```

### Comparing `Scrapset-4.3.4/PKG-INFO` & `Scrapset-4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.4
+Version: 4.3.5
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.4/README.md` & `Scrapset-4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-4.3.4/Scrapset/Scrapset.py` & `Scrapset-4.3.5/Scrapset/Scrapset.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         options.add_argument('--disable-gpu')
         options.add_argument("--window-size=1920,1200")
         options.add_argument('--disable-dev-shm-usage')
         driver = webdriver.Chrome(options=options)
         return driver
 
     def data_set_page(self, url, last_page, initial_page):
-        # try:
+        try:
             driver = webdriver.Chrome()
             self.url = url
             time.sleep(1)
             
             list_of_dic = {'title': [], 'size': [],'all_details':[],'up_vote':[]}  # Initialize the dictionary
 
             while initial_page < last_page:  
@@ -44,16 +44,16 @@
                         continue
                     list_of_dic['size'].append(data_set_size)
                     list_of_dic['title'].append(data_set_title)
                     list_of_dic['all_details'].append(data_set_details)
                     list_of_dic['up_vote'].append(data_set_upvote)
             driver.quit()
             return list_of_dic
-        # except:
-        #     logging.error("Invalid Url")
+        except:
+            logging.error("Invalid Url")
     def kaggle_discussions(self,url,initial_page,last_page):
         try:
             self.url=url
             driver=webdriver.Chrome()
             time.sleep(1)
             list_of_dic = {'title': [],'all_details':[],'up_vote':[],'comments':[]}  # Initialize the dictionary
             while initial_page <= last_page:
```

### Comparing `Scrapset-4.3.4/Scrapset.egg-info/PKG-INFO` & `Scrapset-4.3.5/Scrapset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.4
+Version: 4.3.5
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.4/licence.txt` & `Scrapset-4.3.5/licence.txt`

 * *Files identical despite different names*


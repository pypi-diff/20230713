# Comparing `tmp/Scrapset-4.3.3.tar.gz` & `tmp/Scrapset-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-4.3.3.tar", last modified: Thu Jul 13 17:01:54 2023, max compression
+gzip compressed data, was "Scrapset-4.3.4.tar", last modified: Thu Jul 13 18:23:00 2023, max compression
```

## Comparing `Scrapset-4.3.3.tar` & `Scrapset-4.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 17:01:54.156991 Scrapset-4.3.3/
--rw-rw-rw-   0        0        0     4648 2023-07-13 17:01:54.156991 Scrapset-4.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 17:01:54.144313 Scrapset-4.3.3/Scrapset/
--rw-rw-rw-   0        0        0    10289 2023-07-13 17:00:31.000000 Scrapset-4.3.3/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       61 2023-07-13 16:57:26.000000 Scrapset-4.3.3/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:01:54.154990 Scrapset-4.3.3/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.3.3/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-13 17:01:54.158987 Scrapset-4.3.3/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-07-13 17:01:45.000000 Scrapset-4.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:23:00.850549 Scrapset-4.3.4/
+-rw-rw-rw-   0        0        0     4648 2023-07-13 18:23:00.851551 Scrapset-4.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 18:23:00.836472 Scrapset-4.3.4/Scrapset/
+-rw-rw-rw-   0        0        0    10290 2023-07-13 18:21:12.000000 Scrapset-4.3.4/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       61 2023-07-13 16:57:26.000000 Scrapset-4.3.4/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:23:00.849457 Scrapset-4.3.4/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 18:23:00.000000 Scrapset-4.3.4/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.3.4/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-13 18:23:00.852865 Scrapset-4.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-07-13 18:22:49.000000 Scrapset-4.3.4/setup.py
```

### Comparing `Scrapset-4.3.3/PKG-INFO` & `Scrapset-4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.3
+Version: 4.3.4
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.3/README.md` & `Scrapset-4.3.4/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-4.3.3/Scrapset/Scrapset.py` & `Scrapset-4.3.4/Scrapset/Scrapset.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
         options.add_argument('--disable-gpu')
         options.add_argument("--window-size=1920,1200")
         options.add_argument('--disable-dev-shm-usage')
         driver = webdriver.Chrome(options=options)
         return driver
 
     def data_set_page(self, url, last_page, initial_page):
-        try:
+        # try:
             driver = webdriver.Chrome()
             self.url = url
             time.sleep(1)
             
             list_of_dic = {'title': [], 'size': [],'all_details':[],'up_vote':[]}  # Initialize the dictionary
 
             while initial_page < last_page:  
                 # i = i + 1
                 initial_page=initial_page + 1 
-                driver.get(self.url + f'/datasets?page={self.initial_page}')
+                driver.get(self.url + f'/datasets?page={initial_page}')
                 time.sleep(0.5)
                 titles = driver.find_elements(By.XPATH, '//*[@id="site-content"]/div[6]/div/div/div/ul/li/div[1]/a')
                 for title in titles:
                     data_set_title = title.find_element(By.XPATH, './div[2]/div').text
                     try: 
                         data_set_size = title.find_element(By.XPATH, './div[2]/span[2]/span').text
                         data_set_details=title.find_element(By.XPATH,'//*[@id="site-content"]/div[6]/div/div/div/ul/li[1]/div[1]/a/div[2]/span').text
@@ -44,16 +44,16 @@
                         continue
                     list_of_dic['size'].append(data_set_size)
                     list_of_dic['title'].append(data_set_title)
                     list_of_dic['all_details'].append(data_set_details)
                     list_of_dic['up_vote'].append(data_set_upvote)
             driver.quit()
             return list_of_dic
-        except:
-            logging.error("Invalid Url")
+        # except:
+        #     logging.error("Invalid Url")
     def kaggle_discussions(self,url,initial_page,last_page):
         try:
             self.url=url
             driver=webdriver.Chrome()
             time.sleep(1)
             list_of_dic = {'title': [],'all_details':[],'up_vote':[],'comments':[]}  # Initialize the dictionary
             while initial_page <= last_page:
```

### Comparing `Scrapset-4.3.3/Scrapset.egg-info/PKG-INFO` & `Scrapset-4.3.4/Scrapset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.3
+Version: 4.3.4
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.3/licence.txt` & `Scrapset-4.3.4/licence.txt`

 * *Files identical despite different names*


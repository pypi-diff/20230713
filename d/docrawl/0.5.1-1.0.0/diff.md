# Comparing `tmp/docrawl-0.5.1.tar.gz` & `tmp/docrawl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-0.5.1.tar", last modified: Fri Jun 23 17:12:01 2023, max compression
+gzip compressed data, was "docrawl-1.0.0.tar", last modified: Thu Jul 13 10:36:04 2023, max compression
```

## Comparing `docrawl-0.5.1.tar` & `docrawl-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 17:12:01.819239 docrawl-0.5.1/
--rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.5.1/LICENSE
--rw-rw-rw-   0        0        0      568 2023-06-23 17:12:01.817244 docrawl-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 17:12:01.786326 docrawl-0.5.1/docrawl/
--rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.5.1/docrawl/__init__.py
--rw-rw-rw-   0        0        0    44925 2023-06-23 17:11:30.000000 docrawl-0.5.1/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6753 2023-06-23 17:11:30.000000 docrawl-0.5.1/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.5.1/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-0.5.1/docrawl/elements.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:12:01.816246 docrawl-0.5.1/docrawl.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-23 17:12:00.000000 docrawl-0.5.1/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-23 17:12:01.000000 docrawl-0.5.1/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 17:12:00.000000 docrawl-0.5.1/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-06-23 17:12:01.000000 docrawl-0.5.1/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 17:12:01.000000 docrawl-0.5.1/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 17:12:01.819239 docrawl-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-06-23 17:11:41.000000 docrawl-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:36:04.993735 docrawl-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-07-13 10:36:04.993735 docrawl-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 10:36:04.974785 docrawl-1.0.0/docrawl/
+-rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-1.0.0/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    11453 2023-07-13 10:34:35.000000 docrawl-1.0.0/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    36374 2023-07-13 10:34:35.000000 docrawl-1.0.0/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2023-07-13 10:34:35.000000 docrawl-1.0.0/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-1.0.0/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-1.0.0/docrawl/elements.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:36:04.992737 docrawl-1.0.0/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 10:36:04.000000 docrawl-1.0.0/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:36:04.993735 docrawl-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-07-13 10:35:43.000000 docrawl-1.0.0/setup.py
```

### Comparing `docrawl-0.5.1/LICENSE` & `docrawl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-0.5.1/PKG-INFO` & `docrawl-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.5.1
+Version: 1.0.0
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.5.1/docrawl/docrawl_core.py` & `docrawl-1.0.0/docrawl/docrawl_core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1212 +1,928 @@
-# import sys #PATH initialization of modules
-# try:
-#    sys.path.append("C:\\Users\\EUROCOM\\Documents\\Git\\DovaX")
-# except:
-#    pass
-from docrawl.docrawl_logger import docrawl_logger
-from docrawl.elements import Element, ElementType, classify_element_by_xpath, PREDEFINED_TAGS
-from collections import UserDict
 import datetime
 import scrapy
 import requests
 import time
-import pickle
 import os
 import re
 import psutil
 import lxml.html
 import pandas as pd
 
-# Due to the problems with selenium wire on linux systems
-try:
-    from selenium import webdriver
-except:
-    docrawl_logger.error('Error while importing selenium-wire, using selenium instead')
-    from selenium import webdriver
-
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.proxy import Proxy, ProxyType
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver import FirefoxOptions, ChromeOptions
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.firefox.service import Service
 from selenium.webdriver.remote.webdriver import WebElement
 
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.chrome import ChromeDriverManager
 
 from scrapy.selector import Selector
-from keepvariable.keepvariable_core import VarSafe, kept_variables, save_variables, load_variable_safe, KeepVariableDummyRedisServer
-
-from typing import Optional
-
-kv_redis: Optional[KeepVariableDummyRedisServer] = None
-
-kv_redis_key_webpage_elements = 'elements'
-kv_redis_key_screenshot = 'screenshot'
 
+from docrawl.docrawl_logger import docrawl_logger
+from docrawl.elements import Element, ElementType, classify_element_by_xpath, PREDEFINED_TAGS
 
-def click_class(browser, class_input, index=0, tag="div", wait1=1):
-    name_input = browser.find_elements_by_xpath('//' + tag + '[@class="' + class_input + '"]')
-    name_input[index].click()
-    time.sleep(wait1)
-    return (name_input)
+# Due to the problems with selenium wire on linux systems
+try:
+    from selenium import webdriver
+except:
+    docrawl_logger.error('Error while importing selenium-wire, using selenium instead')
+    from selenium import webdriver
 
 
-def take_screenshot(browser, page, inp):
-    """
-    Takes screenshot of current page and saves it.
-        :param browser: Selenium driver, browser instance
-        :param inp, list, inputs from launcher (filename)
-    """
+class DocrawlSpider(scrapy.spiders.CrawlSpider):
+    name = "forloop"
 
-    #filename = inp['filename']
+    custom_settings = {
+        'LOG_LEVEL': 'ERROR',
+        'USER_AGENT': "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
+        'DEFAULT_REQUEST_HEADERS': {
+            'Referer': 'https://forloop.ai'
+        }
+        #   'CONCURRENT_REQUESTS' : '20',
+    }
 
-    if type(browser) == webdriver.Firefox:
+    def __init__(self, *a, **kw):
+        self.docrawl_client = kw['docrawl_client']
 
-        try:
-            docrawl_logger.warning('START SCREENSHOT CREATED')
-            root_element = browser.find_element(By.XPATH, '/html')
-            string = browser.get_full_page_screenshot_as_base64()
-            browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
+        self.kv_redis_key_screenshot = self.docrawl_client.kv_redis_keys.get('screenshot', 'screenshot')
+        self.kv_redis_key_elements = self.docrawl_client.kv_redis_keys.get('elements', 'elements')
 
-            # with open(filename, "w+") as fh:
-            #     fh.write(string)
-            #     docrawl_logger.warning('SCRENSHOT CREATED')
-        except Exception as e:
-            string = ""
-            docrawl_logger.error(f'Error while taking page screenshot: {e}')
+        self.browser = self._initialise_browser()
+        browser_meta_data = self.docrawl_client.get_browser_meta_data()
+        browser_meta_data['browser']['pid'] = self._determine_browser_pid()
 
-    elif type(browser) == webdriver.Chrome:
-        # Get params needed for fullpage screenshot
-        page_rect = browser.execute_cdp_cmd('Page.getLayoutMetrics', {})
-
-        # Set the width and height of the viewport to screenshot, same as the site's content size
-        screenshot_config = {'captureBeyondViewport': True,
-                             'fromSurface': True,
-                             'clip': {'width': page_rect['cssContentSize']['width'],
-                                      'height': page_rect['cssContentSize']['height'],
-                                      'x': 0,
-                                      'y': 0,
-                                      'scale': 1},
-                             }
-        # Dictionary with 1 key: data
-        string = browser.execute_cdp_cmd('Page.captureScreenshot', screenshot_config)['data']  # Taking screenshot
-        # with open(filename, "w+") as fh:
-        #     fh.write(string)
-    else:
-        string = ""
-
-    kv_redis.set(key=kv_redis_key_screenshot, value=string)
-    docrawl_logger.warning('SCRENSHOT CREATED')
+        self.docrawl_client.set_browser_meta_data(browser_meta_data)
 
+        self.start_requests()
 
+    def _initialise_browser(self):
+        browser_meta_data = self.docrawl_client.get_browser_meta_data()
 
-def take_png_screenshot(browser, page, inp):
-    """
-    Takes screenshot of current page and saves it.
-        :param browser: Selenium driver, browser instance
-        :param inp, list, inputs from launcher (filename)
-    """
-
-    filename = inp["filename"]
-    '''
-    try:
-        root_element = browser.find_element(By.XPATH, '/html')
-        browser.save_full_page_screenshot(filename)
-
-        browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
-    except Exception as e:
-        print('Error while taking page screenshot!', e)
-    '''
-    if type(browser) == webdriver.Firefox:
+        docrawl_logger.info(f'Browser settings: {browser_meta_data}')
 
         try:
-            root_element = browser.find_element(By.XPATH, '/html')
+            self.driver_type = browser_meta_data['browser']['driver']
+        except Exception as e:
+            docrawl_logger.error(f'Error while loading driver type information: {e}')
+            self.driver_type = 'Firefox'
 
-            screenshot = browser.get_full_page_screenshot_as_file(filename)
-            browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
+        try:
+            self.headless = browser_meta_data['browser']['headless']
+        except Exception as e:
+            docrawl_logger.error(f'Error while loading headless mode information: {e}')
+            self.headless = False
 
-            docrawl_logger.info(f'Png screenshot created')
+        try:
+            proxy_info = browser_meta_data['browser']['proxy']
         except Exception as e:
-            docrawl_logger.error(f'Error while taking page png screenshot: {e}')
+            docrawl_logger.warning(f'Error while loading proxy information: {e}')
+            proxy_info = None
 
+        if self.driver_type == 'Firefox':
+            capabilities = DesiredCapabilities.FIREFOX.copy()
+            self.options = FirefoxOptions()
+            capabilities["marionette"] = True
 
-def extract_page_source(browser, page, inp):
-    """
-    Extracts the source of currently scraped page.
-        :param page: Selenium Selector, page to export source from
-        :param inp: list, inputs from launcher (incl_tables, incl_bullets, output_dir)
-    """
+            sw_options = self._set_proxy(proxy_info)
 
-    filename = inp['filename']
+            if self.headless:
+                self.options.add_argument("--headless")
 
-    with open(filename, 'w+', encoding="utf-8") as f:
-        f.write(browser.page_source)
+                # For headless mode different width of window is needed
+                window_size_x = 1450
 
+            try:
+                self.browser = webdriver.Firefox(options=self.options, capabilities=capabilities,
+                                                 service=Service(GeckoDriverManager().install()))
+            except Exception as e:
+                docrawl_logger.error(f'Error while creating Firefox instance {e}')
+                self.browser = webdriver.Firefox(options=self.options, capabilities=capabilities)
 
-def scan_web_page(browser, page, inp):
-    """
-    Finds different elements (tables, bullet lists) on page.
-        :param page: Selenium Selector, page to search elements in
-        :param inp: list, inputs from launcher (incl_tables, incl_bullets, output_dir)
-        :param browser: webdriver, browser instance
-    """
+        elif self.driver_type == 'Chrome':
+            capabilities = DesiredCapabilities.CHROME
+            self.options = ChromeOptions()
 
-    incl_tables = inp['incl_tables']
-    incl_bullets = inp['incl_bullets']
-    incl_texts = inp['incl_texts']
-    incl_headlines = inp['incl_headlines']
-    incl_links = inp['incl_links']
-    incl_images = inp['incl_images']
-    incl_buttons = inp['incl_buttons']
-    by_xpath = inp['by_xpath']
-    cookies_xpath = inp['cookies_xpath']        # dev param only
-    context_xpath = inp['context_xpath']
-    output_folder = inp['output_folder']
+            sw_options = self._set_proxy(proxy_info)
 
-    # First removed old data
-    kv_redis.set(key=kv_redis_key_webpage_elements, value=[])
+            if self.headless:
+                self.options.add_argument("--headless")
 
-    # Dictionary with elements (XPaths, data)
-    final_elements = {}
+                # For headless mode different width of window is needed
+                window_size_x = 1450
 
-    # Page source for parser
-    innerHTML = browser.execute_script("return document.body.innerHTML")
-    tree = lxml.html.fromstring(innerHTML)
+            try:
+                self.browser = webdriver.Chrome(options=self.options, desired_capabilities=capabilities,
+                                                executable_path=ChromeDriverManager().install())
+            except:
+                pass
 
-    # Url pattern, used to get main page url from current url
-    url_pattern = re.compile('^(((https|http):\/\/|www\.)*[a-zA-Z0-9\.\/\?\:@\-_=#]{2,100}\.[a-zA-Z]{2,6}\/)')
+        window_size_x = 1820
 
-    time_start_f = datetime.datetime.now()
+        self.browser.set_window_size(window_size_x, 980)
 
-    def timedelta_format(end, start):
-        delta = end - start
-        sec = delta.seconds
-        microsec = delta.microseconds
+        return self.browser
 
-        return f'{sec}:{microsec}'
+    def __del__(self):
+        self.browser.quit()
 
-    def string_cleaner(string):
+    def _set_proxy(self, proxy_info: dict) -> dict:
         """
-        Removes whitespaces from string.
-            :param string: string, string to clean
-            :return - cleaned string
+        Sets proxy before launching browser instance.
+        :param proxy_info: proxy params (ip, port, username, password)
         """
 
-        return ''.join(string.strip()).replace('\\', '')
+        # If proxy was not set
+        if proxy_info is None or any([not proxy_info['ip'], not proxy_info['port']]):
+            return None
 
-    def process_bullet(xpath):
-        """
-        Processes (cleans) bullet element, e.g. one <li> element per line
-            :param xpath: XPath of element
-        """
+        proxy_ip = proxy_info['ip']
+        proxy_port = proxy_info['port']
+        proxy_username = proxy_info['username']
+        proxy_password = proxy_info['password']
 
-        tag_2 = page.xpath(xpath)[0]
-        result = []
-        li_tags = tag_2.xpath('.//li')
+        if proxy_username and proxy_password:
+            proxy = f'http://{proxy_username}:{proxy_password}@{proxy_ip}:{proxy_port}'
+        else:
+            proxy = f'{proxy_ip}:{proxy_port}'
 
-        # <li> inside <ol> don't contain numbers, but they could be added here
-        for li_tag in li_tags:
-            data = li_tag.xpath('.//text()').getall()
-            data = [string_cleaner(x) for x in data]  # Cleaning the text
-            data = list(filter(None, data))
-            element = ' '.join(data).replace(u'\xa0', u' ')
-
-            result.append(element + '\n')
-
-        return result
-
-    def save_coordinates_of_elements(selectors, names, xpaths, data):
-        """
-        Saves coordinates of elements (tables, bullet lists, text elements, headlines, links), that could be potentially exported.
-        """
-        elems_pos = []
-
-        existing_xpaths = []
-
-        for selector, name, xpath, data in zip(selectors, names, xpaths, data):
-
-            # Deduplicate elements by xpath (on some pages the same element is selected twice)
-            if xpath in existing_xpaths:
-                continue
-
-            elems_pos.append({'rect': selector.rect,
-                              'name': name,
-                              'xpath': xpath,
-                              'data': data})
-
-            existing_xpaths.append(xpath)
-
-        elements_positions = {"elements_positions": elems_pos}
-        filename = "elements_positions.kpv"
-        with open(filename, "w+", encoding="utf8",
-                  errors='ignore') as file:  # TODO: improve KPV to enable multiple keep variable files -> it collided with browser_metadata_kpv,
-            file.write(str(elements_positions))
-
-        # elements_positions = VarSafe(elements_positions, 'elements_positions', 'elements_positions')
-        # save_variables(kept_variables, 'elements_positions.kpv')
-
-    def extract_element_data(element: WebElement, xpath: str, element_type: ElementType):
-        if element_type in [ElementType.LINK, ElementType.BUTTON]:
-            xpath_new = xpath + '//text()'
-            text = ''.join(page.xpath(xpath_new).extract()).strip()
-        elif element_type == ElementType.IMAGE:
-            xpath_new = xpath + '//text()'
-            text = page.xpath(xpath_new).extract()
-
-            # if data:
-            #     # Handle images with relative path. E.g. images/logo.png
-            #     if not any([data.startswith(x) for x in ['http', 'www']]):
-            #         data = url_pattern.match(browser.current_url).group(1) + data.replace('./', '')
-            #
-            #     with open(path + '.pickle', 'wb') as pickle_file:
-            #         pickle.dump(data, pickle_file)
-        elif element_type == ElementType.BULLET:
-            text = process_bullet(xpath)
-            #xpath_new = xpath + '//li//text()'
-        elif element_type == ElementType.TABLE:
-            table_2 = page.xpath(xpath)[0]
-
-            result = []  # data
-            titles = []  # columns' names
-            tr_tags = table_2.xpath('.//tr')  # <tr> = table row
-            th_tags = table_2.xpath('.//th')  # <th> = table header (non-essential, so if any)
+        # Proxy with authentication
+        if 'http://' in proxy:
+            # selenium-wire proxy settings
+            sw_options = {
+                'proxy': {
+                    'http': proxy,
+                    'https': proxy,
+                    'no_proxy': 'localhost,127.0.0.1'
+                }
+            }
 
-            for th_tag in th_tags:
-                titles.append(''.join(th_tag.xpath('.//text()').extract()).replace('\n', '').replace('\t', ''))
+        # Proxy without authentication
+        else:
+            sw_options = None
+            firefox_proxies = Proxy()
+            firefox_proxies.ssl_proxy = proxy
+            firefox_proxies.http_proxy = proxy
+            firefox_proxies.proxy_type = ProxyType.MANUAL
 
-            for tr_tag in tr_tags:
-                td_tags = tr_tag.xpath('.//td')  # <td> = table data
+            self.options.proxy = firefox_proxies
 
-                row = []
+        return sw_options
 
-                '''
-                    # Sometimes between td tags there more than 1 tag with text, so that would
-                    # be proceeded as separate values despite of fact it should be in one cell.
-                    # That's why the further loop is needed. The result of it is a list of strings,
-                    # that should be in one cell later in dataframe.
-
-                    # Example: 
-
-                    <td>
-                        <a>Text 1</a>
-                        <a>Text 2</a>
-                    </td>
-
-                    # Without loop it would be two strings ("Text 1", "Text 2") and thus they 
-                    # will be in 2 differrent columns. With loop the result would be ["Text 1", "Text 2"] 
-                    # and after join method - "Text 1 Text 2" in just one cell (column).
-               '''
+    def _determine_browser_pid(self):
+        browser_pid = None
 
-                for td_tag in td_tags:
-                    data = td_tag.xpath('.//text()').getall()
+        try:
+            if self.driver_type == 'Firefox':
+                browser_pid = self.browser.capabilities['moz:processID']
+            elif self.driver_type == 'Chrome':
+                self.browser.service.process
+                browser_pid = psutil.Process(self.browser.service.process.pid).pid
 
-                    '''
-                        Some table cells include \n or unicode symbols,
-                        so that creates unneccesary "empty" columns and thus
-                        the number of columns doesn't meet the real one
-                    '''
+            docrawl_logger.success(f'Browser PID: {browser_pid}')
+        except Exception as e:
+            docrawl_logger.error(f'Error while determining browser PID: {e}')
 
-                    data = [string_cleaner(x) for x in data]  # Cleaning the text
+        return browser_pid
 
-                    # data = list(filter(None, data))  # Deleting empty strings
+    def start_requests(self):
+        URLS = ['https://www.forloop.ai']
+        FUNCTIONS = [self.parse]
+        for i in range(len(URLS)):
+            yield scrapy.Request(url=URLS[i], callback=FUNCTIONS[i])  # yield
 
-                    row.append('\n'.join(data))  # Making one string value from list
+    # # # # # # # SCRAPING FUNCTIONS # # # # # # #
 
-                result.append(row)
+    def _init_function(self, inp):
+        pass
 
-                if not titles:  # If table doesn't have <th> tags -> use first row as titles
-                    titles = row  # TODO: IF USER SELECTS THE TABLE, ASK HIM, WHETHER HE WANTS TO HAVE 1 ROW AS TITLES
+    def _click_class(self, inp):
+        class_input = inp.get("filename")
+        index = inp.get("index", 0)
+        tag = inp.get("tag", "div")
 
-            try:
-                # If number of columns' names (titles) is the same as number of columns
-                df = pd.DataFrame(result, columns=titles)
-            except Exception:
-                df = pd.DataFrame(result)
+        name_input = self.browser.find_elements(By.XPATH, f'//{tag}[@class="{class_input}"]')
+        name_input[index].click()
 
-            df = df.iloc[1:, :]  # Removing empty row at the beginning of dataframe
+        return name_input
 
-            df.dropna(axis=0, how='all', inplace=True)
+    def _take_screenshot(self, inp):
+        """
+        Takes screenshot of current page and saves it.
+            :param browser: Selenium driver, browser instance
+            :param inp, list, inputs from launcher (filename)
+        """
 
-            text = df
+        # filename = inp['filename']
+        browser_type = type(self.browser)
 
-            # # If dataframe is not empty
-            # if not df.dropna().empty and len(df.columns) > 1 and len(df) > 1:
-            #     # Serialize DataFrame
-            #
-            #     with open(path + '.pickle', 'wb') as pickle_file:
-            #         pickle.dump(df, pickle_file)
-        else:
-            xpath += '//text()'
+        if browser_type == webdriver.Firefox:
 
-            # Try to extract text from element
             try:
-                text = ''.join(page.xpath(xpath).extract()).strip()
-            # Extract element otherwise
-            except:
-                xpath = xpath.removesuffix('//text()')
-                text = ''.join(page.xpath(xpath).extract()).strip()
+                docrawl_logger.warning('START SCREENSHOT CREATED')
+                root_element = self.browser.find_element(By.XPATH, '/html')
+                string = self.browser.get_full_page_screenshot_as_base64()
+                self.browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
+
+                # with open(filename, "w+") as fh:
+                #     fh.write(string)
+                #     docrawl_logger.warning('SCRENSHOT CREATED')
+            except Exception as e:
+                string = ""
+                docrawl_logger.error(f'Error while taking page screenshot: {e}')
 
-        # attributes = element.get_property('attributes')
-        attributes = browser.execute_script(
-            'var items = {}; for (index = 0; index < arguments[0].attributes.length; ++index) { items[arguments[0].attributes[index].name] = arguments[0].attributes[index].value }; return items;',
-            element)
-
-        # docrawl_logger.warning(attributes)
-        element_data = {
-            'tag_name': re.split('//|/', xpath)[-1].split('[')[0],
-            'text': text,
-            'attributes': attributes
-        }
+        elif browser_type == webdriver.Chrome:
+            # Get params needed for fullpage screenshot
+            page_rect = self.browser.execute_cdp_cmd('Page.getLayoutMetrics', {})
+
+            # Set the width and height of the viewport to screenshot, same as the site's content size
+            screenshot_config = {'captureBeyondViewport': True,
+                                 'fromSurface': True,
+                                 'clip': {'width': page_rect['cssContentSize']['width'],
+                                          'height': page_rect['cssContentSize']['height'],
+                                          'x': 0,
+                                          'y': 0,
+                                          'scale': 1},
+                                 }
+            # Dictionary with 1 key: data
+            string = self.browser.execute_cdp_cmd('Page.captureScreenshot', screenshot_config)['data']  # Taking screenshot
+            # with open(filename, "w+") as fh:
+            #     fh.write(string)
+        else:
+            string = ""
 
-        return element_data
+        self.docrawl_client.set_browser_screenshot(string)
+        docrawl_logger.warning('SCRENSHOT CREATED')
 
-    def serialize_and_append_data(element_name, selector: WebElement, xpath):
+    def _take_png_screenshot(self, inp):
         """
-        Serializes data behind the element and updates dictionary with final elements
-            :param element_name: variable name to save
-            :param selector: Selenium Selector
-            :param xpath: XPath of element
+        Takes screenshot of current page and saves it.
+            :param browser: Selenium driver, browser instance
+            :param inp, list, inputs from launcher (filename)
         """
 
-        path = os.path.join(output_folder, element_name)
+        filename = inp["filename"]
+        '''
+        try:
+            root_element = browser.find_element(By.XPATH, '/html')
+            browser.save_full_page_screenshot(filename)
+
+            browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
+        except Exception as e:
+            print('Error while taking page screenshot!', e)
+        '''
 
-        if 'table' in element_name:
-            table_2 = page.xpath(xpath)[0]
+        browser_type = type(self.browser)
 
-            result = []  # data
-            titles = []  # columns' names
-            tr_tags = table_2.xpath('.//tr')  # <tr> = table row
-            th_tags = table_2.xpath('.//th')  # <th> = table header (non-essential, so if any)
+        if type(self.browser) == webdriver.Firefox:
 
-            for th_tag in th_tags:
-                titles.append(''.join(th_tag.xpath('.//text()').extract()).replace('\n', '').replace('\t', ''))
+            try:
+                root_element = self.browser.find_element(By.XPATH, '/html')
 
-            for tr_tag in tr_tags:
-                td_tags = tr_tag.xpath('.//td')  # <td> = table data
+                screenshot = self.browser.get_full_page_screenshot_as_file(filename)
+                self.browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
 
-                row = []
+                docrawl_logger.info(f'Png screenshot created')
+            except Exception as e:
+                docrawl_logger.error(f'Error while taking page png screenshot: {e}')
 
-                '''
-                    # Sometimes between td tags there more than 1 tag with text, so that would
-                    # be proceeded as separate values despite of fact it should be in one cell.
-                    # That's why the further loop is needed. The result of it is a list of strings,
-                    # that should be in one cell later in dataframe.
-
-                    # Example: 
-
-                    <td>
-                        <a>Text 1</a>
-                        <a>Text 2</a>
-                    </td>
-
-                    # Without loop it would be two strings ("Text 1", "Text 2") and thus they 
-                    # will be in 2 differrent columns. With loop the result would be ["Text 1", "Text 2"] 
-                    # and after join method - "Text 1 Text 2" in just one cell (column).
-               '''
+    def _extract_page_source(self, inp):
+        """
+        Extracts the source of currently scraped page.
+            :param page: Selenium Selector, page to export source from
+            :param inp: list, inputs from launcher (incl_tables, incl_bullets, output_dir)
+        """
 
-                for td_tag in td_tags:
-                    data = td_tag.xpath('.//text()').getall()
+        filename = inp['filename']
 
-                    '''
-                        Some table cells include \n or unicode symbols,
-                        so that creates unneccesary "empty" columns and thus
-                        the number of columns doesn't meet the real one
-                    '''
+        with open(filename, 'w+', encoding="utf-8") as f:
+            f.write(self.browser.page_source)
 
-                    data = [string_cleaner(x) for x in data]  # Cleaning the text
+    def _scan_web_page(self, inp):
+        """
+        Finds different elements (tables, bullet lists) on page.
+            :param page: Selenium Selector, page to search elements in
+            :param inp: list, inputs from launcher (incl_tables, incl_bullets, output_dir)
+            :param browser: webdriver, browser instance
+        """
+
+        incl_tables = inp['incl_tables']
+        incl_bullets = inp['incl_bullets']
+        incl_texts = inp['incl_texts']
+        incl_headlines = inp['incl_headlines']
+        incl_links = inp['incl_links']
+        incl_images = inp['incl_images']
+        incl_buttons = inp['incl_buttons']
+        by_xpath = inp['by_xpath']
+        cookies_xpath = inp['cookies_xpath']  # dev param only
+        context_xpath = inp['context_xpath']
+        output_folder = inp['output_folder']
+
+        # First removed old data
+        self.docrawl_client.set_browser_scanned_elements(elements=[])
+
+        # Dictionary with elements (XPaths, data)
+        final_elements = {}
+
+        # Page source for parser
+        innerHTML = self.browser.execute_script("return document.body.innerHTML")
+        tree = lxml.html.fromstring(innerHTML)
+
+        # Url pattern, used to get main page url from current url
+        url_pattern = re.compile('^(((https|http):\/\/|www\.)*[a-zA-Z0-9\.\/\?\:@\-_=#]{2,100}\.[a-zA-Z]{2,6}\/)')
+
+        time_start_f = datetime.datetime.now()
+
+        def timedelta_format(end, start):
+            delta = end - start
+            sec = delta.seconds
+            microsec = delta.microseconds
+
+            return f'{sec}:{microsec}'
+
+        def string_cleaner(string):
+            """
+            Removes whitespaces from string.
+                :param string: string, string to clean
+                :return - cleaned string
+            """
+
+            return ''.join(string.strip()).replace('\\', '')
+
+        def process_bullet(xpath):
+            """
+            Processes (cleans) bullet element, e.g. one <li> element per line
+                :param xpath: XPath of element
+            """
+
+            tag_2 = self.page.xpath(xpath)[0]
+            result = []
+            li_tags = tag_2.xpath('.//li')
+
+            # <li> inside <ol> don't contain numbers, but they could be added here
+            for li_tag in li_tags:
+                data = li_tag.xpath('.//text()').getall()
+                data = [string_cleaner(x) for x in data]  # Cleaning the text
+                data = list(filter(None, data))
+                element = ' '.join(data).replace(u'\xa0', u' ')
+
+                result.append(element + '\n')
+
+            return result
+
+        def extract_element_data(element: WebElement, xpath: str, element_type: ElementType):
+            if element_type in [ElementType.LINK, ElementType.BUTTON]:
+                xpath_new = xpath + '//text()'
+                text = ''.join(self.page.xpath(xpath_new).extract()).strip()
+            elif element_type == ElementType.IMAGE:
+                xpath_new = xpath + '//text()'
+                text = self.page.xpath(xpath_new).extract()
+
+                # if data:
+                #     # Handle images with relative path. E.g. images/logo.png
+                #     if not any([data.startswith(x) for x in ['http', 'www']]):
+                #         data = url_pattern.match(browser.current_url).group(1) + data.replace('./', '')
+                #
+                #     with open(path + '.pickle', 'wb') as pickle_file:
+                #         pickle.dump(data, pickle_file)
+            elif element_type == ElementType.BULLET:
+                text = process_bullet(xpath)
+                # xpath_new = xpath + '//li//text()'
+            elif element_type == ElementType.TABLE:
+                table_2 = self.page.xpath(xpath)[0]
+
+                result = []  # data
+                titles = []  # columns' names
+                tr_tags = table_2.xpath('.//tr')  # <tr> = table row
+                th_tags = table_2.xpath('.//th')  # <th> = table header (non-essential, so if any)
 
-                    # data = list(filter(None, data))  # Deleting empty strings
+                for th_tag in th_tags:
+                    titles.append(''.join(th_tag.xpath('.//text()').extract()).replace('\n', '').replace('\t', ''))
 
-                    row.append('\n'.join(data))  # Making one string value from list
+                for tr_tag in tr_tags:
+                    td_tags = tr_tag.xpath('.//td')  # <td> = table data
 
-                result.append(row)
+                    row = []
 
-                if not titles:  # If table doesn't have <th> tags -> use first row as titles
-                    titles = row  # TODO: IF USER SELECTS THE TABLE, ASK HIM, WHETHER HE WANTS TO HAVE 1 ROW AS TITLES
+                    '''
+                        # Sometimes between td tags there more than 1 tag with text, so that would
+                        # be proceeded as separate values despite of fact it should be in one cell.
+                        # That's why the further loop is needed. The result of it is a list of strings,
+                        # that should be in one cell later in dataframe.
 
-            try:
-                # If number of columns' names (titles) is the same as number of columns
-                df = pd.DataFrame(result, columns=titles)
-            except Exception:
-                df = pd.DataFrame(result)
+                        # Example: 
 
-            df = df.iloc[1:, :]  # Removing empty row at the beginning of dataframe
+                        <td>
+                            <a>Text 1</a>
+                            <a>Text 2</a>
+                        </td>
 
-            df.dropna(axis=0, how='all', inplace=True)
+                        # Without loop it would be two strings ("Text 1", "Text 2") and thus they 
+                        # will be in 2 differrent columns. With loop the result would be ["Text 1", "Text 2"] 
+                        # and after join method - "Text 1 Text 2" in just one cell (column).
+                   '''
 
-            # If dataframe is not empty
-            if not df.dropna().empty and len(df.columns) > 1 and len(df) > 1:
-                # Serialize DataFrame
+                    for td_tag in td_tags:
+                        data = td_tag.xpath('.//text()').getall()
 
-                with open(path + '.pickle', 'wb') as pickle_file:
-                    pickle.dump(df, pickle_file)
+                        '''
+                            Some table cells include \n or unicode symbols,
+                            so that creates unneccesary "empty" columns and thus
+                            the number of columns doesn't meet the real one
+                        '''
 
-        elif 'bullet' in element_name:
-            data = process_bullet(xpath)
-            xpath += '//li//text()'
+                        data = [string_cleaner(x) for x in data]  # Cleaning the text
 
-            if len(data) > 1:
-                with open(path + '.pickle', 'wb') as pickle_file:
-                    pickle.dump(data, pickle_file)
+                        # data = list(filter(None, data))  # Deleting empty strings
 
-        elif 'image' in element_name:
-            xpath += '/@src'
-            data = page.xpath(xpath).extract()[0]
+                        row.append('\n'.join(data))  # Making one string value from list
 
-            if data:
-                # Handle images with relative path. E.g. images/logo.png
-                if not any([data.startswith(x) for x in ['http', 'www']]):
-                    data = url_pattern.match(browser.current_url).group(1) + data.replace('./', '')
+                    result.append(row)
 
-                with open(path + '.pickle', 'wb') as pickle_file:
-                    pickle.dump(data, pickle_file)
-        else:
-            if 'link' in element_name:
-                # Link tag may contain 2 types od data: link itself (href) and text, so prepare both
-                xpath_href = xpath + '/@href'
-                xpath_text = xpath + '//text()'
-
-                data = {
-                    'link': ''.join(page.xpath(xpath_href).extract()).strip(),
-                    'text': ''.join(page.xpath(xpath_text).extract()).strip()
-                }
+                    if not titles:  # If table doesn't have <th> tags -> use first row as titles
+                        titles = row  # TODO: IF USER SELECTS THE TABLE, ASK HIM, WHETHER HE WANTS TO HAVE 1 ROW AS TITLES
 
-            elif 'button' in element_name:
-                data = ''.join(page.xpath(xpath).extract()).strip()
+                try:
+                    # If number of columns' names (titles) is the same as number of columns
+                    df = pd.DataFrame(result, columns=titles)
+                except Exception:
+                    df = pd.DataFrame(result)
+
+                df = df.iloc[1:, :]  # Removing empty row at the beginning of dataframe
+
+                df.dropna(axis=0, how='all', inplace=True)
+
+                text = df
+
+                # # If dataframe is not empty
+                # if not df.dropna().empty and len(df.columns) > 1 and len(df) > 1:
+                #     # Serialize DataFrame
+                #
+                #     with open(path + '.pickle', 'wb') as pickle_file:
+                #         pickle.dump(df, pickle_file)
             else:
                 xpath += '//text()'
 
                 # Try to extract text from element
                 try:
-                    data = ''.join(page.xpath(xpath).extract()).strip()
+                    text = ''.join(self.page.xpath(xpath).extract()).strip()
                 # Extract element otherwise
                 except:
                     xpath = xpath.removesuffix('//text()')
-                    data = ''.join(page.xpath(xpath).extract()).strip()
-
-            if len(data) > 0:
-                with open(path + '.pickle', 'wb') as pickle_file:
-                    pickle.dump(data, pickle_file)
-
-        if 'context' in element_name:
-            data = None
-        else:
-            try:
-                data = pickle_file.name
-            except Exception as e:
-                data = None
-                docrawl_logger.error(f'Error while retrieving file with data: {e}')
+                    text = ''.join(self.page.xpath(xpath).extract()).strip()
 
+            # attributes = element.get_property('attributes')
+            attributes = self.browser.execute_script(
+                'var items = {}; for (index = 0; index < arguments[0].attributes.length; ++index) { items[arguments[0].attributes[index].name] = arguments[0].attributes[index].value }; return items;',
+                element)
+
+            # docrawl_logger.warning(attributes)
+            element_data = {
+                'tag_name': re.split('//|/', xpath)[-1].split('[')[0],
+                'text': text,
+                'attributes': attributes
+            }
 
-        final_elements.update({element_name:
-                                   {'selector': selector,
-                                    'data': data,
-                                    'xpath': xpath}})
+            return element_data
 
-    new_elements_all = []
+        new_elements_all = []
 
-    def find_elements(element_type: ElementType, custom_tags: list = None):
-        """
-        Finds elements on page using Selenium Selector and HTML Parser
-            :param element_type: type of element (table, bullet, text, headline, link, ...)
-            :param custom_tags: list of custom tags
-        """
+        def find_elements(element_type: ElementType, custom_tags: list = None):
+            """
+            Finds elements on page using Selenium Selector and HTML Parser
+                :param element_type: type of element (table, bullet, text, headline, link, ...)
+                :param custom_tags: list of custom tags
+            """
+
+            tags = PREDEFINED_TAGS[element_type] if not custom_tags else custom_tags
+            elements = []
+            elements_tree = []
+
+            # If tag is not predefined -> there is no need to add prefix
+            prefix = '' if custom_tags else '//'
+
+            for tag in tags:
+                elements.extend(self.browser.find_elements(By.XPATH, f'{prefix}{tag}'))
+                if custom_tags:
+                    tag = tag.replace('/body/', '/div/')  # Otherwise, elements_tree will be empty
+                elements_tree.extend(tree.xpath(f'{prefix}{tag}'))
+
+            if elements:
+                added_xpaths = []  # For deduplication of elements
+                for i, element in enumerate(elements):
+                    elem_name = f'{element_type}_{i}'
+
+                    # Skip tables with no rows
+                    if element_type == ElementType.TABLE and len(element.find_elements(By.XPATH, './/tr')) < 2:
+                        continue
+
+                    try:
+                        xpath = find_element_xpath(elements_tree, i)
+
+                        if xpath not in added_xpaths:
+                            element_data = extract_element_data(element=element, xpath=xpath, element_type=element_type)
+                            element_c = Element(name=elem_name, type=element_type, rect=element.rect, xpath=xpath,
+                                                data=element_data)
+                            new_elements_all.append(element_c.dict())
+                            added_xpaths.append(xpath)
+                        # serialize_and_append_data(f'{element_name}_{i}', element, xpath)
+
+                    except Exception as e:
+                        docrawl_logger.error(f'Error while extracting data for element {elem_name}: {e}')
+
+        def find_element_xpath(tree, i):
+            """
+            Finds the XPath of element using HTML parser.
+                :param tree: list of elements
+                :param i: element's number
+            """
+            xpath = tree[i].getroottree().getpath(tree[i])
+            xpath = xpath.split('/')
+            xpath[2] = 'body'  # For some reason getpath() generates <div> instead of <body>
+            xpath = '/'.join(xpath)
+
+            return xpath
+
+        ##### TABLES SECTION #####
+        if incl_tables:
+            find_elements(element_type=ElementType.TABLE)
+
+        ##### BULLET SECTION #####
+        if incl_bullets:
+            find_elements(element_type=ElementType.BULLET)
+
+        ##### TEXTS SECTION #####
+        if incl_texts:
+            find_elements(element_type=ElementType.TEXT)
+
+        ##### HEADLINES SECTION #####
+        if incl_headlines:
+            find_elements(element_type=ElementType.HEADLINE)
+
+        ##### LINKS SECTION #####
+        if incl_links:
+            find_elements(element_type=ElementType.LINK)
+
+        ##### IMAGES SECTION #####
+        if incl_images:
+            find_elements(element_type=ElementType.IMAGE)
+
+        ##### BUTTONS SECTION #####
+        if incl_buttons:
+            find_elements(element_type=ElementType.BUTTON)
+
+        ##### CUSTOM XPATH SECTION #####
+        if by_xpath:
+            # Temporary workaround due to weird behaviour of lists in kpv
+            if ';' in by_xpath:
+                list_of_xpaths = by_xpath.split(';')[:-1]
+            else:
+                list_of_xpaths = [by_xpath]
 
-        tags = PREDEFINED_TAGS[element_type] if not custom_tags else custom_tags
-        elements = []
-        elements_tree = []
+            for i, elem in enumerate(list_of_xpaths):
+                # With text() at the end will not work
+                xpath = elem.removesuffix('/text()').rstrip('/')
 
-        # If tag is not predefined -> there is no need to add prefix
-        prefix = '' if custom_tags else '//'
+                custom_tags = [xpath]
+                element_type = classify_element_by_xpath(xpath)
 
-        for tag in tags:
-            elements.extend(browser.find_elements(By.XPATH, f'{prefix}{tag}'))
-            if custom_tags:
-                tag = tag.replace('/body/', '/div/')  # Otherwise, elements_tree will be empty
-            elements_tree.extend(tree.xpath(f'{prefix}{tag}'))
+                find_elements(element_type=element_type, custom_tags=custom_tags)
 
-        if elements:
-            added_xpaths = []       # For deduplication of elements
-            for i, element in enumerate(elements):
-                elem_name = f'{element_type}_{i}'
+        if context_xpath:
+            try:
+                find_elements(element_type=ElementType.CONTEXT, custom_tags=[context_xpath])
+            except Exception as e:
+                docrawl_logger.error(f'Error while retrieving context elements: {e}')
 
-                # Skip tables with no rows
-                if element_type == ElementType.TABLE and len(element.find_elements(By.XPATH, './/tr')) < 2:
-                    continue
+        if cookies_xpath:
+            find_elements(element_type=ElementType.COOKIES, custom_tags=[cookies_xpath])
 
-                try:
-                    xpath = find_element_xpath(elements_tree, i)
+        ##### SAVING COORDINATES OF ELEMENTS #####
 
-                    if xpath not in added_xpaths:
-                        element_data = extract_element_data(element=element, xpath=xpath, element_type=element_type)
-                        element_c = Element(name=elem_name, type=element_type, rect=element.rect, xpath=xpath, data=element_data)
-                        new_elements_all.append(element_c.dict())
-                        added_xpaths.append(xpath)
-                    #serialize_and_append_data(f'{element_name}_{i}', element, xpath)
-
-                except Exception as e:
-                    docrawl_logger.error(f'Error while extracting data for element {elem_name}: {e}')
-
-    def find_element_xpath(tree, i):
-        """
-        Finds the XPath of element using HTML parser.
-            :param tree: list of elements
-            :param i: element's number
-        """
-        xpath = tree[i].getroottree().getpath(tree[i])
-        xpath = xpath.split('/')
-        xpath[2] = 'body'  # For some reason getpath() generates <div> instead of <body>
-        xpath = '/'.join(xpath)
-
-        return xpath
-
-    ##### TABLES SECTION #####
-    if incl_tables:
-        find_elements(element_type=ElementType.TABLE)
-
-    ##### BULLET SECTION #####
-    if incl_bullets:
-        find_elements(element_type=ElementType.BULLET)
-
-    ##### TEXTS SECTION #####
-    if incl_texts:
-        find_elements(element_type=ElementType.TEXT)
-
-    ##### HEADLINES SECTION #####
-    if incl_headlines:
-        find_elements(element_type=ElementType.HEADLINE)
-
-    ##### LINKS SECTION #####
-    if incl_links:
-        find_elements(element_type=ElementType.LINK)
-
-    ##### IMAGES SECTION #####
-    if incl_images:
-        find_elements(element_type=ElementType.IMAGE)
-
-    ##### BUTTONS SECTION #####
-    if incl_buttons:
-        find_elements(element_type=ElementType.BUTTON)
-
-    ##### CUSTOM XPATH SECTION #####
-    if by_xpath:
-        # Temporary workaround due to weird behaviour of lists in kpv
-        if ';' in by_xpath:
-            list_of_xpaths = by_xpath.split(';')[:-1]
-        else:
-            list_of_xpaths = [by_xpath]
+        self.docrawl_client.set_browser_scanned_elements(new_elements_all)
+        docrawl_logger.info(
+            f'Scan Web Page function duration {timedelta_format(datetime.datetime.now(), time_start_f)}')
 
-        for i, elem in enumerate(list_of_xpaths):
-            # With text() at the end will not work
-            xpath = elem.removesuffix('/text()').rstrip('/')
+    def _wait_until_element_is_located(self, inp):
+        """
+        Waits until certain element is located on page and then clicks on it.
+            :param browser: Selenium driver, browser instance
+            :param inp, list, inputs from launcher (xpath)
 
-            custom_tags = [xpath]
-            element_type = classify_element_by_xpath(xpath)
+        Note: click() method may be replaced with another
+        """
 
-            find_elements(element_type=element_type, custom_tags=custom_tags)
+        xpath = inp['xpath']
 
-    if context_xpath:
         try:
-            find_elements(element_type=ElementType.CONTEXT, custom_tags=[context_xpath])
+            WebDriverWait(self.browser, 5).until(EC.element_to_be_clickable((By.XPATH, xpath))).click()
         except Exception as e:
-            docrawl_logger.error(f'Error while retrieving context elements: {e}')
-
-    if cookies_xpath:
-        find_elements(element_type=ElementType.COOKIES, custom_tags=[cookies_xpath])
-
-    ##### SAVING COORDINATES OF ELEMENTS #####
-
-    # names = list(final_elements.keys())
-    # selectors = [x['selector'] for x in final_elements.values()]
-    # xpaths = [x['xpath'] for x in final_elements.values()]
-    # data = [x['data'] for x in final_elements.values()]
-    #
-    # save_coordinates_of_elements(selectors, names, xpaths, data)
-
-    kv_redis.set(key=kv_redis_key_webpage_elements, value=new_elements_all)
-    docrawl_logger.info(f'Scan Web Page function duration {timedelta_format(datetime.datetime.now(), time_start_f)}')
-
-
-def wait_until_element_is_located(browser, page, inp):
-    """
-    Waits until certain element is located on page and then clicks on it.
-        :param browser: Selenium driver, browser instance
-        :param inp, list, inputs from launcher (xpath)
-
-    Note: click() method may be replaced with another
-    """
-
-    xpath = inp['xpath']
-
-    try:
-        WebDriverWait(browser, 5).until(EC.element_to_be_clickable((By.XPATH, xpath))).click()
-    except Exception as e:
-        docrawl_logger.error(f'Error while locating element: {e}')
-
-
-def get_current_url(browser, page, inp):
-    """
-    Returns the URL of current opened website
-        :param page: :param browser: driver instance
-        :param inp: list, inputs from launcher (filename)
-    """
-
-    filename = inp['filename']
-    url = str(browser.current_url)
-
-    try:
-        with open(filename, 'w+', encoding="utf-8") as f:
-            f.write(url)
-    except Exception as e:
-        docrawl_logger.error(f'Error while getting current URL: {e}')
-
-
-def close_browser(browser, page, inp):
-    """
-    Closes browser (removes driver instance).
-        :param browser: driver instance
-    """
-
-    try:
-        browser.quit()
-        '''
-        if not browser.current_url:
-            time.sleep(1)
-            close_browser(browser)
-        '''
+            docrawl_logger.error(f'Error while locating element: {e}')
 
-        # Remove proxy after closing browser instance
-        proxy = {'ip': '', 'port': '', 'username': '', 'password': ''}
-        proxy = VarSafe(proxy, "proxy", "proxy")
-
-        save_variables(kept_variables, 'browser_meta_data.kpv')
-
-    except ConnectionRefusedError:
-        pass
-    except Exception as e:
-        docrawl_logger.error(f'Error while closing the browser: {e}')
-
-
-def scroll_web_page(browser, page, inp):
-    """
-    Scrolls page up / down by n-pixels.
-        :param browser: driver instance
-        :param inp: list, inputs from launcher (scroll_to, scroll_by, scroll_max)
-    """
-
-    scroll_to = inp['scroll_to']
-    scroll_by = inp['scroll_by']
-    scroll_max = inp['scroll_max']
-
-    script = ''
-
-    if scroll_to == 'Down':
-        if scroll_max:
-            script = 'window.scrollTo(0, document.body.scrollHeight);var lenOfPage=document.body.scrollHeight;return lenOfPage;'
-        else:
-            try:
-                # script = f'window.scrollBy(0, {scroll_by});'       # instant scrolling
-                script = f'window.scrollBy({{top: {scroll_by}, left: 0, behavior: "smooth"}});'  # smooth scrolling
-            except:
-                pass
-    elif scroll_to == 'Up':
-        if scroll_max:
-            script = 'window.scrollTo(0, 0)'
-        else:
-            try:
-                # script = f'window.scrollBy(0, -{scroll_by});'      # instant scrolling
-                script = f'window.scrollBy({{top: -{scroll_by}, left: 0, behavior: "smooth"}});'  # smooth scrolling
-            except:
-                pass
-
-    if script:
-        browser.execute_script(script)
-
-
-def download_images(browser, page, inp):
-    """
-    Downloads images using XPath
-        :param browser: driver instance
-        :param inp: list, inputs from launcher (image xpath, filename)
-    """
-
-    image_xpath = inp['image_xpath']
-    filename = inp['filename']
-    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64; rv:50.0) Gecko/20100101 Firefox/50.0'}
-
-    # If entered filename contains extension -> drop extension
-    if '.' in filename:
-        filename = filename.split('.')[0]
-
-    images = browser.find_elements(By.XPATH, image_xpath)
-
-    if len(images) == 0:
-        pass
-    elif len(images) == 1:
-        image_url = images[0].get_attribute('data-src')
-
-        if not image_url:
-            image_url = images[0].get_attribute('src')
-
-        image_extension = image_url.split('.')[-1].split('?')[0]  # Drop ?xxx after image extension
-
-        r = requests.get(image_url, headers=headers)
-        with open(f'{filename}.{image_extension}', 'wb') as outfile:
-            outfile.write(r.content)
-    else:
-        # Use provided filename as directory name. Images themselves will be filename_base_0, filename_base_1, filename_base_2 etc.
-        images_directory = filename
-        if not os.path.exists(images_directory):
-            os.mkdir(images_directory)
-
-        filename_base = filename
-
-        for i, image in enumerate(images):
-            try:
-                # Sometimes the image url is stored within data-src tag -> TODO: add new argument to handler with tag?
-                image_url = image.get_attribute('data-src')
-                if not image_url:
-                    image_url = image.get_attribute('src')
-
-                image_extension = image_url.split('.')[-1].split('?')[0]  # Drop ?xxx after image extension
-                filename = f'{filename_base}_{i}.{image_extension}'
-
-                r = requests.get(image_url, headers=headers)
-                with open(f'{images_directory}/{filename}', 'wb') as outfile:
-                    outfile.write(r.content)
-            except:
-                pass
-
-
-def click_xpath(browser, page, inp):
-    xpath = inp['xpath']
-
-    xpath = xpath.removesuffix('//text()').rstrip('/')
-    docrawl_logger.info(f'Searching for element to click: {xpath}')
-    element = browser.find_element(By.XPATH, xpath)
-
-    if element.is_enabled():
-        docrawl_logger.info('Button is enabled')
-        element.click()
-    else:
-        docrawl_logger.warning('Button is not enabled, trying to enable it')
-        browser.execute_script("arguments[0].removeAttribute('disabled','disabled')", element)
-        element.click()
-
-
-def click_name(browser, page, inp):
-    text = inp['text']
-
-    browser.find_element_by_link_text(text).click()
-
-
-def extract_xpath(browser, page, inp):
-    """
-    write_in_file_mode ... w+, a+
-    """
-    xpath = inp['xpath']
-    filename = inp['filename']  # "extracted_data.txt"
-
-    if not xpath.endswith('/text()') and not '@' in xpath.split('/')[-1]:
-        xpath += '/text()'
-
-    # Extract link from "a" tags
-    if xpath.split('/')[-1] == 'a' or xpath.split('/')[-1] == '/a' or xpath.split('/')[-1].startswith('a['):
-        xpath += '/@href'
+    def _get_current_url(self, inp):
+        """
+        Returns the URL of current opened website
+            :param page: :param browser: driver instance
+            :param inp: list, inputs from launcher (filename)
+        """
 
-    try:
-        write_in_file_mode = inp['write_in_file_mode']
-    except:
-        write_in_file_mode = "w+"
+        filename = inp['filename']
+        url = str(self.browser.current_url)
 
-    data = page.xpath(xpath).extract()
+        try:
+            with open(filename, 'w+', encoding="utf-8") as f:
+                f.write(url)
+        except Exception as e:
+            docrawl_logger.error(f'Error while getting current URL: {e}')
 
-    if not data:
-        data = ['None']
+    def _close_browser(self, inp):
+        """
+        Closes browser (removes driver instance).
+            :param browser: driver instance
+        """
 
-    with open(filename, write_in_file_mode, encoding="utf-8") as f:
-        if isinstance(data, list):
-            for i, row in enumerate(data):
-                row = row.strip()
+        try:
+            self.browser.quit()
+            '''
+            if not browser.current_url:
+                time.sleep(1)
+                close_browser(browser)
+            '''
 
-                if row:
-                    f.write(row.strip() + "\n")
-        else:
-            f.write(data.strip())
 
+            # Remove proxy after closing browser instance
+            proxy = {'ip': '', 'port': '', 'username': '', 'password': ''}
+            browser_meta_data = self.docrawl_client.get_browser_meta_data()
+            browser_meta_data['browser']['proxy'] = proxy
 
-def extract_multiple_xpaths(browser, page, inp):
-    result = []
-    xpaths = inp['xpaths']
-    filename = inp['filename']  # "extracted_data.txt"
+            self.docrawl_client.set_browser_meta_data(browser_meta_data)
 
-    for i, xpath in enumerate(xpaths):
-        data = page.xpath(xpath).extract()
-        docrawl_logger.info(f'Data from extracted XPath: {data}')
-        result.append(data)
+        except ConnectionRefusedError:
+            pass
+        except Exception as e:
+            docrawl_logger.error(f'Error while closing the browser: {e}')
 
-    short_filename = filename.split(".txt")[0]
-    df = pd.DataFrame(result)
-    df.to_excel(short_filename + ".xlsx")
+    def _scroll_web_page(self, inp):
+        """
+        Scrolls page up / down by n-pixels.
+            :param browser: driver instance
+            :param inp: list, inputs from launcher (scroll_to, scroll_by, scroll_max)
+        """
 
-    with open(filename, "w+", encoding="utf-8") as f:
-        pass
+        scroll_to = inp['scroll_to']
+        scroll_by = inp['scroll_by']
+        scroll_max = inp['scroll_max']
 
+        script = ''
 
-def extract_table_xpath(browser, page, inp):
-    row_xpath = inp['xpath_row']
-    column_xpath = inp['xpath_col']
-    filename = inp['filename']  # "extracted_data.txt"
-    first_row_header = inp['first_row_header']
-
-    result = []
-    trs = page.xpath(row_xpath)
-    ths = page.xpath(row_xpath + '//th')
-    headers = []
-
-    # Try to find headers within <th> tags
-    for th_tag in ths:
-        headers.append(''.join(th_tag.xpath('.//text()').extract()).replace('\n', '').replace('\t', ''))
-
-    if trs:
-        for j, tr in enumerate(trs):
-            xp = row_xpath + "[" + str(j + 1) + "]" + column_xpath
-
-            td_tags = page.xpath(xp)
-            row = []
-            for td in td_tags:
-                data = td.xpath('.//text()').getall()
-
-                '''r
-                    Some table cells include \n or unicode symbols,
-                    so that creates unneccesary "empty" columns and thus
-                    the number of columns doesn't meet the real one
-                '''
-
-                data = [''.join(x.strip()).replace('\\', '') for x in data]  # Cleaning the text
-
-                # data = list(filter(None, data))  # Deleting empty strings
-
-                row.append('\n'.join(data).strip())  # Making one string value from list
-
-            # details = page.xpath(xp).extract() #j+1 because xpath indices start with 1 (not with 0)
-
-            # If first row should be headers and headers were not defined before
-            if first_row_header and not headers:
-                headers = row
+        if scroll_to == 'Down':
+            if scroll_max:
+                script = 'window.scrollTo(0, document.body.scrollHeight);var lenOfPage=document.body.scrollHeight;return lenOfPage;'
             else:
-                result.append(row)
+                try:
+                    # script = f'window.scrollBy(0, {scroll_by});'       # instant scrolling
+                    script = f'window.scrollBy({{top: {scroll_by}, left: 0, behavior: "smooth"}});'  # smooth scrolling
+                except:
+                    pass
+        elif scroll_to == 'Up':
+            if scroll_max:
+                script = 'window.scrollTo(0, 0)'
+            else:
+                try:
+                    # script = f'window.scrollBy(0, -{scroll_by});'      # instant scrolling
+                    script = f'window.scrollBy({{top: -{scroll_by}, left: 0, behavior: "smooth"}});'  # smooth scrolling
+                except:
+                    pass
 
-    short_filename = filename.split(".pickle")[0]
+        if script:
+            self.browser.execute_script(script)
 
-    if headers:
-        # Could be the situation when len of headers is not the same as len of row
-        try:
-            df = pd.DataFrame(result, columns=headers)
-        except:
-            df = pd.DataFrame(result)
-    else:
-        df = pd.DataFrame(result)
+    def _download_images(self, inp):
+        """
+        Downloads images using XPath
+            :param browser: driver instance
+            :param inp: list, inputs from launcher (image xpath, filename)
+        """
 
-    # Remove empty rows
-    df.dropna(axis=0, how='all', inplace=True)
-    df.to_excel(short_filename + '.xlsx')
+        image_xpath = inp['image_xpath']
+        filename = inp['filename']
+        headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64; rv:50.0) Gecko/20100101 Firefox/50.0'}
 
-    kv_redis.set(key='extracted_table', value=df)
+        # If entered filename contains extension -> drop extension
+        if '.' in filename:
+            filename = filename.split('.')[0]
 
+        images = self.browser.find_elements(By.XPATH, image_xpath)
 
-class BrowserMetaData(UserDict):
-    """
-    Stores browser metadata such as driver, proxy, request and function info.
+        if len(images) == 0:
+            pass
+        elif len(images) == 1:
+            image_url = images[0].get_attribute('data-src')
 
-    Ensures synchronisation with .kpv file.
+            if not image_url:
+                image_url = images[0].get_attribute('src')
 
-    Expected structure:
+            image_extension = image_url.split('.')[-1].split('?')[0]  # Drop ?xxx after image extension
 
-    browser_metadata = {
-        "browser": {"driver": "Firefox", "headless": True, "browser_pid": 1234},
-        "proxy": {"ip": "192.123.23.2", "port": 17, "username": "qwerty", "password": "12345"},
-        "request": {"url": "https://forloop.ai", "loaded": True},
-        "function": {"name": "extract_xpath", "input": "/html/main/div[4]/span", "done": False}
-    }
-    """
+            r = requests.get(image_url, headers=headers)
+            with open(f'{filename}.{image_extension}', 'wb') as outfile:
+                outfile.write(r.content)
+        else:
+            # Use provided filename as directory name. Images themselves will be filename_base_0, filename_base_1, filename_base_2 etc.
+            images_directory = filename
+            if not os.path.exists(images_directory):
+                os.mkdir(images_directory)
 
-    def __init__(self, kpv_file: str = 'browser_meta_data.kpv'):
-        super().__init__()
+            filename_base = filename
 
-        self.kpv_file = kpv_file
-        self._set_init_values()
+            for i, image in enumerate(images):
+                try:
+                    # Sometimes the image url is stored within data-src tag -> TODO: add new argument to handler with tag?
+                    image_url = image.get_attribute('data-src')
+                    if not image_url:
+                        image_url = image.get_attribute('src')
+
+                    image_extension = image_url.split('.')[-1].split('?')[0]  # Drop ?xxx after image extension
+                    filename = f'{filename_base}_{i}.{image_extension}'
+
+                    r = requests.get(image_url, headers=headers)
+                    with open(f'{images_directory}/{filename}', 'wb') as outfile:
+                        outfile.write(r.content)
+                except:
+                    pass
 
-    def __str__(self):
-        """
-        Prints metadata in certain order.
-        """
+    def _click_xpath(self, inp):
+        xpath = inp['xpath']
 
-        elements_order = ['browser', 'proxy', 'request', 'function']
-        ordered_dict = dict()
+        xpath = xpath.removesuffix('//text()').rstrip('/')
+        docrawl_logger.info(f'Searching for element to click: {xpath}')
+        element = self.browser.find_element(By.XPATH, xpath)
+
+        if element.is_enabled():
+            docrawl_logger.info('Button is enabled')
+            element.click()
+        else:
+            docrawl_logger.warning('Button is not enabled, trying to enable it')
+            self.browser.execute_script("arguments[0].removeAttribute('disabled','disabled')", element)
+            element.click()
 
-        for elem in elements_order:
-            ordered_dict[elem] = self.data.get(elem)
+    def _click_name(self, inp):
+        text = inp['text']
 
-        return str(ordered_dict)
+        self.browser.find_element(By.LINK_TEXT(text)).click()
 
-    def _set_init_values(self):
+    def _extract_xpath(self, inp):
         """
-        Initial value for function must be set so crawler is able to start requests.
+        write_in_file_mode ... w+, a+
         """
+        xpath = inp['xpath']
+        filename = inp['filename']  # "extracted_data.txt"
 
-        init_function = {"name": "print", "input": "Bla", "done": False}
-        self.__setitem__('function', init_function)
+        if not xpath.endswith('/text()') and not '@' in xpath.split('/')[-1]:
+            xpath += '/text()'
 
-    def __setitem__(self, key, value):
-        VarSafe(value, key, key)
-        save_variables(kept_variables, self.kpv_file)
-        super().__setitem__(key, value)
+        # Extract link from "a" tags
+        if xpath.split('/')[-1] == 'a' or xpath.split('/')[-1] == '/a' or xpath.split('/')[-1].startswith('a['):
+            xpath += '/@href'
 
-    def __getitem__(self, key):
         try:
-            value = load_variable_safe(self.kpv_file, key)
-        except Exception as e:
-            value = None
-
-        # Update value in dict
-        self.__setitem__(key, value)
-
-        return self.data[key]
-
-
-class DocrawlSpider(scrapy.spiders.CrawlSpider):
-    name = "forloop"
-    # allowed_domains = ['google.com']
-
-    custom_settings = {
-        'LOG_LEVEL': 'ERROR',
-        'USER_AGENT': "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
-        'DEFAULT_REQUEST_HEADERS': {
-            'Referer': 'https://forloop.ai'
-        }
-        #   'CONCURRENT_REQUESTS' : '20',
-    }
+            write_in_file_mode = inp['write_in_file_mode']
+        except:
+            write_in_file_mode = "w+"
 
-    def __init__(self, *a, **kw):
-        # can be replaced for debugging with browser = webdriver.FireFox()
-        # self.browser = webdriver.PhantomJS(executable_path=PHANTOMJS_PATH, service_args=['--ignore-ssl-errors=true'])
-        #super().__init__(*a, **kw)
-        self.meta_data = BrowserMetaData()
-
-        # TODO: get rid of global variables
-        global kv_redis
-        global kv_redis_key_webpage_elements
-        global kv_redis_key_screenshot
+        data = self.page.xpath(xpath).extract()
 
-        kv_redis = kw['kv_redis']
-        kv_redis_keys = kw['kv_redis_keys']
+        if not data:
+            data = ['None']
 
-        kv_redis_key_webpage_elements = kv_redis_keys.get('elements', kv_redis_key_webpage_elements)
-        kv_redis_key_screenshot = kv_redis_keys.get('screenshot', kv_redis_key_screenshot)
+        with open(filename, write_in_file_mode, encoding="utf-8") as f:
+            if isinstance(data, list):
+                for i, row in enumerate(data):
+                    row = row.strip()
 
-        self.browser = self._initialise_browser()
+                    if row:
+                        f.write(row.strip() + "\n")
+            else:
+                f.write(data.strip())
 
-        browser_info = {
-            'driver': self.driver_type,
-            'headless': self.headless,
-            'browser_pid': self.browser_pid
-        }
+    def _extract_multiple_xpaths(self, inp):
+        result = []
+        xpaths = inp['xpaths']
+        filename = inp['filename']  # "extracted_data.txt"
 
-        self.meta_data['browser'] = browser_info
+        for i, xpath in enumerate(xpaths):
+            data = self.page.xpath(xpath).extract()
+            docrawl_logger.info(f'Data from extracted XPath: {data}')
+            result.append(data)
 
-        self.start_requests()
+        short_filename = filename.split(".txt")[0]
+        df = pd.DataFrame(result)
+        df.to_excel(short_filename + ".xlsx")
 
-    def _initialise_browser(self):
-        try:
-            self.driver_type = self.meta_data['browser']['driver']
-        except Exception as e:
-            docrawl_logger.error(f'Error while loading driver type information: {e}')
-            self.driver_type = 'Firefox'
+        with open(filename, "w+", encoding="utf-8") as f:
+            pass
 
-        try:
-            self.headless = self.meta_data['browser']['headless']
-        except Exception as e:
-            docrawl_logger.error(f'Error while loading headless mode information: {e}')
-            self.headless = False
+    def _extract_table_xpath(self, inp):
+        row_xpath = inp['xpath_row']
+        column_xpath = inp['xpath_col']
+        filename = inp['filename']  # "extracted_data.txt"
+        first_row_header = inp['first_row_header']
 
-        try:
-            proxy_info = self.meta_data['proxy']
-        except Exception as e:
-            docrawl_logger.error(f'Error while loading proxy information: {e}')
-            proxy_info = None
+        result = []
+        trs = self.page.xpath(row_xpath)
+        ths = self.page.xpath(row_xpath + '//th')
+        headers = []
+
+        # Try to find headers within <th> tags
+        for th_tag in ths:
+            headers.append(''.join(th_tag.xpath('.//text()').extract()).replace('\n', '').replace('\t', ''))
+
+        if trs:
+            for j, tr in enumerate(trs):
+                xp = row_xpath + "[" + str(j + 1) + "]" + column_xpath
 
-        if self.driver_type == 'Firefox':
-            capabilities = DesiredCapabilities.FIREFOX.copy()
-            self.options = FirefoxOptions()
-            capabilities["marionette"] = True
+                td_tags = self.page.xpath(xp)
+                row = []
+                for td in td_tags:
+                    data = td.xpath('.//text()').getall()
 
-            sw_options = self._set_proxy(proxy_info)
+                    '''r
+                        Some table cells include \n or unicode symbols,
+                        so that creates unneccesary "empty" columns and thus
+                        the number of columns doesn't meet the real one
+                    '''
 
-            if self.headless:
-                self.options.add_argument("--headless")
+                    data = [''.join(x.strip()).replace('\\', '') for x in data]  # Cleaning the text
 
-                # For headless mode different width of window is needed
-                window_size_x = 1450
+                    # data = list(filter(None, data))  # Deleting empty strings
 
-            try:
-                self.browser = webdriver.Firefox(options=self.options, capabilities=capabilities,
-                                                 service=Service(GeckoDriverManager().install()))
-            except Exception as e:
-                docrawl_logger.error(f'Error while creating Firefox instance {e}')
-                self.browser = webdriver.Firefox(options=self.options, capabilities=capabilities)
+                    row.append('\n'.join(data).strip())  # Making one string value from list
 
-        elif self.driver_type == 'Chrome':
-            capabilities = DesiredCapabilities.CHROME
-            self.options = ChromeOptions()
+                # details = page.xpath(xp).extract() #j+1 because xpath indices start with 1 (not with 0)
 
-            sw_options = self._set_proxy(proxy_info)
+                # If first row should be headers and headers were not defined before
+                if first_row_header and not headers:
+                    headers = row
+                else:
+                    result.append(row)
 
-            if self.headless:
-                self.options.add_argument("--headless")
-
-                # For headless mode different width of window is needed
-                window_size_x = 1450
+        short_filename = filename.split(".pickle")[0]
 
+        if headers:
+            # Could be the situation when len of headers is not the same as len of row
             try:
-                self.browser = webdriver.Chrome(options=self.options, desired_capabilities=capabilities,
-                                                executable_path=ChromeDriverManager().install())
+                df = pd.DataFrame(result, columns=headers)
             except:
-                pass
-
-        window_size_x = 1820
-
-        self.browser.set_window_size(window_size_x, 980)
-
-        self._determine_browser_pid()
-
-        return self.browser
-
-    def __del__(self):
-        self.browser.quit()
-
-    def _set_proxy(self, proxy_info: dict) -> dict:
-        """
-        Sets proxy before launching browser instance.
-        :param proxy_info: proxy params (ip, port, username, password)
-        """
-
-        # If proxy was not set
-        if proxy_info is None or any([not proxy_info['ip'], not proxy_info['port']]):
-            return None
-
-        proxy_ip = proxy_info['ip']
-        proxy_port = proxy_info['port']
-        proxy_username = proxy_info['username']
-        proxy_password = proxy_info['password']
-
-        if proxy_username and proxy_password:
-            proxy = f'http://{proxy_username}:{proxy_password}@{proxy_ip}:{proxy_port}'
-        else:
-            proxy = f'{proxy_ip}:{proxy_port}'
-
-        # Proxy with authentication
-        if 'http://' in proxy:
-            # selenium-wire proxy settings
-            sw_options = {
-                'proxy': {
-                    'http': proxy,
-                    'https': proxy,
-                    'no_proxy': 'localhost,127.0.0.1'
-                }
-            }
-
-        # Proxy without authentication
+                df = pd.DataFrame(result)
         else:
-            sw_options = None
-            firefox_proxies = Proxy()
-            firefox_proxies.ssl_proxy = proxy
-            firefox_proxies.http_proxy = proxy
-            firefox_proxies.proxy_type = ProxyType.MANUAL
-
-            self.options.proxy = firefox_proxies
-
-        return sw_options
-
-    def _determine_browser_pid(self):
-        self.browser_pid = None
-        try:
-            if self.driver_type == 'Firefox':
-                self.browser_pid = self.browser.capabilities['moz:processID']
-            elif self.driver_type == 'Chrome':
-                self.browser.service.process
-                browser_pid = psutil.Process(self.browser.service.process.pid)
-                self.browser_pid = browser_pid.pid
+            df = pd.DataFrame(result)
 
-            # self.browser_pid = VarSafe(self.browser_pid, "browser_pid", "browser_pid")
-            # save_variables(kept_variables, "scr_vars.kpv")
-            docrawl_logger.success(f'Browser PID: {self.browser_pid}')
-        except Exception as e:
-            docrawl_logger.error(f'Error while determining browser PID: {e}')
+        # Remove empty rows
+        df.dropna(axis=0, how='all', inplace=True)
+        df.to_excel(short_filename + '.xlsx')
 
-    def start_requests(self):
-        URLS = ['https://www.forloop.ai']
-        FUNCTIONS = [self.parse]
-        for i in range(len(URLS)):
-            yield scrapy.Request(url=URLS[i], callback=FUNCTIONS[i])  # yield
+        self.docrawl_client.kv_redis.set(key='extracted_table', value=df)
 
     def parse(self, response):
-        self.browser.get(self.meta_data['request']['url'])
+        self.browser.get(self.docrawl_client.get_browser_meta_data()['request']['url'])
 
         docrawl_core_done = False
-        page = Selector(text=self.browser.page_source)
 
         while not docrawl_core_done:
-            spider_request = self.meta_data['request']
-            spider_function = self.meta_data['function']
+            browser_meta_data = self.docrawl_client.get_browser_meta_data()
+            spider_request = browser_meta_data['request']
+            spider_function = browser_meta_data['function']
 
             try:
                 time.sleep(1)
                 docrawl_logger.info('Docrawl core loop')
-                docrawl_logger.info(f'Browser meta data: {self.meta_data}')
 
                 if not spider_request['loaded']:
                     self.browser.get(spider_request['url'])
-                    page = Selector(text=self.browser.page_source)
+                    self.page = Selector(text=self.browser.page_source)
 
                     spider_request['loaded'] = True
-                    self.meta_data['request'] = spider_request
+                    browser_meta_data['request'] = spider_request
+
+                    self.docrawl_client.set_browser_meta_data(browser_meta_data)
 
                 if not spider_function['done']:
                     function_str = spider_function['name']
-                    function = eval(function_str)
 
                     inp = spider_function['input']
                     docrawl_logger.info(f'Function input from docrawl core: {inp}')
 
-                    if function_str in FUNCTIONS.keys():
-                        FUNCTIONS[function_str](browser=self.browser, page=page, inp=inp)
-                    else:
-                        function(inp)
+                    getattr(self, f'_{function_str}')(inp=inp)
 
                     spider_function['done'] = True
-                    self.meta_data['function'] = spider_function
+                    browser_meta_data['function'] = spider_function
+
+                    self.docrawl_client.set_browser_meta_data(browser_meta_data)
 
-                page = Selector(text=self.browser.page_source)
             except KeyboardInterrupt:
                 break
-
-
-FUNCTIONS = {"click_xpath": click_xpath,
-             "click_name": click_name,
-             "extract_xpath": extract_xpath,
-             "extract_multiple_xpaths": extract_multiple_xpaths,
-             "extract_table_xpath": extract_table_xpath,
-             "get_current_url": get_current_url,
-             "scan_web_page": scan_web_page,
-             "close_browser": close_browser,
-             "extract_page_source": extract_page_source,
-             "wait_until_element_is_located": wait_until_element_is_located,
-             "take_screenshot": take_screenshot,
-             "take_png_screenshot": take_png_screenshot,
-             "scroll_web_page": scroll_web_page,
-             "download_images": download_images,
-             }
+            except Exception as e:
+                docrawl_logger.error(f'Error while executing docrawl loop: {e}')
```

### Comparing `docrawl-0.5.1/docrawl/docrawl_launcher.py` & `docrawl-1.0.0/docrawl/docrawl_launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+
+TO BE DEPRECATED
+
+"""
+
+
 import docrawl.docrawl_core as docrawl_core
 from scrapy.crawler import CrawlerRunner
 from crochet import setup
 import keepvariable.keepvariable_core as kv
 import time
 from typing import Optional
 from docrawl.docrawl_logger import docrawl_logger
@@ -37,15 +44,15 @@
 def take_png_screenshot(filename):
     """
     Launches take_screenshot from core.
         :param filename: string, output filename (where to save the screenshot)
     """
 
     inp = {
-        'filename': filename
+        'filename': str(filename)       # Cast to str, e.g. when Path object is passed
     }
     run_function('take_png_screenshot', inp)
 
 
 def extract_page_source(filename):
     """
     Launches extract_page_source from core.
```

### Comparing `docrawl-0.5.1/docrawl/docrawl_logger.py` & `docrawl-1.0.0/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.5.1/docrawl/elements.py` & `docrawl-1.0.0/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.5.1/docrawl.egg-info/PKG-INFO` & `docrawl-1.0.0/docrawl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.5.1
+Version: 1.0.0
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.5.1/setup.py` & `docrawl-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='0.5.1',
+    version='1.0.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```


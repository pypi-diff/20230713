# Comparing `tmp/ural-0.8.0.tar.gz` & `tmp/ural-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ural-0.8.0.tar", last modified: Tue Apr 30 12:28:35 2019, max compression
+gzip compressed data, was "dist/ural-0.9.0.tar", last modified: Thu Sep 12 14:48:18 2019, max compression
```

## Comparing `ural-0.8.0.tar` & `ural-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-04-30 12:28:35.000000 ural-0.8.0/
--rw-r--r--   0 Yomgui     (501) staff       (20)     9375 2019-04-30 12:28:35.000000 ural-0.8.0/PKG-INFO
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/
--rw-r--r--   0 Yomgui     (501) staff       (20)     9375 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/zip-safe
--rw-r--r--   0 Yomgui     (501) staff       (20)      610 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/SOURCES.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       49 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/entry_points.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       48 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/requires.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        5 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/top_level.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2019-04-30 12:28:35.000000 ural-0.8.0/ural.egg-info/dependency_links.txt
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-04-30 12:28:35.000000 ural-0.8.0/ural/
--rw-r--r--   0 Yomgui     (501) staff       (20)     1569 2019-04-03 13:45:15.000000 ural-0.8.0/ural/normalized_lru_from_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      820 2019-04-17 12:03:58.000000 ural-0.8.0/ural/is_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      710 2018-12-13 17:12:14.000000 ural-0.8.0/ural/patterns.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      841 2018-12-14 10:39:22.000000 ural-0.8.0/ural/urls_from_html.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      504 2019-04-17 12:09:02.000000 ural-0.8.0/ural/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      931 2018-12-13 17:12:14.000000 ural-0.8.0/ural/force_protocol.py
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-04-30 12:28:35.000000 ural-0.8.0/ural/cli/
--rw-r--r--   0 Yomgui     (501) staff       (20)      749 2019-04-17 12:17:03.000000 ural-0.8.0/ural/cli/domain.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1116 2019-01-12 17:44:10.000000 ural-0.8.0/ural/cli/normalize.py
--rw-r--r--   0 Yomgui     (501) staff       (20)        0 2019-01-12 17:44:10.000000 ural-0.8.0/ural/cli/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1806 2019-02-21 10:04:26.000000 ural-0.8.0/ural/cli/join.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      423 2019-01-12 17:44:10.000000 ural-0.8.0/ural/cli/utils.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     4022 2019-04-17 12:18:34.000000 ural-0.8.0/ural/cli/__main__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1538 2019-04-03 13:45:18.000000 ural-0.8.0/ural/lru_from_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      547 2018-11-12 15:03:34.000000 ural-0.8.0/ural/strip_protocol.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     5748 2019-04-30 12:27:19.000000 ural-0.8.0/ural/normalize_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      875 2018-12-13 17:12:14.000000 ural-0.8.0/ural/ensure_protocol.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      656 2018-12-14 10:39:37.000000 ural-0.8.0/ural/urls_from_text.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      566 2019-04-17 12:08:35.000000 ural-0.8.0/ural/get_domain_name.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      930 2019-02-21 10:04:26.000000 ural-0.8.0/ural/lru_trie.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     6626 2019-04-30 12:27:19.000000 ural-0.8.0/README.md
--rw-r--r--   0 Yomgui     (501) staff       (20)      897 2019-04-30 12:27:25.000000 ural-0.8.0/setup.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       38 2019-04-30 12:28:35.000000 ural-0.8.0/setup.cfg
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    11013 2019-09-12 14:48:18.000000 ural-0.9.0/PKG-INFO
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    11013 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2019-09-12 14:47:54.000000 ural-0.9.0/ural.egg-info/zip-safe
+-rw-r--r--   0 Yomgui     (501) staff       (20)      627 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/SOURCES.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       49 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/entry_points.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       48 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/requires.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        5 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/top_level.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/dependency_links.txt
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/ural/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1569 2019-04-03 13:45:15.000000 ural-0.9.0/ural/normalized_lru_from_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      820 2019-04-17 12:03:58.000000 ural-0.9.0/ural/is_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      710 2018-12-13 17:12:14.000000 ural-0.9.0/ural/patterns.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      841 2018-12-14 10:39:22.000000 ural-0.9.0/ural/urls_from_html.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      690 2019-05-13 14:14:51.000000 ural-0.9.0/ural/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      931 2018-12-13 17:12:14.000000 ural-0.9.0/ural/force_protocol.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/ural/cli/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      749 2019-04-17 12:17:03.000000 ural-0.9.0/ural/cli/domain.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1116 2019-01-12 17:44:10.000000 ural-0.9.0/ural/cli/normalize.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)        0 2019-01-12 17:44:10.000000 ural-0.9.0/ural/cli/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1806 2019-02-21 10:04:26.000000 ural-0.9.0/ural/cli/join.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      423 2019-01-12 17:44:10.000000 ural-0.9.0/ural/cli/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4022 2019-04-17 12:18:34.000000 ural-0.9.0/ural/cli/__main__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2272 2019-09-12 14:44:13.000000 ural-0.9.0/ural/facebook.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1538 2019-04-03 13:45:18.000000 ural-0.9.0/ural/lru_from_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      547 2018-11-12 15:03:34.000000 ural-0.9.0/ural/strip_protocol.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     6144 2019-06-25 15:30:43.000000 ural-0.9.0/ural/normalize_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      875 2019-05-13 14:14:55.000000 ural-0.9.0/ural/ensure_protocol.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      656 2018-12-14 10:39:37.000000 ural-0.9.0/ural/urls_from_text.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      566 2019-04-17 12:08:35.000000 ural-0.9.0/ural/get_domain_name.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      930 2019-02-21 10:04:26.000000 ural-0.9.0/ural/lru_trie.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     7944 2019-09-12 14:39:48.000000 ural-0.9.0/README.md
+-rw-r--r--   0 Yomgui     (501) staff       (20)      889 2019-09-12 14:46:58.000000 ural-0.9.0/setup.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       38 2019-09-12 14:48:18.000000 ural-0.9.0/setup.cfg
```

### Comparing `ural-0.8.0/PKG-INFO` & `ural-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ural
-Version: 0.8.0
+Version: 0.9.0
 Summary: A helper library full of URL-related heuristics.
 Home-page: http://github.com/medialab/ural
 Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://travis-ci.org/medialab/ural.svg)](https://travis-ci.org/medialab/ural)
         
@@ -20,25 +20,33 @@
         pip install ural
         ```
         
         ## Usage
         
         ### Functions
         
+        *Generic functions*
+        
         * [ensure_protocol](#ensure_protocol)
         * [get_domain_name](#get_domain_name)
         * [force_protocol](#force_protocol)
         * [is_url](#is_url)
         * [lru_from_url](#lru_from_url)
         * [normalize_url](#normalize_url)
         * [normalized_lru_from_url](#normalized_lru_from_url)
         * [strip_protocol](#strip_protocol)
         * [urls_from_html](#urls_from_html)
         * [urls_from_text](#urls_from_text)
         
+        *Platform-specific functions*
+        
+        * [facebook](#facebook)
+          * [convert_facebook_url_to_mobile](#convert_facebook_url_to_mobile)
+          * [extract_user_from_url](#extract_user_from_url)
+        
         ### Classes
         
         * [LRUTrie](#LRUTrie)
           * [set](#set)
           * [match](#match)
           * [values](#values)
         
@@ -148,17 +156,18 @@
         ```
         
         *Arguments*
         
         * **url** *string*: URL to normalize.
         * **sort_query** *boolean* [`True`]: whether to sort query items.
         * **strip_authentication** *boolean* [`True`]: whether to strip authentication.
+        * **strip_fragment** *boolean|str* [`'except-routing'`]: whether to strip the url's fragment. If set to `except-routing`, will only strip the fragment if the fragment is not deemed to be js routing (i.e. if it contains a `/`).
         * **strip_index** *boolean* [`True`]: whether to strip trailing index.
-        * **strip_trailing_slash** *boolean* [`False`]: whether to strip trailing slash.
         * **strip_lang_subdomains** *boolean* [`False`]: whether to strip language subdomains (ex: 'fr-FR.lemonde.fr' to only 'lemonde.fr' because 'fr-FR' isn't a relevant subdomain, it indicates the language and the country).
+        * **strip_trailing_slash** *boolean* [`False`]: whether to strip trailing slash.
         
         ---
         
         #### normalized_lru_from_url
         
         Function normalizing url and returning its parts in hierarchical order.
         
@@ -229,14 +238,45 @@
         
         *Arguments*
         
         * **string** *string*: source string.
         
         ---
         
+        ### Facebook
+        
+        #### convert_facebook_url_to_mobile
+        
+        Function returning the mobile version of the given Facebook url. Will raise an exception if a non-Facebook url is given.
+        
+        ```python
+        from ural.facebook import convert_facebook_url_to_mobile
+        
+        convert_facebook_url_to_mobile('http://www.facebook.com/post/974583586343')
+        >>> 'http://m.facebook.com/post/974583586343'
+        ```
+        
+        ---
+        
+        #### extract_user_from_url
+        
+        Function extracting user information from a facebook user url.
+        
+        ```python
+        from ural.facebook import extract_user_from_url
+        
+        extract_user_from_url('https://www.facebook.com/people/Sophia-Aman/102016783928989')
+        >>> FacebookUser(id='102016783928989', handle=None, url='https://www.facebook.com/profile.php?id=102016783928989)
+        
+        extract_user_from_url('/annelaure.rivolu?rc=p&__tn__=R')
+        >>> FacebookUser(id=None, handle='annelaure.rivolu', url='https://www.facebook.com/annelaure.rivolu)
+        ```
+        
+        ---
+        
         ### Classes
         
         #### LRUTrie
         
         Class implementing a prefix tree (Trie) storing LRUs and their metadata, allowing to find the longest common prefix between two urls.
         
         ##### set
```

### Comparing `ural-0.8.0/ural.egg-info/PKG-INFO` & `ural-0.9.0/ural.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ural
-Version: 0.8.0
+Version: 0.9.0
 Summary: A helper library full of URL-related heuristics.
 Home-page: http://github.com/medialab/ural
 Author: Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://travis-ci.org/medialab/ural.svg)](https://travis-ci.org/medialab/ural)
         
@@ -20,25 +20,33 @@
         pip install ural
         ```
         
         ## Usage
         
         ### Functions
         
+        *Generic functions*
+        
         * [ensure_protocol](#ensure_protocol)
         * [get_domain_name](#get_domain_name)
         * [force_protocol](#force_protocol)
         * [is_url](#is_url)
         * [lru_from_url](#lru_from_url)
         * [normalize_url](#normalize_url)
         * [normalized_lru_from_url](#normalized_lru_from_url)
         * [strip_protocol](#strip_protocol)
         * [urls_from_html](#urls_from_html)
         * [urls_from_text](#urls_from_text)
         
+        *Platform-specific functions*
+        
+        * [facebook](#facebook)
+          * [convert_facebook_url_to_mobile](#convert_facebook_url_to_mobile)
+          * [extract_user_from_url](#extract_user_from_url)
+        
         ### Classes
         
         * [LRUTrie](#LRUTrie)
           * [set](#set)
           * [match](#match)
           * [values](#values)
         
@@ -148,17 +156,18 @@
         ```
         
         *Arguments*
         
         * **url** *string*: URL to normalize.
         * **sort_query** *boolean* [`True`]: whether to sort query items.
         * **strip_authentication** *boolean* [`True`]: whether to strip authentication.
+        * **strip_fragment** *boolean|str* [`'except-routing'`]: whether to strip the url's fragment. If set to `except-routing`, will only strip the fragment if the fragment is not deemed to be js routing (i.e. if it contains a `/`).
         * **strip_index** *boolean* [`True`]: whether to strip trailing index.
-        * **strip_trailing_slash** *boolean* [`False`]: whether to strip trailing slash.
         * **strip_lang_subdomains** *boolean* [`False`]: whether to strip language subdomains (ex: 'fr-FR.lemonde.fr' to only 'lemonde.fr' because 'fr-FR' isn't a relevant subdomain, it indicates the language and the country).
+        * **strip_trailing_slash** *boolean* [`False`]: whether to strip trailing slash.
         
         ---
         
         #### normalized_lru_from_url
         
         Function normalizing url and returning its parts in hierarchical order.
         
@@ -229,14 +238,45 @@
         
         *Arguments*
         
         * **string** *string*: source string.
         
         ---
         
+        ### Facebook
+        
+        #### convert_facebook_url_to_mobile
+        
+        Function returning the mobile version of the given Facebook url. Will raise an exception if a non-Facebook url is given.
+        
+        ```python
+        from ural.facebook import convert_facebook_url_to_mobile
+        
+        convert_facebook_url_to_mobile('http://www.facebook.com/post/974583586343')
+        >>> 'http://m.facebook.com/post/974583586343'
+        ```
+        
+        ---
+        
+        #### extract_user_from_url
+        
+        Function extracting user information from a facebook user url.
+        
+        ```python
+        from ural.facebook import extract_user_from_url
+        
+        extract_user_from_url('https://www.facebook.com/people/Sophia-Aman/102016783928989')
+        >>> FacebookUser(id='102016783928989', handle=None, url='https://www.facebook.com/profile.php?id=102016783928989)
+        
+        extract_user_from_url('/annelaure.rivolu?rc=p&__tn__=R')
+        >>> FacebookUser(id=None, handle='annelaure.rivolu', url='https://www.facebook.com/annelaure.rivolu)
+        ```
+        
+        ---
+        
         ### Classes
         
         #### LRUTrie
         
         Class implementing a prefix tree (Trie) storing LRUs and their metadata, allowing to find the longest common prefix between two urls.
         
         ##### set
```

### Comparing `ural-0.8.0/ural.egg-info/SOURCES.txt` & `ural-0.9.0/ural.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 ural/__init__.py
 ural/ensure_protocol.py
+ural/facebook.py
 ural/force_protocol.py
 ural/get_domain_name.py
 ural/is_url.py
 ural/lru_from_url.py
 ural/lru_trie.py
 ural/normalize_url.py
 ural/normalized_lru_from_url.py
```

### Comparing `ural-0.8.0/ural/normalized_lru_from_url.py` & `ural-0.9.0/ural/normalized_lru_from_url.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/is_url.py` & `ural-0.9.0/ural/is_url.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/patterns.py` & `ural-0.9.0/ural/patterns.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/urls_from_html.py` & `ural-0.9.0/ural/urls_from_html.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/force_protocol.py` & `ural-0.9.0/ural/force_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/cli/domain.py` & `ural-0.9.0/ural/cli/domain.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/cli/normalize.py` & `ural-0.9.0/ural/cli/normalize.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/cli/join.py` & `ural-0.9.0/ural/cli/join.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/cli/__main__.py` & `ural-0.9.0/ural/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/lru_from_url.py` & `ural-0.9.0/ural/lru_from_url.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/strip_protocol.py` & `ural-0.9.0/ural/strip_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/normalize_url.py` & `ural-0.9.0/ural/normalize_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
     from urllib.parse import parse_qsl, urlsplit, urlunsplit
 except ImportError:
     from urlparse import parse_qsl, urlsplit, urlunsplit
 
 from ural.patterns import PROTOCOL_RE
 
 IRRELEVANT_QUERY_RE = re.compile(
-    r'^(?:__twitter_impression|echobox|fbclid|utm_.+|amp_.+|amp|s?een|xt(?:loc|ref|cr|np|or|s))$', re.I)
+    r'^(?:__twitter_impression|echobox|fbclid|fref|utm_.+|amp_.+|amp|s?een|xt(?:loc|ref|cr|np|or|s))$', re.I)
 
 IRRELEVANT_SUBDOMAIN_RE = re.compile(r'\b(?:www\d?|mobile|m)\.', re.I)
 
 IRRELEVANT_QUERY_COMBOS = {
-    'ref': ('fb', 'tw', 'tw_i'),
+    'ref': ('fb', 'ts', 'tw', 'tw_i'),
     'platform': ('hootsuite')
 }
 
 
 def attempt_to_decode_idna(string):
     try:
         return string.encode('utf8').decode('idna')
@@ -51,15 +51,17 @@
     if key in IRRELEVANT_QUERY_COMBOS:
         return value in IRRELEVANT_QUERY_COMBOS[key]
 
     return False
 
 
 def normalize_url(url, parsed=False, sort_query=True, strip_authentication=True,
-                  strip_trailing_slash=False, strip_index=True, strip_protocol=True, strip_irrelevant_subdomain=True, strip_lang_subdomains=False):
+                  strip_trailing_slash=False, strip_index=True, strip_protocol=True,
+                  strip_irrelevant_subdomain=True, strip_lang_subdomains=False,
+                  strip_fragment='except-routing'):
     """
     Function normalizing the given url by stripping it of usually
     non-discriminant parts such as irrelevant query items or sub-domains etc.
 
     This is a very useful utility when attempting to match similar urls
     written slightly differently when shared on social media etc.
 
@@ -72,14 +74,18 @@
         strip_trailing_slash (bool, optional): Whether to drop trailing slash.
             Defaults to `False`.
         strip_index (bool, optional): Whether to drop trailing index at the end
             of the url. Defaults to `True`.
         strip_lang_subdomains (bool, optional): Whether to drop language subdomains
             (ex: 'fr-FR.lemonde.fr' to only 'lemonde.fr' because 'fr-FR' isn't a relevant subdomain, it indicates the language and the country).
             Defaults to `False`.
+        strip_fragment (bool|str, optional): Whether to drop non-routing fragment from the url?
+            If set to `except-routing` will only drop non-routing fragment (i.e. fragments that
+            do not contain a "/").
+            Defaults to `except-routing`.
 
     Returns:
         string: The normalized url.
 
     """
 
     has_protocol = PROTOCOL_RE.match(url)
@@ -134,16 +140,17 @@
 
         if sort_query:
             qsl = sorted(qsl)
 
         query = '&'.join(qsl)
 
     # Dropping fragment if it's not routing
-    if fragment and len(fragment.split('/')) <= 1:
-        fragment = ''
+    if fragment and strip_fragment:
+        if strip_fragment is True or '/' not in fragment:
+            fragment = ''
 
     # Dropping irrelevant subdomains
     if strip_irrelevant_subdomain:
         netloc = re.sub(
             IRRELEVANT_SUBDOMAIN_RE,
             '',
             netloc
```

### Comparing `ural-0.8.0/ural/ensure_protocol.py` & `ural-0.9.0/ural/ensure_protocol.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/urls_from_text.py` & `ural-0.9.0/ural/urls_from_text.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/get_domain_name.py` & `ural-0.9.0/ural/get_domain_name.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/ural/lru_trie.py` & `ural-0.9.0/ural/lru_trie.py`

 * *Files identical despite different names*

### Comparing `ural-0.8.0/README.md` & `ural-0.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,25 +12,33 @@
 pip install ural
 ```
 
 ## Usage
 
 ### Functions
 
+*Generic functions*
+
 * [ensure_protocol](#ensure_protocol)
 * [get_domain_name](#get_domain_name)
 * [force_protocol](#force_protocol)
 * [is_url](#is_url)
 * [lru_from_url](#lru_from_url)
 * [normalize_url](#normalize_url)
 * [normalized_lru_from_url](#normalized_lru_from_url)
 * [strip_protocol](#strip_protocol)
 * [urls_from_html](#urls_from_html)
 * [urls_from_text](#urls_from_text)
 
+*Platform-specific functions*
+
+* [facebook](#facebook)
+  * [convert_facebook_url_to_mobile](#convert_facebook_url_to_mobile)
+  * [extract_user_from_url](#extract_user_from_url)
+
 ### Classes
 
 * [LRUTrie](#LRUTrie)
   * [set](#set)
   * [match](#match)
   * [values](#values)
 
@@ -140,17 +148,18 @@
 ```
 
 *Arguments*
 
 * **url** *string*: URL to normalize.
 * **sort_query** *boolean* [`True`]: whether to sort query items.
 * **strip_authentication** *boolean* [`True`]: whether to strip authentication.
+* **strip_fragment** *boolean|str* [`'except-routing'`]: whether to strip the url's fragment. If set to `except-routing`, will only strip the fragment if the fragment is not deemed to be js routing (i.e. if it contains a `/`).
 * **strip_index** *boolean* [`True`]: whether to strip trailing index.
-* **strip_trailing_slash** *boolean* [`False`]: whether to strip trailing slash.
 * **strip_lang_subdomains** *boolean* [`False`]: whether to strip language subdomains (ex: 'fr-FR.lemonde.fr' to only 'lemonde.fr' because 'fr-FR' isn't a relevant subdomain, it indicates the language and the country).
+* **strip_trailing_slash** *boolean* [`False`]: whether to strip trailing slash.
 
 ---
 
 #### normalized_lru_from_url
 
 Function normalizing url and returning its parts in hierarchical order.
 
@@ -221,14 +230,45 @@
 
 *Arguments*
 
 * **string** *string*: source string.
 
 ---
 
+### Facebook
+
+#### convert_facebook_url_to_mobile
+
+Function returning the mobile version of the given Facebook url. Will raise an exception if a non-Facebook url is given.
+
+```python
+from ural.facebook import convert_facebook_url_to_mobile
+
+convert_facebook_url_to_mobile('http://www.facebook.com/post/974583586343')
+>>> 'http://m.facebook.com/post/974583586343'
+```
+
+---
+
+#### extract_user_from_url
+
+Function extracting user information from a facebook user url.
+
+```python
+from ural.facebook import extract_user_from_url
+
+extract_user_from_url('https://www.facebook.com/people/Sophia-Aman/102016783928989')
+>>> FacebookUser(id='102016783928989', handle=None, url='https://www.facebook.com/profile.php?id=102016783928989)
+
+extract_user_from_url('/annelaure.rivolu?rc=p&__tn__=R')
+>>> FacebookUser(id=None, handle='annelaure.rivolu', url='https://www.facebook.com/annelaure.rivolu)
+```
+
+---
+
 ### Classes
 
 #### LRUTrie
 
 Class implementing a prefix tree (Trie) storing LRUs and their metadata, allowing to find the longest common prefix between two urls.
 
 ##### set
```

### Comparing `ural-0.8.0/setup.py` & `ural-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r') as f:
     long_description = f.read()
 
 setup(name='ural',
-      version='0.8.0',
+      version='0.9.0',
       description='A helper library full of URL-related heuristics.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/medialab/ural',
       license='MIT',
       author='Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou',
       author_email='kropotkinepiotr@gmail.com',
       keywords='url',
       python_requires='>=2.7',
       packages=find_packages(exclude=['test']),
       package_data={'docs': ['README.md']},
       install_requires=[
-          'phylactery>=0.2.2',
-          'pycountry>=18.12.8',
-          'tld>=0.9.3'
+        'phylactery>=0.2.2',
+        'pycountry>=18.12.8',
+        'tld>=0.9.3'
       ],
       entry_points={
-          'console_scripts': ['ural=ural.cli.__main__:main']
+        'console_scripts': ['ural=ural.cli.__main__:main']
       },
       zip_safe=True)
```


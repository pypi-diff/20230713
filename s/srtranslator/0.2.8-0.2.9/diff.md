# Comparing `tmp/srtranslator-0.2.8.tar.gz` & `tmp/srtranslator-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srtranslator-0.2.8.tar", last modified: Tue Jun 20 18:44:52 2023, max compression
+gzip compressed data, was "srtranslator-0.2.9.tar", last modified: Wed Jul 12 23:32:50 2023, max compression
```

## Comparing `srtranslator-0.2.8.tar` & `srtranslator-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.084520 srtranslator-0.2.8/
--rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.8/LICENSE.md
--rw-rw-rw-   0        0        0     2923 2023-06-20 18:44:52.084520 srtranslator-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2518 2023-06-20 18:44:06.000000 srtranslator-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 18:44:52.085520 srtranslator-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-06-20 18:44:20.000000 srtranslator-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.076513 srtranslator-0.2.8/srtranslator/
--rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.8/srtranslator/__init__.py
--rw-rw-rw-   0        0        0     2455 2023-06-08 15:16:00.000000 srtranslator-0.2.8/srtranslator/__main__.py
--rw-rw-rw-   0        0        0     6026 2023-05-05 15:00:20.000000 srtranslator-0.2.8/srtranslator/srt_file.py
-drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.083518 srtranslator-0.2.8/srtranslator/translators/
--rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.8/srtranslator/translators/__init__.py
--rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.8/srtranslator/translators/base.py
--rw-rw-rw-   0        0        0      445 2023-03-31 14:58:33.000000 srtranslator-0.2.8/srtranslator/translators/deepl_api.py
--rw-rw-rw-   0        0        0     5476 2023-06-20 18:42:52.000000 srtranslator-0.2.8/srtranslator/translators/deepl_scrap.py
--rw-rw-rw-   0        0        0     1074 2023-06-12 14:36:42.000000 srtranslator-0.2.8/srtranslator/translators/deeplx.py
--rw-rw-rw-   0        0        0     4235 2023-05-04 18:23:52.000000 srtranslator-0.2.8/srtranslator/translators/selenium_utils.py
--rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.8/srtranslator/translators/translatepy.py
-drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.079515 srtranslator-0.2.8/srtranslator.egg-info/
--rw-rw-rw-   0        0        0     2923 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      657 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 23:32:50.561935 srtranslator-0.2.9/
+-rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.9/LICENSE.md
+-rw-rw-rw-   0        0        0     2923 2023-07-12 23:32:50.560934 srtranslator-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2518 2023-06-20 18:44:06.000000 srtranslator-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 23:32:50.561935 srtranslator-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-07-12 23:32:24.000000 srtranslator-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:32:50.552927 srtranslator-0.2.9/srtranslator/
+-rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.9/srtranslator/__init__.py
+-rw-rw-rw-   0        0        0     2455 2023-06-08 15:16:00.000000 srtranslator-0.2.9/srtranslator/__main__.py
+-rw-rw-rw-   0        0        0     6026 2023-05-05 15:00:20.000000 srtranslator-0.2.9/srtranslator/srt_file.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:32:50.559933 srtranslator-0.2.9/srtranslator/translators/
+-rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.9/srtranslator/translators/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.9/srtranslator/translators/base.py
+-rw-rw-rw-   0        0        0      445 2023-07-12 23:31:46.000000 srtranslator-0.2.9/srtranslator/translators/deepl_api.py
+-rw-rw-rw-   0        0        0     5476 2023-07-12 23:31:03.000000 srtranslator-0.2.9/srtranslator/translators/deepl_scrap.py
+-rw-rw-rw-   0        0        0      303 2023-06-28 20:10:58.000000 srtranslator-0.2.9/srtranslator/translators/deeplcli.py
+-rw-rw-rw-   0        0        0     1074 2023-06-12 14:36:42.000000 srtranslator-0.2.9/srtranslator/translators/deeplx.py
+-rw-rw-rw-   0        0        0     4235 2023-05-04 18:23:52.000000 srtranslator-0.2.9/srtranslator/translators/selenium_utils.py
+-rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.9/srtranslator/translators/translatepy.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:32:50.554929 srtranslator-0.2.9/srtranslator.egg-info/
+-rw-rw-rw-   0        0        0     2923 2023-07-12 23:32:50.000000 srtranslator-0.2.9/srtranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-12 23:32:50.000000 srtranslator-0.2.9/srtranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:32:50.000000 srtranslator-0.2.9/srtranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      657 2023-07-12 23:32:50.000000 srtranslator-0.2.9/srtranslator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 23:32:50.000000 srtranslator-0.2.9/srtranslator.egg-info/top_level.txt
```

### Comparing `srtranslator-0.2.8/PKG-INFO` & `srtranslator-0.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: srtranslator
-Version: 0.2.8
-Summary: Traslate a .SRT file using any custom translator
-Home-page: https://github.com/sinedie/SRTranslator
-Author: EAR
-Author-email: sinedie@protonmail.com
-License: FREE
-Keywords: python,srt,languages,translator,subtitles
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # SRTranslator
 
 ## Install
 
 [PyPI](https://pypi.org/project/srtranslator/)
 
 ```bash
@@ -94,9 +80,7 @@
   -s, --show-browser    Show browser window
   -w WRAP_LIMIT, --wrap-limit WRAP_LIMIT
                         Number of characters -including spaces- to wrap a line of text. Default: 50
   -t {deepl-scrap,translatepy,deepl-api}, --translator {deepl-scrap,translatepy,deepl-api}
                         Built-in translator to use
   --auth AUTH           Api key if needed on translator
 ```
-
-
```

### Comparing `srtranslator-0.2.8/README.md` & `srtranslator-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: srtranslator
+Version: 0.2.9
+Summary: Traslate a .SRT file using any custom translator
+Home-page: https://github.com/sinedie/SRTranslator
+Author: EAR
+Author-email: sinedie@protonmail.com
+License: FREE
+Keywords: python,srt,languages,translator,subtitles
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # SRTranslator
 
 ## Install
 
 [PyPI](https://pypi.org/project/srtranslator/)
 
 ```bash
@@ -80,7 +94,9 @@
   -s, --show-browser    Show browser window
   -w WRAP_LIMIT, --wrap-limit WRAP_LIMIT
                         Number of characters -including spaces- to wrap a line of text. Default: 50
   -t {deepl-scrap,translatepy,deepl-api}, --translator {deepl-scrap,translatepy,deepl-api}
                         Built-in translator to use
   --auth AUTH           Api key if needed on translator
 ```
+
+
```

### Comparing `srtranslator-0.2.8/setup.py` & `srtranslator-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name="srtranslator",
     description="Traslate a .SRT file using any custom translator",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/sinedie/SRTranslator",
-    version="0.2.8",
+    version="0.2.9",
     author="EAR",
     author_email="sinedie@protonmail.com",
     license="FREE",
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages(),
     keywords=["python", "srt", "languages", "translator", "subtitles"],
```

### Comparing `srtranslator-0.2.8/srtranslator/__main__.py` & `srtranslator-0.2.9/srtranslator/__main__.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.8/srtranslator/srt_file.py` & `srtranslator-0.2.9/srtranslator/srt_file.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.8/srtranslator/translators/deepl_scrap.py` & `srtranslator-0.2.9/srtranslator/translators/deepl_scrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Button,
     Text,
 )
 
 
 class DeeplTranslator(Translator):
     url = "https://www.deepl.com/translator"
-    max_char = 3000
+    max_char = 1500
     languages = {
         "auto": "Any language (detect)",
         "bg": "Bulgarian",
         "zh": "Chinese",
         "cs": "Czech",
         "da": "Danish",
         "nl": "Dutch",
```

### Comparing `srtranslator-0.2.8/srtranslator/translators/deeplx.py` & `srtranslator-0.2.9/srtranslator/translators/deeplx.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.8/srtranslator/translators/selenium_utils.py` & `srtranslator-0.2.9/srtranslator/translators/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.8/srtranslator/translators/translatepy.py` & `srtranslator-0.2.9/srtranslator/translators/translatepy.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.8/srtranslator.egg-info/PKG-INFO` & `srtranslator-0.2.9/srtranslator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtranslator
-Version: 0.2.8
+Version: 0.2.9
 Summary: Traslate a .SRT file using any custom translator
 Home-page: https://github.com/sinedie/SRTranslator
 Author: EAR
 Author-email: sinedie@protonmail.com
 License: FREE
 Keywords: python,srt,languages,translator,subtitles
 Platform: UNKNOWN
```

### Comparing `srtranslator-0.2.8/srtranslator.egg-info/SOURCES.txt` & `srtranslator-0.2.9/srtranslator.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 srtranslator.egg-info/dependency_links.txt
 srtranslator.egg-info/requires.txt
 srtranslator.egg-info/top_level.txt
 srtranslator/translators/__init__.py
 srtranslator/translators/base.py
 srtranslator/translators/deepl_api.py
 srtranslator/translators/deepl_scrap.py
+srtranslator/translators/deeplcli.py
 srtranslator/translators/deeplx.py
 srtranslator/translators/selenium_utils.py
 srtranslator/translators/translatepy.py
```

### Comparing `srtranslator-0.2.8/srtranslator.egg-info/requires.txt` & `srtranslator-0.2.9/srtranslator.egg-info/requires.txt`

 * *Files identical despite different names*


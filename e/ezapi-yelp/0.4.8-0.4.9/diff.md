# Comparing `tmp/ezapi-yelp-0.4.8.tar.gz` & `tmp/ezapi-yelp-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezapi-yelp-0.4.8.tar", last modified: Thu Mar  9 09:27:00 2023, max compression
+gzip compressed data, was "ezapi-yelp-0.4.9.tar", last modified: Thu Jul 13 04:25:57 2023, max compression
```

## Comparing `ezapi-yelp-0.4.8.tar` & `ezapi-yelp-0.4.9.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.876539 ezapi-yelp-0.4.8/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.869400 ezapi-yelp-0.4.8/.github/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.872002 ezapi-yelp-0.4.8/.github/workflows/
--rw-r--r--   0 zehengl    (501) staff       (20)      245 2022-09-02 16:04:11.000000 ezapi-yelp-0.4.8/.github/workflows/pcu.yml
--rw-r--r--   0 zehengl    (501) staff       (20)      685 2023-03-09 09:13:57.000000 ezapi-yelp-0.4.8/.github/workflows/pytest.yml
--rw-r--r--   0 zehengl    (501) staff       (20)       70 2022-04-28 05:51:53.000000 ezapi-yelp-0.4.8/.gitignore
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.872589 ezapi-yelp-0.4.8/.vscode/
--rw-r--r--   0 zehengl    (501) staff       (20)      469 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.8/.vscode/extensions.json
--rw-r--r--   0 zehengl    (501) staff       (20)      584 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.8/.vscode/settings.json
--rw-r--r--   0 zehengl    (501) staff       (20)     1066 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.8/LICENSE
--rw-r--r--   0 zehengl    (501) staff       (20)     3295 2023-03-09 09:27:00.876357 ezapi-yelp-0.4.8/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)     2728 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.8/README.md
--rw-r--r--   0 zehengl    (501) staff       (20)      974 2023-03-09 09:19:35.000000 ezapi-yelp-0.4.8/pyproject.toml
--rw-r--r--   0 zehengl    (501) staff       (20)      127 2023-03-09 08:52:48.000000 ezapi-yelp-0.4.8/requirements-dev.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       28 2023-03-09 08:52:09.000000 ezapi-yelp-0.4.8/requirements-test.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-03-09 08:50:50.000000 ezapi-yelp-0.4.8/requirements.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-03-09 09:27:00.876582 ezapi-yelp-0.4.8/setup.cfg
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.869662 ezapi-yelp-0.4.8/src/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.873718 ezapi-yelp-0.4.8/src/ezapi_yelp.egg-info/
--rw-r--r--   0 zehengl    (501) staff       (20)     3295 2023-03-09 09:27:00.000000 ezapi-yelp-0.4.8/src/ezapi_yelp.egg-info/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)      592 2023-03-09 09:27:00.000000 ezapi-yelp-0.4.8/src/ezapi_yelp.egg-info/SOURCES.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-03-09 09:27:00.000000 ezapi-yelp-0.4.8/src/ezapi_yelp.egg-info/dependency_links.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-03-09 09:27:00.000000 ezapi-yelp-0.4.8/src/ezapi_yelp.egg-info/requires.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        5 2023-03-09 09:27:00.000000 ezapi-yelp-0.4.8/src/ezapi_yelp.egg-info/top_level.txt
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.874191 ezapi-yelp-0.4.8/src/yelp/
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.8/src/yelp/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)     6298 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.8/src/yelp/fusion.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.875596 ezapi-yelp-0.4.8/tests/
--rw-r--r--   0 zehengl    (501) staff       (20)      318 2023-03-09 09:18:09.000000 ezapi-yelp-0.4.8/tests/conftest.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-09 09:27:00.876019 ezapi-yelp-0.4.8/tests/helpers/
--rw-r--r--   0 zehengl    (501) staff       (20)      454 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.8/tests/helpers/data.py
--rw-r--r--   0 zehengl    (501) staff       (20)      170 2023-03-09 09:01:13.000000 ezapi-yelp-0.4.8/tests/helpers/utils.py
--rw-r--r--   0 zehengl    (501) staff       (20)     3990 2023-03-09 09:25:07.000000 ezapi-yelp-0.4.8/tests/test_business_endpoints.py
--rw-r--r--   0 zehengl    (501) staff       (20)      653 2023-03-09 09:25:17.000000 ezapi-yelp-0.4.8/tests/test_category_endpoints.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1147 2023-03-09 09:25:25.000000 ezapi-yelp-0.4.8/tests/test_event_endpoints.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.865167 ezapi-yelp-0.4.9/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.857834 ezapi-yelp-0.4.9/.github/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.861148 ezapi-yelp-0.4.9/.github/workflows/
+-rw-r--r--   0 zehengl    (501) staff       (20)      308 2023-04-29 06:48:02.000000 ezapi-yelp-0.4.9/.github/workflows/gh-deploy.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      243 2023-03-10 06:35:08.000000 ezapi-yelp-0.4.9/.github/workflows/pcu.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      760 2023-04-29 06:48:02.000000 ezapi-yelp-0.4.9/.github/workflows/pytest.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)       70 2022-04-28 05:51:53.000000 ezapi-yelp-0.4.9/.gitignore
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.861702 ezapi-yelp-0.4.9/.vscode/
+-rw-r--r--   0 zehengl    (501) staff       (20)      469 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.9/.vscode/extensions.json
+-rw-r--r--   0 zehengl    (501) staff       (20)      584 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.9/.vscode/settings.json
+-rw-r--r--   0 zehengl    (501) staff       (20)     1066 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.9/LICENSE
+-rw-r--r--   0 zehengl    (501) staff       (20)     3043 2023-07-13 04:25:57.864997 ezapi-yelp-0.4.9/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     2476 2023-03-22 15:51:14.000000 ezapi-yelp-0.4.9/README.md
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.861956 ezapi-yelp-0.4.9/docs/
+-rw-r--r--   0 zehengl    (501) staff       (20)      278 2023-03-13 06:56:37.000000 ezapi-yelp-0.4.9/docs/index.md
+-rw-r--r--   0 zehengl    (501) staff       (20)     1345 2023-06-05 03:50:08.000000 ezapi-yelp-0.4.9/mkdocs.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      974 2023-03-09 09:19:35.000000 ezapi-yelp-0.4.9/pyproject.toml
+-rw-r--r--   0 zehengl    (501) staff       (20)      152 2023-06-05 03:49:44.000000 ezapi-yelp-0.4.9/requirements-dev.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)      115 2023-07-13 04:25:20.000000 ezapi-yelp-0.4.9/requirements-docs.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       28 2023-06-26 14:02:50.000000 ezapi-yelp-0.4.9/requirements-test.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-06-05 03:49:44.000000 ezapi-yelp-0.4.9/requirements.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-07-13 04:25:57.865207 ezapi-yelp-0.4.9/setup.cfg
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.858342 ezapi-yelp-0.4.9/src/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.862766 ezapi-yelp-0.4.9/src/ezapi_yelp.egg-info/
+-rw-r--r--   0 zehengl    (501) staff       (20)     3043 2023-07-13 04:25:57.000000 ezapi-yelp-0.4.9/src/ezapi_yelp.egg-info/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)      671 2023-07-13 04:25:57.000000 ezapi-yelp-0.4.9/src/ezapi_yelp.egg-info/SOURCES.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-07-13 04:25:57.000000 ezapi-yelp-0.4.9/src/ezapi_yelp.egg-info/dependency_links.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-07-13 04:25:57.000000 ezapi-yelp-0.4.9/src/ezapi_yelp.egg-info/requires.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        5 2023-07-13 04:25:57.000000 ezapi-yelp-0.4.9/src/ezapi_yelp.egg-info/top_level.txt
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.863197 ezapi-yelp-0.4.9/src/yelp/
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.9/src/yelp/__init__.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     6298 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.9/src/yelp/fusion.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.864233 ezapi-yelp-0.4.9/tests/
+-rw-r--r--   0 zehengl    (501) staff       (20)      323 2023-03-22 15:47:33.000000 ezapi-yelp-0.4.9/tests/conftest.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:25:57.864663 ezapi-yelp-0.4.9/tests/helpers/
+-rw-r--r--   0 zehengl    (501) staff       (20)      454 2022-04-13 05:50:48.000000 ezapi-yelp-0.4.9/tests/helpers/data.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      170 2023-03-09 09:01:13.000000 ezapi-yelp-0.4.9/tests/helpers/utils.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     3990 2023-03-09 09:25:07.000000 ezapi-yelp-0.4.9/tests/test_business_endpoints.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      653 2023-03-09 09:25:17.000000 ezapi-yelp-0.4.9/tests/test_category_endpoints.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1147 2023-03-09 09:25:25.000000 ezapi-yelp-0.4.9/tests/test_event_endpoints.py
```

### Comparing `ezapi-yelp-0.4.8/.github/workflows/pytest.yml` & `ezapi-yelp-0.4.9/.github/workflows/pytest.yml`

 * *Files 26% similar despite different names*

```diff
@@ -8,22 +8,23 @@
     - cron: "0 6 1 * *"
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 2
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
-      - name: Checkout
-        uses: actions/checkout@v2
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Checkout 🛎️
+        uses: actions/checkout@v3
+      - name: Set up Python ${{ matrix.python-version }} 🐍
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Test with pytest
+      - name: Test with pytest 🧪
         run: |
+          python -m pip install -U pip
           pip install -r requirements-test.txt
           pip install -e .
           pytest
         env:
-          token: ${{ secrets.TOKEN }}
+          yelp_token: ${{ secrets.YELP_TOKEN }}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ezapi-yelp-0.4.8/.vscode/settings.json` & `ezapi-yelp-0.4.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ezapi-yelp-0.4.8/LICENSE` & `ezapi-yelp-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ezapi-yelp-0.4.8/PKG-INFO` & `ezapi-yelp-0.4.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: ezapi-yelp
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Python wrapper for Yelp API
 Author-email: Zeheng Li <imzehengl@gmail.com>
 Maintainer-email: Zeheng Li <imzehengl@gmail.com>
 Project-URL: repository, https://github.com/zehengl/ezapi-yelp
 Project-URL: homepage, https://zehengl.github.io/ezapi-yelp/
 Keywords: Yelp Fusion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-    <img src="https://cdn3.iconfinder.com/data/icons/data-sharing-and-cloud-lineal-style/512/apiprogrammingdevolperinterfaceappcomputer-512.png" alt="logo" height="196">
     <img src="https://cdn2.iconfinder.com/data/icons/social-media-applications/64/social_media_applications_28-yelp-512.png" alt="yelp" height="96">
 </div>
 
 # ezapi-yelp
 
 [![pytest](https://github.com/zehengl/ezapi-yelp/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-yelp/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
@@ -72,24 +71,26 @@
 print(yelp_fusion.event_lookup("oakland-saucy-oakland-restaurant-pop-up"))
 print(yelp_fusion.event_search(location="Oakland"))
 print(yelp_fusion.featured_event(location="Oakland"))
 ```
 
 ## Test
 
-    git clone git@github.com:zehengl/ezapi-yelp.git
-    export token="..."
-    cd ezapi-yelp
-    python setup.py test
+```bash
+git clone git@github.com:zehengl/ezapi-yelp.git
+cd ezapi-yelp
+export yelp_token="..."
+python -m venv .venv
+source .venv/bin/activate
+pip install -e .
+pip install -r requirements-test.txt
+pytest
+```
 
-Use `$Env:token="..."` to set the api key environment variable on Windows.
+Use `$Env:yelp_token="..."` to set the api key environment variable on Windows.
 
 ## Credits
 
-- [Icon][1] by [Photolio][2]
-
-- [Icon][3] by [tulpahn][4]
+- [Icon][1] by [tulpahn][2]
 
-[1]: https://www.iconfinder.com/icons/4904814/api_app_computer_devolper_interface_programming_icon
-[2]: https://www.iconfinder.com/Muhammad_Auns
-[3]: https://www.iconfinder.com/icons/4102600/applications_media_social_yelp_icon
-[4]: https://www.iconfinder.com/tulpahn
+[1]: https://www.iconfinder.com/icons/4102600/applications_media_social_yelp_icon
+[2]: https://www.iconfinder.com/tulpahn
```

### Comparing `ezapi-yelp-0.4.8/README.md` & `ezapi-yelp-0.4.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 <div align="center">
-    <img src="https://cdn3.iconfinder.com/data/icons/data-sharing-and-cloud-lineal-style/512/apiprogrammingdevolperinterfaceappcomputer-512.png" alt="logo" height="196">
     <img src="https://cdn2.iconfinder.com/data/icons/social-media-applications/64/social_media_applications_28-yelp-512.png" alt="yelp" height="96">
 </div>
 
 # ezapi-yelp
 
 [![pytest](https://github.com/zehengl/ezapi-yelp/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-yelp/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
@@ -56,24 +55,26 @@
 print(yelp_fusion.event_lookup("oakland-saucy-oakland-restaurant-pop-up"))
 print(yelp_fusion.event_search(location="Oakland"))
 print(yelp_fusion.featured_event(location="Oakland"))
 ```
 
 ## Test
 
-    git clone git@github.com:zehengl/ezapi-yelp.git
-    export token="..."
-    cd ezapi-yelp
-    python setup.py test
+```bash
+git clone git@github.com:zehengl/ezapi-yelp.git
+cd ezapi-yelp
+export yelp_token="..."
+python -m venv .venv
+source .venv/bin/activate
+pip install -e .
+pip install -r requirements-test.txt
+pytest
+```
 
-Use `$Env:token="..."` to set the api key environment variable on Windows.
+Use `$Env:yelp_token="..."` to set the api key environment variable on Windows.
 
 ## Credits
 
-- [Icon][1] by [Photolio][2]
-
-- [Icon][3] by [tulpahn][4]
+- [Icon][1] by [tulpahn][2]
 
-[1]: https://www.iconfinder.com/icons/4904814/api_app_computer_devolper_interface_programming_icon
-[2]: https://www.iconfinder.com/Muhammad_Auns
-[3]: https://www.iconfinder.com/icons/4102600/applications_media_social_yelp_icon
-[4]: https://www.iconfinder.com/tulpahn
+[1]: https://www.iconfinder.com/icons/4102600/applications_media_social_yelp_icon
+[2]: https://www.iconfinder.com/tulpahn
```

### Comparing `ezapi-yelp-0.4.8/pyproject.toml` & `ezapi-yelp-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezapi-yelp-0.4.8/src/ezapi_yelp.egg-info/PKG-INFO` & `ezapi-yelp-0.4.9/src/ezapi_yelp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: ezapi-yelp
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Python wrapper for Yelp API
 Author-email: Zeheng Li <imzehengl@gmail.com>
 Maintainer-email: Zeheng Li <imzehengl@gmail.com>
 Project-URL: repository, https://github.com/zehengl/ezapi-yelp
 Project-URL: homepage, https://zehengl.github.io/ezapi-yelp/
 Keywords: Yelp Fusion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-    <img src="https://cdn3.iconfinder.com/data/icons/data-sharing-and-cloud-lineal-style/512/apiprogrammingdevolperinterfaceappcomputer-512.png" alt="logo" height="196">
     <img src="https://cdn2.iconfinder.com/data/icons/social-media-applications/64/social_media_applications_28-yelp-512.png" alt="yelp" height="96">
 </div>
 
 # ezapi-yelp
 
 [![pytest](https://github.com/zehengl/ezapi-yelp/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-yelp/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
@@ -72,24 +71,26 @@
 print(yelp_fusion.event_lookup("oakland-saucy-oakland-restaurant-pop-up"))
 print(yelp_fusion.event_search(location="Oakland"))
 print(yelp_fusion.featured_event(location="Oakland"))
 ```
 
 ## Test
 
-    git clone git@github.com:zehengl/ezapi-yelp.git
-    export token="..."
-    cd ezapi-yelp
-    python setup.py test
+```bash
+git clone git@github.com:zehengl/ezapi-yelp.git
+cd ezapi-yelp
+export yelp_token="..."
+python -m venv .venv
+source .venv/bin/activate
+pip install -e .
+pip install -r requirements-test.txt
+pytest
+```
 
-Use `$Env:token="..."` to set the api key environment variable on Windows.
+Use `$Env:yelp_token="..."` to set the api key environment variable on Windows.
 
 ## Credits
 
-- [Icon][1] by [Photolio][2]
-
-- [Icon][3] by [tulpahn][4]
+- [Icon][1] by [tulpahn][2]
 
-[1]: https://www.iconfinder.com/icons/4904814/api_app_computer_devolper_interface_programming_icon
-[2]: https://www.iconfinder.com/Muhammad_Auns
-[3]: https://www.iconfinder.com/icons/4102600/applications_media_social_yelp_icon
-[4]: https://www.iconfinder.com/tulpahn
+[1]: https://www.iconfinder.com/icons/4102600/applications_media_social_yelp_icon
+[2]: https://www.iconfinder.com/tulpahn
```

### Comparing `ezapi-yelp-0.4.8/src/yelp/fusion.py` & `ezapi-yelp-0.4.9/src/yelp/fusion.py`

 * *Files identical despite different names*

### Comparing `ezapi-yelp-0.4.8/tests/test_business_endpoints.py` & `ezapi-yelp-0.4.9/tests/test_business_endpoints.py`

 * *Files identical despite different names*

### Comparing `ezapi-yelp-0.4.8/tests/test_category_endpoints.py` & `ezapi-yelp-0.4.9/tests/test_category_endpoints.py`

 * *Files identical despite different names*

### Comparing `ezapi-yelp-0.4.8/tests/test_event_endpoints.py` & `ezapi-yelp-0.4.9/tests/test_event_endpoints.py`

 * *Files identical despite different names*


# Comparing `tmp/ezapi-icc-pro-0.1.0.tar.gz` & `tmp/ezapi-icc-pro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezapi-icc-pro-0.1.0.tar", last modified: Wed Mar  1 02:49:48 2023, max compression
+gzip compressed data, was "ezapi-icc-pro-0.1.1.tar", last modified: Thu Jul 13 04:23:40 2023, max compression
```

## Comparing `ezapi-icc-pro-0.1.0.tar` & `ezapi-icc-pro-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,60 @@
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.832273 ezapi-icc-pro-0.1.0/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.824960 ezapi-icc-pro-0.1.0/.github/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.826843 ezapi-icc-pro-0.1.0/.github/workflows/
--rw-r--r--   0 zehengl    (501) staff       (20)      904 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 zehengl    (501) staff       (20)       53 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/.gitignore
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.827273 ezapi-icc-pro-0.1.0/.vscode/
--rw-r--r--   0 zehengl    (501) staff       (20)      469 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/.vscode/extensions.json
--rw-r--r--   0 zehengl    (501) staff       (20)      667 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/.vscode/settings.json
--rw-r--r--   0 zehengl    (501) staff       (20)     1383 2023-03-01 02:49:48.832072 ezapi-icc-pro-0.1.0/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)      822 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/README.md
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.827403 ezapi-icc-pro-0.1.0/docs/
--rw-r--r--   0 zehengl    (501) staff       (20)      171 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/docs/index.md
--rw-r--r--   0 zehengl    (501) staff       (20)     1102 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/mkdocs.yml
--rw-r--r--   0 zehengl    (501) staff       (20)      990 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/pyproject.toml
--rw-r--r--   0 zehengl    (501) staff       (20)      152 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/requirements-dev.txt
--rw-r--r--   0 zehengl    (501) staff       (20)      115 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/requirements-docs.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       48 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/requirements-test.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/requirements.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-03-01 02:49:48.832324 ezapi-icc-pro-0.1.0/setup.cfg
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.825301 ezapi-icc-pro-0.1.0/src/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.828170 ezapi-icc-pro-0.1.0/src/ezapi_icc_pro.egg-info/
--rw-r--r--   0 zehengl    (501) staff       (20)     1383 2023-03-01 02:49:48.000000 ezapi-icc-pro-0.1.0/src/ezapi_icc_pro.egg-info/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)      916 2023-03-01 02:49:48.000000 ezapi-icc-pro-0.1.0/src/ezapi_icc_pro.egg-info/SOURCES.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-03-01 02:49:48.000000 ezapi-icc-pro-0.1.0/src/ezapi_icc_pro.egg-info/dependency_links.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-03-01 02:49:48.000000 ezapi-icc-pro-0.1.0/src/ezapi_icc_pro.egg-info/requires.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        8 2023-03-01 02:49:48.000000 ezapi-icc-pro-0.1.0/src/ezapi_icc_pro.egg-info/top_level.txt
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.829820 ezapi-icc-pro-0.1.0/src/icc_pro/
--rw-r--r--   0 zehengl    (501) staff       (20)     1484 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)      867 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/accumulations.py
--rw-r--r--   0 zehengl    (501) staff       (20)      964 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/analog_inputs.py
--rw-r--r--   0 zehengl    (501) staff       (20)      862 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/core.py
--rw-r--r--   0 zehengl    (501) staff       (20)      278 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/meters.py
--rw-r--r--   0 zehengl    (501) staff       (20)      850 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/programs.py
--rw-r--r--   0 zehengl    (501) staff       (20)      921 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/sensors.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1012 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/token.py
--rw-r--r--   0 zehengl    (501) staff       (20)      930 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/valves.py
--rw-r--r--   0 zehengl    (501) staff       (20)      307 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/src/icc_pro/virtual_meters.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-01 02:49:48.831740 ezapi-icc-pro-0.1.0/tests/
--rw-r--r--   0 zehengl    (501) staff       (20)        0 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)      501 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/conftest.py
--rw-r--r--   0 zehengl    (501) staff       (20)      320 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_accumulations.py
--rw-r--r--   0 zehengl    (501) staff       (20)      722 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_analog_inputs.py
--rw-r--r--   0 zehengl    (501) staff       (20)      730 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_icc_pro.py
--rw-r--r--   0 zehengl    (501) staff       (20)      422 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_meters.py
--rw-r--r--   0 zehengl    (501) staff       (20)      432 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_programs.py
--rw-r--r--   0 zehengl    (501) staff       (20)      669 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_sensors.py
--rw-r--r--   0 zehengl    (501) staff       (20)      134 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_tokens.py
--rw-r--r--   0 zehengl    (501) staff       (20)      578 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_valves.py
--rw-r--r--   0 zehengl    (501) staff       (20)      461 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.0/tests/test_virtual_meters.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.705114 ezapi-icc-pro-0.1.1/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.696106 ezapi-icc-pro-0.1.1/.github/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.699049 ezapi-icc-pro-0.1.1/.github/workflows/
+-rw-r--r--   0 zehengl    (501) staff       (20)      308 2023-04-29 07:10:03.000000 ezapi-icc-pro-0.1.1/.github/workflows/gh-deploy.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      243 2023-03-03 16:39:48.000000 ezapi-icc-pro-0.1.1/.github/workflows/pcu.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      948 2023-04-29 07:10:44.000000 ezapi-icc-pro-0.1.1/.github/workflows/pytest.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)       53 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/.gitignore
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.699443 ezapi-icc-pro-0.1.1/.vscode/
+-rw-r--r--   0 zehengl    (501) staff       (20)      469 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/.vscode/extensions.json
+-rw-r--r--   0 zehengl    (501) staff       (20)      667 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/.vscode/settings.json
+-rw-r--r--   0 zehengl    (501) staff       (20)     1066 2023-03-10 06:29:10.000000 ezapi-icc-pro-0.1.1/LICENSE
+-rw-r--r--   0 zehengl    (501) staff       (20)     1883 2023-07-13 04:23:40.704930 ezapi-icc-pro-0.1.1/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     1300 2023-03-27 22:02:29.000000 ezapi-icc-pro-0.1.1/README.md
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.699567 ezapi-icc-pro-0.1.1/docs/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.701289 ezapi-icc-pro-0.1.1/docs/endpoints/
+-rw-r--r--   0 zehengl    (501) staff       (20)     1007 2023-03-23 02:52:47.000000 ezapi-icc-pro-0.1.1/docs/endpoints/analog_inputs.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      205 2023-03-03 16:39:48.000000 ezapi-icc-pro-0.1.1/docs/endpoints/index.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      278 2023-03-23 02:52:47.000000 ezapi-icc-pro-0.1.1/docs/endpoints/meters.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      391 2023-03-23 02:52:47.000000 ezapi-icc-pro-0.1.1/docs/endpoints/programs.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      971 2023-03-23 02:52:47.000000 ezapi-icc-pro-0.1.1/docs/endpoints/sensors.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      454 2023-03-23 02:52:47.000000 ezapi-icc-pro-0.1.1/docs/endpoints/valves.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      294 2023-03-23 02:52:47.000000 ezapi-icc-pro-0.1.1/docs/endpoints/virtual_meters.md
+-rw-r--r--   0 zehengl    (501) staff       (20)      528 2023-03-23 02:52:47.000000 ezapi-icc-pro-0.1.1/docs/index.md
+-rw-r--r--   0 zehengl    (501) staff       (20)     1669 2023-04-15 03:33:19.000000 ezapi-icc-pro-0.1.1/mkdocs.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      296 2023-03-27 22:02:29.000000 ezapi-icc-pro-0.1.1/pcufile.toml
+-rw-r--r--   0 zehengl    (501) staff       (20)      990 2023-05-09 07:04:55.000000 ezapi-icc-pro-0.1.1/pyproject.toml
+-rw-r--r--   0 zehengl    (501) staff       (20)      152 2023-07-13 04:22:43.000000 ezapi-icc-pro-0.1.1/requirements-dev.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)      143 2023-07-13 04:22:19.000000 ezapi-icc-pro-0.1.1/requirements-docs.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       48 2023-07-13 04:22:19.000000 ezapi-icc-pro-0.1.1/requirements-test.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-05-24 18:31:12.000000 ezapi-icc-pro-0.1.1/requirements.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-07-13 04:23:40.705156 ezapi-icc-pro-0.1.1/setup.cfg
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.696686 ezapi-icc-pro-0.1.1/src/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.702016 ezapi-icc-pro-0.1.1/src/ezapi_icc_pro.egg-info/
+-rw-r--r--   0 zehengl    (501) staff       (20)     1883 2023-07-13 04:23:40.000000 ezapi-icc-pro-0.1.1/src/ezapi_icc_pro.egg-info/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     1169 2023-07-13 04:23:40.000000 ezapi-icc-pro-0.1.1/src/ezapi_icc_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-07-13 04:23:40.000000 ezapi-icc-pro-0.1.1/src/ezapi_icc_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-07-13 04:23:40.000000 ezapi-icc-pro-0.1.1/src/ezapi_icc_pro.egg-info/requires.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        8 2023-07-13 04:23:40.000000 ezapi-icc-pro-0.1.1/src/ezapi_icc_pro.egg-info/top_level.txt
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.703188 ezapi-icc-pro-0.1.1/src/icc_pro/
+-rw-r--r--   0 zehengl    (501) staff       (20)     1484 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/__init__.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      867 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/accumulations.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      964 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/analog_inputs.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      862 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/core.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      278 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/meters.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      955 2023-03-03 16:39:48.000000 ezapi-icc-pro-0.1.1/src/icc_pro/programs.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      921 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/sensors.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1012 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/token.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      972 2023-03-03 16:39:48.000000 ezapi-icc-pro-0.1.1/src/icc_pro/valves.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      307 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/src/icc_pro/virtual_meters.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:23:40.704665 ezapi-icc-pro-0.1.1/tests/
+-rw-r--r--   0 zehengl    (501) staff       (20)      501 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/conftest.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      320 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/test_accumulations.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      722 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/test_analog_inputs.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      730 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/test_icc_pro.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      422 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/test_meters.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1206 2023-03-03 16:39:48.000000 ezapi-icc-pro-0.1.1/tests/test_programs.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      669 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/test_sensors.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      134 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/test_tokens.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      861 2023-03-03 16:39:48.000000 ezapi-icc-pro-0.1.1/tests/test_valves.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      461 2023-03-01 02:46:33.000000 ezapi-icc-pro-0.1.1/tests/test_virtual_meters.py
```

### Comparing `ezapi-icc-pro-0.1.0/.github/workflows/pytest.yml` & `ezapi-icc-pro-0.1.1/.github/workflows/pytest.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,22 @@
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: Checkout 🛎️
-        uses: actions/checkout@v2
-      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/checkout@v3
+      - name: Set up Python ${{ matrix.python-version }} 🐍
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Test with pytest 🧪
         run: |
+          python -m pip install -U pip
           pip install -r requirements-test.txt
           pip install -e .
           pytest
         env:
           iccpro_host: ${{ secrets.ICCPRO_HOST }}
           iccpro_username: ${{ secrets.ICCPRO_USERNAME }}
           iccpro_password: ${{ secrets.ICCPRO_PASSWORD }}
```

### Comparing `ezapi-icc-pro-0.1.0/.vscode/settings.json` & `ezapi-icc-pro-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/PKG-INFO` & `ezapi-icc-pro-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 Metadata-Version: 2.1
 Name: ezapi-icc-pro
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for ICC PRO RESTful API
 Author-email: Zeheng Li <imzehengl@gmail.com>
 Maintainer-email: Zeheng Li <imzehengl@gmail.com>
 Project-URL: repository, https://github.com/zehengl/ezapi-icc-pro
 Project-URL: homepage, https://zehengl.github.io/ezapi-icc-pro/
 Keywords: ICC PRO
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
-    <img src="https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png" alt="logo" height="196">
+    <img src="https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png" alt="logo" height="128">
 </div>
 
 # ezapi-icc-pro
 
 [![pytest](https://github.com/zehengl/ezapi-icc-pro/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-icc-pro/actions/workflows/pytest.yml)
 ![coding_style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![PyPI - License](https://img.shields.io/pypi/l/ezapi-icc-pro)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ezapi-icc-pro)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/ezapi-icc-pro)
+[![Downloads](https://pepy.tech/badge/ezapi-icc-pro)](https://pepy.tech/project/ezapi-icc-pro)
 
 A Python wrapper for ICC PRO RESTful API
 
 ## Install
 
+From [PyPi](https://pypi.org/project/ezapi-icc-pro/)
+
+    pip install ezapi-icc-pro
+
 From [GitHub](https://github.com/zehengl/ezapi-icc-pro)
 
     pip install git+https://github.com/zehengl/ezapi-icc-pro.git
 
+## Usage
+
+Check out these [examples](https://zehengl.github.io/ezapi-icc-pro/endpoints/).
+
 ## Credits
 
 - [Logo][1] by [Chanut is Industries][2]
 
 [1]: https://www.iconfinder.com/icons/4629153/agricultural_agriculture_agritect_farming_irrigation_smart_farm_water_icon
 [2]: https://www.iconfinder.com/Chanut-is
```

### Comparing `ezapi-icc-pro-0.1.0/README.md` & `ezapi-icc-pro-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 <div align="center">
-    <img src="https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png" alt="logo" height="196">
+    <img src="https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png" alt="logo" height="128">
 </div>
 
 # ezapi-icc-pro
 
 [![pytest](https://github.com/zehengl/ezapi-icc-pro/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-icc-pro/actions/workflows/pytest.yml)
 ![coding_style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![PyPI - License](https://img.shields.io/pypi/l/ezapi-icc-pro)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ezapi-icc-pro)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/ezapi-icc-pro)
+[![Downloads](https://pepy.tech/badge/ezapi-icc-pro)](https://pepy.tech/project/ezapi-icc-pro)
 
 A Python wrapper for ICC PRO RESTful API
 
 ## Install
 
+From [PyPi](https://pypi.org/project/ezapi-icc-pro/)
+
+    pip install ezapi-icc-pro
+
 From [GitHub](https://github.com/zehengl/ezapi-icc-pro)
 
     pip install git+https://github.com/zehengl/ezapi-icc-pro.git
 
+## Usage
+
+Check out these [examples](https://zehengl.github.io/ezapi-icc-pro/endpoints/).
+
 ## Credits
 
 - [Logo][1] by [Chanut is Industries][2]
 
 [1]: https://www.iconfinder.com/icons/4629153/agricultural_agriculture_agritect_farming_irrigation_smart_farm_water_icon
 [2]: https://www.iconfinder.com/Chanut-is
```

### Comparing `ezapi-icc-pro-0.1.0/mkdocs.yml` & `ezapi-icc-pro-0.1.1/mkdocs.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 site_name: ezapi-icc-pro
 nav:
   - Home: index.md
+  - Endpoints:
+      - endpoints/index.md
+      - Valves: endpoints/valves.md
+      - Meters: endpoints/meters.md
+      - Virtual Meters: endpoints/virtual_meters.md
+      - Programs: endpoints/programs.md
+      - Analog Inputs: endpoints/analog_inputs.md
+      - Sensors: endpoints/sensors.md
 theme:
   name: material
   favicon: https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png
   logo: https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png
   font:
     text: Roboto
   palette:
@@ -18,25 +26,36 @@
       primary: indigo
       accent: indigo
       toggle:
         icon: material/toggle-switch-off-outline
         name: Switch to light mode
   features:
     - header.autohide
-repo_name: zehengl/ezapi-icc-pro
+    - content.code.copy
+    - navigation.top
+repo_name: ezapi-icc-pro
 repo_url: https://github.com/zehengl/ezapi-icc-pro
 plugins:
   - search
   - tags
   - minify:
       minify_html: true
   - git-revision-date-localized:
-      type: date
+      type: timeago
+      enable_creation_date: true
+  - section-index
 extra:
   social:
     - icon: fontawesome/brands/github
       link: https://github.com/zehengl
     - icon: fontawesome/brands/linkedin
       link: https://linkedin.com/in/zehengl
 markdown_extensions:
   - attr_list
   - md_in_html
+  - pymdownx.highlight:
+      anchor_linenums: true
+      line_spans: __span
+      pygments_lang_class: true
+  - pymdownx.inlinehilite
+  - pymdownx.snippets
+  - pymdownx.superfences
```

### Comparing `ezapi-icc-pro-0.1.0/pyproject.toml` & `ezapi-icc-pro-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/src/ezapi_icc_pro.egg-info/PKG-INFO` & `ezapi-icc-pro-0.1.1/src/ezapi_icc_pro.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 Metadata-Version: 2.1
 Name: ezapi-icc-pro
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for ICC PRO RESTful API
 Author-email: Zeheng Li <imzehengl@gmail.com>
 Maintainer-email: Zeheng Li <imzehengl@gmail.com>
 Project-URL: repository, https://github.com/zehengl/ezapi-icc-pro
 Project-URL: homepage, https://zehengl.github.io/ezapi-icc-pro/
 Keywords: ICC PRO
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
-    <img src="https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png" alt="logo" height="196">
+    <img src="https://cdn0.iconfinder.com/data/icons/smart-farm-line-agriculture-technology/512/Irrigation-512.png" alt="logo" height="128">
 </div>
 
 # ezapi-icc-pro
 
 [![pytest](https://github.com/zehengl/ezapi-icc-pro/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-icc-pro/actions/workflows/pytest.yml)
 ![coding_style](https://img.shields.io/badge/code%20style-black-000000.svg)
+![PyPI - License](https://img.shields.io/pypi/l/ezapi-icc-pro)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ezapi-icc-pro)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/ezapi-icc-pro)
+[![Downloads](https://pepy.tech/badge/ezapi-icc-pro)](https://pepy.tech/project/ezapi-icc-pro)
 
 A Python wrapper for ICC PRO RESTful API
 
 ## Install
 
+From [PyPi](https://pypi.org/project/ezapi-icc-pro/)
+
+    pip install ezapi-icc-pro
+
 From [GitHub](https://github.com/zehengl/ezapi-icc-pro)
 
     pip install git+https://github.com/zehengl/ezapi-icc-pro.git
 
+## Usage
+
+Check out these [examples](https://zehengl.github.io/ezapi-icc-pro/endpoints/).
+
 ## Credits
 
 - [Logo][1] by [Chanut is Industries][2]
 
 [1]: https://www.iconfinder.com/icons/4629153/agricultural_agriculture_agritect_farming_irrigation_smart_farm_water_icon
 [2]: https://www.iconfinder.com/Chanut-is
```

### Comparing `ezapi-icc-pro-0.1.0/src/icc_pro/__init__.py` & `ezapi-icc-pro-0.1.1/src/icc_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/src/icc_pro/accumulations.py` & `ezapi-icc-pro-0.1.1/src/icc_pro/accumulations.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/src/icc_pro/analog_inputs.py` & `ezapi-icc-pro-0.1.1/src/icc_pro/analog_inputs.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/src/icc_pro/core.py` & `ezapi-icc-pro-0.1.1/src/icc_pro/core.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/src/icc_pro/sensors.py` & `ezapi-icc-pro-0.1.1/src/icc_pro/sensors.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/src/icc_pro/token.py` & `ezapi-icc-pro-0.1.1/src/icc_pro/token.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/src/icc_pro/valves.py` & `ezapi-icc-pro-0.1.1/src/icc_pro/valves.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     def get_valves_status(self, **kwargs):
         url = urljoin(self.host, f"{ValvesMixin.url}/getgisstatus")
         req = PreparedRequest()
         req.prepare_url(url, kwargs)
         return self.make_request("GET", req.url)
 
     def create_valves_snapshot(self):
-        pass
+        raise NotImplementedError
 
     def update_valves_snapshot(self):
-        pass
+        raise NotImplementedError
```

### Comparing `ezapi-icc-pro-0.1.0/tests/test_analog_inputs.py` & `ezapi-icc-pro-0.1.1/tests/test_analog_inputs.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/tests/test_icc_pro.py` & `ezapi-icc-pro-0.1.1/tests/test_icc_pro.py`

 * *Files identical despite different names*

### Comparing `ezapi-icc-pro-0.1.0/tests/test_sensors.py` & `ezapi-icc-pro-0.1.1/tests/test_sensors.py`

 * *Files identical despite different names*


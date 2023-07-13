# Comparing `tmp/geovisio_cli-0.2.2.tar.gz` & `tmp/geovisio_cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geovisio_cli-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geovisio_cli-0.2.2.tar` & `geovisio_cli-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.2.2/.gitignore
--rw-r--r--   0        0        0     1413 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/.gitlab-ci.yml
--rw-r--r--   0        0        0     3789 2023-06-26 07:08:10.068178 geovisio_cli-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.2.2/LICENSE
--rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/Makefile
--rw-r--r--   0        0        0     7516 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/README.md
--rw-r--r--   0        0        0     3250 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/USAGE.md
--rw-r--r--   0        0        0       53 2023-06-26 07:08:10.068178 geovisio_cli-0.2.2/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.2.2/geovisio_cli/exception.py
--rw-r--r--   0        0        0     6180 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/geovisio_cli/main.py
--rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/geovisio_cli/model.py
--rw-r--r--   0        0        0    21407 2023-06-20 08:50:48.042695 geovisio_cli-0.2.2/geovisio_cli/sequence.py
--rw-r--r--   0        0        0     2107 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/geovisio_cli/utils.py
--rw-r--r--   0        0        0     1221 2023-06-26 07:08:10.068178 geovisio_cli-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      234 2023-06-19 17:19:08.702865 geovisio_cli-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.2.2/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.2.2/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.2.2/tests/integration/docker-compose-gitlab-override.yml
--rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.2.2/tests/integration/keycloak-realm.json
--rw-r--r--   0        0        0     3210 2023-06-22 08:20:49.394297 geovisio_cli-0.2.2/tests/integration/test_auth.py
--rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/tests/integration/test_status.py
--rw-r--r--   0        0        0     7087 2023-06-22 08:20:49.394297 geovisio_cli-0.2.2/tests/integration/test_upload.py
--rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.2.2/tests/test_process.py
--rw-r--r--   0        0        0    10801 2023-06-22 08:20:49.394297 geovisio_cli-0.2.2/tests/test_sequence.py
--rw-r--r--   0        0        0      682 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/tests/test_utils.py
--rw-r--r--   0        0        0     8685 1970-01-01 00:00:00.000000 geovisio_cli-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1413 2023-06-22 09:18:10.500879 geovisio_cli-0.2.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3984 2023-07-13 14:36:20.319561 geovisio_cli-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.2.3/LICENSE
+-rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.2.3/Makefile
+-rw-r--r--   0        0        0     7577 2023-07-13 14:32:37.766769 geovisio_cli-0.2.3/README.md
+-rw-r--r--   0        0        0     3259 2023-07-13 14:36:20.319561 geovisio_cli-0.2.3/USAGE.md
+-rw-r--r--   0        0        0       53 2023-07-13 14:36:20.319561 geovisio_cli-0.2.3/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.2.3/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.2.3/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     6180 2023-06-22 09:18:10.500879 geovisio_cli-0.2.3/geovisio_cli/main.py
+-rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.2.3/geovisio_cli/model.py
+-rw-r--r--   0        0        0    21407 2023-06-20 08:50:48.042695 geovisio_cli-0.2.3/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0     2107 2023-06-22 09:18:10.500879 geovisio_cli-0.2.3/geovisio_cli/utils.py
+-rw-r--r--   0        0        0     1246 2023-07-13 14:32:37.766769 geovisio_cli-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-19 17:19:08.702865 geovisio_cli-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.2.3/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.2.3/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.2.3/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.2.3/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.2.3/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.2.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.2.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.2.3/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.2.3/tests/integration/docker-compose-gitlab-override.yml
+-rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.2.3/tests/integration/keycloak-realm.json
+-rw-r--r--   0        0        0     3210 2023-06-22 08:20:49.394297 geovisio_cli-0.2.3/tests/integration/test_auth.py
+-rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.2.3/tests/integration/test_status.py
+-rw-r--r--   0        0        0     7087 2023-06-22 08:20:49.394297 geovisio_cli-0.2.3/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.2.3/tests/test_process.py
+-rw-r--r--   0        0        0    10979 2023-07-13 14:32:37.766769 geovisio_cli-0.2.3/tests/test_sequence.py
+-rw-r--r--   0        0        0      682 2023-06-22 09:18:10.500879 geovisio_cli-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0     8769 1970-01-01 00:00:00.000000 geovisio_cli-0.2.3/PKG-INFO
```

### Comparing `geovisio_cli-0.2.2/.gitlab-ci.yml` & `geovisio_cli-0.2.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/CHANGELOG.md` & `geovisio_cli-0.2.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.3] - 2023-07-13
+
+### Changed
+- Support of Python >= 3.8
+
 ## [0.2.2] - 2023-06-26
 
 ### Fixes
 - Add missing `packaging` dependency
 
 ## [0.2.1] - 2023-06-22
 
@@ -74,15 +79,17 @@
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.2.1...main
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.2.3...main
+[0.2.3]: https://gitlab.com/geovisio/cli/-/compare/0.2.2...0.2.3
+[0.2.2]: https://gitlab.com/geovisio/cli/-/compare/0.2.1...0.2.2
 [0.2.1]: https://gitlab.com/geovisio/cli/-/compare/0.2.0...0.2.1
 [0.2.0]: https://gitlab.com/geovisio/cli/-/compare/0.1.0...0.2.0
 [0.1.0]: https://gitlab.com/geovisio/cli/-/compare/0.0.5...0.1.0
 [0.0.5]: https://gitlab.com/geovisio/cli/-/compare/0.0.4...0.0.5
 [0.0.4]: https://gitlab.com/geovisio/cli/-/compare/0.0.3...0.0.4
 [0.0.3]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...0.0.3
 [0.0.2]: https://gitlab.com/geovisio/cli/-/compare/0.0.1...0.0.2
```

### Comparing `geovisio_cli-0.2.2/CODE_OF_CONDUCT.md` & `geovisio_cli-0.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/LICENSE` & `geovisio_cli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/Makefile` & `geovisio_cli-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/README.md` & `geovisio_cli-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 ## Install
 
 GeoVisio CLI can be installed using two methods:
 
 - From [PyPI](https://pypi.org/project/geovisio_cli/), the Python central package repository
 - Using this [Git repository](https://gitlab.com/geovisio/cli)
 
+Geovisio CLI is compatible with all Python versions >= 3.8.
+
 ### From PyPI
 
 Just launch this command:
 
 ```bash
 pip install geovisio_cli
 ```
```

### Comparing `geovisio_cli-0.2.2/USAGE.md` & `geovisio_cli-0.2.3/USAGE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `geovisio`
 
-GeoVisio command-line client
+GeoVisio command-line client (v0.2.3)
 
 **Usage**:
 
 ```console
 $ geovisio [OPTIONS] COMMAND [ARGS]...
 ```
```

### Comparing `geovisio_cli-0.2.2/geovisio_cli/auth.py` & `geovisio_cli-0.2.3/geovisio_cli/auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/geovisio_cli/main.py` & `geovisio_cli-0.2.3/geovisio_cli/main.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/geovisio_cli/sequence.py` & `geovisio_cli-0.2.3/geovisio_cli/sequence.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/geovisio_cli/utils.py` & `geovisio_cli-0.2.3/geovisio_cli/utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/pyproject.toml` & `geovisio_cli-0.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-[build-system]
-requires = ["flit_core ~= 3.8,<4"]
-build-backend = "flit_core.buildapi"
-
 [project]
 name = "geovisio_cli"
 authors = [
     {name = "Antoine Desbordes", email = "antoine.desbordes@gmail.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
@@ -13,17 +9,18 @@
 dynamic = ["version", "description"]
 dependencies = [
     "requests ~= 2.28.0",
     "typer ~= 0.9.0",
     "rich[all] ~= 13.3.0",
     "toml ~= 0.10.2",
     "qrcode ~= 7.4.2",
-    "geopic-tag-reader ~= 0.1.3",
+    "geopic-tag-reader ~= 0.2.0",
     "packaging ~= 23.1",
 ]
+requires-python = ">=3.8"
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/cli"
 
 [project.scripts]
 geovisio="geovisio_cli.main:app"
 
@@ -44,7 +41,11 @@
 ]
 build = ["flit ~= 3.8.0"]
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
+
+[build-system]
+requires = ["flit_core ~= 3.8,<4"]
+build-backend = "flit_core.buildapi"
```

### Comparing `geovisio_cli-0.2.2/tests/fixtures/e1.jpg` & `geovisio_cli-0.2.3/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/fixtures/e2.jpg` & `geovisio_cli-0.2.3/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/fixtures/e3.jpg` & `geovisio_cli-0.2.3/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/integration/conftest.py` & `geovisio_cli-0.2.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.2.3/tests/integration/docker-compose-geovisio.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/integration/docker-compose-gitlab-override.yml` & `geovisio_cli-0.2.3/tests/integration/docker-compose-gitlab-override.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/integration/keycloak-realm.json` & `geovisio_cli-0.2.3/tests/integration/keycloak-realm.json`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/integration/test_auth.py` & `geovisio_cli-0.2.3/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/integration/test_upload.py` & `geovisio_cli-0.2.3/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/test_process.py` & `geovisio_cli-0.2.3/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/tests/test_sequence.py` & `geovisio_cli-0.2.3/tests/test_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,25 @@
         ),
     ),
 )
 def test_sort_files_time(data, method, expected):
     dataPictures = []
     for p in data:
         name, ts = p
-        m = reader.GeoPicTags(47.7, -1.78, ts, 0, "flat", "Panoramax", "180++", 4)
+        m = reader.GeoPicTags(
+            lon=47.7,
+            lat=-1.78,
+            ts=ts,
+            heading=0,
+            type="flat",
+            make="Panoramax",
+            model="180++",
+            focal_length=4,
+            crop=None,
+        )
         dataPictures.append(sequence.Picture(path=name, metadata=m))
 
     resPictures = sequence._sort_files(dataPictures, method)
     assert expected == [pic.path for pic in resPictures]
 
 
 def test_rw_sequence_toml(tmp_path):
```

### Comparing `geovisio_cli-0.2.2/tests/test_utils.py` & `geovisio_cli-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.2/PKG-INFO` & `geovisio_cli-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
 Requires-Dist: typer ~= 0.9.0
 Requires-Dist: rich[all] ~= 13.3.0
 Requires-Dist: toml ~= 0.10.2
 Requires-Dist: qrcode ~= 7.4.2
-Requires-Dist: geopic-tag-reader ~= 0.1.3
+Requires-Dist: geopic-tag-reader ~= 0.2.0
 Requires-Dist: packaging ~= 23.1
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
 Requires-Dist: black ~= 22.8.0 ; extra == "dev"
 Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
 Requires-Dist: types-requests ~= 2.28.0 ; extra == "dev"
 Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
 Requires-Dist: testcontainers-compose ~= 0.0.1rc1 ; extra == "dev"
@@ -64,14 +65,16 @@
 ## Install
 
 GeoVisio CLI can be installed using two methods:
 
 - From [PyPI](https://pypi.org/project/geovisio_cli/), the Python central package repository
 - Using this [Git repository](https://gitlab.com/geovisio/cli)
 
+Geovisio CLI is compatible with all Python versions >= 3.8.
+
 ### From PyPI
 
 Just launch this command:
 
 ```bash
 pip install geovisio_cli
 ```
```


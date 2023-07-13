# Comparing `tmp/metget-0.2.4.tar.gz` & `tmp/metget-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metget-0.2.4.tar", last modified: Tue Jul 11 21:34:31 2023, max compression
+gzip compressed data, was "metget-0.2.5.tar", last modified: Thu Jul 13 19:37:07 2023, max compression
```

## Comparing `metget-0.2.4.tar` & `metget-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.566354 metget-0.2.4/
--rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.4/LICENSE.md
--rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:34:31.564894 metget-0.2.4/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)    10600 2023-07-11 21:13:31.000000 metget-0.2.4/README.md
--rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-11 21:34:02.000000 metget-0.2.4/pyproject.toml
--rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-11 21:34:31.566412 metget-0.2.4/setup.cfg
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.559345 metget-0.2.4/src/
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.560871 metget-0.2.4/src/metget.egg-info/
--rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/SOURCES.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/dependency_links.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/entry_points.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/requires.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-11 21:34:31.000000 metget-0.2.4/src/metget.egg-info/top_level.txt
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.563703 metget-0.2.4/src/metget_client/
--rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-11 21:34:02.000000 metget-0.2.4/src/metget_client/__init__.py
--rw-r--r--   0 zcobell    (502) staff       (20)    19413 2023-07-11 21:17:13.000000 metget-0.2.4/src/metget_client/metget_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)    10010 2023-07-11 21:30:40.000000 metget-0.2.4/src/metget_client/metget_client.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/metget_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/metget_data.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/metget_environment.py
--rw-r--r--   0 zcobell    (502) staff       (20)    17241 2023-07-11 02:36:15.000000 metget-0.2.4/src/metget_client/metget_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     3937 2023-07-10 15:06:46.000000 metget-0.2.4/src/metget_client/metget_track.py
--rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.4/src/metget_client/spinnerlogger.py
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-11 21:34:31.564684 metget-0.2.4/test/
--rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_cli.py
--rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     8940 2023-07-11 21:28:48.000000 metget-0.2.4/test/test_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2632 2023-07-11 21:08:59.000000 metget-0.2.4/test/test_track.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.993081 metget-0.2.5/
+-rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.2.5/LICENSE.md
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-13 19:37:07.992939 metget-0.2.5/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)    10600 2023-07-11 21:13:31.000000 metget-0.2.5/README.md
+-rw-r--r--   0 zcobell    (502) staff       (20)     1643 2023-07-13 18:52:45.000000 metget-0.2.5/pyproject.toml
+-rw-r--r--   0 zcobell    (502) staff       (20)       38 2023-07-13 19:37:07.993121 metget-0.2.5/setup.cfg
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.987687 metget-0.2.5/src/
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.989073 metget-0.2.5/src/metget.egg-info/
+-rw-r--r--   0 zcobell    (502) staff       (20)    11522 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)      649 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/SOURCES.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        1 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/dependency_links.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       59 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/entry_points.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       26 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/requires.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       14 2023-07-13 19:37:07.000000 metget-0.2.5/src/metget.egg-info/top_level.txt
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.991542 metget-0.2.5/src/metget_client/
+-rw-r--r--   0 zcobell    (502) staff       (20)       68 2023-07-13 18:52:45.000000 metget-0.2.5/src/metget_client/__init__.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    19413 2023-07-11 21:17:13.000000 metget-0.2.5/src/metget_client/metget_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    10010 2023-07-11 21:30:40.000000 metget-0.2.5/src/metget_client/metget_client.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2766 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/metget_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2780 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/metget_data.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2798 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/metget_environment.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    17369 2023-07-13 18:47:43.000000 metget-0.2.5/src/metget_client/metget_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     3981 2023-07-13 18:48:29.000000 metget-0.2.5/src/metget_client/metget_track.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     5540 2023-07-08 15:58:57.000000 metget-0.2.5/src/metget_client/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2023-07-13 19:37:07.992683 metget-0.2.5/test/
+-rw-r--r--   0 zcobell    (502) staff       (20)    10257 2023-07-11 21:08:59.000000 metget-0.2.5/test/test_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)      240 2023-07-11 21:08:59.000000 metget-0.2.5/test/test_cli.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     1617 2023-07-11 21:08:59.000000 metget-0.2.5/test/test_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     8688 2023-07-13 18:49:26.000000 metget-0.2.5/test/test_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2560 2023-07-13 18:49:26.000000 metget-0.2.5/test/test_track.py
```

### Comparing `metget-0.2.4/LICENSE.md` & `metget-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/PKG-INFO` & `metget-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.4
+Version: 0.2.5
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.2.4/README.md` & `metget-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/pyproject.toml` & `metget-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metget"
-version = "0.2.4"
+version = "0.2.5"
 description = "A client package for interaction with a MetGet server instance"
 authors = [
     { name = "Zach Cobell", email = "zcobell@thewaterinstitute.org" },
 ]
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.8"
@@ -40,15 +40,15 @@
 [tool.setuptools.dynamic]
 version = { attr = "metget_client.__version__" }
 
 [project.scripts]
 metget = "metget_client:metget_client_cli"
 
 [tool.bumpver]
-current_version = "0.2.4"
+current_version = "0.2.5"
 version_pattern = 'MAJOR.MINOR.PATCH[PYTAGNUM]'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `metget-0.2.4/src/metget.egg-info/PKG-INFO` & `metget-0.2.5/src/metget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.2.4
+Version: 0.2.5
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.2.4/src/metget.egg-info/SOURCES.txt` & `metget-0.2.5/src/metget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/src/metget_client/metget_build.py` & `metget-0.2.5/src/metget_client/metget_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/src/metget_client/metget_client.py` & `metget-0.2.5/src/metget_client/metget_client.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/src/metget_client/metget_credits.py` & `metget-0.2.5/src/metget_client/metget_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/src/metget_client/metget_data.py` & `metget-0.2.5/src/metget_client/metget_data.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/src/metget_client/metget_environment.py` & `metget-0.2.5/src/metget_client/metget_environment.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/src/metget_client/metget_status.py` & `metget-0.2.5/src/metget_client/metget_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,29 +99,30 @@
         This method is used to get the status of the track data (NHC)
 
         Args:
             model: The model to get the status for
         """
         import requests
         import prettytable
+        import json
 
         url = "{:s}/status?model={:s}".format(self.__environment["endpoint"], model)
         url = self.__add_url_start_end_parameters(url)
         if self.__args.storm:
             url += "&storm={:s}".format(self.__args.storm)
         if self.__args.basin:
             url += "&basin={:s}".format(self.__args.basin)
 
         response = requests.get(
             url, headers={"x-api-key": self.__environment["apikey"]}
         )
         data = response.json()["body"]
 
         if self.__args.format == "json":
-            print(data)
+            print(json.dumps(data))
         elif self.__args.format == "pretty":
             storm_tracks = []
             for year in data["best_track"].keys():
                 for basin in data["best_track"][year].keys():
                     for storm in data["best_track"][year][basin]:
                         start_time = data["best_track"][year][basin][storm][
                             "best_track_start"
@@ -200,29 +201,30 @@
             model: The model to get the status for
 
         Returns:
             None
         """
         import requests
         import prettytable
+        import json
 
         url = "{:s}/status?model={:s}".format(self.__environment["endpoint"], model)
         url = self.__add_url_start_end_parameters(url)
         if self.__args.storm:
             url += "&storm={:s}".format(self.__args.storm)
             if self.__args.ensemble_member:
                 url += "&member={:s}".format(self.__args.ensemble_member)
 
         response = requests.get(
             url, headers={"x-api-key": self.__environment["apikey"]}
         )
         data = response.json()["body"]
 
         if self.__args.format == "json":
-            print(data)
+            print(json.dumps(data))
         elif self.__args.format == "pretty":
             if self.__args.storm and self.__args.ensemble_member:
                 model_name = "{:s}-{:s}-{:s}".format(
                     model, self.__args.storm, self.__args.ensemble_member
                 )
                 self.__print_status_generic(
                     model_name, data[self.__args.storm][self.__args.ensemble_member]
@@ -345,17 +347,18 @@
             model: The model to get the status for
             data: The data to print the status for
 
         Returns:
             None
         """
         import prettytable
+        import json
 
         if self.__args.format == "json":
-            print(data)
+            print(json.dumps(data))
         elif self.__args.format == "pretty":
             if data == {}:
                 print("No data found.")
                 return
 
             if self.__args.storm:
                 model_name = "{:s}-{:s}".format(model.upper(), self.__args.storm)
@@ -424,17 +427,18 @@
             data: The data to get the status for
 
         Returns:
             None
         """
         import prettytable
         from datetime import datetime, timedelta
+        import json
 
         if self.__args.format == "json":
-            print(data)
+            print(json.dumps(data))
         elif self.__args.format == "pretty":
 
             complete_cycles = data["cycles_complete"]
 
             print(
                 "Status for model: {:s} (class: {:s})".format(model, self.__model_class)
             )
```

### Comparing `metget-0.2.4/src/metget_client/metget_track.py` & `metget-0.2.5/src/metget_client/metget_track.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
     def get_track(self):
         """
         This method is used to get the track data from the api
         """
         import requests
         from datetime import datetime
+        import json
 
         url = self.__environment["endpoint"] + "/stormtrack"
 
         if not self.__args.storm:
             raise ValueError("Storm must be specified for track data")
 
         if not self.__args.type:
@@ -89,18 +90,18 @@
             raise ValueError("Type must be besttrack or forecast")
 
         # Get the track data with the requests library
         response = requests.get(url, params=params)
 
         # Check the response status code
         if response.status_code == 200:
-            print(response.json()["body"]["geojson"])
+            print(json.dumps(response.json()["body"]["geojson"]))
         else:
             print("Error: {}".format(response.status_code))
-            print(response.json())
+            print(json.dumps(response.json()))
 
 
 def metget_track(args: argparse.Namespace) -> None:
     """
     This method is used to get the track data from the api
 
     Args:
```

### Comparing `metget-0.2.4/src/metget_client/spinnerlogger.py` & `metget-0.2.5/src/metget_client/spinnerlogger.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/test/test_build.py` & `metget-0.2.5/test/test_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/test/test_credits.py` & `metget-0.2.5/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.2.4/test/test_status.py` & `metget-0.2.5/test/test_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     args.format = "json"
 
     s = MetGetStatus(args)
     with requests_mock.Mocker() as m:
         m.get(METGET_DMY_ENDPOINT + "/status?model=gfs", json=GFS_STATUS_JSON)
         s.get_status()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         out_dict = json.loads(out)
         assert out_dict == GFS_STATUS_JSON["body"]
 
 
 def test_status_hwrf(capfd) -> None:
     """
     Tests the status command for the HWRF model
@@ -87,15 +86,14 @@
     args.format = "json"
 
     s = MetGetStatus(args)
     with requests_mock.Mocker() as m:
         m.get(url, json=HWRF_STATUS_JSON)
         s.get_status()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         out_dict = json.loads(out)
         assert out_dict == HWRF_STATUS_JSON["body"]
 
     args.storm = "bret03l"
     s2 = MetGetStatus(args)
     url = (
         METGET_DMY_ENDPOINT
@@ -109,15 +107,14 @@
             }
         )
     )
     with requests_mock.Mocker() as m:
         m.get(url, json=HWRF_STATUS_BRET_JSON)
         s2.get_status()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         out_dict = json.loads(out)
         assert out_dict == HWRF_STATUS_BRET_JSON["body"]
 
     args.format = "pretty"
     s3 = MetGetStatus(args)
     with requests_mock.Mocker() as m:
         m.get(url, json=HWRF_STATUS_BRET_JSON)
@@ -156,15 +153,14 @@
             + "/status?"
             + urlencode({"model": "nhc", "start": "2023-06-01"}),
             json=NHC_STATUS_JSON,
         )
         s = MetGetStatus(args)
         s.get_status()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         assert json.loads(out) == NHC_STATUS_JSON["body"]
 
     args.format = "pretty"
     with requests_mock.Mocker() as m:
         m.get(
             METGET_DMY_ENDPOINT
             + "/status?"
@@ -213,15 +209,14 @@
                 }
             ),
             json=GEFS_STATUS_JSON_C00,
         )
         s = MetGetStatus(args)
         s.get_status()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         assert json.loads(out) == GEFS_STATUS_JSON_C00["body"]["c00"]
 
     args.format = "pretty"
     with requests_mock.Mocker() as m:
         m.get(
             METGET_DMY_ENDPOINT
             + "/status?"
@@ -248,15 +243,14 @@
             + "/status?"
             + urlencode({"model": "gefs", "start": "2023-06-01", "end": "2023-06-08"}),
             json=GEFS_STATUS_JSON,
         )
         s = MetGetStatus(args)
         s.get_status()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         assert json.loads(out) == GEFS_STATUS_JSON["body"]
 
     args.format = "pretty"
     with requests_mock.Mocker() as m:
         m.get(
             METGET_DMY_ENDPOINT
             + "/status?"
@@ -303,15 +297,14 @@
                 }
             ),
             json=COAMPS_CTCX_STATUS_JSON,
         )
         s = MetGetStatus(args)
         s.get_status()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         assert json.loads(out) == COAMPS_CTCX_STATUS_JSON["body"]
 
     args.format = "pretty"
     with requests_mock.Mocker() as m:
         m.get(
             METGET_DMY_ENDPOINT
             + "/status?"
```

### Comparing `metget-0.2.4/test/test_track.py` & `metget-0.2.5/test/test_track.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,14 @@
                 }
             )
         )
         m.get(url, json=NHC_IAN_BESTRACK_JSON)
         s = MetGetTrack(args)
         s.get_track()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         out_dict = json.loads(out)
         assert out_dict == NHC_IAN_BESTRACK_JSON["body"]["geojson"]
 
 
 def test_forecast_track(capfd) -> None:
     """
     Tests the forecast track data
@@ -92,10 +91,9 @@
                 }
             )
         )
         m.get(url, json=NHC_IAN_FORECAST_JSON)
         s = MetGetTrack(args)
         s.get_track()
         out, err = capfd.readouterr()
-        out = out.replace("'", '"')
         out_dict = json.loads(out)
         assert out_dict == NHC_IAN_FORECAST_JSON["body"]["geojson"]
```


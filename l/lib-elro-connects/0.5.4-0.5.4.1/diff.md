# Comparing `tmp/lib-elro-connects-0.5.4.tar.gz` & `tmp/lib-elro-connects-0.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-elro-connects-0.5.4.tar", last modified: Mon Sep  5 16:47:46 2022, max compression
+gzip compressed data, was "lib-elro-connects-0.5.4.1.tar", last modified: Thu Jul 13 14:08:10 2023, max compression
```

## Comparing `lib-elro-connects-0.5.4.tar` & `lib-elro-connects-0.5.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:47:46.751641 lib-elro-connects-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-09-05 16:47:46.751641 lib-elro-connects-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:47:46.751641 lib-elro-connects-0.5.4/elro/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/elro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9494 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/elro/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/elro/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/elro/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/elro/device.py
--rw-r--r--   0 runner    (1001) docker     (121)    10151 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/elro/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:47:46.751641 lib-elro-connects-0.5.4/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/examples/cloud_login_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5533 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/examples/fire_alarm_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 16:47:46.751641 lib-elro-connects-0.5.4/lib_elro_connects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-09-05 16:47:46.000000 lib-elro-connects-0.5.4/lib_elro_connects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-05 16:47:46.000000 lib-elro-connects-0.5.4/lib_elro_connects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 16:47:46.000000 lib-elro-connects-0.5.4/lib_elro_connects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-05 16:47:46.000000 lib-elro-connects-0.5.4/lib_elro_connects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-05 16:47:46.000000 lib-elro-connects-0.5.4/lib_elro_connects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-09-05 16:47:46.751641 lib-elro-connects-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-09-05 16:47:38.000000 lib-elro-connects-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:10.970515 lib-elro-connects-0.5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-13 14:08:10.970515 lib-elro-connects-0.5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:10.970515 lib-elro-connects-0.5.4.1/elro/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/elro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/elro/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/elro/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/elro/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/elro/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/elro/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:10.970515 lib-elro-connects-0.5.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/examples/cloud_login_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5573 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/examples/fire_alarm_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:08:10.970515 lib-elro-connects-0.5.4.1/lib_elro_connects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-13 14:08:10.000000 lib-elro-connects-0.5.4.1/lib_elro_connects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-13 14:08:10.000000 lib-elro-connects-0.5.4.1/lib_elro_connects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:08:10.000000 lib-elro-connects-0.5.4.1/lib_elro_connects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 14:08:10.000000 lib-elro-connects-0.5.4.1/lib_elro_connects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 14:08:10.000000 lib-elro-connects-0.5.4.1/lib_elro_connects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 14:08:10.970515 lib-elro-connects-0.5.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-13 14:07:55.000000 lib-elro-connects-0.5.4.1/setup.py
```

### Comparing `lib-elro-connects-0.5.4/LICENSE` & `lib-elro-connects-0.5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-elro-connects-0.5.4/PKG-INFO` & `lib-elro-connects-0.5.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-elro-connects
-Version: 0.5.4
+Version: 0.5.4.1
 Summary: Elro Connects P1 API
 Home-page: https://github.com/jbouwh/lib-elro-connects
 Author: Jan Bouwhuis
 Author-email: jan@jbsoft.nl
 License: MIT Licence
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Home Automation
@@ -16,27 +16,26 @@
 Provides-Extra: test
 License-File: LICENSE
 
 ![PyPI version](https://badge.fury.io/py/lib-elro-connects.svg)
 
 **NOTE**
 
-This project is suppose to proved an API to the Elro connects K1 adapter
+This project is suppose to provide an API for the Elro connects K1 adapter.
+Thare is a Elro Connects K2 adapter, but is not supported with this library.
 
 The code idea is based on the the code of Bas van den Berg https://github.com/dib0/elro_connects.
 
 Aim of this library is to provide a API for the Elro Connects P1 connector. Example code is included.
 
 The code requires Python 3.9 or higher.
 
-A PyPi package wil become avaiable. To be installed with:
+A PyPi package wil become available. To be installed with:
 `pip install lib-elro-connects`
 
-THIS CODE IS NOT READY FOR PRODUCTION YET, but let me know if you would like to help.
-
 Kind regards,
 
 Jan Bouwhuis
 
 ## Supported Devices by ELRO K1 connects SF40GA
 
 ### Fire alarms
```

### Comparing `lib-elro-connects-0.5.4/README.md` & `lib-elro-connects-0.5.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ![PyPI version](https://badge.fury.io/py/lib-elro-connects.svg)
 
 **NOTE**
 
-This project is suppose to proved an API to the Elro connects K1 adapter
+This project is suppose to provide an API for the Elro connects K1 adapter.
+Thare is a Elro Connects K2 adapter, but is not supported with this library.
 
 The code idea is based on the the code of Bas van den Berg https://github.com/dib0/elro_connects.
 
 Aim of this library is to provide a API for the Elro Connects P1 connector. Example code is included.
 
 The code requires Python 3.9 or higher.
 
-A PyPi package wil become avaiable. To be installed with:
+A PyPi package wil become available. To be installed with:
 `pip install lib-elro-connects`
 
-THIS CODE IS NOT READY FOR PRODUCTION YET, but let me know if you would like to help.
-
 Kind regards,
 
 Jan Bouwhuis
 
 ## Supported Devices by ELRO K1 connects SF40GA
 
 ### Fire alarms
```

### Comparing `lib-elro-connects-0.5.4/elro/api.py` & `lib-elro-connects-0.5.4.1/elro/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,19 @@
                         command_data,
                         iteration,
                         raw_data[0].decode("utf-8").strip()
                         if raw_data[0] is not None
                         else None,
                     )
                     self._protocol.datagram_data = self._loop.create_future()
+                    if (
+                        raw_data[0].decode("utf-8").strip().casefold()
+                        == "{ST_answer_OK}".casefold()
+                    ):
+                        continue
                     data = validate_json(raw_data[0])
                     params = data["params"]
                     cmd_id = params["data"]["cmdId"]
                     content = params["data"].get(attributes["content_field"], "")
                     if Command(cmd_id) in attributes["receive_types"]:
                         self._transport.sendto(ACK_APP.encode("utf-8"))
                         if content == attributes["content_sync_finished"]:
```

### Comparing `lib-elro-connects-0.5.4/elro/auth.py` & `lib-elro-connects-0.5.4.1/elro/auth.py`

 * *Files identical despite different names*

### Comparing `lib-elro-connects-0.5.4/elro/command.py` & `lib-elro-connects-0.5.4.1/elro/command.py`

 * *Files identical despite different names*

### Comparing `lib-elro-connects-0.5.4/elro/device.py` & `lib-elro-connects-0.5.4.1/elro/device.py`

 * *Files identical despite different names*

### Comparing `lib-elro-connects-0.5.4/elro/utils.py` & `lib-elro-connects-0.5.4.1/elro/utils.py`

 * *Files identical despite different names*

### Comparing `lib-elro-connects-0.5.4/examples/cloud_login_demo.py` & `lib-elro-connects-0.5.4.1/examples/cloud_login_demo.py`

 * *Files identical despite different names*

### Comparing `lib-elro-connects-0.5.4/examples/fire_alarm_demo.py` & `lib-elro-connects-0.5.4.1/examples/fire_alarm_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
                 names = await self.async_process_command(GET_DEVICE_NAMES)
                 update_state_data(data, names)
                 print(f"=={datetime.now()}")
                 for key, item in data.items():
                     print(
                         f"{key} ({item.get('name')}): status={item['device_state']} data={item['device_status_data']}"
                     )
-            except Exception:  # pylint: disable=broad-except
-                pass
+            except Exception as err:  # pylint: disable=broad-except
+                print(f"Exception caught {err.args}")
             finally:
                 await asyncio.sleep(INTERVAL)
 
     async def async_demo2(self) -> None:
         """Main routine to demonstrate the API code."""
         logging.basicConfig(level=logging.DEBUG)
         # You can call await self.async_connect() but if there is no actice session
```

### Comparing `lib-elro-connects-0.5.4/lib_elro_connects.egg-info/PKG-INFO` & `lib-elro-connects-0.5.4.1/lib_elro_connects.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-elro-connects
-Version: 0.5.4
+Version: 0.5.4.1
 Summary: Elro Connects P1 API
 Home-page: https://github.com/jbouwh/lib-elro-connects
 Author: Jan Bouwhuis
 Author-email: jan@jbsoft.nl
 License: MIT Licence
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Home Automation
@@ -16,27 +16,26 @@
 Provides-Extra: test
 License-File: LICENSE
 
 ![PyPI version](https://badge.fury.io/py/lib-elro-connects.svg)
 
 **NOTE**
 
-This project is suppose to proved an API to the Elro connects K1 adapter
+This project is suppose to provide an API for the Elro connects K1 adapter.
+Thare is a Elro Connects K2 adapter, but is not supported with this library.
 
 The code idea is based on the the code of Bas van den Berg https://github.com/dib0/elro_connects.
 
 Aim of this library is to provide a API for the Elro Connects P1 connector. Example code is included.
 
 The code requires Python 3.9 or higher.
 
-A PyPi package wil become avaiable. To be installed with:
+A PyPi package wil become available. To be installed with:
 `pip install lib-elro-connects`
 
-THIS CODE IS NOT READY FOR PRODUCTION YET, but let me know if you would like to help.
-
 Kind regards,
 
 Jan Bouwhuis
 
 ## Supported Devices by ELRO K1 connects SF40GA
 
 ### Fire alarms
```

### Comparing `lib-elro-connects-0.5.4/setup.cfg` & `lib-elro-connects-0.5.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `lib-elro-connects-0.5.4/setup.py` & `lib-elro-connects-0.5.4.1/setup.py`

 * *Files identical despite different names*


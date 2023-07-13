# Comparing `tmp/jcloud-0.2.9.dev3.tar.gz` & `tmp/jcloud-0.2.9.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcloud-0.2.9.dev3.tar", last modified: Tue May 16 08:49:54 2023, max compression
+gzip compressed data, was "jcloud-0.2.9.dev4.tar", last modified: Thu May 18 10:10:20 2023, max compression
```

## Comparing `jcloud-0.2.9.dev3.tar` & `jcloud-0.2.9.dev4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.972805 jcloud-0.2.9.dev3/jcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/env_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/jcloud/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/parsers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.972805 jcloud-0.2.9.dev3/jcloud/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/jcloud/resources/project-template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/executor1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/resources/project-template/flow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/jcloud/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:54.972805 jcloud-0.2.9.dev3/jcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 08:49:54.000000 jcloud-0.2.9.dev3/jcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:49:54.976805 jcloud-0.2.9.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-16 08:49:50.000000 jcloud-0.2.9.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.454125 jcloud-0.2.9.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-18 10:10:20.454125 jcloud-0.2.9.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.450124 jcloud-0.2.9.dev4/jcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 10:10:19.000000 jcloud-0.2.9.dev4/jcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/env_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.450124 jcloud-0.2.9.dev4/jcloud/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/parsers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.446124 jcloud-0.2.9.dev4/jcloud/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.450124 jcloud-0.2.9.dev4/jcloud/resources/project-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/resources/project-template/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.454125 jcloud-0.2.9.dev4/jcloud/resources/project-template/executor1/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/resources/project-template/executor1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/resources/project-template/executor1/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/resources/project-template/executor1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/resources/project-template/flow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/jcloud/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.450124 jcloud-0.2.9.dev4/jcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-18 10:10:20.000000 jcloud-0.2.9.dev4/jcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-18 10:10:20.000000 jcloud-0.2.9.dev4/jcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:10:20.000000 jcloud-0.2.9.dev4/jcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 10:10:20.000000 jcloud-0.2.9.dev4/jcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:10:20.000000 jcloud-0.2.9.dev4/jcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 10:10:20.000000 jcloud-0.2.9.dev4/jcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 10:10:20.000000 jcloud-0.2.9.dev4/jcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 10:10:20.454125 jcloud-0.2.9.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-18 10:10:12.000000 jcloud-0.2.9.dev4/setup.py
```

### Comparing `jcloud-0.2.9.dev3/LICENSE` & `jcloud-0.2.9.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/PKG-INFO` & `jcloud-0.2.9.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.9.dev3
+Version: 0.2.9.dev4
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.9.dev3 Summary: Simplify
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.9.dev4 Summary: Simplify
 deploying and managing Jina projects on Jina Cloud Home-page: https://
 github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
 Keywords: jcloud neural-search serverless deployment devops mlops Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
```

### Comparing `jcloud-0.2.9.dev3/README.md` & `jcloud-0.2.9.dev4/README.md`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/__main__.py` & `jcloud-0.2.9.dev4/jcloud/__main__.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/api.py` & `jcloud-0.2.9.dev4/jcloud/api.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/constants.py` & `jcloud-0.2.9.dev4/jcloud/constants.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/env_helper.py` & `jcloud-0.2.9.dev4/jcloud/env_helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/flow.py` & `jcloud-0.2.9.dev4/jcloud/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,34 +125,41 @@
                 async with get_aiohttp_session() as session:
                     async with session.post(
                         url=FLOWS_API,
                         headers=self.auth_header,
                         **await self._get_post_params(),
                     ) as response:
                         json_response = await response.json()
-                        _exit_if_response_error(
-                            response,
-                            expected_status=HTTPStatus.CREATED,
-                            json_response=json_response,
-                        )
-
+                        response.raise_for_status()
                         self.flow_id: str = json_response['id']
                         logger.info(
                             f'Successfully submitted flow with ID {self.flow_id}'
                         )
                         return json_response
             except aiohttp.ClientConnectionError as e:
                 if i == 0:
                     logger.debug(
                         'POST /flows at 1st attempt failed, will retry in 2s...'
                     )
                     await asyncio.sleep(2)
                 else:
                     logger.debug('POST /flows retry failed too...')
                     raise e
+            except aiohttp.ClientResponseError as e:
+                if e.status == HTTPStatus.SERVICE_UNAVAILABLE and i == 0:
+                    logger.debug(
+                        'POST /flows at 1st attempt failed, will retry in 2s...'
+                    )
+                    await asyncio.sleep(2)
+                else:
+                    _exit_if_response_error(
+                        response,
+                        expected_status=HTTPStatus.CREATED,
+                        json_response=json_response,
+                    )
 
     async def update(self):
         async def _update():
             for i in range(2):
                 try:
                     async with get_aiohttp_session() as session:
                         api_url = FLOWS_API + "/" + self.flow_id
```

### Comparing `jcloud-0.2.9.dev3/jcloud/helper.py` & `jcloud-0.2.9.dev4/jcloud/helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/normalize.py` & `jcloud-0.2.9.dev4/jcloud/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/__init__.py` & `jcloud-0.2.9.dev4/jcloud/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/base.py` & `jcloud-0.2.9.dev4/jcloud/parsers/base.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/custom_actions.py` & `jcloud-0.2.9.dev4/jcloud/parsers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/helper.py` & `jcloud-0.2.9.dev4/jcloud/parsers/helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/list.py` & `jcloud-0.2.9.dev4/jcloud/parsers/list.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/logs.py` & `jcloud-0.2.9.dev4/jcloud/parsers/logs.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/normalize.py` & `jcloud-0.2.9.dev4/jcloud/parsers/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/parsers/remove.py` & `jcloud-0.2.9.dev4/jcloud/parsers/remove.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud/survey.py` & `jcloud-0.2.9.dev4/jcloud/survey.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/jcloud.egg-info/PKG-INFO` & `jcloud-0.2.9.dev4/jcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.9.dev3
+Version: 0.2.9.dev4
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.9.dev3 Summary: Simplify
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.9.dev4 Summary: Simplify
 deploying and managing Jina projects on Jina Cloud Home-page: https://
 github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
 Keywords: jcloud neural-search serverless deployment devops mlops Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
```

### Comparing `jcloud-0.2.9.dev3/jcloud.egg-info/SOURCES.txt` & `jcloud-0.2.9.dev4/jcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.9.dev3/setup.py` & `jcloud-0.2.9.dev4/setup.py`

 * *Files identical despite different names*


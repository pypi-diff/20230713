# Comparing `tmp/ujenkins-0.8.1.tar.gz` & `tmp/ujenkins-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ujenkins-0.8.1.tar", last modified: Thu Jan  5 10:15:53 2023, max compression
+gzip compressed data, was "ujenkins-0.9.0.tar", last modified: Sat Mar  4 20:42:01 2023, max compression
```

## Comparing `ujenkins-0.8.1.tar` & `ujenkins-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:15:53.339827 ujenkins-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-05 10:15:41.000000 ujenkins-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-05 10:15:41.000000 ujenkins-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-01-05 10:15:53.339827 ujenkins-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-01-05 10:15:41.000000 ujenkins-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-05 10:15:41.000000 ujenkins-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-05 10:15:53.339827 ujenkins-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-01-05 10:15:41.000000 ujenkins-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:15:53.335827 ujenkins-0.8.1/ujenkins/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:15:53.339827 ujenkins-0.8.1/ujenkins/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/adapters/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/adapters/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:15:53.339827 ujenkins-0.8.1/ujenkins/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/builds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/endpoints/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 10:15:41.000000 ujenkins-0.8.1/ujenkins/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:15:53.339827 ujenkins-0.8.1/ujenkins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-01-05 10:15:53.000000 ujenkins-0.8.1/ujenkins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-05 10:15:53.000000 ujenkins-0.8.1/ujenkins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 10:15:53.000000 ujenkins-0.8.1/ujenkins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-05 10:15:53.000000 ujenkins-0.8.1/ujenkins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-05 10:15:53.000000 ujenkins-0.8.1/ujenkins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:42:01.655234 ujenkins-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-04 20:41:49.000000 ujenkins-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-04 20:41:49.000000 ujenkins-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-03-04 20:42:01.655234 ujenkins-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-03-04 20:41:49.000000 ujenkins-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-04 20:41:49.000000 ujenkins-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-04 20:42:01.655234 ujenkins-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-04 20:41:49.000000 ujenkins-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:42:01.655234 ujenkins-0.9.0/ujenkins/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:42:01.655234 ujenkins-0.9.0/ujenkins/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/adapters/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/adapters/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:42:01.655234 ujenkins-0.9.0/ujenkins/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/builds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/endpoints/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 20:41:49.000000 ujenkins-0.9.0/ujenkins/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:42:01.655234 ujenkins-0.9.0/ujenkins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-03-04 20:42:01.000000 ujenkins-0.9.0/ujenkins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-04 20:42:01.000000 ujenkins-0.9.0/ujenkins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 20:42:01.000000 ujenkins-0.9.0/ujenkins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-04 20:42:01.000000 ujenkins-0.9.0/ujenkins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-04 20:42:01.000000 ujenkins-0.9.0/ujenkins.egg-info/top_level.txt
```

### Comparing `ujenkins-0.8.1/LICENSE` & `ujenkins-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/setup.cfg` & `ujenkins-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 [flake8]
 max-line-length = 99
 inline-quotes = single
 
 [testenv:pylint]
 skip_install = true
 deps = 
-	pylint==2.*
+	pylint==2.16
 	-r{toxinidir}/requirements.txt
 	-r{toxinidir}/tests/requirements.txt
 commands = 
 	pylint \
-	--disable=E0611,R0801,W0212,W0511,C0103,C0114,C0115,C0116,C0209,R0902,R0903,R0911 \
+	--disable=E0611,R0801,W0212,W0511,C0103,C0114,C0115,C0116,C0209,R0902,R0903,R0911,R1713 \
 	--good-names=e,i,k,v \
 	ujenkins tests
 
 [testenv:isort]
 deps = isort==5.*
 commands = isort ujenkins tests
```

### Comparing `ujenkins-0.8.1/setup.py` & `ujenkins-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/ujenkins/adapters/aio.py` & `ujenkins-0.9.0/ujenkins/adapters/aio.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,17 +142,22 @@
         if self.timeout and 'timeout' not in kwargs:
             kwargs['timeout'] = self.timeout
 
         if self.crumb:
             kwargs.setdefault('headers', {})
             kwargs['headers'].update(self.crumb)
 
+        if path.startswith('http'):
+            url = path
+        else:
+            url = self.host + path
+
         response = await self.session.request(
             method,
-            f'{self.host}{path}',
+            url,
             auth=self.auth,
             ssl=self.verify,
             **kwargs
         )
 
         body = await response.text()
```

### Comparing `ujenkins-0.8.1/ujenkins/adapters/sync.py` & `ujenkins-0.9.0/ujenkins/adapters/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,22 @@
         if self.timeout and 'timeout' not in kwargs:
             kwargs['timeout'] = self.timeout
 
         if self.crumb:
             kwargs.setdefault('headers', {})
             kwargs['headers'].update(self.crumb)
 
+        if path.startswith('http'):
+            url = path
+        else:
+            url = self.host + path
+
         response = self.session.request(
             method,
-            f'{self.host}{path}',
+            url,
             verify=self.verify,
             **kwargs
         )
 
         result = self._process(
             Response(response.status_code, response.headers, response.text),
             _callback
```

### Comparing `ujenkins-0.8.1/ujenkins/core.py` & `ujenkins-0.9.0/ujenkins/core.py`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/ujenkins/endpoints/builds.py` & `ujenkins-0.9.0/ujenkins/endpoints/builds.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
             # backward compatibility
             if isinstance(parameters, dict):
                 parameters.update(**kwargs)
             elif parameters is None:
                 parameters = kwargs
             else:
-                parameters = dict(parameters=parameters)
+                parameters = {'parameters': parameters}
                 parameters.update(**kwargs)
 
             formatted_parameters = [
                 {'name': k, 'value': str(v)} for k, v in parameters.items()
             ]  # type: Any
 
             if len(formatted_parameters) == 1:
```

### Comparing `ujenkins-0.8.1/ujenkins/endpoints/jobs.py` & `ujenkins-0.9.0/ujenkins/endpoints/jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 import json
 
 from functools import partial
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from ujenkins.exceptions import JenkinsNotFoundError
 
 
 class Jobs:
 
     def __init__(self, jenkins) -> None:
         self.jenkins = jenkins
 
-    def _get_all_jobs(self, url: str, parent: str) -> Dict[str, dict]:
+    def get(self, url: str = '', depth: Optional[int] = None) -> Dict[str, dict]:
+        """
+        Get jobs in selected folder, by default root is used.
+
+        Args:
+            url (str):
+                URL from job property, by default root is used.
+
+            depth (Optional[int]):
+                Get jobs recursively including folders from selected URL using
+                depth value, default is None which means no recursion.
+
+        Example:
 
+        .. code-block:: python
+
+            {'folder': {'_class': 'com.cloudbees.hudson.plugins.folder.Folder',
+                        'name': 'folder',
+                        'url': 'http://localhost/job/folder/'},
+             'project': {'_class': 'hudson.model.FreeStyleProject',
+                         'color': 'blue',
+                         'name': 'project',
+                         'url': 'http://localhost/job/project/'}}
+
+        Returns:
+            Dict[str, dict]: full name and job properties.
+        """
         def callback(response):
             all_jobs = {}
-
             jobs = json.loads(response.body)['jobs']
             for job in jobs:
-                all_jobs[parent + job['name']] = job
+                all_jobs[job['name']] = job
 
             return all_jobs
 
+        params = None
+
+        if depth:
+            tree = ',jobs[name,url,color'*depth + ']'*depth
+            params = {'tree': tree.lstrip(',')}
+
         return self.jenkins._request(
             'GET',
             url + '/api/json',
+            params=params,
             _callback=callback,
         )
 
-    def get(self) -> Dict[str, dict]:
-        """
-        Get dict of all existed jobs in system, including jobs in folder.
-
-        Example:
-
-        .. code-block:: python
-
-            {
-                'test': {
-                    'name': 'test',
-                    'url': 'http://localhost/job/test/'
-                },
-                'folder/foo': {
-                    'name': 'folder/job',
-                    'url': 'http://localhost/job/folder/job/foo/'
-                }
-            }
-
-        Returns:
-            Dict[str, dict]: name and job properties.
-        """
-        return self._get_all_jobs('', '')
-
     def get_info(self, name: str) -> dict:
         """
         Get detailed information of specified job.
 
         Args:
             name (str):
                 Job name.
```

### Comparing `ujenkins-0.8.1/ujenkins/endpoints/nodes.py` & `ujenkins-0.9.0/ujenkins/endpoints/nodes.py`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/ujenkins/endpoints/plugins.py` & `ujenkins-0.9.0/ujenkins/endpoints/plugins.py`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/ujenkins/endpoints/queue.py` & `ujenkins-0.9.0/ujenkins/endpoints/queue.py`

 * *Files 21% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 
         Returns:
             None
         """
         return self.jenkins._request(
             'POST',
             '/queue/cancelItem',
-            params=dict(id=item_id),
+            params={'id': item_id},
         )
```

### Comparing `ujenkins-0.8.1/ujenkins/endpoints/system.py` & `ujenkins-0.9.0/ujenkins/endpoints/system.py`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/ujenkins/endpoints/views.py` & `ujenkins-0.9.0/ujenkins/endpoints/views.py`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/ujenkins/helpers.py` & `ujenkins-0.9.0/ujenkins/helpers.py`

 * *Files identical despite different names*

### Comparing `ujenkins-0.8.1/ujenkins.egg-info/SOURCES.txt` & `ujenkins-0.9.0/ujenkins.egg-info/SOURCES.txt`

 * *Files identical despite different names*


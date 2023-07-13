# Comparing `tmp/django_google_cloud_tasks-2.3.2.tar.gz` & `tmp/django_google_cloud_tasks-2.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.3.2.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.3.2rc1.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.3.2.tar` & `django_google_cloud_tasks-2.3.2rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11358 2023-07-13 13:15:22.007288 django_google_cloud_tasks-2.3.2/LICENSE.md
--rw-r--r--   0        0        0      153 2023-07-13 13:15:22.007288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6245 2023-07-13 13:15:22.007288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-07-13 13:15:22.007288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-07-13 13:15:22.007288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1389 2023-07-13 13:15:22.007288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2023-07-13 13:15:22.007288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1870 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0      718 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py
--rw-r--r--   0        0        0        0 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4660 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2693 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4775 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2498 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2853 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0    10404 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      869 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     3014 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/django_cloud_tasks/views.py
--rw-r--r--   0        0        0     1192 2023-07-13 13:15:22.011288 django_google_cloud_tasks-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-07-24 16:19:35.292566 django_google_cloud_tasks-2.3.2rc1/LICENSE.md
+-rw-r--r--   0        0        0      153 2023-04-05 13:39:44.250424 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6245 2023-04-05 13:39:44.250645 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      446 2023-04-05 13:39:44.250738 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2023-04-05 13:39:44.250892 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1389 2023-04-05 13:39:44.250988 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2022-07-24 16:19:35.293209 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-05 13:39:44.251171 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2023-04-05 13:39:44.251329 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2022-07-24 16:19:35.294227 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2023-03-12 12:43:20.381324 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2023-04-05 13:39:44.251483 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-05 13:39:44.251578 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1870 2023-05-18 17:35:04.723809 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2023-04-05 13:39:44.251981 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2023-04-05 13:39:44.252082 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0      718 2023-07-12 22:34:08.147477 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py
+-rw-r--r--   0        0        0        0 2022-07-24 16:19:35.294840 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4660 2023-07-12 22:33:24.926967 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2022-07-24 16:19:35.295438 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2693 2023-07-12 21:35:20.582493 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2023-04-05 13:39:44.252578 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2023-04-05 13:39:44.252714 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4775 2023-04-05 13:39:44.252856 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     2498 2023-07-12 22:39:37.634109 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2853 2023-07-12 18:50:35.010367 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0    10404 2023-06-09 17:31:58.572005 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2022-07-24 16:19:35.296011 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-04-05 13:39:44.253503 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      869 2023-07-13 12:30:00.096447 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2022-07-24 16:19:35.296184 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3014 2023-05-18 17:35:04.725038 django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0     1196 2023-07-13 12:36:02.306115 django_google_cloud_tasks-2.3.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.3.2rc1/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.3.2/LICENSE.md` & `django_google_cloud_tasks-2.3.2rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/signals.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/routine_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tasks/task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.3.2rc1/django_cloud_tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.3.2/pyproject.toml` & `django_google_cloud_tasks-2.3.2rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.3.2"
+version = "2.3.2.rc1"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
```


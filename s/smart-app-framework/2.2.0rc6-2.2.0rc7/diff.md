# Comparing `tmp/smart_app_framework-2.2.0rc6-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.2.0rc7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 306342 bytes, number of entries: 333
+Zip file size: 306348 bytes, number of entries: 333
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -207,15 +207,15 @@
 -rw-r--r--  2.0 unx     6670 b- defN 80-Jan-01 00:00 smart_kit/action/http.py
 -rw-r--r--  2.0 unx     1106 b- defN 80-Jan-01 00:00 smart_kit/action/http_with_cookie.py
 -rw-r--r--  2.0 unx     2418 b- defN 80-Jan-01 00:00 smart_kit/action/smart_geo_action.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/compatibility/__init__.py
 -rw-r--r--  2.0 unx     3119 b- defN 80-Jan-01 00:00 smart_kit/compatibility/commands.py
 -rw-r--r--  2.0 unx     4159 b- defN 80-Jan-01 00:00 smart_kit/configs/__init__.py
 -rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 smart_kit/configs/logger_config.py
--rw-r--r--  2.0 unx     4120 b- defN 80-Jan-01 00:00 smart_kit/configs/settings.py
+-rw-r--r--  2.0 unx     4158 b- defN 80-Jan-01 00:00 smart_kit/configs/settings.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/handlers/__init__.py
 -rw-r--r--  2.0 unx     1187 b- defN 80-Jan-01 00:00 smart_kit/handlers/handle_close_app.py
 -rw-r--r--  2.0 unx     3008 b- defN 80-Jan-01 00:00 smart_kit/handlers/handle_respond.py
 -rw-r--r--  2.0 unx     1674 b- defN 80-Jan-01 00:00 smart_kit/handlers/handle_server_action.py
 -rw-r--r--  2.0 unx      997 b- defN 80-Jan-01 00:00 smart_kit/handlers/handle_take_runtime_permissions.py
 -rw-r--r--  2.0 unx      764 b- defN 80-Jan-01 00:00 smart_kit/handlers/handler_base.py
 -rw-r--r--  2.0 unx     1429 b- defN 80-Jan-01 00:00 smart_kit/handlers/handler_run_app.py
@@ -325,11 +325,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     3946 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3322 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc6.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc6.dist-info/RECORD
-333 files, 986473 bytes uncompressed, 253736 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc7.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc7.dist-info/RECORD
+333 files, 986511 bytes uncompressed, 253742 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -984,17 +984,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc6.dist-info/METADATA
+Filename: smart_app_framework-2.2.0rc7.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc6.dist-info/WHEEL
+Filename: smart_app_framework-2.2.0rc7.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc6.dist-info/RECORD
+Filename: smart_app_framework-2.2.0rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smart_kit/configs/settings.py

```diff
@@ -43,14 +43,15 @@
         """
         return repositories
 
     def _load_base_repositories(self) -> typing.List[FileRepository]:
         """Load base repositories with service settings"""
         template_settings_repo = UpdatableFileRepository(
             self.subfolder_path("template_config.yml"), loader=yaml.safe_load, key="template_settings")
+        template_settings_repo.load()
 
         use_secrets_path_for_kafka: bool = template_settings_repo.data.get("kafka_use_secrets_path", True)
         kafka_config_repo = FileRepository(
             self._get_kafka_settings_filepath("kafka_config.yml", use_secrets_path=use_secrets_path_for_kafka),
             loader=yaml.safe_load, key="kafka")
 
         ceph_config_repo = FileRepository(
```

## Comparing `smart_app_framework-2.2.0rc6.dist-info/METADATA` & `smart_app_framework-2.2.0rc7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.2.0rc6
+Version: 2.2.0rc7
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.2.0rc6.dist-info/RECORD` & `smart_app_framework-2.2.0rc7.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 smart_kit/action/http.py,sha256=IdUEoUl-pOtEuZxEF9gxHaypg5Ilk7P-lYqPsFhuueE,6670
 smart_kit/action/http_with_cookie.py,sha256=sXHgD1-5WvLUSDkSzB71UgJi-G8E_CdY9khjmeg4Fjs,1106
 smart_kit/action/smart_geo_action.py,sha256=KL3S1QIl5YbQMVx7RycpyYOsvHpLfyYYnZGG9FRvYa4,2418
 smart_kit/compatibility/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/compatibility/commands.py,sha256=xJoyXrK4p08Rl5XWkUivSnXUz2RbTZUCJQnL3IVekpw,3119
 smart_kit/configs/__init__.py,sha256=5dgcy-wMsn-gQ_SHbnshpD3YHQ4Svx0S5Y53np-syQg,4159
 smart_kit/configs/logger_config.py,sha256=NqwGPvznwfsNn7v_Xo1q_J0LTbaHUjJjhKOqYIIDYUQ,890
-smart_kit/configs/settings.py,sha256=oMu272q0dWzw1QuZaNfGHDFJCV5WQ_3z-ZAB2YB2hxo,4120
+smart_kit/configs/settings.py,sha256=iLKapGU_X6P3nOx7kzZ8ns-WjFYdr-XJOIyKiOMxO4o,4158
 smart_kit/handlers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/handlers/handle_close_app.py,sha256=3wh7LD4VkPSDaBbQvHwUXUsSj9Tjb33MpzUs-ONHb-o,1187
 smart_kit/handlers/handle_respond.py,sha256=-8mewCr--xSj_imUtmGTk926ZnNwhChPOwAE7Zspn4Y,3008
 smart_kit/handlers/handle_server_action.py,sha256=rQt2WQ4Tlc2jFgWDg_PLwmLioomhlp8oX9GNNxrMzJc,1674
 smart_kit/handlers/handle_take_runtime_permissions.py,sha256=0PTWl4uXh-ngWkZC0ZlTD0YZGsmITh39dc1vRshEb-s,997
 smart_kit/handlers/handler_base.py,sha256=vBZVsG0QDwm1qtKAAg4bWZfMdW-zo0StW7OteNrxAJ0,764
 smart_kit/handlers/handler_run_app.py,sha256=OIXTNrntk3y-W6j2huqrfasDQidtVSafH37ry1dpYtQ,1429
@@ -324,10 +324,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=UP2Zmp0VW4YZpDPe_lGQ-5L_wF5wd7J4B33kXyUINmQ,3946
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=n5N4FHjXyeZAASjVB2zhoOMsbnWiixI0OQsk4KkcDFg,3322
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.2.0rc6.dist-info/METADATA,sha256=I3KnOXkopT0MoN__oz1mMWnsWMGJ3p3S05JZQZQ8sa0,10823
-smart_app_framework-2.2.0rc6.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.2.0rc6.dist-info/RECORD,,
+smart_app_framework-2.2.0rc7.dist-info/METADATA,sha256=H4tt4BBK19TO1GfaiHbChwDsxlN3uTfukmgM5VFBL1o,10823
+smart_app_framework-2.2.0rc7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.2.0rc7.dist-info/RECORD,,
```


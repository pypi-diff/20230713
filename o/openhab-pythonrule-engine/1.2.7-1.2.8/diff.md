# Comparing `tmp/openhab_pythonrule_engine-1.2.7.tar.gz` & `tmp/openhab_pythonrule_engine-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.7.tar", last modified: Tue Jul 11 04:53:53 2023, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.8.tar", last modified: Thu Jul 13 04:18:35 2023, max compression
```

## Comparing `openhab_pythonrule_engine-1.2.7.tar` & `openhab_pythonrule_engine-1.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cron_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_change_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/loaded_rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/source_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 04:53:52.000000 openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:53:53.000000 openhab_pythonrule_engine-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-11 04:53:41.000000 openhab_pythonrule_engine-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cron_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/item_change_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/loaded_rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/source_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/setup.py
```

### Comparing `openhab_pythonrule_engine-1.2.7/PKG-INFO` & `openhab_pythonrule_engine-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab_pythonrule_engine
-Version: 1.2.7
+Version: 1.2.8
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.7/README.md` & `openhab_pythonrule_engine-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/app.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/cron_processor.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cron_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from time import sleep
 from threading import Thread
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 from openhab_pythonrule_engine.trigger import Trigger
 from openhab_pythonrule_engine.processor import Processor
 
 
+logging = logging.getLogger(__name__)
+
 class CronTrigger(Trigger):
 
     def __init__(self, expression: str, cron: str, func):
         self.cron = cron
         super().__init__(expression, func)
 
 
@@ -24,15 +26,15 @@
         return CronTriggerParser(self).on_annotation
 
     def __process(self):
         while self.is_running:
             try:
                 for cron_trigger in self.triggers:
                     if pycron.is_now(cron_trigger.cron):
-                        self.process_trigger(cron_trigger)
+                        self.invoke_trigger(cron_trigger)
             except Exception as e:
                 logging.warning("Error occurred by executing cron", e)
             sleep(60)  # minimum 60 sec!
 
     def on_start(self):
         self.thread.start()
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import sseclient
 from datetime import datetime
 from threading import Thread
 from typing import Optional
 from dataclasses import dataclass
 
-
+logging = logging.getLogger(__name__)
 
 @dataclass()
 class ItemEvent:
     item_name: str
     operation: str
     payload: str
 
@@ -46,30 +46,36 @@
         self.thread = Thread(target=self.__listen, daemon=True)
         self.thread.start()
 
     def __listen(self):
         previous_error_time = None
         while self.is_running:
             try:
-                response = requests.get(self.event_uri, stream=True)
+                conn_timeout = 30
+                read_timeout = 5 * 60
+                response = requests.get(self.event_uri, stream=True, timeout=(conn_timeout, read_timeout))
                 client = sseclient.SSEClient(response)
-                if previous_error_time is not None:
+                if previous_error_time is None:
+                    logging.info("sse stream " + self.event_uri + " established")
+                else:
                     logging.info("sse stream " + self.event_uri + " re-opened (after " + str(round((datetime.now() - previous_error_time).total_seconds()/60)) + " min)")
                 previous_error_time = None
                 try:
                     for event in client.events():
                         data = json.loads(event.data)
                         self.event_listener.on_event(data)
                 finally:
                     logging.debug("closing sse stream")
                     client.close()
                     response.close()
             except Exception as e:
+                retry_in_sec = 5
                 if previous_error_time is None:
                     logging.warning("sse stream " + self.event_uri + " disconnected: " + str(e))
+                    logging.info("try to reconnect sse stream in (each) " + str(retry_in_sec) + " sec")
                     previous_error_time = datetime.now()
-                time.sleep(5)
+                time.sleep(retry_in_sec)
 
     def stop(self):
         self.is_running = False
         Thread.join(self.thread)
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/invoke.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import inspect
 import logging
-from logging import Logger
 
 
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 
 
 
-logging = logging.getLogger(__name__)
-
-
 class Invoker():
 
     TYPE_SINGLE_PARAM_ITEMREGISTRY = "TYPE_SINGLE_PARAM_ITEMREGISTRY"
 
     def __init__(self, func, type: str):
         self.__func = func
         self.name = func.__name__
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_change_processor.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/item_change_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import logging
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 from openhab_pythonrule_engine.trigger import Trigger
 from openhab_pythonrule_engine.processor import Processor
 from openhab_pythonrule_engine.eventbus_consumer import EventConsumer, ItemEvent, parse_item_event
 
+logging = logging.getLogger(__name__)
+
+
 
 class ItemTrigger(Trigger):
 
     def __init__(self, expression: str, func):
         super().__init__(expression, func)
 
     def matches(self, item_event: ItemEvent) -> bool:
@@ -52,15 +55,15 @@
         return ItemTriggerParser(self).on_annotation
 
     def on_event(self, event):
         self.item_registry.on_event(event)
         item_event = parse_item_event(event)
         if item_event is not None:
             for item_changed_trigger in [trigger for trigger in self.triggers if trigger.matches(item_event)]:
-                self.process_trigger(item_changed_trigger)
+                self.invoke_trigger(item_changed_trigger)
 
     def on_start(self):
         self.__event_consumer.start()
 
     def on_stop(self):
         self.__event_consumer.stop()
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/item_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from dataclasses import dataclass
 from requests import Session
 from threading import RLock
 from requests.auth import HTTPBasicAuth
 from typing import Optional, List, Dict, Any
 from openhab_pythonrule_engine.cache import Cache
 
+logging = logging.getLogger(__name__)
+
 
 @dataclass
 class Item:
     item_name: str
     read_only: bool
     group_names: List[str]
     value: Any
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/loaded_rule_processor.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/loaded_rule_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from openhab_pythonrule_engine.trigger import Trigger
 from openhab_pythonrule_engine.processor import Processor
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 
 
+
 class RuleLoadedTrigger(Trigger):
 
     def __init__(self, expression: str, func):
         super().__init__(expression, func)
 
 
 class RuleLoadedProcessor(Processor):
@@ -14,15 +15,15 @@
     def __init__(self, item_registry: ItemRegistry, listener):
         super().__init__("rule loadded", item_registry, listener)
 
     def parser(self):
         return RuleLoadedTriggerParser(self).on_annotation
 
     def on_add_trigger(self, trigger: Trigger):
-        self.process_trigger(trigger)
+        self.invoke_trigger(trigger)
 
 
 class RuleLoadedTriggerParser:
 
     def __init__(self, rule_loaded_processor: RuleLoadedProcessor):
         self.rule_loaded_processor = rule_loaded_processor
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/rule_engine.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/rule_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import logging
 import os
 import sys
 import importlib
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 from openhab_pythonrule_engine.item_registry import ItemRegistry
-from openhab_pythonrule_engine.processor import Processor
+from openhab_pythonrule_engine.trigger import Trigger
 from openhab_pythonrule_engine.cron_processor import CronProcessor
 from openhab_pythonrule_engine.item_change_processor import ItemChangeProcessor
 from openhab_pythonrule_engine.loaded_rule_processor import RuleLoadedProcessor
 from openhab_pythonrule_engine.source_scanner import visit
 
+logging = logging.getLogger(__name__)
+
 
 class FileSystemListener(FileSystemEventHandler):
 
     def __init__(self, rule_engine, dir):
         self.rule_engine = rule_engine
         self.dir = dir
         logging.info("observing rules directory " + dir)
@@ -51,39 +53,34 @@
 
 
 class RuleEngine:
 
     def __init__(self, openhab_uri:str, python_rule_directory: str, user: str, pwd: str):
         self.is_running = False
         self.openhab_uri = openhab_uri
-        self.loaded_modules = dict()
-        self.last_executed = ""
-        self.last_error = ""
         self.__item_registry = ItemRegistry(openhab_uri, user, pwd)
         self.__processors = [ItemChangeProcessor(openhab_uri, self.__item_registry, self.on_executed),
                              CronProcessor(self.__item_registry, self.on_executed),
                              RuleLoadedProcessor(self.__item_registry, self.on_executed)]
         self.file_system_listener = FileSystemListener(self, python_rule_directory)
         self.listeners = set()
 
-    def on_executed(self, source: Processor, success: bool):
-        if success:
-            self.last_executed = source.last_executed
-        else:
-            self.last_executed = source.last_error
+    def triggers(self):
+        return [trigger for processor in self.__processors for trigger in processor.triggers]
+
+    def on_executed(self, trigger: Trigger, error: Exception):
         self.__notify_listener()
 
     def __del__(self):
         self.stop()
 
     def add_listener(self, listener):
         self.listeners.add(listener)
         self.__notify_listener()
 
-
     def __notify_listener(self):
         for listener in self.listeners:
             try:
                 listener()
             except Exception as e:
                 logging.warning("error occurred calling " + str(listener) + " " + str(e))
 
@@ -114,15 +111,14 @@
                     [processor.remove_triggers(modulename) for processor in self.__processors]
                     importlib.reload(sys.modules[modulename])
                     msg = "'" + filename + "' reloaded"
                 else:
                     importlib.import_module(modulename)
                     msg = "'" + filename + "' loaded for the first time"
                 num_annotations = visit(modulename, [processor.parser() for processor in self.__processors])
-                self.loaded_modules[filename] = num_annotations
                 if num_annotations > 0:
                     logging.info(msg)
                 self.__notify_listener()
             except Exception as e:
                 logging.warning("error occurred by (re)loading " + filename + " " + str(e), e)
 
     def unload_module(self, filename: str, silent: bool = False):
@@ -130,14 +126,13 @@
             try:
                 modulename = self.__filename_to_modulename(filename)
                 if modulename in sys.modules:
                     if not silent:
                         logging.info("\"unloading\" '" + filename + "'")
                     [processor.remove_triggers(modulename) for processor in self.__processors]
                     del sys.modules[modulename]
-                del self.loaded_modules[filename]
                 self.__notify_listener()
             except Exception as e:
                 logging.warning("error occurred by unloading " + filename + " " + str(e), e)
 
     def __filename_to_modulename(self, filename):
         return filename[:-3]
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/source_scanner.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/source_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import inspect
 import sys
 from typing import List
 
-
 def visit(modulename: str, visitors: List) -> int:
     num_notations = 0
     try:
         for func in inspect.getmembers(sys.modules[modulename], inspect.isfunction):
             num_notations += process_meta_data_annotation(func, visitors)
     except Exception as e:
         print(e)
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine/trigger.py` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/trigger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 import logging
 from abc import ABC
 from datetime import datetime
-from dataclasses import dataclass
-from typing import Optional
 from openhab_pythonrule_engine.invoke import Invoker
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 
-
+logging = logging.getLogger(__name__)
 
 
 class Trigger(ABC):
 
     def __init__(self, expression: str, func):
         self.expression = expression
-        self.func = func
-        self.invoker = Invoker.create(func)
-
-    def is_valid(self) -> bool:
-        return self.invoker is not None
+        self.__func = func
+        self.__invoker = Invoker.create(func)
+        self.last_executed = None
+        self.last_failed = None
 
     def invoke(self, item_registry: ItemRegistry):
-        logging.debug("executing rule " + self.invoker.name + " (triggerred by '" + self.expression + "')")
         try:
-            self.invoker.invoke(item_registry)
+            logging.debug('executing rule ' + self.module + '/' + self.function_name + '  @when("' + self.expression + '")')
+            self.__invoker.invoke(item_registry)
+            self.last_executed = datetime.now()
         except Exception as e:
-            logging.warning("Error occurred by invoking " + self.name, e)
+            logging.warning("Error occurred by executing rule " + self.function_name, e)
+            self.last_failed = datetime.now()
 
     @property
     def module(self) -> str:
-        return self.func.__module__
+        return self.__func.__module__
 
     @property
-    def name(self) -> str:
-        return self.func.__name__
+    def function_name(self) -> str:
+        return self.__func.__name__
 
     def fingerprint(self) -> str:
-        return str(self.func) + "/" + self.expression
+        return str(self.module) + "/" + str(self.function_name) + "/" + self.expression
 
     def __hash__(self):
         return hash(self.fingerprint())
 
     def __eq__(self, other):
         return self.fingerprint() == other.fingerprint()
 
     def __lt__(self, other):
         return self.fingerprint() < other.fingerprint()
 
-    def __str__(self):
-        return self.expression
-
-    def __repr__(self):
-        return self.__str__()
-
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab-pythonrule-engine
-Version: 1.2.7
+Version: 1.2.8
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.7/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.7/setup.py` & `openhab_pythonrule_engine-1.2.8/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/openhab_pythonrule_engine-1.2.8.tar.gz` & `tmp/openhab_pythonrule_engine-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.8.tar", last modified: Thu Jul 13 04:18:35 2023, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.9.tar", last modified: Thu Jul 13 16:55:49 2023, max compression
```

## Comparing `openhab_pythonrule_engine-1.2.8.tar` & `openhab_pythonrule_engine-1.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cron_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/item_change_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/loaded_rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/source_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 04:18:35.000000 openhab_pythonrule_engine-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-13 04:18:20.000000 openhab_pythonrule_engine-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/cron_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/item_change_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/loaded_rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/source_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:55:49.000000 openhab_pythonrule_engine-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-13 16:55:36.000000 openhab_pythonrule_engine-1.2.9/setup.py
```

### Comparing `openhab_pythonrule_engine-1.2.8/PKG-INFO` & `openhab_pythonrule_engine-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab_pythonrule_engine
-Version: 1.2.8
+Version: 1.2.9
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.8/README.md` & `openhab_pythonrule_engine-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/app.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/cron_processor.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/rule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,54 @@
 import logging
-import pycron
-from time import sleep
-from threading import Thread
+from abc import ABC, abstractmethod
+from datetime import datetime
+from openhab_pythonrule_engine.invoke import Invoker
 from openhab_pythonrule_engine.item_registry import ItemRegistry
-from openhab_pythonrule_engine.trigger import Trigger
-from openhab_pythonrule_engine.processor import Processor
-
 
 logging = logging.getLogger(__name__)
 
-class CronTrigger(Trigger):
 
-    def __init__(self, expression: str, cron: str, func):
-        self.cron = cron
-        super().__init__(expression, func)
+class Rule(ABC):
 
+    def __init__(self, trigger_expression: str, func):
+        self.trigger_expression = trigger_expression
+        self.__func = func
+        self.__invoker = Invoker.create(func)
+        self.last_executed = None
+        self.last_failed = None
 
-class CronProcessor(Processor):
+    def invoke(self, item_registry: ItemRegistry):
+        try:
+            logging.debug('executing ' + self.module + '.py#' + self.function_name + '(...) on @when("' + self.trigger_expression + '")')
+            self.__invoker.invoke(item_registry)
+            self.last_executed = datetime.now()
+        except Exception as e:
+            logging.warning("Error occurred by executing rule " + self.function_name, e)
+            self.last_failed = datetime.now()
 
-    def __init__(self, item_registry: ItemRegistry, listener):
-        self.thread = Thread(target=self.__process, daemon=True)
-        super().__init__("cron", item_registry, listener)
+    @property
+    def module(self) -> str:
+        return self.__func.__module__
 
-    def parser(self):
-        return CronTriggerParser(self).on_annotation
+    @property
+    def function_name(self) -> str:
+        return self.__func.__name__
 
-    def __process(self):
-        while self.is_running:
-            try:
-                for cron_trigger in self.triggers:
-                    if pycron.is_now(cron_trigger.cron):
-                        self.invoke_trigger(cron_trigger)
-            except Exception as e:
-                logging.warning("Error occurred by executing cron", e)
-            sleep(60)  # minimum 60 sec!
+    def fingerprint(self) -> str:
+        return str(self.module) + "/" + str(self.function_name) + "/" + self.trigger_expression
 
-    def on_start(self):
-        self.thread.start()
+    def __hash__(self):
+        return hash(self.fingerprint())
 
-    def on_stop(self):
-        Thread.join(self.thread)
+    def __eq__(self, other):
+        return self.fingerprint() == other.fingerprint()
 
+    def __lt__(self, other):
+        return self.fingerprint() < other.fingerprint()
 
-class CronTriggerParser:
 
-    def __init__(self, cron_processor: CronProcessor):
-        self.cron_processor = cron_processor
 
-    def is_vaild_cron(self, cron: str) -> bool:
-        try:
-            pycron.is_now(cron)
-            return True
-        except Exception as e:
-            return False
+class ExecutionListener(ABC):
 
-    def on_annotation(self, annotation: str, func) -> bool:
-        if annotation.lower().startswith("time cron"):
-            cron = annotation[len("time cron"):].strip()
-            if self.is_vaild_cron(cron):
-                self.cron_processor.add_trigger(CronTrigger(annotation, cron, func))
-                return True
-            else:
-                logging.warning("cron " + cron + " is invalid (syntax error?)")
-        return False
+    @abstractmethod
+    def on_executed(self, rule: Rule, error: Exception):
+        pass
```

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,25 +57,27 @@
                 if previous_error_time is None:
                     logging.info("sse stream " + self.event_uri + " established")
                 else:
                     logging.info("sse stream " + self.event_uri + " re-opened (after " + str(round((datetime.now() - previous_error_time).total_seconds()/60)) + " min)")
                 previous_error_time = None
                 try:
                     for event in client.events():
-                        data = json.loads(event.data)
-                        self.event_listener.on_event(data)
+                        if self.is_running:
+                            data = json.loads(event.data)
+                            self.event_listener.on_event(data)
+                        else:
+                            break
                 finally:
                     logging.debug("closing sse stream")
                     client.close()
                     response.close()
             except Exception as e:
                 retry_in_sec = 5
                 if previous_error_time is None:
-                    logging.warning("sse stream " + self.event_uri + " disconnected: " + str(e))
+                    logging.warning("sse stream " + self.event_uri + " failed: " + str(e))
                     logging.info("try to reconnect sse stream in (each) " + str(retry_in_sec) + " sec")
                     previous_error_time = datetime.now()
                 time.sleep(retry_in_sec)
 
     def stop(self):
         self.is_running = False
-        Thread.join(self.thread)
```

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/invoke.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/item_registry.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/loaded_rule_processor.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/loaded_rule_processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from openhab_pythonrule_engine.trigger import Trigger
+import weakref
+from openhab_pythonrule_engine.rule import Rule
 from openhab_pythonrule_engine.processor import Processor
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 
 
 
-class RuleLoadedTrigger(Trigger):
+class RuleLoadedRule(Rule):
 
-    def __init__(self, expression: str, func):
-        super().__init__(expression, func)
+    def __init__(self, trigger_expression: str, func):
+        super().__init__(trigger_expression, func)
 
 
 class RuleLoadedProcessor(Processor):
 
-    def __init__(self, item_registry: ItemRegistry, listener):
-        super().__init__("rule loadded", item_registry, listener)
+    def __init__(self, item_registry: ItemRegistry, execution_listener_ref: weakref):
+        super().__init__("rule loaded", item_registry, execution_listener_ref)
 
     def parser(self):
         return RuleLoadedTriggerParser(self).on_annotation
 
-    def on_add_trigger(self, trigger: Trigger):
-        self.invoke_trigger(trigger)
+    def on_add_rule(self, rule: Rule):
+        self.invoke_rule(rule)
 
 
 class RuleLoadedTriggerParser:
 
     def __init__(self, rule_loaded_processor: RuleLoadedProcessor):
         self.rule_loaded_processor = rule_loaded_processor
 
     def on_annotation(self, annotation: str, func):
         if annotation.lower().strip() == "rule loaded":
-            self.rule_loaded_processor.add_trigger(RuleLoadedTrigger(annotation, func))
+            self.rule_loaded_processor.add_rule(RuleLoadedRule(annotation, func))
             return True
         return False
```

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/rule_engine.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/rule_engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,133 @@
 import logging
 import os
 import sys
 import importlib
+import weakref
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 from openhab_pythonrule_engine.item_registry import ItemRegistry
-from openhab_pythonrule_engine.trigger import Trigger
+from openhab_pythonrule_engine.rule import Rule, ExecutionListener
 from openhab_pythonrule_engine.cron_processor import CronProcessor
 from openhab_pythonrule_engine.item_change_processor import ItemChangeProcessor
 from openhab_pythonrule_engine.loaded_rule_processor import RuleLoadedProcessor
 from openhab_pythonrule_engine.source_scanner import visit
 
 logging = logging.getLogger(__name__)
 
 
 class FileSystemListener(FileSystemEventHandler):
 
-    def __init__(self, rule_engine, dir):
-        self.rule_engine = rule_engine
+    def __init__(self, rule_engine_ref: weakref, dir):
+        self.rule_engine_ref = rule_engine_ref
         self.dir = dir
-        logging.info("observing rules directory " + dir)
         self.observer = Observer()
 
+    def __unload_module(self, path: str):
+        rule_engine = self.rule_engine_ref()
+        if rule_engine is not None:
+            rule_engine.unload_module(path)
+
+    def __load_module(self, path: str):
+        rule_engine = self.rule_engine_ref()
+        if rule_engine is not None:
+            rule_engine.load_module(path)
+
     def start(self):
+        logging.info("observing rules directory '" + self.dir + "' started")
         for file in os.scandir(self.dir):
-            self.rule_engine.load_module(file.name)
+            self.__load_module(file.name)
         self.observer.schedule(self, self.dir, recursive=False)
         self.observer.start()
 
     def stop(self):
         self.observer.stop()
-        for file in os.scandir(dir):
-            self.rule_engine.unload_module(file.name)
+        logging.info("observing rules directory '" + self.dir + "' stopped")
 
     def on_moved(self, event):
-        self.rule_engine.unload_module(self.filename(event.src_path))
-        self.rule_engine.load_module(self.filename(event.dest_path))
+        self.__unload_module(self.filename(event.src_path))
+        self.__load_module(self.filename(event.dest_path))
 
     def on_deleted(self, event):
-        self.rule_engine.unload_module(self.filename(event.src_path))
+        self.__unload_module(self.filename(event.src_path))
 
     def on_created(self, event):
-        self.rule_engine.load_module(self.filename(event.src_path))
+        self.__load_module(self.filename(event.src_path))
 
     def on_modified(self, event):
-        self.rule_engine.load_module(self.filename(event.src_path))
+        self.__load_module(self.filename(event.src_path))
 
     def filename(self, path):
         path = path.replace("\\", "/")
         return path[path.rindex("/")+1:]
 
 
-
-class RuleEngine:
+class RuleEngine(ExecutionListener):
 
     def __init__(self, openhab_uri:str, python_rule_directory: str, user: str, pwd: str):
         self.is_running = False
         self.openhab_uri = openhab_uri
         self.__item_registry = ItemRegistry(openhab_uri, user, pwd)
-        self.__processors = [ItemChangeProcessor(openhab_uri, self.__item_registry, self.on_executed),
-                             CronProcessor(self.__item_registry, self.on_executed),
-                             RuleLoadedProcessor(self.__item_registry, self.on_executed)]
-        self.file_system_listener = FileSystemListener(self, python_rule_directory)
+        self.__processors = [ItemChangeProcessor(openhab_uri, self.__item_registry, weakref.ref(self)),
+                             CronProcessor(self.__item_registry, weakref.ref(self)),
+                             RuleLoadedProcessor(self.__item_registry, weakref.ref(self))]
+        self.file_system_listener = FileSystemListener(weakref.ref(self), python_rule_directory)
         self.listeners = set()
 
-    def triggers(self):
-        return [trigger for processor in self.__processors for trigger in processor.triggers]
+    def rules(self):
+        return [rule for processor in self.__processors for rule in processor.rules]
 
-    def on_executed(self, trigger: Trigger, error: Exception):
+    def on_executed(self, rule: Rule, error: Exception):
         self.__notify_listener()
 
-    def __del__(self):
-        self.stop()
-
     def add_listener(self, listener):
         self.listeners.add(listener)
         self.__notify_listener()
 
     def __notify_listener(self):
         for listener in self.listeners:
             try:
                 listener()
             except Exception as e:
                 logging.warning("error occurred calling " + str(listener) + " " + str(e))
 
     def start(self):
         if not self.is_running:
+            logging.info("starting rule engine...")
             self.is_running = True
             if self.python_rule_directory not in sys.path:
                 sys.path.insert(0, self.python_rule_directory)
             [processor.start() for processor in self.__processors]
             self.file_system_listener.start()
+            logging.info("rule engine started")
+
+    def __del__(self):
+        self.stop()
 
     def stop(self):
+        logging.info("stopping rule engine...")
         self.is_running = False
         self.file_system_listener.stop()
         [processor.stop() for processor in self.__processors]
+        for module in {rule.module for rule in self.rules()}:
+            self.unload_module(module + ".py")
+        logging.info("rule engine stopped")
 
     @property
     def python_rule_directory(self):
         return self.file_system_listener.dir
 
     def load_module(self, filename: str):
         if filename.endswith(".py"):
             try:
                 modulename = self.__filename_to_modulename(filename)
                 msg = None
                 # reload?
                 if modulename in sys.modules:
-                    [processor.remove_triggers(modulename) for processor in self.__processors]
+                    [processor.remove_rules(modulename) for processor in self.__processors]
                     importlib.reload(sys.modules[modulename])
                     msg = "'" + filename + "' reloaded"
                 else:
                     importlib.import_module(modulename)
                     msg = "'" + filename + "' loaded for the first time"
                 num_annotations = visit(modulename, [processor.parser() for processor in self.__processors])
                 if num_annotations > 0:
@@ -122,17 +137,17 @@
                 logging.warning("error occurred by (re)loading " + filename + " " + str(e), e)
 
     def unload_module(self, filename: str, silent: bool = False):
         if filename.endswith(".py"):
             try:
                 modulename = self.__filename_to_modulename(filename)
                 if modulename in sys.modules:
-                    if not silent:
-                        logging.info("\"unloading\" '" + filename + "'")
-                    [processor.remove_triggers(modulename) for processor in self.__processors]
+                    [processor.remove_rules(modulename) for processor in self.__processors]
                     del sys.modules[modulename]
+                    if not silent:
+                        logging.info("'" + filename + "' unloaded")
                 self.__notify_listener()
             except Exception as e:
                 logging.warning("error occurred by unloading " + filename + " " + str(e), e)
 
     def __filename_to_modulename(self, filename):
         return filename[:-3]
```

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/rule_engine_webthing.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/rule_engine_webthing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import tornado.ioloop
 import logging
 from webthing import (Value, Property, Thing, SingleThing, WebThingServer)
-from datetime import datetime
 from typing import List
 from openhab_pythonrule_engine.rule_engine import RuleEngine
-from openhab_pythonrule_engine.trigger import Trigger
+
+
+logging = logging.getLogger(__name__)
 
 
 class RuleEngineThing(Thing):
 
     def __init__(self, description: str, rule_engine: RuleEngine):
         Thing.__init__(
             self,
@@ -72,40 +73,40 @@
         self.rule_engine.add_listener(self.on_update)
 
     def on_update(self):
         self.ioloop.add_callback(self.__handle)
 
     def __print_module_info(self) -> List[str]:
         func_info = {}
-        for trigger in self.rule_engine.triggers():
-            key = trigger.module + "#" + trigger.function_name
+        for rule in self.rule_engine.rules():
+            key = rule.module + "#" + rule.function_name
             expressions = func_info.get(key, set())
-            expressions.add(trigger.expression)
+            expressions.add(rule.expression)
             func_info[key] = expressions
         sorted_keys = sorted(list(func_info.keys()))
         return [key + " (" + ", ".join(func_info[key]) + ")" for key in sorted_keys]
 
     def __print_last_executed(self) -> List[str]:
         func_info = {}
-        for trigger in self.rule_engine.triggers():
-            if trigger.last_executed is not None:
-                key = trigger.module + "#" + trigger.function_name
+        for rule in self.rule_engine.rules():
+            if rule.last_executed is not None:
+                key = rule.module + "#" + rule.function_name
                 execution_times = func_info.get(key, [])
-                execution_times.append(trigger.last_executed)
+                execution_times.append(rule.last_executed)
                 func_info[key] = execution_times
         sorted_keys = sorted(list(func_info.keys()))
         return [key + " (" + sorted(func_info[key])[-1].strftime("%H:%M:%S") + ")" for key in sorted_keys]
 
     def __print_last_failed(self) -> List[str]:
         func_info = {}
-        for trigger in self.rule_engine.triggers():
-            if trigger.last_failed is not None:
-                key = trigger.module + "#" + trigger.function_name
+        for rule in self.rule_engine.rules():
+            if rule.last_failed is not None:
+                key = rule.module + "#" + rule.function_name
                 execution_times = func_info.get(key, [])
-                execution_times.append(trigger.last_failed)
+                execution_times.append(rule.last_failed)
                 func_info[key] = execution_times
         sorted_keys = sorted(list(func_info.keys()))
         return [key + " (" + sorted(func_info[key])[-1].strftime("%H:%M:%S") + ")" for key in sorted_keys]
 
     def __handle(self):
         self.last_executed.notify_of_external_update(", ".join(self.__print_last_executed()))
         self.last_failed.notify_of_external_update(", ".join(self.__print_last_failed()))
```

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/source_scanner.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/source_scanner.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine/trigger.py` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine/processor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,69 @@
 import logging
+import weakref
 from abc import ABC
-from datetime import datetime
-from openhab_pythonrule_engine.invoke import Invoker
+from openhab_pythonrule_engine.rule import Rule
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 
 logging = logging.getLogger(__name__)
 
 
-class Trigger(ABC):
+class Processor(ABC):
 
-    def __init__(self, expression: str, func):
-        self.expression = expression
-        self.__func = func
-        self.__invoker = Invoker.create(func)
-        self.last_executed = None
-        self.last_failed = None
+    def __init__(self, name: str, item_registry: ItemRegistry, execution_listener_ref: weakref):
+        self.name = name
+        self.item_registry = item_registry
+        self.is_running = False
+        self.rules = set()
+        self.execution_listener_ref = execution_listener_ref
 
-    def invoke(self, item_registry: ItemRegistry):
+    def __notify_listener(self, rule: Rule, error: Exception = None):
         try:
-            logging.debug('executing rule ' + self.module + '/' + self.function_name + '  @when("' + self.expression + '")')
-            self.__invoker.invoke(item_registry)
-            self.last_executed = datetime.now()
+            execution_listener = self.execution_listener_ref()
+            if execution_listener is not None:
+                execution_listener.on_executed(rule, error)
         except Exception as e:
-            logging.warning("Error occurred by executing rule " + self.function_name, e)
-            self.last_failed = datetime.now()
+            logging.warning("error occurred calling " + self.execution_listener_ref() + " " + str(e))
 
-    @property
-    def module(self) -> str:
-        return self.__func.__module__
+    def add_rule(self, rule: Rule):
+        logging.info(' * register ' + rule.module + '.py#' + rule.function_name + '(...) on @when("' + rule.trigger_expression + '")')
+        self.rules.add(rule)
+        self.on_add_rule(rule)
+
+    def remove_rules(self, module: str):
+        rules_of_module = {rule for rule in self.rules if rule.module == module}
+        for rule in rules_of_module:
+            logging.info(' * unregister ' + rule.module + '.py#' + rule.function_name + '(...) on @when("' + rule.trigger_expression + '")')
+        self.rules = self.rules - rules_of_module
+        self.on_remove_rules(module)
 
-    @property
-    def function_name(self) -> str:
-        return self.__func.__name__
-
-    def fingerprint(self) -> str:
-        return str(self.module) + "/" + str(self.function_name) + "/" + self.expression
-
-    def __hash__(self):
-        return hash(self.fingerprint())
+    def invoke_rule(self, rule: Rule):
+        try:
+            rule.invoke(self.item_registry)
+            self.__notify_listener(rule)
+        except Exception as e:
+            logging.warning("Error occurred by executing rule " + rule.function_name, e)
+            self.__notify_listener(rule, e)
 
-    def __eq__(self, other):
-        return self.fingerprint() == other.fingerprint()
+    def start(self):
+        if not self.is_running:
+            self.is_running = True
+            self.on_start()
+            logging.info("'" + self.name + " processor' started")
+
+    def on_start(self):
+        pass
+
+    def stop(self):
+        self.is_running = False
+        self.on_stop()
+        logging.info("'" + self.name + "' processor stopped")
 
-    def __lt__(self, other):
-        return self.fingerprint() < other.fingerprint()
+    def on_stop(self):
+        pass
 
+    def on_add_rule(self, rule: Rule):
+        pass
 
+    def on_remove_rules(self, module: str):
+        pass
```

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab-pythonrule-engine
-Version: 1.2.8
+Version: 1.2.9
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.8/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.2.9/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 openhab_pythonrule_engine/cron_processor.py
 openhab_pythonrule_engine/eventbus_consumer.py
 openhab_pythonrule_engine/invoke.py
 openhab_pythonrule_engine/item_change_processor.py
 openhab_pythonrule_engine/item_registry.py
 openhab_pythonrule_engine/loaded_rule_processor.py
 openhab_pythonrule_engine/processor.py
+openhab_pythonrule_engine/rule.py
 openhab_pythonrule_engine/rule_engine.py
 openhab_pythonrule_engine/rule_engine_webthing.py
 openhab_pythonrule_engine/source_scanner.py
-openhab_pythonrule_engine/trigger.py
 openhab_pythonrule_engine.egg-info/PKG-INFO
 openhab_pythonrule_engine.egg-info/SOURCES.txt
 openhab_pythonrule_engine.egg-info/dependency_links.txt
 openhab_pythonrule_engine.egg-info/entry_points.txt
 openhab_pythonrule_engine.egg-info/requires.txt
 openhab_pythonrule_engine.egg-info/top_level.txt
```

### Comparing `openhab_pythonrule_engine-1.2.8/setup.py` & `openhab_pythonrule_engine-1.2.9/setup.py`

 * *Files identical despite different names*


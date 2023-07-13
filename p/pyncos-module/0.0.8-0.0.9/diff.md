# Comparing `tmp/pyncos-module-0.0.8.tar.gz` & `tmp/pyncos-module-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncos-module-0.0.8.tar", last modified: Wed Jul 12 16:23:34 2023, max compression
+gzip compressed data, was "pyncos-module-0.0.9.tar", last modified: Wed Jul 12 16:26:56 2023, max compression
```

## Comparing `pyncos-module-0.0.8.tar` & `pyncos-module-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:23:34.046602 pyncos-module-0.0.8/
--rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      423 2023-07-12 16:23:34.046602 pyncos-module-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 16:23:34.034083 pyncos-module-0.0.8/ncos/
--rw-rw-rw-   0        0        0       23 2023-07-12 16:12:11.000000 pyncos-module-0.0.8/ncos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:23:34.035082 pyncos-module-0.0.8/ncos/commons/
--rw-rw-rw-   0        0        0      698 2023-07-12 16:20:56.000000 pyncos-module-0.0.8/ncos/commons/__init__.py
--rw-rw-rw-   0        0        0     5864 2023-07-12 16:23:25.000000 pyncos-module-0.0.8/ncos/module.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:23:34.037083 pyncos-module-0.0.8/ncos/networks/
--rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.8/ncos/networks/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-07-12 16:11:50.000000 pyncos-module-0.0.8/ncos/networks/mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:23:34.039596 pyncos-module-0.0.8/ncos/utils/
--rw-rw-rw-   0        0        0      406 2023-07-12 16:11:58.000000 pyncos-module-0.0.8/ncos/utils/__init__.py
--rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.8/ncos/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:23:34.044602 pyncos-module-0.0.8/pyncos_module.egg-info/
--rw-rw-rw-   0        0        0      423 2023-07-12 16:23:33.000000 pyncos-module-0.0.8/pyncos_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-07-12 16:23:33.000000 pyncos-module-0.0.8/pyncos_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:23:33.000000 pyncos-module-0.0.8/pyncos_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 16:23:33.000000 pyncos-module-0.0.8/pyncos_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 16:23:34.046602 pyncos-module-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-07-12 16:23:32.000000 pyncos-module-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:26:56.498132 pyncos-module-0.0.9/
+-rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      423 2023-07-12 16:26:56.498132 pyncos-module-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:26:56.485039 pyncos-module-0.0.9/ncos/
+-rw-rw-rw-   0        0        0       23 2023-07-12 16:12:11.000000 pyncos-module-0.0.9/ncos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:26:56.487040 pyncos-module-0.0.9/ncos/commons/
+-rw-rw-rw-   0        0        0      698 2023-07-12 16:20:56.000000 pyncos-module-0.0.9/ncos/commons/__init__.py
+-rw-rw-rw-   0        0        0     5892 2023-07-12 16:26:19.000000 pyncos-module-0.0.9/ncos/module.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:26:56.489125 pyncos-module-0.0.9/ncos/networks/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.9/ncos/networks/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-07-12 16:11:50.000000 pyncos-module-0.0.9/ncos/networks/mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:26:56.491131 pyncos-module-0.0.9/ncos/utils/
+-rw-rw-rw-   0        0        0      406 2023-07-12 16:11:58.000000 pyncos-module-0.0.9/ncos/utils/__init__.py
+-rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.9/ncos/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:26:56.496131 pyncos-module-0.0.9/pyncos_module.egg-info/
+-rw-rw-rw-   0        0        0      423 2023-07-12 16:26:56.000000 pyncos-module-0.0.9/pyncos_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-12 16:26:56.000000 pyncos-module-0.0.9/pyncos_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:26:56.000000 pyncos-module-0.0.9/pyncos_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 16:26:56.000000 pyncos-module-0.0.9/pyncos_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:26:56.498132 pyncos-module-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-07-12 16:26:50.000000 pyncos-module-0.0.9/setup.py
```

### Comparing `pyncos-module-0.0.8/LICENSE.txt` & `pyncos-module-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.8/ncos/commons/__init__.py` & `pyncos-module-0.0.9/ncos/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.8/ncos/module.py` & `pyncos-module-0.0.9/ncos/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,27 +31,28 @@
       self.__topic__(MODULES_INSTALL_PUSH_TOPIC):           self.on_installed,
       self.__topic__(MODULES_DATA_PULL_TOPIC):              self.on_data_pull,
       self.__topic__(MODULES_CONFIG_TOPIC):                 self.on_config,
       self.__topic__(MODULES_ACTION_TOPIC):                 self.on_action
     }
 
   
-  def install(self):
+  def __install__(self):
     self.handle_post_install()
     self.broker.publish(
       'NCOS/modules/install', 
       dumps({'slot': self.__slot_name__, 'moduleId': self.id, 'moduleName': self.__module_name__}))
 
   def on_installed(self, topic, payload:dict):
     _success = payload['success'] if 'success' in payload else False
     _error = payload['error'] if 'error' in payload else ''
     self.handle_installed(_success, _error)
     
     
   def on_NCOS_ready(self, topic, payload:dict):
+    self.__install__()
     self.handle_NCOS_ready(payload)
   
   
   def on_data_pull(self, topic, payload:dict):
     self.handle_data_pull(payload)
```

### Comparing `pyncos-module-0.0.8/ncos/networks/mqtt.py` & `pyncos-module-0.0.9/ncos/networks/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.8/ncos/utils/logger.py` & `pyncos-module-0.0.9/ncos/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.8/setup.py` & `pyncos-module-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pyncos-module", 
-    version="0.0.8",   
+    version="0.0.9",   
     author="xuwh",  
     author_email="xuwhdev@gmail.com", 
     description="", 
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://gitee.com/zwsjz/carbot-module-lib", 
     packages=setuptools.find_packages(),
```


# Comparing `tmp/Akatosh-2.1.2.tar.gz` & `tmp/Akatosh-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.2.tar", last modified: Wed Jul 12 07:58:50 2023, max compression
+gzip compressed data, was "Akatosh-2.1.3.tar", last modified: Thu Jul 13 06:20:03 2023, max compression
```

## Comparing `Akatosh-2.1.2.tar` & `Akatosh-2.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 07:58:50.888119 Akatosh-2.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-12 07:58:50.824120 Akatosh-2.1.2/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.2/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    12961 2023-07-12 07:56:31.000000 Akatosh-2.1.2/Akatosh/entity.py
--rw-rw-rw-   0        0        0    13327 2023-07-12 07:37:05.000000 Akatosh-2.1.2/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.2/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-12 04:33:32.000000 Akatosh-2.1.2/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.2/Akatosh/states.py
--rw-rw-rw-   0        0        0     5356 2023-07-12 07:48:11.000000 Akatosh-2.1.2/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:58:50.877124 Akatosh-2.1.2/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 07:58:50.000000 Akatosh-2.1.2/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-12 07:58:50.885120 Akatosh-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.2/README.md
--rw-rw-rw-   0        0        0      635 2023-07-12 07:20:32.000000 Akatosh-2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 07:58:50.891145 Akatosh-2.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 06:20:03.243374 Akatosh-2.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-13 06:20:03.229376 Akatosh-2.1.3/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-13 05:05:39.000000 Akatosh-2.1.3/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    13438 2023-07-13 06:17:06.000000 Akatosh-2.1.3/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    13327 2023-07-13 05:05:39.000000 Akatosh-2.1.3/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-11 12:42:40.000000 Akatosh-2.1.3/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-11 12:42:40.000000 Akatosh-2.1.3/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-11 12:42:40.000000 Akatosh-2.1.3/Akatosh/states.py
+-rw-rw-rw-   0        0        0     5356 2023-07-13 05:05:39.000000 Akatosh-2.1.3/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:20:03.239376 Akatosh-2.1.3/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-13 06:20:03.241376 Akatosh-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-11 12:42:40.000000 Akatosh-2.1.3/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-13 06:18:52.000000 Akatosh-2.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 06:20:03.243374 Akatosh-2.1.3/setup.cfg
```

### Comparing `Akatosh-2.1.2/Akatosh/entity.py` & `Akatosh-2.1.3/Akatosh/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         for res in self.ocupied_resources:
             res.collect(self)
 
     def unregister_from_lists(self):
         """Remove this entity from all registered entity lists."""
         for list in self.registered_lists[:]:
             list.remove(self)
-            
+
     def cancel_unfinished_events(self):
         """Cancel all unfinished events."""
         for event in self.events:
             if not event.ended:
                 event.cancel()
 
     def continuous_event(
@@ -260,15 +260,15 @@
     @property
     def events(self):
         """Return the events engaged by the entity."""
         return self._events
 
 
 class EntityList(list):
-    """Customized list for entities."""
+    """Customized list for entities. This list ensures all items are entities and unique. When an entity is terminated, it will be removed from all entity lists automatically."""
 
     def __init__(self, iterable: Iterable[Entity] = [], label: str | None = None):
         """Create a list for entities, with optional label.
 
         Args:
             iterable (Iterable[Entity]): Iterable of entities.
         """
@@ -278,31 +278,35 @@
     def insert(self, __index: int, __object: Entity) -> None:
         """Insert an entity to the list.
 
         Args:
             __index (SupportsIndex): the index to insert the entity.
             __object (Entity): the entity to be inserted.
         """
-        super().insert(__index, __object)
-        __object.registered_lists.append(self)
-        logger.debug(
-            f"Entity {__object.label} is inserted to {self.label if self.label else self} at {__index}."
-        )
+        if __object not in self:
+            super().insert(__index, __object)
+            if self not in __object.registered_lists:
+                __object.registered_lists.append(self)
+            logger.debug(
+                f"Entity {__object.label} is inserted to {self.label if self.label else self} at {__index}."
+            )
 
     def append(self, __object: Entity) -> None:
         """Append an entity to the list.
 
         Args:
             __object (Entity): the entity to be appended.
         """
-        super().append(__object)
-        __object.registered_lists.append(self)
-        logger.debug(
-            f"Entity {__object.label} is appended to {self.label if self.label else self}."
-        )
+        if __object not in self:
+            super().append(__object)
+            if self not in __object.registered_lists:
+                __object.registered_lists.append(self)
+            logger.debug(
+                f"Entity {__object.label} is appended to {self.label if self.label else self}."
+            )
 
     def remove(self, __object: Entity) -> None:
         """Remove an entity from the list.
 
         Args:
             __object (Entity): the entity to be removed.
         """
@@ -337,17 +341,20 @@
 
     def extend(self, __iterable: Iterable[Entity]) -> None:
         """Extend the list with an iterable of entities.
 
         Args:
             __iterable (Iterable[Entity]): the iterable of entities.
         """
-        super().extend(__iterable)
         for item in __iterable:
-            item.registered_lists.append(self)
+            if item not in self:
+                super().append(item)
+        for item in __iterable:
+            if self not in item.registered_lists:
+                item.registered_lists.append(self)
         logger.debug(
             f"{self.label if self.label else self} is extended with {__iterable}."
         )
 
     @property
     def label(self):
         """Return the label of the entity list."""
```

### Comparing `Akatosh-2.1.2/Akatosh/event.py` & `Akatosh-2.1.3/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.2/Akatosh/resource.py` & `Akatosh-2.1.3/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.2/Akatosh/universe.py` & `Akatosh-2.1.3/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.2/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.3/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.2
+Version: 2.1.3
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.2/PKG-INFO` & `Akatosh-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.2
+Version: 2.1.3
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.2/README.md` & `Akatosh-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.2/pyproject.toml` & `Akatosh-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.2"
+version = "2.1.3"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```


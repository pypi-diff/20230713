# Comparing `tmp/tcod_ecs-3.2.0.tar.gz` & `tmp/tcod_ecs-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-3.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-3.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-3.2.0.tar` & `tcod_ecs-3.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-07-03 03:27:18.545176 tcod_ecs-3.2.0/LICENSE
--rw-r--r--   0        0        0     8461 2023-07-03 03:27:18.545176 tcod_ecs-3.2.0/README.md
--rw-r--r--   0        0        0     3478 2023-07-03 03:27:18.549176 tcod_ecs-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    38097 2023-07-03 03:27:18.549176 tcod_ecs-3.2.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0      160 2023-07-03 03:27:26.565305 tcod_ecs-3.2.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0        0 2023-07-03 03:27:18.549176 tcod_ecs-3.2.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0     9656 1970-01-01 00:00:00.000000 tcod_ecs-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/LICENSE
+-rw-r--r--   0        0        0     8461 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/README.md
+-rw-r--r--   0        0        0     3500 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    38965 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-13 05:18:50.947566 tcod_ecs-3.3.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     9656 1970-01-01 00:00:00.000000 tcod_ecs-3.3.0/PKG-INFO
```

### Comparing `tcod_ecs-3.2.0/LICENSE` & `tcod_ecs-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.2.0/README.md` & `tcod_ecs-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.2.0/pyproject.toml` & `tcod_ecs-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 required_plugins = ["pytest-cov>=4.0.0", "pytest-benchmark>=4.0.0"]
 addopts = "--doctest-modules --cov=tcod --cov-report=term-missing --doctest-glob=*.md --benchmark-disable"
 testpaths = ["."]
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html
-exclude_lines = ['^\s*\.\.\.', "if TYPE_CHECKING:"]
+exclude_lines = ['^\s*\.\.\.', "if TYPE_CHECKING:", "# pragma: no cover"]
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules/
 select = [
     "C90", # mccabe
     "E",   # pycodestyle
     "W",   # pycodestyle
```

### Comparing `tcod_ecs-3.2.0/tcod/ecs/__init__.py` & `tcod_ecs-3.3.0/tcod/ecs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 from typing_extensions import Self
 
 from tcod.ecs import _version
 
 __version__ = _version.__version__
 
-if sys.version_info >= (3, 10):
+if sys.version_info >= (3, 10):  # pragma: no cover
     from types import EllipsisType
-else:
+else:  # pragma: no cover
     EllipsisType = Any
 
 T = TypeVar("T")
 _T1 = TypeVar("_T1")
 _T2 = TypeVar("_T2")
 _T3 = TypeVar("_T3")
 _T4 = TypeVar("_T4")
@@ -150,17 +150,27 @@
 
             >>> entity.tags.add("tag") # Add tag.
             >>> "tag" in entity.tags  # Check tag.
             True
             >>> list(world.Q.all_of(tags=["tag"]))  # Query tags.
             [<Entity(uid='entity')>]
             >>> entity.tags.discard("tag")
+            >>> entity.tags |= {"IsPortable", "CanBurn", "OnFire"}  # Supports in-place syntax
+            >>> {"CanBurn", "OnFire"}.issubset(entity.tags)
+            True
+            >>> entity.tags -= {"OnFire"}
+            >>> {"CanBurn", "OnFire"}.issubset(entity.tags)
+            False
         """
         return EntityTags(self)
 
+    @tags.setter
+    def tags(self, value: EntityTags) -> None:
+        assert value.entity is self
+
     @property
     def relation_components(self) -> EntityComponentRelations:
         """Access an entities relation components.
 
         Example::
 
             >>> entity.relation_components[str][other_entity] = "foo" # Assign component to relation.
@@ -425,14 +435,32 @@
         """Iterate over this entities tags."""
         return iter(self.entity.world._tags_by_entity.get(self.entity, ()))
 
     def __len__(self) -> int:
         """Return the number of tags this entity has."""
         return len(self.entity.world._tags_by_entity.get(self.entity, ()))
 
+    def __ior__(self, other: AbstractSet[object]) -> Self:
+        """Add tags in-place.
+
+        .. versionadded:: 3.3
+        """
+        for to_add in other:
+            self.add(to_add)
+        return self
+
+    def __isub__(self, other: AbstractSet[Any]) -> Self:
+        """Remove tags in-place.
+
+        .. versionadded:: 3.3
+        """
+        for to_discard in other:
+            self.discard(to_discard)
+        return self
+
 
 class EntityRelationsMapping(MutableSet[Entity]):
     """A proxy attribute to access entity relation targets like a set.
 
     See :any:`Entity.relation_tags_many`.
     """
```

### Comparing `tcod_ecs-3.2.0/PKG-INFO` & `tcod_ecs-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 3.2.0
+Version: 3.3.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


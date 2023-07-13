# Comparing `tmp/tcod_ecs-3.3.0.tar.gz` & `tmp/tcod_ecs-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-3.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-3.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-3.3.0.tar` & `tcod_ecs-3.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/LICENSE
--rw-r--r--   0        0        0     8461 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/README.md
--rw-r--r--   0        0        0     3500 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/pyproject.toml
--rw-r--r--   0        0        0    38965 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0      160 2023-07-13 05:18:50.947566 tcod_ecs-3.3.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0        0 2023-07-13 05:18:43.175369 tcod_ecs-3.3.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0     9656 1970-01-01 00:00:00.000000 tcod_ecs-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-13 06:01:45.198624 tcod_ecs-3.4.0/LICENSE
+-rw-r--r--   0        0        0     8409 2023-07-13 06:01:45.198624 tcod_ecs-3.4.0/README.md
+-rw-r--r--   0        0        0     3499 2023-07-13 06:01:45.198624 tcod_ecs-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0    39512 2023-07-13 06:01:45.198624 tcod_ecs-3.4.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-13 06:01:52.738556 tcod_ecs-3.4.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0        0 2023-07-13 06:01:45.198624 tcod_ecs-3.4.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     9604 1970-01-01 00:00:00.000000 tcod_ecs-3.4.0/PKG-INFO
```

### Comparing `tcod_ecs-3.3.0/LICENSE` & `tcod_ecs-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.3.0/README.md` & `tcod_ecs-3.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 # Examples
 
 ## World
 
 ```py
 >>> import tcod.ecs
->>> world = tcod.ecs.World()  # New empty world.
+>>> world = tcod.ecs.World()  # New empty world
 
 ```
 
 ## Entity
 
 Each Entity is identified by its unique id (`uid`) which can be any hashable object and the `world` it belongs to.
 New unique entities can be created with `World.new_entity` which uses a new `object()` as the `uid`.
@@ -94,42 +94,42 @@
 >>> int in entity.components
 True
 >>> del entity.components[int]
 >>> entity.components[int]  # Missing keys raise KeyError
 Traceback (most recent call last):
   ...
 KeyError: <Entity...>
->>> entity.components.get(int, "default")  # Test keys with `.get()` like a dictionary.
+>>> entity.components.get(int, "default")  # Test keys with `.get()` like a dictionary
 'default'
 >>> @attrs.define
 ... class Vector2:
 ...     x: int = 0
 ...     y: int = 0
 >>> entity.components[Vector2] = Vector2(1, 2)
 >>> entity.components[Vector2]
 Vector2(x=1, y=2)
->>> entity.components.update({int: 11, Vector2: Vector2(0, 0)})  # Multiple values can be assigned like a dict.
+>>> entity.components |= {int: 11, Vector2: Vector2(0, 0)}  # Multiple values can be assigned like a dict
 >>> entity.components[int]
 11
 >>> entity.components[Vector2]
 Vector2(x=0, y=0)
 
-# Queries can be made on all entities of a world with matching components.
+# Queries can be made on all entities of a world with matching components
 >>> for e in world.Q.all_of(components=[Vector2]):
 ...     e.components[Vector2].x += 10
 >>> entity.components[Vector2]
 Vector2(x=10, y=0)
 
-# You can match components and iterate over them at the same time.  This can be combined with the above.
+# You can match components and iterate over them at the same time.  This can be combined with the above
 >>> for pos, i in world.Q[Vector2, int]:
 ...     print((pos, i))
 (Vector2(x=10, y=0), 11)
 
-# You can include `Entity` to iterate over entities with their components.
-# This always iterates over the entity itself instead of an Entity component.
+# You can include `Entity` to iterate over entities with their components
+# This always iterates over the entity itself instead of an Entity component
 >>> for e, pos, i in world.Q[tcod.ecs.Entity, Vector2, int]:
 ...     print((e, pos, i))
 (<Entity...>, Vector2(x=10, y=0), 11)
 
 ```
 
 ## Named Components
@@ -145,31 +145,29 @@
 >>> entity.components[Vector2] = Vector2(0, 0)
 >>> entity.components[("velocity", Vector2)] = Vector2(1, 1)
 >>> entity.components[("velocity", Vector2)]
 Vector2(x=1, y=1)
 >>> @attrs.define(frozen=True)
 ... class Slot:
 ...     index: int
->>> entity.components.update(  # Like a dict Entity.components has the `.update()` method.
-...     {
-...         ("hp", int): 10,
-...         ("max_hp", int): 12,
-...         ("atk", int): 1,
-...         str: "foo",
-...         (Slot(1), str): "empty",
-...     }
-... )
+>>> entity.components |= {  # Like a dict Entity.components can use |= to update items in-place
+...     ("hp", int): 10,
+...     ("max_hp", int): 12,
+...     ("atk", int): 1,
+...     str: "foo",
+...     (Slot(1), str): "empty",
+... }
 >>> entity.components[("hp", int)]
 10
 >>> entity.components[str]
 'foo'
 >>> entity.components[(Slot(1), str)]
 'empty'
 
-# Queries can be made on all named components with the same syntax as normal ones.
+# Queries can be made on all named components with the same syntax as normal ones
 >>> for e in world.Q.all_of(components=[("hp", int), ("max_hp", int)]):
 ...     e.components[("hp", int)] = e.components[("max_hp", int)]
 >>> entity.components[("hp", int)]
 12
 >>> for e, pos, delta in world.Q[tcod.ecs.Entity, Vector2, ("velocity", Vector2)]:
 ...     e.components[Vector2] = Vector2(pos.x + delta.x, pos.y + delta.y)
 >>> entity.components[Vector2]
@@ -200,33 +198,33 @@
 Use `Entity.relation_tag[tag] = target` to associate a tag exclusively with a target entity.
 Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
 Tags and relations share the same space then queried, so tags can not be in the format of a component key.
 Relations are unidirectional.
 
 ```py
 >>> @attrs.define
-... class OrbitOf:  # OrbitOf component.
+... class OrbitOf:  # OrbitOf component
 ...     dist: int
->>> LandedOn = "LandedOn"  # LandedOn tag.
+>>> LandedOn = "LandedOn"  # LandedOn tag
 >>> star = world.new_entity()
 >>> planet = world.new_entity()
 >>> moon = world.new_entity()
 >>> ship = world.new_entity()
 >>> player = world.new_entity()
 >>> moon_rock = world.new_entity()
 >>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
 >>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
 >>> ship.relation_tag[LandedOn] = moon
 >>> moon_rock.relation_tag[LandedOn] = moon
 >>> player.relation_tag[LandedOn] = moon_rock
 >>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
 True
->>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
+>>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit
 True
->>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
+>>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited
 True
 >>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
 True
 >>> set(world.Q.all_of(relations=[(LandedOn, ...)]).none_of(relations=[(LandedOn, moon)])) == {player}
 True
 
 ```
```

### Comparing `tcod_ecs-3.3.0/pyproject.toml` & `tcod_ecs-3.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 line_length = 120
 profile = "black"
 skip_gitignore = true
 
 [tool.mypy] # https://mypy.readthedocs.io/en/stable/config_file.html
 files = "**/*.py"
 explicit_package_bases = true
-python_version = "3.10"            # Type check Python version with EllipsisType.
+python_version = "3.10"            # Type check Python version with EllipsisType
 warn_unused_configs = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
```

### Comparing `tcod_ecs-3.3.0/tcod/ecs/__init__.py` & `tcod_ecs-3.4.0/tcod/ecs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         >>> import tcod.ecs
         >>> world = tcod.ecs.World()  # Create a new world
         >>> world.new_entity()  # Create a new entity
         <Entity(uid=object at ...)>
         >>> entity = world["entity"]  # Get an entity from a specific identifier
         >>> other_entity = world["other"]
-    """  # Changes here should be reflected in conftest.py.
+    """  # Changes here should be reflected in conftest.py
 
     __slots__ = ("world", "uid", "__weakref__")
 
     world: Final[World]  # type:ignore[misc]  # https://github.com/python/mypy/issues/5774
     """The :any:`World` this entity belongs to."""
     uid: Final[object]  # type:ignore[misc]
     """This entities unique identifier."""
@@ -125,37 +125,46 @@
 
     @property
     def components(self) -> EntityComponents:
         """Access an entities components.
 
         Example::
 
-            >>> entity.components[str] = "foo"  # Assign component.
-            >>> entity.components[("name", str)] = "my_name" # Assign named component.
+            >>> entity.components[str] = "foo"  # Assign component
+            >>> entity.components[("name", str)] = "my_name" # Assign named component
+            >>> entity.components |= {  # Update components in-place
+            ...     ("hp", int): 10,
+            ...     ("attack", int): 4,
+            ...     ("defense", int): 1,
+            ... }
             >>> ("name", str) in entity.components
             True
             >>> {str, ("name", str)}.issubset(entity.components.keys())
             True
-            >>> list(world.Q.all_of(components=[str]))  # Query components.
+            >>> list(world.Q.all_of(components=[str]))  # Query components
             [<Entity(uid='entity')>]
-            >>> list(world.Q[tcod.ecs.Entity, str, ("name", str)])  # Query zip components.
+            >>> list(world.Q[tcod.ecs.Entity, str, ("name", str)])  # Query zip components
             [(<Entity(uid='entity')>, 'foo', 'my_name')]
         """
         return EntityComponents(self)
 
+    @components.setter
+    def components(self, value: EntityComponents) -> None:
+        assert value.entity is self
+
     @property
     def tags(self) -> EntityTags:
         """Access an entities tags.
 
         Example::
 
-            >>> entity.tags.add("tag") # Add tag.
-            >>> "tag" in entity.tags  # Check tag.
+            >>> entity.tags.add("tag") # Add tag
+            >>> "tag" in entity.tags  # Check tag
             True
-            >>> list(world.Q.all_of(tags=["tag"]))  # Query tags.
+            >>> list(world.Q.all_of(tags=["tag"]))  # Query tags
             [<Entity(uid='entity')>]
             >>> entity.tags.discard("tag")
             >>> entity.tags |= {"IsPortable", "CanBurn", "OnFire"}  # Supports in-place syntax
             >>> {"CanBurn", "OnFire"}.issubset(entity.tags)
             True
             >>> entity.tags -= {"OnFire"}
             >>> {"CanBurn", "OnFire"}.issubset(entity.tags)
@@ -169,16 +178,16 @@
 
     @property
     def relation_components(self) -> EntityComponentRelations:
         """Access an entities relation components.
 
         Example::
 
-            >>> entity.relation_components[str][other_entity] = "foo" # Assign component to relation.
-            >>> entity.relation_components[("distance", int)][other_entity] = 42 # Also works for named components.
+            >>> entity.relation_components[str][other_entity] = "foo" # Assign component to relation
+            >>> entity.relation_components[("distance", int)][other_entity] = 42 # Also works for named components
             >>> other_entity in entity.relation_components[str]
             True
             >>> list(world.Q.all_of(relations=[(str, other_entity)]))
             [<Entity(uid='entity')>]
             >>> list(world.Q.all_of(relations=[(str, ...)]))
             [<Entity(uid='entity')>]
             >>> list(world.Q.all_of(relations=[(entity, str, None)]))
@@ -190,18 +199,18 @@
 
     @property
     def relation_tag(self) -> EntityRelationsExclusive:
         """Access an entities exclusive relations.
 
         Example::
 
-            >>> entity.relation_tag["ChildOf"] = other_entity  # Assign relation.
-            >>> list(world.Q.all_of(relations=[("ChildOf", other_entity)]))  # Get children of other_entity.
+            >>> entity.relation_tag["ChildOf"] = other_entity  # Assign relation
+            >>> list(world.Q.all_of(relations=[("ChildOf", other_entity)]))  # Get children of other_entity
             [<Entity(uid='entity')>]
-            >>> list(world.Q.all_of(relations=[(entity, "ChildOf", None)]))  # Get parents of entity.
+            >>> list(world.Q.all_of(relations=[(entity, "ChildOf", None)]))  # Get parents of entity
             [<Entity(uid='other')>]
             >>> del entity.relation_tag["ChildOf"]
         """
         return EntityRelationsExclusive(self)
 
     @property
     def relation_tags(self) -> EntityRelationsExclusive:
@@ -215,32 +224,32 @@
 
     @property
     def relation_tags_many(self) -> EntityRelations:
         """Access an entities many-to-many relations.
 
         Example::
 
-            >>> entity.relation_tags_many["KnownBy"].add(other_entity)  # Assign relation.
+            >>> entity.relation_tags_many["KnownBy"].add(other_entity)  # Assign relation
         """
         return EntityRelations(self)
 
     def _set_name(self, value: object, stacklevel: int = 1) -> None:
         warnings.warn(
             "The name feature has been deprecated and will be removed.",
             FutureWarning,
             stacklevel=stacklevel + 1,
         )
         old_name = self.name
-        if old_name is not None:  # Remove self from names.
+        if old_name is not None:  # Remove self from names
             del self.world._names_by_name[old_name]
             del self.world._names_by_entity[self]
 
-        if value is not None:  # Add self to names.
+        if value is not None:  # Add self to names
             old_entity = self.world._names_by_name.get(value)
-            if old_entity is not None:  # Remove entity with old name, name will be overwritten.
+            if old_entity is not None:  # Remove entity with old name, name will be overwritten
                 del self.world._names_by_entity[old_entity]
             self.world._names_by_name[value] = self
             self.world._names_by_entity[self] = value
 
     @property
     def name(self) -> object:
         """The unique name of this entity or None.
@@ -265,15 +274,15 @@
             <Entity(uid=object at ...)>
             >>> world["foo"]
             <Entity(uid='foo')>
         """
         uid_str = f"object at 0x{id(self.uid):X}" if self.uid.__class__ == object else repr(self.uid)
         items = [f"{self.__class__.__name__}(uid={uid_str})"]
         name = self.name
-        if name is not None:  # Switch to older style.
+        if name is not None:  # Switch to older style
             items = [self.__class__.__name__, f"name={name!r}"]
         return f"<{' '.join(items)}>"
 
     def __reduce__(self) -> tuple[type[Entity], tuple[World, object]]:
         """Pickle this Entity.
 
         Note that any pickled entity will include the world it belongs to and all the entities of that world.
@@ -371,22 +380,30 @@
 
         .. versionadded:: 3.0
 
         .. deprecated:: 3.1
             This method has been deprecated. Iterate over items instead.
         """
         warnings.warn("This method has been deprecated. Iterate over items instead.", FutureWarning, stacklevel=2)
-        # Naive implementation until I feel like optimizing it.
+        # Naive implementation until I feel like optimizing it
         for key in self:
             if not isinstance(key, tuple):
                 continue
             key_name, key_component = key
             if key_component is component_type and isinstance(key_name, name_type):
                 yield key_name, key_component
 
+    def __ior__(self, value: Mapping[_ComponentKey[Any], Any] | Iterable[tuple[_ComponentKey[Any], Any]]) -> Self:
+        """Update components in-place.
+
+        .. versionadded:: 3.4
+        """
+        self.update(value)
+        return self
+
     if TYPE_CHECKING:  # Type-hinted overrides
 
         @overload
         def get(self, __key: _ComponentKey[T]) -> T | None:
             ...
 
         @overload
@@ -800,19 +817,19 @@
             FutureWarning,
             stacklevel=2,
         )
         return Entity(self, None)
 
     def __setstate__(self, state: dict[str, Any]) -> None:
         """Unpickle this object and handle state migration."""
-        global_: Entity | None = state.pop("global_", None)  # Migrate from version <=1.2.0.
+        global_: Entity | None = state.pop("global_", None)  # Migrate from version <=1.2.0
 
         self.__dict__.update(state)
 
-        if global_ is not None and global_.uid is not None:  # Migrate from version <=1.2.0.
+        if global_ is not None and global_.uid is not None:  # Migrate from version <=1.2.0
             global_._force_remap(None)
 
     def __getitem__(self, uid: object) -> Entity:
         """Return an entity associated with a unique id.
 
         Example::
 
@@ -913,15 +930,15 @@
             yield self.world._components_by_type.get(component, {}).keys()
         for tag in self._none_of_tags:
             yield self.world._tags_by_key.get(tag, set())
         for relation in self._none_of_relations:
             yield self.world._relations_lookup.get(relation, set())
 
     def _get_entities(self, extra_components: AbstractSet[_ComponentKey[object]] = frozenset()) -> set[Entity]:
-        # Place the smallest sets first to speed up intersections.
+        # Place the smallest sets first to speed up intersections
         requires = sorted(self.__iter_requires(extra_components), key=len)
         excludes = list(self.__iter_excludes())
 
         if not requires:
             if excludes:
                 msg = "A Query can not function only excluding entities."
             else:
```

### Comparing `tcod_ecs-3.3.0/PKG-INFO` & `tcod_ecs-3.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 3.3.0
+Version: 3.4.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 
 # Examples
 
 ## World
 
 ```py
 >>> import tcod.ecs
->>> world = tcod.ecs.World()  # New empty world.
+>>> world = tcod.ecs.World()  # New empty world
 
 ```
 
 ## Entity
 
 Each Entity is identified by its unique id (`uid`) which can be any hashable object and the `world` it belongs to.
 New unique entities can be created with `World.new_entity` which uses a new `object()` as the `uid`.
@@ -120,42 +120,42 @@
 >>> int in entity.components
 True
 >>> del entity.components[int]
 >>> entity.components[int]  # Missing keys raise KeyError
 Traceback (most recent call last):
   ...
 KeyError: <Entity...>
->>> entity.components.get(int, "default")  # Test keys with `.get()` like a dictionary.
+>>> entity.components.get(int, "default")  # Test keys with `.get()` like a dictionary
 'default'
 >>> @attrs.define
 ... class Vector2:
 ...     x: int = 0
 ...     y: int = 0
 >>> entity.components[Vector2] = Vector2(1, 2)
 >>> entity.components[Vector2]
 Vector2(x=1, y=2)
->>> entity.components.update({int: 11, Vector2: Vector2(0, 0)})  # Multiple values can be assigned like a dict.
+>>> entity.components |= {int: 11, Vector2: Vector2(0, 0)}  # Multiple values can be assigned like a dict
 >>> entity.components[int]
 11
 >>> entity.components[Vector2]
 Vector2(x=0, y=0)
 
-# Queries can be made on all entities of a world with matching components.
+# Queries can be made on all entities of a world with matching components
 >>> for e in world.Q.all_of(components=[Vector2]):
 ...     e.components[Vector2].x += 10
 >>> entity.components[Vector2]
 Vector2(x=10, y=0)
 
-# You can match components and iterate over them at the same time.  This can be combined with the above.
+# You can match components and iterate over them at the same time.  This can be combined with the above
 >>> for pos, i in world.Q[Vector2, int]:
 ...     print((pos, i))
 (Vector2(x=10, y=0), 11)
 
-# You can include `Entity` to iterate over entities with their components.
-# This always iterates over the entity itself instead of an Entity component.
+# You can include `Entity` to iterate over entities with their components
+# This always iterates over the entity itself instead of an Entity component
 >>> for e, pos, i in world.Q[tcod.ecs.Entity, Vector2, int]:
 ...     print((e, pos, i))
 (<Entity...>, Vector2(x=10, y=0), 11)
 
 ```
 
 ## Named Components
@@ -171,31 +171,29 @@
 >>> entity.components[Vector2] = Vector2(0, 0)
 >>> entity.components[("velocity", Vector2)] = Vector2(1, 1)
 >>> entity.components[("velocity", Vector2)]
 Vector2(x=1, y=1)
 >>> @attrs.define(frozen=True)
 ... class Slot:
 ...     index: int
->>> entity.components.update(  # Like a dict Entity.components has the `.update()` method.
-...     {
-...         ("hp", int): 10,
-...         ("max_hp", int): 12,
-...         ("atk", int): 1,
-...         str: "foo",
-...         (Slot(1), str): "empty",
-...     }
-... )
+>>> entity.components |= {  # Like a dict Entity.components can use |= to update items in-place
+...     ("hp", int): 10,
+...     ("max_hp", int): 12,
+...     ("atk", int): 1,
+...     str: "foo",
+...     (Slot(1), str): "empty",
+... }
 >>> entity.components[("hp", int)]
 10
 >>> entity.components[str]
 'foo'
 >>> entity.components[(Slot(1), str)]
 'empty'
 
-# Queries can be made on all named components with the same syntax as normal ones.
+# Queries can be made on all named components with the same syntax as normal ones
 >>> for e in world.Q.all_of(components=[("hp", int), ("max_hp", int)]):
 ...     e.components[("hp", int)] = e.components[("max_hp", int)]
 >>> entity.components[("hp", int)]
 12
 >>> for e, pos, delta in world.Q[tcod.ecs.Entity, Vector2, ("velocity", Vector2)]:
 ...     e.components[Vector2] = Vector2(pos.x + delta.x, pos.y + delta.y)
 >>> entity.components[Vector2]
@@ -226,33 +224,33 @@
 Use `Entity.relation_tag[tag] = target` to associate a tag exclusively with a target entity.
 Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
 Tags and relations share the same space then queried, so tags can not be in the format of a component key.
 Relations are unidirectional.
 
 ```py
 >>> @attrs.define
-... class OrbitOf:  # OrbitOf component.
+... class OrbitOf:  # OrbitOf component
 ...     dist: int
->>> LandedOn = "LandedOn"  # LandedOn tag.
+>>> LandedOn = "LandedOn"  # LandedOn tag
 >>> star = world.new_entity()
 >>> planet = world.new_entity()
 >>> moon = world.new_entity()
 >>> ship = world.new_entity()
 >>> player = world.new_entity()
 >>> moon_rock = world.new_entity()
 >>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
 >>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
 >>> ship.relation_tag[LandedOn] = moon
 >>> moon_rock.relation_tag[LandedOn] = moon
 >>> player.relation_tag[LandedOn] = moon_rock
 >>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
 True
->>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
+>>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit
 True
->>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
+>>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited
 True
 >>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
 True
 >>> set(world.Q.all_of(relations=[(LandedOn, ...)]).none_of(relations=[(LandedOn, moon)])) == {player}
 True
 
 ```
```


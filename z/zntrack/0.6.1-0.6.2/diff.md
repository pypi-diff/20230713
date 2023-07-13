# Comparing `tmp/zntrack-0.6.1.tar.gz` & `tmp/zntrack-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zntrack-0.6.1.tar", max compression
+gzip compressed data, was "zntrack-0.6.2.tar", max compression
```

## Comparing `zntrack-0.6.1.tar` & `zntrack-0.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.6.1/LICENSE
--rw-r--r--   0        0        0     6396 2023-05-30 07:36:43.136455 zntrack-0.6.1/README.md
--rw-r--r--   0        0        0     2320 2023-06-15 14:22:03.077439 zntrack-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      770 2023-05-30 07:36:43.146455 zntrack-0.6.1/zntrack/__init__.py
--rw-r--r--   0        0        0     2940 2023-04-08 19:50:48.755766 zntrack-0.6.1/zntrack/cli/__init__.py
--rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.6.1/zntrack/core/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-30 07:36:43.146455 zntrack-0.6.1/zntrack/core/load.py
--rw-r--r--   0        0        0    11277 2023-06-15 13:55:07.555376 zntrack-0.6.1/zntrack/core/node.py
--rw-r--r--   0        0        0    14022 2023-03-16 14:38:52.672721 zntrack-0.6.1/zntrack/core/nodify.py
--rw-r--r--   0        0        0     2080 2023-04-11 11:21:14.631288 zntrack-0.6.1/zntrack/exceptions/__init__.py
--rw-r--r--   0        0        0      195 2023-03-16 14:38:52.672721 zntrack-0.6.1/zntrack/fields/__init__.py
--rw-r--r--   0        0        0     5135 2023-04-10 18:15:43.822843 zntrack-0.6.1/zntrack/fields/dvc/__init__.py
--rw-r--r--   0        0        0     9915 2023-04-10 18:15:43.822843 zntrack-0.6.1/zntrack/fields/field.py
--rw-r--r--   0        0        0     3562 2023-04-08 19:50:48.755766 zntrack-0.6.1/zntrack/fields/meta/__init__.py
--rw-r--r--   0        0        0    16145 2023-05-26 12:06:51.613839 zntrack-0.6.1/zntrack/fields/zn/__init__.py
--rw-r--r--   0        0        0     2648 2023-05-26 07:06:39.819686 zntrack-0.6.1/zntrack/notebooks/jupyter.py
--rw-r--r--   0        0        0      159 2023-06-15 13:55:07.555376 zntrack-0.6.1/zntrack/project/__init__.py
--rw-r--r--   0        0        0    12971 2023-06-15 14:22:03.087439 zntrack-0.6.1/zntrack/project/zntrack_project.py
--rw-r--r--   0        0        0     1822 2023-03-16 14:38:52.702721 zntrack-0.6.1/zntrack/tools/__init__.py
--rw-r--r--   0        0        0     5909 2023-05-26 07:06:39.829686 zntrack-0.6.1/zntrack/utils/__init__.py
--rw-r--r--   0        0        0     2161 2023-01-31 09:35:21.909593 zntrack-0.6.1/zntrack/utils/cli.py
--rw-r--r--   0        0        0     3354 2023-04-10 11:58:36.429618 zntrack-0.6.1/zntrack/utils/config.py
--rw-r--r--   0        0        0     4776 2023-04-26 09:50:10.373360 zntrack-0.6.1/zntrack/utils/file_io.py
--rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.6.1/zntrack/utils/node_wd.py
--rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 zntrack-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.6.2/LICENSE
+-rw-r--r--   0        0        0     6396 2023-05-30 07:36:43.136455 zntrack-0.6.2/README.md
+-rw-r--r--   0        0        0     2313 2023-07-13 12:14:13.470232 zntrack-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      770 2023-05-30 07:36:43.146455 zntrack-0.6.2/zntrack/__init__.py
+-rw-r--r--   0        0        0     2890 2023-07-12 16:04:27.866686 zntrack-0.6.2/zntrack/cli/__init__.py
+-rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.6.2/zntrack/core/__init__.py
+-rw-r--r--   0        0        0     3414 2023-07-13 12:14:13.530231 zntrack-0.6.2/zntrack/core/load.py
+-rw-r--r--   0        0        0    11905 2023-07-12 16:04:27.886686 zntrack-0.6.2/zntrack/core/node.py
+-rw-r--r--   0        0        0    14023 2023-07-12 16:04:27.886686 zntrack-0.6.2/zntrack/core/nodify.py
+-rw-r--r--   0        0        0     2080 2023-04-11 11:21:14.631288 zntrack-0.6.2/zntrack/exceptions/__init__.py
+-rw-r--r--   0        0        0      195 2023-03-16 14:38:52.672721 zntrack-0.6.2/zntrack/fields/__init__.py
+-rw-r--r--   0        0        0     5434 2023-06-28 16:11:25.311451 zntrack-0.6.2/zntrack/fields/dvc/__init__.py
+-rw-r--r--   0        0        0     9915 2023-04-10 18:15:43.822843 zntrack-0.6.2/zntrack/fields/field.py
+-rw-r--r--   0        0        0     3562 2023-04-08 19:50:48.755766 zntrack-0.6.2/zntrack/fields/meta/__init__.py
+-rw-r--r--   0        0        0    18754 2023-07-13 12:14:13.530231 zntrack-0.6.2/zntrack/fields/zn/__init__.py
+-rw-r--r--   0        0        0     2648 2023-05-26 07:06:39.819686 zntrack-0.6.2/zntrack/notebooks/jupyter.py
+-rw-r--r--   0        0        0      159 2023-06-15 13:55:07.555376 zntrack-0.6.2/zntrack/project/__init__.py
+-rw-r--r--   0        0        0    14355 2023-07-13 12:14:13.600230 zntrack-0.6.2/zntrack/project/zntrack_project.py
+-rw-r--r--   0        0        0     1822 2023-03-16 14:38:52.702721 zntrack-0.6.2/zntrack/tools/__init__.py
+-rw-r--r--   0        0        0     6060 2023-07-13 12:14:13.600230 zntrack-0.6.2/zntrack/utils/__init__.py
+-rw-r--r--   0        0        0     2161 2023-01-31 09:35:21.909593 zntrack-0.6.2/zntrack/utils/cli.py
+-rw-r--r--   0        0        0     3354 2023-04-10 11:58:36.429618 zntrack-0.6.2/zntrack/utils/config.py
+-rw-r--r--   0        0        0     4776 2023-04-26 09:50:10.373360 zntrack-0.6.2/zntrack/utils/file_io.py
+-rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.6.2/zntrack/utils/node_wd.py
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 zntrack-0.6.2/PKG-INFO
```

### Comparing `zntrack-0.6.1/LICENSE` & `zntrack-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/README.md` & `zntrack-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/pyproject.toml` & `zntrack-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "ZnTrack"
-version = "0.6.1"
+version = "0.6.2"
 description = "Create, Run and Benchmark DVC Pipelines in Python"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "data-version-control", "machine-learning", "reproducibility", "collaboration"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
-dvc = "^2.52.0, !=2.53.0"
+dvc = "^3.2.2"
 pyyaml = "^6.0"
 tqdm = "^4.64.0"
 pandas = "^1.4.3"
 typer = "^0.7.0"
 
 dot4dict = "^0.1.1"
 zninit = "^0.1.9"
 znjson = "^0.2.2"
-znflow = "^0.1.11"
+znflow = "^0.1.13"
 
 
 [tool.poetry.urls]
 documentation = "https://zntrack.readthedocs.io"
 repository = "https://github.com/zincware/ZnTrack"
 
 
@@ -32,15 +32,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest-benchmark = "^3.4.1"
 pytest = "^7.1.2"
 numpy = "^1.23"
 matplotlib = "^3.5.2"
 ase = "^3.22.1"
-pre-commit = "^2.20.0"
+pre-commit = ">=2.20,<4.0"
 coverage = "^6.4"
 nbmake = "^1.3.3"
 pytest-xdist = "^2.5.0"
 optuna = "^3.1.1"
 scikit-learn = "^1.2.2"
 
 [tool.poetry.group.notebook.dependencies]
```

### Comparing `zntrack-0.6.1/zntrack/__init__.py` & `zntrack-0.6.2/zntrack/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/cli/__init__.py` & `zntrack-0.6.2/zntrack/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """The ZnTrack CLI."""
 import contextlib
 import importlib.metadata
 import os
 import pathlib
 import sys
-import uuid
 
 import git
 import typer
 import yaml
 
 from zntrack import Node, utils
 
@@ -43,15 +42,15 @@
     ),
 ) -> None:
     """ZnTrack CLI main callback."""
     _ = version  # this would be greyed out otherwise
 
 
 @app.command()
-def run(node: str, name: str = None, hash_only: bool = False) -> None:
+def run(node: str, name: str = None, meta_only: bool = False) -> None:
     """Execute a ZnTrack Node.
 
     Use as 'zntrack run module.Node --name node_name'.
     """
     env_file = pathlib.Path("env.yaml")
     if env_file.exists():
         env = yaml.safe_load(env_file.read_text())
@@ -74,19 +73,18 @@
 
     cls = getattr(module, cls)
 
     if getattr(cls, "is_node", False):
         cls(exec_func=True)
     elif issubclass(cls, Node):
         node: Node = cls.from_rev(name=name, results=False)
-        if hash_only:
-            (node.nwd / "hash").write_text(str(uuid.uuid4()))
-        else:
+        if not meta_only:
             node.run()
             node.save(parameter=False)
+        node.save(meta_only=True)
     else:
         raise ValueError(f"Node {node} is not a ZnTrack Node.")
 
 
 @app.command()
 def init(
     name: str = "New Project",
```

### Comparing `zntrack-0.6.1/zntrack/core/load.py` & `zntrack-0.6.2/zntrack/core/load.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,28 +73,30 @@
 
 
 def from_rev(name, remote=".", rev=None, **kwargs) -> T:
     """Load a ZnTrack Node by its name.
 
     Parameters
     ----------
-    name : str
+    name : str|Node
         The name of the node.
     remote : str, optional
         The remote to load the node from. Defaults to workspace.
     rev : str, optional
         The revision to load the node from. Defaults to HEAD.
     **kwargs
         Additional keyword arguments to pass to the node's constructor.
 
     Returns
     -------
     Node
         The loaded node.
     """
+    if isinstance(name, Node):
+        name = name.name
     stage = _get_stage(name, remote, rev)
 
     cmd = stage.cmd
     run_str = cmd.split()[2]
     name = cmd.split()[4]
 
     package_and_module, cls_name = run_str.rsplit(".", 1)
```

### Comparing `zntrack-0.6.1/zntrack/core/node.py` & `zntrack-0.6.2/zntrack/core/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """The ZnTrack Node class."""
 from __future__ import annotations
 
 import contextlib
 import dataclasses
 import functools
-import importlib
+import json
 import logging
 import pathlib
 import time
 import typing
+import uuid
 
 import dvc.api
 import dvc.cli
 import dvc.utils.strictyaml
 import znflow
 import zninit
 import znjson
@@ -162,16 +163,25 @@
     def nwd(self) -> pathlib.Path:
         """Get the node working directory."""
         nwd = pathlib.Path("nodes", znflow.get_attribute(self, "name"))
         if not nwd.exists():
             nwd.mkdir(parents=True)
         return nwd
 
-    def save(self, parameter: bool = True, results: bool = True) -> None:
+    def save(
+        self, parameter: bool = True, results: bool = True, meta_only: bool = False
+    ) -> None:
         """Save the node's output to disk."""
+        if meta_only:
+            # the meta data will only be written here.
+            import json
+
+            (self.nwd / "node-meta.json").write_text(json.dumps({"uuid": str(self.uuid)}))
+            return
+
         # TODO have an option to save and run dvc commit afterwards.
 
         # TODO: check if there is a difference in saving
         # a loaded node vs a new node and why
         from zntrack.fields import Field, FieldGroup
 
         # Jupyter Notebook
@@ -216,14 +226,21 @@
                 for attr in zninit.get_descriptors(Field, self=self):
                     if attr.group == FieldGroup.RESULT and not results:
                         continue
                     attr.load(self)
         except KeyError as err:
             raise exceptions.NodeNotAvailableError(self) from err
 
+        with contextlib.suppress(FileNotFoundError):
+            # If the uuid is available, we can assume that all data for
+            #  this Node is available.
+            with self.state.fs.open(self.nwd / "node-meta.json") as f:
+                node_meta = json.load(f)
+                self._uuid = uuid.UUID(node_meta["uuid"])
+                self.state.results = NodeStatusResults.AVAILABLE
         # TODO: documentation about _post_init and _post_load_ and when they are called
         self._post_load_()
 
     @classmethod
     def from_rev(
         cls, name=None, remote=None, rev=None, lazy: bool = None, results: bool = True
     ) -> Node:
@@ -241,14 +258,17 @@
             # In this case, we just ignore it. This can e.g. happen
             #  if the init is auto-generated.
             # We call '__init__' before loading, because
             #  the `__init__` might do something like self.param = kwargs["param"]
             #  and this would overwrite the loaded value.
             node.__init__()
 
+        node._in_construction = False
+        node._external_ = True
+
         kwargs = {} if lazy is None else {"lazy": lazy}
         with config.updated_config(**kwargs):
             node.load(results=results)
 
         return node
 
     @deprecated(
@@ -294,17 +314,20 @@
         cmd += ["--always-changed"]
     if desc:
         cmd += ["--desc", desc]
     field_cmds = []
     for attr in zninit.get_descriptors(Field, self=node):
         field_cmds += attr.get_stage_add_argument(node)
         optionals += attr.get_optional_dvc_cmd(node)
+
     for field_cmd in set(field_cmds):
         cmd += list(field_cmd)
 
+    cmd += ["--metrics-no-cache", f"{(node.nwd /'node-meta.json').as_posix()}"]
+
     module = module_handler(node.__class__)
     cmd += [f"zntrack run {module}.{node.__class__.__name__} --name {node.name}"]
     optionals = [x for x in optionals if x]  # remove empty entries []
     return [cmd] + optionals
 
 
 @dataclasses.dataclass
@@ -316,45 +339,40 @@
     name: str
     remote: str
     rev: str
 
     @classmethod
     def from_node(cls, node: Node):
         """Create a _NodeIdentifier from a Node object."""
+        # TODO module and cls are not needed (from_rev can handle name, rev, remote only)
         return cls(
             module=module_handler(node),
             cls=node.__class__.__name__,
             name=node.name,
             remote=node.state.remote,
             rev=node.state.rev,
         )
 
     def get_node(self) -> Node:
         """Get the node from the identifier."""
-        module = importlib.import_module(self.module)
-        cls = getattr(module, self.cls)
-        return cls.from_rev(name=self.name, remote=self.remote, rev=self.rev)
+        from zntrack import from_rev
+
+        return from_rev(name=self.name, remote=self.remote, rev=self.rev)
 
 
 class NodeConverter(znjson.ConverterBase):
     """A converter for the Node class."""
 
     level = 100
     representation = "zntrack.Node"
     instance = Node
 
     def encode(self, obj: Node) -> dict:
         """Convert the Node object to dict."""
-        node_identifier = NodeIdentifier.from_node(obj)
-        if node_identifier.rev is not None:
-            raise NotImplementedError(
-                "Dependencies to other revisions are not supported yet"
-            )
-
-        return dataclasses.asdict(node_identifier)
+        return dataclasses.asdict(NodeIdentifier.from_node(obj))
 
     def decode(self, value: dict) -> Node:
         """Create Node object from dict."""
         # TODO if rev = HEAD, replace with the rev from the 'Node.from_rev'
         return NodeIdentifier(**value).get_node()
```

### Comparing `zntrack-0.6.1/zntrack/core/nodify.py` & `zntrack-0.6.2/zntrack/core/nodify.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         Notebook name for jupyter support
     module: str
         like "src.my_module"
     func_or_cls: str
         The name of the Node class or function to be imported and run
     call_args: str
         Additional str like "(run_func=True)" or ".load().run_and_save"
+
     Returns
     -------
     list[str]
         The list to be passed to the subprocess call.
     """
     script = ["stage", "add", "-n", node_name]
     script += dvc_run_option.dvc_args
```

### Comparing `zntrack-0.6.1/zntrack/exceptions/__init__.py` & `zntrack-0.6.2/zntrack/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/fields/dvc/__init__.py` & `zntrack-0.6.2/zntrack/fields/dvc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,20 @@
     The DVCOption field is designed for paths only.
     """
 
     group = FieldGroup.PARAMETER
 
     def __init__(self, *args, **kwargs):
         """Create a DVCOption field."""
+        if node_wd.nwd in args or node_wd.nwd in kwargs.values():
+            raise ValueError(
+                "Can not set `zntrack.nwd` as value for {self}. Please use"
+                " `zntrack.nwd/...` to create a path relative to the node working"
+                " directory."
+            )
         self.dvc_option = kwargs.pop("dvc_option")
         super().__init__(*args, **kwargs)
 
     def get_files(self, instance: "Node") -> list:
         """Get the files affected by this field.
 
         Parameters
```

### Comparing `zntrack-0.6.1/zntrack/fields/field.py` & `zntrack-0.6.2/zntrack/fields/field.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/fields/meta/__init__.py` & `zntrack-0.6.2/zntrack/fields/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/fields/zn/__init__.py` & `zntrack-0.6.2/zntrack/fields/zn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -274,14 +274,30 @@
         file = self.get_files(instance)[0]
         return [(f"--{self.dvc_option}", file.as_posix())]
 
 
 _default = object()
 
 
+def _get_all_connections_and_instances(value) -> list["Node"]:
+    """Get Nodes from Connections and CombinedConnections."""
+    connections = []
+    stack = [value]
+    while stack:
+        node = stack.pop()
+        if isinstance(node, znflow.CombinedConnections):
+            stack.extend(node.connections)
+        elif isinstance(node, znflow.Connection):
+            instance = node.instance
+            while isinstance(instance, znflow.Connection):
+                instance = instance.instance
+            connections.append(instance)
+    return connections
+
+
 class Dependency(LazyField):
     """A dependency field."""
 
     dvc_option = "deps"
     group = FieldGroup.PARAMETER
 
     def __init__(self, default=_default):
@@ -313,24 +329,64 @@
         if not isinstance(value, (list, tuple)):
             value = [value]
         if isinstance(value, tuple):
             value = list(value)
 
         others = []
         for node in value:
-            if isinstance(node, znflow.CombinedConnections):
-                others.extend(node.connections)
+            if isinstance(node, (znflow.CombinedConnections, znflow.Connection)):
+                others.extend(_get_all_connections_and_instances(node))
+            else:
+                others.append(node)
 
-        value.extend(others)
+        value = others
 
         for node in value:
+            node: Node
             if node is None:
                 continue
-            if isinstance(node, znflow.Connection):
-                node = node.instance
+            if node._external_:
+                from zntrack.utils import run_dvc_cmd
+
+                # TODO save these files in a specific directory called `external`
+                # TODO the `dvc import cmd` should not run here but rather be a stage?
+
+                deps_file = pathlib.Path("external", f"{node.uuid}.json")
+                deps_file.parent.mkdir(exist_ok=True, parents=True)
+
+                # zntrack run node.name --external \
+                # --remote node.state.remote --rev node.state.rev
+
+                # when combining with zn.nodes this should be used
+                # dvc stage add <name> --params params.yaml:<name>
+                # --outs nodes/<name>/node-meta.json zntrack run <name> --external
+
+                cmd = [
+                    "import",
+                    node.state.remote if node.state.remote is not None else ".",
+                    (node.nwd / "node-meta.json").as_posix(),
+                    "-o",
+                    deps_file.as_posix(),
+                ]
+                if node.state.rev is not None:
+                    cmd.extend(["--rev", node.state.rev])
+                # TODO how can we test, that the loaded file truly is the correct one?
+                if not deps_file.exists():
+                    run_dvc_cmd(cmd)
+                files.append(deps_file.as_posix())
+                # dvc import node-meta.json + add as dependency file
+                continue
+            # if node.state.rev is not None or node.state.remote is not None:
+            #     # TODO if the Node has a `rev` or `remote` attribute, we need to
+            #     #  get the UUID file of the respective Node through node.state.fs.open
+            #     # save that somewhere (can't use NWD, because we can now have multiple
+            #     # nodes with the same name...)
+            #     # and make the uuid a dependency of the node.
+            #     continue
+            files.append(node.nwd / "node-meta.json")
             for field in zninit.get_descriptors(Field, self=node):
                 if field.dvc_option in ["params", "deps"]:
                     # We do not want to depend on parameter files or
                     # recursively on dependencies.
                     continue
                 files.extend(field.get_files(node))
                 log.debug(f"Found field {field} and extended files to {files}")
@@ -462,39 +518,40 @@
 
             _cmd = [
                 "stage",
                 "add",
                 "--name",
                 name,
                 "--force",
-                "--outs",
-                f"nodes/{name}/hash",
+                "--metrics-no-cache",
+                f"nodes/{name}/node-meta.json",
                 "--params",
                 f"zntrack.json:{instance.name}.{self.name}",
             ]
             field_cmds = []
             for attr in zninit.get_descriptors(Params, self=node):
                 field_cmds += attr.get_stage_add_argument(node)
 
             for field_cmd in set(field_cmds):
                 _cmd += list(field_cmd)
 
             _cmd += [
                 f"zntrack run {module}.{node.__class__.__name__} --name"
-                f" {name} --hash-only"
+                f" {name} --meta-only"
             ]
 
             cmd.append(_cmd)
 
         return cmd
 
     def get_files(self, instance: "Node") -> list:
         """Get the files affected by this field."""
         return [
-            pathlib.Path(f"nodes/{name}/hash") for name in self.get_node_names(instance)
+            pathlib.Path(f"nodes/{name}/node-meta.json")
+            for name in self.get_node_names(instance)
         ]
 
 
 def params(*args, **kwargs) -> Params:
     """Create a params field."""
     return Params(*args, **kwargs)
```

### Comparing `zntrack-0.6.1/zntrack/notebooks/jupyter.py` & `zntrack-0.6.2/zntrack/notebooks/jupyter.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/project/zntrack_project.py` & `zntrack-0.6.2/zntrack/project/zntrack_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,14 +116,16 @@
 
     def update_node_names(self, check=True):
         """Update the node names to be unique."""
         node_names = []
         for node_uuid in self.graph.get_sorted_nodes():
             node: Node = self.graph.nodes[node_uuid]["value"]
             if node.name in node_names:
+                if node._external_:
+                    continue
                 if self.automatic_node_names:
                     idx = 1
                     while f"{node.name}_{idx}" in node_names:
                         idx += 1
                     node.name = f"{node.name}_{idx}"
                     log.debug(f"Updating {node.name = }")
 
@@ -142,29 +144,34 @@
             the number of groups + 1.
         """
         if name is None:
             name = f"Group{len(self._groups) + 1}"
         self._groups.append(name)
 
         existing_nodes = self.graph.get_sorted_nodes()
+
+        group = NodeGroup(name=name, nodes=[])
+
         try:
-            yield
+            yield group
         finally:
             for node_uuid in self.graph.get_sorted_nodes():
                 node: Node = self.graph.nodes[node_uuid]["value"]
                 if node_uuid not in existing_nodes:
                     node.name = f"{name}_{node.name}"
+                    group.nodes.append(node)
 
     def run(
         self,
         eager=False,
         repro: bool = True,
         optional: dict = None,
         save: bool = True,
         environment: dict = None,
+        nodes: list = None,
     ):
         """Run the Project Graph.
 
         Parameters
         ----------
         eager : bool, default = False
             if True, run the nodes in eager mode.
@@ -176,25 +183,44 @@
             if True, run dvc repro after running the nodes.
         optional : dict, default = None
             A dictionary of optional arguments for each node.
             Use {node_name: {arg_name: arg_value}} to pass arguments to nodes.
             Possible arg_names are e.g. 'always_changed: True'
         environment : dict, default = None
             A dictionary of environment variables for all nodes.
+        nodes : list, default = None
+            A list of node names to run. If None, run all nodes.
         """
         if not save and not eager:
             raise ValueError("Save can only be false if eager is True")
 
         self._handle_environment(environment)
 
         if optional is None:
             optional = {}
 
+        node_names = None
+        if nodes is not None:
+            node_names = []
+            for node in nodes:
+                if isinstance(node, str):
+                    node_names.append(node)
+                elif isinstance(node, Node):
+                    node_names.append(node.name)
+                elif isinstance(node, NodeGroup):
+                    node_names.extend([x.name for x in node.nodes])
+                else:
+                    raise ValueError(f"Unknown node type {type(node)}")
+
         for node_uuid in self.graph.get_sorted_nodes():
             node: Node = self.graph.nodes[node_uuid]["value"]
+            if node_names is not None and node.name not in node_names:
+                continue
+            if node._external_:
+                continue
             if eager:
                 # update connectors
                 log.info(f"Running node {node}")
                 self.graph._update_node_attributes(node, UpdateConnectors())
                 node.run()
                 if save:
                     node.save()
@@ -202,24 +228,27 @@
             else:
                 log.info(f"Adding node {node}")
                 cmd = get_dvc_cmd(node, **optional.get(node.name, {}))
                 for x in cmd:
                     run_dvc_cmd(x)
                 node.save(results=False)
         if not eager and repro:
-            run_dvc_cmd(["repro"])
+            self.repro()
             # TODO should we load the nodes here? Maybe, if lazy loading is implemented.
 
-    def build(self, environment: dict = None, optional: dict = None) -> None:
+    def build(
+        self, environment: dict = None, optional: dict = None, nodes: list = None
+    ) -> None:
         """Build the project graph without running it."""
-        self.run(repro=False, environment=environment, optional=optional)
+        self.run(repro=False, environment=environment, optional=optional, nodes=nodes)
 
     def repro(self) -> None:
         """Run dvc repro."""
         run_dvc_cmd(["repro"])
+        # TODO load nodes afterwards!
 
     def _handle_environment(self, environment: dict):
         """Write global environment variables to the env.yaml file."""
         if environment is not None:
             file = pathlib.Path("env.yaml")
             try:
                 context = yaml.safe_load(file.read_text())
@@ -376,7 +405,23 @@
         self.repo.index.commit(f"parameters for {name}")
         run_dvc_cmd(["exp", "run", "--name", name, "--queue"])
 
         for node_uuid in self.graph.get_sorted_nodes():
             node = self.graph.nodes[node_uuid]["value"]
             node.state.rev = name
         active_branch.checkout()
+
+
+@dataclasses.dataclass
+class NodeGroup:
+    """A group of nodes."""
+
+    name: str
+    nodes: list[Node]
+
+    def __contains__(self, item: Node) -> bool:
+        """Check if the Node is in the group."""
+        return item in self.nodes
+
+    def __len__(self) -> int:
+        """Get the number of nodes in the group."""
+        return len(self.nodes)
```

### Comparing `zntrack-0.6.1/zntrack/tools/__init__.py` & `zntrack-0.6.2/zntrack/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/utils/__init__.py` & `zntrack-0.6.2/zntrack/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 def run_dvc_cmd(script):
     """Run the DVC script via subprocess calls.
 
     Parameters
     ----------
     script: tuple[str]|list[str]
         A list of strings to pass the subprocess command
+
     Raises
     ------
     DVCProcessError:
         if the dvc cli command fails.
     """
     dvc_short_string = " ".join(script[:5])
     if len(script) > 5:
@@ -109,15 +110,16 @@
     if config.log_level == logging.DEBUG:
         script = [x for x in script if x != "--quiet"]
         script = script[:2] + ["--verbose", "--verbose"] + script[2:]
 
     return_code = dvc.cli.main(script)
     if return_code != 0:
         raise DVCProcessError(
-            f"DVC CLI failed ({return_code}) for cmd: \n \"{' '.join(script)}\" "
+            f'DVC CLI failed ({return_code}) for cmd: \n "dvc'
+            f' {" ".join(x for x in script if x != "--quiet")}" '
         )
     # fix for https://github.com/iterative/dvc/issues/8631
     for logger_name, logger in logging.root.manager.loggerDict.items():
         if logger_name.startswith("zntrack"):
             logger.disabled = False
     return return_code
 
@@ -154,33 +156,37 @@
     RUNNING : int
         the Node instance is currently running.
         This state will be set when the run method is called.
     FINISHED : int
         the Node instance has finished running.
     FAILED : int
         the Node instance has failed to run.
+    AVAILABLE : int
+        the Node instance was loaded and results are available.
     """
 
     UNKNOWN = 0
     PENDING = 1
     RUNNING = 2
     FINISHED = 3
     FAILED = 4
+    AVAILABLE = 5
 
 
 def cwd_temp_dir(required_files=None) -> tempfile.TemporaryDirectory:
     """Change into a temporary directory.
 
     Helper for e.g. the docs to quickly change into a temporary directory
     and copy all files, e.g. the Notebook into that directory.
 
     Parameters
     ----------
     required_files: list, optional
         A list of optional files to be copied
+
     Returns
     -------
     temp_dir:
         The temporary  directory file. Close with temp_dir.cleanup() at the end.
     """
     temp_dir = tempfile.TemporaryDirectory()  # pylint: disable=consider-using-with
     # add ignore_cleanup_errors=True in Py3.10?
```

### Comparing `zntrack-0.6.1/zntrack/utils/cli.py` & `zntrack-0.6.2/zntrack/utils/cli.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/utils/config.py` & `zntrack-0.6.2/zntrack/utils/config.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/utils/file_io.py` & `zntrack-0.6.2/zntrack/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/zntrack/utils/node_wd.py` & `zntrack-0.6.2/zntrack/utils/node_wd.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.1/PKG-INFO` & `zntrack-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: zntrack
-Version: 0.6.1
+Version: 0.6.2
 Summary: Create, Run and Benchmark DVC Pipelines in Python
 License: Apache-2.0
 Keywords: data-science,data-version-control,machine-learning,reproducibility,collaboration
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dot4dict (>=0.1.1,<0.2.0)
-Requires-Dist: dvc (>=2.52.0,<3.0.0,!=2.53.0)
+Requires-Dist: dvc (>=3.2.2,<4.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: znflow (>=0.1.11,<0.2.0)
+Requires-Dist: znflow (>=0.1.13,<0.2.0)
 Requires-Dist: zninit (>=0.1.9,<0.2.0)
 Requires-Dist: znjson (>=0.2.2,<0.3.0)
 Project-URL: documentation, https://zntrack.readthedocs.io
 Project-URL: repository, https://github.com/zincware/ZnTrack
 Description-Content-Type: text/markdown
 
 [![coeralls](https://coveralls.io/repos/github/zincware/ZnTrack/badge.svg)](https://coveralls.io/github/zincware/ZnTrack)
```


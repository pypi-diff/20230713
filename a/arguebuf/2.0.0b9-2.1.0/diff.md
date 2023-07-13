# Comparing `tmp/arguebuf-2.0.0b9.tar.gz` & `tmp/arguebuf-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguebuf-2.0.0b9.tar", max compression
+gzip compressed data, was "arguebuf-2.1.0.tar", max compression
```

## Comparing `arguebuf-2.0.0b9.tar` & `arguebuf-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,72 @@
--rw-r--r--   0        0        0     1067 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/LICENSE
--rw-r--r--   0        0        0     1590 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/README.md
--rw-r--r--   0        0        0     1030 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/__init__.py
--rw-r--r--   0        0        0       29 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/__main__.py
--rw-r--r--   0        0        0      284 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/app.py
--rw-r--r--   0        0        0     6098 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/graph.py
--rw-r--r--   0        0        0     2032 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/model.py
--rw-r--r--   0        0        0     1315 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/text.py
--rw-r--r--   0        0        0     2377 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/translator.py
--rw-r--r--   0        0        0       50 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/__init__.py
--rw-r--r--   0        0        0     1295 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/analyst.py
--rw-r--r--   0        0        0     6354 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/edge.py
--rw-r--r--   0        0        0    49429 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/graph.py
--rw-r--r--   0        0        0     1224 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/metadata.py
--rw-r--r--   0        0        0    28976 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/node.py
--rw-r--r--   0        0        0     2465 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/participant.py
--rw-r--r--   0        0        0     1852 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/reference.py
--rw-r--r--   0        0        0     2203 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/resource.py
--rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/py.typed
--rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/__init__.py
--rw-r--r--   0        0        0      639 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/aif.py
--rw-r--r--   0        0        0     3123 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/aml.py
--rw-r--r--   0        0        0      496 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/argdown_json.py
--rw-r--r--   0        0        0     5670 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/graphviz.py
--rw-r--r--   0        0        0     4301 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/microtexts.py
--rw-r--r--   0        0        0     1863 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/ova.py
--rw-r--r--   0        0        0      646 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/sadface.py
--rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/__init__.py
--rw-r--r--   0        0        0      623 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/dt.py
--rw-r--r--   0        0        0     1927 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/traversal.py
--rw-r--r--   0        0        0     3335 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/utils.py
--rw-r--r--   0        0        0     1506 2023-01-19 14:45:31.688577 arguebuf-2.0.0b9/pyproject.toml
--rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 arguebuf-2.0.0b9/setup.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 arguebuf-2.0.0b9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-13 14:27:04.988132 arguebuf-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6757 2023-07-13 14:27:04.988132 arguebuf-2.1.0/README.md
+-rw-r--r--   0        0        0      922 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/__main__.py
+-rw-r--r--   0        0        0      396 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/app.py
+-rw-r--r--   0        0        0     5958 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/graph.py
+-rw-r--r--   0        0        0     2051 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/model.py
+-rw-r--r--   0        0        0     1572 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/server.py
+-rw-r--r--   0        0        0     1302 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/text.py
+-rw-r--r--   0        0        0     2377 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/translator.py
+-rw-r--r--   0        0        0      623 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dt.py
+-rw-r--r--   0        0        0      705 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_config.py
+-rw-r--r--   0        0        0     1759 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_aif.py
+-rw-r--r--   0        0        0     2612 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_d2.py
+-rw-r--r--   0        0        0      637 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_dict.py
+-rw-r--r--   0        0        0     4983 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_graphviz.py
+-rw-r--r--   0        0        0      383 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_io.py
+-rw-r--r--   0        0        0      537 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_json.py
+-rw-r--r--   0        0        0     3235 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_networkx.py
+-rw-r--r--   0        0        0      677 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_path.py
+-rw-r--r--   0        0        0     5555 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_protobuf.py
+-rw-r--r--   0        0        0     1916 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_xaif.py
+-rw-r--r--   0        0        0     1130 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/__init__.py
+-rw-r--r--   0        0        0     1063 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_config.py
+-rw-r--r--   0        0        0     2988 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_aif.py
+-rw-r--r--   0        0        0     6996 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_aml.py
+-rw-r--r--   0        0        0     2317 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_argdown.py
+-rw-r--r--   0        0        0     1846 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_brat.py
+-rw-r--r--   0        0        0     4468 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_casebase.py
+-rw-r--r--   0        0        0      867 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_dict.py
+-rw-r--r--   0        0        0      864 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_io.py
+-rw-r--r--   0        0        0      447 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_json.py
+-rw-r--r--   0        0        0     3825 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_kialo.py
+-rw-r--r--   0        0        0     4208 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_microtexts.py
+-rw-r--r--   0        0        0     5149 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_ova.py
+-rw-r--r--   0        0        0     2904 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_path.py
+-rw-r--r--   0        0        0     5992 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_protobuf.py
+-rw-r--r--   0        0        0     3506 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_sadface.py
+-rw-r--r--   0        0        0      588 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_text.py
+-rw-r--r--   0        0        0     2828 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_xaif.py
+-rw-r--r--   0        0        0     1052 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/__init__.py
+-rw-r--r--   0        0        0      665 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/analyst.py
+-rw-r--r--   0        0        0     2430 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/edge.py
+-rw-r--r--   0        0        0    19299 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/graph.py
+-rw-r--r--   0        0        0      652 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/metadata.py
+-rw-r--r--   0        0        0     5911 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/node.py
+-rw-r--r--   0        0        0     1247 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/participant.py
+-rw-r--r--   0        0        0      754 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/reference.py
+-rw-r--r--   0        0        0      806 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/resource.py
+-rw-r--r--   0        0        0     9859 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/scheme.py
+-rw-r--r--   0        0        0      668 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/typing.py
+-rw-r--r--   0        0        0       73 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/userdata.py
+-rw-r--r--   0        0        0     3432 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/utils.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/py.typed
+-rw-r--r--   0        0        0       96 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/render/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/render/_render_d2.py
+-rw-r--r--   0        0        0     1346 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/render/_render_graphviz.py
+-rw-r--r--   0        0        0      164 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/__init__.py
+-rw-r--r--   0        0        0      639 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/aif.py
+-rw-r--r--   0        0        0      496 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/argdown.py
+-rw-r--r--   0        0        0     1837 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/d2.py
+-rw-r--r--   0        0        0      205 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/graphviz.py
+-rw-r--r--   0        0        0      212 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/microtexts.py
+-rw-r--r--   0        0        0     1864 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/ova.py
+-rw-r--r--   0        0        0      646 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/sadface.py
+-rw-r--r--   0        0        0     1109 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/xaif.py
+-rw-r--r--   0        0        0     3866 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/traverse.py
+-rw-r--r--   0        0        0      393 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/utils.py
+-rw-r--r--   0        0        0     1774 2023-07-13 14:28:13.639916 arguebuf-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7942 1970-01-01 00:00:00.000000 arguebuf-2.1.0/PKG-INFO
```

### Comparing `arguebuf-2.0.0b9/LICENSE` & `arguebuf-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b9/arguebuf/cli/graph.py` & `arguebuf-2.1.0/arguebuf/cli/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import shutil
 import typing as t
 from pathlib import Path
 
 import typer
 
 import arguebuf as ag
-from arguebuf.cli.translator import Translator
-from arguebuf.schema.graphviz import EdgeStyle
-from arguebuf.schema.graphviz import export as to_gv
 
 from . import model
+from .translator import Translator
 
 cli = typer.Typer()
 
 
 @cli.command()
 def translate(
     input_folder: Path,
     source_lang: str,
     target_lang: str,
     auth_key: str,
     input_glob: str,
     output_folder: t.Optional[Path] = None,
-    output_format: ag.GraphFormat = ag.GraphFormat.ARGUEBUF,
+    output_format: ag.dump.Format = ag.dump.Format.ARGUEBUF,
     clean: bool = False,
     overwrite: bool = False,
     start: int = 1,
 ) -> None:
     if not output_folder:
         output_folder = input_folder
 
@@ -41,50 +39,47 @@
     with typer.progressbar(
         path_pairs[start - 1 :],
         item_show_func=model.PathPair.label,
         show_pos=True,
     ) as bar:
         for path_pair in bar:
             if overwrite or not path_pair.target.exists():
-                graph = ag.Graph.from_file(path_pair.source)
+                graph = ag.load.file(path_pair.source)
                 translator.translate(graph)
-                graph.to_file(path_pair.target, output_format)
-
-
-def _strip_node_labels(node: ag.Node) -> str:
-    label: str = ""
+                ag.dump.file(
+                    graph, path_pair.target, ag.dump.Config(format=output_format)
+                )
 
-    for char in node.label:
-        if char.isspace():
-            label += char
-        else:
-            label += "–"
 
-    return label
+def _strip_node_labels(node: ag.AbstractNode) -> str:
+    return "".join(char if char.isspace() else "–" for char in node.label)
 
 
 @cli.command()
 def render(
     input_folder: Path,
     input_glob: str,
     output_folder: t.Optional[Path] = None,
     output_format: str = ".pdf",
     strip_scheme_nodes: bool = False,
     strip_node_labels: bool = False,
-    edge_style: t.Optional[EdgeStyle] = None,
+    edge_style: t.Optional[ag.schemas.graphviz.EdgeStyle] = None,
     nodesep: t.Optional[float] = None,
     ranksep: t.Optional[float] = None,
     node_wrap_col: t.Optional[int] = None,
     node_margin: t.Tuple[float, float] = (0, 0),
     font_name: t.Optional[str] = None,
     font_size: t.Optional[float] = None,
     clean: bool = False,
     overwrite: bool = False,
     start: int = 1,
     max_nodes: t.Optional[int] = None,
+    prog: str = "dot",
+    dpi: int = 300,
+    monochrome: bool = False,
 ) -> None:
     if not output_folder:
         output_folder = input_folder
 
     if clean:
         shutil.rmtree(output_folder)
         output_folder.mkdir()
@@ -97,93 +92,91 @@
     with typer.progressbar(
         paths[start - 1 :],
         item_show_func=model.PathPair.label,
         show_pos=True,
     ) as bar:
         for path_pair in bar:
             if overwrite or not path_pair.target.exists():
-                g = ag.Graph.from_file(path_pair.source)
+                g = ag.load.file(path_pair.source)
 
                 if strip_scheme_nodes:
                     g.strip_scheme_nodes()
 
-                gv = to_gv(
+                gv = ag.dump.graphviz(
                     g,
                     nodesep=nodesep,
                     ranksep=ranksep,
                     wrap_col=node_wrap_col,
-                    margin=node_margin
-                    if all(margin > 0 for margin in node_margin)
-                    else None,
+                    margin=(
+                        node_margin
+                        if all(margin > 0 for margin in node_margin)
+                        else None
+                    ),
                     font_name=font_name,
                     font_size=font_size,
                     atom_label=_strip_node_labels if strip_node_labels else None,
                     scheme_label=_strip_node_labels if strip_node_labels else None,
                     edge_style=edge_style,
                     max_nodes=max_nodes,
+                    monochrome=monochrome,
                 )
-                ag.render(gv, path_pair.target)
+                ag.render.graphviz(gv, path_pair.target, prog, dpi)
 
 
 @cli.command()
 def convert(
     input_folder: Path,
     input_glob: str,
     output_folder: t.Optional[Path] = None,
-    output_format: ag.GraphFormat = ag.GraphFormat.ARGUEBUF,
+    output_format: ag.dump.Format = ag.dump.Format.ARGUEBUF,
     clean: bool = False,
     overwrite: bool = False,
     start: int = 1,
     text_folder: t.Optional[Path] = None,
-    text_glob: t.Optional[str] = None,
+    text_suffix: str = ".txt",
 ) -> None:
     if not output_folder:
         output_folder = input_folder
 
-    texts: dict[str, str] = {}
-
-    if text_folder and text_glob:
-        for file in text_folder.glob(text_glob):
-            with file.open("r") as f:
-                filename = str(file.relative_to(text_folder).with_suffix(""))
-                texts[filename] = f.read()
-
     if clean:
         shutil.rmtree(output_folder)
         output_folder.mkdir()
 
     paths = model.PathPair.create(input_folder, output_folder, input_glob, ".json")
     bar: t.Iterable[model.PathPair]
 
     with typer.progressbar(
         paths[start - 1 :],
         item_show_func=model.PathPair.label,
         show_pos=True,
     ) as bar:
         for path_pair in bar:
             if overwrite or not path_pair.target.exists():
-                graph = ag.Graph.from_file(path_pair.source)
-                relative_source = str(
-                    path_pair.source.relative_to(input_folder).with_suffix("")
-                )
+                text_file = None
 
-                if text := texts.get(relative_source):
-                    graph.add_resource(ag.Resource(text))
+                if text_folder:
+                    text_file = text_folder / path_pair.source.relative_to(
+                        input_folder
+                    ).with_suffix(text_suffix)
 
-                graph.to_file(path_pair.target, output_format)
+                graph = ag.load.file(path_pair.source, text_file=text_file)
+
+                ag.dump.file(
+                    graph, path_pair.target, ag.dump.Config(format=output_format)
+                )
 
 
 @cli.command()
 def statistics(
     input_folder: Path,
     input_glob: str,
 ):
     files = sorted(input_folder.glob(input_glob))
 
-    graphs = [ag.Graph.from_file(file) for file in files]
+    graphs = [ag.load.file(file) for file in files]
     atom_nodes = [len(graph.atom_nodes) for graph in graphs]
     scheme_nodes = [len(graph.scheme_nodes) for graph in graphs]
     edges = [len(graph.edges) for graph in graphs]
 
     total_graphs = len(graphs)
     total_atom_nodes = sum(atom_nodes)
     total_scheme_nodes = sum(scheme_nodes)
```

### Comparing `arguebuf-2.0.0b9/arguebuf/cli/model.py` & `arguebuf-2.1.0/arguebuf/cli/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 
             pairs.extend(
                 cls(file_in, file_out) for file_in, file_out in zip(files_in, files_out)
             )
 
         else:
             raise ValueError(
-                "Folder given as input. Please also provide a folder as output together with a shell globbing pattern and an output suffix."
+                "Folder given as input. Please also provide a folder as output together"
+                " with a shell globbing pattern and an output suffix."
             )
 
         return pairs
 
     @staticmethod
     def label(path_pair: t.Optional[PathPair]) -> str:
         """Generate a string for representing a path pair.
```

### Comparing `arguebuf-2.0.0b9/arguebuf/cli/text.py` & `arguebuf-2.1.0/arguebuf/cli/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import shutil
 import typing as t
 from pathlib import Path
 
-import deepl
 import typer
 from arguebuf.cli.translator import Translator
 
 from . import model
 
 cli = typer.Typer()
```

### Comparing `arguebuf-2.0.0b9/arguebuf/cli/translator.py` & `arguebuf-2.1.0/arguebuf/cli/translator.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b9/arguebuf/models/analyst.py` & `arguebuf-2.1.0/arguebuf/model/edge.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,98 @@
-from __future__ import annotations
+from __future__ import absolute_import, annotations
 
+import logging
 import typing as t
 
-from arg_services.graph.v1 import graph_pb2
-from arguebuf.models import Userdata
-from arguebuf.services import utils
+from arguebuf.model import utils
+from arguebuf.model.metadata import Metadata
+from arguebuf.model.node import AbstractNode
+from arguebuf.model.userdata import Userdata
+
+log = logging.getLogger(__name__)
+
+__all__ = ("warn_missing_nodes", "Edge")
+
+
+def warn_missing_nodes(
+    edge_id: t.Optional[str], source_id: t.Optional[str], target_id: t.Optional[str]
+) -> None:
+    log.warning(
+        f"Skipping edge '{edge_id}': Source '{source_id}' or target '{target_id}' not"
+        " found."
+    )
+
+
+class Edge:
+    """Edge in AIF format. Connection from one Node object to another Node object."""
+
+    __slots__ = (
+        "_id",
+        "_source",
+        "_target",
+        "metadata",
+        "userdata",
+    )
 
-
-class Analyst:
-    name: t.Optional[str]
-    email: t.Optional[str]
-    userdata: Userdata
     _id: str
+    _source: AbstractNode
+    _target: AbstractNode
+    metadata: Metadata
+    userdata: Userdata
 
     def __init__(
         self,
-        name: t.Optional[str] = None,
-        email: t.Optional[str] = None,
+        source: AbstractNode,
+        target: AbstractNode,
+        metadata: t.Optional[Metadata] = None,
         userdata: t.Optional[Userdata] = None,
         id: t.Optional[str] = None,
-    ) -> None:
-        self.name = name
-        self.email = email
-        self.userdata = userdata or {}
+    ):
+        # if isinstance(source, AtomNode) and isinstance(target, AtomNode):
+        #     raise ValueError("Cannot create an edge between two atom nodes.")
+
         self._id = id or utils.uuid()
+        self._source = source
+        self._target = target
+        self.metadata = metadata or Metadata()
+        self.userdata = userdata or {}
 
-    @property
-    def id(self) -> str:
-        return self._id
+        self.__post_init__()
+
+    def __post_init__(self):
+        pass
 
-    def to_protobuf(self) -> graph_pb2.Analyst:
-        """Export Analyst object into a Graph's Analyst object in PROTOBUF format."""
-        obj = graph_pb2.Analyst(
-            name=self.name or "",
-            email=self.email or "",
+    def __eq__(self, other: t.Optional[Edge]) -> bool:
+        if other is None:
+            return False
+
+        return (
+            self.id == other.id
+            and self.source == other.source
+            and self.target == other.target
         )
-        obj.userdata.update(self.userdata)
 
-        return obj
+    def __hash__(self) -> int:
+        return hash((self.id, self.source, self.target))
 
-    @classmethod
-    def from_protobuf(cls, id: str, obj: graph_pb2.Analyst) -> Analyst:
-        """Generate Analyst object from PROTOBUF format Graph's Analyst object."""
-        return cls(
-            obj.name,
-            obj.email,
-            dict(obj.userdata.items()),
-            id,
+    def __str__(self) -> str:
+        return str(self.id)
+
+    def __repr__(self):
+        return utils.class_repr(
+            self,
+            [str(self._id), f"{self._source.__repr__()}->{self._target.__repr__()}"],
         )
+
+    @property
+    def id(self) -> str:
+        return self._id
+
+    @property
+    def source(self) -> AbstractNode:
+        """Gives the 'From'-Node."""
+        return self._source
+
+    @property
+    def target(self) -> AbstractNode:
+        """Gives the 'To'-Node."""
+        return self._target
```

### Comparing `arguebuf-2.0.0b9/arguebuf/models/edge.py` & `arguebuf-2.1.0/arguebuf/model/node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,236 +1,234 @@
 from __future__ import absolute_import, annotations
 
-import logging
 import typing as t
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
 
-import networkx as nx
 import pendulum
-from arg_services.graph.v1 import graph_pb2
 
-from arguebuf.models import Userdata
-from arguebuf.models.metadata import Metadata
-from arguebuf.models.node import Node
-from arguebuf.schema import aif, argdown_json, ova, sadface
-from arguebuf.services import dt, utils
-
-log = logging.getLogger(__name__)
-
-
-def _warn_missing_nodes(
-    edge_id: t.Optional[str], source_id: t.Optional[str], target_id: t.Optional[str]
-) -> None:
-    log.warning(
-        f"Skipping edge '{edge_id}': Source '{source_id}' or target '{target_id}' not found."
-    )
+from arguebuf.model import utils
+from arguebuf.model.metadata import Metadata
+from arguebuf.model.participant import Participant
+from arguebuf.model.reference import Reference
+from arguebuf.model.scheme import Attack, Preference, Rephrase, Scheme, Support
+from arguebuf.model.typing import TextType
+from arguebuf.model.userdata import Userdata
+from arguebuf.schemas import argdown
+
+NO_SCHEME_LABEL = "Unknown"
+
+__all__ = (
+    "AbstractNode",
+    "AtomNode",
+    "SchemeNode",
+    "AtomOrSchemeNode",
+    "NO_SCHEME_LABEL",
+)
+
+
+@dataclass
+class Color:
+    bg: str
+    fg: str
+    border: str
 
+    def __init__(
+        self,
+        bg: t.Optional[str] = None,
+        fg: t.Optional[str] = None,
+        border: t.Optional[str] = None,
+    ) -> None:
+        self.bg = bg or "#000000"
+        self.fg = fg or "#ffffff"
+        self.border = border or self.bg
 
-class Edge:
-    """Edge in AIF format. Connection from one Node object to another Node object."""
 
-    __slots__ = (
-        "_id",
-        "_source",
-        "_target",
-        "metadata",
-        "userdata",
-    )
+COLOR_MONOCHROME = Color(bg="#ffffff", fg="#000000", border="#000000")
+
+
+scheme2color: t.Dict[t.Type[Scheme], Color] = {
+    Support: Color(bg="#4CAF50"),
+    Attack: Color(bg="#F44336"),
+    Rephrase: Color(bg="#009688"),
+    Preference: Color(bg="#009688"),
+}
+
+
+class AbstractNode(ABC):
+    """Node in the AIF format."""
 
     _id: str
-    _source: Node
-    _target: Node
     metadata: Metadata
     userdata: Userdata
 
     def __init__(
         self,
-        source: Node,
-        target: Node,
         metadata: t.Optional[Metadata] = None,
         userdata: t.Optional[Userdata] = None,
         id: t.Optional[str] = None,
     ):
-        # if isinstance(source, AtomNode) and isinstance(target, AtomNode):
-        #     raise ValueError("Cannot create an edge between two atom nodes.")
-
         self._id = id or utils.uuid()
-        self._source = source
-        self._target = target
         self.metadata = metadata or Metadata()
         self.userdata = userdata or {}
 
         self.__post_init__()
 
     def __post_init__(self):
         pass
 
+    def __eq__(self, other: AbstractNode) -> bool:
+        if other is None:
+            return False
+
+        return self.id == other.id
+
+    def __hash__(self) -> int:
+        return hash(self.id)
+
+    def __str__(self) -> str:
+        return str(self.id)
+
     def __repr__(self):
-        return utils.class_repr(
-            self,
-            [str(self._id), f"{self._source.__repr__()}->{self._target.__repr__()}"],
-        )
+        return utils.class_repr(self, [self.id])
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
-    def source(self) -> Node:
-        """Gives the 'From'-Node."""
-        return self._source
+    @abstractmethod
+    def label(self) -> str:
+        """Generate a matching node label (e.g., for graphviz)"""
+
+    @abstractmethod
+    def color(self, major_claim: bool, monochrome: bool) -> Color:
+        """Get the color used in OVA based on `category`."""
+
+
+class AtomNode(AbstractNode, t.Generic[TextType]):
+    __slots__ = (
+        "_id",
+        "metadata",
+        "userdata",
+        "text",
+        "_reference",
+        "_participant",
+    )
+
+    text: TextType
+    _reference: t.Optional[Reference]
+    _participant: t.Optional[Participant]
+
+    def __init__(
+        self,
+        text: TextType,
+        reference: t.Optional[Reference] = None,
+        participant: t.Optional[Participant] = None,
+        metadata: t.Optional[Metadata] = None,
+        userdata: t.Optional[Userdata] = None,
+        id: t.Optional[str] = None,
+    ):
+        super().__init__(metadata, userdata, id)
+        self.text = text
+        self._reference = reference
+        self._participant = participant
 
     @property
-    def target(self) -> Node:
-        """Gives the 'To'-Node."""
-        return self._target
+    def plain_text(self) -> str:
+        """Get the standard `text` as string."""
 
-    @classmethod
-    def from_sadface(
-        cls,
-        obj: sadface.Edge,
-        nodes: t.Mapping[str, Node],
-    ) -> t.Optional[Edge]:
-        """Generate Edge object from SADFace Edge format."""
-        source_id = obj.get("source_id")
-        target_id = obj.get("target_id")
-
-        if source_id in nodes and target_id in nodes:
-            return cls(
-                id=obj["id"],
-                source=nodes[source_id],
-                target=nodes[target_id],
-            )
-        else:
-            _warn_missing_nodes(obj["id"], source_id, target_id)
+        return utils.xstr(self.text)
+
+    @property
+    def label(self) -> str:
+        return self.plain_text
+
+    @property
+    def reference(self) -> t.Optional[Reference]:
+        return self._reference
 
-        return None
+    @property
+    def participant(self) -> t.Optional[Participant]:
+        return self._participant
+
+    def __repr__(self):
+        return utils.class_repr(self, [self._id, self.plain_text])
 
     @classmethod
     def from_argdown_json(
         cls,
-        obj: argdown_json.Edge,
-        nodes: t.Mapping[str, Node],
-    ) -> t.Optional[Edge]:
-        """Generate Edge object from Argdown JSON Edge format."""
-        if "from" in obj:
-            source_id = obj["from"]
-        else:
-            source_id = obj["source"]
-
-        if "to" in obj:
-            target_id = obj["to"]
-        else:
-            target_id = obj["target"]
-
-        edge_id = obj["id"]
-
-        if source_id in nodes and target_id in nodes:
-            return cls(
-                id=edge_id,
-                source=nodes[source_id],
-                target=nodes[target_id],
-            )
-        else:
-            _warn_missing_nodes(edge_id, source_id, target_id)
+        obj: argdown.Node,
+        nlp: t.Optional[t.Callable[[str], t.Any]] = None,
+    ) -> AtomNode:
+        """Generate AtomNode object from Argdown JSON Node object."""
+        timestamp = pendulum.now()
+        return cls(
+            id=obj["id"],
+            text=utils.parse(obj["labelText"], nlp),
+            metadata=Metadata(timestamp, timestamp),
+        )
 
-        return None
+    def color(self, major_claim: bool, monochrome: bool) -> Color:
+        """Get the color for rendering the node."""
+        if monochrome:
+            return COLOR_MONOCHROME
 
-    @classmethod
-    def from_ova(
-        cls,
-        obj: ova.Edge,
-        nodes: t.Mapping[str, Node],
-    ) -> t.Optional[Edge]:
-        """Generate Edge object from OVA Edge format."""
-        source_id = str(obj["from"]["id"])
-        target_id = str(obj["to"]["id"])
-        date = dt.from_format(obj.get("date"), ova.DATE_FORMAT) or pendulum.now()
-
-        if source_id in nodes and target_id in nodes:
-            return cls(
-                id=utils.uuid(),
-                source=nodes[source_id],
-                target=nodes[target_id],
-                metadata=Metadata(date, date),
-            )
-        else:
-            _warn_missing_nodes(None, source_id, target_id)
+        return Color(bg="#0D47A1") if major_claim else Color(bg="#2196F3")
 
-        return None
 
-    @classmethod
-    def from_aif(
-        cls,
-        obj: aif.Edge,
-        nodes: t.Mapping[str, Node],
-    ) -> t.Optional[Edge]:
-        """Generate Edge object from AIF Edge format."""
-        source_id = obj.get("fromID")
-        target_id = obj.get("toID")
-
-        if source_id in nodes and target_id in nodes:
-            return cls(
-                id=obj["edgeID"],
-                source=nodes[source_id],
-                target=nodes[target_id],
-            )
-        else:
-            _warn_missing_nodes(obj["edgeID"], source_id, target_id)
-
-        return None
-
-    def to_aif(self) -> aif.Edge:
-        """Export Edge object into AIF Edge format."""
-        return {
-            "edgeID": str(self.id),
-            "fromID": str(self.source.id),
-            "toID": str(self.target.id),
-            "formEdgeID": None,
-        }
+class SchemeNode(AbstractNode):
+    __slots__ = (
+        "_id",
+        "created",
+        "updated",
+        "userdata",
+        "scheme",
+        "premise_descriptors",
+    )
 
-    @classmethod
-    def from_protobuf(
-        cls,
-        id: str,
-        obj: graph_pb2.Edge,
-        nodes: t.Mapping[str, Node],
-    ) -> t.Optional[Edge]:
-        """Generate Edge object from PROTOBUF Edge format."""
-        if obj.source in nodes and obj.target in nodes:
-            return cls(
-                nodes[obj.source],
-                nodes[obj.target],
-                Metadata.from_protobuf(obj.metadata),
-                dict(obj.userdata.items()),
-                id=id,
-            )
-        else:
-            _warn_missing_nodes(id, obj.source, obj.target)
-
-        return None
-
-    def to_protobuf(self) -> graph_pb2.Edge:
-        """Export Edge object into PROTOBUF Edge format."""
-        obj = graph_pb2.Edge(
-            source=self._source.id,
-            target=self._target.id,
-            metadata=self.metadata.to_protobuf(),
+    scheme: t.Optional[Scheme]
+    premise_descriptors: t.List[str]
+
+    def __init__(
+        self,
+        scheme: t.Optional[Scheme] = None,
+        premise_descriptors: t.Optional[t.List[str]] = None,
+        metadata: t.Optional[Metadata] = None,
+        userdata: t.Optional[Userdata] = None,
+        id: t.Optional[str] = None,
+    ):
+        super().__init__(metadata, userdata, id)
+        self.scheme = scheme
+        self.premise_descriptors = premise_descriptors or []
+
+    def __repr__(self):
+        return utils.class_repr(
+            self,
+            [
+                self._id,
+                type(self.scheme).__name__ if self.scheme else NO_SCHEME_LABEL,
+                self.scheme.value if self.scheme else "",
+            ],
         )
-        obj.userdata.update(self.userdata)
 
-        return obj
+    @property
+    def label(self) -> str:
+        label = NO_SCHEME_LABEL
 
-    def to_nx(
-        self,
-        g: nx.DiGraph,
-        attrs: t.Optional[t.MutableMapping[str, t.Callable[[Edge], t.Any]]] = None,
-    ) -> None:
-        """Submethod used to export Graph object g into NX Graph format."""
+        if self.scheme:
+            label = type(self.scheme).__name__
 
-        if attrs is None:
-            attrs = {}
+            if self.scheme.value != "Default":
+                label = f"{label}: {self.scheme.value}"
 
-        g.add_edge(
-            self.source.id,
-            self.target.id,
-            **{key: func(self) for key, func in attrs.items()},
-        )
+        return label
+
+    def color(self, major_claim: bool, monochrome: bool) -> Color:
+        """Get the color used in OVA based on `category`."""
+        if monochrome:
+            return COLOR_MONOCHROME
+
+        return scheme2color[type(self.scheme)] if self.scheme else Color(bg="#009688")
+
+
+AtomOrSchemeNode = t.Union[AtomNode, SchemeNode]
```

### Comparing `arguebuf-2.0.0b9/arguebuf/schema/aif.py` & `arguebuf-2.1.0/arguebuf/schemas/aif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b9/arguebuf/schema/graphviz.py` & `arguebuf-2.1.0/arguebuf/dump/_dump_graphviz.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,140 @@
 import textwrap
 import typing as t
-from enum import Enum
-from pathlib import Path
 
 from graphviz import Digraph
 
-from arguebuf.models.edge import Edge
-from arguebuf.models.graph import Graph
-from arguebuf.models.node import AtomNode, Node, SchemeNode
+from arguebuf.model import Graph
+from arguebuf.model.edge import Edge
+from arguebuf.model.node import AtomNode, SchemeNode
+from arguebuf.schemas.graphviz import EdgeStyle, GraphvizGraph
 
 try:
     from pygraphviz import AGraph
 
-    init_gv = lambda *args, **kwargs: AGraph(*args, **kwargs, directed=True)
-    add_gv_node = lambda graph, *args, **kwargs: graph.add_node(*args, **kwargs)
-    add_gv_edge = lambda graph, *args, **kwargs: graph.add_edge(*args, **kwargs)
+    def init_gv_graph(*args, **kwargs):  # type: ignore
+        return AGraph(*args, **kwargs, directed=True)
+
+    def add_gv_node(graph, *args, **kwargs):  # type: ignore
+        return graph.add_node(*args, **kwargs)
+
+    def add_gv_edge(graph, *args, **kwargs):  # type: ignore
+        return graph.add_edge(*args, **kwargs)
+
 except ModuleNotFoundError:
-    init_gv = lambda *args, **kwargs: Digraph(*args, **kwargs)
-    add_gv_node = lambda graph, *args, **kwargs: graph.node(*args, **kwargs)
-    add_gv_edge = lambda graph, *args, **kwargs: graph.edge(*args, **kwargs)
 
-GraphvizGraph = t.Union[Digraph, t.Any]
+    def init_gv_graph(*args, **kwargs):  # type: ignore
+        return Digraph(*args, **kwargs)
+
+    def add_gv_node(graph, *args, **kwargs):  # type: ignore
+        return graph.node(*args, **kwargs)
 
+    def add_gv_edge(graph, *args, **kwargs):  # type: ignore
+        return graph.edge(*args, **kwargs)
 
-class EdgeStyle(Enum):
-    BEZIER = "curved"
-    STRAIGHT = "line"
-    STEP = "ortho"
 
+__all__ = ("dump_graphviz",)
 
-def to_gv(
+
+def dump_graphviz(
     graph: Graph,
     nodesep: t.Optional[float] = None,
     ranksep: t.Optional[float] = None,
     wrap_col: t.Optional[int] = None,
     margin: t.Optional[t.Tuple[float, float]] = None,
     font_name: t.Optional[str] = None,
     font_size: t.Optional[float] = None,
     atom_label: t.Optional[t.Callable[[AtomNode], str]] = None,
     scheme_label: t.Optional[t.Callable[[SchemeNode], str]] = None,
     graph_attr: t.Optional[t.Mapping[str, str]] = None,
     node_attr: t.Optional[t.Mapping[str, str]] = None,
     edge_attr: t.Optional[t.Mapping[str, str]] = None,
     edge_style: t.Optional[EdgeStyle] = None,
     max_nodes: t.Optional[int] = None,
+    monochrome: bool = False,
 ) -> t.Optional[GraphvizGraph]:
     """Transform a Graph instance into an instance of GraphViz directed graph. Make sure that a GraphViz Executable path is set on your machine for visualization. Refer to the GraphViz library for additional information."""
 
     if len(graph.nodes) > (max_nodes or 1000):
         return None
 
-    gv_margin: t.Callable[[t.Tuple[float, float]], str] = lambda x: f"{x[0]},{x[1]}"
+    def gv_margin(x):
+        return f"{x[0]},{x[1]}"
 
     if not graph_attr:
         graph_attr = {}
 
     if not node_attr:
         node_attr = {}
 
     if not edge_attr:
         edge_attr = {}
 
-    gv_graph = AGraph(
-        directed=True,
+    gv_graph = init_gv_graph(
         name=str(graph.name),
         strict=True,
-        # format=format or "pdf",
-        # engine=engine or "dot",
     )
+    # NameError
 
     gv_graph.node_attr.update(
         {
             "fontname": font_name or "Arial",
             "fontsize": str(font_size or 11),
             "margin": gv_margin(margin or (0.15, 0.1)),
             "style": "rounded,filled",
             "shape": "box",
             "width": "0",
             "height": "0",
             **node_attr,
         }
     )
-    gv_graph.edge_attr.update({"color": "#9E9E9E", **edge_attr})
+    gv_graph.edge_attr.update(
+        {"color": "#000000" if monochrome else "#9E9E9E", **edge_attr}
+    )
     gv_graph.graph_attr.update(
         {
-            # "bgcolor": "#000000",
             "rankdir": "BT",
             "margin": "0",
             "nodesep": str(nodesep or 0.25),
             "ranksep": str(ranksep or 0.5),
             "overlap": "false",
             "splines": edge_style.value if edge_style else EdgeStyle.STEP.value,
             **graph_attr,
         }
     )
 
-    for node in graph._atom_nodes.values():
-        _atom_to_gv(
+    for node in graph.atom_nodes.values():
+        _dump_atom(
             node,
             gv_graph,
             graph.major_claim == node,
             label_func=atom_label,
             wrap_col=wrap_col or 36,
+            monochrome=monochrome,
         )
 
-    for node in graph._scheme_nodes.values():
-        _scheme_to_gv(
-            node,
-            gv_graph,
-            label_func=scheme_label,
-        )
+    for node in graph.scheme_nodes.values():
+        _dump_scheme(node, gv_graph, label_func=scheme_label, monochrome=monochrome)
 
-    for edge in graph._edges.values():
-        _edge_to_gv(edge, gv_graph)
+    for edge in graph.edges.values():
+        _dump_edge(edge, gv_graph)
 
     return gv_graph
 
 
-def _atom_to_gv(
+def _dump_atom(
     node: AtomNode,
     g: GraphvizGraph,
     major_claim: bool,
     wrap_col: int,
+    monochrome: bool,
     label_func: t.Optional[t.Callable[[AtomNode], str]] = None,
 ) -> None:
     """Submethod used to export Graph object g into GV Graph format."""
-    color = node.color(major_claim)
+    color = node.color(major_claim, monochrome)
     label = label_func(node) if label_func else node.label
 
     # TODO: Improve wrapping
     # https://stackoverflow.com/a/26538082/7626878
     add_gv_node(
         g,
         node.id,
@@ -137,56 +142,35 @@
         fontcolor=color.fg,
         fillcolor=color.bg,
         color=color.border,
         root=str(major_claim),
     )
 
 
-def _scheme_to_gv(
+def _dump_scheme(
     node: SchemeNode,
     g: GraphvizGraph,
+    monochrome: bool,
     label_func: t.Optional[t.Callable[[SchemeNode], str]] = None,
 ) -> None:
     """Submethod used to export Graph object g into GV Graph format."""
 
-    color = node.color(major_claim=False)
+    color = node.color(False, monochrome)
     label = label_func(node) if label_func else node.label
 
     add_gv_node(
         g,
         node.id,
         label=label,
         fontcolor=color.fg,
         fillcolor=color.bg,
         color=color.border,
     )
 
 
-def _edge_to_gv(edge: Edge, g: GraphvizGraph) -> None:
+def _dump_edge(edge: Edge, g: GraphvizGraph) -> None:
     """Submethod used to export Graph object g into GV Graph format."""
     add_gv_edge(
         g,
         edge.source.id,
         edge.target.id,
     )
-
-
-def render(
-    graph: t.Optional[GraphvizGraph],
-    path: t.Union[Path, str],
-    prog: t.Literal["neato", "dot", "twopi", "circo", "fdp", "nop"] = "dot",
-) -> None:
-    """Visualize a Graph instance using a GraphViz backend. Make sure that a GraphViz Executable path is set on your machine for visualization."""
-    if isinstance(path, str):
-        path = Path(path)
-
-    if graph is None:
-        pass
-    elif isinstance(graph, Graph):
-        raise ValueError(
-            "This method expects a graph in the 'DOT' format."
-            "Please use 'graph.to_gv()' to convert your argument graph to the 'DOT' format."
-        )
-    elif isinstance(graph, Digraph):
-        graph.render(outfile=path, renderer=prog)
-    else:
-        graph.draw(path=path, prog=prog)
```

### Comparing `arguebuf-2.0.0b9/arguebuf/schema/microtexts.py` & `arguebuf-2.1.0/arguebuf/load/_load_microtexts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import typing as t
 from dataclasses import dataclass
-from enum import Enum
 
 from lxml import etree
 
-import arguebuf as ag
-from arguebuf import AtomNode, Edge, Graph, SchemeNode
-from arguebuf.services import utils
+from arguebuf.model import Graph, utils
+from arguebuf.model.node import Attack, Support
+from arguebuf.schemas.microtexts import EdgeType
 
+from ._config import Config, DefaultConfig
 
-class EdgeType(Enum):
-    SEGMENTATION = "seg"
-    SUPPORT_DEFAULT = "sup"
-    SUPPORT_EXAMPLE = "exa"
-    ADDITIONAL_SOURCE = "add"
-    ATTACK_ATOM = "reb"
-    ATTACK_SCHEME = "und"
+__all__ = ("load_microtexts",)
 
 
 @dataclass
 class _Edge:
     source: str
     target: str
     type: EdgeType
@@ -33,32 +27,26 @@
             EdgeType(str(elem.attrib["type"])),
         )
         for elem in elems
         if isinstance(elem, etree._Element)
     }
 
 
-def from_microtexts(
-    obj: t.IO,
-    name: t.Optional[str] = None,
-    graph_class: t.Type[Graph] = Graph,
-    atom_class: t.Type[AtomNode] = AtomNode,
-    scheme_class: t.Type[SchemeNode] = SchemeNode,
-    edge_class: t.Type[Edge] = Edge,
-    nlp: t.Optional[t.Callable[[str], t.Any]] = None,
+def load_microtexts(
+    obj: t.IO, name: t.Optional[str] = None, config: Config = DefaultConfig
 ) -> Graph:
     """
     Generate Graph structure from AML argument graph file
     ElementTree XML API: https://docs.python.org/3/library/xml.etree.elementtree.html#
     """
 
     tree = etree.parse(obj)
     root = tree.getroot()
     id = root.get("id")
-    g = graph_class(name or id)
+    g = config.GraphClass(name or id)
     g.userdata = {"stance": root.get("stance"), "topic": root.get("topic_id")}
 
     segmentation_edge_tags = root.xpath("//edge[@type='seg']")
     atom_edge_tags = root.xpath("//edge[@type='sup' or @type='exa' or @type='reb']")
     scheme_edge_tags = root.xpath("//edge[@type='add']")
     edge_edge_tags = root.xpath("//edge[@type='und']")
     edu_tags = root.xpath("//edu")
@@ -89,45 +77,50 @@
 
     for adu in adu_tags:
         if isinstance(adu, etree._Element) and (adu_id := adu.get("id")):
             adu_source_id = adu2source[adu_id]
             adu_source = source_tags[adu_source_id]
 
             if adu_source.text is not None:
-                atom = atom_class(utils.parse(adu_source.text, nlp), id=adu_id)
+                atom = config.AtomNodeClass(
+                    utils.parse(adu_source.text, config.nlp), id=adu_id
+                )
 
                 if type := adu.get("type"):
                     atom.userdata["type"] = type
 
                 g.add_node(atom)
 
+                if adu_source.get("implicit"):
+                    g.major_claim = atom
+
     for edge_id, edge in atom_edges.items():
-        scheme_node = scheme_class(id=edge_id)
+        scheme_node = config.SchemeNodeClass(id=edge_id)
 
         if edge.type == EdgeType.SUPPORT_DEFAULT:
-            scheme_node.scheme = ag.Support.DEFAULT
+            scheme_node.scheme = Support.DEFAULT
         elif edge.type == EdgeType.SUPPORT_EXAMPLE:
-            scheme_node.scheme = ag.Support.EXAMPLE
+            scheme_node.scheme = Support.EXAMPLE
         elif edge.type == EdgeType.ATTACK_ATOM:
-            scheme_node.scheme = ag.Attack.DEFAULT
+            scheme_node.scheme = Attack.DEFAULT
 
         if (source_atom := g.atom_nodes.get(edge.source)) and (
             target_atom := g.atom_nodes.get(edge.target)
         ):
-            g.add_edge(edge_class(source_atom, scheme_node))
-            g.add_edge(edge_class(scheme_node, target_atom))
+            g.add_edge(config.EdgeClass(source_atom, scheme_node))
+            g.add_edge(config.EdgeClass(scheme_node, target_atom))
 
-    for edge in scheme_edges.values():
-        if (scheme_node := g.scheme_nodes.get(edge.target)) and (
+    for edge_id, edge in edge_edges.items():
+        if (target_scheme := g.scheme_nodes.get(edge.target)) and (
             atom_node := g.atom_nodes.get(edge.source)
         ):
-            g.add_edge(edge_class(atom_node, scheme_node))
+            source_scheme = config.SchemeNodeClass(id=edge_id, scheme=Attack.DEFAULT)
+            g.add_edge(config.EdgeClass(atom_node, source_scheme))
+            g.add_edge(config.EdgeClass(source_scheme, target_scheme))
 
-    for edge_id, edge in edge_edges.items():
-        if (target_scheme := g.scheme_nodes.get(edge.target)) and (
+    for edge in scheme_edges.values():
+        if (scheme_node := g.scheme_nodes.get(edge.target)) and (
             atom_node := g.atom_nodes.get(edge.source)
         ):
-            source_scheme = scheme_class(id=edge_id)
-            g.add_edge(edge_class(atom_node, source_scheme))
-            g.add_edge(edge_class(source_scheme, target_scheme))
+            g.add_edge(config.EdgeClass(atom_node, scheme_node))
 
     return g
```

### Comparing `arguebuf-2.0.0b9/arguebuf/schema/ova.py` & `arguebuf-2.1.0/arguebuf/schemas/ova.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from arguebuf.schema.aif import NodeType
+from arguebuf.schemas.aif import NodeType
 
 DATE_FORMAT = "DD/MM/YYYY - HH:mm:ss"
 DATE_FORMAT_ANALYSIS = "DD/MM/YYYY"
 
 Node = t.TypedDict(
     "Node",
     {
```

### Comparing `arguebuf-2.0.0b9/arguebuf/schema/sadface.py` & `arguebuf-2.1.0/arguebuf/schemas/sadface.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b9/arguebuf/services/dt.py` & `arguebuf-2.1.0/arguebuf/dt.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b9/arguebuf/services/utils.py` & `arguebuf-2.1.0/arguebuf/model/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,103 +33,112 @@
 
         return out
 
     return text
 
 
 def type_error(actual: t.Type, expected: t.Type) -> str:
-    return f"Expected type '{expected}', but got '{actual}'. Make sure that you are passing the correct method arguments."
+    return (
+        f"Expected type '{expected}', but got '{actual}'. Make sure that you are"
+        " passing the correct method arguments."
+    )
 
 
 def duplicate_key_error(name: str, key: str) -> str:
-    return f"Graph '{name}' already contains an element with key '{key}'. The keys have to be unique within each graph."
+    return (
+        f"Graph '{name}' already contains an element with key '{key}'. The keys have to"
+        " be unique within each graph."
+    )
 
 
 def missing_key_error(name: str, key: str) -> str:
-    return f"Graph '{name}' does not contain an element with key '{key}'. It cannot be removed."
+    return (
+        f"Graph '{name}' does not contain an element with key '{key}'. It cannot be"
+        " removed."
+    )
 
 
-T = t.TypeVar("T")
-U = t.TypeVar("U")
+_T = t.TypeVar("_T")
+_U = t.TypeVar("_U")
 
 
-class ImmutableList(abc.Sequence[T]):
+class ImmutableList(abc.Sequence[_T]):
     """Read-only view."""
 
     __slots__ = "_store"
 
-    _store: t.MutableSequence[T]
+    _store: t.MutableSequence[_T]
 
-    def __init__(self, items: t.Optional[t.MutableSequence[T]] = None):
-        self._store = items or list()
+    def __init__(self, items: t.Optional[t.MutableSequence[_T]] = None):
+        self._store = items or []
 
     def __len__(self) -> int:
         return self._store.__len__()
 
     @t.overload
-    def __getitem__(self, key: int) -> T:
+    def __getitem__(self, key: int) -> _T:
         pass  # Don't put code here
 
     @t.overload
-    def __getitem__(self, key: slice) -> t.Sequence[T]:
+    def __getitem__(self, key: slice) -> t.Sequence[_T]:
         pass  # Don't put code here
 
-    def __getitem__(self, key: t.Union[int, slice]) -> t.Union[T, t.Sequence[T]]:
+    def __getitem__(self, key: t.Union[int, slice]) -> t.Union[_T, t.Sequence[_T]]:
         return self._store.__getitem__(key)
 
     def __repr__(self) -> str:
         return self._store.__repr__()
 
     def __str__(self) -> str:
         return self._store.__str__()
 
 
-class ImmutableSet(abc.Set[T]):
+class ImmutableSet(abc.Set[_T]):
     """Read-only view."""
 
     __slots__ = "_store"
 
-    _store: t.MutableSet[T]
+    _store: t.MutableSet[_T]
 
-    def __init__(self, items: t.Optional[t.MutableSet[T]] = None):
+    def __init__(self, items: t.Optional[t.MutableSet[_T]] = None):
         self._store = items or set()
 
     def __len__(self) -> int:
         return self._store.__len__()
 
     def __contains__(self, item: object) -> bool:
         return self._store.__contains__(item)
 
-    def __iter__(self) -> t.Iterator[T]:
+    def __iter__(self) -> t.Iterator[_T]:
         return self._store.__iter__()
 
     def __repr__(self) -> str:
         return self._store.__repr__()
 
     def __str__(self) -> str:
         return self._store.__str__()
 
 
-class ImmutableDict(t.Mapping[T, U]):
+class ImmutableDict(t.Mapping[_T, _U]):
     """Read-only view."""
 
     __slots__ = "_store"
 
-    _store: t.MutableMapping[T, U]
+    _store: t.MutableMapping[_T, _U]
 
-    def __init__(self, items: t.Optional[t.MutableMapping[T, U]] = None):
-        self._store = items or dict()
+    def __init__(self, items: t.Optional[t.MutableMapping[_T, _U]] = None):
+        self._store = items or {}
 
     def __len__(self) -> int:
         return self._store.__len__()
 
-    def __getitem__(self, key: T) -> U:
+    def __getitem__(self, key: _T) -> _U:
         return self._store.__getitem__(key)
 
-    def __contains__(self, key: T) -> bool:
+    def __contains__(self, key: _T) -> bool:
         return self._store.__contains__(key)
 
     def __iter__(self) -> t.Iterator:
         return self._store.__iter__()
 
     def __repr__(self) -> str:
         return self._store.__repr__()
```


# Comparing `tmp/arguebuf-2.1.0.tar.gz` & `tmp/arguebuf-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguebuf-2.1.0.tar", max compression
+gzip compressed data, was "arguebuf-2.1.1.tar", max compression
```

## Comparing `arguebuf-2.1.0.tar` & `arguebuf-2.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1067 2023-07-13 14:27:04.988132 arguebuf-2.1.0/LICENSE
--rw-r--r--   0        0        0     6757 2023-07-13 14:27:04.988132 arguebuf-2.1.0/README.md
--rw-r--r--   0        0        0      922 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/__init__.py
--rw-r--r--   0        0        0       29 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/__main__.py
--rw-r--r--   0        0        0      396 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/app.py
--rw-r--r--   0        0        0     5958 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/graph.py
--rw-r--r--   0        0        0     2051 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/model.py
--rw-r--r--   0        0        0     1572 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/server.py
--rw-r--r--   0        0        0     1302 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/text.py
--rw-r--r--   0        0        0     2377 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/cli/translator.py
--rw-r--r--   0        0        0      623 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dt.py
--rw-r--r--   0        0        0      705 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/__init__.py
--rw-r--r--   0        0        0      310 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_config.py
--rw-r--r--   0        0        0     1759 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_aif.py
--rw-r--r--   0        0        0     2612 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_d2.py
--rw-r--r--   0        0        0      637 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_dict.py
--rw-r--r--   0        0        0     4983 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_graphviz.py
--rw-r--r--   0        0        0      383 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_io.py
--rw-r--r--   0        0        0      537 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_json.py
--rw-r--r--   0        0        0     3235 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_networkx.py
--rw-r--r--   0        0        0      677 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_path.py
--rw-r--r--   0        0        0     5555 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_protobuf.py
--rw-r--r--   0        0        0     1916 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/dump/_dump_xaif.py
--rw-r--r--   0        0        0     1130 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/__init__.py
--rw-r--r--   0        0        0     1063 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_config.py
--rw-r--r--   0        0        0     2988 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_aif.py
--rw-r--r--   0        0        0     6996 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_aml.py
--rw-r--r--   0        0        0     2317 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_argdown.py
--rw-r--r--   0        0        0     1846 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_brat.py
--rw-r--r--   0        0        0     4468 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_casebase.py
--rw-r--r--   0        0        0      867 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_dict.py
--rw-r--r--   0        0        0      864 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_io.py
--rw-r--r--   0        0        0      447 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_json.py
--rw-r--r--   0        0        0     3825 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_kialo.py
--rw-r--r--   0        0        0     4208 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_microtexts.py
--rw-r--r--   0        0        0     5149 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_ova.py
--rw-r--r--   0        0        0     2904 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_path.py
--rw-r--r--   0        0        0     5992 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_protobuf.py
--rw-r--r--   0        0        0     3506 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_sadface.py
--rw-r--r--   0        0        0      588 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_text.py
--rw-r--r--   0        0        0     2828 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/load/_load_xaif.py
--rw-r--r--   0        0        0     1052 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/__init__.py
--rw-r--r--   0        0        0      665 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/analyst.py
--rw-r--r--   0        0        0     2430 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/edge.py
--rw-r--r--   0        0        0    19299 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/graph.py
--rw-r--r--   0        0        0      652 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/metadata.py
--rw-r--r--   0        0        0     5911 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/node.py
--rw-r--r--   0        0        0     1247 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/participant.py
--rw-r--r--   0        0        0      754 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/reference.py
--rw-r--r--   0        0        0      806 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/resource.py
--rw-r--r--   0        0        0     9859 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/scheme.py
--rw-r--r--   0        0        0      668 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/typing.py
--rw-r--r--   0        0        0       73 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/userdata.py
--rw-r--r--   0        0        0     3432 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/model/utils.py
--rw-r--r--   0        0        0        0 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/py.typed
--rw-r--r--   0        0        0       96 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/render/__init__.py
--rw-r--r--   0        0        0      976 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/render/_render_d2.py
--rw-r--r--   0        0        0     1346 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/render/_render_graphviz.py
--rw-r--r--   0        0        0      164 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/__init__.py
--rw-r--r--   0        0        0      639 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/aif.py
--rw-r--r--   0        0        0      496 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/argdown.py
--rw-r--r--   0        0        0     1837 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/d2.py
--rw-r--r--   0        0        0      205 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/graphviz.py
--rw-r--r--   0        0        0      212 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/microtexts.py
--rw-r--r--   0        0        0     1864 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/ova.py
--rw-r--r--   0        0        0      646 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/sadface.py
--rw-r--r--   0        0        0     1109 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/schemas/xaif.py
--rw-r--r--   0        0        0     3866 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/traverse.py
--rw-r--r--   0        0        0      393 2023-07-13 14:27:04.988132 arguebuf-2.1.0/arguebuf/utils.py
--rw-r--r--   0        0        0     1774 2023-07-13 14:28:13.639916 arguebuf-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7942 1970-01-01 00:00:00.000000 arguebuf-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-13 16:09:41.843059 arguebuf-2.1.1/LICENSE
+-rw-r--r--   0        0        0     6757 2023-07-13 16:09:41.843059 arguebuf-2.1.1/README.md
+-rw-r--r--   0        0        0      922 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/__main__.py
+-rw-r--r--   0        0        0      396 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/app.py
+-rw-r--r--   0        0        0     5958 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/graph.py
+-rw-r--r--   0        0        0     2051 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/model.py
+-rw-r--r--   0        0        0     1572 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/server.py
+-rw-r--r--   0        0        0     1302 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/text.py
+-rw-r--r--   0        0        0     2377 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/cli/translator.py
+-rw-r--r--   0        0        0      623 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/dt.py
+-rw-r--r--   0        0        0      705 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/dump/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/dump/_config.py
+-rw-r--r--   0        0        0     1759 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/dump/_dump_aif.py
+-rw-r--r--   0        0        0     2612 2023-07-13 16:09:41.843059 arguebuf-2.1.1/arguebuf/dump/_dump_d2.py
+-rw-r--r--   0        0        0      768 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_dict.py
+-rw-r--r--   0        0        0     4983 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_graphviz.py
+-rw-r--r--   0        0        0      383 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_io.py
+-rw-r--r--   0        0        0      537 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_json.py
+-rw-r--r--   0        0        0     3235 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_networkx.py
+-rw-r--r--   0        0        0      677 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_path.py
+-rw-r--r--   0        0        0     5555 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_protobuf.py
+-rw-r--r--   0        0        0     1916 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/dump/_dump_xaif.py
+-rw-r--r--   0        0        0     1130 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/__init__.py
+-rw-r--r--   0        0        0     1063 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_config.py
+-rw-r--r--   0        0        0     2988 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_aif.py
+-rw-r--r--   0        0        0     6996 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_aml.py
+-rw-r--r--   0        0        0     2317 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_argdown.py
+-rw-r--r--   0        0        0     1846 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_brat.py
+-rw-r--r--   0        0        0     4468 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_casebase.py
+-rw-r--r--   0        0        0      867 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_dict.py
+-rw-r--r--   0        0        0      864 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_io.py
+-rw-r--r--   0        0        0      447 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_json.py
+-rw-r--r--   0        0        0     3825 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_kialo.py
+-rw-r--r--   0        0        0     4208 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_microtexts.py
+-rw-r--r--   0        0        0     5149 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_ova.py
+-rw-r--r--   0        0        0     2904 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_path.py
+-rw-r--r--   0        0        0     5992 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_protobuf.py
+-rw-r--r--   0        0        0     3506 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_sadface.py
+-rw-r--r--   0        0        0      588 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_text.py
+-rw-r--r--   0        0        0     2828 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/load/_load_xaif.py
+-rw-r--r--   0        0        0     1052 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/__init__.py
+-rw-r--r--   0        0        0      665 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/analyst.py
+-rw-r--r--   0        0        0     2430 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/edge.py
+-rw-r--r--   0        0        0    19299 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/graph.py
+-rw-r--r--   0        0        0      652 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/metadata.py
+-rw-r--r--   0        0        0     5911 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/node.py
+-rw-r--r--   0        0        0     1247 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/participant.py
+-rw-r--r--   0        0        0      754 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/reference.py
+-rw-r--r--   0        0        0      806 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/resource.py
+-rw-r--r--   0        0        0     9859 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/scheme.py
+-rw-r--r--   0        0        0      668 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/typing.py
+-rw-r--r--   0        0        0       73 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/userdata.py
+-rw-r--r--   0        0        0     3432 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/model/utils.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/py.typed
+-rw-r--r--   0        0        0       96 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/render/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/render/_render_d2.py
+-rw-r--r--   0        0        0     1346 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/render/_render_graphviz.py
+-rw-r--r--   0        0        0      164 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/__init__.py
+-rw-r--r--   0        0        0      639 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/aif.py
+-rw-r--r--   0        0        0      496 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/argdown.py
+-rw-r--r--   0        0        0     1837 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/d2.py
+-rw-r--r--   0        0        0      205 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/graphviz.py
+-rw-r--r--   0        0        0      212 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/microtexts.py
+-rw-r--r--   0        0        0     1864 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/ova.py
+-rw-r--r--   0        0        0      646 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/sadface.py
+-rw-r--r--   0        0        0     1109 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/schemas/xaif.py
+-rw-r--r--   0        0        0     3866 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/traverse.py
+-rw-r--r--   0        0        0      393 2023-07-13 16:09:41.847060 arguebuf-2.1.1/arguebuf/utils.py
+-rw-r--r--   0        0        0     1774 2023-07-13 16:10:49.313757 arguebuf-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7942 1970-01-01 00:00:00.000000 arguebuf-2.1.1/PKG-INFO
```

### Comparing `arguebuf-2.1.0/LICENSE` & `arguebuf-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/README.md` & `arguebuf-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/__init__.py` & `arguebuf-2.1.1/arguebuf/__init__.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/cli/graph.py` & `arguebuf-2.1.1/arguebuf/cli/graph.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/cli/model.py` & `arguebuf-2.1.1/arguebuf/cli/model.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/cli/server.py` & `arguebuf-2.1.1/arguebuf/cli/server.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/cli/text.py` & `arguebuf-2.1.1/arguebuf/cli/text.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/cli/translator.py` & `arguebuf-2.1.1/arguebuf/cli/translator.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dt.py` & `arguebuf-2.1.1/arguebuf/dt.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/__init__.py` & `arguebuf-2.1.1/arguebuf/dump/__init__.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_aif.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_aif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_d2.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_d2.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_dict.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 from google.protobuf.json_format import MessageToDict
 
 from arguebuf.model import Graph
 
 from ._config import Config, DefaultConfig, Format
 from ._dump_aif import dump_aif
 from ._dump_protobuf import dump_protobuf
+from ._dump_xaif import dump_xaif
 
 __all__ = ("dump_dict",)
 
 
 def dump_dict(graph: Graph, config: Config = DefaultConfig) -> t.Dict[str, t.Any]:
     """Export structure of Graph instance to DICT argument graph format."""
 
     if config.format == Format.AIF:
         return t.cast(dict[str, t.Any], dump_aif(graph))
+    elif config.format == Format.XAIF:
+        return t.cast(dict[str, t.Any], dump_xaif(graph))
 
     return MessageToDict(dump_protobuf(graph), including_default_value_fields=False)
```

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_graphviz.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_graphviz.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_json.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_json.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_networkx.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_networkx.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_path.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_path.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_protobuf.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_protobuf.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/dump/_dump_xaif.py` & `arguebuf-2.1.1/arguebuf/dump/_dump_xaif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/__init__.py` & `arguebuf-2.1.1/arguebuf/load/__init__.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_config.py` & `arguebuf-2.1.1/arguebuf/load/_config.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_aif.py` & `arguebuf-2.1.1/arguebuf/load/_load_aif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_aml.py` & `arguebuf-2.1.1/arguebuf/load/_load_aml.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_argdown.py` & `arguebuf-2.1.1/arguebuf/load/_load_argdown.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_brat.py` & `arguebuf-2.1.1/arguebuf/load/_load_brat.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_casebase.py` & `arguebuf-2.1.1/arguebuf/load/_load_casebase.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_dict.py` & `arguebuf-2.1.1/arguebuf/load/_load_dict.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_io.py` & `arguebuf-2.1.1/arguebuf/load/_load_io.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_kialo.py` & `arguebuf-2.1.1/arguebuf/load/_load_kialo.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_microtexts.py` & `arguebuf-2.1.1/arguebuf/load/_load_microtexts.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_ova.py` & `arguebuf-2.1.1/arguebuf/load/_load_ova.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_path.py` & `arguebuf-2.1.1/arguebuf/load/_load_path.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_protobuf.py` & `arguebuf-2.1.1/arguebuf/load/_load_protobuf.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_sadface.py` & `arguebuf-2.1.1/arguebuf/load/_load_sadface.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_text.py` & `arguebuf-2.1.1/arguebuf/load/_load_text.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/load/_load_xaif.py` & `arguebuf-2.1.1/arguebuf/load/_load_xaif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/__init__.py` & `arguebuf-2.1.1/arguebuf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/analyst.py` & `arguebuf-2.1.1/arguebuf/model/analyst.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/edge.py` & `arguebuf-2.1.1/arguebuf/model/edge.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/graph.py` & `arguebuf-2.1.1/arguebuf/model/graph.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/metadata.py` & `arguebuf-2.1.1/arguebuf/model/metadata.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/node.py` & `arguebuf-2.1.1/arguebuf/model/node.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/participant.py` & `arguebuf-2.1.1/arguebuf/model/participant.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/reference.py` & `arguebuf-2.1.1/arguebuf/model/reference.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/resource.py` & `arguebuf-2.1.1/arguebuf/model/resource.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/scheme.py` & `arguebuf-2.1.1/arguebuf/model/scheme.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/typing.py` & `arguebuf-2.1.1/arguebuf/model/typing.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/model/utils.py` & `arguebuf-2.1.1/arguebuf/model/utils.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/render/_render_d2.py` & `arguebuf-2.1.1/arguebuf/render/_render_d2.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/render/_render_graphviz.py` & `arguebuf-2.1.1/arguebuf/render/_render_graphviz.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/schemas/aif.py` & `arguebuf-2.1.1/arguebuf/schemas/aif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/schemas/d2.py` & `arguebuf-2.1.1/arguebuf/schemas/d2.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/schemas/ova.py` & `arguebuf-2.1.1/arguebuf/schemas/ova.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/schemas/sadface.py` & `arguebuf-2.1.1/arguebuf/schemas/sadface.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/schemas/xaif.py` & `arguebuf-2.1.1/arguebuf/schemas/xaif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/arguebuf/traverse.py` & `arguebuf-2.1.1/arguebuf/traverse.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.1.0/pyproject.toml` & `arguebuf-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arguebuf"
-version = "2.1.0"
+version = "2.1.1"
 description = "A library for loading argument graphs in various formats (e.g., AIF)."
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arguebuf-python"
 documentation = "https://arguebuf.readthedocs.io/en/latest"
```

### Comparing `arguebuf-2.1.0/PKG-INFO` & `arguebuf-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arguebuf
-Version: 2.1.0
+Version: 2.1.1
 Summary: A library for loading argument graphs in various formats (e.g., AIF).
 Home-page: https://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


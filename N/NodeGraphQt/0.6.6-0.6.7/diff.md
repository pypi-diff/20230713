# Comparing `tmp/NodeGraphQt-0.6.6.tar.gz` & `tmp/NodeGraphQt-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.6.6.tar", last modified: Mon Jul  3 07:12:53 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.6.7.tar", last modified: Thu Jul 13 12:39:52 2023, max compression
```

## Comparing `NodeGraphQt-0.6.6.tar` & `NodeGraphQt-0.6.7.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.396490 NodeGraphQt-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.388490 NodeGraphQt-0.6.6/NodeGraphQt/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.392490 NodeGraphQt-0.6.6/NodeGraphQt/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)   101117 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/base/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.392490 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.392490 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.392490 NodeGraphQt-0.6.6/NodeGraphQt/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/nodes/backdrop_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/nodes/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/nodes/base_node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/nodes/port_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/pkg_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.392490 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_backdrop.py
--rw-r--r--   0 runner    (1001) docker     (123)    36302 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_port_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_port_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_text_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.396490 NodeGraphQt-0.6.6/NodeGraphQt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.396490 NodeGraphQt-0.6.6/NodeGraphQt/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/icons/node_base.png
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/node_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/node_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/tab_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    54896 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/NodeGraphQt/widgets/viewer_nav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.388490 NodeGraphQt-0.6.6/NodeGraphQt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-03 07:12:53.000000 NodeGraphQt-0.6.6/NodeGraphQt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-03 07:12:53.000000 NodeGraphQt-0.6.6/NodeGraphQt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 07:12:53.000000 NodeGraphQt-0.6.6/NodeGraphQt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 07:12:53.000000 NodeGraphQt-0.6.6/NodeGraphQt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 07:12:53.000000 NodeGraphQt-0.6.6/NodeGraphQt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-03 07:12:53.396490 NodeGraphQt-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.388490 NodeGraphQt-0.6.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.396490 NodeGraphQt-0.6.6/examples/hotkeys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/examples/hotkeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/examples/hotkeys/hotkey_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:53.396490 NodeGraphQt-0.6.6/examples/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/examples/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/examples/nodes/basic_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/examples/nodes/custom_ports_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/examples/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/examples/nodes/widget_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 07:12:53.396490 NodeGraphQt-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 07:12:45.000000 NodeGraphQt-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.859164 NodeGraphQt-0.6.7/NodeGraphQt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101117 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26941 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/backdrop_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/port_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/pkg_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36302 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_text_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/NodeGraphQt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/NodeGraphQt/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/icons/node_base.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/tab_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54896 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer_nav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.859164 NodeGraphQt-0.6.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/examples/hotkeys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/hotkeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/hotkeys/hotkey_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/examples/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/basic_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/custom_ports_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/widget_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-13 12:39:52.871165 NodeGraphQt-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/setup.py
```

### Comparing `NodeGraphQt-0.6.6/LICENSE.md` & `NodeGraphQt-0.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/__init__.py` & `NodeGraphQt-0.6.7/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.6.7/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.6.7/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.6.7/NodeGraphQt/base/graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.6.7/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/base/model.py` & `NodeGraphQt-0.6.7/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/base/node.py` & `NodeGraphQt-0.6.7/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/base/port.py` & `NodeGraphQt-0.6.7/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/constants.py` & `NodeGraphQt-0.6.7/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.6.7/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.6.7/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.6.7/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.6.7/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.6
+Version: 0.6.7
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.6 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.7 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.6/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.6.7/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/PKG-INFO` & `NodeGraphQt-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.6
+Version: 0.6.7
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.6 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.7 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.6/README.md` & `NodeGraphQt-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.6.7/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.6.7/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.6.7/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.6.7/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.6/setup.cfg` & `NodeGraphQt-0.6.7/setup.cfg`

 * *Files identical despite different names*


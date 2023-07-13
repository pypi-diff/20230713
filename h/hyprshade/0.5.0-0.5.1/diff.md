# Comparing `tmp/hyprshade-0.5.0.tar.gz` & `tmp/hyprshade-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.5.0.tar", max compression
+gzip compressed data, was "hyprshade-0.5.1.tar", max compression
```

## Comparing `hyprshade-0.5.0.tar` & `hyprshade-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.5.0/LICENSE
--rw-r--r--   0        0        0     2266 2023-07-13 03:26:40.709879 hyprshade-0.5.0/README.md
--rw-r--r--   0        0        0      125 2023-07-10 08:25:37.637388 hyprshade-0.5.0/examples/config.toml
--rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.5.0/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.5.0/hyprshade/__main__.py
--rw-r--r--   0        0        0     2740 2023-07-13 13:17:34.751788 hyprshade-0.5.0/hyprshade/cli.py
--rw-r--r--   0        0        0     3718 2023-07-12 13:25:08.051277 hyprshade-0.5.0/hyprshade/config.py
--rw-r--r--   0        0        0      524 2023-07-13 13:02:51.672749 hyprshade-0.5.0/hyprshade/constants.py
--rw-r--r--   0        0        0      652 2023-07-13 13:07:02.148760 hyprshade-0.5.0/hyprshade/helpers.py
--rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.5.0/hyprshade/utils.py
--rw-r--r--   0        0        0     1036 2023-07-13 13:25:04.682808 hyprshade-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.5.0/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.5.0/shaders/vibrance.glsl
--rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 hyprshade-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2440 2023-07-13 14:02:53.695910 hyprshade-0.5.1/README.md
+-rw-r--r--   0        0        0      125 2023-07-10 08:25:37.637388 hyprshade-0.5.1/examples/config.toml
+-rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.5.1/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.5.1/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2298 2023-07-13 14:02:53.697909 hyprshade-0.5.1/hyprshade/cli.py
+-rw-r--r--   0        0        0     3718 2023-07-12 13:25:08.051277 hyprshade-0.5.1/hyprshade/config.py
+-rw-r--r--   0        0        0      492 2023-07-13 14:02:53.696910 hyprshade-0.5.1/hyprshade/constants.py
+-rw-r--r--   0        0        0      652 2023-07-13 13:07:02.148760 hyprshade-0.5.1/hyprshade/helpers.py
+-rw-r--r--   0        0        0      748 2023-07-13 14:02:53.696910 hyprshade-0.5.1/hyprshade/hyprctl.py
+-rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.5.1/hyprshade/utils.py
+-rw-r--r--   0        0        0     1036 2023-07-13 14:04:50.764915 hyprshade-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.5.1/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.5.1/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.5.1/PKG-INFO
```

### Comparing `hyprshade-0.5.0/LICENSE` & `hyprshade-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.0/README.md` & `hyprshade-0.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,20 @@
 
 Or with [pipx](https://pypa.github.io/pipx/):
 
 ```sh
 pipx install hyprshade
 ```
 
-## Scheduling
+## Usage
+
+Hyprshade uses the shader files in your `~/.config/hypr/shaders` directory
+(in addition to the ones installed to `/usr/share/hyprshade`) for all of its commands.
+
+### Scheduling
 
 To have specific shaders enabled during certain periods of the day, you can
 create a config file in either `~/.config/hypr/hyprshade.toml` or `~/.config/hyprshade/config.toml`.
 
 ```toml
 [[shades]]
 name = "vibrance"
```

### Comparing `hyprshade-0.5.0/hyprshade/cli.py` & `hyprshade-0.5.1/hyprshade/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,44 @@
 import os
-import sys
 from datetime import datetime
 from itertools import chain
 from os import path
 
 import typer
 
-from hyprshade.constants import (
-    EMPTY_STR,
-    SHADER_DIRS,
-)
+from hyprshade.constants import SHADER_DIRS
 from hyprshade.helpers import resolve_shader_path
+from hyprshade.hyprctl import clear_screen_shader, get_screen_shader, set_screen_shader
 from hyprshade.utils import systemd_user_config_home
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command()
-def ls() -> int:
-    """List available screen shaders"""
-
-    for shader in chain(
-        *map(
-            os.listdir,
-            SHADER_DIRS,
-        )
-    ):
-        shader, _ = path.splitext(shader)
-        print(shader)
-
-    return 0
-
-
-@app.command()
 def on(shader_name_or_path: str) -> int:
     """Turn on screen shader"""
 
     shader_path = resolve_shader_path(shader_name_or_path)
-    code = os.system(f"hyprctl keyword decoration:screen_shader '{shader_path}'")
-    return code
+    return set_screen_shader(shader_path)
 
 
 @app.command()
 def off() -> int:
     """Turn off screen shader"""
 
-    code = os.system(f"hyprctl keyword decoration:screen_shader '{EMPTY_STR}'")
-    return code
+    return clear_screen_shader()
 
 
 @app.command()
 def toggle(shader_name_or_path: str) -> int:
     """Toggle screen shader"""
 
-    import json
-    from json import JSONDecodeError
-
-    current_shader: str | None = None
-    try:
-        o = json.load(os.popen("hyprctl -j getoption decoration:screen_shader"))
-        current_shader = str(o["str"]).strip()
-    except JSONDecodeError:
-        print("Failed to get current screen shader", file=sys.stderr)
-        return 1
-
-    if path.isfile(current_shader) and path.samefile(
-        resolve_shader_path(shader_name_or_path), current_shader
-    ):
-        off()
-        return 0
+    current_shader = get_screen_shader()
+    if path.samefile(resolve_shader_path(shader_name_or_path), current_shader):
+        return off()
 
     return on(shader_name_or_path)
 
 
 @app.command()
 def auto() -> int:
     """Turn on/off screen shader based on schedule"""
@@ -113,18 +79,33 @@
         )
         f.write(
             f"""[Unit]
 Description=Apply screen filter on schedule
 
 [Timer]
 {on_calendar}
-Persistent=true
 
 [Install]
 WantedBy=timers.target"""
         )
 
     return 0
 
 
+@app.command()
+def ls() -> int:
+    """List available screen shaders"""
+
+    for shader in chain(
+        *map(
+            os.listdir,
+            SHADER_DIRS,
+        )
+    ):
+        shader, _ = path.splitext(shader)
+        print(shader)
+
+    return 0
+
+
 def main():
     app()
```

### Comparing `hyprshade-0.5.0/hyprshade/config.py` & `hyprshade-0.5.1/hyprshade/config.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.0/hyprshade/helpers.py` & `hyprshade-0.5.1/hyprshade/helpers.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.0/hyprshade/utils.py` & `hyprshade-0.5.1/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.0/pyproject.toml` & `hyprshade-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 include = ["examples", "shaders"]
```

### Comparing `hyprshade-0.5.0/shaders/blue-light-filter.glsl` & `hyprshade-0.5.1/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.0/shaders/vibrance.glsl` & `hyprshade-0.5.1/shaders/vibrance.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.0/PKG-INFO` & `hyprshade-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprshade
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 License: MIT
 Author: John Bernard
 Author-email: loqusion@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,20 @@
 
 Or with [pipx](https://pypa.github.io/pipx/):
 
 ```sh
 pipx install hyprshade
 ```
 
-## Scheduling
+## Usage
+
+Hyprshade uses the shader files in your `~/.config/hypr/shaders` directory
+(in addition to the ones installed to `/usr/share/hyprshade`) for all of its commands.
+
+### Scheduling
 
 To have specific shaders enabled during certain periods of the day, you can
 create a config file in either `~/.config/hypr/hyprshade.toml` or `~/.config/hyprshade/config.toml`.
 
 ```toml
 [[shades]]
 name = "vibrance"
```


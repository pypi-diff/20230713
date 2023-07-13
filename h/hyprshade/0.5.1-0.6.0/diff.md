# Comparing `tmp/hyprshade-0.5.1.tar.gz` & `tmp/hyprshade-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.5.1.tar", max compression
+gzip compressed data, was "hyprshade-0.6.0.tar", max compression
```

## Comparing `hyprshade-0.5.1.tar` & `hyprshade-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.5.1/LICENSE
--rw-r--r--   0        0        0     2440 2023-07-13 14:02:53.695910 hyprshade-0.5.1/README.md
--rw-r--r--   0        0        0      125 2023-07-10 08:25:37.637388 hyprshade-0.5.1/examples/config.toml
--rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.5.1/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.5.1/hyprshade/__main__.py
--rw-r--r--   0        0        0     2298 2023-07-13 14:02:53.697909 hyprshade-0.5.1/hyprshade/cli.py
--rw-r--r--   0        0        0     3718 2023-07-12 13:25:08.051277 hyprshade-0.5.1/hyprshade/config.py
--rw-r--r--   0        0        0      492 2023-07-13 14:02:53.696910 hyprshade-0.5.1/hyprshade/constants.py
--rw-r--r--   0        0        0      652 2023-07-13 13:07:02.148760 hyprshade-0.5.1/hyprshade/helpers.py
--rw-r--r--   0        0        0      748 2023-07-13 14:02:53.696910 hyprshade-0.5.1/hyprshade/hyprctl.py
--rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.5.1/hyprshade/utils.py
--rw-r--r--   0        0        0     1036 2023-07-13 14:04:50.764915 hyprshade-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.5.1/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.5.1/shaders/vibrance.glsl
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-13 17:26:18.998108 hyprshade-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2440 2023-07-13 17:26:18.998108 hyprshade-0.6.0/README.md
+-rw-r--r--   0        0        0      125 2023-07-13 17:26:18.998108 hyprshade-0.6.0/examples/config.toml
+-rw-r--r--   0        0        0        0 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2484 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/cli.py
+-rw-r--r--   0        0        0     3709 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/config.py
+-rw-r--r--   0        0        0      483 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/constants.py
+-rw-r--r--   0        0        0      643 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/helpers.py
+-rw-r--r--   0        0        0      803 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/hyprctl.py
+-rw-r--r--   0        0        0      812 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/utils.py
+-rw-r--r--   0        0        0     1036 2023-07-13 17:26:18.998108 hyprshade-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-13 17:26:18.998108 hyprshade-0.6.0/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-13 17:26:18.998108 hyprshade-0.6.0/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.6.0/PKG-INFO
```

### Comparing `hyprshade-0.5.1/LICENSE` & `hyprshade-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.1/README.md` & `hyprshade-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.1/hyprshade/cli.py` & `hyprshade-0.6.0/hyprshade/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from datetime import datetime
 from itertools import chain
 from os import path
 
 import typer
 
-from hyprshade.constants import SHADER_DIRS
-from hyprshade.helpers import resolve_shader_path
-from hyprshade.hyprctl import clear_screen_shader, get_screen_shader, set_screen_shader
-from hyprshade.utils import systemd_user_config_home
+from .constants import SHADER_DIRS
+from .helpers import resolve_shader_path
+from .hyprctl import clear_screen_shader, get_screen_shader, set_screen_shader
+from .utils import systemd_user_config_home
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command()
 def on(shader_name_or_path: str) -> int:
     """Turn on screen shader"""
@@ -29,15 +29,17 @@
 
 
 @app.command()
 def toggle(shader_name_or_path: str) -> int:
     """Toggle screen shader"""
 
     current_shader = get_screen_shader()
-    if path.samefile(resolve_shader_path(shader_name_or_path), current_shader):
+    if current_shader is not None and path.samefile(
+        resolve_shader_path(shader_name_or_path), current_shader
+    ):
         return off()
 
     return on(shader_name_or_path)
 
 
 @app.command()
 def auto() -> int:
@@ -91,21 +93,25 @@
     return 0
 
 
 @app.command()
 def ls() -> int:
     """List available screen shaders"""
 
+    current_shader = get_screen_shader()
+    shader_base = path.basename(current_shader) if current_shader else None
+
     for shader in chain(
         *map(
             os.listdir,
             SHADER_DIRS,
         )
     ):
+        c = "*" if shader == shader_base else " "
         shader, _ = path.splitext(shader)
-        print(shader)
+        print(f"{c} {shader}")
 
     return 0
 
 
 def main():
     app()
```

### Comparing `hyprshade-0.5.1/hyprshade/config.py` & `hyprshade-0.6.0/hyprshade/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from itertools import chain, pairwise
 from os import path
 from typing import Literal, NotRequired, TypedDict, cast
 
 import tomllib
 from more_itertools import first_true, nth, partition
 
-from hyprshade.utils import hypr_config_home, hyprshade_config_home, is_time_between
+from .utils import hypr_config_home, hyprshade_config_home, is_time_between
 
 TimeInterval = tuple[time, time]
 
 
 class ShadeDict(TypedDict):
     name: str
     start_time: time
```

### Comparing `hyprshade-0.5.1/hyprshade/helpers.py` & `hyprshade-0.6.0/hyprshade/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from os import path
 
-from hyprshade.constants import SHADER_DIRS
+from .constants import SHADER_DIRS
 
 
 def resolve_shader_path(shader_name_or_path: str) -> str:
     shader_path = shader_name_or_path
     if not path.isfile(shader_path):
         for shaders_dir in SHADER_DIRS:
             shader_path = path.join(shaders_dir, glsl_ext(shader_name_or_path))
```

### Comparing `hyprshade-0.5.1/hyprshade/hyprctl.py` & `hyprshade-0.6.0/hyprshade/hyprctl.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,20 @@
     return os.system(f"hyprctl keyword decoration:screen_shader '{shader_path}'")
 
 
 def clear_screen_shader() -> int:
     return set_screen_shader(EMPTY_STR)
 
 
-def get_screen_shader() -> str:
+def get_screen_shader() -> str | None:
     try:
         o = json.load(os.popen("hyprctl -j getoption decoration:screen_shader"))
     except JSONDecodeError as e:
         raise RuntimeError("Failed to parse JSON returned by hyprctl") from e
 
     shader = str(o["str"]).strip()
     if not path.isfile(shader):
         raise RuntimeError(f"Got shader {shader} from hyprctl, which does not exist")
 
+    if shader == EMPTY_STR:
+        return None
     return shader
```

### Comparing `hyprshade-0.5.1/hyprshade/utils.py` & `hyprshade-0.6.0/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.1/pyproject.toml` & `hyprshade-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.5.1"
+version = "0.6.0"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 include = ["examples", "shaders"]
```

### Comparing `hyprshade-0.5.1/shaders/blue-light-filter.glsl` & `hyprshade-0.6.0/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.1/shaders/vibrance.glsl` & `hyprshade-0.6.0/shaders/vibrance.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.5.1/PKG-INFO` & `hyprshade-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprshade
-Version: 0.5.1
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: John Bernard
 Author-email: loqusion@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


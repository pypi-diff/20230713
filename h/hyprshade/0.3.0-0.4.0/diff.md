# Comparing `tmp/hyprshade-0.3.0.tar.gz` & `tmp/hyprshade-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.3.0.tar", max compression
+gzip compressed data, was "hyprshade-0.4.0.tar", max compression
```

## Comparing `hyprshade-0.3.0.tar` & `hyprshade-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.3.0/LICENSE
--rw-r--r--   0        0        0     2311 2023-07-12 12:40:55.928150 hyprshade-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.3.0/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.3.0/hyprshade/__main__.py
--rw-r--r--   0        0        0     2669 2023-07-12 12:44:09.002160 hyprshade-0.3.0/hyprshade/cli.py
--rw-r--r--   0        0        0     3718 2023-07-12 12:36:54.366139 hyprshade-0.3.0/hyprshade/config.py
--rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.3.0/hyprshade/helpers.py
--rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.3.0/hyprshade/utils.py
--rw-r--r--   0        0        0     1024 2023-07-12 12:44:55.348162 hyprshade-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.3.0/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.3.0/shaders/vibrance.glsl
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 hyprshade-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2266 2023-07-13 03:26:40.709879 hyprshade-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.4.0/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.4.0/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2740 2023-07-13 13:17:34.751788 hyprshade-0.4.0/hyprshade/cli.py
+-rw-r--r--   0        0        0     3718 2023-07-12 13:25:08.051277 hyprshade-0.4.0/hyprshade/config.py
+-rw-r--r--   0        0        0      524 2023-07-13 13:02:51.672749 hyprshade-0.4.0/hyprshade/constants.py
+-rw-r--r--   0        0        0      652 2023-07-13 13:07:02.148760 hyprshade-0.4.0/hyprshade/helpers.py
+-rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.4.0/hyprshade/utils.py
+-rw-r--r--   0        0        0     1024 2023-07-13 13:18:06.239790 hyprshade-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.4.0/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.4.0/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 hyprshade-0.4.0/PKG-INFO
```

### Comparing `hyprshade-0.3.0/LICENSE` & `hyprshade-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.3.0/README.md` & `hyprshade-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 # Hyprshade
 
 Frontend to Hyprland's screen shader feature
 
-<!--toc:start-->
-
-- [Hyprshade](#hyprshade)
-  - [Description](#description)
-  - [Installation](#installation)
-    - [Arch Linux](#arch-linux)
-    - [Other](#other)
-  - [Scheduling](#scheduling)
-  <!--toc:end-->
-
 ## Description
 
 Hyprshade takes full advantage of Hyprland's `decoration:screen_shader` feature
 by automating the process of switching screen shaders, either from a user-defined
 schedule or on the fly. It can be used as a replacement[^1] for apps that adjust
 the screen's color temperature such as [f.lux](https://justgetflux.com/),
 [redshift](http://jonls.dk/redshift/), or [gammastep](https://gitlab.com/chinstrap/gammastep)
@@ -86,7 +76,15 @@
 hyprshade install
 systemctl --user enable --now hyprshade.timer
 ```
 
 > `hyprshade install` must be run after updating `hyprshade.toml`.
 
 By default, they are installed to `~/.config/systemd/user` as [user units](https://wiki.archlinux.org/title/Systemd/User).
+
+You also probably want the following line in your `hyprland.conf`:
+
+```sh
+exec = hyprshade auto
+```
+
+This ensures that the correct shader is enabled when you log in.
```

### Comparing `hyprshade-0.3.0/hyprshade/cli.py` & `hyprshade-0.4.0/hyprshade/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import os
 import sys
 from datetime import datetime
+from itertools import chain
 from os import path
-from typing import Final
 
 import typer
 
-from hyprshade.helpers import get_shader_path, get_shaders_dir
+from hyprshade.constants import (
+    EMPTY_STR,
+    SHADER_DIRS,
+)
+from hyprshade.helpers import resolve_shader_path
 from hyprshade.utils import systemd_user_config_home
 
-EMPTY_STR: Final = "[[EMPTY]]"
-
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command()
 def ls() -> int:
     """List available screen shaders"""
 
-    shaders_dir = get_shaders_dir()
-    for shader in os.listdir(shaders_dir):
-        shader = path.splitext(shader)[0]
+    for shader in chain(
+        *map(
+            os.listdir,
+            SHADER_DIRS,
+        )
+    ):
+        shader, _ = path.splitext(shader)
         print(shader)
+
     return 0
 
 
 @app.command()
 def on(shader_name_or_path: str) -> int:
     """Turn on screen shader"""
 
-    shader_path = get_shader_path(shader_name_or_path)
+    shader_path = resolve_shader_path(shader_name_or_path)
     code = os.system(f"hyprctl keyword decoration:screen_shader '{shader_path}'")
     return code
 
 
 @app.command()
 def off() -> int:
     """Turn off screen shader"""
@@ -54,15 +61,15 @@
         o = json.load(os.popen("hyprctl -j getoption decoration:screen_shader"))
         current_shader = str(o["str"]).strip()
     except JSONDecodeError:
         print("Failed to get current screen shader", file=sys.stderr)
         return 1
 
     if path.isfile(current_shader) and path.samefile(
-        get_shader_path(shader_name_or_path), current_shader
+        resolve_shader_path(shader_name_or_path), current_shader
     ):
         off()
         return 0
 
     return on(shader_name_or_path)
 
 
@@ -98,15 +105,15 @@
 Type=oneshot
 ExecStart="/usr/bin/hyprshade" auto
 """
         )
 
     with open(path.join(systemd_user_config_home(), "hyprshade.timer"), "w") as f:
         on_calendar = "\n".join(
-            f"OnCalendar=*-*-* {x}" for x in schedule.on_calendar_entries()
+            sorted([f"OnCalendar=*-*-* {x}" for x in schedule.on_calendar_entries()])
         )
         f.write(
             f"""[Unit]
 Description=Apply screen filter on schedule
 
 [Timer]
 {on_calendar}
```

### Comparing `hyprshade-0.3.0/hyprshade/config.py` & `hyprshade-0.4.0/hyprshade/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from collections.abc import Iterable
+from collections.abc import Iterator
 from datetime import time
 from itertools import chain, pairwise
 from os import path
 from typing import Literal, NotRequired, TypedDict, cast
 
 import tomllib
 from more_itertools import first_true, nth, partition
@@ -71,21 +71,21 @@
     def find_shade(self, t: time) -> str | None:
         for entry_name, (start_time, end_time) in self._resolved_entries():
             if is_time_between(t, start_time, end_time):
                 return entry_name
 
         return self.default_shade_name
 
-    def on_calendar_entries(self) -> Iterable[time]:
+    def on_calendar_entries(self) -> Iterator[time]:
         for entry in self.entries:
             yield entry.start_time
             if entry.end_time is not None:
                 yield entry.end_time
 
-    def _resolved_entries(self) -> Iterable[tuple[str, TimeInterval]]:
+    def _resolved_entries(self) -> Iterator[tuple[str, TimeInterval]]:
         for entry, next_entry in pairwise(chain(self.entries, [self.entries[0]])):
             start_time = entry.start_time
             end_time = entry.end_time or next_entry.start_time
             yield entry.name, (start_time, end_time)
 
 
 class Config:
```

### Comparing `hyprshade-0.3.0/hyprshade/utils.py` & `hyprshade-0.4.0/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.3.0/pyproject.toml` & `hyprshade-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 include = ["shaders"]
```

### Comparing `hyprshade-0.3.0/shaders/blue-light-filter.glsl` & `hyprshade-0.4.0/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.3.0/shaders/vibrance.glsl` & `hyprshade-0.4.0/shaders/vibrance.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.3.0/PKG-INFO` & `hyprshade-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprshade
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: John Bernard
 Author-email: loqusion@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,24 +13,14 @@
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Hyprshade
 
 Frontend to Hyprland's screen shader feature
 
-<!--toc:start-->
-
-- [Hyprshade](#hyprshade)
-  - [Description](#description)
-  - [Installation](#installation)
-    - [Arch Linux](#arch-linux)
-    - [Other](#other)
-  - [Scheduling](#scheduling)
-  <!--toc:end-->
-
 ## Description
 
 Hyprshade takes full advantage of Hyprland's `decoration:screen_shader` feature
 by automating the process of switching screen shaders, either from a user-defined
 schedule or on the fly. It can be used as a replacement[^1] for apps that adjust
 the screen's color temperature such as [f.lux](https://justgetflux.com/),
 [redshift](http://jonls.dk/redshift/), or [gammastep](https://gitlab.com/chinstrap/gammastep)
@@ -102,7 +92,15 @@
 systemctl --user enable --now hyprshade.timer
 ```
 
 > `hyprshade install` must be run after updating `hyprshade.toml`.
 
 By default, they are installed to `~/.config/systemd/user` as [user units](https://wiki.archlinux.org/title/Systemd/User).
 
+You also probably want the following line in your `hyprland.conf`:
+
+```sh
+exec = hyprshade auto
+```
+
+This ensures that the correct shader is enabled when you log in.
+
```


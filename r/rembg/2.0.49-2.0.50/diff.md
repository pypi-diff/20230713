# Comparing `tmp/rembg-2.0.49.tar.gz` & `tmp/rembg-2.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.49.tar", last modified: Fri Jun 30 00:48:08 2023, max compression
+gzip compressed data, was "rembg-2.0.50.tar", last modified: Thu Jul 13 03:38:53 2023, max compression
```

## Comparing `rembg-2.0.49.tar` & `rembg-2.0.50.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 00:46:58.000000 rembg-2.0.49/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-30 00:46:58.000000 rembg-2.0.49/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-30 00:48:08.546652 rembg-2.0.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-06-30 00:46:58.000000 rembg-2.0.49/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-30 00:46:58.000000 rembg-2.0.49/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 00:48:08.546652 rembg-2.0.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-30 00:46:58.000000 rembg-2.0.49/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-30 00:46:58.000000 rembg-2.0.49/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-30 00:46:58.000000 rembg-2.0.49/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:38:53.385582 rembg-2.0.50/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 03:37:37.000000 rembg-2.0.50/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 03:37:37.000000 rembg-2.0.50/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-13 03:38:53.385582 rembg-2.0.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-13 03:37:37.000000 rembg-2.0.50/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-13 03:37:37.000000 rembg-2.0.50/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:38:53.385582 rembg-2.0.50/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 03:38:53.385582 rembg-2.0.50/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:38:53.385582 rembg-2.0.50/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:38:53.385582 rembg-2.0.50/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/u2net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-13 03:37:37.000000 rembg-2.0.50/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:38:53.381582 rembg-2.0.50/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-13 03:38:53.000000 rembg-2.0.50/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-13 03:38:53.000000 rembg-2.0.50/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:38:53.000000 rembg-2.0.50/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 03:38:53.000000 rembg-2.0.50/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 03:38:53.000000 rembg-2.0.50/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 03:38:53.000000 rembg-2.0.50/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 03:38:53.385582 rembg-2.0.50/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-13 03:37:37.000000 rembg-2.0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:38:53.385582 rembg-2.0.50/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-13 03:37:37.000000 rembg-2.0.50/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-13 03:37:37.000000 rembg-2.0.50/versioneer.py
```

### Comparing `rembg-2.0.49/LICENSE.txt` & `rembg-2.0.50/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/PKG-INFO` & `rembg-2.0.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.49
+Version: 2.0.50
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.49/README.md` & `rembg-2.0.50/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/bg.py` & `rembg-2.0.50/rembg/bg.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,14 +70,20 @@
     cutout = np.clip(cutout * 255, 0, 255).astype(np.uint8)
     cutout = Image.fromarray(cutout)
 
     return cutout
 
 
 def naive_cutout(img: PILImage, mask: PILImage) -> PILImage:
+    empty = Image.new("RGBA", (img.size), 0)
+    cutout = Image.composite(img, empty, mask)
+    return cutout
+
+
+def putalpha_cutout(img: PILImage, mask: PILImage) -> PILImage:
     img.putalpha(mask)
     return img
 
 
 def get_concat_v_multi(imgs: List[PILImage]) -> PILImage:
     pivot = imgs.pop(0)
     for im in imgs:
@@ -143,14 +149,16 @@
         img = Image.open(io.BytesIO(data))
     elif isinstance(data, np.ndarray):
         return_type = ReturnType.NDARRAY
         img = Image.fromarray(data)
     else:
         raise ValueError("Input type {} is not supported.".format(type(data)))
 
+    putalpha = kwargs.pop("putalpha", False)
+
     # Fix image orientation
     img = fix_image_orientation(img)
 
     if session is None:
         session = new_session("u2net", *args, **kwargs)
 
     masks = session.predict(img, *args, **kwargs)
@@ -169,18 +177,23 @@
                     img,
                     mask,
                     alpha_matting_foreground_threshold,
                     alpha_matting_background_threshold,
                     alpha_matting_erode_size,
                 )
             except ValueError:
-                cutout = naive_cutout(img, mask)
-
+                if putalpha:
+                    cutout = putalpha_cutout(img, mask)
+                else:
+                    cutout = naive_cutout(img, mask)
         else:
-            cutout = naive_cutout(img, mask)
+            if putalpha:
+                cutout = putalpha_cutout(img, mask)
+            else:
+                cutout = naive_cutout(img, mask)
 
         cutouts.append(cutout)
 
     cutout = img
     if len(cutouts) > 0:
         cutout = get_concat_v_multi(cutouts)
```

### Comparing `rembg-2.0.49/rembg/cli.py` & `rembg-2.0.50/rembg/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,16 @@
                     exit(1)
 
     import click
 
     from . import _version
     from .commands import command_functions
 
-    @click.group()
+    @click.group()  # type: ignore
     @click.version_option(version=_version.get_versions()["version"])
     def _main() -> None:
         pass
 
     for command in command_functions:
-        _main.add_command(command)
+        _main.add_command(command)  # type: ignore
 
-    _main()
+    _main()  # type: ignore
```

### Comparing `rembg-2.0.49/rembg/commands/b_command.py` & `rembg-2.0.50/rembg/commands/b_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from PIL import Image
 
 from ..bg import remove
 from ..session_factory import new_session
 from ..sessions import sessions_names
 
 
-@click.command(
+@click.command(  # type: ignore
     name="b",
     help="for a byte stream as input",
 )
 @click.option(
     "-m",
     "--model",
     default="u2net",
```

### Comparing `rembg-2.0.49/rembg/commands/i_command.py` & `rembg-2.0.50/rembg/commands/i_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import click
 
 from ..bg import remove
 from ..session_factory import new_session
 from ..sessions import sessions_names
 
 
-@click.command(
+@click.command(  # type: ignore
     name="i",
     help="for a file as input",
 )
 @click.option(
     "-m",
     "--model",
     default="u2net",
```

### Comparing `rembg-2.0.49/rembg/commands/p_command.py` & `rembg-2.0.50/rembg/commands/p_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from watchdog.observers import Observer
 
 from ..bg import remove
 from ..session_factory import new_session
 from ..sessions import sessions_names
 
 
-@click.command(
+@click.command(  # type: ignore
     name="p",
     help="for a folder as input",
 )
 @click.option(
     "-m",
     "--model",
     default="u2net",
```

### Comparing `rembg-2.0.49/rembg/commands/s_command.py` & `rembg-2.0.50/rembg/commands/s_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .._version import get_versions
 from ..bg import remove
 from ..session_factory import new_session
 from ..sessions import sessions_names
 from ..sessions.base import BaseSession
 
 
-@click.command(
+@click.command(  # type: ignore
     name="s",
     help="for a http server",
 )
 @click.option(
     "-p",
     "--port",
     default=5000,
```

### Comparing `rembg-2.0.49/rembg/session_factory.py` & `rembg-2.0.50/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/__init__.py` & `rembg-2.0.50/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/base.py` & `rembg-2.0.50/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/dis_anime.py` & `rembg-2.0.50/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/dis_general_use.py` & `rembg-2.0.50/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/sam.py` & `rembg-2.0.50/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/silueta.py` & `rembg-2.0.50/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/u2net.py` & `rembg-2.0.50/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.50/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/u2net_custom.py` & `rembg-2.0.50/rembg/sessions/u2net_custom.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.50/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg/sessions/u2netp.py` & `rembg-2.0.50/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/rembg.egg-info/PKG-INFO` & `rembg-2.0.50/rembg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.49
+Version: 2.0.50
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.49/rembg.egg-info/SOURCES.txt` & `rembg-2.0.50/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/setup.py` & `rembg-2.0.50/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/tests/test_remove.py` & `rembg-2.0.50/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.49/versioneer.py` & `rembg-2.0.50/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/click_extra-4.6.0.tar.gz` & `tmp/click_extra-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.6.0.tar", max compression
+gzip compressed data, was "click_extra-4.6.1.tar", max compression
```

## Comparing `click_extra-4.6.0.tar` & `click_extra-4.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6104 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/__init__.py
--rw-r--r--   0        0        0    30238 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/colorize.py
--rw-r--r--   0        0        0    16715 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/commands.py
--rw-r--r--   0        0        0    16405 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/config.py
--rw-r--r--   0        0        0     4069 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/decorators.py
--rw-r--r--   0        0        0     6211 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/docs_update.py
--rw-r--r--   0        0        0    11805 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/logging.py
--rw-r--r--   0        0        0    25392 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/parameters.py
--rw-r--r--   0        0        0    17118 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/py.typed
--rw-r--r--   0        0        0     7676 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/pygments.py
--rw-r--r--   0        0        0     4969 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/sphinx.py
--rw-r--r--   0        0        0     5969 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/tabulate.py
--rw-r--r--   0        0        0     2542 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/testing.py
--rw-r--r--   0        0        0      770 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    11504 2023-07-12 16:24:52.178848 click_extra-4.6.0/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    18365 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    15075 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    17059 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7354 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    18184 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0    10884 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8396 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14491 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3165 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8259 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3551 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     6359 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2544 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/timer.py
--rw-r--r--   0        0        0    10995 2023-07-12 16:24:52.182848 click_extra-4.6.0/click_extra/version.py
--rw-r--r--   0        0        0     7584 2023-07-12 16:24:52.186848 click_extra-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     6631 2023-07-12 16:24:52.186848 click_extra-4.6.0/readme.md
--rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 click_extra-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     6104 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/__init__.py
+-rw-r--r--   0        0        0    30238 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/colorize.py
+-rw-r--r--   0        0        0    16715 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/commands.py
+-rw-r--r--   0        0        0    16405 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/config.py
+-rw-r--r--   0        0        0     4069 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/decorators.py
+-rw-r--r--   0        0        0     6211 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11805 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/logging.py
+-rw-r--r--   0        0        0    25392 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/parameters.py
+-rw-r--r--   0        0        0    17118 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/py.typed
+-rw-r--r--   0        0        0     7676 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/pygments.py
+-rw-r--r--   0        0        0     4969 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5969 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2542 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    11504 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    18365 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    15075 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    17059 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7354 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    18184 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0    10884 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8396 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14491 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3165 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8259 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3551 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     6359 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2544 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/timer.py
+-rw-r--r--   0        0        0    11757 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/version.py
+-rw-r--r--   0        0        0     7584 2023-07-13 15:33:32.402569 click_extra-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6631 2023-07-13 15:33:32.402569 click_extra-4.6.1/readme.md
+-rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 click_extra-4.6.1/PKG-INFO
```

### Comparing `click_extra-4.6.0/click_extra/__init__.py` & `click_extra-4.6.1/click_extra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.6.0"
+__version__ = "4.6.1"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
```

### Comparing `click_extra-4.6.0/click_extra/colorize.py` & `click_extra-4.6.1/click_extra/colorize.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/commands.py` & `click_extra-4.6.1/click_extra/commands.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/config.py` & `click_extra-4.6.1/click_extra/config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/decorators.py` & `click_extra-4.6.1/click_extra/decorators.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/docs_update.py` & `click_extra-4.6.1/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/logging.py` & `click_extra-4.6.1/click_extra/logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/parameters.py` & `click_extra-4.6.1/click_extra/parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/platforms.py` & `click_extra-4.6.1/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/pygments.py` & `click_extra-4.6.1/click_extra/pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/sphinx.py` & `click_extra-4.6.1/click_extra/sphinx.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tabulate.py` & `click_extra-4.6.1/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/telemetry.py` & `click_extra-4.6.1/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/testing.py` & `click_extra-4.6.1/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/__init__.py` & `click_extra-4.6.1/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/conftest.py` & `click_extra-4.6.1/click_extra/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_colorize.py` & `click_extra-4.6.1/click_extra/tests/test_colorize.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_commands.py` & `click_extra-4.6.1/click_extra/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_config.py` & `click_extra-4.6.1/click_extra/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_logging.py` & `click_extra-4.6.1/click_extra/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_parameters.py` & `click_extra-4.6.1/click_extra/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_platforms.py` & `click_extra-4.6.1/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_pygments.py` & `click_extra-4.6.1/click_extra/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_tabulate.py` & `click_extra-4.6.1/click_extra/tests/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_telemetry.py` & `click_extra-4.6.1/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_testing.py` & `click_extra-4.6.1/click_extra/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_timer.py` & `click_extra-4.6.1/click_extra/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/tests/test_version.py` & `click_extra-4.6.1/click_extra/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/timer.py` & `click_extra-4.6.1/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/click_extra/version.py` & `click_extra-4.6.1/click_extra/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Gather CLI metadata and print them."""
 
 from __future__ import annotations
 
 import inspect
+import logging
 import re
 import warnings
 from functools import cached_property
 from gettext import gettext as _
 from importlib import metadata
 from typing import TYPE_CHECKING, cast
 
+import click
 from boltons.ecoutils import get_profile
 
 from . import Context, Parameter, Style, echo, get_current_context
 from .colorize import default_theme
 from .parameters import ExtraOption
 
 if TYPE_CHECKING:
@@ -126,51 +128,66 @@
             **kwargs,
         )
 
     @cached_property
     def package_name(self) -> str:
         """Try to guess the package name.
 
-        Inspects the stack frames to find the exact name of the installed package.
+        Inspects the execution stack frames to find the package in which the user's CLI
+        is implemented.
         """
-        package_name: str | None = None
+        # Keep a list of all frames inspected for debugging.
+        frame_chain: list[tuple[str, str]] = []
 
-        frame = inspect.currentframe()
+        # Move back up the execution stack.
+        package_name: str | None = None
+        for frame_info in inspect.stack():
+            frame = frame_info.frame
 
-        f_back = None
-        if frame is not None:
-            # Get back one frame.
-            f_back = frame.f_back
-            if f_back is not None:
-                f_class = f_back.f_locals["self"].__class__
-                f_source = f"{f_class.__module__}.{f_class.__name__}"
-                # Skip the intermediate frame added by the `@cached_property` decorator.
-                if f_source == "functools.cached_property":
-                    # Get back 2 frames: i.e. the frame before the decorator.
-                    f_back = f_back.f_back
+            # Get the current package name from the frame's globals.
+            frame_name = frame.f_globals["__name__"]
 
-        f_globals = f_back.f_globals if f_back is not None else None
+            # Keep track of the inspected frames.
+            frame_chain.append((frame_name, frame_info.function))
 
-        # Break reference cycle
-        # https://docs.python.org/3/library/inspect.html#the-interpreter-stack
-        del frame
+            # Stop at the invoke() function of any CliRunner class, which is used for
+            # testing.
+            if frame_info.function == "invoke" and isinstance(
+                frame.f_locals.get("self"),
+                click.testing.CliRunner,
+            ):
+                pass
+
+            # Skip the intermediate frames added by the `@cached_property` decorator
+            # and the Click ecosystem.
+            elif frame_name.startswith(("functools", "click_extra", "cloup", "click")):
+                continue
 
-        if f_globals is not None:
-            package_name = f_globals.get("__name__")
+            # We found the frame where the CLI is implemented.
+            package_name = frame_name.split(".")[0]
 
+            # Re-interpret the package name if it defined as `__main__` entry-point.
             if package_name == "__main__":
-                package_name = f_globals.get("__package__")
+                package_name = frame.f_globals.get("__package__")
+                if package_name:
+                    package_name = package_name.split(".")[0]
 
-            if package_name:
-                package_name = package_name.partition(".")[0]
+            break
+
+        # Break reference cycle
+        # https://docs.python.org/3/library/inspect.html#the-interpreter-stack
+        del frame
 
         if not package_name:
+            logger = logging.getLogger("click_extra")
+            for counter, (p_name, f_name) in enumerate(frame_chain):
+                logger.debug(f"Inspected frame #{counter}: {p_name}, {f_name}")
             msg = (
-                "Could not determine the package name automatically. Try passing "
-                "'package_name' instead."
+                "Could not determine the package name automatically from the frame "
+                "stack. Try passing 'package_name' instead."
             )
             raise RuntimeError(msg)
 
         return package_name
 
     @cached_property
     def version(self) -> str:
```

### Comparing `click_extra-4.6.0/pyproject.toml` & `click_extra-4.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.6.0"
+version = "4.6.1"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -182,15 +182,15 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.6.0"
+current_version = "4.6.1"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./click_extra/__init__.py"
 
 [[tool.bumpversion.files]]
 filename = "./pyproject.toml"
```

### Comparing `click_extra-4.6.0/readme.md` & `click_extra-4.6.1/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.0/PKG-INFO` & `click_extra-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.6.0
+Version: 4.6.1
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.6.0 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.6.1 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
```


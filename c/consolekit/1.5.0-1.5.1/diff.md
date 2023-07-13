# Comparing `tmp/consolekit-1.5.0.tar.gz` & `tmp/consolekit-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolekit-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "consolekit-1.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `consolekit-1.5.0.tar` & `consolekit-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-06-29 15:57:01.811913 consolekit-1.5.0/LICENSE
--rw-r--r--   0        0        0     5471 2023-06-29 15:57:01.811913 consolekit-1.5.0/README.rst
--rw-r--r--   0        0        0     4832 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/__init__.py
--rw-r--r--   0        0        0     1488 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/__init__.pyi
--rw-r--r--   0        0        0     1507 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/_types.py
--rw-r--r--   0        0        0    13518 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/commands.py
--rw-r--r--   0        0        0    11911 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/input.py
--rw-r--r--   0        0        0    15750 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/options.py
--rw-r--r--   0        0        0        0 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/py.typed
--rw-r--r--   0        0        0    16739 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/terminal_colours.py
--rw-r--r--   0        0        0     6084 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/terminal_colours.pyi
--rw-r--r--   0        0        0     8778 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/testing.py
--rw-r--r--   0        0        0     6801 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/tracebacks.py
--rw-r--r--   0        0        0    13859 2023-06-29 15:57:01.811913 consolekit-1.5.0/consolekit/utils.py
--rw-r--r--   0        0        0     5222 2023-06-29 15:57:01.815913 consolekit-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     7651 1970-01-01 00:00:00.000000 consolekit-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 21:19:57.842867 consolekit-1.5.1/LICENSE
+-rw-r--r--   0        0        0     5471 2023-07-13 21:19:57.842867 consolekit-1.5.1/README.rst
+-rw-r--r--   0        0        0     4832 2023-07-13 21:19:57.842867 consolekit-1.5.1/consolekit/__init__.py
+-rw-r--r--   0        0        0     1488 2023-07-13 21:19:57.842867 consolekit-1.5.1/consolekit/__init__.pyi
+-rw-r--r--   0        0        0     1507 2023-07-13 21:19:57.842867 consolekit-1.5.1/consolekit/_types.py
+-rw-r--r--   0        0        0    13518 2023-07-13 21:19:57.842867 consolekit-1.5.1/consolekit/commands.py
+-rw-r--r--   0        0        0    11911 2023-07-13 21:19:57.846867 consolekit-1.5.1/consolekit/input.py
+-rw-r--r--   0        0        0    16040 2023-07-13 21:19:57.846867 consolekit-1.5.1/consolekit/options.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:19:57.850867 consolekit-1.5.1/consolekit/py.typed
+-rw-r--r--   0        0        0    16739 2023-07-13 21:19:57.850867 consolekit-1.5.1/consolekit/terminal_colours.py
+-rw-r--r--   0        0        0     6084 2023-07-13 21:19:57.850867 consolekit-1.5.1/consolekit/terminal_colours.pyi
+-rw-r--r--   0        0        0     8778 2023-07-13 21:19:57.850867 consolekit-1.5.1/consolekit/testing.py
+-rw-r--r--   0        0        0     6801 2023-07-13 21:19:57.850867 consolekit-1.5.1/consolekit/tracebacks.py
+-rw-r--r--   0        0        0    13859 2023-07-13 21:19:57.850867 consolekit-1.5.1/consolekit/utils.py
+-rw-r--r--   0        0        0     5222 2023-07-13 21:19:57.850867 consolekit-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7651 1970-01-01 00:00:00.000000 consolekit-1.5.1/PKG-INFO
```

### Comparing `consolekit-1.5.0/LICENSE` & `consolekit-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/README.rst` & `consolekit-1.5.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/consolekit
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.5.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.5.1
 	:target: https://github.com/domdfcoding/consolekit/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/commit/master
 	:alt: GitHub last commit
```

### Comparing `consolekit-1.5.0/consolekit/__init__.py` & `consolekit-1.5.1/consolekit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from consolekit.options import _Option
 
 # pylint: enable=redefined-builtin
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "1.5.0"
+__version__: str = "1.5.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 if not bool(getattr(sys, "ps1", sys.flags.interactive)):  # pragma: no cover
 	try:
 		# stdlib
 		import readline
 		readline.set_history_length(0)
```

### Comparing `consolekit-1.5.0/consolekit/__init__.pyi` & `consolekit-1.5.1/consolekit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/_types.py` & `consolekit-1.5.1/consolekit/_types.py`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/commands.py` & `consolekit-1.5.1/consolekit/commands.py`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/input.py` & `consolekit-1.5.1/consolekit/input.py`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/options.py` & `consolekit-1.5.1/consolekit/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -440,14 +440,25 @@
 			elif value in ("()", str(self.default)) or not value:
 				return self.default  # type: ignore[return-value]
 			else:
 				return self.type_cast_value(ctx, value)
 		else:
 			return None
 
+	if int(click.__version__.split('.')[0]) == 7:  # pragma: nocover
+
+		def get_default(self, ctx):  # noqa: MAN001,MAN002,D102
+			if callable(self.default):
+				rv = self.default()
+			else:
+				rv = self.default
+
+			ret = tuple(self.type(x or (), self, ctx) for x in rv or ())
+			return ret
+
 
 class _Option(click.Option):
 
 	def prompt_for_value(self, ctx: click.Context):  # noqa: MAN002
 		"""
 		This is an alternative flow that can be activated in the full value processing if a value does not exist.
```

### Comparing `consolekit-1.5.0/consolekit/terminal_colours.py` & `consolekit-1.5.1/consolekit/terminal_colours.py`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/terminal_colours.pyi` & `consolekit-1.5.1/consolekit/terminal_colours.pyi`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/testing.py` & `consolekit-1.5.1/consolekit/testing.py`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/tracebacks.py` & `consolekit-1.5.1/consolekit/tracebacks.py`

 * *Files identical despite different names*

### Comparing `consolekit-1.5.0/consolekit/utils.py` & `consolekit-1.5.1/consolekit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 		"hidden_cursor",
 		"long_echo",
 		)
 
 _deprecator = deprecation_alias.deprecated(
 		deprecated_in="1.0.0",
 		removed_in="2.0.0",
-		current_version="1.5.0",
+		current_version="1.5.1",
 		details="Import from consolekit.tracebacks instead."
 		)
 
 handle_tracebacks = _deprecator(tracebacks.handle_tracebacks)
 traceback_handler = _deprecator(tracebacks.traceback_handler)
```

### Comparing `consolekit-1.5.0/pyproject.toml` & `consolekit-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "flit-core<4,>=3.2",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "consolekit"
-version = "1.5.0"
+version = "1.5.1"
 description = "Additional utilities for click."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "click", "terminal",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
```

### Comparing `consolekit-1.5.0/PKG-INFO` & `consolekit-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolekit
-Version: 1.5.0
+Version: 1.5.1
 Summary: Additional utilities for click.
 Keywords: click,terminal
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -143,15 +143,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/consolekit
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.5.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/consolekit/v1.5.1
 	:target: https://github.com/domdfcoding/consolekit/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/consolekit
 	:target: https://github.com/domdfcoding/consolekit/commit/master
 	:alt: GitHub last commit
```


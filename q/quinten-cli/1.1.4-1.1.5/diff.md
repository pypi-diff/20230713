# Comparing `tmp/quinten-cli-1.1.4.tar.gz` & `tmp/quinten-cli-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quinten-cli-1.1.4.tar", last modified: Sat May 20 19:44:00 2023, max compression
+gzip compressed data, was "quinten-cli-1.1.5.tar", last modified: Thu Jul 13 10:21:49 2023, max compression
```

## Comparing `quinten-cli-1.1.4.tar` & `quinten-cli-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/cli/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/env.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/input_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/install.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/output_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1526 2023-05-20 19:43:16.000000 quinten-cli-1.1.4/cli/progress.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     5097 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/run.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/status.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-05-20 19:37:43.000000 quinten-cli-1.1.4/pyproject.toml
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/quinten_cli.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      418 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/entry_points.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/top_level.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/setup.cfg
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/tests/test_api.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1249 2023-05-20 19:37:23.000000 quinten-cli-1.1.4/tests/test_progress_ui.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.950682 quinten-cli-1.1.5/cli/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/env.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/input_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/install.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/output_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1526 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/progress.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     5158 2023-07-13 10:21:37.000000 quinten-cli-1.1.5/cli/run.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/status.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-07-13 10:21:18.000000 quinten-cli-1.1.5/pyproject.toml
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/quinten_cli.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      418 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/top_level.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/setup.cfg
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/tests/test_api.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1249 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/tests/test_progress_ui.py
```

### Comparing `quinten-cli-1.1.4/LICENSE` & `quinten-cli-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.4/PKG-INFO` & `quinten-cli-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.4
+Version: 1.1.5
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.4/cli/__init__.py` & `quinten-cli-1.1.5/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.4/cli/input_interface.py` & `quinten-cli-1.1.5/cli/input_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.4/cli/install.py` & `quinten-cli-1.1.5/cli/install.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.4/cli/output_interface.py` & `quinten-cli-1.1.5/cli/output_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.4/cli/progress.py` & `quinten-cli-1.1.5/cli/progress.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.4/cli/run.py` & `quinten-cli-1.1.5/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,19 @@
     wait=True,
     console=False,
     text=True,
     check=True,
     shell=False,
     capture_output_tty=False,
     title=None,
+    verbose_errors=True,
     **kwargs,
 ) -> str | subprocess.CompletedProcess:
-    """
-    tty: also works for special outputs that clear the output and move the cursor
+    """Tty: also works for special outputs that clear the output and move the
+    cursor.
     """
     args = prepare_args(args, command=shell or console, root=root)
 
     if console:
         run("activate_window Konsole", check=False)
         wait = False  # avoid blocking if console not opened yet
         if title is not None:
@@ -84,37 +85,38 @@
         # needed for non-login scripts to be able to activate console
         if "DISPLAY" not in os.environ:
             os.environ["DISPLAY"] = ":0.0"
 
     if not wait:
         kwargs["stdout"] = kwargs["stderr"] = subprocess.DEVNULL
 
-    try:
-        if capture_output_tty:
-            import tempfile  # noqa: autoimport
-
-            import pexpect  # noqa: autoimport
-
-            with tempfile.TemporaryFile() as tmp:
-                child = pexpect.spawn(args[0], [*args[1:]], timeout=None, logfile=tmp)
-                if "capture_output" in kwargs:
-                    child.expect(pexpect.EOF)
-                else:
-                    child.interact()
-                tmp.seek(0)
-                res = tmp.read().decode()
-        else:
+    if capture_output_tty:
+        import tempfile  # noqa: autoimport
+
+        import pexpect  # noqa: autoimport
+
+        with tempfile.TemporaryFile() as tmp:
+            child = pexpect.spawn(args[0], [*args[1:]], timeout=None, logfile=tmp)
+            if "capture_output" in kwargs:
+                child.expect(pexpect.EOF)
+            else:
+                child.interact()
+            tmp.seek(0)
+            res = tmp.read().decode()
+    else:
+        try:
             res = (
                 subprocess.run(args, text=text, check=check, shell=shell, **kwargs)
                 if wait
                 else subprocess.Popen(args, shell=shell, **kwargs)
             )
-    except subprocess.CalledProcessError as e:
-        raise Exception(e.stderr or e)  # more verbose errors
-
+        except subprocess.CalledProcessError as error:
+            if verbose_errors:
+                error = Exception(error.stderr or error)  # more verbose errors
+            raise error
     return res
 
 
 def prepare_args(args, command=False, root=False):
     args = [str(arg) for arg in iterate_args(args, command)]
     if command:
         subargs_str = shlex.join(args[1:])
```

### Comparing `quinten-cli-1.1.4/pyproject.toml` & `quinten-cli-1.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "quinten-cli"
-version = "1.1.4"
+version = "1.1.5"
 description = ""
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "python-dotenv",
```

### Comparing `quinten-cli-1.1.4/quinten_cli.egg-info/PKG-INFO` & `quinten-cli-1.1.5/quinten_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.4
+Version: 1.1.5
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.4/tests/test_progress_ui.py` & `quinten-cli-1.1.5/tests/test_progress_ui.py`

 * *Files identical despite different names*


# Comparing `tmp/ssh_terminal_manager-0.4.0.tar.gz` & `tmp/ssh_terminal_manager-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.4.0.tar", last modified: Thu Jul 13 07:01:07 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.5.0.tar", last modified: Thu Jul 13 09:58:08 2023, max compression
```

## Comparing `ssh_terminal_manager-0.4.0.tar` & `ssh_terminal_manager-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.4.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.4.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      797 2023-07-13 07:00:04.000000 ssh_terminal_manager-0.4.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.459457 ssh_terminal_manager-0.4.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.459457 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8400 2023-07-12 10:33:18.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      383 2023-07-12 08:15:06.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.174756 ssh_terminal_manager-0.5.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.5.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-13 09:58:08.170756 ssh_terminal_manager-0.5.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.5.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-13 09:53:35.000000 ssh_terminal_manager-0.5.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 09:58:08.174756 ssh_terminal_manager-0.5.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.166756 ssh_terminal_manager-0.5.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.170756 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8398 2023-07-13 09:29:07.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      383 2023-07-13 07:22:57.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.170756 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.4.0/LICENSE` & `ssh_terminal_manager-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.4.0/pyproject.toml` & `ssh_terminal_manager-0.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
-description = "Control and monitor devices with SSH terminal commands"
+description = "Use terminal commands to control and monitor remote devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
@@ -20,14 +20,14 @@
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.4.0",
+  "terminal-manager >= 0.5.0",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.on_change = Event()
 
     def update(self, name, value) -> None:
         if getattr(self, name) == value:
             return
 
         setattr(self, name, value)
-        self._manager.logger.debug("%s: %s is %s", self._manager.name, name, value)
+        self._manager.logger.info("%s: %s is %s", self._manager.name, name, value)
         self.on_change.notify(self)
 
 
 class SSHManager(Manager):
     def __init__(
         self,
         host: str,
@@ -236,15 +236,15 @@
             host = await icmplib.async_ping(
                 self.host,
                 count=1,
                 timeout=self.ping_timeout,
                 privileged=False,
             )
         except Exception as exc:  # pylint: disable=broad-except
-            self.logger.debug("%s: Ping request failed (%s)", self.name, exc)
+            self.logger.info("%s: Ping request failed (%s)", self.name, exc)
             self.state.update(ONLINE, False)
         else:
             self.state.update(ONLINE, host.is_alive)
 
         if not self.state.online:
             if raise_errors:
                 raise OfflineError("Host is offline")
```


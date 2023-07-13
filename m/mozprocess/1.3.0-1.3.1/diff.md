# Comparing `tmp/mozprocess-1.3.0.tar.gz` & `tmp/mozprocess-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozprocess-1.3.0.tar", last modified: Fri Jun  4 19:59:18 2021, max compression
+gzip compressed data, was "dist/mozprocess-1.3.1.tar", last modified: Thu Jul 13 17:01:31 2023, max compression
```

## Comparing `mozprocess-1.3.0.tar` & `mozprocess-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 19:59:18.000000 mozprocess-1.3.0/
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    55346 2021-05-19 09:48:19.000000 mozprocess-1.3.0/mozprocess/processhandler.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    16785 2021-01-11 15:46:26.000000 mozprocess-1.3.0/mozprocess/winprocess.py
--rw-r--r--   0 jgraham   (1000) jgraham   (1000)      285 2018-10-20 23:26:05.000000 mozprocess-1.3.0/mozprocess/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5212 2021-01-11 15:46:26.000000 mozprocess-1.3.0/mozprocess/qijo.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1309 2021-06-04 09:37:16.000000 mozprocess-1.3.0/setup.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      785 2021-06-04 19:59:18.000000 mozprocess-1.3.0/PKG-INFO
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       67 2021-06-04 19:59:18.000000 mozprocess-1.3.0/setup.cfg
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess.egg-info/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       37 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess.egg-info/entry_points.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2021-06-04 19:58:44.000000 mozprocess-1.3.0/mozprocess.egg-info/not-zip-safe
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        8 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess.egg-info/requires.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       11 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess.egg-info/top_level.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      785 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess.egg-info/PKG-INFO
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      353 2021-06-04 19:59:18.000000 mozprocess-1.3.0/mozprocess.egg-info/SOURCES.txt
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-13 17:01:31.000000 mozprocess-1.3.1/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      774 2023-07-13 17:01:31.000000 mozprocess-1.3.1/PKG-INFO
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      245 2023-07-13 00:32:46.000000 mozprocess-1.3.1/mozprocess/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    52852 2023-07-13 00:32:46.000000 mozprocess-1.3.1/mozprocess/processhandler.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     5172 2023-03-10 23:28:57.000000 mozprocess-1.3.1/mozprocess/qijo.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    16753 2023-03-10 23:28:57.000000 mozprocess-1.3.1/mozprocess/winprocess.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      774 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      353 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       37 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/entry_points.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/not-zip-safe
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        8 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/requires.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       11 2023-07-13 17:01:31.000000 mozprocess-1.3.1/mozprocess.egg-info/top_level.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-07-13 17:01:31.000000 mozprocess-1.3.1/setup.cfg
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1269 2023-07-13 16:46:47.000000 mozprocess-1.3.1/setup.py
```

### Comparing `mozprocess-1.3.0/mozprocess/processhandler.py` & `mozprocess-1.3.1/mozprocess/processhandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,34 +5,32 @@
 # mozprocess is typically used as an alternative to the python subprocess module.
 # It has been used in many Mozilla test harnesses with some success -- but also
 # with on-going concerns, especially regarding reliability and exception handling.
 #
 # New code should try to use the standard subprocess module, and only use
 # mozprocess if absolutely necessary.
 
-from __future__ import absolute_import, print_function, unicode_literals
-
 import codecs
 import errno
 import io
 import os
 import signal
 import subprocess
 import sys
 import threading
+import time
 import traceback
 from datetime import datetime
 
 import six
-import time
 
 if six.PY2:
-    from Queue import Queue, Empty  # Python 2
+    from Queue import Empty, Queue  # Python 2
 else:
-    from queue import Queue, Empty  # Python 3
+    from queue import Empty, Queue  # Python 3
 
 __all__ = [
     "ProcessHandlerMixin",
     "ProcessHandler",
     "LogOutput",
     "StoreOutput",
     "StreamOutput",
@@ -44,23 +42,24 @@
 INTERVAL_PROCESS_ALIVE_CHECK = 0.02
 
 # We dont use mozinfo because it is expensive to import, see bug 933558.
 isWin = os.name == "nt"
 isPosix = os.name == "posix"  # includes MacOS X
 
 if isWin:
-    from ctypes import sizeof, addressof, c_ulong, byref, WinError, c_longlong
+    from ctypes import WinError, addressof, byref, c_longlong, c_ulong, sizeof
+
     from . import winprocess
     from .qijo import (
-        JobObjectAssociateCompletionPortInformation,
+        IO_COUNTERS,
         JOBOBJECT_ASSOCIATE_COMPLETION_PORT,
-        JobObjectExtendedLimitInformation,
         JOBOBJECT_BASIC_LIMIT_INFORMATION,
         JOBOBJECT_EXTENDED_LIMIT_INFORMATION,
-        IO_COUNTERS,
+        JobObjectAssociateCompletionPortInformation,
+        JobObjectExtendedLimitInformation,
     )
 
 
 class ProcessHandlerMixin(object):
     """
     A class for launching and manipulating local processes.
 
@@ -122,14 +121,16 @@
             creationflags=0,
             ignore_children=False,
             encoding="utf-8",
         ):
 
             # Parameter for whether or not we should attempt to track child processes
             self._ignore_children = ignore_children
+            self._job = None
+            self._io_port = None
 
             if not self._ignore_children and not isWin:
                 # Set the process group id for linux systems
                 # Sets process group id to the pid of the parent process
                 # NOTE: This prevents you from using preexec_fn and managing
                 #       child processes, TODO: Ideally, find a way around this
                 def setpgidfn():
@@ -286,102 +287,33 @@
             return self.returncode
 
         """ Private Members of Process class """
 
         if isWin:
             # Redefine the execute child so that we can track process groups
             def _execute_child(self, *args_tuple):
-                # workaround for bug 1670130
-                if sys.hexversion >= 0x03090000:  # after 3.9.0
-                    (
-                        args,
-                        executable,
-                        preexec_fn,
-                        close_fds,
-                        pass_fds,
-                        cwd,
-                        env,
-                        startupinfo,
-                        creationflags,
-                        shell,
-                        p2cread,
-                        p2cwrite,
-                        c2pread,
-                        c2pwrite,
-                        errread,
-                        errwrite,
-                        restore_signals,
-                        gid,
-                        gids,
-                        uid,
-                        umask,
-                        start_new_session,
-                    ) = args_tuple
-                elif six.PY3:
-                    (
-                        args,
-                        executable,
-                        preexec_fn,
-                        close_fds,
-                        pass_fds,
-                        cwd,
-                        env,
-                        startupinfo,
-                        creationflags,
-                        shell,
-                        p2cread,
-                        p2cwrite,
-                        c2pread,
-                        c2pwrite,
-                        errread,
-                        errwrite,
-                        restore_signals,
-                        start_new_session,
-                    ) = args_tuple
-                # workaround for bug 950894
-                elif sys.hexversion < 0x02070600:  # prior to 2.7.6
-                    (
-                        args,
-                        executable,
-                        preexec_fn,
-                        close_fds,
-                        cwd,
-                        env,
-                        universal_newlines,
-                        startupinfo,
-                        creationflags,
-                        shell,
-                        p2cread,
-                        p2cwrite,
-                        c2pread,
-                        c2pwrite,
-                        errread,
-                        errwrite,
-                    ) = args_tuple
-                    to_close = set()
-                else:  # 2.7.6 and later
-                    (
-                        args,
-                        executable,
-                        preexec_fn,
-                        close_fds,
-                        cwd,
-                        env,
-                        universal_newlines,
-                        startupinfo,
-                        creationflags,
-                        shell,
-                        to_close,
-                        p2cread,
-                        p2cwrite,
-                        c2pread,
-                        c2pwrite,
-                        errread,
-                        errwrite,
-                    ) = args_tuple
+                (
+                    args,
+                    executable,
+                    preexec_fn,
+                    close_fds,
+                    pass_fds,
+                    cwd,
+                    env,
+                    startupinfo,
+                    creationflags,
+                    shell,
+                    p2cread,
+                    p2cwrite,
+                    c2pread,
+                    c2pwrite,
+                    errread,
+                    errwrite,
+                    *_,
+                ) = args_tuple
                 if not isinstance(args, six.string_types):
                     args = subprocess.list2cmdline(args)
 
                 # Always or in the create new process group
                 creationflags |= winprocess.CREATE_NEW_PROCESS_GROUP
 
                 if startupinfo is None:
@@ -1283,15 +1215,15 @@
     def __init__(self, stream, text=True):
         self.stream = stream
         self.text = text
 
     def __call__(self, line):
         ensure = six.ensure_text if self.text else six.ensure_binary
         try:
-            self.stream.write(ensure(line) + ensure("\n"))
+            self.stream.write(ensure(line, errors="ignore") + ensure("\n"))
         except TypeError:
             print(
                 "HEY! If you're reading this, you're about to encounter a "
                 "type error, probably as a result of a conversion from "
                 "Python 2 to Python 3. This is almost definitely because "
                 "you're trying to write binary data to a text-encoded "
                 "stream, or text data to a binary-encoded stream. Check how "
```

### Comparing `mozprocess-1.3.0/mozprocess/winprocess.py` & `mozprocess-1.3.1/mozprocess/winprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,27 @@
 # INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS.
 # IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, INDIRECT OR
 # CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS
 # OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT,
 # NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-from __future__ import absolute_import, unicode_literals, print_function
-
 import subprocess
 import sys
 from ctypes import (
-    cast,
-    create_unicode_buffer,
+    POINTER,
+    WINFUNCTYPE,
+    Structure,
+    WinError,
     c_ulong,
     c_void_p,
-    POINTER,
+    cast,
+    create_unicode_buffer,
     sizeof,
-    Structure,
     windll,
-    WinError,
-    WINFUNCTYPE,
 )
 from ctypes.wintypes import BOOL, BYTE, DWORD, HANDLE, LPCWSTR, LPWSTR, UINT, WORD
 
 from .qijo import QueryInformationJobObject
 
 LPVOID = c_void_p
 LPBYTE = POINTER(BYTE)
@@ -495,14 +493,15 @@
 WAIT_ABANDONED = 0x0080
 
 # http://msdn.microsoft.com/en-us/library/ms683189%28VS.85%29.aspx
 STILL_ACTIVE = 259
 
 # Used when we terminate a process.
 ERROR_CONTROL_C_EXIT = 0x23C
+ERROR_CONTROL_C_EXIT_DECIMAL = 3221225786
 
 # GetExitCodeProcess()
 
 GetExitCodeProcessProto = WINFUNCTYPE(
     BOOL,
     HANDLE,
     LPDWORD,  # Return type  # hProcess  # lpExitCode
```

### Comparing `mozprocess-1.3.0/mozprocess/qijo.py` & `mozprocess-1.3.1/mozprocess/qijo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from ctypes import (
-    c_void_p,
     POINTER,
-    sizeof,
+    WINFUNCTYPE,
     Structure,
-    windll,
     WinError,
-    WINFUNCTYPE,
     addressof,
     c_size_t,
     c_ulong,
+    c_void_p,
+    sizeof,
+    windll,
 )
 from ctypes.wintypes import BOOL, BYTE, DWORD, HANDLE, LARGE_INTEGER
 
 import six
 
 LPVOID = c_void_p
 LPDWORD = POINTER(DWORD)
```

### Comparing `mozprocess-1.3.0/setup.py` & `mozprocess-1.3.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from setuptools import setup
 
-PACKAGE_VERSION = "1.3.0"
+PACKAGE_VERSION = "1.3.1"
 
 setup(
     name="mozprocess",
     version=PACKAGE_VERSION,
     description="Mozilla-authored process handling",
     long_description="see https://firefox-source-docs.mozilla.org/mozbase/index.html",
     classifiers=[
```

### Comparing `mozprocess-1.3.0/PKG-INFO` & `mozprocess-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mozprocess
-Version: 1.3.0
+Version: 1.3.1
 Summary: Mozilla-authored process handling
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```

### Comparing `mozprocess-1.3.0/mozprocess.egg-info/PKG-INFO` & `mozprocess-1.3.1/mozprocess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mozprocess
-Version: 1.3.0
+Version: 1.3.1
 Summary: Mozilla-authored process handling
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Tools team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
-Description: see https://firefox-source-docs.mozilla.org/mozbase/index.html
 Keywords: mozilla
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+
+see https://firefox-source-docs.mozilla.org/mozbase/index.html
+
```


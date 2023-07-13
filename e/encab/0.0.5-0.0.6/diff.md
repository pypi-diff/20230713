# Comparing `tmp/encab-0.0.5.tar.gz` & `tmp/encab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encab-0.0.5.tar", last modified: Wed Jul 12 07:36:57 2023, max compression
+gzip compressed data, was "encab-0.0.6.tar", last modified: Thu Jul 13 17:57:16 2023, max compression
```

## Comparing `encab-0.0.5.tar` & `encab-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.913200 encab-0.0.5/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.5/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-12 07:36:57.913200 encab-0.0.5/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4299 2023-07-11 14:32:39.000000 encab-0.0.5/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      968 2023-07-12 07:32:46.000000 encab-0.0.5/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-12 07:36:57.913200 encab-0.0.5/setup.cfg
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.905199 encab-0.0.5/src/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.909199 encab-0.0.5/src/encab/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.5/src/encab/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.5/src/encab/__main__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11029 2023-07-12 07:11:39.000000 encab-0.0.5/src/encab/config.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8042 2023-07-12 07:29:23.000000 encab-0.0.5/src/encab/encab.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.913200 encab-0.0.5/src/encab/ext/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.5/src/encab/ext/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.5/src/encab/ext/log_sanitizer.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12061 2023-07-11 09:18:42.000000 encab-0.0.5/src/encab/ext/startup_script.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.5/src/encab/ext/validation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.5/src/encab/extensions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7603 2023-07-11 13:57:15.000000 encab-0.0.5/src/encab/program.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10017 2023-03-02 07:37:32.000000 encab-0.0.5/src/encab/program_state.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3160 2023-01-25 12:22:05.000000 encab-0.0.5/src/encab/programs.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.913200 encab-0.0.5/src/encab.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      526 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.161249 encab-0.0.6/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.6/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-13 17:57:16.157248 encab-0.0.6/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4406 2023-07-13 17:45:41.000000 encab-0.0.6/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-07-13 17:41:31.000000 encab-0.0.6/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-13 17:57:16.161249 encab-0.0.6/setup.cfg
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.149248 encab-0.0.6/src/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.153248 encab-0.0.6/src/encab/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.6/src/encab/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.6/src/encab/__main__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11029 2023-07-12 07:11:39.000000 encab-0.0.6/src/encab/config.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8042 2023-07-13 17:42:02.000000 encab-0.0.6/src/encab/encab.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.157248 encab-0.0.6/src/encab/ext/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.6/src/encab/ext/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.6/src/encab/ext/log_sanitizer.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12061 2023-07-11 09:18:42.000000 encab-0.0.6/src/encab/ext/startup_script.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.6/src/encab/ext/validation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.6/src/encab/extensions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7603 2023-07-11 13:57:15.000000 encab-0.0.6/src/encab/program.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10017 2023-03-02 07:37:32.000000 encab-0.0.6/src/encab/program_state.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3160 2023-01-25 12:22:05.000000 encab-0.0.6/src/encab/programs.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.157248 encab-0.0.6/src/encab.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      526 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/top_level.txt
```

### Comparing `encab-0.0.5/LICENSE` & `encab-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/PKG-INFO` & `encab-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-Metadata-Version: 2.1
-Name: encab
-Version: 0.0.5
-Summary: Docker entrypoint tool
-Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
-Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
-Project-URL: Documentation, https://encab.readthedocs.io
-Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# Encab: A Simple Process Manager
 
-# Encab: A Docker Entrypoint Tool
+**Encab** is a process manager that simplifies running multiple services in a container or from the command line.
 
-**Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
+It's essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
 
 1. Add it as your [Dockerfile Entrypoint][1],
 together with the encab configuration file `encab.yml`,
 
 ```dockerfile
    ...
@@ -39,15 +26,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.3
+   INFO  encab: encab 0.0.6
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -73,15 +60,15 @@
 
 ## Installation
 
 ### Install locally
 
 #### Prerequisites
 
-- [Python](https://www.python.org/) Version >= 3.7
+- [Python](https://www.python.org/) Version >= 3.9
 - activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
 
 ```sh
    pip install -U encab
 ```
 
 #### Run locally
@@ -102,15 +89,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.3
+INFO  encab: encab 0.0.6
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -173,15 +160,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.3
+   INFO  encab: encab 0.0.6
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.5/README.md` & `encab-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,27 @@
-# Encab: A Docker Entrypoint Tool
+Metadata-Version: 2.1
+Name: encab
+Version: 0.0.6
+Summary: Process manager
+Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
+Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
+Project-URL: Documentation, https://encab.readthedocs.io
+Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-**Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
+# Encab: A Simple Process Manager
+
+**Encab** is a process manager that simplifies running multiple services in a container or from the command line.
+
+It's essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
 
 1. Add it as your [Dockerfile Entrypoint][1],
 together with the encab configuration file `encab.yml`,
 
 ```dockerfile
    ...
@@ -24,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.3
+   INFO  encab: encab 0.0.6
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -58,15 +75,15 @@
 
 ## Installation
 
 ### Install locally
 
 #### Prerequisites
 
-- [Python](https://www.python.org/) Version >= 3.7
+- [Python](https://www.python.org/) Version >= 3.9
 - activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
 
 ```sh
    pip install -U encab
 ```
 
 #### Run locally
@@ -87,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.3
+INFO  encab: encab 0.0.6
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -158,15 +175,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.3
+   INFO  encab: encab 0.0.6
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.5/pyproject.toml` & `encab-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=63.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encab"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Sebastian Kuebeck", email="sebastian.kuebeck@encab.io" },
 ]
-description = "Docker entrypoint tool"
+description = "Process manager"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `encab-0.0.5/src/encab/config.py` & `encab-0.0.6/src/encab/config.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab/encab.py` & `encab-0.0.6/src/encab/encab.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     try:
         config, location = load_config(encab_stream)
 
         logger = set_up_logger(config)
 
         extra = {"program": ENCAB}
 
-        logger.info("encab 0.0.5", extra=extra)
+        logger.info("encab 0.0.6", extra=extra)
         logger.info("Using configuration %s", location, extra=extra)
 
         logger.debug(
             "Encab config: %s",
             shorten(str(config), width=127, placeholder="..."),
             extra=extra,
         )
```

### Comparing `encab-0.0.5/src/encab/ext/log_sanitizer.py` & `encab-0.0.6/src/encab/ext/log_sanitizer.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab/ext/startup_script.py` & `encab-0.0.6/src/encab/ext/startup_script.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab/ext/validation.py` & `encab-0.0.6/src/encab/ext/validation.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab/extensions.py` & `encab-0.0.6/src/encab/extensions.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab/program.py` & `encab-0.0.6/src/encab/program.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab/program_state.py` & `encab-0.0.6/src/encab/program_state.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab/programs.py` & `encab-0.0.6/src/encab/programs.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.5/src/encab.egg-info/PKG-INFO` & `encab-0.0.6/src/encab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.5
-Summary: Docker entrypoint tool
+Version: 0.0.6
+Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Encab: A Docker Entrypoint Tool
+# Encab: A Simple Process Manager
 
-**Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
+**Encab** is a process manager that simplifies running multiple services in a container or from the command line.
+
+It's essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
 
 1. Add it as your [Dockerfile Entrypoint][1],
 together with the encab configuration file `encab.yml`,
 
 ```dockerfile
    ...
@@ -39,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.3
+   INFO  encab: encab 0.0.6
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -73,15 +75,15 @@
 
 ## Installation
 
 ### Install locally
 
 #### Prerequisites
 
-- [Python](https://www.python.org/) Version >= 3.7
+- [Python](https://www.python.org/) Version >= 3.9
 - activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
 
 ```sh
    pip install -U encab
 ```
 
 #### Run locally
@@ -102,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.3
+INFO  encab: encab 0.0.6
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -173,15 +175,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.3
+   INFO  encab: encab 0.0.6
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.5/src/encab.egg-info/SOURCES.txt` & `encab-0.0.6/src/encab.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/vernum-3.1.5.tar.gz` & `tmp/vernum-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernum-3.1.5.tar", last modified: Sun Jun 25 03:19:57 2023, max compression
+gzip compressed data, was "vernum-3.2.0.tar", last modified: Thu Jul 13 05:04:04 2023, max compression
```

## Comparing `vernum-3.1.5.tar` & `vernum-3.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:19:57.283413 vernum-3.1.5/
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-25 03:19:25.000000 vernum-3.1.5/.version
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-25 03:19:47.000000 vernum-3.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1647 2023-06-25 03:19:57.283413 vernum-3.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-06-25 03:19:47.000000 vernum-3.1.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-25 03:19:47.000000 vernum-3.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 03:19:57.283413 vernum-3.1.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:19:57.282413 vernum-3.1.5/vernum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 03:19:47.000000 vernum-3.1.5/vernum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-25 03:19:47.000000 vernum-3.1.5/vernum/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2349 2023-06-25 03:19:47.000000 vernum-3.1.5/vernum/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 03:19:57.283413 vernum-3.1.5/vernum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1647 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-25 03:19:57.000000 vernum-3.1.5/vernum.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:04:04.942824 vernum-3.2.0/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-13 05:03:13.000000 vernum-3.2.0/.version
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-13 05:03:56.000000 vernum-3.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-13 05:04:04.942824 vernum-3.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-13 05:03:56.000000 vernum-3.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-13 05:03:56.000000 vernum-3.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 05:04:04.942824 vernum-3.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:04:04.941907 vernum-3.2.0/vernum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 05:03:56.000000 vernum-3.2.0/vernum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-13 05:03:56.000000 vernum-3.2.0/vernum/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-07-13 05:03:56.000000 vernum-3.2.0/vernum/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:04:04.942824 vernum-3.2.0/vernum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-13 05:04:04.000000 vernum-3.2.0/vernum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-13 05:04:04.000000 vernum-3.2.0/vernum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 05:04:04.000000 vernum-3.2.0/vernum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-13 05:04:04.000000 vernum-3.2.0/vernum.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 05:04:04.000000 vernum-3.2.0/vernum.egg-info/top_level.txt
```

### Comparing `vernum-3.1.5/LICENSE` & `vernum-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vernum-3.1.5/PKG-INFO` & `vernum-3.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: vernum
-Version: 3.1.5
+Version: 3.2.0
 Summary: Easy semantic versioning for projects in Git
 Author-email: Steampunk Wizard <vernum@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VerNum
 
 Version numbering and git tagging for project releases
 
+[Watch the video](https://www.youtube.com/watch?v=JD8WdVNv1ac)
+
 ## Installation
 
 Requires Python 3 to run the command; your project can be anything.
 
 ```
 pip3 install vernum
 ```
```

### Comparing `vernum-3.1.5/README.md` & `vernum-3.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # VerNum
 
 Version numbering and git tagging for project releases
 
+[Watch the video](https://www.youtube.com/watch?v=JD8WdVNv1ac)
+
 ## Installation
 
 Requires Python 3 to run the command; your project can be anything.
 
 ```
 pip3 install vernum
 ```
```

### Comparing `vernum-3.1.5/pyproject.toml` & `vernum-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vernum-3.1.5/vernum/handler.py` & `vernum-3.2.0/vernum/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,26 @@
                                     capture_output=True, text=True)
             if result.returncode != 0:
                 raise SystemExit(result.stderr)
             return result.stdout.strip()
 
     def get_previous_version(self):
         branch = self.git("branch --show-current", dry_ok=True)
-        tags = self.git(f"tag --sort=-creatordate --merged {branch}", dry_ok=True)
+        tags = self.git(f"tag --merged {branch}", dry_ok=True)
+        result = (0,0,0)
         for tag in tags.split('\n'):
             if match:=FORMAT.match(tag):
-                return (int(x) for x in match.groups())
+                version = tuple(int(x) for x in match.groups())
+                if version > result:
+                    result = version
+        return result
+                        
 
     def update_version(self, level):
-        major, minor, patch = self.get_previous_version() or (0,0,0)
+        major, minor, patch = self.get_previous_version()
         if level == 'major':
             major += 1
             minor = 0
             patch = 0
         elif level == 'minor':
             minor += 1
             patch = 0
```

### Comparing `vernum-3.1.5/vernum.egg-info/PKG-INFO` & `vernum-3.2.0/vernum.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: vernum
-Version: 3.1.5
+Version: 3.2.0
 Summary: Easy semantic versioning for projects in Git
 Author-email: Steampunk Wizard <vernum@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VerNum
 
 Version numbering and git tagging for project releases
 
+[Watch the video](https://www.youtube.com/watch?v=JD8WdVNv1ac)
+
 ## Installation
 
 Requires Python 3 to run the command; your project can be anything.
 
 ```
 pip3 install vernum
 ```
```


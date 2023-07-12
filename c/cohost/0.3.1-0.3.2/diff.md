# Comparing `tmp/cohost-0.3.1.tar.gz` & `tmp/cohost-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohost-0.3.1.tar", last modified: Tue Jul 11 04:08:09 2023, max compression
+gzip compressed data, was "cohost-0.3.2.tar", last modified: Wed Jul 12 22:54:58 2023, max compression
```

## Comparing `cohost-0.3.1.tar` & `cohost-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 04:07:59.000000 cohost-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-11 04:08:09.369651 cohost-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-11 04:07:59.000000 cohost-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/cohost/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/cohost/models/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-11 04:07:59.000000 cohost-0.3.1/cohost/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:08:09.369651 cohost-0.3.1/cohost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 04:08:09.000000 cohost-0.3.1/cohost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-11 04:07:59.000000 cohost-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:08:09.369651 cohost-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:58.063857 cohost-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 22:54:42.000000 cohost-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-12 22:54:58.063857 cohost-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-12 22:54:42.000000 cohost-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:58.059857 cohost-0.3.2/cohost/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:58.063857 cohost-0.3.2/cohost/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/models/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-12 22:54:42.000000 cohost-0.3.2/cohost/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:58.059857 cohost-0.3.2/cohost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-12 22:54:58.000000 cohost-0.3.2/cohost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-12 22:54:58.000000 cohost-0.3.2/cohost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:54:58.000000 cohost-0.3.2/cohost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 22:54:58.000000 cohost-0.3.2/cohost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 22:54:58.000000 cohost-0.3.2/cohost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-12 22:54:42.000000 cohost-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:54:58.063857 cohost-0.3.2/setup.cfg
```

### Comparing `cohost-0.3.1/LICENSE` & `cohost-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cohost-0.3.1/PKG-INFO` & `cohost-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.3.1
+Version: 0.3.2
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
```

### Comparing `cohost-0.3.1/README.md` & `cohost-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cohost-0.3.1/cohost/models/block.py` & `cohost-0.3.2/cohost/models/block.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.1/cohost/models/notification.py` & `cohost-0.3.2/cohost/models/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         super().__init__(createdAt, fromProject)
         self.toPost = toPost
         self.sharePost = sharePost
         self.transparentShare = transparentShare
 
     def __str__(self) -> str:
         if self.transparentShare:
-            return "{} shared {} with extra | {}".format(
+            return "{} shared {} | {}".format(
                 self.fromProject.handle,
                 self.toPost.postId,
                 self.timestamp
             )
-        return "{} shared {} | {}".format(
+        return "{} shared {} with extra | {}".format(
             self.fromProject.handle,
             self.toPost.postId,
             self.timestamp
         )
 
 
 class Comment(BaseNotification):
@@ -102,14 +102,15 @@
                 sharePostId = notif['sharePostIds'][i]
             unwrapped.append({
                 'type': notif['type'].replace('grouped', '').lower(),
                 'fromProjectId': fromProjectId,
                 'relationshipId': relationshipId,
                 'sharePostId': sharePostId,
                 'createdAt': notif['createdAt'],
+                'toPostId': notif.get('toPostId', None),
                 'transparentShare': notif.get('transparentShare', None)
             })
     return unwrapped
 
 
 def buildFromNotifList(notificationsApiResp: dict, user):
     from cohost.models.comment import Comment as CommentModel
```

### Comparing `cohost-0.3.1/cohost/models/post.py` & `cohost-0.3.2/cohost/models/post.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.1/cohost/models/project.py` & `cohost-0.3.2/cohost/models/project.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.1/cohost/models/user.py` & `cohost-0.3.2/cohost/models/user.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.1/cohost/network.py` & `cohost-0.3.2/cohost/network.py`

 * *Files identical despite different names*

### Comparing `cohost-0.3.1/cohost.egg-info/PKG-INFO` & `cohost-0.3.2/cohost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.3.1
+Version: 0.3.2
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
```

### Comparing `cohost-0.3.1/pyproject.toml` & `cohost-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cohost"
-version = "0.3.1"
+version = "0.3.2"
 description = "Unofficial Python API wrapper for Cohost.org - the fourth website!"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = [ "cohost.org", "cohost", "api" ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```


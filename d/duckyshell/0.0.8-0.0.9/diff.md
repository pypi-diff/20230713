# Comparing `tmp/duckyshell-0.0.8.tar.gz` & `tmp/duckyshell-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckyshell-0.0.8.tar", last modified: Thu Jul 13 09:53:54 2023, max compression
+gzip compressed data, was "duckyshell-0.0.9.tar", last modified: Thu Jul 13 09:55:50 2023, max compression
```

## Comparing `duckyshell-0.0.8.tar` & `duckyshell-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:53:54.107949 duckyshell-0.0.8/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      342 2023-07-13 09:53:54.101773 duckyshell-0.0.8/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.8/README.md
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:53:54.035501 duckyshell-0.0.8/duckyshell.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      342 2023-07-13 09:53:53.000000 duckyshell-0.0.8/duckyshell.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      154 2023-07-13 09:53:53.000000 duckyshell-0.0.8/duckyshell.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-13 09:53:53.000000 duckyshell-0.0.8/duckyshell.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-13 09:53:53.000000 duckyshell-0.0.8/duckyshell.egg-info/top_level.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-13 09:53:54.113478 duckyshell-0.0.8/setup.cfg
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      477 2023-07-13 09:46:30.000000 duckyshell-0.0.8/setup.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:55:50.296183 duckyshell-0.0.9/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      342 2023-07-13 09:55:50.288156 duckyshell-0.0.9/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.9/README.md
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:55:50.224405 duckyshell-0.0.9/duckyshell.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      342 2023-07-13 09:55:49.000000 duckyshell-0.0.9/duckyshell.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      154 2023-07-13 09:55:49.000000 duckyshell-0.0.9/duckyshell.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-13 09:55:49.000000 duckyshell-0.0.9/duckyshell.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-13 09:55:49.000000 duckyshell-0.0.9/duckyshell.egg-info/top_level.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-13 09:55:50.296183 duckyshell-0.0.9/setup.cfg
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      477 2023-07-13 09:55:46.000000 duckyshell-0.0.9/setup.py
```

### Comparing `duckyshell-0.0.8/README.md` & `duckyshell-0.0.9/README.md`

 * *Files identical despite different names*


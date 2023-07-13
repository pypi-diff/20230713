# Comparing `tmp/rx7-3.3.0.tar.gz` & `tmp/rx7-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rx7-3.3.0.tar", last modified: Sat Apr 29 15:54:26 2023, max compression
+gzip compressed data, was "rx7-4.0.0.tar", last modified: Thu Jul 13 20:28:25 2023, max compression
```

## Comparing `rx7-3.3.0.tar` & `rx7-4.0.0.tar`

### file list

```diff
@@ -1,18 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 15:54:26.058930 rx7-3.3.0/
--rw-rw-rw-   0        0        0    22541 2021-08-29 10:01:16.000000 rx7-3.3.0/COLORS.html
--rw-rw-rw-   0        0        0     7815 2022-12-20 17:30:11.000000 rx7-3.3.0/LICENSE
--rw-rw-rw-   0        0        0       20 2021-08-29 10:01:16.000000 rx7-3.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    33137 2023-04-29 15:54:26.056903 rx7-3.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    32753 2023-04-29 15:43:56.000000 rx7-3.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 15:54:26.038952 rx7-3.3.0/rx7/
--rw-rw-rw-   0        0        0    73831 2023-04-29 15:40:33.000000 rx7-3.3.0/rx7/__init__.py
--rw-rw-rw-   0        0        0     1134 2023-03-09 20:00:51.000000 rx7-3.3.0/rx7/__main__.py
--rw-rw-rw-   0        0        0    20066 2021-08-29 10:01:16.000000 rx7-3.3.0/rx7/removed.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:54:26.054909 rx7-3.3.0/rx7.egg-info/
--rw-rw-rw-   0        0        0    33137 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 15:54:26.059894 rx7-3.3.0/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-04-29 15:46:03.000000 rx7-3.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:28:25.793652 rx7-4.0.0/
+-rw-rw-rw-   0        0        0       24 2023-05-10 21:05:01.000000 rx7-4.0.0/.gitattributes
+-rw-rw-rw-   0        0        0     2219 2023-05-10 21:05:01.000000 rx7-4.0.0/.gitignore
+-rw-rw-rw-   0        0        0     2514 2023-07-10 19:10:18.000000 rx7-4.0.0/.todo
+-rw-rw-rw-   0        0        0    10525 2023-07-10 19:23:13.000000 rx7-4.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    22541 2023-05-10 21:05:01.000000 rx7-4.0.0/COLORS.html
+-rw-rw-rw-   0        0        0     7815 2023-05-10 21:05:56.000000 rx7-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-07-13 20:27:53.000000 rx7-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    21277 2023-07-13 20:28:25.789652 rx7-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20550 2023-06-09 17:14:13.000000 rx7-4.0.0/README.md
+-rw-rw-rw-   0        0        0     1155 2023-07-13 20:26:03.000000 rx7-4.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-13 20:28:25.768649 rx7-4.0.0/rx7/
+-rw-rw-rw-   0        0        0      547 2023-07-10 19:30:54.000000 rx7-4.0.0/rx7/__init__.py
+-rw-rw-rw-   0        0        0     1124 2023-07-10 17:56:52.000000 rx7-4.0.0/rx7/__main__.py
+-rw-rw-rw-   0        0        0     1221 2023-05-10 21:05:01.000000 rx7-4.0.0/rx7/_dev.py
+-rw-rw-rw-   0        0        0      457 2023-07-10 17:58:31.000000 rx7-4.0.0/rx7/_developer.py
+-rw-rw-rw-   0        0        0    10768 2023-05-10 21:05:01.000000 rx7-4.0.0/rx7/datetime.py
+-rw-rw-rw-   0        0        0     5806 2023-07-10 19:11:07.000000 rx7-4.0.0/rx7/decorator.py
+-rw-rw-rw-   0        0        0    10389 2023-07-10 19:05:47.000000 rx7-4.0.0/rx7/files.py
+-rw-rw-rw-   0        0        0    12384 2023-05-10 21:05:01.000000 rx7-4.0.0/rx7/functions.py
+-rw-rw-rw-   0        0        0     3804 2023-07-10 18:11:32.000000 rx7-4.0.0/rx7/internet.py
+-rw-rw-rw-   0        0        0     5719 2023-07-03 23:24:53.000000 rx7-4.0.0/rx7/io.py
+-rw-rw-rw-   0        0        0     2766 2023-07-10 19:08:56.000000 rx7-4.0.0/rx7/random.py
+-rw-rw-rw-   0        0        0     2404 2023-05-11 11:48:02.000000 rx7-4.0.0/rx7/record.py
+-rw-rw-rw-   0        0        0     3542 2023-05-10 21:05:01.000000 rx7-4.0.0/rx7/style.py
+-rw-rw-rw-   0        0        0     6141 2023-05-10 21:05:01.000000 rx7-4.0.0/rx7/system.py
+-rw-rw-rw-   0        0        0      788 2023-07-02 15:27:38.000000 rx7-4.0.0/rx7/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:28:25.787677 rx7-4.0.0/rx7.egg-info/
+-rw-rw-rw-   0        0        0    21277 2023-07-13 20:28:25.000000 rx7-4.0.0/rx7.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-07-13 20:28:25.000000 rx7-4.0.0/rx7.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 20:28:25.000000 rx7-4.0.0/rx7.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-07-13 20:28:25.000000 rx7-4.0.0/rx7.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-13 20:28:25.000000 rx7-4.0.0/rx7.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 20:28:25.793652 rx7-4.0.0/setup.cfg
```

### Comparing `rx7-3.3.0/COLORS.html` & `rx7-4.0.0/COLORS.html`

 * *Files identical despite different names*

### Comparing `rx7-3.3.0/LICENSE` & `rx7-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rx7-3.3.0/rx7/__main__.py` & `rx7-4.0.0/rx7/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 import webbrowser
 import argparse
 
 
 parser = argparse.ArgumentParser(
     "RX7 module",
     add_help = False
@@ -23,15 +22,15 @@
     "--colors", "--color", "-c",
     action = "store_true",
     help = "Open a html Page That Contains All Colors and Information About style Class"
 )
 
 args = parser.parse_args()
 
-if args.help or (not any(args.wiki,args.colors)):
+if args.help or (not any([args.wiki,args.colors])):
     print('Available Arguments:')
     print('  [-h, --help]       Open rx7 Documention Page (pypi Page)')
     print('  [--colors]          Open a html Page That Contains All Colors and Information About style Class')
     print('-------')
 elif args.wiki:
     webbrowser.open_new_tab(f'./../COLORS.html')
 elif args.colors:
```


# Comparing `tmp/aihero-0.1.9.tar.gz` & `tmp/aihero-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihero-0.1.9.tar", last modified: Tue Jul 26 02:46:55 2022, max compression
+gzip compressed data, was "aihero-0.2.1.tar", last modified: Thu Jul 13 06:50:41 2023, max compression
```

## Comparing `aihero-0.1.9.tar` & `aihero-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2022-07-26 02:46:55.670497 aihero-0.1.9/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2022-07-03 18:23:15.000000 aihero-0.1.9/LICENSE
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     6083 2022-07-26 02:46:55.670658 aihero-0.1.9/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     5108 2022-07-26 02:46:48.000000 aihero-0.1.9/README.md
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2022-07-26 02:46:55.668511 aihero-0.1.9/aihero/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1415 2022-07-19 21:05:02.000000 aihero-0.1.9/aihero/__init__.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     3329 2022-07-25 21:19:10.000000 aihero-0.1.9/aihero/api.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     5609 2022-07-26 02:14:07.000000 aihero-0.1.9/aihero/automation.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      812 2022-07-26 02:41:53.000000 aihero-0.1.9/aihero/detect_sentiment.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2022-07-25 21:15:11.000000 aihero-0.1.9/aihero/exceptions.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1918 2022-07-26 02:41:11.000000 aihero-0.1.9/aihero/recommend_items_to_people.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1999 2022-07-26 02:41:15.000000 aihero-0.1.9/aihero/recommend_people_from_two_groups_to_each_other.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1706 2022-07-26 02:41:21.000000 aihero-0.1.9/aihero/recommend_people_to_each_other.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     2224 2022-07-26 02:41:26.000000 aihero-0.1.9/aihero/tag_entire_images.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1993 2022-07-26 02:42:01.000000 aihero-0.1.9/aihero/tag_short_text.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     2871 2022-07-12 03:27:58.000000 aihero-0.1.9/aihero/workspace.py
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2022-07-26 02:46:55.670180 aihero-0.1.9/aihero.egg-info/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     6083 2022-07-26 02:46:55.000000 aihero-0.1.9/aihero.egg-info/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      494 2022-07-26 02:46:55.000000 aihero-0.1.9/aihero.egg-info/SOURCES.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2022-07-26 02:46:55.000000 aihero-0.1.9/aihero.egg-info/dependency_links.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        6 2022-07-26 02:46:55.000000 aihero-0.1.9/aihero.egg-info/requires.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2022-07-26 02:46:55.000000 aihero-0.1.9/aihero.egg-info/top_level.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1009 2022-07-26 02:46:55.671445 aihero-0.1.9/setup.cfg
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2022-07-03 23:32:39.000000 aihero-0.1.9/setup.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:50:41.283684 aihero-0.2.1/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.1/LICENSE
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 06:50:41.283877 aihero-0.2.1/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.1/README.md
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:50:41.279384 aihero-0.2.1/aihero/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       29 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/__init__.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     3170 2023-07-13 06:46:01.000000 aihero-0.2.1/aihero/client.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.1/aihero/exceptions.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/openai_helper.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1195 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/project.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     4771 2023-07-12 04:51:12.000000 aihero-0.2.1/aihero/promptstash.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 06:50:41.282867 aihero-0.2.1/aihero.egg-info/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        6 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/requires.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-13 06:50:41.000000 aihero-0.2.1/aihero.egg-info/top_level.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1009 2023-07-13 06:50:41.284970 aihero-0.2.1/setup.cfg
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.1/setup.py
```

### Comparing `aihero-0.1.9/LICENSE` & `aihero-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aihero-0.1.9/setup.cfg` & `aihero-0.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aihero
-version = 0.1.9
+version = 0.2.1
 description = AI Hero Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ai-hero/python-client-sdk
 author = AI Hero Team
 author_email = team@aihero.studio
 license = MIT
```


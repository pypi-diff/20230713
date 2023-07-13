# Comparing `tmp/wi1-bot-1.3.4.tar.gz` & `tmp/wi1-bot-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.3.4.tar", last modified: Tue May 16 02:51:25 2023, max compression
+gzip compressed data, was "wi1-bot-1.3.5.tar", last modified: Thu Jul 13 05:32:41 2023, max compression
```

## Comparing `wi1-bot-1.3.4.tar` & `wi1-bot-1.3.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 02:51:23.000000 wi1-bot-1.3.4/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/add_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 02:51:25.000000 wi1-bot-1.3.4/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.497362 wi1-bot-1.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 05:32:40.000000 wi1-bot-1.3.5/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/add_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-13 05:32:40.000000 wi1-bot-1.3.5/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.3.4/.github/workflows/pypi-publish.yml` & `wi1-bot-1.3.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/.pre-commit-config.yaml` & `wi1-bot-1.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/LICENSE` & `wi1-bot-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/PKG-INFO` & `wi1-bot-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.4
+Version: 1.3.5
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.3.4/README.md` & `wi1-bot-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/config.yaml.template` & `wi1-bot-1.3.5/config.yaml.template`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/pyproject.toml` & `wi1-bot-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/arr/download.py` & `wi1-bot-1.3.5/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/arr/episode.py` & `wi1-bot-1.3.5/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/arr/movie.py` & `wi1-bot-1.3.5/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/arr/radarr.py` & `wi1-bot-1.3.5/wi1_bot/arr/radarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/arr/sonarr.py` & `wi1-bot-1.3.5/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/config.py` & `wi1-bot-1.3.5/wi1_bot/config.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/discord/bot.py` & `wi1-bot-1.3.5/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.3.5/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.3.5/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/discord/helpers.py` & `wi1-bot-1.3.5/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/push.py` & `wi1-bot-1.3.5/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/scripts/add_tag.py` & `wi1-bot-1.3.5/wi1_bot/scripts/add_tag.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/scripts/start.py` & `wi1-bot-1.3.5/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.3.5/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.3.5/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.3.5/wi1_bot/transcoder/transcoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,14 +120,21 @@
                 if "received signal 15" in last_output:
                     self.logger.debug(
                         f"transcoding interrupted by signal: {path}, will retry"
                     )
                     raise SignalInterrupt
 
                 perm_log_path = tmp_folder / f"{path.stem}.log"
+
+                if "general" in config and "log_dir" in config["general"]:
+                    log_dir = pathlib.Path(config["general"]["log_dir"]).resolve()
+
+                    perm_log_path = log_dir / "transcoder-errors" / f"{path.stem}.log"
+                    perm_log_path.mkdir(parents=True, exist_ok=True)
+
                 shutil.copy(tmp_log_path, perm_log_path)
                 self.logger.error(f"log file: {perm_log_path}")
 
                 push.send(
                     f"{path.name} has failed to transcode, log: {perm_log_path}",
                     title="transcoding error",
                 )
```

### Comparing `wi1-bot-1.3.4/wi1_bot/webhook.py` & `wi1-bot-1.3.5/wi1_bot/webhook.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.4/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.3.5/wi1_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.4
+Version: 1.3.5
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.3.4/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.3.5/wi1_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*


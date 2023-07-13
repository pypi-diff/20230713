# Comparing `tmp/gchar-0.0.9.tar.gz` & `tmp/gchar-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gchar-0.0.9.tar", last modified: Sat Apr 15 11:41:06 2023, max compression
+gzip compressed data, was "gchar-0.1.0.tar", last modified: Thu Jul 13 11:10:29 2023, max compression
```

## Comparing `gchar-0.0.9.tar` & `gchar-0.1.0.tar`

### file list

```diff
@@ -1,134 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.726343 gchar-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 11:40:25.000000 gchar-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-15 11:40:25.000000 gchar-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-15 11:41:06.726343 gchar-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-15 11:40:25.000000 gchar-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.710343 gchar-0.0.9/gchar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.710343 gchar-0.0.9/gchar/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.710343 gchar-0.0.9/gchar/games/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.714343 gchar-0.0.9/gchar/games/arknights/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/arknights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/arknights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/arknights/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   259287 2023-04-15 11:40:57.000000 gchar-0.0.9/gchar/games/arknights/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)   719302 2023-04-15 11:40:57.000000 gchar-0.0.9/gchar/games/arknights/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/arknights/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/arknights/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-15 11:40:57.000000 gchar-0.0.9/gchar/games/arknights/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    41356 2023-04-15 11:40:57.000000 gchar-0.0.9/gchar/games/arknights/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   285047 2023-04-15 11:40:57.000000 gchar-0.0.9/gchar/games/arknights/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/arknights/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.718343 gchar-0.0.9/gchar/games/azurlane/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/azurlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/azurlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/azurlane/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   571315 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/azurlane/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)  1261496 2023-04-15 11:40:57.000000 gchar-0.0.9/gchar/games/azurlane/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/azurlane/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/azurlane/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/azurlane/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    91374 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/azurlane/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   537380 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/azurlane/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/azurlane/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.718343 gchar-0.0.9/gchar/games/base/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/base/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/base/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/base/moegirl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/base/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/base/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/base/skin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.718343 gchar-0.0.9/gchar/games/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/dispatch/access.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.722343 gchar-0.0.9/gchar/games/fgo/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/fgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/fgo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/fgo/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   631491 2023-04-15 11:40:56.000000 gchar-0.0.9/gchar/games/fgo/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)  1166076 2023-04-15 11:40:56.000000 gchar-0.0.9/gchar/games/fgo/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/fgo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/fgo/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-15 11:40:56.000000 gchar-0.0.9/gchar/games/fgo/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    55053 2023-04-15 11:40:57.000000 gchar-0.0.9/gchar/games/fgo/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   281606 2023-04-15 11:40:56.000000 gchar-0.0.9/gchar/games/fgo/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/fgo/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.722343 gchar-0.0.9/gchar/games/genshin/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/genshin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/genshin/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   143310 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/genshin/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)    71892 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/genshin/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/genshin/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/genshin/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/genshin/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/genshin/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)    71591 2023-04-15 11:40:58.000000 gchar-0.0.9/gchar/games/genshin/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/genshin/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.722343 gchar-0.0.9/gchar/games/girlsfrontline/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/girlsfrontline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/girlsfrontline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/girlsfrontline/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   364422 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/girlsfrontline/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)   589632 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/girlsfrontline/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/girlsfrontline/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/girlsfrontline/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/girlsfrontline/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    59325 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/girlsfrontline/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   270008 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/girlsfrontline/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/girlsfrontline/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.726343 gchar-0.0.9/gchar/games/neuralcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/neuralcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/neuralcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/neuralcloud/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   391243 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/neuralcloud/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)   147890 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/neuralcloud/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/neuralcloud/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/neuralcloud/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 11:40:59.000000 gchar-0.0.9/gchar/games/neuralcloud/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-04-15 11:41:00.000000 gchar-0.0.9/gchar/games/neuralcloud/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)    42560 2023-04-15 11:41:00.000000 gchar-0.0.9/gchar/games/neuralcloud/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/games/neuralcloud/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.726343 gchar-0.0.9/gchar/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.726343 gchar-0.0.9/gchar/resources/danbooru/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/danbooru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/danbooru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/danbooru/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/danbooru/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/danbooru/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.726343 gchar-0.0.9/gchar/resources/pixiv/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/pixiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/pixiv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/pixiv/games.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/pixiv/keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/pixiv/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/resources/pixiv/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.726343 gchar-0.0.9/gchar/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-15 11:40:25.000000 gchar-0.0.9/gchar/utils/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.710343 gchar-0.0.9/gchar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-15 11:41:06.000000 gchar-0.0.9/gchar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-15 11:41:06.000000 gchar-0.0.9/gchar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:41:06.000000 gchar-0.0.9/gchar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-15 11:41:06.000000 gchar-0.0.9/gchar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 11:41:06.000000 gchar-0.0.9/gchar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 11:40:25.000000 gchar-0.0.9/requirements-crawl.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-15 11:40:25.000000 gchar-0.0.9/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 11:40:25.000000 gchar-0.0.9/requirements-speedup.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-15 11:40:25.000000 gchar-0.0.9/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 11:40:25.000000 gchar-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 11:41:06.726343 gchar-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-15 11:40:25.000000 gchar-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:06.726343 gchar-0.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-15 11:40:25.000000 gchar-0.0.9/test/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 11:09:10.000000 gchar-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-13 11:09:10.000000 gchar-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-13 11:10:29.370192 gchar-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-13 11:09:10.000000 gchar-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/arknights/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/arknights/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/azurlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/azurlane/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/base/skin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/bluearchive/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/bluearchive/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/dispatch/access.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/fgo/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/fgo/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar/games/genshin/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/genshin/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/girlsfrontline/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/girlsfrontline/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/neuralcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/neuralcloud/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/nikke/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/nikke/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/pathtonowhere/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/pathtonowhere/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/games/starrail/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/games/starrail/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/resources/pixiv/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/pixiv/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/resources/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/sites/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/resources/sites/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.370192 gchar-0.1.0/gchar/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-13 11:09:10.000000 gchar-0.1.0/gchar/utils/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:10:29.366192 gchar-0.1.0/gchar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 11:10:29.000000 gchar-0.1.0/gchar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-crawl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-speedup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 11:09:10.000000 gchar-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:10:29.370192 gchar-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-13 11:09:10.000000 gchar-0.1.0/setup.py
```

### Comparing `gchar-0.0.9/LICENSE` & `gchar-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gchar-0.0.9/PKG-INFO` & `gchar-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gchar
-Version: 0.0.9
+Version: 0.1.0
 Summary: Game character manager.
 Home-page: https://github.com/narugo1992/gchar
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,19 +12,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: crawl
-Provides-Extra: speedup
 Provides-Extra: test
+Provides-Extra: speedup
 Provides-Extra: doc
 License-File: LICENSE
 
 # gchar
 
 [![PyPI](https://img.shields.io/pypi/v/gchar)](https://pypi.org/project/gchar/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gchar)
@@ -55,46 +55,73 @@
 
 ```shell
 pip install gchar
 ```
 
 ## Quick Start
 
+### Game Character Query
+
 Find the characters (nicknames are supported for arknights and fgo)
 
+Currently Supported Games (If you need data of other games,
+you can [create an issue](https://github.com/narugo1992/gchar/issues/new)):
+
+* Arknights (crawled from [PRTS Wiki](https://prts.wiki))
+* Fate/Grand Order (crawled from [FGO Wiki](https://fgo.wiki))
+* Azur Lane (crawled from [BiliGame Wiki](https://wiki.biligame.com/blhx))
+* Girls' Front-Line (crawled from [IOPWiki](https://iopwiki.com/))
+* Genshin Impact (crawled from [Fandom](https://genshin-impact.fandom.com/ja/wiki/%E5%8E%9F%E7%A5%9E_Wiki))
+* Neural Cloud (crawled from [42lab wiki](http://wiki.42lab.cloud))
+* Blue Archive (crawled from [bluearchive wiki](https://bluearchive.wiki/) and [Gamekee BA](https://ba.gamekee.com))
+* Nikke: Goddess of Victory (crawled from [Fandom](https://nikke-goddess-of-victory-international.fandom.com)
+  and [Gamekee Nikke](https://nikke.gamekee.com))
+* Path To Nowhere (crawled from [BiliGame Wiki](https://wiki.biligame.com/wqmt))
+* Honkai: Star Rail (crawled from [Star Rail Station](https://starrailstation.com)
+  and [BiliGame Wiki](https://wiki.biligame.com))
+
 ```
 >>> from gchar.games import get_character
 >>> 
->>> get_character('CEO')
-<Character 171 - 彭忒西勒亚/黄金国的berserker/penthesilea/berserker_of_el_dorado/ペンテシレイア/エルドラドのバーサーカー, female, 4****>
->>> get_character('黑呆')
-<Character 3 - 阿尔托莉雅·潘德拉贡〔alter〕/altria_pendragon_alter/アルトリア・ペンドラゴン〔オルタ〕, female, 4****>
->>> get_character('amiya')
+>>> get_character('amiya')  # english name
 <Character R001 - 阿米娅/amiya/アーミヤ, female, 5*****>
->>> get_character('小火龙')
-<Character RL03 - 伊芙利特/ifrit/イフリータ, female, 6******>
->>> get_character('宵宫')
-<Character 宵宫/yoimiya/宵宮/よいみや, female, 5*****, weapon: Weapon.BOW, element: Element.PYRO>
 >>> get_character('z18')
-<Character 346 - z18/hans_ludemann/ハンス・リューデマン, 稀有(2**), group: Group.KMS>
+<Character 346 - Z18/hans_ludemann/ハンス・リューデマン, 稀有(2**), group: Group.KMS>
 >>> get_character('416')
 <Character 65 - HK416/416/416, 5*****, clazz: Clazz.AR>
+>>> 
+>>> get_character('夕')  # chinese name
+<Character NM02 - 夕/dusk/シー, female, 6******>
+>>> get_character('宵宫')
+<Character 宵宫/yoimiya/宵宮/よいみや, female, 5*****, weapon: Weapon.BOW, element: Element.PYRO>
+>>> 
+>>> get_character('スルト')  # japanese name
+<Character R111 - 史尔特尔/surtr/スルト, female, 6******>
+>>> 
+>>> get_character('CEO')  # alias
+<Character 171 - 彭忒西勒亚/黄金国的Berserker/penthesilea/berserker_of_el_dorado/ペンテシレイア/エルドラドのバーサーカー, female, 4****, class: Clazz.BERSERKER>
+>>> get_character('黑呆')
+<Character 3 - 阿尔托莉雅·潘德拉贡〔Alter〕/altria_pendragon_alter/アルトリア・ペンドラゴン〔オルタ〕/アルトリア・ペンドラゴン・オルタ/アルトリア・オルタ, female, 4****, class: Clazz.SABER>
+>>> get_character('小火龙')
+<Character RL03 - 伊芙利特/ifrit/イフリータ, female, 6******>
 ```
 
 List all character with specific condition of one game
 
 ```python
 from gchar.games.arknights import Character
 
 for ch in Character.all():  # 5star, boys
     if ch.rarity == 5 and ch.gender == 'male':
         print(ch)
 
 ```
 
+### Pixiv Resources
+
 Get search keywords for pixiv
 
 ```
 >>> from gchar.resources.pixiv import get_pixiv_keywords
 >>> 
 >>> get_pixiv_keywords('CEO')
 'Fate/GrandOrder (berserker_of_el_dorado OR penthesilea OR エルドラドのバーサーカー OR ペンテシレイア OR 彭忒西勒亚 OR 黄金国的berserker)'
@@ -106,49 +133,75 @@
 'アークナイツ (blaze OR ブレイズ OR 煌)'
 >>> get_pixiv_keywords('林雨霞')
 'アークナイツ (lin OR 林) -angelina -flint -folinic -ling -守林人 -巡林者 -杜林'
 >>> get_pixiv_keywords('夕')
 'アークナイツ (dusk OR シー OR 夕) -ケルシー -シージ -シーン'
 ```
 
-Get tags for danbooru
+See how many posts on pixiv
+
+```
+>>> from gchar.resources.pixiv import get_pixiv_posts
+>>> 
+>>> # first one is all, second one is r18
+>>> get_pixiv_posts('CEO')
+(867, 113)
+>>> get_pixiv_posts('黑贞')
+(21908, 3820)
+>>> get_pixiv_posts('amiya')
+(14130, 1113)
+>>> get_pixiv_posts('blazer')  # fuzzy match is supported, but slower
+(1967, 383)
+>>> get_pixiv_posts('林雨霞')
+(259, 44)
+>>> get_pixiv_posts('夕')
+(2908, 424)
+```
+
+### Other Sites' Resource
+
+Get tags for danbooru and other sites
+
+Currently supported sites:
+
+* [Anime Pictures](https://anime-pictures.net), named `anime_pictures`
+* [Atfbooru](https://booru.allthefallen.moe), named `atfbooru`
+* [Sankaku](https://chan.sankakucomplex.com), named `sankaku`
+* [Danbooru](https://danbooru.donmai.us), named `danbooru`
+* [Hypnohub](https://hypnohub.net), named `hypnohub`
+* [Konachan](https://konachan.com), named `konachan`
+* [Konachan.Net](https://konachan.net), named `konachan_net`
+* [Lolibooru](https://lolibooru.moe), named `lolibooru`
+* [Rule34](https://rule34.xxx), named `rule34`
+* [Safebooru](https://safebooru.donmai.us), named `safebooru`
+* [Xbooru](https://xbooru.com), named `xbooru`
+* [Yande](https://yande.re), named `yande`
+* [Zerochan](https://zerochan.net), named `zerochan`
 
 ```
->>> from gchar.resources.danbooru import get_danbooru_tag
+>>> from gchar.resources.sites import get_site_tag
 >>> 
->>> get_danbooru_tag('CEO')
+>>> # first one is all, second one is r18
+>>> get_site_tag('CEO', 'danbooru')
 'penthesilea_(fate)'
->>> get_danbooru_tag('黑贞')
+>>> get_site_tag('黑贞', 'danbooru')
 "jeanne_d'arc_alter_(fate)"
->>> get_danbooru_tag('amiya')
+>>> get_site_tag('amiya', 'danbooru')
 'amiya_(arknights)'
->>> get_danbooru_tag('blazer')  # fuzzy match is supported
-'blaze_(arknights)'
->>> get_danbooru_tag('林雨霞')
+>>> get_site_tag('林雨霞', 'danbooru')
 'lin_(arknights)'
->>> get_danbooru_tag('夕')
+>>> get_site_tag('夕', 'danbooru')
 'dusk_(arknights)'
+>>> get_site_tag('夕', 'danbooru', with_posts=True)  # see how many images
+('dusk_(arknights)', 1397)
+>>> get_site_tag('夕', 'zerochan')  # another sites
+'Dusk (Arknights)'
 ```
 
-Currently Supported Games (If you need data of other games,
-you can [create an issue](https://github.com/narugo1992/gchar/issues/new)):
-
-* Arknights (crawled from [https://prts.wiki](https://prts.wiki))
-* Fate/Grand Order (crawled from [https://fgo.wiki](https://fgo.wiki))
-* Azur Lane (crawled from [https://wiki.biligame.com/blhx](https://wiki.biligame.com/blhx))
-* Girls' Front-Line (crawled from [https://iopwiki.com/](https://iopwiki.com/))
-* Genshin Impact (crawled
-  from [https://genshin-impact.fandom.com/ja/wiki/%E5%8E%9F%E7%A5%9E_Wiki](https://genshin-impact.fandom.com/ja/wiki/%E5%8E%9F%E7%A5%9E_Wiki))
-
 ## FAQ
 
-### The data here is out-of-date
+Q: How timely is the data?
 
-Just update the local data with the following commands.
-
-```shell
-python -m gchar update        # download newest data of all the games
-python -m gchar update -g fgo # download newest data of fgo
-python -m gchar update --help # help information
-
-```
+A: The data is updated approximately once a day and is hosted on Github Action, ensuring its timeliness. In the event of
+a malfunction on the crawled Wiki site that prevents data updates, the corresponding Wiki team will be contacted to
+resolve the issue.
```

### Comparing `gchar-0.0.9/gchar/games/arknights/character.py` & `gchar-0.1.0/gchar/games/arknights/character.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,125 @@
+import math
 from typing import List, Tuple
 
-from .index import _KNOWN_DATA_FIELDS, INDEXER
 from .name import EnglishName, JapaneseName, ChineseName, ChineseAliasName
-from .property import Level, Clazz
+from .property import Rarity, Clazz
 from ..base import Character as _BaseCharacter
 
+_KNOWN_DATA_FIELDS = [
+    'data-adapt', 'data-atk', 'data-birth_place', 'data-block', 'data-cost', 'data-def', 'data-en',
+    'data-flex', 'data-group', 'data-hp', 'data-id', 'data-interval', 'data-ja', 'data-logo',
+    'data-nation', 'data-obtain_method', 'data-phy', 'data-plan', 'data-position', 'data-potential',
+    'data-profession', 'data-race', 'data-rarity', 'data-re_deploy', 'data-res', 'data-sex',
+    'data-skill', 'data-sortid', 'data-subprofession', 'data-tag', 'data-team', 'data-tolerance',
+    'data-trust', 'data-zh'
+]
+
 
 class Character(_BaseCharacter):
     """
+    A class for modeling characters in the Arknights game.
+
     Here is an example of operator data from prts.wiki
 
-    .. code-block::
+    .. code-block:: json
         :linenos:
-        :language: text
 
         {
-            "data-cn": "龙舌兰",
-            "data-position": "近战位",
-            "data-en": "Tequila",
-            "data-sex": "男",
-            "data-tag": "爆发",
-            "data-race": "佩洛",
-            "data-rarity": "4",
-            "data-class": "近卫",
-            "data-approach": "活动获得",
-            "data-camp": "玻利瓦尔",
+            "data-adapt": "普通",
+            "data-atk": "102",
+            "data-birth_place": "未公开",
+            "data-block": "1",
+            "data-cost": "3",
+            "data-def": "28",
+            "data-en": "U-Official",
+            "data-flex": "缺陷",
+            "data-group": "",
+            "data-hp": "385",
+            "data-id": "U007",
+            "data-interval": "1.3s",
+            "data-ja": "",
+            "data-logo": "罗德岛",
+            "data-nation": "罗德岛",
+            "data-obtain_method": "活动获得",
+            "data-phy": "普通",
+            "data-plan": "缺陷",
+            "data-position": "远程位",
+            "data-potential": "`",
+            "data-profession": "辅助",
+            "data-race": "札拉克",
+            "data-rarity": "0",
+            "data-re_deploy": "200s",
+            "data-res": "0",
+            "data-sex": "女",
+            "data-skill": "缺陷",
+            "data-sortid": "274",
+            "data-subprofession": "吟游者",
+            "data-tag": "控场",
             "data-team": "",
-            "data-des": "近卫干员龙舌兰，在战场上也面带笑容。",
-            "data-feature": "通常不攻击且阻挡数为0，技能未开启时<span style=\"color:#00B0FF;\">40</span>
-                             秒内攻击力逐渐提升至最高<span style=\"color:#00B0FF;\">+200%</span>且技能结束时重置攻击力",
-            "data-str": "标准",
-            "data-flex": "标准",
             "data-tolerance": "普通",
-            "data-plan": "优良",
-            "data-skill": "标准",
-            "data-adapt": "普通",
-            "data-moredes": "别担心，他会把一切都安排妥帖。",
-            "data-icon": "//prts.wiki/images/4/42/%E5%A4%B4%E5%83%8F_%E9%BE%99%E8%88%8C%E5%85%B0.png",
-            "data-half": "//prts.wiki/images/thumb/3/34/%E5%8D%8A%E8%BA%AB%E5%83%8F_%E9%BE%99%E8%88%8C%E5%85
-                          %B0_1.png/110px-%E5%8D%8A%E8%BA%AB%E5%83%8F_%E9%BE%99%E8%88%8C%E5%85%B0_1.png",
-            "data-ori-hp": "1,871",
-            "data-ori-atk": "137",
-            "data-ori-def": "238",
-            "data-ori-res": "15",
-            "data-ori-dt": "80s",
-            "data-ori-dc": "11→13",
-            "data-ori-block": "2→2→3",
-            "data-ori-cd": "1.2s",
-            "data-index": "BV12",
-            "data-jp": "テキーラ",
-            "data-birthplace": "玻利瓦尔",
-            "data-nation": "玻利瓦尔",
-            "data-group": ""
+            "data-trust": "120,20,0",
+            "data-zh": "U-Official"
         }
     """
+    __game_name__ = 'arknights'
+    __official_name__ = 'Arknights'
     __cnname_class__ = ChineseName
     __enname_class__ = EnglishName
     __jpname_class__ = JapaneseName
     __alias_name_class__ = ChineseAliasName
-    __indexer__ = INDEXER
 
     def __init__(self, raw_data: dict):
+        """
+        Initialize a character with the raw data.
+
+        :param raw_data: The raw data of the character.
+        :type raw_data: dict
+        """
         self.__origin_raw_data = raw_data
         self.__raw_data = raw_data['data']
         self.__skins = raw_data['skins']
         self.__is_extra = None
 
     def _index(self):
-        return self.__raw_data['data-index']
+        return self.__raw_data.get('data-index') or self.__raw_data.get('data-id')
 
     def _gender(self):
         return self.__raw_data['data-sex']
 
     @property
-    def rarity(self) -> Level:
-        return Level.loads(int(self.__raw_data['data-rarity']) + 1)
+    def rarity(self) -> Rarity:
+        """
+        Get the rarity of the character.
+
+        :return: The rarity of the character.
+        :rtype: :class:`Rarity`
+        """
+        return Rarity.loads(int(self.__raw_data['data-rarity']) + 1)
 
     @property
     def clazz(self) -> Clazz:
-        return Clazz.loads(self.__raw_data['data-class'])
+        """
+        Get the class of the character.
+
+        :return: The class of the character.
+        :rtype: Clazz
+        """
+        return Clazz.loads(self.__raw_data.get('data-class') or self.__raw_data.get('data-profession'))
 
     def _cnname(self):
-        return self.__raw_data['data-cn']
+        return self.__raw_data.get('data-cn') or self.__raw_data.get('data-zh') or None
 
     def _enname(self):
-        return self.__raw_data.get('data-en', None)
+        return self.__raw_data.get('data-en') or None
 
     def _jpname(self):
-        return self.__raw_data.get('data-jp', None)
+        return self.__raw_data.get('data-jp') or self.__raw_data.get('data-ja') or None
 
-    def _alias_names(self):
+    def _custom_alias_names(self):
         return list(self.__origin_raw_data.get('alias', []) or [])
 
     def _skins(self) -> List[Tuple[str, str]]:
         return [(item['name'], item['url']) for item in self.__skins]
 
     def __getattr__(self, item: str):
         key = 'data-' + item.replace('_', '-')
@@ -104,15 +130,17 @@
 
     def _is_extra(self) -> bool:
         return (self.enname and 'the' in self.enname) or \
             (self.enname == 'amiya' and self.cnname != '阿米娅')
 
     def _order(self):
         release_info = self.__origin_raw_data['release']
-        return release_info['time'], release_info['index']
+        _release_time = release_info['time'] if release_info['time'] is not None else math.inf
+        _release_index = release_info['index'] if release_info['index'] is not None else math.inf
+        return _release_time, _release_index
 
     def _release_time(self):
         _release_time, _ = self._order()
         return _release_time
 
     def __repr__(self):
         return f'<{type(self).__name__} {self.index} - {"/".join(map(str, self._names()))}, ' \
```

### Comparing `gchar-0.0.9/gchar/games/arknights/name.py` & `gchar-0.1.0/gchar/games/fgo/name.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from transliterate import translit
+import re
+
+import unicodedata
+from unidecode import unidecode
 
 from ..base import ChineseName as _GenericChineseName
 from ..base import EnglishName as _GenericEnglishName
 from ..base import JapaneseName as _GenericJapaneseName
 
 
 class ChineseName(_GenericChineseName):
     @classmethod
     def _preprocess(cls, name: str) -> str:
-        return _GenericChineseName._preprocess(name).replace('・', '·')
+        return _GenericChineseName._preprocess(name).replace('・', '·').replace("\"", '') \
+            .replace("“", '').replace("”", '')
 
 
 class ChineseAliasName(_GenericChineseName):
     @classmethod
     def _preprocess(cls, name: str) -> str:
-        return _GenericChineseName._preprocess(name).replace('・', '·')
+        return unicodedata.normalize('NFKC', _GenericChineseName._preprocess(name))
 
 
 class JapaneseName(_GenericJapaneseName):
-    pass
+    @classmethod
+    def _preprocess(cls, name: str) -> str:
+        return unicodedata.normalize('NFKC', _GenericJapaneseName._preprocess(name))
 
 
 class EnglishName(_GenericEnglishName):
     @classmethod
-    def _word_trans(cls, text: str):
-        return translit(text.replace('\'', '').replace('\"', ''), 'ru', reversed=True)
+    def _word_trans(cls, name: str) -> str:
+        return ' '.join(re.findall('[a-zA-Z0-9]+', unidecode(name.lower())))
```

### Comparing `gchar-0.0.9/gchar/games/arknights/property.py` & `gchar-0.1.0/gchar/games/genshin/property.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,114 @@
-from enum import IntEnum, unique, Enum
+from enum import unique, Enum, IntEnum
 
 
 @unique
-class Level(IntEnum):
-    ONE = 0x1
-    TWO = 0x2
-    THREE = 0x3
+class Rarity(IntEnum):
     FOUR = 0x4
     FIVE = 0x5
-    SIX = 0x6
 
     @classmethod
-    def loads(cls, val) -> 'Level':
+    def loads(cls, val) -> 'Rarity':
         if isinstance(val, cls):
             return val
         elif isinstance(val, int):
             for name, item in cls.__members__.items():
                 if item.value == val:
                     return item.value
 
             raise ValueError(f'Invalid level value - {val!r}.')
         else:
             raise TypeError(f'Invalid level type - {val!r}.')
 
 
 @unique
-class Clazz(Enum):
-    GUARD = 0x1
-    DEFENDER = 0x2
-    CASTER = 0x3
-    SNIPER = 0x4
-    SPECIALIST = 0x5
-    SUPPORTER = 0x6
-    MEDIC = 0x7
-    VANGUARD = 0x8
+class Weapon(Enum):
+    CATALYST = 0x1
+    CLAYMORE = 0x2
+    SWORD = 0x3
+    BOW = 0x4
+    POLEARM = 0x5
 
     def __eq__(self, other):
-        if isinstance(other, Clazz):
-            return self.value == other.value
+        if isinstance(other, Weapon):
+            return other.value == self.value
         else:
             try:
-                return self == self.loads(other)
+                other = Weapon.loads(other)
             except (TypeError, ValueError):
                 return False
+            else:
+                return other == self
 
     @classmethod
-    def loads(cls, val) -> 'Clazz':
+    def loads(cls, val) -> 'Weapon':
         if isinstance(val, cls):
             return val
         elif isinstance(val, str):
-            val = val.lower().strip()
-            if val in {'近卫', 'guard'}:
-                return cls.GUARD
-            elif val in {'重装', 'defender'}:
-                return cls.DEFENDER
-            elif val in {'术师', 'caster'}:
-                return cls.CASTER
-            elif val in {'狙击', 'sniper'}:
-                return cls.SNIPER
-            elif val in {'特种', 'specialist'}:
-                return cls.SPECIALIST
-            elif val in {'辅助', 'supporter'}:
-                return cls.SUPPORTER
-            elif val in {'医疗', 'medic'}:
-                return cls.MEDIC
-            elif val in {'先锋', 'vanguard'}:
-                return cls.VANGUARD
+            pval = val.upper().strip()
+            if pval in cls.__members__:
+                return cls.__members__[pval]
+
+            if pval in {'单手剑'}:
+                return cls.SWORD
+            elif pval in {'双手剑'}:
+                return cls.CLAYMORE
+            elif pval in {'长柄武器'}:
+                return cls.POLEARM
+            elif pval in {'法器'}:
+                return cls.CATALYST
+            elif pval in {'弓'}:
+                return cls.BOW
+
+            raise ValueError(f'Invalid weapon value - {val!r}.')
+        else:
+            raise TypeError(f'Invalid weapon type - {val!r}.')
+
+
+@unique
+class Element(Enum):
+    PYRO = 0x1
+    ANEMO = 0x2
+    CRYO = 0x3
+    ELECTRO = 0x4
+    DENDRO = 0x5
+    GEO = 0x6
+    HYDRO = 0x7
+
+    def __eq__(self, other):
+        if isinstance(other, Element):
+            return other.value == self.value
+        else:
+            try:
+                other = Element.loads(other)
+            except (TypeError, ValueError):
+                return False
             else:
-                raise ValueError(f'Invalid class value - {val!r}.')
+                return other == self
+
+    @classmethod
+    def loads(cls, val) -> 'Element':
+        if isinstance(val, cls):
+            return val
+        elif isinstance(val, str):
+            pval = val.upper().strip()
+            if pval in cls.__members__:
+                return cls.__members__[pval]
+
+            if pval in {'火'}:
+                return cls.PYRO
+            elif pval in {'风'}:
+                return cls.ANEMO
+            elif pval in {'冰'}:
+                return cls.CRYO
+            elif pval in {'雷'}:
+                return cls.ELECTRO
+            elif pval in {'草'}:
+                return cls.DENDRO
+            elif pval in {'岩'}:
+                return cls.GEO
+            elif pval in {'水'}:
+                return cls.HYDRO
 
+            raise ValueError(f'Invalid element value - {val!r}.')
         else:
-            raise TypeError(f'Invalid class type - {val!r}.')
+            raise TypeError(f'Invalid element type - {val!r}.')
```

### Comparing `gchar-0.0.9/gchar/games/azurlane/character.py` & `gchar-0.1.0/gchar/games/starrail/character.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,84 @@
-from typing import List, Optional, Union, Tuple
+from typing import List, Tuple, Optional
 
-from .index import INDEXER
-from .name import EnglishName, JapaneseName, ChineseName, ChineseAliasName
-from .property import BasicRarity, ResearchRarity, Group
-from ..base import Character as _BaseCharacter
+from .name import ChineseName, EnglishName, JapaneseName, KoreanName
+from .property import Rarity
+from ..base import Character as _BaseCharacter, Gender
+from ..base.name import _BaseName
 
 
 class Character(_BaseCharacter):
+    __game_name__ = 'starrail'
+    __official_name__ = 'Honkai Star Rail'
     __cnname_class__ = ChineseName
     __enname_class__ = EnglishName
     __jpname_class__ = JapaneseName
-    __alias_name_class__ = ChineseAliasName
-    __indexer__ = INDEXER
 
-    def __init__(self, raw_data: dict):
+    def __init__(self, raw_data):
         self.__raw_data = raw_data
 
-    def _index(self) -> str:
+    def _index(self):
         return self.__raw_data['id']
 
     def _cnname(self):
-        return self.__raw_data['cnname']['short']
-
-    def _enname(self):
-        return self.__raw_data['enname']['short']
+        return self.__raw_data['cnname']
 
     def _jpname(self):
-        if self.__raw_data['jpnames']:
-            return self.__raw_data['jpnames'][0]
-        else:
-            return None
-
-    def _jpnames(self):
-        return self.__raw_data['jpnames']
-
-    def _alias_names(self):
-        return self.__raw_data['alias']
-
-    def _gender(self):
-        return 'female'
+        return self.__raw_data['jpname']
 
-    @property
-    def rarity(self) -> Optional[Union[BasicRarity, ResearchRarity]]:
-        val = self.__raw_data['rarity']
-        try:
-            return BasicRarity.loads(val)
-        except (ValueError, TypeError):
-            return ResearchRarity.loads(val)
+    def _enname(self):
+        return self.__raw_data['enname']
 
-    @property
-    def group(self) -> Union[Group, str]:
-        try:
-            return Group.loads(self.__raw_data['group'])
-        except (TypeError, ValueError):
-            return self.__raw_data['group']
+    def _krname(self):
+        return self.__raw_data['krname']
 
     @property
-    def is_meta(self) -> bool:
-        return self.__raw_data['is_meta']
+    def krname(self) -> Optional[KoreanName]:
+        name = self._krname()
+        return KoreanName(name) if name is not None else None
 
-    @property
-    def is_refit(self) -> bool:
-        return self.__raw_data['is_refit']
+    def _krnames(self):
+        name = self._krname()
+        return [name] if name else []
 
     @property
-    def is_mu(self) -> bool:
-        return self.__raw_data['is_mu']
+    def krnames(self) -> List[KoreanName]:
+        return [KoreanName(name) for name in self._krnames()]
 
-    @property
-    def is_chibi(self) -> bool:
-        return self.__raw_data['is_chibi']
+    def _names(self) -> List[_BaseName]:
+        return [*_BaseCharacter._names(self), *self.krnames]
 
-    def _is_extra(self) -> bool:
-        return self.is_meta or self.is_refit or self.is_mu or self.is_chibi
+    def _gender(self):
+        return Gender.loads(self.__raw_data['gender'])
 
     def _skins(self) -> List[Tuple[str, str]]:
-        return [(item['name'], item['url']) for item in self.__raw_data['skins']]
+        return [
+            (skin['name'], skin['url'])
+            for skin in self.__raw_data['skins']
+        ]
 
     def _release_time(self):
-        release_info = self.__raw_data['release']
-        return release_info['time']
+        return self.__raw_data['release']['time']
 
     def _order(self):
-        return self._release_time()
+        return self._release_time(),
+
+    @property
+    def rarity(self):
+        return Rarity.loads(self.__raw_data['rarity'])
+
+    @property
+    def destiny(self):
+        return self.__raw_data['destiny']
+
+    @property
+    def element(self):
+        return self.__raw_data['element']
+
+    @property
+    def group(self):
+        return self.__raw_data['group']
 
     def __repr__(self):
-        return f'<{type(self).__name__} {self.index} - {"/".join(map(str, self._names()))}, ' \
-               f'{self.rarity.label}({int(self.rarity)}{"*" * self.rarity}), ' \
-               f'group: {self.group if isinstance(self.group, Group) else self.group}>'
+        return f'<{type(self).__name__} {"/".join(map(str, self._names()))}, ' \
+               f'{self.rarity.name}({int(self.rarity)}{"*" * self.rarity}), ' \
+               f'element: {self.element}, destiny: {self.destiny}>'
```

### Comparing `gchar-0.0.9/gchar/games/azurlane/name.py` & `gchar-0.1.0/gchar/games/neuralcloud/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.9/gchar/games/base/character.py` & `gchar-0.1.0/gchar/games/azurlane/property.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,188 +1,208 @@
-from itertools import chain
-from typing import List, Union, Type, Iterator, Optional, Callable, Tuple
+from enum import unique, IntEnum, Enum
 
-from .index import BaseIndexer
-from .name import _BaseName, ChineseName, EnglishName, JapaneseName
-from .property import Gender
-from .skin import Skin
-from ...utils import Comparable
-
-
-class CharacterMeta(type):
-    def __init__(cls, name, bases, dict_):
-        type.__init__(cls, name, bases, dict_)
-        cls.__original_names = set([name for name in dir(type) if name.startswith('__') and name.endswith('__')])
-        if not hasattr(cls, '__indexer__'):
-            cls.__indexer__: Optional[BaseIndexer] = None
 
-    @property
-    def __index_func__(cls) -> Optional[Callable]:
-        if cls.__indexer__:
-            return cls.__indexer__.get_index
+@unique
+class Group(Enum):
+    """
+    An enumeration representing the groups in the Azur Lane game.
+    """
+
+    USS = 0x1
+    HMS = 0x2
+    IJN = 0x3
+    KMS = 0x4
+    DE = 0x5
+    RN = 0x6
+    SN = 0x7
+    FFNF = 0x8
+    MNF = 0x9
+
+    def __eq__(self, other):
+        if isinstance(other, Group):
+            return self.value == other.value
         else:
-            return None
-
-    @property
-    def __game_name__(cls):
-        return cls.__indexer__.__game_name__
-
-
-class Character(Comparable, metaclass=CharacterMeta):
-    __cnname_class__: Type[ChineseName] = ChineseName
-    __enname_class__: Type[EnglishName] = EnglishName
-    __jpname_class__: Type[JapaneseName] = JapaneseName
-    __alias_name_class__: Optional[Type[ChineseName]] = None
-    __indexer__: Optional[BaseIndexer] = None
-
-    def _index(self):
-        raise NotImplementedError  # pragma: no cover
-
-    @property
-    def index(self):
-        return self._index()
-
-    def _cnname(self):
-        raise NotImplementedError  # pragma: no cover
-
-    def _cnnames(self):
-        cnname = self._cnname()
-        return [cnname] if cnname else []
-
-    @property
-    def cnname(self):
-        cnname = self._cnname()
-        return self.__cnname_class__(cnname) if cnname else None
-
-    @property
-    def cnnames(self):
-        names = [self.__cnname_class__(name) for name in self._cnnames() if name]
-        return [name for name in names if name]
-
-    def _jpname(self):
-        raise NotImplementedError  # pragma: no cover
-
-    def _jpnames(self):
-        jpname = self._jpname()
-        return [jpname] if jpname else []
-
-    @property
-    def jpname(self):
-        jpname = self._jpname()
-        return self.__jpname_class__(jpname) if jpname else None
-
-    @property
-    def jpnames(self):
-        names = [self.__jpname_class__(name) for name in self._jpnames() if name]
-        return [name for name in names if name]
-
-    def _enname(self):
-        raise NotImplementedError  # pragma: no cover
-
-    def _ennames(self):
-        enname = self._enname()
-        return [enname] if enname else []
-
-    @property
-    def enname(self):
-        enname = self._enname()
-        return self.__enname_class__(enname) if enname else None
-
-    @property
-    def ennames(self):
-        names = [self.__enname_class__(name) for name in self._ennames() if name]
-        return [name for name in names if name]
-
-    def _alias_names(self):
-        return []
-
-    @property
-    def alias_names(self):
-        return [self.__alias_name_class__(name) for name in self._alias_names()]
-
-    def _names(self) -> List[_BaseName]:
-        return [*self.cnnames, *self.ennames, *self.jpnames]
+            try:
+                return self == Group.loads(other)
+            except (TypeError, ValueError):
+                return False
 
-    @property
-    def names(self) -> List[str]:
-        return sorted(set(map(str, self._names())))
-
-    def _gender(self):
-        raise NotImplementedError  # pragma: no cover
-
-    @property
-    def gender(self) -> Gender:
-        return Gender.loads(self._gender())
-
-    def _is_extra(self) -> bool:
-        return False
-
-    @property
-    def is_extra(self) -> bool:
-        return bool(self._is_extra())
+    @classmethod
+    def loads(cls, val) -> 'Group':
+        """
+        Load a Group value from a string or an int.
+
+        :param val: The value to load.
+        :type val: Union[str, int]
+        :return: The loaded Group value.
+        :rtype: Group
+        """
+        if isinstance(val, cls):
+            return val
+        elif isinstance(val, str):
+            if val == '白鹰':
+                return cls.USS
+            elif val == '皇家':
+                return cls.HMS
+            elif val == '重樱':
+                return cls.IJN
+            elif val == '铁血':
+                return cls.KMS
+            elif val == '东煌':
+                return cls.DE
+            elif val == '撒丁帝国':
+                return cls.RN
+            elif val == '北方联合':
+                return cls.SN
+            elif val == '自由鸢尾':
+                return cls.FFNF
+            elif val == '维希教廷':
+                return cls.MNF
+            else:
+                raise ValueError(f'Invalid group value - {val!r}.')
+        else:
+            raise TypeError(f'Invalid group type - {val!r}.')
 
-    def _skins(self) -> List[Tuple[str, str]]:
-        raise NotImplementedError
 
-    @property
-    def skins(self) -> List[Skin]:
-        return [Skin(name, url) for name, url in self._skins()]
+@unique
+class BasicRarity(IntEnum):
+    """
+    An enumeration representing the basic rarity levels in the Azur Lane game.
+    """
+
+    COMMON = 0x1
+    RARE = 0x2
+    ELITE = 0x3
+    ULTRA = 0x4
+    EPIC = 0x5
+
+    @property
+    def label(self) -> str:
+        """
+        Get the label corresponding to the rarity level.
+
+        :return: The label of the rarity level.
+        :rtype: str
+        """
+        if self == self.COMMON:
+            return '普通'
+        elif self == self.RARE:
+            return '稀有'
+        elif self == self.ELITE:
+            return '精锐'
+        elif self == self.ULTRA:
+            return '超稀有'
+        elif self == self.EPIC:
+            return '海上传奇'
+        else:
+            raise ValueError(f'Unknown basic level - {self!r}.')  # pragma: no cover
 
-    def _release_time(self):
-        raise NotImplementedError  # pragma: no cover
+    def __eq__(self, other):
+        if isinstance(other, BasicRarity):
+            return self.value == other.value
+        else:
+            try:
+                return self == self.loads(other)
+            except (TypeError, ValueError):
+                return False
 
-    @property
-    def release_time(self) -> Optional[float]:
-        return self._release_time()
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
-    def _order(self):
-        return ()
+    @classmethod
+    def loads(cls, val) -> 'BasicRarity':
+        """
+        Load a BasicRarity value from a string or an int.
+
+        :param val: The value to load.
+        :type val: Union[str, int]
+        :return: The loaded BasicRarity value.
+        :rtype: BasicRarity
+        """
+        if isinstance(val, cls):
+            return val
+        elif isinstance(val, int):
+            for name, item in cls.__members__.items():
+                if item.value == val:
+                    return item
+
+            raise ValueError(f'Invalid level value - {val!r}.')
+        elif isinstance(val, str):
+            if val == '普通':
+                return cls.COMMON
+            elif val == '稀有':
+                return cls.RARE
+            elif val == '精锐':
+                return cls.ELITE
+            elif val == '超稀有':
+                return cls.ULTRA
+            elif val == '海上传奇':
+                return cls.EPIC
+            else:
+                raise ValueError(f'Invalid level string - {val!r}.')
+        else:
+            raise TypeError(f'Invalid level type - {val!r}.')
 
-    def _key(self):
-        return self._order(), self._index(), (1 if self._is_extra() else 0)
 
-    def __eq__(self, other) -> bool:
-        if type(other) == type(self):
-            return self.index == other.index
-        else:
-            if self.index is not None and self.index == other:
-                return True
-            for name in chain(self._names(), self.alias_names):
-                if name == other:
-                    return True
+@unique
+class ResearchRarity(IntEnum):
+    """
+    An enumeration representing the research rarity levels in the Azur Lane game.
+    """
+
+    TOP = 0x4
+    DECISIVE = 0x5
+
+    @property
+    def label(self) -> str:
+        """
+        Get the label corresponding to the research rarity level.
+
+        :return: The label of the research rarity level.
+        :rtype: str
+        """
+        if self == self.TOP:
+            return '最高方案'
+        elif self == self.DECISIVE:
+            return '决战方案'
+        else:
+            raise ValueError(f'Unknown research level - {self!r}.')  # pragma: no cover
 
-            return False
+    def __eq__(self, other):
+        if isinstance(other, ResearchRarity):
+            return self.value == other.value
+        else:
+            try:
+                return self == self.loads(other)
+            except (TypeError, ValueError):
+                return False
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     @classmethod
-    def _simple_all(cls, timeout: int = 5, contains_extra: bool = True, **kwargs):
-        all_chs = [cls(data) for data in cls.__index_func__(timeout=timeout)]
-        chs = [ch for ch in all_chs if contains_extra or not ch.is_extra]
-        return chs
-
-    @classmethod
-    def all(cls, timeout: int = 5, contains_extra: bool = True, **kwargs):
-        return sorted(cls._simple_all(timeout, contains_extra, **kwargs))
-
-    @classmethod
-    def get(cls, name, **kwargs):
-        for item in cls.all(**kwargs):
-            if item == name:
-                return item
-
-        return None
-
-
-def _yield_all_characters(ch: Union[Character, list, tuple, Type[Character]], **kwargs) -> Iterator[Character]:
-    if isinstance(ch, Character):
-        yield ch
-    elif isinstance(ch, type) and issubclass(ch, Character):
-        yield from ch.all(**kwargs)
-    elif isinstance(ch, (list, tuple)):
-        for item in ch:
-            yield from _yield_all_characters(item, **kwargs)
-
-
-def list_all_characters(*chs: Union[Character, list, tuple, Type[Character]], **kwargs) -> List[Character]:
-    return list(_yield_all_characters(chs, **kwargs))
+    def loads(cls, val) -> 'ResearchRarity':
+        """
+        Load a ResearchRarity value from a string or an int.
+
+        :param val: The value to load.
+        :type val: Union[str, int]
+        :return: The loaded ResearchRarity value.
+        :rtype: ResearchRarity
+        """
+        if isinstance(val, cls):
+            return val
+        elif isinstance(val, int):
+            for name, item in cls.__members__.items():
+                if item.value == val:
+                    return item
+
+            raise ValueError(f'Invalid level value - {val!r}.')
+        elif isinstance(val, str):
+            if val == '最高方案':
+                return cls.TOP
+            elif val == '决战方案':
+                return cls.DECISIVE
+            else:
+                raise ValueError(f'Invalid level string - {val!r}.')
+        else:
+            raise TypeError(f'Invalid level type - {val!r}.')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gchar-0.0.9/gchar/games/fgo/character.py` & `gchar-0.1.0/gchar/games/fgo/character.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import re
 from functools import lru_cache
 from typing import List, Optional, Tuple
 
-from .index import INDEXER
 from .name import ChineseName, JapaneseName, EnglishName, ChineseAliasName
 from .property import Rarity, Clazz
 from ..base import Character as _BaseCharacter
 
 
 class Character(_BaseCharacter):
+    __game_name__ = 'fgo'
+    __official_name__ = 'Fate/Grand Order'
     __cnname_class__ = ChineseName
     __jpname_class__ = JapaneseName
     __enname_class__ = EnglishName
     __alias_name_class__ = ChineseAliasName
-    __indexer__ = INDEXER
 
     def __init__(self, raw_data: dict):
         self.__raw_data = raw_data
 
-    @property
-    def raw_data(self) -> dict:
-        return dict(self.__raw_data)
-
     def _index(self) -> int:
         return self.__raw_data['id']
 
     def _gender(self):
         return self.__raw_data['gender']
 
     @property
@@ -70,15 +66,15 @@
 
     def _enname(self):
         return self._ennames()[0]
 
     def _ennames(self):
         return self.__raw_data['ennames']
 
-    def _alias_names(self):
+    def _custom_alias_names(self):
         return self.__raw_data['alias']
 
     def _is_extra(self) -> bool:
         for ch in self.__raw_data['similar']:
             id_ = ch['id']
             the_ch = self._get_by_id(id_)
             if id_ < self.__raw_data['id'] and the_ch is not None and \
```

### Comparing `gchar-0.0.9/gchar/games/genshin/character.py` & `gchar-0.1.0/gchar/games/girlsfrontline/character.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-from typing import List, Optional, Tuple
+from typing import List, Tuple
 
-from .index import INDEXER
-from .name import EnglishName, JapaneseName, ChineseName
-from .property import Rarity, Weapon, Element
+import math
+
+from .name import EnglishName, JapaneseName, ChineseName, ChineseAliasName
+from .property import Rarity, Clazz
 from ..base import Character as _BaseCharacter
 
 
 class Character(_BaseCharacter):
-    __cnname_class__ = ChineseName
+    __game_name__ = 'girlsfrontline'
+    __official_name__ = 'Girls\' Frontline'
     __enname_class__ = EnglishName
+    __cnname_class__ = ChineseName
     __jpname_class__ = JapaneseName
-    __indexer__ = INDEXER
+    __alias_name_class__ = ChineseAliasName
 
     def __init__(self, raw_data: dict):
         self.__raw_data = raw_data
 
-    def _index(self) -> str:
-        return str(self.enname)
-
-    def _gender(self):
-        return self.__raw_data['gender']
+    def _index(self) -> int:
+        return self.__raw_data['id']
 
     def _cnname(self):
         return self.__raw_data['cnname']
 
+    def _cnnames(self):
+        return self.__raw_data['cnnames']
+
     def _enname(self):
         return self.__raw_data['enname']
 
     def _jpname(self):
-        _jpnames = self._jpnames()
-        if _jpnames:
-            return _jpnames[0]
-        else:
-            return None  # pragma: no cover
+        return self.__raw_data['jpname']
 
-    def _jpnames(self):
-        return self.__raw_data['jpnames']
+    def _custom_alias_names(self):
+        return self.__raw_data['alias']
+
+    def _gender(self):
+        return 'female'
 
     @property
     def rarity(self) -> Rarity:
         return Rarity.loads(self.__raw_data['rarity'])
 
     @property
-    def weapon(self) -> Weapon:
-        return Weapon.loads(self.__raw_data['weapon'])
-
-    @property
-    def element(self) -> Optional[Element]:
-        element = self.__raw_data['element']
-        if element:
-            return Element.loads(element)
-        else:
-            return None
+    def clazz(self) -> Clazz:
+        return Clazz.loads(self.__raw_data['class'])
 
     def _skins(self) -> List[Tuple[str, str]]:
-        return [(item['name'], item['url']) for item in self.__raw_data['skins']]
+        return [(item['desc'], item['url']) for item in self.__raw_data['skins']]
 
     def _release_time(self):
         release_info = self.__raw_data['release']
         return release_info['time']
 
     def _order(self):
-        return self._release_time()
+        _release_time = self._release_time()
+        return _release_time if _release_time is not None else math.inf
 
     def __repr__(self):
-        return f'<{type(self).__name__} {"/".join(map(str, self._names()))}, ' \
-               f'{self.gender.name.lower()}, {self.rarity}{"*" * self.rarity}, ' \
-               f'weapon: {self.weapon}, element: {self.element}>'
+        if isinstance(self.rarity.value, int):
+            _rarity_repr = f'{self.rarity.value}{"*" * self.rarity.value}'
+        else:
+            _rarity_repr = f'{self.rarity.name}'
+
+        return f'<{type(self).__name__} {self.index} - {"/".join(map(str, self._names()))}, ' \
+               f'{_rarity_repr}, clazz: {self.clazz}>'
```

### Comparing `gchar-0.0.9/gchar/games/girlsfrontline/character.py` & `gchar-0.1.0/gchar/games/neuralcloud/character.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,98 @@
-import math
-from typing import List, Tuple
+from typing import List, Tuple, Mapping, Optional
 
-from .index import INDEXER
-from .name import EnglishName, JapaneseName, ChineseName, ChineseAliasName
-from .property import Rarity, Clazz
+from .name import EnglishName, ChineseName, ChineseAliasName, JapaneseName
+from .property import Clazz, Rarity
 from ..base import Character as _BaseCharacter
+from ..girlsfrontline import Character as GFCharacter
+from ...utils import optional_lru_cache
 
 
 class Character(_BaseCharacter):
+    __game_name__ = 'neuralcloud'
+    __official_name__ = 'Neural Cloud'
     __enname_class__ = EnglishName
     __cnname_class__ = ChineseName
     __jpname_class__ = JapaneseName
     __alias_name_class__ = ChineseAliasName
-    __indexer__ = INDEXER
 
     def __init__(self, raw_data: dict):
         self.__raw_data = raw_data
 
     def _index(self) -> int:
         return self.__raw_data['id']
 
     def _cnname(self):
         return self.__raw_data['cnname']
 
-    def _cnnames(self):
-        return self.__raw_data['cnnames']
+    @property
+    def cnnames(self):
+        names = [self.__cnname_class__(name) for name in self._cnnames() if name]
+        if self.gf_char:
+            names.extend(self.gf_char.cnnames)
 
-    def _enname(self):
-        return self.__raw_data['enname']
+        return [name for name in names if name]
 
     def _jpname(self):
         return self.__raw_data['jpname']
 
-    def _alias_names(self):
+    @property
+    def jpnames(self):
+        names = [self.__jpname_class__(name) for name in self._jpnames() if name]
+        if self.gf_char:
+            names.extend(self.gf_char.jpnames)
+        return [name for name in names if name]
+
+    def _enname(self):
+        return self.__raw_data['enname']
+
+    @property
+    def ennames(self):
+        names = [self.__enname_class__(name) for name in self._ennames() if name]
+        if self.gf_char:
+            names.extend(self.gf_char.ennames)
+        return [name for name in names if name]
+
+    def _custom_alias_names(self):
         return self.__raw_data['alias']
 
     def _gender(self):
-        return 'female'
+        return self.__raw_data['gender']
+
+    @property
+    def clazz(self) -> Clazz:
+        return Clazz.loads(self.__raw_data['class'])
 
     @property
     def rarity(self) -> Rarity:
         return Rarity.loads(self.__raw_data['rarity'])
 
     @property
-    def clazz(self) -> Clazz:
-        return Clazz.loads(self.__raw_data['class'])
+    def company(self) -> str:
+        return self.__raw_data.get('company', None)
+
+    @property
+    def gf_char(self) -> Optional[GFCharacter]:
+        if self.__raw_data["gf"]:
+            return self._list_index_of_gf()[self.__raw_data["gf"]["id"]]
+        else:
+            return None
 
     def _skins(self) -> List[Tuple[str, str]]:
-        return [(item['desc'], item['url']) for item in self.__raw_data['skins']]
+        return [(item['name'], item['url']) for item in self.__raw_data['skins']]
+
+    def __repr__(self):
+        # return f'233 {type(self).__name__} {self.index} {self._names()} {self.rarity} {self.clazz}'
+        return f'<{type(self).__name__} {self.index} - {"/".join(map(str, self._names()))}, ' \
+               f'rarity: {self.rarity}{"*" * self.rarity}, clazz: {self.clazz.name}>'
 
     def _release_time(self):
         release_info = self.__raw_data['release']
         return release_info['time']
 
     def _order(self):
-        _release_time = self._release_time()
-        return _release_time if _release_time is not None else math.inf
-
-    def __repr__(self):
-        if isinstance(self.rarity.value, int):
-            _rarity_repr = f'{self.rarity.value}{"*" * self.rarity.value}'
-        else:
-            _rarity_repr = f'{self.rarity.name}'
+        return self._release_time()
 
-        return f'<{type(self).__name__} {self.index} - {"/".join(map(str, self._names()))}, ' \
-               f'{_rarity_repr}, clazz: {self.clazz}>'
+    @classmethod
+    @optional_lru_cache()
+    def _list_index_of_gf(cls) -> Mapping[int, GFCharacter]:
+        return {ch.index: ch for ch in GFCharacter.all(contains_extra=False)}
```

### Comparing `gchar-0.0.9/gchar/games/girlsfrontline/name.py` & `gchar-0.1.0/gchar/games/girlsfrontline/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.9/gchar/games/girlsfrontline/property.py` & `gchar-0.1.0/gchar/games/girlsfrontline/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.9/gchar/games/neuralcloud/character.py` & `gchar-0.1.0/gchar/games/genshin/character.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,69 @@
-from typing import List, Tuple, Mapping, Optional
+from typing import List, Optional, Tuple
 
-from .index import INDEXER
-from .name import EnglishName, ChineseName, ChineseAliasName, JapaneseName
-from .property import Clazz, Rarity
+from .name import EnglishName, JapaneseName, ChineseName
+from .property import Rarity, Weapon, Element
 from ..base import Character as _BaseCharacter
-from ..girlsfrontline import Character as GFCharacter
-from ...utils import optional_lru_cache
 
 
 class Character(_BaseCharacter):
-    __enname_class__ = EnglishName
+    __game_name__ = 'genshin'
+    __official_name__ = 'Genshin Impact'
     __cnname_class__ = ChineseName
+    __enname_class__ = EnglishName
     __jpname_class__ = JapaneseName
-    __alias_name_class__ = ChineseAliasName
-    __indexer__ = INDEXER
 
     def __init__(self, raw_data: dict):
         self.__raw_data = raw_data
 
-    def _index(self) -> int:
-        return self.__raw_data['id']
+    def _index(self) -> str:
+        return str(self.enname)
+
+    def _gender(self):
+        return self.__raw_data['gender']
 
     def _cnname(self):
         return self.__raw_data['cnname']
 
-    @property
-    def cnnames(self):
-        names = [self.__cnname_class__(name) for name in self._cnnames() if name]
-        if self.gf_char:
-            names.extend(self.gf_char.cnnames)
-
-        return [name for name in names if name]
-
-    def _jpname(self):
-        return self.__raw_data['jpname']
-
-    @property
-    def jpnames(self):
-        names = [self.__jpname_class__(name) for name in self._jpnames() if name]
-        if self.gf_char:
-            names.extend(self.gf_char.jpnames)
-        return [name for name in names if name]
-
     def _enname(self):
         return self.__raw_data['enname']
 
-    @property
-    def ennames(self):
-        names = [self.__enname_class__(name) for name in self._ennames() if name]
-        if self.gf_char:
-            names.extend(self.gf_char.ennames)
-        return [name for name in names if name]
-
-    def _alias_names(self):
-        return self.__raw_data['alias']
-
-    def _gender(self):
-        return self.__raw_data['gender']
+    def _jpname(self):
+        _jpnames = self._jpnames()
+        if _jpnames:
+            return _jpnames[0]
+        else:
+            return None  # pragma: no cover
 
-    @property
-    def clazz(self) -> Clazz:
-        return Clazz.loads(self.__raw_data['class'])
+    def _jpnames(self):
+        return self.__raw_data['jpnames']
 
     @property
     def rarity(self) -> Rarity:
         return Rarity.loads(self.__raw_data['rarity'])
 
     @property
-    def company(self) -> str:
-        return self.__raw_data.get('company', None)
+    def weapon(self) -> Weapon:
+        return Weapon.loads(self.__raw_data['weapon'])
 
     @property
-    def gf_char(self) -> Optional[GFCharacter]:
-        if self.__raw_data["gf"]:
-            return self._list_index_of_gf()[self.__raw_data["gf"]["id"]]
+    def element(self) -> Optional[Element]:
+        element = self.__raw_data['element']
+        if element:
+            return Element.loads(element)
         else:
             return None
 
     def _skins(self) -> List[Tuple[str, str]]:
         return [(item['name'], item['url']) for item in self.__raw_data['skins']]
 
-    def __repr__(self):
-        # return f'233 {type(self).__name__} {self.index} {self._names()} {self.rarity} {self.clazz}'
-        return f'<{type(self).__name__} {self.index} - {"/".join(map(str, self._names()))}, ' \
-               f'rarity: {self.rarity}{"*" * self.rarity}, clazz: {self.clazz.name}>'
-
     def _release_time(self):
         release_info = self.__raw_data['release']
         return release_info['time']
 
     def _order(self):
         return self._release_time()
 
-    @classmethod
-    @optional_lru_cache()
-    def _list_index_of_gf(cls) -> Mapping[int, GFCharacter]:
-        return {ch.index: ch for ch in GFCharacter.all(contains_extra=False)}
+    def __repr__(self):
+        return f'<{type(self).__name__} {"/".join(map(str, self._names()))}, ' \
+               f'{self.gender.name.lower()}, {self.rarity}{"*" * self.rarity}, ' \
+               f'weapon: {self.weapon}, element: {self.element}>'
```

### Comparing `gchar-0.0.9/gchar/games/neuralcloud/property.py` & `gchar-0.1.0/gchar/games/neuralcloud/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.9/gchar/utils/cli.py` & `gchar-0.1.0/gchar/utils/cli.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.9/gchar.egg-info/PKG-INFO` & `gchar-0.1.0/gchar.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gchar
-Version: 0.0.9
+Version: 0.1.0
 Summary: Game character manager.
 Home-page: https://github.com/narugo1992/gchar
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,19 +12,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: crawl
-Provides-Extra: speedup
 Provides-Extra: test
+Provides-Extra: speedup
 Provides-Extra: doc
 License-File: LICENSE
 
 # gchar
 
 [![PyPI](https://img.shields.io/pypi/v/gchar)](https://pypi.org/project/gchar/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gchar)
@@ -55,46 +55,73 @@
 
 ```shell
 pip install gchar
 ```
 
 ## Quick Start
 
+### Game Character Query
+
 Find the characters (nicknames are supported for arknights and fgo)
 
+Currently Supported Games (If you need data of other games,
+you can [create an issue](https://github.com/narugo1992/gchar/issues/new)):
+
+* Arknights (crawled from [PRTS Wiki](https://prts.wiki))
+* Fate/Grand Order (crawled from [FGO Wiki](https://fgo.wiki))
+* Azur Lane (crawled from [BiliGame Wiki](https://wiki.biligame.com/blhx))
+* Girls' Front-Line (crawled from [IOPWiki](https://iopwiki.com/))
+* Genshin Impact (crawled from [Fandom](https://genshin-impact.fandom.com/ja/wiki/%E5%8E%9F%E7%A5%9E_Wiki))
+* Neural Cloud (crawled from [42lab wiki](http://wiki.42lab.cloud))
+* Blue Archive (crawled from [bluearchive wiki](https://bluearchive.wiki/) and [Gamekee BA](https://ba.gamekee.com))
+* Nikke: Goddess of Victory (crawled from [Fandom](https://nikke-goddess-of-victory-international.fandom.com)
+  and [Gamekee Nikke](https://nikke.gamekee.com))
+* Path To Nowhere (crawled from [BiliGame Wiki](https://wiki.biligame.com/wqmt))
+* Honkai: Star Rail (crawled from [Star Rail Station](https://starrailstation.com)
+  and [BiliGame Wiki](https://wiki.biligame.com))
+
 ```
 >>> from gchar.games import get_character
 >>> 
->>> get_character('CEO')
-<Character 171 - 彭忒西勒亚/黄金国的berserker/penthesilea/berserker_of_el_dorado/ペンテシレイア/エルドラドのバーサーカー, female, 4****>
->>> get_character('黑呆')
-<Character 3 - 阿尔托莉雅·潘德拉贡〔alter〕/altria_pendragon_alter/アルトリア・ペンドラゴン〔オルタ〕, female, 4****>
->>> get_character('amiya')
+>>> get_character('amiya')  # english name
 <Character R001 - 阿米娅/amiya/アーミヤ, female, 5*****>
->>> get_character('小火龙')
-<Character RL03 - 伊芙利特/ifrit/イフリータ, female, 6******>
->>> get_character('宵宫')
-<Character 宵宫/yoimiya/宵宮/よいみや, female, 5*****, weapon: Weapon.BOW, element: Element.PYRO>
 >>> get_character('z18')
-<Character 346 - z18/hans_ludemann/ハンス・リューデマン, 稀有(2**), group: Group.KMS>
+<Character 346 - Z18/hans_ludemann/ハンス・リューデマン, 稀有(2**), group: Group.KMS>
 >>> get_character('416')
 <Character 65 - HK416/416/416, 5*****, clazz: Clazz.AR>
+>>> 
+>>> get_character('夕')  # chinese name
+<Character NM02 - 夕/dusk/シー, female, 6******>
+>>> get_character('宵宫')
+<Character 宵宫/yoimiya/宵宮/よいみや, female, 5*****, weapon: Weapon.BOW, element: Element.PYRO>
+>>> 
+>>> get_character('スルト')  # japanese name
+<Character R111 - 史尔特尔/surtr/スルト, female, 6******>
+>>> 
+>>> get_character('CEO')  # alias
+<Character 171 - 彭忒西勒亚/黄金国的Berserker/penthesilea/berserker_of_el_dorado/ペンテシレイア/エルドラドのバーサーカー, female, 4****, class: Clazz.BERSERKER>
+>>> get_character('黑呆')
+<Character 3 - 阿尔托莉雅·潘德拉贡〔Alter〕/altria_pendragon_alter/アルトリア・ペンドラゴン〔オルタ〕/アルトリア・ペンドラゴン・オルタ/アルトリア・オルタ, female, 4****, class: Clazz.SABER>
+>>> get_character('小火龙')
+<Character RL03 - 伊芙利特/ifrit/イフリータ, female, 6******>
 ```
 
 List all character with specific condition of one game
 
 ```python
 from gchar.games.arknights import Character
 
 for ch in Character.all():  # 5star, boys
     if ch.rarity == 5 and ch.gender == 'male':
         print(ch)
 
 ```
 
+### Pixiv Resources
+
 Get search keywords for pixiv
 
 ```
 >>> from gchar.resources.pixiv import get_pixiv_keywords
 >>> 
 >>> get_pixiv_keywords('CEO')
 'Fate/GrandOrder (berserker_of_el_dorado OR penthesilea OR エルドラドのバーサーカー OR ペンテシレイア OR 彭忒西勒亚 OR 黄金国的berserker)'
@@ -106,49 +133,75 @@
 'アークナイツ (blaze OR ブレイズ OR 煌)'
 >>> get_pixiv_keywords('林雨霞')
 'アークナイツ (lin OR 林) -angelina -flint -folinic -ling -守林人 -巡林者 -杜林'
 >>> get_pixiv_keywords('夕')
 'アークナイツ (dusk OR シー OR 夕) -ケルシー -シージ -シーン'
 ```
 
-Get tags for danbooru
+See how many posts on pixiv
+
+```
+>>> from gchar.resources.pixiv import get_pixiv_posts
+>>> 
+>>> # first one is all, second one is r18
+>>> get_pixiv_posts('CEO')
+(867, 113)
+>>> get_pixiv_posts('黑贞')
+(21908, 3820)
+>>> get_pixiv_posts('amiya')
+(14130, 1113)
+>>> get_pixiv_posts('blazer')  # fuzzy match is supported, but slower
+(1967, 383)
+>>> get_pixiv_posts('林雨霞')
+(259, 44)
+>>> get_pixiv_posts('夕')
+(2908, 424)
+```
+
+### Other Sites' Resource
+
+Get tags for danbooru and other sites
+
+Currently supported sites:
+
+* [Anime Pictures](https://anime-pictures.net), named `anime_pictures`
+* [Atfbooru](https://booru.allthefallen.moe), named `atfbooru`
+* [Sankaku](https://chan.sankakucomplex.com), named `sankaku`
+* [Danbooru](https://danbooru.donmai.us), named `danbooru`
+* [Hypnohub](https://hypnohub.net), named `hypnohub`
+* [Konachan](https://konachan.com), named `konachan`
+* [Konachan.Net](https://konachan.net), named `konachan_net`
+* [Lolibooru](https://lolibooru.moe), named `lolibooru`
+* [Rule34](https://rule34.xxx), named `rule34`
+* [Safebooru](https://safebooru.donmai.us), named `safebooru`
+* [Xbooru](https://xbooru.com), named `xbooru`
+* [Yande](https://yande.re), named `yande`
+* [Zerochan](https://zerochan.net), named `zerochan`
 
 ```
->>> from gchar.resources.danbooru import get_danbooru_tag
+>>> from gchar.resources.sites import get_site_tag
 >>> 
->>> get_danbooru_tag('CEO')
+>>> # first one is all, second one is r18
+>>> get_site_tag('CEO', 'danbooru')
 'penthesilea_(fate)'
->>> get_danbooru_tag('黑贞')
+>>> get_site_tag('黑贞', 'danbooru')
 "jeanne_d'arc_alter_(fate)"
->>> get_danbooru_tag('amiya')
+>>> get_site_tag('amiya', 'danbooru')
 'amiya_(arknights)'
->>> get_danbooru_tag('blazer')  # fuzzy match is supported
-'blaze_(arknights)'
->>> get_danbooru_tag('林雨霞')
+>>> get_site_tag('林雨霞', 'danbooru')
 'lin_(arknights)'
->>> get_danbooru_tag('夕')
+>>> get_site_tag('夕', 'danbooru')
 'dusk_(arknights)'
+>>> get_site_tag('夕', 'danbooru', with_posts=True)  # see how many images
+('dusk_(arknights)', 1397)
+>>> get_site_tag('夕', 'zerochan')  # another sites
+'Dusk (Arknights)'
 ```
 
-Currently Supported Games (If you need data of other games,
-you can [create an issue](https://github.com/narugo1992/gchar/issues/new)):
-
-* Arknights (crawled from [https://prts.wiki](https://prts.wiki))
-* Fate/Grand Order (crawled from [https://fgo.wiki](https://fgo.wiki))
-* Azur Lane (crawled from [https://wiki.biligame.com/blhx](https://wiki.biligame.com/blhx))
-* Girls' Front-Line (crawled from [https://iopwiki.com/](https://iopwiki.com/))
-* Genshin Impact (crawled
-  from [https://genshin-impact.fandom.com/ja/wiki/%E5%8E%9F%E7%A5%9E_Wiki](https://genshin-impact.fandom.com/ja/wiki/%E5%8E%9F%E7%A5%9E_Wiki))
-
 ## FAQ
 
-### The data here is out-of-date
+Q: How timely is the data?
 
-Just update the local data with the following commands.
-
-```shell
-python -m gchar update        # download newest data of all the games
-python -m gchar update -g fgo # download newest data of fgo
-python -m gchar update --help # help information
-
-```
+A: The data is updated approximately once a day and is hosted on Github Action, ensuring its timeliness. In the event of
+a malfunction on the crawled Wiki site that prevents data updates, the corresponding Wiki team will be contacted to
+resolve the issue.
```

### Comparing `gchar-0.0.9/gchar.egg-info/requires.txt` & `gchar-0.1.0/gchar.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-hbutils>=0.8.1
+hbutils>=0.9.1
 tqdm>=4.0.0
 click>=7.0.0
 transliterate>=1.10.2
+huggingface_hub>=0.14.0
 unidecode
-pyquery
 thefuzz
 editdistance
 requests
 pyyaml
 
-[crawl]
-numpy
-hfmirror>=0.0.2
-
 [doc]
 Jinja2~=3.0.0
 sphinx~=3.2.0
 sphinx_rtd_theme~=0.4.3
 enum_tools
 sphinx-toolbox
 plantumlcli>=0.0.2
@@ -40,7 +36,8 @@
 pytest-rerunfailures~=10.2
 pytest-timeout~=2.0.2
 pytest-benchmark~=3.4.0
 easydict<2,>=1.7
 testtools>=2
 where>=1.0.2
 responses>=0.20.0
+numpy
```

### Comparing `gchar-0.0.9/setup.py` & `gchar-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 def _load_req(file: str):
     with open(file, 'r', 'utf-8') as f:
         return [line.strip() for line in f.readlines() if line.strip()]
 
 
 requirements = _load_req('requirements.txt')
 
+_REQ_BLACKLIST = ['crawl']
 _REQ_PATTERN = re.compile('^requirements-([a-zA-Z0-9_]+)\\.txt$')
 group_requirements = {
     item.group(1): _load_req(item.group(0))
-    for item in [_REQ_PATTERN.fullmatch(reqpath) for reqpath in os.listdir()] if item
+    for item in [_REQ_PATTERN.fullmatch(reqpath) for reqpath in os.listdir()]
+    if item and item.group(1) not in _REQ_BLACKLIST
 }
 
 with open('README.md', 'r', 'utf-8') as f:
     readme = f.read()
 
 setup(
     # information
@@ -59,9 +61,10 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```


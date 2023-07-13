# Comparing `tmp/ezapi-tmdb-0.8.2.tar.gz` & `tmp/ezapi-tmdb-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezapi-tmdb-0.8.2.tar", last modified: Fri Mar 10 04:10:11 2023, max compression
+gzip compressed data, was "ezapi-tmdb-0.8.3.tar", last modified: Thu Jul 13 04:27:13 2023, max compression
```

## Comparing `ezapi-tmdb-0.8.2.tar` & `ezapi-tmdb-0.8.3.tar`

### file list

```diff
@@ -1,93 +1,98 @@
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.659233 ezapi-tmdb-0.8.2/
--rw-r--r--   0 zehengl    (501) staff       (20)      755 2022-04-13 06:13:13.000000 ezapi-tmdb-0.8.2/.all-contributorsrc
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.647063 ezapi-tmdb-0.8.2/.github/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.649539 ezapi-tmdb-0.8.2/.github/workflows/
--rw-r--r--   0 zehengl    (501) staff       (20)      245 2022-09-07 01:05:34.000000 ezapi-tmdb-0.8.2/.github/workflows/pcu.yml
--rw-r--r--   0 zehengl    (501) staff       (20)      889 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/.github/workflows/pytest.yml
--rw-r--r--   0 zehengl    (501) staff       (20)       72 2022-04-28 05:13:36.000000 ezapi-tmdb-0.8.2/.gitignore
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.649949 ezapi-tmdb-0.8.2/.vscode/
--rw-r--r--   0 zehengl    (501) staff       (20)      437 2022-04-13 06:13:13.000000 ezapi-tmdb-0.8.2/.vscode/extensions.json
--rw-r--r--   0 zehengl    (501) staff       (20)      584 2022-04-13 06:13:13.000000 ezapi-tmdb-0.8.2/.vscode/settings.json
--rw-r--r--   0 zehengl    (501) staff       (20)     1066 2022-04-13 06:13:13.000000 ezapi-tmdb-0.8.2/LICENSE
--rw-r--r--   0 zehengl    (501) staff       (20)     5891 2023-03-10 04:10:11.659062 ezapi-tmdb-0.8.2/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)     5331 2023-01-22 23:27:25.000000 ezapi-tmdb-0.8.2/README.md
--rw-r--r--   0 zehengl    (501) staff       (20)     1089 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/pyproject.toml
--rw-r--r--   0 zehengl    (501) staff       (20)      127 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/requirements-dev.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       49 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/requirements-test.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-03-01 02:19:37.000000 ezapi-tmdb-0.8.2/requirements.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-03-10 04:10:11.659273 ezapi-tmdb-0.8.2/setup.cfg
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.647325 ezapi-tmdb-0.8.2/src/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.650728 ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/
--rw-r--r--   0 zehengl    (501) staff       (20)     5891 2023-03-10 04:10:11.000000 ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/PKG-INFO
--rw-r--r--   0 zehengl    (501) staff       (20)     2122 2023-03-10 04:10:11.000000 ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/SOURCES.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-03-10 04:10:11.000000 ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/dependency_links.txt
--rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-03-10 04:10:11.000000 ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/requires.txt
--rw-r--r--   0 zehengl    (501) staff       (20)        5 2023-03-10 04:10:11.000000 ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/top_level.txt
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.651030 ezapi-tmdb-0.8.2/src/tmdb/
--rw-r--r--   0 zehengl    (501) staff       (20)       65 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/__init__.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.651753 ezapi-tmdb-0.8.2/src/tmdb/four/
--rw-r--r--   0 zehengl    (501) staff       (20)     1395 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/four/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)     2581 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/four/account.py
--rw-r--r--   0 zehengl    (501) staff       (20)      711 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/four/auth.py
--rw-r--r--   0 zehengl    (501) staff       (20)       73 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/four/base.py
--rw-r--r--   0 zehengl    (501) staff       (20)      607 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/four/list.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.655275 ezapi-tmdb-0.8.2/src/tmdb/three/
--rw-r--r--   0 zehengl    (501) staff       (20)     2496 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/__init__.py
--rw-r--r--   0 zehengl    (501) staff       (20)     3841 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/account.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1818 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/authentication.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1326 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/base.py
--rw-r--r--   0 zehengl    (501) staff       (20)      552 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/certifications.py
--rw-r--r--   0 zehengl    (501) staff       (20)      717 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/changes.py
--rw-r--r--   0 zehengl    (501) staff       (20)      897 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/collections.py
--rw-r--r--   0 zehengl    (501) staff       (20)      856 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/companies.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1464 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/configuration.py
--rw-r--r--   0 zehengl    (501) staff       (20)      303 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/credits.py
--rw-r--r--   0 zehengl    (501) staff       (20)      494 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/discover.py
--rw-r--r--   0 zehengl    (501) staff       (20)      361 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/find.py
--rw-r--r--   0 zehengl    (501) staff       (20)      504 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/genres.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1006 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/guest_sessions.py
--rw-r--r--   0 zehengl    (501) staff       (20)      566 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/keywords.py
--rw-r--r--   0 zehengl    (501) staff       (20)     2261 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/lists.py
--rw-r--r--   0 zehengl    (501) staff       (20)     5981 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/movies.py
--rw-r--r--   0 zehengl    (501) staff       (20)      855 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/networks.py
--rw-r--r--   0 zehengl    (501) staff       (20)     2859 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/people.py
--rw-r--r--   0 zehengl    (501) staff       (20)      303 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/reviews.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1843 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/search.py
--rw-r--r--   0 zehengl    (501) staff       (20)      346 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/trending.py
--rw-r--r--   0 zehengl    (501) staff       (20)     5922 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/tv.py
--rw-r--r--   0 zehengl    (501) staff       (20)      354 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/tv_episode_groups.py
--rw-r--r--   0 zehengl    (501) staff       (20)     3990 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/tv_episodes.py
--rw-r--r--   0 zehengl    (501) staff       (20)     2188 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/tv_seasons.py
--rw-r--r--   0 zehengl    (501) staff       (20)      769 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/src/tmdb/three/watch_providers.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.647647 ezapi-tmdb-0.8.2/tests/
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.655413 ezapi-tmdb-0.8.2/tests/four/
--rw-r--r--   0 zehengl    (501) staff       (20)     2377 2022-08-19 06:09:38.000000 ezapi-tmdb-0.8.2/tests/four/test_v4.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.658728 ezapi-tmdb-0.8.2/tests/three/
--rw-r--r--   0 zehengl    (501) staff       (20)      850 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/conftest.py
-drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-03-10 04:10:11.658844 ezapi-tmdb-0.8.2/tests/three/helpers/
--rw-r--r--   0 zehengl    (501) staff       (20)      170 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/helpers/utils.py
--rw-r--r--   0 zehengl    (501) staff       (20)     2145 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_account.py
--rw-r--r--   0 zehengl    (501) staff       (20)      865 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_authentication.py
--rw-r--r--   0 zehengl    (501) staff       (20)      231 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_certifications.py
--rw-r--r--   0 zehengl    (501) staff       (20)      321 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_changes.py
--rw-r--r--   0 zehengl    (501) staff       (20)      428 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_collections.py
--rw-r--r--   0 zehengl    (501) staff       (20)      390 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_companies.py
--rw-r--r--   0 zehengl    (501) staff       (20)      557 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_configuration.py
--rw-r--r--   0 zehengl    (501) staff       (20)      168 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_credits.py
--rw-r--r--   0 zehengl    (501) staff       (20)      207 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_discover.py
--rw-r--r--   0 zehengl    (501) staff       (20)      616 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_find.py
--rw-r--r--   0 zehengl    (501) staff       (20)      215 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_genres.py
--rw-r--r--   0 zehengl    (501) staff       (20)      671 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_guest_sessions.py
--rw-r--r--   0 zehengl    (501) staff       (20)      268 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_keywords.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1024 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_lists.py
--rw-r--r--   0 zehengl    (501) staff       (20)     3270 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_movies.py
--rw-r--r--   0 zehengl    (501) staff       (20)      385 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_networks.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1241 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_people.py
--rw-r--r--   0 zehengl    (501) staff       (20)      168 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_reviews.py
--rw-r--r--   0 zehengl    (501) staff       (20)      567 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_search.py
--rw-r--r--   0 zehengl    (501) staff       (20)      782 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_trending.py
--rw-r--r--   0 zehengl    (501) staff       (20)     3078 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_tv.py
--rw-r--r--   0 zehengl    (501) staff       (20)      208 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_tv_episode_groups.py
--rw-r--r--   0 zehengl    (501) staff       (20)     2369 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_tv_episodes.py
--rw-r--r--   0 zehengl    (501) staff       (20)     1332 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_tv_seasons.py
--rw-r--r--   0 zehengl    (501) staff       (20)      311 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.2/tests/three/test_watch_providers.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.907179 ezapi-tmdb-0.8.3/
+-rw-r--r--   0 zehengl    (501) staff       (20)     1032 2023-03-24 21:13:46.000000 ezapi-tmdb-0.8.3/.all-contributorsrc
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.890890 ezapi-tmdb-0.8.3/.github/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.894257 ezapi-tmdb-0.8.3/.github/workflows/
+-rw-r--r--   0 zehengl    (501) staff       (20)      308 2023-04-29 06:46:36.000000 ezapi-tmdb-0.8.3/.github/workflows/gh-deploy.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      243 2023-04-29 06:46:36.000000 ezapi-tmdb-0.8.3/.github/workflows/pcu.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)      934 2023-04-29 06:46:36.000000 ezapi-tmdb-0.8.3/.github/workflows/pytest.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)       72 2022-04-28 05:13:36.000000 ezapi-tmdb-0.8.3/.gitignore
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.894584 ezapi-tmdb-0.8.3/.vscode/
+-rw-r--r--   0 zehengl    (501) staff       (20)      437 2022-04-13 06:13:13.000000 ezapi-tmdb-0.8.3/.vscode/extensions.json
+-rw-r--r--   0 zehengl    (501) staff       (20)      584 2022-04-13 06:13:13.000000 ezapi-tmdb-0.8.3/.vscode/settings.json
+-rw-r--r--   0 zehengl    (501) staff       (20)     1066 2022-04-13 06:13:13.000000 ezapi-tmdb-0.8.3/LICENSE
+-rw-r--r--   0 zehengl    (501) staff       (20)     6080 2023-07-13 04:27:13.907004 ezapi-tmdb-0.8.3/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     5520 2023-03-24 21:13:46.000000 ezapi-tmdb-0.8.3/README.md
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.894785 ezapi-tmdb-0.8.3/docs/
+-rw-r--r--   0 zehengl    (501) staff       (20)      366 2023-03-13 07:16:12.000000 ezapi-tmdb-0.8.3/docs/index.md
+-rw-r--r--   0 zehengl    (501) staff       (20)     1387 2023-05-15 04:02:28.000000 ezapi-tmdb-0.8.3/mkdocs.yml
+-rw-r--r--   0 zehengl    (501) staff       (20)     1089 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/pyproject.toml
+-rw-r--r--   0 zehengl    (501) staff       (20)      152 2023-07-13 04:26:24.000000 ezapi-tmdb-0.8.3/requirements-dev.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)      143 2023-07-13 04:26:24.000000 ezapi-tmdb-0.8.3/requirements-docs.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       50 2023-07-13 04:26:24.000000 ezapi-tmdb-0.8.3/requirements-test.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-06-30 16:40:47.000000 ezapi-tmdb-0.8.3/requirements.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       38 2023-07-13 04:27:13.907221 ezapi-tmdb-0.8.3/setup.cfg
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.891302 ezapi-tmdb-0.8.3/src/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.895759 ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/
+-rw-r--r--   0 zehengl    (501) staff       (20)     6080 2023-07-13 04:27:13.000000 ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/PKG-INFO
+-rw-r--r--   0 zehengl    (501) staff       (20)     2201 2023-07-13 04:27:13.000000 ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/SOURCES.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        1 2023-07-13 04:27:13.000000 ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/dependency_links.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)       31 2023-07-13 04:27:13.000000 ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/requires.txt
+-rw-r--r--   0 zehengl    (501) staff       (20)        5 2023-07-13 04:27:13.000000 ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/top_level.txt
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.895897 ezapi-tmdb-0.8.3/src/tmdb/
+-rw-r--r--   0 zehengl    (501) staff       (20)       65 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/__init__.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.896856 ezapi-tmdb-0.8.3/src/tmdb/four/
+-rw-r--r--   0 zehengl    (501) staff       (20)     1395 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/four/__init__.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     2581 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/four/account.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      711 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/four/auth.py
+-rw-r--r--   0 zehengl    (501) staff       (20)       73 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/four/base.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      607 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/four/list.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.901587 ezapi-tmdb-0.8.3/src/tmdb/three/
+-rw-r--r--   0 zehengl    (501) staff       (20)     2496 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/__init__.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     3841 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/account.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1818 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/authentication.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1326 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/base.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      552 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/certifications.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      717 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/changes.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      897 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/collections.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      856 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/companies.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1464 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/configuration.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      303 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/credits.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      494 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/discover.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      361 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/find.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      504 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/genres.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1006 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/guest_sessions.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      566 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/keywords.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     2261 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/lists.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     5981 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/movies.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      855 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/networks.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     2859 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/people.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      303 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/reviews.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1843 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/search.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      346 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/trending.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     5922 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/tv.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      354 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/tv_episode_groups.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     3990 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/tv_episodes.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     2188 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/tv_seasons.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      769 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/src/tmdb/three/watch_providers.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.891703 ezapi-tmdb-0.8.3/tests/
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.901746 ezapi-tmdb-0.8.3/tests/four/
+-rw-r--r--   0 zehengl    (501) staff       (20)     2392 2023-03-22 16:13:35.000000 ezapi-tmdb-0.8.3/tests/four/test_v4.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.906527 ezapi-tmdb-0.8.3/tests/three/
+-rw-r--r--   0 zehengl    (501) staff       (20)      865 2023-03-22 16:13:35.000000 ezapi-tmdb-0.8.3/tests/three/conftest.py
+drwxr-xr-x   0 zehengl    (501) staff       (20)        0 2023-07-13 04:27:13.906700 ezapi-tmdb-0.8.3/tests/three/helpers/
+-rw-r--r--   0 zehengl    (501) staff       (20)      170 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/helpers/utils.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     2145 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_account.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      875 2023-03-22 16:13:35.000000 ezapi-tmdb-0.8.3/tests/three/test_authentication.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      231 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_certifications.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      321 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_changes.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      428 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_collections.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      390 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_companies.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      557 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_configuration.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      168 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_credits.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      207 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_discover.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      616 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_find.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      215 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_genres.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      671 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_guest_sessions.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      268 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_keywords.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1024 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_lists.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     3270 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_movies.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      385 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_networks.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1241 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_people.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      168 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_reviews.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      567 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_search.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      782 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_trending.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     3078 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_tv.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      208 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_tv_episode_groups.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     2369 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_tv_episodes.py
+-rw-r--r--   0 zehengl    (501) staff       (20)     1332 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_tv_seasons.py
+-rw-r--r--   0 zehengl    (501) staff       (20)      311 2023-03-10 04:09:34.000000 ezapi-tmdb-0.8.3/tests/three/test_watch_providers.py
```

### Comparing `ezapi-tmdb-0.8.2/.all-contributorsrc` & `ezapi-tmdb-0.8.3/.all-contributorsrc`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8939393939393938%*

 * *Differences: {"'commitConvention'": "'angular'",*

 * * "'contributors'": "{insert: [(2, OrderedDict([('login', 'joselimajr'), ('name', 'joselimajr'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/3194122?v=4'), "*

 * *                   "('profile', 'https://github.com/joselimajr'), ('contributions', "*

 * *                   "['ideas'])]))]}"}*

```diff
@@ -1,9 +1,10 @@
 {
     "commit": false,
+    "commitConvention": "angular",
     "contributors": [
         {
             "avatar_url": "https://avatars.githubusercontent.com/u/10906962?v=4",
             "contributions": [
                 "code"
             ],
             "login": "Cologler",
@@ -14,14 +15,23 @@
             "avatar_url": "https://avatars.githubusercontent.com/u/13171938?v=4",
             "contributions": [
                 "code"
             ],
             "login": "rafaelpierre",
             "name": "Rafael Pierre",
             "profile": "https://github.com/rafaelpierre"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/3194122?v=4",
+            "contributions": [
+                "ideas"
+            ],
+            "login": "joselimajr",
+            "name": "joselimajr",
+            "profile": "https://github.com/joselimajr"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `ezapi-tmdb-0.8.2/.github/workflows/pytest.yml` & `ezapi-tmdb-0.8.3/.github/workflows/pytest.yml`

 * *Files 24% similar despite different names*

```diff
@@ -11,23 +11,23 @@
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 1
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: Checkout 🛎️
-        uses: actions/checkout@v2
-      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/checkout@v3
+      - name: Set up Python ${{ matrix.python-version }} 🐍
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Test with pytest 🧪
         run: |
           python -m pip install -U pip
           pip install -r requirements-test.txt
           pip install -e .
           pytest
         env:
-          username: ${{ secrets.USERNAME }}
-          password: ${{ secrets.PASSWORD }}
-          api_key: ${{ secrets.API_KEY }}
-          access_token: ${{ secrets.ACCESS_TOKEN }}
+          tmdb_username: ${{ secrets.TMDB_USERNAME }}
+          tmdb_password: ${{ secrets.TMDB_PASSWORD }}
+          tmdb_api_key: ${{ secrets.TMDB_API_KEY }}
+          tmdb_access_token: ${{ secrets.TMDB_ACCESS_TOKEN }}
```

### Comparing `ezapi-tmdb-0.8.2/.vscode/settings.json` & `ezapi-tmdb-0.8.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/LICENSE` & `ezapi-tmdb-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/PKG-INFO` & `ezapi-tmdb-0.8.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1
-Name: ezapi-tmdb
-Version: 0.8.2
-Summary: A Python wrapper for TMDb API
-Author-email: Zeheng Li <imzehengl@gmail.com>
-Maintainer-email: Zeheng Li <imzehengl@gmail.com>
-Project-URL: repository, https://github.com/zehengl/ezapi-tmdb
-Project-URL: homepage, https://zehengl.github.io/ezapi-tmdb/
-Keywords: TMDb
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
-    <img src="https://cdn3.iconfinder.com/data/icons/data-sharing-and-cloud-lineal-style/512/apiprogrammingdevolperinterfaceappcomputer-512.png" alt="logo" height="196">
     <img src="https://www.themoviedb.org/assets/2/v4/logos/v2/blue_square_2-d537fb228cf3ded904ef09b136fe3fec72548ebc1fea3fbbd1ad9e36364db38b.svg" alt="yelp" height="96">
 </div>
 
 # ezapi-tmdb
 
 [![pytest](https://github.com/zehengl/ezapi-tmdb/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-tmdb/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
@@ -113,46 +96,51 @@
 
 tmdb.get_list(14105)
 tmdb.get_account_favorite_movies(account_id)
 ```
 
 ## Test
 
-    git clone git@github.com:zehengl/ezapi-tmdb.git
-    export api_key="..."
-    export username="..."
-    export password="..."
-    export access_token="..."
-    cd ezapi-tmdb
-    python setup.py test
+```bash
+git clone git@github.com:zehengl/ezapi-tmdb.git
+cd ezapi-tmdb
+export tmdb_api_key="..."
+export tmdb_username="..."
+export tmdb_password="..."
+export tmdb_access_token="..."
+python -m venv .venv
+source .venv/bin/activate
+pip install -e .
+pip install -r requirements-test.txt
+pytest
+```
 
-Use `$Env:api_key="..."` , `$Env:username="..."`, `$Env:password="..."`, and `$Env:access_token="..."` to set the api key, username, password, and access token environment variables on Windows.
+Use `$Env:tmdb_api_key="..."` , `$Env:tmdb_username="..."`, `$Env:tmdb_password="..."`, and `$Env:tmdb_access_token="..."` to set the api key, username, password, and access token environment variables on Windows.
 
 ## Credits
 
-- [Icon][1] by [Photolio][2]
-
-- Icon from [www.themoviedb.org][3]
+- Icon from [www.themoviedb.org][1]
 
-[1]: https://www.iconfinder.com/icons/4904814/api_app_computer_devolper_interface_programming_icon
-[2]: https://www.iconfinder.com/Muhammad_Auns
-[3]: https://www.themoviedb.org/about/logos-attribution
+[1]: https://www.themoviedb.org/about/logos-attribution
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/Cologler"><img src="https://avatars.githubusercontent.com/u/10906962?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Cologler</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=Cologler" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/rafaelpierre"><img src="https://avatars.githubusercontent.com/u/13171938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Rafael Pierre</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=rafaelpierre" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Cologler"><img src="https://avatars.githubusercontent.com/u/10906962?v=4?s=100" width="100px;" alt="Cologler"/><br /><sub><b>Cologler</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=Cologler" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rafaelpierre"><img src="https://avatars.githubusercontent.com/u/13171938?v=4?s=100" width="100px;" alt="Rafael Pierre"/><br /><sub><b>Rafael Pierre</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=rafaelpierre" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/joselimajr"><img src="https://avatars.githubusercontent.com/u/3194122?v=4?s=100" width="100px;" alt="joselimajr"/><br /><sub><b>joselimajr</b></sub></a><br /><a href="#ideas-joselimajr" title="Ideas, Planning, & Feedback">🤔</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `ezapi-tmdb-0.8.2/README.md` & `ezapi-tmdb-0.8.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+Metadata-Version: 2.1
+Name: ezapi-tmdb
+Version: 0.8.3
+Summary: A Python wrapper for TMDb API
+Author-email: Zeheng Li <imzehengl@gmail.com>
+Maintainer-email: Zeheng Li <imzehengl@gmail.com>
+Project-URL: repository, https://github.com/zehengl/ezapi-tmdb
+Project-URL: homepage, https://zehengl.github.io/ezapi-tmdb/
+Keywords: TMDb
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
-    <img src="https://cdn3.iconfinder.com/data/icons/data-sharing-and-cloud-lineal-style/512/apiprogrammingdevolperinterfaceappcomputer-512.png" alt="logo" height="196">
     <img src="https://www.themoviedb.org/assets/2/v4/logos/v2/blue_square_2-d537fb228cf3ded904ef09b136fe3fec72548ebc1fea3fbbd1ad9e36364db38b.svg" alt="yelp" height="96">
 </div>
 
 # ezapi-tmdb
 
 [![pytest](https://github.com/zehengl/ezapi-tmdb/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-tmdb/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
@@ -97,46 +112,51 @@
 
 tmdb.get_list(14105)
 tmdb.get_account_favorite_movies(account_id)
 ```
 
 ## Test
 
-    git clone git@github.com:zehengl/ezapi-tmdb.git
-    export api_key="..."
-    export username="..."
-    export password="..."
-    export access_token="..."
-    cd ezapi-tmdb
-    python setup.py test
+```bash
+git clone git@github.com:zehengl/ezapi-tmdb.git
+cd ezapi-tmdb
+export tmdb_api_key="..."
+export tmdb_username="..."
+export tmdb_password="..."
+export tmdb_access_token="..."
+python -m venv .venv
+source .venv/bin/activate
+pip install -e .
+pip install -r requirements-test.txt
+pytest
+```
 
-Use `$Env:api_key="..."` , `$Env:username="..."`, `$Env:password="..."`, and `$Env:access_token="..."` to set the api key, username, password, and access token environment variables on Windows.
+Use `$Env:tmdb_api_key="..."` , `$Env:tmdb_username="..."`, `$Env:tmdb_password="..."`, and `$Env:tmdb_access_token="..."` to set the api key, username, password, and access token environment variables on Windows.
 
 ## Credits
 
-- [Icon][1] by [Photolio][2]
-
-- Icon from [www.themoviedb.org][3]
+- Icon from [www.themoviedb.org][1]
 
-[1]: https://www.iconfinder.com/icons/4904814/api_app_computer_devolper_interface_programming_icon
-[2]: https://www.iconfinder.com/Muhammad_Auns
-[3]: https://www.themoviedb.org/about/logos-attribution
+[1]: https://www.themoviedb.org/about/logos-attribution
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/Cologler"><img src="https://avatars.githubusercontent.com/u/10906962?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Cologler</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=Cologler" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/rafaelpierre"><img src="https://avatars.githubusercontent.com/u/13171938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Rafael Pierre</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=rafaelpierre" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Cologler"><img src="https://avatars.githubusercontent.com/u/10906962?v=4?s=100" width="100px;" alt="Cologler"/><br /><sub><b>Cologler</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=Cologler" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rafaelpierre"><img src="https://avatars.githubusercontent.com/u/13171938?v=4?s=100" width="100px;" alt="Rafael Pierre"/><br /><sub><b>Rafael Pierre</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=rafaelpierre" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/joselimajr"><img src="https://avatars.githubusercontent.com/u/3194122?v=4?s=100" width="100px;" alt="joselimajr"/><br /><sub><b>joselimajr</b></sub></a><br /><a href="#ideas-joselimajr" title="Ideas, Planning, & Feedback">🤔</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `ezapi-tmdb-0.8.2/pyproject.toml` & `ezapi-tmdb-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/PKG-INFO` & `ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: ezapi-tmdb
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Python wrapper for TMDb API
 Author-email: Zeheng Li <imzehengl@gmail.com>
 Maintainer-email: Zeheng Li <imzehengl@gmail.com>
 Project-URL: repository, https://github.com/zehengl/ezapi-tmdb
 Project-URL: homepage, https://zehengl.github.io/ezapi-tmdb/
 Keywords: TMDb
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-    <img src="https://cdn3.iconfinder.com/data/icons/data-sharing-and-cloud-lineal-style/512/apiprogrammingdevolperinterfaceappcomputer-512.png" alt="logo" height="196">
     <img src="https://www.themoviedb.org/assets/2/v4/logos/v2/blue_square_2-d537fb228cf3ded904ef09b136fe3fec72548ebc1fea3fbbd1ad9e36364db38b.svg" alt="yelp" height="96">
 </div>
 
 # ezapi-tmdb
 
 [![pytest](https://github.com/zehengl/ezapi-tmdb/actions/workflows/pytest.yml/badge.svg)](https://github.com/zehengl/ezapi-tmdb/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
@@ -113,46 +112,51 @@
 
 tmdb.get_list(14105)
 tmdb.get_account_favorite_movies(account_id)
 ```
 
 ## Test
 
-    git clone git@github.com:zehengl/ezapi-tmdb.git
-    export api_key="..."
-    export username="..."
-    export password="..."
-    export access_token="..."
-    cd ezapi-tmdb
-    python setup.py test
+```bash
+git clone git@github.com:zehengl/ezapi-tmdb.git
+cd ezapi-tmdb
+export tmdb_api_key="..."
+export tmdb_username="..."
+export tmdb_password="..."
+export tmdb_access_token="..."
+python -m venv .venv
+source .venv/bin/activate
+pip install -e .
+pip install -r requirements-test.txt
+pytest
+```
 
-Use `$Env:api_key="..."` , `$Env:username="..."`, `$Env:password="..."`, and `$Env:access_token="..."` to set the api key, username, password, and access token environment variables on Windows.
+Use `$Env:tmdb_api_key="..."` , `$Env:tmdb_username="..."`, `$Env:tmdb_password="..."`, and `$Env:tmdb_access_token="..."` to set the api key, username, password, and access token environment variables on Windows.
 
 ## Credits
 
-- [Icon][1] by [Photolio][2]
-
-- Icon from [www.themoviedb.org][3]
+- Icon from [www.themoviedb.org][1]
 
-[1]: https://www.iconfinder.com/icons/4904814/api_app_computer_devolper_interface_programming_icon
-[2]: https://www.iconfinder.com/Muhammad_Auns
-[3]: https://www.themoviedb.org/about/logos-attribution
+[1]: https://www.themoviedb.org/about/logos-attribution
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/Cologler"><img src="https://avatars.githubusercontent.com/u/10906962?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Cologler</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=Cologler" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/rafaelpierre"><img src="https://avatars.githubusercontent.com/u/13171938?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Rafael Pierre</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=rafaelpierre" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Cologler"><img src="https://avatars.githubusercontent.com/u/10906962?v=4?s=100" width="100px;" alt="Cologler"/><br /><sub><b>Cologler</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=Cologler" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rafaelpierre"><img src="https://avatars.githubusercontent.com/u/13171938?v=4?s=100" width="100px;" alt="Rafael Pierre"/><br /><sub><b>Rafael Pierre</b></sub></a><br /><a href="https://github.com/zehengl/ezapi-tmdb/commits?author=rafaelpierre" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/joselimajr"><img src="https://avatars.githubusercontent.com/u/3194122?v=4?s=100" width="100px;" alt="joselimajr"/><br /><sub><b>joselimajr</b></sub></a><br /><a href="#ideas-joselimajr" title="Ideas, Planning, & Feedback">🤔</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `ezapi-tmdb-0.8.2/src/ezapi_tmdb.egg-info/SOURCES.txt` & `ezapi-tmdb-0.8.3/src/ezapi_tmdb.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 .all-contributorsrc
 .gitignore
 LICENSE
 README.md
+mkdocs.yml
 pyproject.toml
 requirements-dev.txt
+requirements-docs.txt
 requirements-test.txt
 requirements.txt
+.github/workflows/gh-deploy.yml
 .github/workflows/pcu.yml
 .github/workflows/pytest.yml
 .vscode/extensions.json
 .vscode/settings.json
+docs/index.md
 src/ezapi_tmdb.egg-info/PKG-INFO
 src/ezapi_tmdb.egg-info/SOURCES.txt
 src/ezapi_tmdb.egg-info/dependency_links.txt
 src/ezapi_tmdb.egg-info/requires.txt
 src/ezapi_tmdb.egg-info/top_level.txt
 src/tmdb/__init__.py
 src/tmdb/four/__init__.py
```

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/four/__init__.py` & `ezapi-tmdb-0.8.3/src/tmdb/four/__init__.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/four/account.py` & `ezapi-tmdb-0.8.3/src/tmdb/four/account.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/four/auth.py` & `ezapi-tmdb-0.8.3/src/tmdb/four/auth.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/four/list.py` & `ezapi-tmdb-0.8.3/src/tmdb/four/list.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/__init__.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/__init__.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/account.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/account.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/authentication.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/authentication.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/base.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/base.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/certifications.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/certifications.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/changes.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/changes.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/collections.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/collections.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/companies.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/companies.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/configuration.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/configuration.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/guest_sessions.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/guest_sessions.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/keywords.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/keywords.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/lists.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/lists.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/movies.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/movies.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/networks.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/networks.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/people.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/people.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/search.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/search.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/tv.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/tv.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/tv_episodes.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/tv_episodes.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/tv_seasons.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/tv_seasons.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/src/tmdb/three/watch_providers.py` & `ezapi-tmdb-0.8.3/src/tmdb/three/watch_providers.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/four/test_v4.py` & `ezapi-tmdb-0.8.3/tests/four/test_v4.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from tmdb.four import TMDb
 
 load_dotenv()
 
 
 class TMDb4TestClass(BaseCase):
     def test_v4_api(self):
-        access_token = os.getenv("access_token")
-        username = os.getenv("username")
-        password = os.getenv("password")
+        access_token = os.getenv("tmdb_access_token")
+        username = os.getenv("tmdb_username")
+        password = os.getenv("tmdb_password")
 
         msg = "Missing one or more configs (username, password, access_token)"
         if not all([username, password, access_token]):
             assert False, msg
 
         tmdb = TMDb(access_token)
```

### Comparing `ezapi-tmdb-0.8.2/tests/three/conftest.py` & `ezapi-tmdb-0.8.3/tests/three/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "helpers"))
 load_dotenv()
 
 
 @pytest.fixture(scope="module")
 def tmdb():
-    api_key = os.getenv("api_key", None)
+    api_key = os.getenv("tmdb_api_key", None)
 
     return TMDb(api_key) if api_key else None
 
 
 @pytest.fixture(scope="module")
 def session_id(tmdb):
-    username = os.getenv("username")
-    password = os.getenv("password")
+    username = os.getenv("tmdb_username")
+    password = os.getenv("tmdb_password")
     request_token = tmdb.create_request_token().get("request_token")
 
     tmdb.create_session_with_login(username, password, request_token)
 
     session_id = tmdb.create_session(request_token).get("session_id")
 
     yield session_id
```

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_account.py` & `ezapi-tmdb-0.8.3/tests/three/test_account.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_authentication.py` & `ezapi-tmdb-0.8.3/tests/three/test_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 @polite
 def test_create_request_token(tmdb):
     assert tmdb.create_request_token() is not None
 
 
 @polite
 def test_session_workflow_with_login(tmdb):
-    username = os.getenv("username")
-    password = os.getenv("password")
+    username = os.getenv("tmdb_username")
+    password = os.getenv("tmdb_password")
     request_token = tmdb.create_request_token().get("request_token")
 
     assert username and password and request_token
     assert tmdb.create_session_with_login(username, password, request_token)
 
     session_id = tmdb.create_session(request_token).get("session_id")
```

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_configuration.py` & `ezapi-tmdb-0.8.3/tests/three/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_find.py` & `ezapi-tmdb-0.8.3/tests/three/test_find.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_guest_sessions.py` & `ezapi-tmdb-0.8.3/tests/three/test_guest_sessions.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_lists.py` & `ezapi-tmdb-0.8.3/tests/three/test_lists.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_movies.py` & `ezapi-tmdb-0.8.3/tests/three/test_movies.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_people.py` & `ezapi-tmdb-0.8.3/tests/three/test_people.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_search.py` & `ezapi-tmdb-0.8.3/tests/three/test_search.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_trending.py` & `ezapi-tmdb-0.8.3/tests/three/test_trending.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_tv.py` & `ezapi-tmdb-0.8.3/tests/three/test_tv.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_tv_episodes.py` & `ezapi-tmdb-0.8.3/tests/three/test_tv_episodes.py`

 * *Files identical despite different names*

### Comparing `ezapi-tmdb-0.8.2/tests/three/test_tv_seasons.py` & `ezapi-tmdb-0.8.3/tests/three/test_tv_seasons.py`

 * *Files identical despite different names*


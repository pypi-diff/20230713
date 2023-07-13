# Comparing `tmp/martor-1.6.8.tar.gz` & `tmp/martor-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martor-1.6.8.tar", last modified: Tue Dec 21 13:21:00 2021, max compression
+gzip compressed data, was "martor-1.6.9.tar", last modified: Tue Jan 11 13:16:28 2022, max compression
```

## Comparing `martor-1.6.8.tar` & `martor-1.6.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.840108 martor-1.6.8/
--rw-r--r--   0 agus       (501) staff       (20)    35141 2021-11-18 13:32:26.000000 martor-1.6.8/LICENSE
--rw-r--r--   0 agus       (501) staff       (20)      130 2021-11-18 13:32:26.000000 martor-1.6.8/MANIFEST.in
--rw-r--r--   0 agus       (501) staff       (20)    12564 2021-12-21 13:21:00.840250 martor-1.6.8/PKG-INFO
--rw-r--r--   0 agus       (501) staff       (20)    11093 2021-12-21 11:14:22.000000 martor-1.6.8/README.md
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.763863 martor-1.6.8/martor/
--rw-r--r--   0 agus       (501) staff       (20)      131 2021-12-21 10:58:37.000000 martor-1.6.8/martor/__init__.py
--rw-r--r--   0 agus       (501) staff       (20)      301 2021-12-21 10:58:53.000000 martor-1.6.8/martor/admin.py
--rw-r--r--   0 agus       (501) staff       (20)     1493 2021-12-21 11:01:12.000000 martor-1.6.8/martor/api.py
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.768003 martor-1.6.8/martor/extensions/
--rw-r--r--   0 agus       (501) staff       (20)        0 2021-11-18 13:32:26.000000 martor-1.6.8/martor/extensions/__init__.py
--rw-r--r--   0 agus       (501) staff       (20)     1391 2021-12-21 10:58:37.000000 martor-1.6.8/martor/extensions/del_ins.py
--rw-r--r--   0 agus       (501) staff       (20)    13543 2021-12-21 10:58:38.000000 martor-1.6.8/martor/extensions/emoji.py
--rw-r--r--   0 agus       (501) staff       (20)      333 2021-12-21 10:58:37.000000 martor-1.6.8/martor/extensions/escape_html.py
--rw-r--r--   0 agus       (501) staff       (20)     5559 2021-12-21 12:58:50.000000 martor-1.6.8/martor/extensions/mdx_video.py
--rw-r--r--   0 agus       (501) staff       (20)     1699 2021-12-21 12:58:59.000000 martor-1.6.8/martor/extensions/mention.py
--rw-r--r--   0 agus       (501) staff       (20)     2306 2021-12-21 11:08:58.000000 martor-1.6.8/martor/extensions/urlize.py
--rw-r--r--   0 agus       (501) staff       (20)      534 2021-12-21 10:58:37.000000 martor-1.6.8/martor/fields.py
--rw-r--r--   0 agus       (501) staff       (20)      350 2021-12-21 10:58:37.000000 martor-1.6.8/martor/models.py
--rw-r--r--   0 agus       (501) staff       (20)     3984 2021-12-21 13:11:24.000000 martor-1.6.8/martor/settings.py
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.756918 martor-1.6.8/martor/static/
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.769640 martor-1.6.8/martor/static/dicts/
--rw-r--r--   0 agus       (501) staff       (20)      545 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/dicts/README.md
--rw-r--r--   0 agus       (501) staff       (20)     3041 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/dicts/en_US.aff
--rw-r--r--   0 agus       (501) staff       (20)   696405 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/dicts/en_US.dic
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.756693 martor-1.6.8/martor/static/martor/
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.777121 martor-1.6.8/martor/static/martor/css/
--rw-r--r--   0 agus       (501) staff       (20)     1933 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/martor/css/martor-admin.css
--rw-r--r--   0 agus       (501) staff       (20)     1765 2021-12-21 10:32:49.000000 martor-1.6.8/martor/static/martor/css/martor-admin.min.css
--rw-r--r--   0 agus       (501) staff       (20)    11003 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/martor/css/martor.bootstrap.css
--rw-r--r--   0 agus       (501) staff       (20)    10508 2021-12-21 10:32:49.000000 martor-1.6.8/martor/static/martor/css/martor.bootstrap.min.css
--rw-r--r--   0 agus       (501) staff       (20)     9970 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/martor/css/martor.semantic.css
--rw-r--r--   0 agus       (501) staff       (20)     9616 2021-12-21 10:32:49.000000 martor-1.6.8/martor/static/martor/css/martor.semantic.min.css
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.781057 martor-1.6.8/martor/static/martor/js/
--rw-r--r--   0 agus       (501) staff       (20)    39477 2021-12-21 10:32:49.000000 martor-1.6.8/martor/static/martor/js/martor.bootstrap.js
--rw-r--r--   0 agus       (501) staff       (20)    15160 2021-12-21 10:32:49.000000 martor-1.6.8/martor/static/martor/js/martor.bootstrap.min.js
--rw-r--r--   0 agus       (501) staff       (20)    39520 2021-12-21 10:32:49.000000 martor-1.6.8/martor/static/martor/js/martor.semantic.js
--rw-r--r--   0 agus       (501) staff       (20)    15121 2021-12-21 10:32:49.000000 martor-1.6.8/martor/static/martor/js/martor.semantic.min.js
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.757501 martor-1.6.8/martor/static/plugins/
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.785180 martor-1.6.8/martor/static/plugins/css/
--rw-r--r--   0 agus       (501) staff       (20)      635 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/css/ace.min.css
--rw-r--r--   0 agus       (501) staff       (20)   160257 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/css/bootstrap.min.css
--rw-r--r--   0 agus       (501) staff       (20)      948 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/css/resizable.min.css
--rw-r--r--   0 agus       (501) staff       (20)   627789 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/css/semantic.min.css
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.800305 martor-1.6.8/martor/static/plugins/fonts/
--rw-r--r--   0 agus       (501) staff       (20)    98640 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/brand-icons.eot
--rw-r--r--   0 agus       (501) staff       (20)   507628 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/brand-icons.svg
--rw-r--r--   0 agus       (501) staff       (20)    98404 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/brand-icons.ttf
--rw-r--r--   0 agus       (501) staff       (20)    63728 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/brand-icons.woff
--rw-r--r--   0 agus       (501) staff       (20)    54488 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/brand-icons.woff2
--rw-r--r--   0 agus       (501) staff       (20)    40166 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/icons.eot
--rw-r--r--   0 agus       (501) staff       (20)    64121 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/icons.svg
--rw-r--r--   0 agus       (501) staff       (20)    39924 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/icons.ttf
--rw-r--r--   0 agus       (501) staff       (20)    24676 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/icons.woff
--rw-r--r--   0 agus       (501) staff       (20)    40148 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/icons.woff2
--rw-r--r--   0 agus       (501) staff       (20)    31156 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/outline-icons.eot
--rw-r--r--   0 agus       (501) staff       (20)   107201 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/outline-icons.svg
--rw-r--r--   0 agus       (501) staff       (20)    30928 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/outline-icons.ttf
--rw-r--r--   0 agus       (501) staff       (20)    14712 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/outline-icons.woff
--rw-r--r--   0 agus       (501) staff       (20)    12240 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/fonts/outline-icons.woff2
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.801844 martor-1.6.8/martor/static/plugins/images/
--rw-r--r--   0 agus       (501) staff       (20)     1095 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/images/commonmark.png
--rw-r--r--   0 agus       (501) staff       (20)    28123 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/images/flags.png
--rw-r--r--   0 agus       (501) staff       (20)     3296 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/images/heart.png
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.834479 martor-1.6.8/martor/static/plugins/js/
--rw-r--r--   0 agus       (501) staff       (20)   366334 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/ace.js
--rw-r--r--   0 agus       (501) staff       (20)    81199 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/bootstrap.min.js
--rw-r--r--   0 agus       (501) staff       (20)     9895 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/emojis.min.js
--rw-r--r--   0 agus       (501) staff       (20)    35473 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/ext-language_tools.js
--rw-r--r--   0 agus       (501) staff       (20)    44794 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/highlight.min.js
--rw-r--r--   0 agus       (501) staff       (20)    89501 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/jquery.min.js
--rw-r--r--   0 agus       (501) staff       (20)    72380 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/jquery.slim.min.js
--rw-r--r--   0 agus       (501) staff       (20)    72315 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/mode-markdown.js
--rw-r--r--   0 agus       (501) staff       (20)     2234 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/resizable.min.js
--rw-r--r--   0 agus       (501) staff       (20)   275721 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/semantic.min.js
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.835097 martor-1.6.8/martor/static/plugins/js/snippets/
--rw-r--r--   0 agus       (501) staff       (20)     2255 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/snippets/markdown.js
--rw-r--r--   0 agus       (501) staff       (20)     4765 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/spellcheck.js
--rw-r--r--   0 agus       (501) staff       (20)     2453 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/theme-github.js
--rw-r--r--   0 agus       (501) staff       (20)    26818 2021-11-18 13:32:26.000000 martor-1.6.8/martor/static/plugins/js/typo.js
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.757898 martor-1.6.8/martor/templates/
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.758153 martor-1.6.8/martor/templates/martor/
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.836771 martor-1.6.8/martor/templates/martor/bootstrap/
--rw-r--r--   0 agus       (501) staff       (20)     3504 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/bootstrap/editor.html
--rw-r--r--   0 agus       (501) staff       (20)     1550 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/bootstrap/emoji.html
--rw-r--r--   0 agus       (501) staff       (20)     7029 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/bootstrap/guide.html
--rw-r--r--   0 agus       (501) staff       (20)    13591 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/bootstrap/toolbar.html
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.838066 martor-1.6.8/martor/templates/martor/semantic/
--rw-r--r--   0 agus       (501) staff       (20)     1268 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/semantic/editor.html
--rw-r--r--   0 agus       (501) staff       (20)      513 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/semantic/emoji.html
--rw-r--r--   0 agus       (501) staff       (20)     5238 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/semantic/guide.html
--rw-r--r--   0 agus       (501) staff       (20)     4396 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templates/martor/semantic/toolbar.html
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.838581 martor-1.6.8/martor/templatetags/
--rw-r--r--   0 agus       (501) staff       (20)        0 2021-11-18 13:32:26.000000 martor-1.6.8/martor/templatetags/__init__.py
--rw-r--r--   0 agus       (501) staff       (20)      441 2021-12-21 10:53:18.000000 martor-1.6.8/martor/templatetags/martortags.py
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.839887 martor-1.6.8/martor/tests/
--rw-r--r--   0 agus       (501) staff       (20)        0 2021-11-18 13:32:26.000000 martor-1.6.8/martor/tests/__init__.py
--rw-r--r--   0 agus       (501) staff       (20)      197 2021-12-21 10:58:37.000000 martor-1.6.8/martor/tests/models.py
--rw-r--r--   0 agus       (501) staff       (20)     3059 2021-12-21 13:07:54.000000 martor-1.6.8/martor/tests/tests.py
--rw-r--r--   0 agus       (501) staff       (20)      441 2021-12-21 10:58:37.000000 martor-1.6.8/martor/tests/urls.py
--rw-r--r--   0 agus       (501) staff       (20)      205 2021-12-21 10:58:37.000000 martor-1.6.8/martor/tests/views.py
--rw-r--r--   0 agus       (501) staff       (20)      795 2021-12-21 11:02:40.000000 martor-1.6.8/martor/urls.py
--rw-r--r--   0 agus       (501) staff       (20)     1966 2021-12-21 13:08:04.000000 martor-1.6.8/martor/utils.py
--rw-r--r--   0 agus       (501) staff       (20)     2848 2021-12-21 10:58:37.000000 martor-1.6.8/martor/views.py
--rw-r--r--   0 agus       (501) staff       (20)     4390 2021-12-21 10:58:37.000000 martor-1.6.8/martor/widgets.py
-drwxr-xr-x   0 agus       (501) staff       (20)        0 2021-12-21 13:21:00.765900 martor-1.6.8/martor.egg-info/
--rw-r--r--   0 agus       (501) staff       (20)    12564 2021-12-21 13:21:00.000000 martor-1.6.8/martor.egg-info/PKG-INFO
--rw-r--r--   0 agus       (501) staff       (20)     3217 2021-12-21 13:21:00.000000 martor-1.6.8/martor.egg-info/SOURCES.txt
--rw-r--r--   0 agus       (501) staff       (20)        1 2021-12-21 13:21:00.000000 martor-1.6.8/martor.egg-info/dependency_links.txt
--rw-r--r--   0 agus       (501) staff       (20)        1 2021-11-18 13:44:05.000000 martor-1.6.8/martor.egg-info/not-zip-safe
--rw-r--r--   0 agus       (501) staff       (20)       32 2021-12-21 13:21:00.000000 martor-1.6.8/martor.egg-info/requires.txt
--rw-r--r--   0 agus       (501) staff       (20)        7 2021-12-21 13:21:00.000000 martor-1.6.8/martor.egg-info/top_level.txt
--rw-r--r--   0 agus       (501) staff       (20)       32 2021-12-21 12:19:45.000000 martor-1.6.8/requirements.txt
--rw-r--r--   0 agus       (501) staff       (20)       79 2021-12-21 13:21:00.840751 martor-1.6.8/setup.cfg
--rw-r--r--   0 agus       (501) staff       (20)     1859 2021-11-18 13:32:26.000000 martor-1.6.8/setup.py
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.987654 martor-1.6.9/
+-rw-r--r--   0 agus       (501) staff       (20)    35141 2021-11-18 13:32:26.000000 martor-1.6.9/LICENSE
+-rw-r--r--   0 agus       (501) staff       (20)      130 2021-11-18 13:32:26.000000 martor-1.6.9/MANIFEST.in
+-rw-r--r--   0 agus       (501) staff       (20)    12564 2022-01-11 13:16:28.987821 martor-1.6.9/PKG-INFO
+-rw-r--r--   0 agus       (501) staff       (20)    11093 2021-12-21 11:14:22.000000 martor-1.6.9/README.md
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.955814 martor-1.6.9/martor/
+-rw-r--r--   0 agus       (501) staff       (20)      131 2022-01-11 13:12:43.000000 martor-1.6.9/martor/__init__.py
+-rw-r--r--   0 agus       (501) staff       (20)      301 2021-12-21 10:58:53.000000 martor-1.6.9/martor/admin.py
+-rw-r--r--   0 agus       (501) staff       (20)     1493 2021-12-21 11:01:12.000000 martor-1.6.9/martor/api.py
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.960542 martor-1.6.9/martor/extensions/
+-rw-r--r--   0 agus       (501) staff       (20)        0 2021-11-18 13:32:26.000000 martor-1.6.9/martor/extensions/__init__.py
+-rw-r--r--   0 agus       (501) staff       (20)     1391 2021-12-21 10:58:37.000000 martor-1.6.9/martor/extensions/del_ins.py
+-rw-r--r--   0 agus       (501) staff       (20)    13543 2021-12-21 10:58:38.000000 martor-1.6.9/martor/extensions/emoji.py
+-rw-r--r--   0 agus       (501) staff       (20)      333 2021-12-21 10:58:37.000000 martor-1.6.9/martor/extensions/escape_html.py
+-rw-r--r--   0 agus       (501) staff       (20)     5559 2021-12-21 12:58:50.000000 martor-1.6.9/martor/extensions/mdx_video.py
+-rw-r--r--   0 agus       (501) staff       (20)     1699 2021-12-21 12:58:59.000000 martor-1.6.9/martor/extensions/mention.py
+-rw-r--r--   0 agus       (501) staff       (20)     2306 2021-12-21 11:08:58.000000 martor-1.6.9/martor/extensions/urlize.py
+-rw-r--r--   0 agus       (501) staff       (20)      534 2021-12-21 10:58:37.000000 martor-1.6.9/martor/fields.py
+-rw-r--r--   0 agus       (501) staff       (20)      350 2021-12-21 10:58:37.000000 martor-1.6.9/martor/models.py
+-rw-r--r--   0 agus       (501) staff       (20)     3984 2021-12-21 13:11:24.000000 martor-1.6.9/martor/settings.py
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.947214 martor-1.6.9/martor/static/
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.961329 martor-1.6.9/martor/static/dicts/
+-rw-r--r--   0 agus       (501) staff       (20)      545 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/dicts/README.md
+-rw-r--r--   0 agus       (501) staff       (20)     3041 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/dicts/en_US.aff
+-rw-r--r--   0 agus       (501) staff       (20)   696405 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/dicts/en_US.dic
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.947081 martor-1.6.9/martor/static/martor/
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.963968 martor-1.6.9/martor/static/martor/css/
+-rw-r--r--   0 agus       (501) staff       (20)     1933 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/martor/css/martor-admin.css
+-rw-r--r--   0 agus       (501) staff       (20)     1765 2022-01-11 13:13:05.000000 martor-1.6.9/martor/static/martor/css/martor-admin.min.css
+-rw-r--r--   0 agus       (501) staff       (20)    11003 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/martor/css/martor.bootstrap.css
+-rw-r--r--   0 agus       (501) staff       (20)    10508 2022-01-11 13:13:06.000000 martor-1.6.9/martor/static/martor/css/martor.bootstrap.min.css
+-rw-r--r--   0 agus       (501) staff       (20)     9970 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/martor/css/martor.semantic.css
+-rw-r--r--   0 agus       (501) staff       (20)     9616 2022-01-11 13:13:06.000000 martor-1.6.9/martor/static/martor/css/martor.semantic.min.css
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.965323 martor-1.6.9/martor/static/martor/js/
+-rw-r--r--   0 agus       (501) staff       (20)    39477 2022-01-11 13:13:06.000000 martor-1.6.9/martor/static/martor/js/martor.bootstrap.js
+-rw-r--r--   0 agus       (501) staff       (20)    15160 2022-01-11 13:13:06.000000 martor-1.6.9/martor/static/martor/js/martor.bootstrap.min.js
+-rw-r--r--   0 agus       (501) staff       (20)    39520 2022-01-11 13:13:06.000000 martor-1.6.9/martor/static/martor/js/martor.semantic.js
+-rw-r--r--   0 agus       (501) staff       (20)    15121 2022-01-11 13:13:06.000000 martor-1.6.9/martor/static/martor/js/martor.semantic.min.js
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.947697 martor-1.6.9/martor/static/plugins/
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.966844 martor-1.6.9/martor/static/plugins/css/
+-rw-r--r--   0 agus       (501) staff       (20)      635 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/css/ace.min.css
+-rw-r--r--   0 agus       (501) staff       (20)   160257 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/css/bootstrap.min.css
+-rw-r--r--   0 agus       (501) staff       (20)      948 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/css/resizable.min.css
+-rw-r--r--   0 agus       (501) staff       (20)   627789 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/css/semantic.min.css
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.976469 martor-1.6.9/martor/static/plugins/fonts/
+-rw-r--r--   0 agus       (501) staff       (20)    98640 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/brand-icons.eot
+-rw-r--r--   0 agus       (501) staff       (20)   507628 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/brand-icons.svg
+-rw-r--r--   0 agus       (501) staff       (20)    98404 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/brand-icons.ttf
+-rw-r--r--   0 agus       (501) staff       (20)    63728 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/brand-icons.woff
+-rw-r--r--   0 agus       (501) staff       (20)    54488 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/brand-icons.woff2
+-rw-r--r--   0 agus       (501) staff       (20)    40166 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/icons.eot
+-rw-r--r--   0 agus       (501) staff       (20)    64121 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/icons.svg
+-rw-r--r--   0 agus       (501) staff       (20)    39924 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/icons.ttf
+-rw-r--r--   0 agus       (501) staff       (20)    24676 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/icons.woff
+-rw-r--r--   0 agus       (501) staff       (20)    40148 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/icons.woff2
+-rw-r--r--   0 agus       (501) staff       (20)    31156 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/outline-icons.eot
+-rw-r--r--   0 agus       (501) staff       (20)   107201 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/outline-icons.svg
+-rw-r--r--   0 agus       (501) staff       (20)    30928 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/outline-icons.ttf
+-rw-r--r--   0 agus       (501) staff       (20)    14712 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/outline-icons.woff
+-rw-r--r--   0 agus       (501) staff       (20)    12240 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/fonts/outline-icons.woff2
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.977758 martor-1.6.9/martor/static/plugins/images/
+-rw-r--r--   0 agus       (501) staff       (20)     1095 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/images/commonmark.png
+-rw-r--r--   0 agus       (501) staff       (20)    28123 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/images/flags.png
+-rw-r--r--   0 agus       (501) staff       (20)     3296 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/images/heart.png
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.982844 martor-1.6.9/martor/static/plugins/js/
+-rw-r--r--   0 agus       (501) staff       (20)   366334 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/ace.js
+-rw-r--r--   0 agus       (501) staff       (20)    81199 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/bootstrap.min.js
+-rw-r--r--   0 agus       (501) staff       (20)     9895 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/emojis.min.js
+-rw-r--r--   0 agus       (501) staff       (20)    35473 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/ext-language_tools.js
+-rw-r--r--   0 agus       (501) staff       (20)    44794 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/highlight.min.js
+-rw-r--r--   0 agus       (501) staff       (20)    89501 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/jquery.min.js
+-rw-r--r--   0 agus       (501) staff       (20)    72380 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/jquery.slim.min.js
+-rw-r--r--   0 agus       (501) staff       (20)    72315 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/mode-markdown.js
+-rw-r--r--   0 agus       (501) staff       (20)     2234 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/resizable.min.js
+-rw-r--r--   0 agus       (501) staff       (20)   275721 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/semantic.min.js
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.983188 martor-1.6.9/martor/static/plugins/js/snippets/
+-rw-r--r--   0 agus       (501) staff       (20)     2255 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/snippets/markdown.js
+-rw-r--r--   0 agus       (501) staff       (20)     4765 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/spellcheck.js
+-rw-r--r--   0 agus       (501) staff       (20)     2453 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/theme-github.js
+-rw-r--r--   0 agus       (501) staff       (20)    26818 2021-11-18 13:32:26.000000 martor-1.6.9/martor/static/plugins/js/typo.js
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.948178 martor-1.6.9/martor/templates/
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.948557 martor-1.6.9/martor/templates/martor/
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.984306 martor-1.6.9/martor/templates/martor/bootstrap/
+-rw-r--r--   0 agus       (501) staff       (20)     3504 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/bootstrap/editor.html
+-rw-r--r--   0 agus       (501) staff       (20)     1550 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/bootstrap/emoji.html
+-rw-r--r--   0 agus       (501) staff       (20)     7029 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/bootstrap/guide.html
+-rw-r--r--   0 agus       (501) staff       (20)    13591 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/bootstrap/toolbar.html
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.985583 martor-1.6.9/martor/templates/martor/semantic/
+-rw-r--r--   0 agus       (501) staff       (20)     1268 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/semantic/editor.html
+-rw-r--r--   0 agus       (501) staff       (20)      513 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/semantic/emoji.html
+-rw-r--r--   0 agus       (501) staff       (20)     5238 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/semantic/guide.html
+-rw-r--r--   0 agus       (501) staff       (20)     4396 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templates/martor/semantic/toolbar.html
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.986097 martor-1.6.9/martor/templatetags/
+-rw-r--r--   0 agus       (501) staff       (20)        0 2021-11-18 13:32:26.000000 martor-1.6.9/martor/templatetags/__init__.py
+-rw-r--r--   0 agus       (501) staff       (20)      441 2021-12-21 10:53:18.000000 martor-1.6.9/martor/templatetags/martortags.py
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.987421 martor-1.6.9/martor/tests/
+-rw-r--r--   0 agus       (501) staff       (20)        0 2021-11-18 13:32:26.000000 martor-1.6.9/martor/tests/__init__.py
+-rw-r--r--   0 agus       (501) staff       (20)      197 2021-12-21 10:58:37.000000 martor-1.6.9/martor/tests/models.py
+-rw-r--r--   0 agus       (501) staff       (20)     3059 2021-12-21 13:07:54.000000 martor-1.6.9/martor/tests/tests.py
+-rw-r--r--   0 agus       (501) staff       (20)      441 2021-12-21 10:58:37.000000 martor-1.6.9/martor/tests/urls.py
+-rw-r--r--   0 agus       (501) staff       (20)      205 2021-12-21 10:58:37.000000 martor-1.6.9/martor/tests/views.py
+-rw-r--r--   0 agus       (501) staff       (20)      795 2021-12-21 11:02:40.000000 martor-1.6.9/martor/urls.py
+-rw-r--r--   0 agus       (501) staff       (20)     1970 2022-01-11 13:11:55.000000 martor-1.6.9/martor/utils.py
+-rw-r--r--   0 agus       (501) staff       (20)     2848 2021-12-21 10:58:37.000000 martor-1.6.9/martor/views.py
+-rw-r--r--   0 agus       (501) staff       (20)     4390 2021-12-21 10:58:37.000000 martor-1.6.9/martor/widgets.py
+drwxr-xr-x   0 agus       (501) staff       (20)        0 2022-01-11 13:16:28.958218 martor-1.6.9/martor.egg-info/
+-rw-r--r--   0 agus       (501) staff       (20)    12564 2022-01-11 13:16:28.000000 martor-1.6.9/martor.egg-info/PKG-INFO
+-rw-r--r--   0 agus       (501) staff       (20)     3217 2022-01-11 13:16:28.000000 martor-1.6.9/martor.egg-info/SOURCES.txt
+-rw-r--r--   0 agus       (501) staff       (20)        1 2022-01-11 13:16:28.000000 martor-1.6.9/martor.egg-info/dependency_links.txt
+-rw-r--r--   0 agus       (501) staff       (20)        1 2021-11-18 13:44:05.000000 martor-1.6.9/martor.egg-info/not-zip-safe
+-rw-r--r--   0 agus       (501) staff       (20)       32 2022-01-11 13:16:28.000000 martor-1.6.9/martor.egg-info/requires.txt
+-rw-r--r--   0 agus       (501) staff       (20)        7 2022-01-11 13:16:28.000000 martor-1.6.9/martor.egg-info/top_level.txt
+-rw-r--r--   0 agus       (501) staff       (20)       32 2021-12-21 12:19:45.000000 martor-1.6.9/requirements.txt
+-rw-r--r--   0 agus       (501) staff       (20)       79 2022-01-11 13:16:28.988391 martor-1.6.9/setup.cfg
+-rw-r--r--   0 agus       (501) staff       (20)     1859 2021-11-18 13:32:26.000000 martor-1.6.9/setup.py
```

### Comparing `martor-1.6.8/LICENSE` & `martor-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/PKG-INFO` & `martor-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: martor
-Version: 1.6.8
+Version: 1.6.9
 Summary: Django Markdown Editor
 Home-page: https://github.com/agusmakmun/django-markdown-editor
 Author: Agus Makmun (Summon Agus)
 Author-email: summon.agus@gmail.com
 License: GNUGPL-v3
-Download-URL: https://github.com/agusmakmun/django-markdown-editor/tarball/v1.6.8
+Download-URL: https://github.com/agusmakmun/django-markdown-editor/tarball/v1.6.9
 Keywords: martor,django markdown,django markdown editor
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
```

### Comparing `martor-1.6.8/README.md` & `martor-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/api.py` & `martor-1.6.9/martor/api.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/extensions/del_ins.py` & `martor-1.6.9/martor/extensions/del_ins.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/extensions/emoji.py` & `martor-1.6.9/martor/extensions/emoji.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/extensions/mdx_video.py` & `martor-1.6.9/martor/extensions/mdx_video.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/extensions/mention.py` & `martor-1.6.9/martor/extensions/mention.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/extensions/urlize.py` & `martor-1.6.9/martor/extensions/urlize.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/fields.py` & `martor-1.6.9/martor/fields.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/settings.py` & `martor-1.6.9/martor/settings.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/dicts/README.md` & `martor-1.6.9/martor/static/dicts/README.md`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/dicts/en_US.aff` & `martor-1.6.9/martor/static/dicts/en_US.aff`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/dicts/en_US.dic` & `martor-1.6.9/martor/static/dicts/en_US.dic`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/martor/css/martor-admin.css` & `martor-1.6.9/martor/static/martor/css/martor-admin.css`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/martor/css/martor-admin.min.css` & `martor-1.6.9/martor/static/martor/css/martor-admin.min.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 /**
- * Name         : Martor v1.6.8
+ * Name         : Martor v1.6.9
  * Created by   : Agus Makmun (Summon Agus)
- * Release date : 21-Dec-2021
+ * Release date : 11-Jan-2022
  * License      : GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
  * Repository   : https://github.com/agusmakmun/django-markdown-editor
 **/
 :root{--primary:#79aec8;--secondary:#417690}body{margin:0;padding:0;font-size:14px;color:#333;background:#fff}#container{-webkit-box-sizing:unset;box-sizing:unset}#branding h1{margin:0!important}body,button,h1,h2,h3,h4,h5,input,optgroup,select{font-family:Roboto,"Lucida Grande","DejaVu Sans","Bitstream Vera Sans",Verdana,Arial,sans-serif}h1,h2,h3,h4,h5{font-weight:700!important;line-height:unset!important}h1{margin:0 0 20px!important;font-weight:300!important;font-size:20px!important;color:#333!important}h2{font-size:16px!important;margin:1em 0 .5em 0!important}h2.subhead{font-weight:400!important;margin-top:0!important}h3{font-size:14px!important;margin:.8em 0 .3em 0!important;color:#333!important;font-weight:700!important}h4{font-size:12px!important;margin:1em 0 .8em 0!important;padding-bottom:3px!important}h5{font-size:10px!important;margin:1.5em 0 .5em 0!important;color:#333!important;text-transform:uppercase!important;letter-spacing:1px!important}.button,.submit-row input,a.button,input[type=button],input[type=submit]{padding:5px 15px}nav.sticky caption{caption-side:unset}.ui.tabular.menu+.attached:not(.top).segment,.ui.tabular.menu+.attached:not(.top).segment+.attached:not(.top).segment{width:auto}fieldset .form-row>div{width:100%}fieldset .form-row .main-martor{display:grid!important}.submit-row a.deletelink{height:unset}.table.markdown-reference h2{font-size:1.5em;background:0 0;color:unset;padding:0;font-weight:300!important}.js-inline-admin-formset .form-row {display: revert}
```

### Comparing `martor-1.6.8/martor/static/martor/css/martor.bootstrap.css` & `martor-1.6.9/martor/static/martor/css/martor.bootstrap.css`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/martor/css/martor.bootstrap.min.css` & `martor-1.6.9/martor/static/martor/css/martor.bootstrap.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 /**
- * Name         : Martor v1.6.8
+ * Name         : Martor v1.6.9
  * Created by   : Agus Makmun (Summon Agus)
- * Release date : 21-Dec-2021
+ * Release date : 11-Jan-2022
  * License      : GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
  * Repository   : https://github.com/agusmakmun/django-markdown-editor
 **/
 body.overflow{overflow:hidden!important}.martor{height:500px;max-height:500px}.martor-field{width:100%;height:250px;min-height:100px}.main-martor{margin:1em 0;position:relative}.main-martor .modal-header{padding:10px 1rem}.main-martor .modal-header h5{font-size:16px}.main-martor .upload-progress{position:absolute;z-index:100;width:100%;height:100%;padding-top:5em;background:rgba(0,0,0,.85);color:#fff}.martor-toolbar{position:absolute;z-index:100;right:0;top:0}.enable-living .martor-toolbar{position:relative}.martor-toolbar .markdown-image-upload{position:relative;overflow:hidden}.martor-toolbar .markdown-image-upload input[type=file]{position:absolute;top:0;right:0;min-width:100%;min-height:100%;font-size:25px;padding:0 0 0 35px;text-align:right;filter: alpha(opacity=0);opacity:0;outline:none;cursor:inherit;display:block}.emoji-loader-init{min-height:200px!important;padding-top:4em}.emoji-content-body{font-size:12px}.insert-emoji{cursor:pointer}.table.markdown-reference{font-size:12px}.table.markdown-reference h1{font-size:2em}.table.markdown-reference h2{font-size:1.5em}.table.markdown-reference ol,.table.markdown-reference ul{padding-left:1rem!important}div.martor-preview{padding:1rem;overflow:auto;background:#fdfdfd}div.martor-preview-stale{background:repeating-linear-gradient(-45deg, #fff, #fff 10px, #f8f8f8 10px, #f8f8f8 20px) !important}.main-martor .nav-tabs{border-bottom:2px solid #dee2e6}.main-martor .nav-tabs .nav-link:focus,.main-martor .nav-tabs .nav-link:hover,.main-martor .nav-tabs .nav-link:hover{border-color:transparent}.main-martor .nav-tabs .nav-item.show .nav-link,.main-martor .nav-tabs .nav-link.active,.main-martor .nav-tabs .nav-link.active:hover{border-color:transparent;border-bottom:2px solid #333;color:#495057}.main-martor .tab-pane{position:relative}.icon.expand-editor{position:absolute;bottom:-8px;right:8px;z-index:100}.no-border{border:none!important}div.enable-living .martor-preview{display:block!important;opacity:unset!important;margin-top:1em!important;border:1px solid #efefef!important;border-radius:0.28571429rem!important}div.enable-living .tab-martor-menu a.nav-link{display:none!important}.section-martor::-webkit-scrollbar-track{-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,0.3);border-radius:10px;background-color:#F5F5F5}.section-martor::-webkit-scrollbar{height:6px;width:6px;background-color:#F5F5F5}.section-martor::-webkit-scrollbar-thumb{border-radius:10px;-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,.3);background-color:#555}.ace_scrollbar-v{cursor:ns-resize}.main-martor-fullscreen{background:#fff;position:fixed;z-index:9999;max-height:100%;height:100%;width:100%;margin:0;left:0;top:0}.main-martor-fullscreen .fields.martor-toolbar{border-bottom:1px solid #ddd;margin:0}.main-martor-fullscreen .section-martor{height:90%;position:relative}.main-martor-fullscreen .martor-field,.main-martor-fullscreen .martor-preview{min-height:95vh}.marked-emoji,div.martor-preview .marked-emoji{max-width:20px}div.martor-preview{font-size:14px;line-height:1.6}div.martor-preview > *:first-child{margin-top:0 !important}div.martor-preview > *:last-child{margin-bottom:20px !important}div.martor-preview a.absent{color:#c00}div.martor-preview a.anchor{display:block;padding-left:30px;margin-left:-30px;cursor:pointer;position:absolute;top:0;left:0;bottom:0}div.martor-preview h1,div.martor-preview h2,div.martor-preview h3,div.martor-preview h4,div.martor-preview h5,div.martor-preview h6{margin:20px 0 10px;padding:0;font-weight:bold !important;-webkit-font-smoothing:antialiased;cursor:text;position:relative;background:none}div.martor-preview h1:hover a.anchor,div.martor-preview h2:hover a.anchor,div.martor-preview h3:hover a.anchor,div.martor-preview h4:hover a.anchor,div.martor-preview h5:hover a.anchor,div.martor-preview h6:hover a.anchor{text-decoration:none;line-height:1;padding-left:0;margin-left:-22px;top:15%}div.martor-preview h1 code,div.martor-preview h1 tt,div.martor-preview h2 code,div.martor-preview h2 tt,div.martor-preview h3 code,div.martor-preview h3 tt,div.martor-preview h4 code,div.martor-preview h4 tt,div.martor-preview h5 code,div.martor-preview h5 tt,div.martor-preview h6 code,div.martor-preview h6 tt{font-size:inherit}div.martor-preview h1{font-size:28px !important;color:#000 !important}div.martor-preview h2{font-size:24px !important;color:#000 !important}div.martor-preview h3{font-size:18px !important}div.martor-preview h4{font-size:16px !important}div.martor-preview h5{font-size:14px !important;text-transform:none !important}div.martor-preview h6{color:#777;font-size:14px}div.martor-preview blockquote,div.martor-preview dl,div.martor-preview ol,div.martor-preview p,div.martor-preview pre,div.martor-preview table,div.martor-preview ul{margin:15px 0}div.martor-preview hr{background:transparent url("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAYAAAAECAYAAACtBE5DAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAyJpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuMC1jMDYwIDYxLjEzNDc3NywgMjAxMC8wMi8xMi0xNzozMjowMCAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvIiB4bWxuczp4bXBNTT0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL21tLyIgeG1sbnM6c3RSZWY9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9zVHlwZS9SZXNvdXJjZVJlZiMiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENTNSBNYWNpbnRvc2giIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6OENDRjNBN0E2NTZBMTFFMEI3QjRBODM4NzJDMjlGNDgiIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6OENDRjNBN0I2NTZBMTFFMEI3QjRBODM4NzJDMjlGNDgiPiA8eG1wTU06RGVyaXZlZEZyb20gc3RSZWY6aW5zdGFuY2VJRD0ieG1wLmlpZDo4Q0NGM0E3ODY1NkExMUUwQjdCNEE4Mzg3MkMyOUY0OCIgc3RSZWY6ZG9jdW1lbnRJRD0ieG1wLmRpZDo4Q0NGM0E3OTY1NkExMUUwQjdCNEE4Mzg3MkMyOUY0OCIvPiA8L3JkZjpEZXNjcmlwdGlvbj4gPC9yZGY6UkRGPiA8L3g6eG1wbWV0YT4gPD94cGFja2V0IGVuZD0iciI/PqqezsUAAAAfSURBVHjaYmRABcYwBiM2QSA4y4hNEKYDQxAEAAIMAHNGAzhkPOlYAAAAAElFTkSuQmCC") repeat-x 0 0;border:0 none;color:#ccc;height:4px;padding:0}div.martor-preview > h1:first-child,div.martor-preview > h1:first-child+h2,div.martor-preview > h2:first-child,div.martor-preview > h3:first-child,div.martor-preview > h4:first-child,div.martor-preview > h5:first-child,div.martor-preview > h6:first-child{margin-top:0;padding-top:0}div.martor-preview a:first-child h1,div.martor-preview a:first-child h2,div.martor-preview a:first-child h3,div.martor-preview a:first-child h4,div.martor-preview a:first-child h5,div.martor-preview a:first-child h6{margin-top:0;padding-top:0}div.martor-preview h1+p,div.martor-preview h2+p,div.martor-preview h3+p,div.martor-preview h4+p,div.martor-preview h5+p,div.martor-preview h6+p{margin-top:0}div.martor-preview li p.first{display:inline-block}div.martor-preview ul li{list-style:disc}div.martor-preview ol,div.martor-preview ul{padding-left:30px}div.martor-preview ol.no-list,div.martor-preview ul.no-list{list-style-type:none;padding:0}div.martor-preview ol li > :first-child,div.martor-preview ol li ul:first-of-type,div.martor-preview ul li > :first-child,div.martor-preview ul li ul:first-of-type{margin-top:0}div.martor-preview ol ol,div.martor-preview ol ul,div.martor-preview ul ol,div.martor-preview ul ul{margin-bottom:0}div.martor-preview dl{padding:0}div.martor-preview dl dt{font-size:14px;font-weight:bold;font-style:italic;padding:0;margin:15px 0 5px}div.martor-preview dl dt:first-child{padding:0}div.martor-preview dl dt > :first-child{margin-top:0}div.martor-preview dl dt > :last-child{margin-bottom:0}div.martor-preview dl dd{margin:0 0 15px;padding:0 15px}div.martor-preview dl dd > :first-child{margin-top:0}div.martor-preview dl dd > :last-child{margin-bottom:0}div.martor-preview blockquote{border-left:4px solid #DDD;padding:5px 15px;color:#777;background-color:#fff}div.martor-preview blockquote > :first-child{margin-top:0}div.martor-preview blockquote > :last-child{margin-bottom:0}div.martor-preview table th{font-weight:bold}div.martor-preview table td,div.martor-preview table th{border:1px solid #ccc;padding:6px 13px}div.martor-preview table tr{border-top:1px solid #ccc;background-color:#fff}div.martor-preview table tr:nth-child(2n){background-color:#f8f8f8}div.martor-preview img,div.martor-preview p img{max-width:100%;-moz-box-sizing:border-box;box-sizing:border-box}div.martor-preview span.frame{display:block;overflow:hidden}div.martor-preview span.frame > span{border:1px solid #ddd;display:block;float:left;overflow:hidden;margin:13px 0 0;padding:7px;width:auto}div.martor-preview span.frame span img{display:block;float:left}div.martor-preview span.frame span span{clear:both;color:#333;display:block;padding:5px 0 0}div.martor-preview span.align-center{display:block;overflow:hidden;clear:both}div.martor-preview span.align-center > span{display:block;overflow:hidden;margin:13px auto 0;text-align:center}div.martor-preview span.align-center span img{margin:0 auto;text-align:center}div.martor-preview span.align-right{display:block;overflow:hidden;clear:both}div.martor-preview span.align-right > span{display:block;overflow:hidden;margin:13px 0 0;text-align:right}div.martor-preview span.align-right span img{margin:0;text-align:right}div.martor-preview span.float-left{display:block;margin-right:13px;overflow:hidden;float:left}div.martor-preview span.float-left span{margin:13px 0 0}div.martor-preview span.float-right{display:block;margin-left:13px;overflow:hidden;float:right}div.martor-preview span.float-right > span{display:block;overflow:hidden;margin:13px auto 0;text-align:right}div.martor-preview code,div.martor-preview tt{margin:0 2px;padding:0 5px;border:1px solid #eaeaea;background-color:#f8f8f8;border-radius:3px}div.martor-preview code{white-space:nowrap}div.martor-preview pre > code{margin:0;padding:0;white-space:pre;border:none;background:transparent}div.martor-preview .highlight pre,div.martor-preview pre{border:1px solid #f0f0f0;padding:16px;overflow:auto;font-size:85%;line-height:1.45;background-color:#f6f8fa;border-radius:3px}div.martor-preview pre code,div.martor-preview pre tt{margin:0;padding:0;background-color:transparent;border:none}
```

### Comparing `martor-1.6.8/martor/static/martor/css/martor.semantic.css` & `martor-1.6.9/martor/static/martor/css/martor.semantic.css`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/martor/css/martor.semantic.min.css` & `martor-1.6.9/martor/static/martor/css/martor.semantic.min.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 /**
- * Name         : Martor v1.6.8
+ * Name         : Martor v1.6.9
  * Created by   : Agus Makmun (Summon Agus)
- * Release date : 21-Dec-2021
+ * Release date : 11-Jan-2022
  * License      : GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
  * Repository   : https://github.com/agusmakmun/django-markdown-editor
 **/
 .submit-row a{box-sizing:content-box}body.overflow{overflow:hidden!important}.section-martor::-webkit-scrollbar-track{-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,0.3);border-radius:10px;background-color:#F5F5F5}.section-martor::-webkit-scrollbar{height:6px;width:6px;background-color:#F5F5F5}.section-martor::-webkit-scrollbar-thumb{border-radius:10px;-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,.3);background-color:#555}.ace_scrollbar-v{cursor:ns-resize}.main-martor{}.martor-toolbar{padding:0 0.85714286em!important 4px!important !important}.martor-toolbar .ui.icon .markdown-image-upload{position:relative;overflow:hidden}.martor-toolbar .ui.icon .markdown-image-upload input[type=file]{position:absolute;top:0;right:0;min-width:100%;min-height:100%;font-size:25px;padding:0 0 0 35px;text-align:right;filter: alpha(opacity=0);opacity:0;outline:none;cursor:inherit;display:block}.emoji-loader-init{min-height:200px!important}.insert-emoji{cursor:pointer}.main-martor-fullscreen{background:#fff;position:fixed;z-index:9999;max-height:100%;height:100%;width:100%;margin:0;left:0;top:0}.main-martor-fullscreen .fields.martor-toolbar{border-bottom:1px solid #ddd;margin:0}.main-martor-fullscreen .section-martor{height:90%;position:relative}.main-martor-fullscreen .martor-field,.main-martor-fullscreen .martor-preview{min-height:95vh}.marked-emoji,div.martor-preview .marked-emoji{max-width:20px}div.martor-preview{font-size:14px;line-height:1.6}div.martor-preview > *:first-child{margin-top:0 !important}div.martor-preview > *:last-child{margin-bottom:20px !important}div.martor-preview a.absent{color:#c00}div.martor-preview a.anchor{display:block;padding-left:30px;margin-left:-30px;cursor:pointer;position:absolute;top:0;left:0;bottom:0}div.martor-preview h1,div.martor-preview h2,div.martor-preview h3,div.martor-preview h4,div.martor-preview h5,div.martor-preview h6{margin:20px 0 10px;padding:0;font-weight:bold !important;-webkit-font-smoothing:antialiased;cursor:text;position:relative;background:none}div.martor-preview h1:hover a.anchor,div.martor-preview h2:hover a.anchor,div.martor-preview h3:hover a.anchor,div.martor-preview h4:hover a.anchor,div.martor-preview h5:hover a.anchor,div.martor-preview h6:hover a.anchor{text-decoration:none;line-height:1;padding-left:0;margin-left:-22px;top:15%}div.martor-preview h1 code,div.martor-preview h1 tt,div.martor-preview h2 code,div.martor-preview h2 tt,div.martor-preview h3 code,div.martor-preview h3 tt,div.martor-preview h4 code,div.martor-preview h4 tt,div.martor-preview h5 code,div.martor-preview h5 tt,div.martor-preview h6 code,div.martor-preview h6 tt{font-size:inherit}div.martor-preview h1{font-size:28px !important;color:#000 !important}div.martor-preview h2{font-size:24px !important;color:#000 !important}div.martor-preview h3{font-size:18px !important}div.martor-preview h4{font-size:16px !important}div.martor-preview h5{font-size:14px !important;text-transform:none !important}div.martor-preview h6{color:#777;font-size:14px}div.martor-preview blockquote,div.martor-preview dl,div.martor-preview ol,div.martor-preview p,div.martor-preview pre,div.martor-preview table,div.martor-preview ul{margin:15px 0}div.martor-preview hr{background:transparent url("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAYAAAAECAYAAACtBE5DAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAyJpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuMC1jMDYwIDYxLjEzNDc3NywgMjAxMC8wMi8xMi0xNzozMjowMCAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvIiB4bWxuczp4bXBNTT0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL21tLyIgeG1sbnM6c3RSZWY9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9zVHlwZS9SZXNvdXJjZVJlZiMiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENTNSBNYWNpbnRvc2giIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6OENDRjNBN0E2NTZBMTFFMEI3QjRBODM4NzJDMjlGNDgiIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6OENDRjNBN0I2NTZBMTFFMEI3QjRBODM4NzJDMjlGNDgiPiA8eG1wTU06RGVyaXZlZEZyb20gc3RSZWY6aW5zdGFuY2VJRD0ieG1wLmlpZDo4Q0NGM0E3ODY1NkExMUUwQjdCNEE4Mzg3MkMyOUY0OCIgc3RSZWY6ZG9jdW1lbnRJRD0ieG1wLmRpZDo4Q0NGM0E3OTY1NkExMUUwQjdCNEE4Mzg3MkMyOUY0OCIvPiA8L3JkZjpEZXNjcmlwdGlvbj4gPC9yZGY6UkRGPiA8L3g6eG1wbWV0YT4gPD94cGFja2V0IGVuZD0iciI/PqqezsUAAAAfSURBVHjaYmRABcYwBiM2QSA4y4hNEKYDQxAEAAIMAHNGAzhkPOlYAAAAAElFTkSuQmCC") repeat-x 0 0;border:0 none;color:#ccc;height:4px;padding:0}div.martor-preview > h1:first-child,div.martor-preview > h1:first-child+h2,div.martor-preview > h2:first-child,div.martor-preview > h3:first-child,div.martor-preview > h4:first-child,div.martor-preview > h5:first-child,div.martor-preview > h6:first-child{margin-top:0;padding-top:0}div.martor-preview a:first-child h1,div.martor-preview a:first-child h2,div.martor-preview a:first-child h3,div.martor-preview a:first-child h4,div.martor-preview a:first-child h5,div.martor-preview a:first-child h6{margin-top:0;padding-top:0}div.martor-preview h1+p,div.martor-preview h2+p,div.martor-preview h3+p,div.martor-preview h4+p,div.martor-preview h5+p,div.martor-preview h6+p{margin-top:0}div.martor-preview li p.first{display:inline-block}div.martor-preview ul li{list-style:disc}div.martor-preview ol,div.martor-preview ul{padding-left:30px}div.martor-preview ol.no-list,div.martor-preview ul.no-list{list-style-type:none;padding:0}div.martor-preview ol li > :first-child,div.martor-preview ol li ul:first-of-type,div.martor-preview ul li > :first-child,div.martor-preview ul li ul:first-of-type{margin-top:0}div.martor-preview ol ol,div.martor-preview ol ul,div.martor-preview ul ol,div.martor-preview ul ul{margin-bottom:0}div.martor-preview dl{padding:0}div.martor-preview dl dt{font-size:14px;font-weight:bold;font-style:italic;padding:0;margin:15px 0 5px}div.martor-preview dl dt:first-child{padding:0}div.martor-preview dl dt > :first-child{margin-top:0}div.martor-preview dl dt > :last-child{margin-bottom:0}div.martor-preview dl dd{margin:0 0 15px;padding:0 15px}div.martor-preview dl dd > :first-child{margin-top:0}div.martor-preview dl dd > :last-child{margin-bottom:0}div.martor-preview blockquote{border-left:4px solid #DDD;padding:5px 15px;color:#777;background-color:#fff}div.martor-preview blockquote > :first-child{margin-top:0}div.martor-preview blockquote > :last-child{margin-bottom:0}div.martor-preview table th{font-weight:bold}div.martor-preview table td,div.martor-preview table th{border:1px solid #ccc;padding:6px 13px}div.martor-preview table tr{border-top:1px solid #ccc;background-color:#fff}div.martor-preview table tr:nth-child(2n){background-color:#f8f8f8}div.martor-preview img,div.martor-preview p img{max-width:100%;-moz-box-sizing:border-box;box-sizing:border-box}div.martor-preview span.frame{display:block;overflow:hidden}div.martor-preview span.frame > span{border:1px solid #ddd;display:block;float:left;overflow:hidden;margin:13px 0 0;padding:7px;width:auto}div.martor-preview span.frame span img{display:block;float:left}div.martor-preview span.frame span span{clear:both;color:#333;display:block;padding:5px 0 0}div.martor-preview span.align-center{display:block;overflow:hidden;clear:both}div.martor-preview span.align-center > span{display:block;overflow:hidden;margin:13px auto 0;text-align:center}div.martor-preview span.align-center span img{margin:0 auto;text-align:center}div.martor-preview span.align-right{display:block;overflow:hidden;clear:both}div.martor-preview span.align-right > span{display:block;overflow:hidden;margin:13px 0 0;text-align:right}div.martor-preview span.align-right span img{margin:0;text-align:right}div.martor-preview span.float-left{display:block;margin-right:13px;overflow:hidden;float:left}div.martor-preview span.float-left span{margin:13px 0 0}div.martor-preview span.float-right{display:block;margin-left:13px;overflow:hidden;float:right}div.martor-preview span.float-right > span{display:block;overflow:hidden;margin:13px auto 0;text-align:right}div.martor-preview code,div.martor-preview tt{margin:0 2px;padding:0 5px;border:1px solid #eaeaea;background-color:#f8f8f8;border-radius:3px}div.martor-preview code{white-space:nowrap}div.martor-preview pre > code{margin:0;padding:0;white-space:pre;border:none;background:transparent}div.martor-preview .highlight pre,div.martor-preview pre{border:1px solid #f0f0f0;padding:16px;overflow:auto;font-size:85%;line-height:1.45;background-color:#f6f8fa;border-radius:3px}div.martor-preview pre code,div.martor-preview pre tt{margin:0;padding:0;background-color:transparent;border:none}.section-martor{}.section-martor div[data-tab="editor-tab-description"]{padding:0 !important}.martor{height:500px;max-height:500px}.martor-field{width:100%;height:250px;min-height:100px}div.martor-preview{padding:1rem;overflow:auto;background:#F9F9F9}div.martor-preview-stale{background:repeating-linear-gradient(-45deg, #fff, #fff 10px, #f8f8f8 10px, #f8f8f8 20px) !important}.icon.expand-editor{position:absolute;bottom:0.8em;right:0}.no-border{border:none!important}div.enable-living .martor-preview{display:block!important;opacity:unset!important;border:1px solid #efefef!important;border-radius:0.28571429rem!important}div.enable-living .tab-martor-menu a.item{display:none!important}
```

### Comparing `martor-1.6.8/martor/static/martor/js/martor.bootstrap.js` & `martor-1.6.9/martor/static/martor/js/martor.bootstrap.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /**
- * Name         : Martor v1.6.8
+ * Name         : Martor v1.6.9
  * Created by   : Agus Makmun (Summon Agus)
- * Release date : 21-Dec-2021
+ * Release date : 11-Jan-2022
  * License      : GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
  * Repository   : https://github.com/agusmakmun/django-markdown-editor
  **/
 
 (function($) {
     if (!$) {
         $ = django.jQuery;
```

### Comparing `martor-1.6.8/martor/static/martor/js/martor.bootstrap.min.js` & `martor-1.6.9/martor/static/martor/js/martor.bootstrap.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /**
- * Name         : Martor v1.6.8
+ * Name         : Martor v1.6.9
  * Created by   : Agus Makmun (Summon Agus)
- * Release date : 21-Dec-2021
+ * Release date : 11-Jan-2022
  * License      : GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
  * Repository   : https://github.com/agusmakmun/django-markdown-editor
  **/
 ! function(e) {
     e || (e = django.jQuery), e.fn.martor = function() {
         e(".martor").trigger("martor.init");
         var n = function(e) {
```

### Comparing `martor-1.6.8/martor/static/martor/js/martor.semantic.js` & `martor-1.6.9/martor/static/martor/js/martor.semantic.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /**
- * Name         : Martor v1.6.8
+ * Name         : Martor v1.6.9
  * Created by   : Agus Makmun (Summon Agus)
- * Release date : 21-Dec-2021
+ * Release date : 11-Jan-2022
  * License      : GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
  * Repository   : https://github.com/agusmakmun/django-markdown-editor
  **/
 
 (function($) {
     if (!$) {
         $ = django.jQuery;
```

### Comparing `martor-1.6.8/martor/static/martor/js/martor.semantic.min.js` & `martor-1.6.9/martor/static/martor/js/martor.semantic.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /**
- * Name         : Martor v1.6.8
+ * Name         : Martor v1.6.9
  * Created by   : Agus Makmun (Summon Agus)
- * Release date : 21-Dec-2021
+ * Release date : 11-Jan-2022
  * License      : GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
  * Repository   : https://github.com/agusmakmun/django-markdown-editor
  **/
 ! function(e) {
     e || (e = django.jQuery), e.fn.martor = function() {
         e(".martor").trigger("martor.init");
         var n = function(e) {
```

### Comparing `martor-1.6.8/martor/static/plugins/css/ace.min.css` & `martor-1.6.9/martor/static/plugins/css/ace.min.css`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/css/bootstrap.min.css` & `martor-1.6.9/martor/static/plugins/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/css/resizable.min.css` & `martor-1.6.9/martor/static/plugins/css/resizable.min.css`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/css/semantic.min.css` & `martor-1.6.9/martor/static/plugins/css/semantic.min.css`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/brand-icons.eot` & `martor-1.6.9/martor/static/plugins/fonts/brand-icons.eot`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/brand-icons.svg` & `martor-1.6.9/martor/static/plugins/fonts/brand-icons.svg`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/brand-icons.ttf` & `martor-1.6.9/martor/static/plugins/fonts/brand-icons.ttf`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/brand-icons.woff` & `martor-1.6.9/martor/static/plugins/fonts/brand-icons.woff`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/brand-icons.woff2` & `martor-1.6.9/martor/static/plugins/fonts/brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/icons.eot` & `martor-1.6.9/martor/static/plugins/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/icons.svg` & `martor-1.6.9/martor/static/plugins/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/icons.ttf` & `martor-1.6.9/martor/static/plugins/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/icons.woff` & `martor-1.6.9/martor/static/plugins/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/icons.woff2` & `martor-1.6.9/martor/static/plugins/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/outline-icons.eot` & `martor-1.6.9/martor/static/plugins/fonts/outline-icons.eot`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/outline-icons.svg` & `martor-1.6.9/martor/static/plugins/fonts/outline-icons.svg`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/outline-icons.ttf` & `martor-1.6.9/martor/static/plugins/fonts/outline-icons.ttf`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/outline-icons.woff` & `martor-1.6.9/martor/static/plugins/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/fonts/outline-icons.woff2` & `martor-1.6.9/martor/static/plugins/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/images/commonmark.png` & `martor-1.6.9/martor/static/plugins/images/commonmark.png`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/images/flags.png` & `martor-1.6.9/martor/static/plugins/images/flags.png`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/images/heart.png` & `martor-1.6.9/martor/static/plugins/images/heart.png`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/ace.js` & `martor-1.6.9/martor/static/plugins/js/ace.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/bootstrap.min.js` & `martor-1.6.9/martor/static/plugins/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/emojis.min.js` & `martor-1.6.9/martor/static/plugins/js/emojis.min.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/ext-language_tools.js` & `martor-1.6.9/martor/static/plugins/js/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/highlight.min.js` & `martor-1.6.9/martor/static/plugins/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/jquery.min.js` & `martor-1.6.9/martor/static/plugins/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/jquery.slim.min.js` & `martor-1.6.9/martor/static/plugins/js/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/mode-markdown.js` & `martor-1.6.9/martor/static/plugins/js/mode-markdown.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/resizable.min.js` & `martor-1.6.9/martor/static/plugins/js/resizable.min.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/semantic.min.js` & `martor-1.6.9/martor/static/plugins/js/semantic.min.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/snippets/markdown.js` & `martor-1.6.9/martor/static/plugins/js/snippets/markdown.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/spellcheck.js` & `martor-1.6.9/martor/static/plugins/js/spellcheck.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/theme-github.js` & `martor-1.6.9/martor/static/plugins/js/theme-github.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/static/plugins/js/typo.js` & `martor-1.6.9/martor/static/plugins/js/typo.js`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/bootstrap/editor.html` & `martor-1.6.9/martor/templates/martor/bootstrap/editor.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/bootstrap/emoji.html` & `martor-1.6.9/martor/templates/martor/bootstrap/emoji.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/bootstrap/guide.html` & `martor-1.6.9/martor/templates/martor/bootstrap/guide.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/bootstrap/toolbar.html` & `martor-1.6.9/martor/templates/martor/bootstrap/toolbar.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/semantic/editor.html` & `martor-1.6.9/martor/templates/martor/semantic/editor.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/semantic/emoji.html` & `martor-1.6.9/martor/templates/martor/semantic/emoji.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/semantic/guide.html` & `martor-1.6.9/martor/templates/martor/semantic/guide.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/templates/martor/semantic/toolbar.html` & `martor-1.6.9/martor/templates/martor/semantic/toolbar.html`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/tests/tests.py` & `martor-1.6.9/martor/tests/tests.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/urls.py` & `martor-1.6.9/martor/urls.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/utils.py` & `martor-1.6.9/martor/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     # Strip HTML tags
     markdown_text = strip_tags(markdown_text)
 
     # Sanitize Markdown links
     # https://github.com/netbox-community/netbox/commit/5af2b3c2f577a01d177cb24cda1019551a2a4b64
     schemes = "|".join(ALLOWED_URL_SCHEMES)
-    pattern = fr"\[(.+)\]\((?!({schemes})).*:(.+)\)"
+    pattern = fr"\[(.+)\]\((?!({schemes})).*(:|;)(.+)\)"
     markdown_text = re.sub(
         pattern,
         "[\\1](\\3)",
         markdown_text,
         flags=re.IGNORECASE,
     )
```

### Comparing `martor-1.6.8/martor/views.py` & `martor-1.6.9/martor/views.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor/widgets.py` & `martor-1.6.9/martor/widgets.py`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/martor.egg-info/PKG-INFO` & `martor-1.6.9/martor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: martor
-Version: 1.6.8
+Version: 1.6.9
 Summary: Django Markdown Editor
 Home-page: https://github.com/agusmakmun/django-markdown-editor
 Author: Agus Makmun (Summon Agus)
 Author-email: summon.agus@gmail.com
 License: GNUGPL-v3
-Download-URL: https://github.com/agusmakmun/django-markdown-editor/tarball/v1.6.8
+Download-URL: https://github.com/agusmakmun/django-markdown-editor/tarball/v1.6.9
 Keywords: martor,django markdown,django markdown editor
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
```

### Comparing `martor-1.6.8/martor.egg-info/SOURCES.txt` & `martor-1.6.9/martor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `martor-1.6.8/setup.py` & `martor-1.6.9/setup.py`

 * *Files identical despite different names*


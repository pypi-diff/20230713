# Comparing `tmp/modelw_project_maker-2023.4.0b1.tar.gz` & `tmp/modelw_project_maker-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_project_maker-2023.4.0b1.tar", max compression
+gzip compressed data, was "modelw_project_maker-2023.7.0.tar", max compression
```

## Comparing `modelw_project_maker-2023.4.0b1.tar` & `modelw_project_maker-2023.7.0.tar`

### file list

```diff
@@ -1,82 +1,85 @@
--rw-r--r--   0        0        0     5377 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/README.md
--rw-r--r--   0        0        0     1363 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/__init__.py
--rw-r--r--   0        0        0     8748 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/__main__.py
--rw-r--r--   0        0        0       45 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/errors.py
--rw-r--r--   0        0        0      143 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/__init__.py
--rw-r--r--   0        0        0     4470 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_api.py
--rw-r--r--   0        0        0     6518 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_base.py
--rw-r--r--   0        0        0      703 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_common.py
--rw-r--r--   0        0        0     3909 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_front.py
--rw-r--r--   0        0        0     3446 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/namer.py
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/py.typed
--rw-r--r--   0        0        0      178 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.editorconfig
--rw-r--r--   0        0        0       27 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.formatignore
--rw-r--r--   0        0        0     3042 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.gitignore
--rw-r--r--   0        0        0       77 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.prettierrc
--rw-r--r--   0        0        0     1488 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/README.md
--rw-r--r--   0        0        0     3034 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/.dockerignore
--rw-r--r--   0        0        0      381 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/.env-template
--rw-r--r--   0        0        0      181 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/Dockerfile
--rw-r--r--   0        0        0      236 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/Makefile
--rw-r--r--   0        0        0     1140 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/README.md
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
--rw-r--r--   0        0        0       93 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
--rw-r--r--   0        0        0     8589 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
--rw-r--r--   0        0        0     2818 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
--rw-r--r--   0        0        0      655 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
--rw-r--r--   0        0        0      233 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
--rwxr-xr-x   0        0        0      755 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
--rwxr-xr-x   0        0        0      240 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
--rwxr-xr-x   0        0        0      471 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
--rwxr-xr-x   0        0        0      844 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
--rwxr-xr-x   0        0        0      903 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
--rwxr-xr-x   0        0        0     1092 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
--rwxr-xr-x   0        0        0      658 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
--rwxr-xr-x   0        0        0      718 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
--rwxr-xr-x   0        0        0      485 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
--rwxr-xr-x   0        0        0     2749 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
--rwxr-xr-x   0        0        0     2067 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
--rw-r--r--   0        0        0     1883 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
--rw-r--r--   0        0        0      159 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
--rw-r--r--   0        0        0     3921 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
--rw-r--r--   0        0        0     3150 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
--rw-r--r--   0        0        0     1343 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
--rw-r--r--   0        0        0     2486 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
--rw-r--r--   0        0        0      194 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
--rw-r--r--   0        0        0      386 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
--rw-r--r--   0        0        0       70 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
--rw-r--r--   0        0        0      851 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
--rw-r--r--   0        0        0      273 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
--rw-r--r--   0        0        0      219 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
--rw-r--r--   0        0        0     2076 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
--rw-r--r--   0        0        0     1681 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
--rw-r--r--   0        0        0      443 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
--rwxr-xr-x   0        0        0      666 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/manage.py
--rwxr-xr-x   0        0        0      151 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/pmanage
--rw-r--r--   0        0        0      863 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/pyproject.toml
--rw-r--r--   0        0        0     3034 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.dockerignore
--rw-r--r--   0        0        0      182 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.env-template
--rw-r--r--   0        0        0      332 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.eslintrc.js
--rw-r--r--   0        0        0        8 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.gitignore
--rw-r--r--   0        0        0       13 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.nvmrc
--rw-r--r--   0        0        0      185 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/Dockerfile
--rw-r--r--   0        0        0     1599 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/README.md
--rw-r--r--   0        0        0      112 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/components/blocks/title-1.vue
--rw-r--r--   0        0        0    11485 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue
--rw-r--r--   0        0        0      558 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/nuxt.config.js
--rw-r--r--   0        0        0      796 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/package.json
--rw-r--r--   0        0        0     5202 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/pages/[...wagtail].vue
--rw-r--r--   0        0        0       80 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
--rw-r--r--   0        0        0      483 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/plugins/dom.client.ts
--rw-r--r--   0        0        0      505 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/plugins/dom.server.ts
--rw-r--r--   0        0        0     7602 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template.py
--rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 modelw_project_maker-2023.4.0b1/PKG-INFO
+-rw-r--r--   0        0        0     5377 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/README.md
+-rw-r--r--   0        0        0     1355 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/__init__.py
+-rw-r--r--   0        0        0     8748 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/__main__.py
+-rw-r--r--   0        0        0       45 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/errors.py
+-rw-r--r--   0        0        0      143 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/__init__.py
+-rw-r--r--   0        0        0     4470 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_api.py
+-rw-r--r--   0        0        0     6518 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_base.py
+-rw-r--r--   0        0        0      703 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_common.py
+-rw-r--r--   0        0        0     3836 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_front.py
+-rw-r--r--   0        0        0     3446 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/namer.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/py.typed
+-rw-r--r--   0        0        0      178 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.editorconfig
+-rw-r--r--   0        0        0       27 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.formatignore
+-rw-r--r--   0        0        0     3042 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.gitignore
+-rw-r--r--   0        0        0       77 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.prettierrc
+-rw-r--r--   0        0        0     1488 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/README.md
+-rw-r--r--   0        0        0     3034 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/.dockerignore
+-rw-r--r--   0        0        0      381 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/.env-template
+-rw-r--r--   0        0        0      181 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/Dockerfile
+-rw-r--r--   0        0        0      236 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/Makefile
+-rw-r--r--   0        0        0     1140 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
+-rw-r--r--   0        0        0       93 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
+-rw-r--r--   0        0        0     8589 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2818 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
+-rw-r--r--   0        0        0     2036 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
+-rw-r--r--   0        0        0      655 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
+-rw-r--r--   0        0        0      233 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
+-rwxr-xr-x   0        0        0      755 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
+-rwxr-xr-x   0        0        0      240 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
+-rwxr-xr-x   0        0        0      471 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
+-rwxr-xr-x   0        0        0      844 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
+-rwxr-xr-x   0        0        0      903 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
+-rwxr-xr-x   0        0        0     1092 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
+-rwxr-xr-x   0        0        0      658 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
+-rwxr-xr-x   0        0        0      718 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
+-rwxr-xr-x   0        0        0      485 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
+-rwxr-xr-x   0        0        0     2749 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
+-rwxr-xr-x   0        0        0     2067 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
+-rw-r--r--   0        0        0     1883 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
+-rw-r--r--   0        0        0      159 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
+-rw-r--r--   0        0        0     3921 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
+-rw-r--r--   0        0        0     1343 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
+-rw-r--r--   0        0        0     2486 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
+-rw-r--r--   0        0        0      194 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
+-rw-r--r--   0        0        0       70 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
+-rw-r--r--   0        0        0      273 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
+-rw-r--r--   0        0        0      219 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
+-rw-r--r--   0        0        0     2076 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
+-rw-r--r--   0        0        0     1681 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
+-rw-r--r--   0        0        0      443 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
+-rwxr-xr-x   0        0        0      666 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/manage.py
+-rwxr-xr-x   0        0        0      151 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/pmanage
+-rw-r--r--   0        0        0      861 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/pyproject.toml
+-rw-r--r--   0        0        0     3034 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.dockerignore
+-rw-r--r--   0        0        0      182 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.env-template
+-rw-r--r--   0        0        0      332 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.eslintrc.js
+-rw-r--r--   0        0        0        8 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.gitignore
+-rw-r--r--   0        0        0       13 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.nvmrc
+-rw-r--r--   0        0        0      185 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/Dockerfile
+-rw-r--r--   0        0        0     1601 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/README.md
+-rw-r--r--   0        0        0      112 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/components/blocks/title-1.vue
+-rw-r--r--   0        0        0    11513 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/components/server-templated-component.vue
+-rw-r--r--   0        0        0     2941 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/error.vue
+-rw-r--r--   0        0        0      558 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/nuxt.config.js
+-rw-r--r--   0        0        0      789 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/package.json
+-rw-r--r--   0        0        0     5048 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/pages/[...wagtail].vue
+-rw-r--r--   0        0        0       80 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
+-rw-r--r--   0        0        0      483 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/plugins/dom.client.ts
+-rw-r--r--   0        0        0      505 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/plugins/dom.server.ts
+-rw-r--r--   0        0        0       98 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/tsconfig.json
+-rw-r--r--   0        0        0     7602 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template.py
+-rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 modelw_project_maker-2023.7.0/PKG-INFO
```

### Comparing `modelw_project_maker-2023.4.0b1/README.md` & `modelw_project_maker-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/pyproject.toml` & `modelw_project_maker-2023.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-project-maker"
-version = "2023.4.0b1"
+version = "2023.7.0"
 packages = [
     {  include = "model_w/project_maker", from = "src" }
 ]
 
 description = "A tool to create Model-W-compliant projects"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
@@ -14,33 +14,33 @@
 readme = "README.md"
 keywords = ["model-w", "django", "nuxt", "boilerplate", "template"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.scripts]
 project_maker = "model_w.project_maker.__main__:__main__"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 setuptools = "*"
-rich = "^12.5.1"
+rich = "^13.4.2"
 Unidecode = "^1.3.4"
-black = "^22.8.0"
+black = "^22"
 isort = "^5.10.1"
 tomlkit = "^0.11.4"
 node-edge = "^0.1.0b2"
 monoformat = "^0.1.0b3"
-pathspec = "^0.10.2"
+pathspec = "~0.10"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 
 [tool.isort]
 profile = "black"
 known_first_party = [
```

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/__main__.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_api.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_api.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_base.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_base.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_common.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_common.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_front.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_front.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,17 +102,14 @@
             new_path = file_path.parent / ".env"
 
             with open(file_path, encoding="utf-8") as f, open(
                 new_path, "w", encoding="utf-8"
             ) as g:
                 g.write(f.read())
 
-            file_path.rename(new_path)
-            file_path = new_path
-
         if not re.compile(
             r".*\.([jt]sx?|json|md|vue|php|html?|svelte|ya?ml|(s?c|le)ss)$",
             re.IGNORECASE,
         ).match(file_path.name):
             return
 
         info = self.prettier.getFileInfo(f"{file_path}")
```

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/namer.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/namer.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.gitignore` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.gitignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/README.md` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/.dockerignore` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/README.md` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/manage.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/manage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/pyproject.toml` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 license = "Proprietary"
 
 packages = [
     {include = "___project_name__snake___"},
 ]
 
 [tool.poetry.dependencies]
-python = "~3.10"
+python = "~3.11"
 modelw-preset-django = {extras = [
     # :: IF api__celery
     "celery",
     # :: ENDIF
     # :: IF api__channels
     "channels",
     # :: ENDIF
     # :: IF api__wagtail
     "wagtail",
     # :: ENDIF
     # :: IF api__wsgi
     "gunicorn",
     # :: ENDIF
-], version = ">=2023.4.0b1,<2023.7.0", allow-prereleases = true}
+], version = ">=2023.7.0,<2023.8.0", allow-prereleases = true}
 drf-spectacular = {extras = ["sidecar"], version = "^0.26.2"}
 
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
 ipython = "*"
```

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.dockerignore` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/README.md` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The content pages are served by Wagtail on the Django side. This behavior is
 handled by the [catch-all page](./pages/[...wagtail].vue) which will:
 
 1. Call the Wagtail API for the page we're trying to get
 2. If there is any error (404, 500, ...) the error will be rendered as a Nuxt
    error. The same goes with redirections.
 3. If the page is found, it will be rendered using the
-   [`ServerTemplatedComponent`](./components/ServerTemplatedComponent.vue)
+   [`ServerTemplatedComponent`](./components/server-templated-component.vue)
    component. It lets you declare Vue components that have their JS and CSS
    (non-scoped) declared in a `.vue` file but the template coming from the
    server.
 
 In order to render more components through the `ServerTemplatedComponent`, you
 must:
```

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/components/server-templated-component.vue`

 * *Files 0% similar despite different names*

```diff
@@ -36,18 +36,18 @@
     }
 
     return out;
 }
 
 const propWhitelist = [
     /**
-    * These are options that comes from the optionApi
-    * that comes with the standard lifecycle of Vue2 and also part of vue3
-    * you can review it in this link https://vuejs.org/api/options-lifecycle.html
-    */
+     * These are options that comes from the optionApi
+     * that comes with the standard lifecycle of Vue2 and also part of vue3
+     * you can review it in this link https://vuejs.org/api/options-lifecycle.html
+     */
     "beforeCreate",
     "created",
     "beforeMount",
     "mounted",
     "beforeUpdate",
     "updated",
     "beforeUnmount",
@@ -56,20 +56,21 @@
     "data",
     "computed",
     "watch",
     "methods",
     "props",
     "errorCaptured",
     "serverPrefetch",
+    "components",
     /**
-    * These are the methods needed for the composition api,
-    * they help to improve SSR and load speed of the pages.
-    * You can see more information in the next link:
-    * https://vuejs.org/api/composition-api-lifecycle.html#ondeactivated
-    */
+     * These are the methods needed for the composition api,
+     * they help to improve SSR and load speed of the pages.
+     * You can see more information in the next link:
+     * https://vuejs.org/api/composition-api-lifecycle.html#ondeactivated
+     */
     "onMounted",
     "onUpdated",
     "onUnmounted",
     "onBeforeMount",
     "onBeforeUpdate",
     "onBeforeUnmount",
     "onErrorCaptured",
@@ -79,15 +80,15 @@
      * The following ones are only for development porpoise
      */
     "onRenderTracked",
     "onRenderTriggered",
     /**
      * This is only SSR method
      */
-    "onServerPrefetch"
+    "onServerPrefetch",
 ];
 
 export default {
     props: {
         /**
          * HTML content to derive templates from
          */
```

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/nuxt.config.js` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/nuxt.config.js`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/package.json` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'dependencies'": "{'@model-w/preset-nuxt3': '>=2023.7.0 && <2023.8.0', 'http-proxy-middleware': "*

 * *                   "'^2.0.x', 'jsdom': '22.1.x', 'nuxt': '3.6.x', 'sass': '1.63.x', 'vue': "*

 * *                   "'3.3.x'}",*

 * * "'devDependencies'": "{'consola': '^3.2.x'}"}*

```diff
@@ -1,24 +1,24 @@
 {
     "dependencies": {
         "@model-w/axios": "1.x",
-        "@model-w/preset-nuxt3": ">=2023.4.0-beta.1 && <2023.7.0",
+        "@model-w/preset-nuxt3": ">=2023.7.0 && <2023.8.0",
         "@model-w/proxy": "2.x",
         "@model-w/sentry": "1.x",
         "@vuelidate/core": "2.0.x",
         "@vuelidate/validators": "2.0.x",
-        "http-proxy-middleware": "^2.0.6",
-        "jsdom": "21.1.x",
-        "nuxt": "3.4.x",
-        "sass": "1.62.x",
+        "http-proxy-middleware": "^2.0.x",
+        "jsdom": "22.1.x",
+        "nuxt": "3.6.x",
+        "sass": "1.63.x",
         "vite-svg-loader": "4.0.x",
-        "vue": "3.2.x"
+        "vue": "3.3.x"
     },
     "devDependencies": {
-        "consola": "^3.1.0",
+        "consola": "^3.2.x",
         "prettier": "*"
     },
     "name": "___project_name__snake___",
     "private": true,
     "scripts": {
         "build": "nuxt build",
         "dev": "nuxt dev",
```

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/pages/[...wagtail].vue` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/pages/[...wagtail].vue`

 * *Files 25% similar despite different names*

```diff
@@ -1,165 +1,172 @@
 <template>
     <ServerTemplatedComponent
-        :content="html"
+        :content="html as string"
         :components-defs="defs"
         @head="receiveHeadData"
     />
 </template>
 
-<script>
-import { defineNuxtComponent } from "nuxt/app";
-import ServerTemplatedComponent from "~/components/server-templated-component.vue";
-import Title1 from "~/components/blocks/title-1.vue";
+<script setup lang="ts">
+import Title1 from "@/components/blocks/title-1.vue";
+import { MetaObject } from "@nuxt/schema";
+import type { NuxtError } from "#app";
+import type { FetchResponse } from "ofetch";
 
-/**
- * Put here all the components that you might want to render
- */
-const DEFS = {
+const defs = {
     Title1,
 };
 
+const REDIRECT_CODE = [301, 302, 307, 308];
+
+const html = ref<string>("<!DOCTYPE html><html lang='en'></html>");
+
+/**
+ * Just the raw HTTP query to get the response from Django. If we're on the
+ * server, we're adding the appropriate headers so that the authentication and
+ * other security measures can be passed along (which allows for previews to
+ * work).
+ */
+async function fetchDjangoPage(): Promise<FetchResponse<string>> {
+    const headers: Record<string, string> = {
+        "X-Reach-API": "yes",
+    };
+
+    if (process.server) {
+        const proxyHeaders = useRequestHeaders([
+            "cookie",
+            "origin",
+            "referrer",
+            "x-csrftoken",
+        ]);
+        Object.assign(headers, proxyHeaders);
+
+        const hostCandidates = useRequestHeaders(["host", "x-forwarded-host"]);
+        const host =
+            hostCandidates["x-forwarded-host"] || hostCandidates["host"];
+
+        if (host) {
+            headers["X-Forwarded-Host"] = host;
+        }
+    }
+
+    return await $fetch.raw(useRoute().fullPath, {
+        baseURL: process.browser ? undefined : useNuxtApp().$config.apiUrl,
+        headers,
+        redirect: "manual",
+    });
+}
+
 /**
- * This is the "fall-back" page which will try to fetch and render a page from
- * the underlying Wagtail hosted in the API. Everything here is a sane default,
- * however you might want to customize it depending on your use.
+ * Depending on the response, we'll either return the HTML to be used to render
+ * the page or throw an error:
  *
- * The thing you'll want to customize the most is most likely the defs list!
+ * - If it's a redirect, the error will have the status code of the redirect
+ *   and contain a location in the data field. The goal is that the setup
+ *   function can then navigate to that location.
+ * - Otherwise it's any kind of error and we'll re-throw it from the setup
+ *   function so that the error page is triggered.
  */
-export default defineNuxtComponent({
-    components: {
-        ServerTemplatedComponent,
-    },
+function decideResponseStrategy(resp: FetchResponse<string>) {
+    if (200 <= resp.status && resp.status < 300) {
+        const html = resp._data;
+
+        if (html) {
+            return {
+                html,
+            };
+        } else {
+            throw createError({
+                statusCode: 500,
+                message: "Empty response",
+            });
+        }
+    } else if (REDIRECT_CODE.includes(resp.status)) {
+        const location = resp.headers.get("location");
 
-    /**
-     * This is in charge of getting the HTML from the server.
-     *
-     * Basically we're expecting a 200 status code. If that's the case, the
-     * content should be HTML and we'll work with that.
-     *
-     * If not we try to figure out what is going on. If we've got a redirection
-     * then we translate the redirection into Nuxt. Otherwise we just forward
-     * the error. It's up to the implementer to handle errors 404, 500, etc.
-     *
-     * Let's note that this works slightly different depending on if we're
-     * running on the server side or the client side. Indeed, on the server
-     * you'll have a `$config.apiUrl` value which allows to hit directly the
-     * internal API URL, while on the client this value will be undefined and
-     * we'll hit the URL relatively to the root path using the `x-reach-api`
-     * header to tell the proxy to get this page from the API for us.
-     */
-    async asyncData({ $axios, $config, $router, ssrContext }) {
-        async function getAsyncData($axios, baseURL, path, query) {
-            try {
-                const headers = ssrContext?.event.node.req.headers ?? {};
-                headers["x-reach-api"] = "yes";
-                return {
-                    html: await $axios.$get(path, {
-                        baseURL,
-                        headers,
-                        maxRedirects: 0,
-                        params: query,
-                        validateStatus(status) {
-                            return status === 200;
-                        },
-                    }),
-                };
-            } catch (e) {
-                const { response: res } = e;
-
-                if (res) {
-                    const isRedirect = [301, 302, 307, 308].includes(
-                        res.status
-                    );
-                    const location = res.headers.location;
-
-                    if (isRedirect) {
-                        if (location) {
-                            return await getAsyncData(
-                                $axios,
-                                baseURL,
-                                location,
-                                query
-                            );
-                        } else {
-                            // $sentry.captureException(e);
-                            return createError({
-                                statusCode: res.status,
-                                message: "Invalid redirect",
-                            });
-                        }
-                    } else {
-                        // $sentry.captureException(e);
-                        return createError({
-                            statusCode: res.status,
-                            message: res.statusText,
-                        });
-                    }
-                } else {
-                    // $sentry.captureException(e);
-                    // eslint-disable-next-line
-                    console.error(e);
-                    return createError({
-                        statusCode: 500,
-                        message: "Unknown error",
-                    });
-                }
-            }
+        if (location) {
+            throw createError({
+                statusCode: resp.status,
+                message: "Redirect",
+                data: { location },
+            });
+        } else {
+            throw createError({
+                statusCode: 500,
+                message: "Invalid redirect",
+            });
         }
+    } else {
+        throw createError({
+            statusCode: resp.status,
+            message: resp.statusText,
+        });
+    }
+}
 
-        const route = $router.currentRoute.value;
-        return await getAsyncData(
-            $axios,
-            process.browser ? undefined : $config.apiUrl,
-            route.path,
-            route.query
-        );
-    },
-
-    data() {
-        return {
-            /**
-             * HTML code of the page
-             */
-            html: "",
-
-            /**
-             * Head data extracted from the template's head
-             */
-            headData: {},
-        };
-    },
+/**
+ * This is in charge of getting the HTML from the server.
+ *
+ * Basically we're expecting a 200 status code. If that's the case, the
+ * content should be HTML and we'll work with that.
+ *
+ * If not we try to figure out what is going on. If we've got a redirection
+ * then we translate the redirection into Nuxt. Otherwise we just forward
+ * the error. It's up to the implementer to handle errors 404, 500, etc.
+ *
+ * Let's note that those actions will be decided inside here but the action
+ * will be taken from the setup function because Nuxt is made in a very logical
+ * way apparently.
+ *
+ * Let's note that this works slightly different depending on if we're
+ * running on the server side or the client side. Indeed, on the server
+ * you'll have a `$config.apiUrl` value which allows to hit directly the
+ * internal API URL, while on the client this value will be undefined and
+ * we'll hit the URL relatively to the root path using the `x-reach-api`
+ * header to tell the proxy to get this page from the API for us.
+ */
+async function getServerData() {
+    const resp = await fetchDjangoPage();
+    return decideResponseStrategy(resp);
+}
 
+const {
     /**
-     * Propagates the head data from the template into Nuxt's head system
+     * HTML from the server, if any
      */
-    head() {
-        return this.headData ?? {};
-    },
-
-    computed: {
-        /**
-         * Exposes the defs
-         */
-        defs() {
-            return DEFS;
-        },
-
-        /**
-         * Whether the page is a draft
-         */
-        isPreview() {
-            return this.$route.path.replace(/^\/$/, "").endsWith("/preview");
-        },
-    },
-
-    methods: {
-        /**
-         * This serves to receive updates about the head data extracted by
-         * ServerTemplatedComponent
-         */
-        receiveHeadData(head) {
-            this.headData = head;
-        },
-    },
-});
+    data,
+
+    /**
+     * Error that happened during async fetch, if any
+     */
+    error: fetchError,
+} = await useAsyncData("html", getServerData);
+
+if (fetchError.value) {
+    const error = fetchError.value as any as Error | NuxtError;
+
+    if ("statusCode" in error && REDIRECT_CODE.includes(error.statusCode)) {
+        await navigateTo(error.data.location, {
+            redirectCode: error.statusCode,
+        });
+    } else {
+        throw error;
+    }
+}
+
+if (
+    typeof data.value === "object" &&
+    data.value !== null &&
+    "html" in data.value &&
+    typeof data.value.html === "string"
+) {
+    html.value = data.value.html;
+}
+
+/**
+ * Receiver for the head data from the parsed component, which allows to have
+ * the proper meta info at SSR time.
+ */
+function receiveHeadData(head: MetaObject) {
+    useHead(head);
+}
 </script>
```

### Comparing `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template.py` & `modelw_project_maker-2023.7.0/src/model_w/project_maker/template.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.4.0b1/PKG-INFO` & `modelw_project_maker-2023.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: modelw-project-maker
-Version: 2023.4.0b1
+Version: 2023.7.0
 Summary: A tool to create Model-W-compliant projects
 Home-page: https://github.com/ModelW/project-maker
 License: WTFPL
 Keywords: model-w,django,nuxt,boilerplate,template
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Requires-Dist: Unidecode (>=1.3.4,<2.0.0)
-Requires-Dist: black (>=22.8.0,<23.0.0)
+Requires-Dist: black (>=22,<23)
 Requires-Dist: isort (>=5.10.1,<6.0.0)
 Requires-Dist: monoformat (>=0.1.0b3,<0.2.0)
 Requires-Dist: node-edge (>=0.1.0b2,<0.2.0)
-Requires-Dist: pathspec (>=0.10.2,<0.11.0)
-Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: pathspec (>=0.10,<0.11)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: setuptools
 Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
 Project-URL: Documentation, https://github.com/ModelW/project-maker
 Project-URL: Repository, https://github.com/ModelW/project-maker
 Description-Content-Type: text/markdown
 
 # Model&nbsp;W Project Maker
```


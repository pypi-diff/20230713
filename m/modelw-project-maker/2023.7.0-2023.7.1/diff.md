# Comparing `tmp/modelw_project_maker-2023.7.0.tar.gz` & `tmp/modelw_project_maker-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_project_maker-2023.7.0.tar", max compression
+gzip compressed data, was "modelw_project_maker-2023.7.1.tar", max compression
```

## Comparing `modelw_project_maker-2023.7.0.tar` & `modelw_project_maker-2023.7.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     5377 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/README.md
--rw-r--r--   0        0        0     1355 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/__init__.py
--rw-r--r--   0        0        0     8748 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/__main__.py
--rw-r--r--   0        0        0       45 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/errors.py
--rw-r--r--   0        0        0      143 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/__init__.py
--rw-r--r--   0        0        0     4470 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_api.py
--rw-r--r--   0        0        0     6518 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_base.py
--rw-r--r--   0        0        0      703 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_common.py
--rw-r--r--   0        0        0     3836 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_front.py
--rw-r--r--   0        0        0     3446 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/namer.py
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/py.typed
--rw-r--r--   0        0        0      178 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.editorconfig
--rw-r--r--   0        0        0       27 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.formatignore
--rw-r--r--   0        0        0     3042 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.gitignore
--rw-r--r--   0        0        0       77 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.prettierrc
--rw-r--r--   0        0        0     1488 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/README.md
--rw-r--r--   0        0        0     3034 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/.dockerignore
--rw-r--r--   0        0        0      381 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/.env-template
--rw-r--r--   0        0        0      181 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/Dockerfile
--rw-r--r--   0        0        0      236 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/Makefile
--rw-r--r--   0        0        0     1140 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
--rw-r--r--   0        0        0       93 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
--rw-r--r--   0        0        0     8589 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
--rw-r--r--   0        0        0     2818 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
--rw-r--r--   0        0        0     2036 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
--rw-r--r--   0        0        0      655 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
--rw-r--r--   0        0        0      233 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
--rwxr-xr-x   0        0        0      755 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
--rwxr-xr-x   0        0        0      240 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
--rwxr-xr-x   0        0        0      471 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
--rwxr-xr-x   0        0        0      844 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
--rwxr-xr-x   0        0        0      903 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
--rwxr-xr-x   0        0        0     1092 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
--rwxr-xr-x   0        0        0      658 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
--rwxr-xr-x   0        0        0      718 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
--rwxr-xr-x   0        0        0      485 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
--rwxr-xr-x   0        0        0     2749 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
--rwxr-xr-x   0        0        0     2067 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
--rw-r--r--   0        0        0     1883 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
--rw-r--r--   0        0        0      159 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
--rw-r--r--   0        0        0     3921 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
--rw-r--r--   0        0        0     1343 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
--rw-r--r--   0        0        0     2486 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
--rw-r--r--   0        0        0      194 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
--rw-r--r--   0        0        0      386 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
--rw-r--r--   0        0        0       70 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
--rw-r--r--   0        0        0      851 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
--rw-r--r--   0        0        0      273 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
--rw-r--r--   0        0        0      219 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
--rw-r--r--   0        0        0     2076 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
--rw-r--r--   0        0        0     1681 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
--rw-r--r--   0        0        0      443 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
--rwxr-xr-x   0        0        0      666 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/manage.py
--rwxr-xr-x   0        0        0      151 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/pmanage
--rw-r--r--   0        0        0      861 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/pyproject.toml
--rw-r--r--   0        0        0     3034 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.dockerignore
--rw-r--r--   0        0        0      182 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.env-template
--rw-r--r--   0        0        0      332 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.eslintrc.js
--rw-r--r--   0        0        0        8 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.gitignore
--rw-r--r--   0        0        0       13 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.nvmrc
--rw-r--r--   0        0        0      185 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/Dockerfile
--rw-r--r--   0        0        0     1601 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/README.md
--rw-r--r--   0        0        0      112 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/components/blocks/title-1.vue
--rw-r--r--   0        0        0    11513 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/components/server-templated-component.vue
--rw-r--r--   0        0        0     2941 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/error.vue
--rw-r--r--   0        0        0      558 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/nuxt.config.js
--rw-r--r--   0        0        0      789 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/package.json
--rw-r--r--   0        0        0     5048 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/pages/[...wagtail].vue
--rw-r--r--   0        0        0       80 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
--rw-r--r--   0        0        0      483 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/plugins/dom.client.ts
--rw-r--r--   0        0        0      505 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/plugins/dom.server.ts
--rw-r--r--   0        0        0       98 2023-07-13 09:19:29.960557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/tsconfig.json
--rw-r--r--   0        0        0     7602 2023-07-13 09:19:29.956557 modelw_project_maker-2023.7.0/src/model_w/project_maker/template.py
--rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 modelw_project_maker-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5377 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/README.md
+-rw-r--r--   0        0        0     1355 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/src/model_w/project_maker/__init__.py
+-rw-r--r--   0        0        0     8748 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/src/model_w/project_maker/__main__.py
+-rw-r--r--   0        0        0       45 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/src/model_w/project_maker/errors.py
+-rw-r--r--   0        0        0      143 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/__init__.py
+-rw-r--r--   0        0        0     4470 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_api.py
+-rw-r--r--   0        0        0     6518 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_base.py
+-rw-r--r--   0        0        0      703 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_common.py
+-rw-r--r--   0        0        0     3836 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_front.py
+-rw-r--r--   0        0        0     3446 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/namer.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/py.typed
+-rw-r--r--   0        0        0      178 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.editorconfig
+-rw-r--r--   0        0        0       27 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.formatignore
+-rw-r--r--   0        0        0     3042 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.gitignore
+-rw-r--r--   0        0        0       77 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.prettierrc
+-rw-r--r--   0        0        0     1488 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/README.md
+-rw-r--r--   0        0        0     3034 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/.dockerignore
+-rw-r--r--   0        0        0      381 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/.env-template
+-rw-r--r--   0        0        0      181 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/Dockerfile
+-rw-r--r--   0        0        0      236 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/Makefile
+-rw-r--r--   0        0        0     1140 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
+-rw-r--r--   0        0        0       93 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
+-rw-r--r--   0        0        0     8589 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2818 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
+-rw-r--r--   0        0        0     2036 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
+-rw-r--r--   0        0        0      655 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
+-rw-r--r--   0        0        0      233 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
+-rwxr-xr-x   0        0        0      755 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
+-rwxr-xr-x   0        0        0      240 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
+-rwxr-xr-x   0        0        0      471 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
+-rwxr-xr-x   0        0        0      844 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
+-rwxr-xr-x   0        0        0      903 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
+-rwxr-xr-x   0        0        0     1092 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
+-rwxr-xr-x   0        0        0      658 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
+-rwxr-xr-x   0        0        0      718 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
+-rwxr-xr-x   0        0        0      485 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
+-rwxr-xr-x   0        0        0     2749 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
+-rwxr-xr-x   0        0        0     2067 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
+-rw-r--r--   0        0        0     1883 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
+-rw-r--r--   0        0        0      159 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
+-rw-r--r--   0        0        0     3921 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
+-rw-r--r--   0        0        0     1343 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
+-rw-r--r--   0        0        0     2486 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
+-rw-r--r--   0        0        0      194 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
+-rw-r--r--   0        0        0       70 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
+-rw-r--r--   0        0        0      273 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
+-rw-r--r--   0        0        0      219 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
+-rw-r--r--   0        0        0     2076 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
+-rw-r--r--   0        0        0     1681 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
+-rw-r--r--   0        0        0      443 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
+-rwxr-xr-x   0        0        0      666 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/manage.py
+-rwxr-xr-x   0        0        0      151 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/pmanage
+-rw-r--r--   0        0        0      861 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/pyproject.toml
+-rw-r--r--   0        0        0     3034 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.dockerignore
+-rw-r--r--   0        0        0      182 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.env-template
+-rw-r--r--   0        0        0      332 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.eslintrc.js
+-rw-r--r--   0        0        0        8 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.gitignore
+-rw-r--r--   0        0        0       13 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.nvmrc
+-rw-r--r--   0        0        0      185 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/Dockerfile
+-rw-r--r--   0        0        0     1601 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/README.md
+-rw-r--r--   0        0        0      112 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/components/blocks/title-1.vue
+-rw-r--r--   0        0        0    11513 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/components/server-templated-component.vue
+-rw-r--r--   0        0        0     2941 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/error.vue
+-rw-r--r--   0        0        0      558 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/nuxt.config.js
+-rw-r--r--   0        0        0      789 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/package.json
+-rw-r--r--   0        0        0     5048 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/pages/[...wagtail].vue
+-rw-r--r--   0        0        0       80 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
+-rw-r--r--   0        0        0      483 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/plugins/dom.client.ts
+-rw-r--r--   0        0        0      505 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/plugins/dom.server.ts
+-rw-r--r--   0        0        0       98 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/tsconfig.json
+-rw-r--r--   0        0        0     7602 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template.py
+-rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 modelw_project_maker-2023.7.1/PKG-INFO
```

### Comparing `modelw_project_maker-2023.7.0/README.md` & `modelw_project_maker-2023.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This project maker is the simplest way to start a
 [Model W](https://model-w.readthedocs.io/en/latest/) project.
 
 The goal is to be extremely simple:
 
 ```bash
-curl -s https://pypi.run/modelw-project-maker/model_w.project_maker | python3.10
+curl -s https://pypi.run/modelw-project-maker/model_w.project_maker | python3.11
 ```
 
 This will ask you a few questions and create the project's directory for you.
 
 ## Prerequisites
 
 In order to execute the script, you need:
```

### Comparing `modelw_project_maker-2023.7.0/pyproject.toml` & `modelw_project_maker-2023.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-project-maker"
-version = "2023.7.0"
+version = "2023.7.1"
 packages = [
     {  include = "model_w/project_maker", from = "src" }
 ]
 
 description = "A tool to create Model-W-compliant projects"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
```

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/__main__.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_api.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_api.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_base.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_base.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_common.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_common.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/maker/_front.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_front.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/namer.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/namer.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/.gitignore` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.gitignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/README.md` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/.dockerignore` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/README.md` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/manage.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/manage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/api/pyproject.toml` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/.dockerignore` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/README.md` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/components/server-templated-component.vue` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/components/server-templated-component.vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/error.vue` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/error.vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/nuxt.config.js` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/nuxt.config.js`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/package.json` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/package.json`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template/front/pages/[...wagtail].vue` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/pages/[...wagtail].vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/src/model_w/project_maker/template.py` & `modelw_project_maker-2023.7.1/src/model_w/project_maker/template.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.0/PKG-INFO` & `modelw_project_maker-2023.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-project-maker
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: A tool to create Model-W-compliant projects
 Home-page: https://github.com/ModelW/project-maker
 License: WTFPL
 Keywords: model-w,django,nuxt,boilerplate,template
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.11,<4.0
@@ -33,15 +33,15 @@
 
 This project maker is the simplest way to start a
 [Model W](https://model-w.readthedocs.io/en/latest/) project.
 
 The goal is to be extremely simple:
 
 ```bash
-curl -s https://pypi.run/modelw-project-maker/model_w.project_maker | python3.10
+curl -s https://pypi.run/modelw-project-maker/model_w.project_maker | python3.11
 ```
 
 This will ask you a few questions and create the project's directory for you.
 
 ## Prerequisites
 
 In order to execute the script, you need:
```


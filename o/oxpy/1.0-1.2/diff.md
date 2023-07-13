# Comparing `tmp/oxpy-1.0.tar.gz` & `tmp/oxpy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxpy-1.0.tar", last modified: Thu Jul 13 16:43:11 2023, max compression
+gzip compressed data, was "oxpy-1.2.tar", last modified: Thu Jul 13 16:56:06 2023, max compression
```

## Comparing `oxpy-1.0.tar` & `oxpy-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:43:11.376861 oxpy-1.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 16:37:45.000000 oxpy-1.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 16:37:45.000000 oxpy-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     1258 2023-07-13 16:43:11.376861 oxpy-1.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      837 2023-07-13 16:37:45.000000 oxpy-1.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:43:11.372861 oxpy-1.0/oxo_python/
--rw-------   0 runner    (1000) runner    (1000)     2087 2023-07-13 16:37:45.000000 oxpy-1.0/oxo_python/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:43:11.376861 oxpy-1.0/oxpy.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1258 2023-07-13 16:43:11.000000 oxpy-1.0/oxpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-07-13 16:43:11.000000 oxpy-1.0/oxpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:43:11.000000 oxpy-1.0/oxpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:43:11.000000 oxpy-1.0/oxpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-07-13 16:43:11.000000 oxpy-1.0/oxpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 16:43:11.376861 oxpy-1.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      625 2023-07-13 16:42:58.000000 oxpy-1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:56:06.085288 oxpy-1.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 16:49:36.000000 oxpy-1.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 16:49:36.000000 oxpy-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     1182 2023-07-13 16:56:06.085288 oxpy-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      761 2023-07-13 16:55:11.000000 oxpy-1.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:56:06.081288 oxpy-1.2/oxpy/
+-rw-------   0 runner    (1000) runner    (1000)     2087 2023-07-13 16:49:54.000000 oxpy-1.2/oxpy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:56:06.085288 oxpy-1.2/oxpy.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1182 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      204 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 16:56:06.085288 oxpy-1.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      625 2023-07-13 16:55:27.000000 oxpy-1.2/setup.py
```

### Comparing `oxpy-1.0/LICENSE` & `oxpy-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oxpy-1.0/README.md` & `oxpy-1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 ### Здесь есть функции:
 
-- `upload_file_url(url, expires, secret)`: Загрузка файла через ссылку, url=ссылка, expires=время хранения файла в часах(можно оставить пустым), secret=удлинняет ссылку(можно оставить пустым).
-- `upload_file_path(path, expires, secret)`: Тоже самое что и upload_file_url, только нужно указывать путь к файлу.
-- `delete_file(token, url)`: Удаляет файл, token=токен, url=ссылкана файл в 0x0.
-- `change_expires(url, expires, token)`: Изменяет время хранения файла, token=токен, url=ссылка на файл в 0x0, expires=новое время хранение файла в часах.
+- `upload_file_url`: Загрузка файла через ссылку, url=ссылка, expires=время хранения файла в часах(можно оставить пустым), secret=удлинняет ссылку(можно оставить пустым).
+- `upload_file_path`: Тоже самое что и upload_file_url, только нужно указывать путь к файлу.
+- `delete_file`: Удаляет файл, token=токен, url=ссылкана файл в 0x0.
+- `change_expires()`: Изменяет время хранения файла, token=токен, url=ссылка на файл в 0x0, expires=новое время хранение файла в часах.
```

### Comparing `oxpy-1.0/oxo_python/__init__.py` & `oxpy-1.2/oxpy/__init__.py`

 * *Files identical despite different names*

### Comparing `oxpy-1.0/setup.py` & `oxpy-1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description_md = f.read()
 
 setup(name='oxpy',
-      version='1.0',
+      version='1.2',
       description='Библиотека для взаимодействия с https://0x0.st через Python',
       long_description=long_description_md,
       long_description_content_type='text/markdown',
       author_email='neso_hoshi_official@mail.ru',
       zip_safe=False,
       author='Neso Hiroshi',
       classifiers = [
```


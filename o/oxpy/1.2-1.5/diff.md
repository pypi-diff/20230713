# Comparing `tmp/oxpy-1.2.tar.gz` & `tmp/oxpy-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxpy-1.2.tar", last modified: Thu Jul 13 16:56:06 2023, max compression
+gzip compressed data, was "oxpy-1.5.tar", last modified: Thu Jul 13 17:01:04 2023, max compression
```

## Comparing `oxpy-1.2.tar` & `oxpy-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:56:06.085288 oxpy-1.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 16:49:36.000000 oxpy-1.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 16:49:36.000000 oxpy-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     1182 2023-07-13 16:56:06.085288 oxpy-1.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      761 2023-07-13 16:55:11.000000 oxpy-1.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:56:06.081288 oxpy-1.2/oxpy/
--rw-------   0 runner    (1000) runner    (1000)     2087 2023-07-13 16:49:54.000000 oxpy-1.2/oxpy/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:56:06.085288 oxpy-1.2/oxpy.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1182 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      204 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)        5 2023-07-13 16:56:05.000000 oxpy-1.2/oxpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 16:56:06.085288 oxpy-1.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      625 2023-07-13 16:55:27.000000 oxpy-1.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 17:01:04.963980 oxpy-1.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 16:49:36.000000 oxpy-1.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 16:49:36.000000 oxpy-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     1182 2023-07-13 17:01:04.963980 oxpy-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      761 2023-07-13 16:55:11.000000 oxpy-1.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 17:01:04.963980 oxpy-1.5/oxpy/
+-rw-------   0 runner    (1000) runner    (1000)     2088 2023-07-13 16:59:50.000000 oxpy-1.5/oxpy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 17:01:04.963980 oxpy-1.5/oxpy.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1182 2023-07-13 17:01:04.000000 oxpy-1.5/oxpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      204 2023-07-13 17:01:04.000000 oxpy-1.5/oxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 17:01:04.000000 oxpy-1.5/oxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 17:01:04.000000 oxpy-1.5/oxpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2023-07-13 17:01:04.000000 oxpy-1.5/oxpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 17:01:04.967980 oxpy-1.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      625 2023-07-13 17:00:11.000000 oxpy-1.5/setup.py
```

### Comparing `oxpy-1.2/LICENSE` & `oxpy-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oxpy-1.2/PKG-INFO` & `oxpy-1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,6 @@
-Metadata-Version: 2.1
-Name: oxpy
-Version: 1.2
-Summary: Библиотека для взаимодействия с https://0x0.st через Python
-Author: Neso Hiroshi
-Author-email: neso_hoshi_official@mail.ru
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### Здесь есть функции:
 
 - `upload_file_url`: Загрузка файла через ссылку, url=ссылка, expires=время хранения файла в часах(можно оставить пустым), secret=удлинняет ссылку(можно оставить пустым).
 - `upload_file_path`: Тоже самое что и upload_file_url, только нужно указывать путь к файлу.
 - `delete_file`: Удаляет файл, token=токен, url=ссылкана файл в 0x0.
-- `change_expires()`: Изменяет время хранения файла, token=токен, url=ссылка на файл в 0x0, expires=новое время хранение файла в часах.
+- `change_expires()`: Изменяет время хранения файла, token=токен, url=ссылка на файл в 0x0, expires=новое время хранение файла в часах.
```

### Comparing `oxpy-1.2/oxpy/__init__.py` & `oxpy-1.5/oxpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,13 +39,13 @@
             command = f"curl -F'file={path}' https://0x0.st"
         else:
             command = f"curl -F'file={path}' -Fsecret=https://0x0.st"
     else:
         if secret == None:
             command = f"curl -F'file={path}' -Fexpires={expires} https://0x0.st"
         else:
-            command = f"curl -F'file={path' -Fexpires={expires} -Fsecret=https://0x0.st"
+            command = f"curl -F'file={path}' -Fexpires={expires} -Fsecret=https://0x0.st"
     try:
         output = subprocess.check_output(command, shell=True)
         return output.decode().strip()
     except subprocess.CalledProcessError as e:
         return f"Ошибка при загрузке файла:\n {e}"
```

### Comparing `oxpy-1.2/oxpy.egg-info/PKG-INFO` & `oxpy-1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxpy
-Version: 1.2
+Version: 1.5
 Summary: Библиотека для взаимодействия с https://0x0.st через Python
 Author: Neso Hiroshi
 Author-email: neso_hoshi_official@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `oxpy-1.2/setup.py` & `oxpy-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description_md = f.read()
 
 setup(name='oxpy',
-      version='1.2',
+      version='1.5',
       description='Библиотека для взаимодействия с https://0x0.st через Python',
       long_description=long_description_md,
       long_description_content_type='text/markdown',
       author_email='neso_hoshi_official@mail.ru',
       zip_safe=False,
       author='Neso Hiroshi',
       classifiers = [
```


# Comparing `tmp/0x0-python-0.1.tar.gz` & `tmp/0x0-python-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "0x0-python-0.1.tar", last modified: Thu Jul 13 15:46:03 2023, max compression
+gzip compressed data, was "0x0-python-0.2.tar", last modified: Thu Jul 13 16:14:06 2023, max compression
```

## Comparing `0x0-python-0.1.tar` & `0x0-python-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 15:46:03.326890 0x0-python-0.1/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 15:46:03.326890 0x0-python-0.1/0x0_python.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      843 2023-07-13 15:46:02.000000 0x0-python-0.1/0x0_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      217 2023-07-13 15:46:02.000000 0x0-python-0.1/0x0_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 15:46:02.000000 0x0-python-0.1/0x0_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 15:46:02.000000 0x0-python-0.1/0x0_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 15:46:02.000000 0x0-python-0.1/0x0_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 15:42:20.000000 0x0-python-0.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 15:42:20.000000 0x0-python-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)      843 2023-07-13 15:46:03.326890 0x0-python-0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-13 15:44:26.000000 0x0-python-0.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 15:46:03.326890 0x0-python-0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      768 2023-07-13 15:42:20.000000 0x0-python-0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:14:06.041328 0x0-python-0.2/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-13 16:14:06.041328 0x0-python-0.2/0x0_python.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      873 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      217 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-13 16:14:05.000000 0x0-python-0.2/0x0_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-13 15:42:20.000000 0x0-python-0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-13 15:42:20.000000 0x0-python-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)      873 2023-07-13 16:14:06.045328 0x0-python-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-07-13 16:09:38.000000 0x0-python-0.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-13 16:14:06.045328 0x0-python-0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      768 2023-07-13 16:12:58.000000 0x0-python-0.2/setup.py
```

### Comparing `0x0-python-0.1/0x0_python.egg-info/PKG-INFO` & `0x0-python-0.2/0x0_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: 0x0-python
-Version: 0.1
+Version: 0.2
 Summary: Библиотека для взаимодействия с 0x0 point через питон
 Author: Neso Hiroshi
 Author-email: neso_hoshi_official@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1>Ntcn jgbcfybz</h1>
-<p>Здесь есть функции:\n
-- <code>loading(delay)</code>: Прогрессбар. Вместо <code>delay</code> введите задержку.
-- <code>test(text)</code>: Можно оставить аргумент пустым или ввести текст.
-- <code>collatz(number)</code>: Теория 3N + 1. Вместо <code>number</code> введите число.</p>
+<p>Здесь есть функции:</p>
+<ul>
+<li><code>loading(delay)</code>: Прогрессбар. Вместо <code>delay</code> введите задержку.</li>
+<li><code>test(text)</code>: Можно оставить аргумент пустым или ввести текст.</li>
+<li><code>collatz(number)</code>: Теория 3N + 1. Вместо <code>number</code> введите число.</li>
+</ul>
```

### Comparing `0x0-python-0.1/LICENSE` & `0x0-python-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `0x0-python-0.1/PKG-INFO` & `0x0-python-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: 0x0-python
-Version: 0.1
+Version: 0.2
 Summary: Библиотека для взаимодействия с 0x0 point через питон
 Author: Neso Hiroshi
 Author-email: neso_hoshi_official@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1>Ntcn jgbcfybz</h1>
-<p>Здесь есть функции:\n
-- <code>loading(delay)</code>: Прогрессбар. Вместо <code>delay</code> введите задержку.
-- <code>test(text)</code>: Можно оставить аргумент пустым или ввести текст.
-- <code>collatz(number)</code>: Теория 3N + 1. Вместо <code>number</code> введите число.</p>
+<p>Здесь есть функции:</p>
+<ul>
+<li><code>loading(delay)</code>: Прогрессбар. Вместо <code>delay</code> введите задержку.</li>
+<li><code>test(text)</code>: Можно оставить аргумент пустым или ввести текст.</li>
+<li><code>collatz(number)</code>: Теория 3N + 1. Вместо <code>number</code> введите число.</li>
+</ul>
```

### Comparing `0x0-python-0.1/setup.py` & `0x0-python-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from markdown import markdown
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description_md = f.read()
     long_description_html = markdown(long_description_md, extensions=['markdown.extensions.fenced_code'])
 
 setup(name='0x0-python',
-      version='0.1',
+      version='0.2',
       description='Библиотека для взаимодействия с 0x0 point через питон',
       long_description=long_description_html,
       long_description_content_type='text/markdown',
       author_email='neso_hoshi_official@mail.ru',
       zip_safe=False,
       author='Neso Hiroshi',
       classifiers = [
```


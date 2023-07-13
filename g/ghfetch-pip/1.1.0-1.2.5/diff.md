# Comparing `tmp/ghfetch-pip-1.1.0.tar.gz` & `tmp/ghfetch-pip-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghfetch-pip-1.1.0.tar", last modified: Wed Jul 12 22:41:52 2023, max compression
+gzip compressed data, was "ghfetch-pip-1.2.5.tar", last modified: Thu Jul 13 20:57:29 2023, max compression
```

## Comparing `ghfetch-pip-1.1.0.tar` & `ghfetch-pip-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-12 22:41:52.036771 ghfetch-pip-1.1.0/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1071 2023-07-08 19:18:11.000000 ghfetch-pip-1.1.0/LICENSE
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-12 22:41:52.036771 ghfetch-pip-1.1.0/PKG-INFO
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1242 2023-07-12 22:28:59.000000 ghfetch-pip-1.1.0/README.md
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-12 22:41:52.036771 ghfetch-pip-1.1.0/ghfetch/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-12 22:28:59.000000 ghfetch-pip-1.1.0/ghfetch/__init__.py
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    10584 2023-07-12 22:28:59.000000 ghfetch-pip-1.1.0/ghfetch/main.py
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-12 22:41:52.036771 ghfetch-pip-1.1.0/ghfetch_pip.egg-info/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-12 22:41:51.000000 ghfetch-pip-1.1.0/ghfetch_pip.egg-info/PKG-INFO
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      284 2023-07-12 22:41:51.000000 ghfetch-pip-1.1.0/ghfetch_pip.egg-info/SOURCES.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        1 2023-07-12 22:41:51.000000 ghfetch-pip-1.1.0/ghfetch_pip.egg-info/dependency_links.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       46 2023-07-12 22:41:51.000000 ghfetch-pip-1.1.0/ghfetch_pip.egg-info/entry_points.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       20 2023-07-12 22:41:51.000000 ghfetch-pip-1.1.0/ghfetch_pip.egg-info/requires.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        8 2023-07-12 22:41:51.000000 ghfetch-pip-1.1.0/ghfetch_pip.egg-info/top_level.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      219 2023-07-12 22:41:52.036771 ghfetch-pip-1.1.0/setup.cfg
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      483 2023-07-12 22:41:36.000000 ghfetch-pip-1.1.0/setup.py
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1071 2023-07-08 19:18:11.000000 ghfetch-pip-1.2.5/LICENSE
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/PKG-INFO
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1242 2023-07-13 20:55:47.000000 ghfetch-pip-1.2.5/README.md
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/ghfetch/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:55:47.000000 ghfetch-pip-1.2.5/ghfetch/__init__.py
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    10585 2023-07-13 20:55:59.000000 ghfetch-pip-1.2.5/ghfetch/main.py
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/PKG-INFO
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      284 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        1 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       46 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/entry_points.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       20 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/requires.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        8 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/top_level.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      219 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/setup.cfg
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      483 2023-07-13 20:55:59.000000 ghfetch-pip-1.2.5/setup.py
```

### Comparing `ghfetch-pip-1.1.0/LICENSE` & `ghfetch-pip-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ghfetch-pip-1.1.0/README.md` & `ghfetch-pip-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ghfetch-pip-1.1.0/ghfetch/main.py` & `ghfetch-pip-1.2.5/ghfetch/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 
 # requirements
 import asyncio
 import aiohttp
 from rich import print
 from PIL import Image
 
+HOME_PATH = Path().home()
 THIS_PATH = Path(__file__).parent.resolve()
 
+def startup():
+    tmp_folder = Path(f'{HOME_PATH}/.ghfetch/tmp')
+
+    Path(tmp_folder).mkdir(parents=True, exist_ok=True)
+
 async def api_call(is_repo, name):
     BASE_URL = 'https://api.github.com/'
     ENDPOINT_URL = 'repos/' if is_repo else 'users/'
 
     URL = f'{BASE_URL}{ENDPOINT_URL}{name}'
 
     async with aiohttp.request('GET', URL) as res:
@@ -51,18 +57,14 @@
         'stars': info['stargazers_count'],
         'watchers': info['watchers_count'],
         'forks': info['forks_count'],
         'archived': info['archived'],
         **({'license': info['license']['name']} if info['license'] is not None else {'license': None}),
         **({'forked_parent': info['parent']['html_url']} if info['fork'] else {}),
         'languages': asyncio.run(create_languages_stat(info['languages_url'])),
-        # 'size': info['size'],
-        # 'issues': info['open_issues_count'],
-
-        # TODO: Languages: like colors in neofetch, with colors and icons, max 4 lines of height
     }
 
 def fetch_user(info):
     return {'company': info['company'],}
 
 def fetch_main(name):
     is_repo = '/' in name
@@ -104,15 +106,15 @@
 
 def image_to_unicode(url):
     IMAGE_WIDTH = 35
     COLORED_CHAR_LENGTH = 20 # Number of characters needed in raw to print a colored unicode character [#012345]█[/#012345]
     UNICODE_BLOCK_CHAR = '\u2588'
 
     file_name = url.split('/')[-1].split('?')[0]
-    user_img_location = Path(f'{THIS_PATH}/{file_name}.png')
+    user_img_location = Path(f'{HOME_PATH}/.ghfetch/tmp/{file_name}.png')
 
     img_data = requests.get(url).content
 
     with open(user_img_location, 'wb') as file:
         file.write(img_data)
 
     with Image.open(user_img_location) as image:
@@ -220,14 +222,16 @@
             output[n + 12] += ', '.join([(f"{title(k)}: {text(v)}") for k, v in fetched_info["languages"].items()])
 
     for line in output:
         print(line)
 
 
 def main():
+    startup()
+
     if len(sys.argv) != 2:
         return print('Only one argument must be provided')
 
     name = sys.argv[1]
 
     # API call
     fetched_info = fetch_main(name)
```


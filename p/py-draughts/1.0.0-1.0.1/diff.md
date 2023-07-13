# Comparing `tmp/py-draughts-1.0.0.tar.gz` & `tmp/py-draughts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.0.0.tar", last modified: Thu Jul 13 16:45:23 2023, max compression
+gzip compressed data, was "py-draughts-1.0.1.tar", last modified: Thu Jul 13 16:53:48 2023, max compression
```

## Comparing `py-draughts-1.0.0.tar` & `py-draughts-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.102384 py-draughts-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6155 2023-07-13 16:45:23.101383 py-draughts-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4756 2023-07-13 16:44:41.000000 py-draughts-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.050384 py-draughts-1.0.0/draughts/
--rw-rw-rw-   0        0        0      945 2023-07-13 16:45:05.000000 py-draughts-1.0.0/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-12 12:15:32.000000 py-draughts-1.0.0/draughts/american.py
--rw-rw-rw-   0        0        0    10865 2023-07-13 09:58:48.000000 py-draughts-1.0.0/draughts/base.py
--rw-rw-rw-   0        0        0      674 2023-07-11 19:49:33.000000 py-draughts-1.0.0/draughts/models.py
--rw-rw-rw-   0        0        0     4195 2023-07-13 09:58:48.000000 py-draughts-1.0.0/draughts/move.py
--rw-rw-rw-   0        0        0     5193 2023-07-13 16:38:38.000000 py-draughts-1.0.0/draughts/server.py
--rw-rw-rw-   0        0        0     5989 2023-07-12 12:15:34.000000 py-draughts-1.0.0/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:22.999384 py-draughts-1.0.0/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.054384 py-draughts-1.0.0/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.0/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.060385 py-draughts-1.0.0/draughts/static/js/
--rw-rw-rw-   0        0        0     5669 2023-07-13 16:39:11.000000 py-draughts-1.0.0/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.069384 py-draughts-1.0.0/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.0/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2705 2023-07-13 16:36:29.000000 py-draughts-1.0.0/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.0/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.086385 py-draughts-1.0.0/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6155 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 16:45:23.102384 py-draughts-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.097383 py-draughts-1.0.0/test/
--rw-rw-rw-   0        0        0     1123 2023-07-11 18:56:31.000000 py-draughts-1.0.0/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-11 18:56:31.000000 py-draughts-1.0.0/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:48.006384 py-draughts-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6317 2023-07-13 16:53:48.004394 py-draughts-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4899 2023-07-13 16:53:22.000000 py-draughts-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.958394 py-draughts-1.0.1/draughts/
+-rw-rw-rw-   0        0        0      964 2023-07-13 16:53:32.000000 py-draughts-1.0.1/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-12 12:15:32.000000 py-draughts-1.0.1/draughts/american.py
+-rw-rw-rw-   0        0        0    10865 2023-07-13 09:58:48.000000 py-draughts-1.0.1/draughts/base.py
+-rw-rw-rw-   0        0        0      674 2023-07-11 19:49:33.000000 py-draughts-1.0.1/draughts/models.py
+-rw-rw-rw-   0        0        0     4195 2023-07-13 09:58:48.000000 py-draughts-1.0.1/draughts/move.py
+-rw-rw-rw-   0        0        0     5193 2023-07-13 16:38:38.000000 py-draughts-1.0.1/draughts/server.py
+-rw-rw-rw-   0        0        0     5989 2023-07-12 12:15:34.000000 py-draughts-1.0.1/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.884385 py-draughts-1.0.1/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.965391 py-draughts-1.0.1/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.1/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.969391 py-draughts-1.0.1/draughts/static/js/
+-rw-rw-rw-   0        0        0     5669 2023-07-13 16:39:11.000000 py-draughts-1.0.1/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.978386 py-draughts-1.0.1/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.1/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2705 2023-07-13 16:36:29.000000 py-draughts-1.0.1/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.1/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.994388 py-draughts-1.0.1/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6317 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:53:48.007387 py-draughts-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:53:48.002389 py-draughts-1.0.1/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-11 18:56:31.000000 py-draughts-1.0.1/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-11 18:56:31.000000 py-draughts-1.0.1/test/test_board.py
```

### Comparing `py-draughts-1.0.0/LICENSE` & `py-draughts-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/PKG-INFO` & `py-draughts-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.0
-Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
+Version: 1.0.1
+Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
@@ -136,14 +136,18 @@
  . w . w . w . w
  w . w . w . w .
 ```
 
 
 ## UI
 
+1. Allows to play against AI.
+2. Allows to play vs another player. (on the same computer)
+3. Allows to test and find bugs in your engine.
+
 ```python
 from draughts.server import Server
 Server().run()
 ```
 
 #### Use for testing your engine.
```

### Comparing `py-draughts-1.0.0/README.md` & `py-draughts-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,18 @@
  . w . w . w . w
  w . w . w . w .
 ```
 
 
 ## UI
 
+1. Allows to play against AI.
+2. Allows to play vs another player. (on the same computer)
+3. Allows to test and find bugs in your engine.
+
 ```python
 from draughts.server import Server
 Server().run()
 ```
 
 #### Use for testing your engine.
```

### Comparing `py-draughts-1.0.0/draughts/__init__.py` & `py-draughts-1.0.1/draughts/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
-A draughts library for Python, with move generation and validation,
-PDN parsing and writing. Supprots multiple variants of game.
+A draughts library with advenced (customizable) WEB UI move generation and validation,
+PDN parsing and writing. Supports multiple variants of game.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-1.0.0/draughts/american.py` & `py-draughts-1.0.1/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/base.py` & `py-draughts-1.0.1/draughts/base.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/models.py` & `py-draughts-1.0.1/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/move.py` & `py-draughts-1.0.1/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/server.py` & `py-draughts-1.0.1/draughts/server.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/standard.py` & `py-draughts-1.0.1/draughts/standard.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/static/css/style.css` & `py-draughts-1.0.1/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/static/js/script.js` & `py-draughts-1.0.1/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/templates/base.html` & `py-draughts-1.0.1/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/templates/index.html` & `py-draughts-1.0.1/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/draughts/utils.py` & `py-draughts-1.0.1/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.0.1/py_draughts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.0
-Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
+Version: 1.0.1
+Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
@@ -136,14 +136,18 @@
  . w . w . w . w
  w . w . w . w .
 ```
 
 
 ## UI
 
+1. Allows to play against AI.
+2. Allows to play vs another player. (on the same computer)
+3. Allows to test and find bugs in your engine.
+
 ```python
 from draughts.server import Server
 Server().run()
 ```
 
 #### Use for testing your engine.
```

### Comparing `py-draughts-1.0.0/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.0.1/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/setup.py` & `py-draughts-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/test/test_american_board.py` & `py-draughts-1.0.1/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.0/test/test_board.py` & `py-draughts-1.0.1/test/test_board.py`

 * *Files identical despite different names*


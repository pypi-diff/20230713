# Comparing `tmp/py-draughts-1.0.2.tar.gz` & `tmp/py-draughts-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.0.2.tar", last modified: Thu Jul 13 18:26:17 2023, max compression
+gzip compressed data, was "py-draughts-1.0.3.tar", last modified: Thu Jul 13 19:34:38 2023, max compression
```

## Comparing `py-draughts-1.0.2.tar` & `py-draughts-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:17.032570 py-draughts-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6266 2023-07-13 18:26:17.028560 py-draughts-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4848 2023-07-13 18:25:28.000000 py-draughts-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.955914 py-draughts-1.0.2/draughts/
--rw-rw-rw-   0        0        0      964 2023-07-13 18:26:14.000000 py-draughts-1.0.2/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-13 18:02:36.000000 py-draughts-1.0.2/draughts/american.py
--rw-rw-rw-   0        0        0    11185 2023-07-13 18:19:05.000000 py-draughts-1.0.2/draughts/base.py
--rw-rw-rw-   0        0        0      671 2023-07-13 17:34:05.000000 py-draughts-1.0.2/draughts/models.py
--rw-rw-rw-   0        0        0     4197 2023-07-13 18:10:29.000000 py-draughts-1.0.2/draughts/move.py
--rw-rw-rw-   0        0        0     5331 2023-07-13 18:14:29.000000 py-draughts-1.0.2/draughts/server.py
--rw-rw-rw-   0        0        0     5989 2023-07-13 18:10:31.000000 py-draughts-1.0.2/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.911909 py-draughts-1.0.2/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.962557 py-draughts-1.0.2/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.2/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.967592 py-draughts-1.0.2/draughts/static/js/
--rw-rw-rw-   0        0        0     5993 2023-07-13 18:16:53.000000 py-draughts-1.0.2/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.976563 py-draughts-1.0.2/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.2/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2860 2023-07-13 18:13:53.000000 py-draughts-1.0.2/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.2/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:17.003562 py-draughts-1.0.2/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6266 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 18:26:17.032570 py-draughts-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:26:17.021561 py-draughts-1.0.2/test/
--rw-rw-rw-   0        0        0     1123 2023-07-13 17:33:45.000000 py-draughts-1.0.2/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-13 17:33:45.000000 py-draughts-1.0.2/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.927326 py-draughts-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6266 2023-07-13 19:34:38.926325 py-draughts-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4848 2023-07-13 18:25:28.000000 py-draughts-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.890324 py-draughts-1.0.3/draughts/
+-rw-rw-rw-   0        0        0      964 2023-07-13 19:34:17.000000 py-draughts-1.0.3/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-13 18:02:36.000000 py-draughts-1.0.3/draughts/american.py
+-rw-rw-rw-   0        0        0    11486 2023-07-13 19:30:01.000000 py-draughts-1.0.3/draughts/base.py
+-rw-rw-rw-   0        0        0      671 2023-07-13 17:34:05.000000 py-draughts-1.0.3/draughts/models.py
+-rw-rw-rw-   0        0        0     4197 2023-07-13 18:10:29.000000 py-draughts-1.0.3/draughts/move.py
+-rw-rw-rw-   0        0        0     5323 2023-07-13 19:34:18.000000 py-draughts-1.0.3/draughts/server.py
+-rw-rw-rw-   0        0        0     5989 2023-07-13 18:10:31.000000 py-draughts-1.0.3/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.837328 py-draughts-1.0.3/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.893324 py-draughts-1.0.3/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.3/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.896323 py-draughts-1.0.3/draughts/static/js/
+-rw-rw-rw-   0        0        0     5993 2023-07-13 18:16:53.000000 py-draughts-1.0.3/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.904328 py-draughts-1.0.3/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.3/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2860 2023-07-13 18:13:53.000000 py-draughts-1.0.3/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.3/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.918327 py-draughts-1.0.3/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6266 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 19:34:38.928325 py-draughts-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.925324 py-draughts-1.0.3/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-13 17:33:45.000000 py-draughts-1.0.3/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-13 17:33:45.000000 py-draughts-1.0.3/test/test_board.py
```

### Comparing `py-draughts-1.0.2/LICENSE` & `py-draughts-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/PKG-INFO` & `py-draughts-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.2
+Version: 1.0.3
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
```

### Comparing `py-draughts-1.0.2/README.md` & `py-draughts-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/__init__.py` & `py-draughts-1.0.3/draughts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-1.0.2/draughts/american.py` & `py-draughts-1.0.3/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/base.py` & `py-draughts-1.0.3/draughts/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,16 +124,24 @@
 
     @property
     def position(self) -> np.ndarray:
         """Returns board position."""
         return self._pos
 
     @property
-    def is_game_over(self) -> bool:
+    def game_over(self) -> bool:
         """Returns ``True`` if the game is over."""
+        # check if threefold repetition
+        if len(self._moves_stack) >= 8:
+            if (
+                self._moves_stack[-1].square_list
+                == self._moves_stack[-5].square_list
+                == self._moves_stack[-9].square_list
+            ):
+                return True
         return not bool(list(self.legal_moves))
 
     def push(self, move: Move, is_finished: bool = True) -> None:
         """Pushes a move to the board.
         Automatically promotes a piece if it reaches the last row.
 
         If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
```

### Comparing `py-draughts-1.0.2/draughts/models.py` & `py-draughts-1.0.3/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/move.py` & `py-draughts-1.0.3/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/server.py` & `py-draughts-1.0.3/draughts/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import uvicorn
-from fastapi import FastAPI, Request, APIRouter
+from fastapi import FastAPI, Request, APIRouter, BackgroundTasks
 from fastapi.responses import RedirectResponse
 import json
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from draughts import __version__
 from draughts.base import BaseBoard, Color
 from typing import Literal
@@ -113,15 +113,14 @@
     def get_best_move(self, request: Request) -> PositionResponse:
         move = self.get_best_move_method(self.board)
         self.board.push(move)
         return self.position_json
 
     def move(self, request: Request, source: str, target: str) -> PositionResponse:
         move_str = f"{source}-{target}"
-        print(move_str)
         self.board.push_from_str(move_str)
         return self.position_json
 
     def pop(self, request: Request) -> PositionResponse:
         self.board.pop()
         return self.position_json
```

### Comparing `py-draughts-1.0.2/draughts/standard.py` & `py-draughts-1.0.3/draughts/standard.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/static/css/style.css` & `py-draughts-1.0.3/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/static/js/script.js` & `py-draughts-1.0.3/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/templates/base.html` & `py-draughts-1.0.3/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/templates/index.html` & `py-draughts-1.0.3/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/draughts/utils.py` & `py-draughts-1.0.3/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.0.3/py_draughts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.2
+Version: 1.0.3
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
```

### Comparing `py-draughts-1.0.2/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.0.3/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/setup.py` & `py-draughts-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/test/test_american_board.py` & `py-draughts-1.0.3/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.2/test/test_board.py` & `py-draughts-1.0.3/test/test_board.py`

 * *Files identical despite different names*


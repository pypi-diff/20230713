# Comparing `tmp/py-draughts-0.9.9.tar.gz` & `tmp/py-draughts-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-0.9.9.tar", last modified: Wed Jul 12 10:11:51 2023, max compression
+gzip compressed data, was "py-draughts-1.0.0.tar", last modified: Thu Jul 13 16:45:23 2023, max compression
```

## Comparing `py-draughts-0.9.9.tar` & `py-draughts-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.412134 py-draughts-0.9.9/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-0.9.9/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-11 18:05:22.000000 py-draughts-0.9.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6079 2023-07-12 10:11:51.411135 py-draughts-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     4678 2023-07-12 10:10:58.000000 py-draughts-0.9.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.375137 py-draughts-0.9.9/draughts/
--rw-rw-rw-   0        0        0      945 2023-07-12 10:11:28.000000 py-draughts-0.9.9/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-11 16:12:53.000000 py-draughts-0.9.9/draughts/american.py
--rw-rw-rw-   0        0        0    10939 2023-07-12 10:06:21.000000 py-draughts-0.9.9/draughts/base.py
--rw-rw-rw-   0        0        0      674 2023-07-12 09:24:29.000000 py-draughts-0.9.9/draughts/models.py
--rw-rw-rw-   0        0        0     4191 2023-07-11 17:16:02.000000 py-draughts-0.9.9/draughts/move.py
--rw-rw-rw-   0        0        0     5221 2023-07-12 10:03:55.000000 py-draughts-0.9.9/draughts/server.py
--rw-rw-rw-   0        0        0     5989 2023-07-12 09:53:36.000000 py-draughts-0.9.9/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.334145 py-draughts-0.9.9/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.377135 py-draughts-0.9.9/draughts/static/css/
--rw-rw-rw-   0        0        0     2782 2023-07-12 09:24:29.000000 py-draughts-0.9.9/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.378138 py-draughts-0.9.9/draughts/static/js/
--rw-rw-rw-   0        0        0     5824 2023-07-11 15:13:38.000000 py-draughts-0.9.9/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.381136 py-draughts-0.9.9/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-0.9.9/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2500 2023-07-11 13:56:11.000000 py-draughts-0.9.9/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 13:47:51.000000 py-draughts-0.9.9/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.397138 py-draughts-0.9.9/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6079 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-0.9.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 10:11:51.412134 py-draughts-0.9.9/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-07-11 17:45:47.000000 py-draughts-0.9.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.410136 py-draughts-0.9.9/test/
--rw-rw-rw-   0        0        0     1123 2023-07-11 16:12:53.000000 py-draughts-0.9.9/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-11 16:12:53.000000 py-draughts-0.9.9/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.102384 py-draughts-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6155 2023-07-13 16:45:23.101383 py-draughts-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4756 2023-07-13 16:44:41.000000 py-draughts-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.050384 py-draughts-1.0.0/draughts/
+-rw-rw-rw-   0        0        0      945 2023-07-13 16:45:05.000000 py-draughts-1.0.0/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-12 12:15:32.000000 py-draughts-1.0.0/draughts/american.py
+-rw-rw-rw-   0        0        0    10865 2023-07-13 09:58:48.000000 py-draughts-1.0.0/draughts/base.py
+-rw-rw-rw-   0        0        0      674 2023-07-11 19:49:33.000000 py-draughts-1.0.0/draughts/models.py
+-rw-rw-rw-   0        0        0     4195 2023-07-13 09:58:48.000000 py-draughts-1.0.0/draughts/move.py
+-rw-rw-rw-   0        0        0     5193 2023-07-13 16:38:38.000000 py-draughts-1.0.0/draughts/server.py
+-rw-rw-rw-   0        0        0     5989 2023-07-12 12:15:34.000000 py-draughts-1.0.0/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:22.999384 py-draughts-1.0.0/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.054384 py-draughts-1.0.0/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.0/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.060385 py-draughts-1.0.0/draughts/static/js/
+-rw-rw-rw-   0        0        0     5669 2023-07-13 16:39:11.000000 py-draughts-1.0.0/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.069384 py-draughts-1.0.0/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.0/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2705 2023-07-13 16:36:29.000000 py-draughts-1.0.0/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.0/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.086385 py-draughts-1.0.0/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6155 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 16:45:22.000000 py-draughts-1.0.0/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:45:23.102384 py-draughts-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:45:23.097383 py-draughts-1.0.0/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-11 18:56:31.000000 py-draughts-1.0.0/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-11 18:56:31.000000 py-draughts-1.0.0/test/test_board.py
```

### Comparing `py-draughts-0.9.9/LICENSE` & `py-draughts-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/PKG-INFO` & `py-draughts-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 0.9.9
+Version: 1.0.0
 Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -156,23 +156,27 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a5e2ca89-28e1-4dcc-96ae-b18fc602c9bc" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5712f27f-b3fd-44e5-9f6e-08e32b9eddd2" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b14523ea-4bc4-45e1-b5c0-5deea3ed5328" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4de34033-fff5-41e8-a8d8-b1b1ff399149" width="800" />
 
-*Legal moves for selected square (on image "16")*
+*Legal moves for selected square (on image "11")*
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/c8245cbc-06ec-4623-81ab-c9aaa9302627" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5f9c0b41-6bce-4c1d-ac47-042a9e28f61e" width="800" />
 
 
+### testing best moves finding methods:
+
+[Example](examples/engine.py)
+
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
 
 1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
```

### Comparing `py-draughts-0.9.9/README.md` & `py-draughts-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -127,28 +127,32 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a5e2ca89-28e1-4dcc-96ae-b18fc602c9bc" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5712f27f-b3fd-44e5-9f6e-08e32b9eddd2" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b14523ea-4bc4-45e1-b5c0-5deea3ed5328" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4de34033-fff5-41e8-a8d8-b1b1ff399149" width="800" />
 
-*Legal moves for selected square (on image "16")*
+*Legal moves for selected square (on image "11")*
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/c8245cbc-06ec-4623-81ab-c9aaa9302627" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5f9c0b41-6bce-4c1d-ac47-042a9e28f61e" width="800" />
 
 
+### testing best moves finding methods:
+
+[Example](examples/engine.py)
+
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
 
 1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
 2. [Rules and variants](https://en.wikipedia.org/wiki/Checkers)
 3. [List of PDNs](https://github.com/mig0/Games-Checkers/)
 4. [Draughts online](https://lidraughts.org/)
 5. [Additional 1 (Checkers online)](https://checkers.online/play)
-6. [Additional 2 (Chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
+6. [Additional 2 (Chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
```

### Comparing `py-draughts-0.9.9/draughts/__init__.py` & `py-draughts-1.0.0/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A draughts library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
-__version__ = "0.9.9"
+__version__ = "1.0.0"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-0.9.9/draughts/american.py` & `py-draughts-1.0.0/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/draughts/base.py` & `py-draughts-1.0.0/draughts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,14 @@
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         # is promotion
         if (tg // (self.shape[0] // 2)) in (0, self.shape[0] - 1) and abs(
             self._pos[tg]
         ) == 1:
             self._pos[tg] *= Entity.KING.value
             move.is_promotion = True
-            logger.warning(f"Kinged: {tg} on row {tg // self.shape[0]}")
         if move.captured_list:
             self._pos[np.array([sq for sq in move.captured_list])] = Entity.EMPTY
         self._moves_stack.append(move)
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
 
     def pop(self, is_finished=True) -> None:
```

### Comparing `py-draughts-0.9.9/draughts/models.py` & `py-draughts-1.0.0/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/draughts/move.py` & `py-draughts-1.0.0/draughts/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             )
 
             return all(square in longer for square in shorter)
 
         return False
 
     def __len__(self) -> int:
-        return len(self.square_list)
+        return len(self.square_list) + 1
 
     def __add__(self, other: Move) -> Move:
         """Append moves"""
         if self.square_list[-1] != other.square_list[0]:
             raise ValueError(
                 f"Cannot append moves {self} and {other}. Last square of first move should be equal to first square of second move."
             )
```

### Comparing `py-draughts-0.9.9/draughts/server.py` & `py-draughts-1.0.0/draughts/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,132 +2,142 @@
 import uvicorn
 from fastapi import FastAPI, Request, APIRouter
 from fastapi.responses import RedirectResponse
 import json
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from draughts import __version__
-from draughts.standard import Board
+from draughts.base import BaseBoard, Color
 from typing import Literal
 from collections import defaultdict
 from pathlib import Path
+from pydantic import BaseModel, Field
+from draughts.standard import Board
+
+
+class PositionResponse(BaseModel):
+    position: list = Field(description="Current board position")
+    history: list = Field(description="History of moves")
+    turn: Literal["white", "black"] = Field(description="Current turn")
 
 
 class Server:
+    APP = FastAPI(title="py-draughts", version=__version__)
+    static_dir = Path(__file__).parent / "static"
+    APP.mount("/static", StaticFiles(directory=static_dir), name="static")
+    templates_dir = Path(__file__).parent / "templates"
+    templates = Jinja2Templates(directory=templates_dir)
+
     def __init__(
         self,
-        board=Board(),
+        board: BaseBoard = Board(),
         get_best_move_method: callable = None,
-        draw_board=True,
-        populate_board=True,
-        show_pseudo_legal_moves=True,
     ):
-        self.app = FastAPI(title="py-draughts", version=__version__)
-        static_dir = Path(__file__).parent / "static"
-        templates_dir = Path(__file__).parent / "templates"
-        self.app.mount("/static", StaticFiles(directory=static_dir), name="static")
         self.get_best_move_method = get_best_move_method
+        self.board = board
+        self.router = APIRouter()
+        self.router.add_api_route("/", self.index)
+        self.router.add_api_route(
+            "/set_board/{board_type}", self.set_board, methods=["GET"]
+        )
+        self.router.add_api_route("/legal_moves", self.get_legal_moves, methods=["GET"])
+        self.router.add_api_route(
+            "/set_random_position", self.set_random_position, methods=["GET"]
+        )
+        self.router.add_api_route("/best_move", self.get_best_move, methods=["GET"])
+        self.router.add_api_route("/position", self.get_position, methods=["GET"])
+        self.router.add_api_route(
+            "/move/{source}/{target}", self.move, methods=["POST"]
+        )
+        self.router.add_api_route("/pop", self.pop, methods=["GET"])
+        self.APP.include_router(self.router)
         if not get_best_move_method:
             self.get_best_move_method = lambda board: np.random.choice(
                 list(board.legal_moves)
             )
-        self.templates = Jinja2Templates(directory=templates_dir)
-        self.board = board
-        self.board = Board.from_fen(
-            "W:WK5,K6,12,K21,22,32,K46:B1,K3,18,29,K33,34,40,K42,45,K50"
-        )
-        self.router = APIRouter()
-        self.router.add_api_route("/", self.index)
-        self.router.add_api_route("/set_board/{board_type}", self.set_board)
-        self.router.add_api_route("/set_random_position", self.set_random_position)
-        self.router.add_api_route("/random_move", self.get_best_move)
-        self.router.add_api_route("/get_board_info", self.get_board_info)
-        self.router.add_api_route("/get_legal_moves", self.get_legal_moves)
-        self.app.include_router(self.router)
-        self.draw_board = draw_board
-        self.populate_board = populate_board
-        self.show_pseudo_legal_moves = show_pseudo_legal_moves
 
     def set_board(self, request: Request, board_type: Literal["standard", "american"]):
         if board_type == "standard":
             from draughts.standard import Board
 
             self.board = Board()
         elif board_type == "american":
             from draughts.american import Board
 
             self.board = Board()
 
         return RedirectResponse(url="/")
 
     def get_legal_moves(self):
-        legal_moves = list(self.board.legal_moves)
-
         moves_dict = defaultdict(list)
-        for move in list(legal_moves):
+        for move in list(self.board.legal_moves):
             moves_dict[int(move.square_list[0])].extend(map(int, move.square_list[1:]))
         return {
             "legal_moves": json.dumps(moves_dict),
         }
 
-    def get_board_info(self, request: Request):
-        return (
-            {
-                "request": request,
-                "position": json.dumps(self.board.friendly_form.tolist()),
-                "pseudo_legal_king_moves": json.dumps(
-                    self.board.PSEUDO_LEGAL_KING_MOVES
-                ),
-                "pseudo_legal_man_moves": json.dumps(self.board.PSEUDO_LEGAL_MAN_MOVES),
-                "draw_board": json.dumps(self.draw_board),
-                "populate_board": json.dumps(self.populate_board),
-                "show_pseudo_legal_moves": json.dumps(self.show_pseudo_legal_moves),
-                "size": self.board.shape[0] ** 2,
-            },
+    @property
+    def position_json(self) -> PositionResponse:
+        history = []  # (numver, white, black)
+        stack = self.board._moves_stack
+        for idx in range(len(stack)):
+            src, tg = stack[idx].square_list[0] + 1, stack[idx].square_list[-1]
+            if idx % 2 == 0:
+                history.append([(idx // 2) + 1, f"{src}-{tg}"])
+            else:
+                history[-1].append(f"{src}-{tg}")
+        turn = "white" if self.board.turn == Color.WHITE else "black"
+        return PositionResponse(
+            position=self.board.friendly_form.tolist(),
+            history=history,
+            turn=turn,
         )
 
-    def set_random_position(self, request: Request):
+    def get_position(self, request: Request) -> PositionResponse:
+        return self.position_json
+
+    def set_random_position(self, request: Request) -> PositionResponse:
         STARTING_POSITION = np.random.choice(
             [10, 0, -10, 1, -1],
             size=len(self.board.STARTING_POSITION),
             replace=True,
             p=[0.1, 0.6, 0.1, 0.1, 0.1],
         )
+        self.board._moves_stack = []
         self.board._pos = STARTING_POSITION
-        print(f"board fen: {self.board.fen}")
-        return RedirectResponse(url="/")
+        return self.position_json
 
-    def get_best_move(self, request: Request):
-        legal_moves = list(self.board.legal_moves)
-        # print longest capture chain
-        print(max(legal_moves, key=lambda x: len(x.captured_list)))
+    def get_best_move(self, request: Request) -> PositionResponse:
         move = self.get_best_move_method(self.board)
-        print(move)
         self.board.push(move)
-        return {"position": self.board.friendly_form.tolist()}
+        return self.position_json
+
+    def move(self, request: Request, source: str, target: str) -> PositionResponse:
+        move_str = f"{source}-{target}"
+        print(move_str)
+        self.board.push_from_str(move_str)
+        return self.position_json
+
+    def pop(self, request: Request) -> PositionResponse:
+        self.board.pop()
+        return self.position_json
 
     def index(self, request: Request):
         return self.templates.TemplateResponse(
             "index.html",
             {
                 "request": request,
-                "board": json.dumps(self.board.friendly_form.tolist()),
-                "pseudo_legal_king_moves": json.dumps(
-                    self.board.PSEUDO_LEGAL_KING_MOVES
-                ),
-                "pseudo_legal_man_moves": json.dumps(self.board.PSEUDO_LEGAL_MAN_MOVES),
-                "draw_board": json.dumps(self.draw_board),
-                "populate_board": json.dumps(self.populate_board),
-                "show_pseudo_legal_moves": json.dumps(self.show_pseudo_legal_moves),
-                "size": self.board.shape[0] ** 2,
+                "size": len(self.board.STARTING_POSITION) * 2,
             },
         )
 
     def run(self, **kwargs):
-        uvicorn.run(self.app, **kwargs)
+        uvicorn.run(self.APP, **kwargs)
 
 
 if __name__ == "__main__":
+    from draughts.standard import Board
+
     server = Server(
-        get_best_move_method=lambda board: np.random.choice(list(board.legal_moves))
+        get_best_move_method=lambda board: np.random.choice(list(board.legal_moves)),
     )
     server.run()
```

### Comparing `py-draughts-0.9.9/draughts/standard.py` & `py-draughts-1.0.0/draughts/standard.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/draughts/static/css/style.css` & `py-draughts-1.0.0/draughts/static/css/style.css`

 * *Files 21% similar despite different names*

```diff
@@ -69,14 +69,28 @@
     cursor: pointer;
     /* hover-time */
     transition: 0.2s ease-in-out;
     /* not user select */
     user-select: none;
 }
 
+.higlight {
+    background-color: var(--red) !important;
+    border-radius: 70px;
+    transition: 0.1s ease-in-out;
+}
+
+.dark-tile {
+    background-color: var(--dark);
+}
+
+.light-tile {
+    background-color: var(--light);
+    color: var(--dark);
+}
 
 .piece {
     position: absolute;
     width: 80%;
     height: 80%;
     border-radius: 50%;
     opacity: .84;
@@ -102,17 +116,15 @@
 }
 
 .tile:hover {
     /* background */
     border-radius: 6px;
 }
 
-.tile:active {
-    /* background */
-}
+
 
 .tile:active .piece {
     /* background */
     width: 70%;
     height: 70%;
 }
 
@@ -140,8 +152,53 @@
     user-select: none;
 }
 
 .btn-custom:hover {
     background-color: var(--dark);
     color: var(--primary);
     border: 2px solid var(--primary);
+}
+
+.history-container {
+    position: relative;
+    overflow-y: scroll;
+    max-height: 500px;
+    background-color: var(--secondary) !important;
+    border: 0 2px solid var(--primary);
+    border-radius: 10px;
+    font-weight: bold;
+    cursor: pointer;
+}
+
+table {
+    color: var(--light) !important;
+    border: var(--light) !important;
+    font-size: medium;
+}
+
+tr {
+    border: 1px solid var(--light) !important;
+}
+
+/* width */
+::-webkit-scrollbar {
+    width: 10px;
+    /* background: var(--primary); */
+    border-radius: 0px;
+}
+
+/* Track */
+::-webkit-scrollbar-track {
+    border-radius: 0px;
+    background: var(--secondary);
+}
+
+/* Handle */
+::-webkit-scrollbar-thumb {
+    background: var(--primary);
+    /* border-radius: inherit; */
+}
+
+/* auto scroll to bottom */
+.history-container {
+    scroll-behavior: smooth;
 }
```

### Comparing `py-draughts-0.9.9/draughts/templates/base.html` & `py-draughts-1.0.0/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/draughts/templates/index.html` & `py-draughts-1.0.0/draughts/templates/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -14,63 +14,73 @@
         </div>
         <a href="/set_board/american" class="col-12 btn btn-custom mt-3"
           >American (8x8)</a
         >
         <a href="/set_board/standard" class="col-12 btn btn-custom mt-3"
           >Standard (10x10)</a
         >
-        <a href="#" class="col-12 btn btn-custom mt-3">Your own board</a>
+        <a href="#" class="col-12 btn btn-custom mt-3 disabled"
+          >Your own board . . .</a
+        >
         <!-- game settings -->
         <hr class="col-12 bg-secondary" />
         <div class="col-12">
-          <p class="display-6">Game settings</p>
+          <p class="display-6">Game control</p>
         </div>
-        <button id="makeRandomMove" class="col-12 btn btn-custom mt-3">
-          Make random move
+        <button id="makeMove" class="col-12 btn btn-custom mt-3">
+          Make engine move
+          <hr />
+          <code>Calls method provided on server `__init__`</code>
+        </button>
+
+        <button id="popBtn" class="col-12 btn btn-custom mt-3">Undo</button>
+        <button id="randomPos" class="col-12 btn btn-custom mt-3">
+          Set random position
         </button>
-        <a href="/set_random_position" class="col-12 btn btn-custom mt-3"
-          >Set random position</a
-        >
       </div>
     </div>
     <div class="col-6 h-100">
       <div
         id="board"
         class="board"
-        board="{{board}}"
-        pseudo_legal_king_moves="{{pseudo_legal_king_moves}}"
-        pseudo_legal_man_moves="{{pseudo_legal_man_moves}}"
-        draw_board="{{draw_board}}"
-        populate_board="{{populate_board}}"
-        show_pseudo_legal_moves="{{show_pseudo_legal_moves}}"
         crown_icon="{{ url_for('static', path='img/crown-icon.svg') }}"
       >
         {% for i in range(size) %}
         <div class="tile" id="tile-{{ i }}" tile-number="{{ i }}">
           <p id="tile-{{ i }}-text" class="tile-text"></p>
         </div>
         {% endfor %}
       </div>
     </div>
-    <div class="col-2 rounded p-5">
+    <div class="col-2 pl-5 pr-0 pb-5 pt-5 rounded">
       <div class="row">
         <div class="col-12">
           <h1 class="text-center">Game info</h1>
         </div>
         <hr class="col-12 bg-secondary" />
+
         <div class="col-12">
-          <p class="display-6">Game state</p>
-        </div>
-        <div class="col-12">
-          <p class="display-6">Turn</p>
-        </div>
-        <div class="col-12">
-          <p class="display-6">Move count</p>
+          <p class="display-6">Turn: <code id="turn">White</code></p>
         </div>
         <div class="col-12">
           <p class="display-6">Move history</p>
+          <table class="table m-0">
+            <thead>
+              <tr>
+                <th scope="col">Nr</th>
+                <th scope="col">White</th>
+                <th scope="col">Black</th>
+              </tr>
+            </thead>
+          </table>
+
+          <div class="history-container m-0">
+            <table class="table">
+              <tbody id="historyTableBody"></tbody>
+            </table>
+          </div>
         </div>
       </div>
     </div>
   </div>
 </main>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
  {% extends "base.html" %} {% block content %}
 ****** Settings ******
 
 ===============================================================================
 Game type
-American_(8x8) Standard_(10x10) Your_own_board
+American_(8x8) Standard_(10x10) Your_own_board_._._.
 ===============================================================================
-Game settings
- Make random move  Set_random_position
+Game control
+ Make engine move
+===============================================================================
+Calls method provided on server `__init__`  Undo  Set random position
 {% for i in range(size) %}
 {% endfor %}
 ****** Game info ******
 ===============================================================================
-Game state
-Turn
-Move count
+Turn: White
 Move history
+Nr White Black
  {% endblock %}
```

### Comparing `py-draughts-0.9.9/draughts/utils.py` & `py-draughts-1.0.0/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.0.0/py_draughts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 0.9.9
+Version: 1.0.0
 Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -156,23 +156,27 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a5e2ca89-28e1-4dcc-96ae-b18fc602c9bc" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5712f27f-b3fd-44e5-9f6e-08e32b9eddd2" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b14523ea-4bc4-45e1-b5c0-5deea3ed5328" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4de34033-fff5-41e8-a8d8-b1b1ff399149" width="800" />
 
-*Legal moves for selected square (on image "16")*
+*Legal moves for selected square (on image "11")*
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/c8245cbc-06ec-4623-81ab-c9aaa9302627" width="600" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5f9c0b41-6bce-4c1d-ac47-042a9e28f61e" width="800" />
 
 
+### testing best moves finding methods:
+
+[Example](examples/engine.py)
+
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
 
 1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
```

### Comparing `py-draughts-0.9.9/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.0.0/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/setup.py` & `py-draughts-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/test/test_american_board.py` & `py-draughts-1.0.0/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.9/test/test_board.py` & `py-draughts-1.0.0/test/test_board.py`

 * *Files identical despite different names*


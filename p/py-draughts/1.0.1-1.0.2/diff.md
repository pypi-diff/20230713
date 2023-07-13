# Comparing `tmp/py-draughts-1.0.1.tar.gz` & `tmp/py-draughts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.0.1.tar", last modified: Thu Jul 13 16:53:48 2023, max compression
+gzip compressed data, was "py-draughts-1.0.2.tar", last modified: Thu Jul 13 18:26:17 2023, max compression
```

## Comparing `py-draughts-1.0.1.tar` & `py-draughts-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:48.006384 py-draughts-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6317 2023-07-13 16:53:48.004394 py-draughts-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4899 2023-07-13 16:53:22.000000 py-draughts-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.958394 py-draughts-1.0.1/draughts/
--rw-rw-rw-   0        0        0      964 2023-07-13 16:53:32.000000 py-draughts-1.0.1/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-12 12:15:32.000000 py-draughts-1.0.1/draughts/american.py
--rw-rw-rw-   0        0        0    10865 2023-07-13 09:58:48.000000 py-draughts-1.0.1/draughts/base.py
--rw-rw-rw-   0        0        0      674 2023-07-11 19:49:33.000000 py-draughts-1.0.1/draughts/models.py
--rw-rw-rw-   0        0        0     4195 2023-07-13 09:58:48.000000 py-draughts-1.0.1/draughts/move.py
--rw-rw-rw-   0        0        0     5193 2023-07-13 16:38:38.000000 py-draughts-1.0.1/draughts/server.py
--rw-rw-rw-   0        0        0     5989 2023-07-12 12:15:34.000000 py-draughts-1.0.1/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.884385 py-draughts-1.0.1/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.965391 py-draughts-1.0.1/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.1/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.969391 py-draughts-1.0.1/draughts/static/js/
--rw-rw-rw-   0        0        0     5669 2023-07-13 16:39:11.000000 py-draughts-1.0.1/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.978386 py-draughts-1.0.1/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.1/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2705 2023-07-13 16:36:29.000000 py-draughts-1.0.1/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.1/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:47.994388 py-draughts-1.0.1/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6317 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 16:53:47.000000 py-draughts-1.0.1/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 16:53:48.007387 py-draughts-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:53:48.002389 py-draughts-1.0.1/test/
--rw-rw-rw-   0        0        0     1123 2023-07-11 18:56:31.000000 py-draughts-1.0.1/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-11 18:56:31.000000 py-draughts-1.0.1/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:17.032570 py-draughts-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6266 2023-07-13 18:26:17.028560 py-draughts-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4848 2023-07-13 18:25:28.000000 py-draughts-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.955914 py-draughts-1.0.2/draughts/
+-rw-rw-rw-   0        0        0      964 2023-07-13 18:26:14.000000 py-draughts-1.0.2/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-13 18:02:36.000000 py-draughts-1.0.2/draughts/american.py
+-rw-rw-rw-   0        0        0    11185 2023-07-13 18:19:05.000000 py-draughts-1.0.2/draughts/base.py
+-rw-rw-rw-   0        0        0      671 2023-07-13 17:34:05.000000 py-draughts-1.0.2/draughts/models.py
+-rw-rw-rw-   0        0        0     4197 2023-07-13 18:10:29.000000 py-draughts-1.0.2/draughts/move.py
+-rw-rw-rw-   0        0        0     5331 2023-07-13 18:14:29.000000 py-draughts-1.0.2/draughts/server.py
+-rw-rw-rw-   0        0        0     5989 2023-07-13 18:10:31.000000 py-draughts-1.0.2/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.911909 py-draughts-1.0.2/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.962557 py-draughts-1.0.2/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.2/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.967592 py-draughts-1.0.2/draughts/static/js/
+-rw-rw-rw-   0        0        0     5993 2023-07-13 18:16:53.000000 py-draughts-1.0.2/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:16.976563 py-draughts-1.0.2/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.2/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2860 2023-07-13 18:13:53.000000 py-draughts-1.0.2/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.2/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:17.003562 py-draughts-1.0.2/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6266 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 18:26:16.000000 py-draughts-1.0.2/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 18:26:17.032570 py-draughts-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:26:17.021561 py-draughts-1.0.2/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-13 17:33:45.000000 py-draughts-1.0.2/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-13 17:33:45.000000 py-draughts-1.0.2/test/test_board.py
```

### Comparing `py-draughts-1.0.1/LICENSE` & `py-draughts-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.1/PKG-INFO` & `py-draughts-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.1
+Version: 1.0.2
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -160,21 +160,20 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5712f27f-b3fd-44e5-9f6e-08e32b9eddd2" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e1caeb3f-2744-4198-a426-76ad184a448a" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4de34033-fff5-41e8-a8d8-b1b1ff399149" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
 
-*Legal moves for selected square (on image "11")*
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5f9c0b41-6bce-4c1d-ac47-042a9e28f61e" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e6ae7861-624d-497a-b617-e499d817f6a3" width="800" />
 
 
 ### testing best moves finding methods:
 
 [Example](examples/engine.py)
 
 ## Contributing
```

### Comparing `py-draughts-1.0.1/README.md` & `py-draughts-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,21 +131,20 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5712f27f-b3fd-44e5-9f6e-08e32b9eddd2" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e1caeb3f-2744-4198-a426-76ad184a448a" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4de34033-fff5-41e8-a8d8-b1b1ff399149" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
 
-*Legal moves for selected square (on image "11")*
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5f9c0b41-6bce-4c1d-ac47-042a9e28f61e" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e6ae7861-624d-497a-b617-e499d817f6a3" width="800" />
 
 
 ### testing best moves finding methods:
 
 [Example](examples/engine.py)
 
 ## Contributing
```

### Comparing `py-draughts-1.0.1/draughts/__init__.py` & `py-draughts-1.0.2/draughts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-1.0.1/draughts/american.py` & `py-draughts-1.0.2/draughts/american.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Generator
 
 import numpy as np
 from draughts.base import BaseBoard
-from draughts.models import Color, Entity
+from draughts.models import Color, Figure
 from draughts.move import Move
 from draughts.utils import logger
 
 
 # fmt: off
 SQUARES = [B8, D8, F8, H8,
         A7, C7, E7, G7,
@@ -57,15 +57,15 @@
         self, square: int, is_after_capture=False
     ) -> Generator[Move, None, None]:
         row = self.row_idx[square]
         moves = []
         odd = bool(row % 2 != 0 and self.turn == Color.BLACK) or (
             row % 2 == 0 and self.turn == Color.WHITE
         )
-        is_king = bool(self[square] == self.turn.value * Entity.KING)
+        is_king = bool(self[square] == self.turn.value * Figure.KING)
         # is_king = False  # DEBUG
         for mv_offset, cap_offset, dir in [
             (4 - odd, 7, self.turn.value),
             (5 - odd, 9, self.turn.value),
         ] + is_king * [
             (4 - (not odd), 7, -self.turn.value),
             (5 - (not odd), 9, -self.turn.value),
```

### Comparing `py-draughts-1.0.1/draughts/base.py` & `py-draughts-1.0.2/draughts/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from abc import ABC
 from typing import Generator
 from collections import defaultdict
 import numpy as np
 import re
 
-from draughts.models import ENTITY_REPR, Color, Entity, SquareT
+from draughts.models import ENTITY_REPR, Color, Figure, SquareT
 from draughts.move import Move
 from draughts.utils import (
     logger,
     get_king_pseudo_legal_moves,
     get_man_pseudo_legal_moves,
 )
 
@@ -141,21 +141,25 @@
         """
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         # is promotion
-        if (tg // (self.shape[0] // 2)) in (0, self.shape[0] - 1) and abs(
-            self._pos[tg]
-        ) == 1:
-            self._pos[tg] *= Entity.KING.value
+        if (
+            (tg // (self.shape[0] // 2)) == 0
+            and self._pos[tg] == Figure.WHITE_MAN.value
+        ) or (
+            (tg // (self.shape[0] // 2)) == (self.shape[0] - 1)
+            and self._pos[tg] == Figure.BLACK_MAN.value
+        ):
+            self._pos[tg] *= Figure.KING.value
             move.is_promotion = True
         if move.captured_list:
-            self._pos[np.array([sq for sq in move.captured_list])] = Entity.EMPTY
+            self._pos[np.array([sq for sq in move.captured_list])] = Figure.EMPTY
         self._moves_stack.append(move)
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
 
     def pop(self, is_finished=True) -> None:
         """Pops a move from the board.
 
@@ -164,15 +168,15 @@
         """
         move = self._moves_stack.pop()
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
         if move.is_promotion:
-            self._pos[tg] //= Entity.KING.value
+            self._pos[tg] //= Figure.KING.value
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         for sq, entity in zip(move.captured_list, move.captured_entities):
             self._pos[sq] = entity  # Dangerous line
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
         return move
 
@@ -241,15 +245,15 @@
     @classmethod
     def __populate_from_list(cls, fen_list: list[str], color: Color) -> None:
         board_range = range(1, cls.STARTING_POSITION.shape[0] + 1)
         for sq in fen_list:
             if sq.isdigit() and int(sq) in board_range:
                 cls.STARTING_POSITION[int(sq) - 1] = color.value
             elif sq.startswith("K") and sq[1:].isdigit() and int(sq[1:]) in board_range:
-                cls.STARTING_POSITION[int(sq[1:]) - 1] = color.value * Entity.KING.value
+                cls.STARTING_POSITION[int(sq[1:]) - 1] = color.value * Figure.KING.value
             else:
                 raise ValueError(
                     f"Wrong FEN: invalid square value: {sq} for board with length\
                         {cls.STARTING_POSITION.shape[0]}"
                 )
 
     @classmethod
@@ -274,29 +278,36 @@
         for idx, sq in enumerate(self.position):
             new_pos.extend([0] * (idx % (self.shape[0] // 2) != 0))
             new_pos.extend([0, 0] * (idx % self.shape[0] == 0 and idx != 0))
             new_pos.append(sq)
         new_pos.append(0)
         return np.array(new_pos)
 
+    @staticmethod
+    def is_capture(move: Move) -> bool:
+        """
+        Checks if a move is a capture.
+        """
+        return len(move.captured_list) > 0
+
     def __repr__(self) -> str:
         board = ""
         position = self.friendly_form
         for i in range(self.shape[0]):
             # board += f"{'-' * (self.shape[0]*4 + 1) }\n|"
             for j in range(self.shape[0]):
                 board += f" {ENTITY_REPR[position[i*self.shape[0] + j]]}"
             board += "\n"
         return board
 
-    def __iter__(self) -> Generator[Entity, None, None]:
+    def __iter__(self) -> Generator[Figure, None, None]:
         for sq in self.position:
             yield sq
 
-    def __getitem__(self, key: SquareT) -> Entity:
+    def __getitem__(self, key: SquareT) -> Figure:
         return self.position[key]
 
 
 if __name__ == "__main__":
     # board = BaseBoard(BaseBoard.STARTING_POSITION)
     # print(board)
     BaseBoard.from_fen(
```

### Comparing `py-draughts-1.0.1/draughts/models.py` & `py-draughts-1.0.2/draughts/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 
 class Color(Enum):
     WHITE = -1
     BLACK = 1
 
 
-class Entity(IntEnum):
-    BLACK_KING = Color.BLACK.value * 10
+class Figure(IntEnum):
+    BLACK_KING = Color.BLACK.value * 2
     BLACK_MAN = Color.BLACK.value
-    WHITE_KING = Color.WHITE.value * 10
+    WHITE_KING = Color.WHITE.value * 2
     WHITE_MAN = Color.WHITE.value
-    KING = 10
+    KING = 2
     MAN = 1
     EMPTY = 0
 
 
 ENTITY_REPR = {
-    Entity.BLACK_MAN: "b",
-    Entity.WHITE_MAN: "w",
-    Entity.EMPTY: ".",
-    Entity.BLACK_KING: "B",
-    Entity.WHITE_KING: "W",
+    Figure.BLACK_MAN: "b",
+    Figure.WHITE_MAN: "w",
+    Figure.EMPTY: ".",
+    Figure.BLACK_KING: "B",
+    Figure.WHITE_KING: "W",
 }
```

### Comparing `py-draughts-1.0.1/draughts/move.py` & `py-draughts-1.0.2/draughts/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Generator, NewType
 
 import numpy as np
 
-from draughts.models import Color, Entity, SquareT
+from draughts.models import Color, Figure, SquareT
 
 
 class Move:
     """Move representation.
     End user should never interact with this class directly.
 
     As we can read on wikipedia:
@@ -26,15 +26,15 @@
     n - 2 - number of captured pieces
     """
 
     def __init__(
         self,
         visited_squares: list[int],
         captured_list: list[int] = [],
-        captured_entities: list[Entity.value] = [],
+        captured_entities: list[Figure.value] = [],
         is_promotion: bool = False,
     ) -> None:
         self.square_list = visited_squares
         self.captured_list = captured_list
         self.captured_entities = captured_entities
         self.is_promotion = is_promotion
 
@@ -63,15 +63,15 @@
             )
 
             return all(square in longer for square in shorter)
 
         return False
 
     def __len__(self) -> int:
-        return len(self.square_list) + 1
+        return len(self.captured_list) + 1
 
     def __add__(self, other: Move) -> Move:
         """Append moves"""
         if self.square_list[-1] != other.square_list[0]:
             raise ValueError(
                 f"Cannot append moves {self} and {other}. Last square of first move should be equal to first square of second move."
             )
```

### Comparing `py-draughts-1.0.1/draughts/server.py` & `py-draughts-1.0.2/draughts/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.board = board
         self.router = APIRouter()
         self.router.add_api_route("/", self.index)
         self.router.add_api_route(
             "/set_board/{board_type}", self.set_board, methods=["GET"]
         )
         self.router.add_api_route("/legal_moves", self.get_legal_moves, methods=["GET"])
+        self.router.add_api_route("/fen", self.get_fen, methods=["GET"])
         self.router.add_api_route(
             "/set_random_position", self.set_random_position, methods=["GET"]
         )
         self.router.add_api_route("/best_move", self.get_best_move, methods=["GET"])
         self.router.add_api_route("/position", self.get_position, methods=["GET"])
         self.router.add_api_route(
             "/move/{source}/{target}", self.move, methods=["POST"]
@@ -51,14 +52,17 @@
         self.router.add_api_route("/pop", self.pop, methods=["GET"])
         self.APP.include_router(self.router)
         if not get_best_move_method:
             self.get_best_move_method = lambda board: np.random.choice(
                 list(board.legal_moves)
             )
 
+    def get_fen(self):
+        return {"fen": self.board.fen}
+
     def set_board(self, request: Request, board_type: Literal["standard", "american"]):
         if board_type == "standard":
             from draughts.standard import Board
 
             self.board = Board()
         elif board_type == "american":
             from draughts.american import Board
@@ -93,15 +97,15 @@
         )
 
     def get_position(self, request: Request) -> PositionResponse:
         return self.position_json
 
     def set_random_position(self, request: Request) -> PositionResponse:
         STARTING_POSITION = np.random.choice(
-            [10, 0, -10, 1, -1],
+            [2, 0, -2, 1, -1],
             size=len(self.board.STARTING_POSITION),
             replace=True,
             p=[0.1, 0.6, 0.1, 0.1, 0.1],
         )
         self.board._moves_stack = []
         self.board._pos = STARTING_POSITION
         return self.position_json
```

### Comparing `py-draughts-1.0.1/draughts/standard.py` & `py-draughts-1.0.2/draughts/standard.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from typing import Generator
 
 import numpy as np
 from collections import defaultdict
 from draughts.base import BaseBoard
-from draughts.models import Color, Entity
+from draughts.models import Color, Figure
 from draughts.move import Move
 from draughts.utils import (
     logger,
     get_king_pseudo_legal_moves,
     get_man_pseudo_legal_moves,
 )
 
@@ -76,22 +76,22 @@
         moves = []
         # white can move only on even directions
         for idx, direction in enumerate(self.PSEUDO_LEGAL_MAN_MOVES[square]):
             if (
                 len(direction) > 0
                 and (self.turn.value + idx)
                 in [-1, 0, 3, 4]  # TERRIBLE HACK get only directions for given piece
-                and self._pos[direction[0]] == Entity.EMPTY
+                and self._pos[direction[0]] == Figure.EMPTY
                 and not is_capture_mandatory
             ):
                 moves.append(Move([square, direction[0]]))
             elif (
                 len(direction) > 1
                 and self._pos[direction[0]] * self.turn.value < 0
-                and self._pos[direction[1]] == Entity.EMPTY
+                and self._pos[direction[1]] == Figure.EMPTY
             ):
                 move = Move(
                     [square, direction[1]], [direction[0]], [self._pos[direction[0]]]
                 )
                 moves.append(move)
                 self.push(move, False)
                 moves += [move + m for m in self._legal_moves_from(direction[1], True)]
@@ -103,19 +103,19 @@
     ) -> list[Move]:
         moves = []
         for direction in self.PSEUDO_LEGAL_KING_MOVES[square]:
             for idx, target in enumerate(direction):
                 if (
                     len(direction) > idx + 1
                     and self._pos[target] * self.turn.value < 0
-                    and self._pos[direction[idx + 1]] == Entity.EMPTY
+                    and self._pos[direction[idx + 1]] == Figure.EMPTY
                 ):
                     i = idx + 1
                     while (
-                        i < len(direction) and self._pos[direction[i]] == Entity.EMPTY
+                        i < len(direction) and self._pos[direction[i]] == Figure.EMPTY
                     ):
                         move = Move(
                             [square, direction[i]], [target], [self._pos[target]]
                         )
                         moves.append(move)
                         self.push(move, False)
                         moves += [
@@ -124,24 +124,24 @@
                         # if one move is longer then others return only this one
                         self.pop(False)
                         max_len = max([len(m) for m in moves])
                         moves = [m for m in moves if len(m) == max_len]
                         i += 1
                     break
                 if (
-                    self._pos[target] == Entity.EMPTY.value and not is_capture_mandatory
+                    self._pos[target] == Figure.EMPTY.value and not is_capture_mandatory
                 ):  # casual move
                     moves.append(Move([square, target]))
                 else:
                     break
         return moves
 
     def _legal_moves_from(self, square: int, is_capture_mandatory=False) -> list[Move]:
-        entity = Entity(self._pos[square])
-        if abs(entity) == Entity.MAN:
+        entity = Figure(self._pos[square])
+        if abs(entity) == Figure.MAN:
             moves = self._get_man_legal_moves_from(square, is_capture_mandatory)
         else:
             moves = self._get_king_legal_moves_from(square, is_capture_mandatory)
         if is_capture_mandatory:
             moves = [move for move in moves if len(move.captured_list) > 0]
         return moves
```

### Comparing `py-draughts-1.0.1/draughts/static/css/style.css` & `py-draughts-1.0.2/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.1/draughts/static/js/script.js` & `py-draughts-1.0.2/draughts/static/js/script.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -16,16 +16,16 @@
 );
 
 let redColor = getComputedStyle(document.body).getPropertyValue("--red");
 
 const colorMap = {
     1: whiteManColor,
     "-1": blackManColor,
-    10: whiteManColor,
-    "-10": blackManColor,
+    2: whiteManColor,
+    "-2": blackManColor,
 };
 
 // ######################### constants #########################
 var boardArray = null;
 var legalMoves = null;
 var historyData = null;
 var turn = null;
@@ -52,14 +52,24 @@
             boardArray = data["position"];
             historyData = data["history"];
             turn = data["turn"];
             upadateBoard();
         },
     });
 
+const getFen = () =>
+    $.ajax({
+        url: "fen",
+        type: "GET",
+        success: (data) => {
+            navigator.clipboard.writeText(data["fen"]);
+            alert("Copied the text: " + data["fen"]);
+        },
+    });
+
 const getPosition = () =>
     new Promise((resolve, reject) =>
         $.ajax({
             url: "position",
             type: "GET",
             success: (data) => resolve(data["position"]),
             error: reject,
@@ -141,22 +151,22 @@
         }
     });
 };
 
 const updatehistory = () => {
     let tbody = $("#historyTableBody");
     tbody.empty();
-    console.log(historyData);
     if (!historyData) return;
     for (let i = 0; i < historyData.length; i++) {
         if (!historyData[i][2]) historyData[i][2] = "-";
         tbody.append(
             `<tr><td>${historyData[i][0]}</td><td>${historyData[i][1]}</td><td>${historyData[i][2]}</td></tr>`
         );
     }
+    $("#historyContainer").scrollTop($("#historyContainer")[0].scrollHeight);
 };
 
 const upadateBoard = () => {
     for (let i = 0; i < boardArray.length; i++) {
         let tile = $(`#tile-${i}`);
         $(".higlight").removeClass("higlight");
         tile.children(".piece").remove();
@@ -165,15 +175,17 @@
             tile.append(
                 `<div class="piece" id="piece-${i}" style="background-color: ${
           colorMap[boardArray[i]]
         }"></div>`
             );
             $(`#piece-${i}`).click(showLegalMoves);
             if (Math.abs(boardArray[i]) > 1) {
-                $(`#tile-${i}`).append(`<img src="${crown_icon}" class="crown" />`);
+                $(`#tile-${i}`).append(
+                    `<img src="${crown_icon}" alt="crown" class="crown" />`
+                );
             }
         }
     }
     updatehistory();
     $("#turn").text(turn);
 };
 
@@ -200,8 +212,9 @@
 $(document).ready(async () => {
     boardArray = await getPosition();
     init(boardArray);
     upadateBoard();
     $("#makeMove").click(makeBestMove);
     $("#popBtn").click(pop);
     $("#randomPos").click(getRandomPos);
+    $("#copyFen").click(getFen);
 });
```

### Comparing `py-draughts-1.0.1/draughts/templates/base.html` & `py-draughts-1.0.2/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.1/draughts/templates/index.html` & `py-draughts-1.0.2/draughts/templates/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,17 @@
           <code>Calls method provided on server `__init__`</code>
         </button>
 
         <button id="popBtn" class="col-12 btn btn-custom mt-3">Undo</button>
         <button id="randomPos" class="col-12 btn btn-custom mt-3">
           Set random position
         </button>
+        <button id="copyFen" class="col-12 btn btn-custom mt-3">
+          Copy FEN <small>to clipboard</small>
+        </button>
       </div>
     </div>
     <div class="col-6 h-100">
       <div
         id="board"
         class="board"
         crown_icon="{{ url_for('static', path='img/crown-icon.svg') }}"
@@ -69,15 +72,15 @@
                 <th scope="col">Nr</th>
                 <th scope="col">White</th>
                 <th scope="col">Black</th>
               </tr>
             </thead>
           </table>
 
-          <div class="history-container m-0">
+          <div id="historyContainer" class="history-container m-0">
             <table class="table">
               <tbody id="historyTableBody"></tbody>
             </table>
           </div>
         </div>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -4,15 +4,16 @@
 ===============================================================================
 Game type
 American_(8x8) Standard_(10x10) Your_own_board_._._.
 ===============================================================================
 Game control
  Make engine move
 ===============================================================================
-Calls method provided on server `__init__`  Undo  Set random position
+Calls method provided on server `__init__`  Undo  Set random position   Copy
+FEN to clipboard
 {% for i in range(size) %}
 {% endfor %}
 ****** Game info ******
 ===============================================================================
 Turn: White
 Move history
 Nr White Black
```

### Comparing `py-draughts-1.0.1/draughts/utils.py` & `py-draughts-1.0.2/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.1/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.0.2/py_draughts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.1
+Version: 1.0.2
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -160,21 +160,20 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5712f27f-b3fd-44e5-9f6e-08e32b9eddd2" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e1caeb3f-2744-4198-a426-76ad184a448a" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4de34033-fff5-41e8-a8d8-b1b1ff399149" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
 
-*Legal moves for selected square (on image "11")*
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/5f9c0b41-6bce-4c1d-ac47-042a9e28f61e" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e6ae7861-624d-497a-b617-e499d817f6a3" width="800" />
 
 
 ### testing best moves finding methods:
 
 [Example](examples/engine.py)
 
 ## Contributing
```

### Comparing `py-draughts-1.0.1/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.0.2/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.1/setup.py` & `py-draughts-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.1/test/test_american_board.py` & `py-draughts-1.0.2/test/test_american_board.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pytest
 
 import draughts.american as checkers
 from draughts.american import Board, Move, Color
-from draughts.models import Entity
+from draughts.models import Figure
 
 
 class TestAmericanBoard:
     @pytest.fixture(autouse=True)
     def setup(self):
         self.board = Board()
         yield
@@ -28,8 +28,8 @@
         assert self.board.pop() == m1
         assert np.array_equal(self.board.position, Board.STARTING_POSITION)
 
     def test_capture(self):
         moves = ["24-20", "11-16", "20x11", "7x16"]
         for m in moves:
             self.board.push_from_str(m)
-        assert self.board[checkers.F6] == Entity.EMPTY.value
+        assert self.board[checkers.F6] == Figure.EMPTY.value
```

### Comparing `py-draughts-1.0.1/test/test_board.py` & `py-draughts-1.0.2/test/test_board.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 
 import draughts.base as checkers
-from draughts.base import BaseBoard, Color, Entity, Move
+from draughts.base import BaseBoard, Color, Figure, Move
 
 
 class TestBoard:
     @pytest.fixture(autouse=True)
     def setup(self):
         self.board = BaseBoard(BaseBoard.STARTING_POSITION)
         yield
@@ -16,51 +16,51 @@
         assert self.board.turn == Color.WHITE
         assert np.array_equal(self.board.position, BaseBoard.STARTING_POSITION)
 
     def test_move(self):
         m = Move([checkers.A3, checkers.B4])
         self.board.push(m)
         assert self.board.turn == Color.BLACK
-        assert self.board[checkers.A3] == Entity.EMPTY
-        assert self.board[checkers.B4] == Entity.WHITE_MAN
+        assert self.board[checkers.A3] == Figure.EMPTY
+        assert self.board[checkers.B4] == Figure.WHITE_MAN
         m = Move([checkers.F6, checkers.G5])
         self.board.push(m)
         assert self.board.turn == Color.WHITE
-        assert self.board[checkers.F6] == Entity.EMPTY
-        assert self.board[checkers.G5] == Entity.BLACK_MAN
+        assert self.board[checkers.F6] == Figure.EMPTY
+        assert self.board[checkers.G5] == Figure.BLACK_MAN
 
     def test_capture(self):
         m1 = Move([checkers.C3, checkers.B4])
         self.board.push(m1)
 
         m2 = Move([checkers.B6, checkers.A5])
         self.board.push(m2)
 
         m3 = Move([checkers.G3, checkers.H4])
         self.board.push(m3)
 
         m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
         self.board.push(m4)
 
-        assert self.board[checkers.B4] == Entity.EMPTY
-        assert self.board[checkers.C3] == Entity.BLACK_MAN
+        assert self.board[checkers.B4] == Figure.EMPTY
+        assert self.board[checkers.C3] == Figure.BLACK_MAN
 
         m5 = Move([checkers.B2, checkers.D4], captured_list=[checkers.C3])
         self.board.push(m5)
-        assert self.board[checkers.B2] == Entity.EMPTY
-        assert self.board[checkers.C3] == Entity.EMPTY
-        assert self.board[checkers.D4] == Entity.WHITE_MAN
+        assert self.board[checkers.B2] == Figure.EMPTY
+        assert self.board[checkers.C3] == Figure.EMPTY
+        assert self.board[checkers.D4] == Figure.WHITE_MAN
 
     def test_pop(self):
         m = Move([checkers.A3, checkers.B4])
         self.board.push(m)
         assert self.board.turn == Color.BLACK
-        assert self.board[checkers.A3] == Entity.EMPTY
-        assert self.board[checkers.B4] == Entity.WHITE_MAN
+        assert self.board[checkers.A3] == Figure.EMPTY
+        assert self.board[checkers.B4] == Figure.WHITE_MAN
         m = Move([checkers.F6, checkers.G5])
         self.board.push(m)
         self.board.pop()
         assert self.board.turn == Color.BLACK
-        assert self.board[checkers.F6] == Entity.BLACK_MAN
-        assert self.board[checkers.G5] == Entity.EMPTY
-        assert self.board[checkers.A3] == Entity.EMPTY
-        assert self.board[checkers.B4] == Entity.WHITE_MAN
+        assert self.board[checkers.F6] == Figure.BLACK_MAN
+        assert self.board[checkers.G5] == Figure.EMPTY
+        assert self.board[checkers.A3] == Figure.EMPTY
+        assert self.board[checkers.B4] == Figure.WHITE_MAN
```


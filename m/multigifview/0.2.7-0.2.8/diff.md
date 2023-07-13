# Comparing `tmp/multigifview-0.2.7.tar.gz` & `tmp/multigifview-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multigifview-0.2.7.tar", last modified: Fri Jun 24 10:50:11 2022, max compression
+gzip compressed data, was "multigifview-0.2.8.tar", last modified: Thu Jul 13 12:51:01 2023, max compression
```

## Comparing `multigifview-0.2.7.tar` & `multigifview-0.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:50:11.322320 multigifview-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-24 10:49:36.000000 multigifview-0.2.7/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-24 10:49:36.000000 multigifview-0.2.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:50:11.318320 multigifview-0.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:50:11.322320 multigifview-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-06-24 10:49:36.000000 multigifview-0.2.7/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-06-24 10:49:36.000000 multigifview-0.2.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-06-24 10:49:36.000000 multigifview-0.2.7/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (121)    35150 2022-06-24 10:49:36.000000 multigifview-0.2.7/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-06-24 10:50:11.322320 multigifview-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-06-24 10:49:36.000000 multigifview-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:50:11.322320 multigifview-0.2.7/man/
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-06-24 10:50:03.000000 multigifview-0.2.7/man/multigifview.1
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-06-24 10:49:36.000000 multigifview-0.2.7/man/multigifview.1.dev-stub
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:50:11.322320 multigifview-0.2.7/multigifview/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-06-24 10:49:36.000000 multigifview-0.2.7/multigifview/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2345 2022-06-24 10:49:36.000000 multigifview-0.2.7/multigifview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11743 2022-06-24 10:49:36.000000 multigifview-0.2.7/multigifview/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8027 2022-06-24 10:49:36.000000 multigifview-0.2.7/multigifview/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:50:11.322320 multigifview-0.2.7/multigifview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-06-24 10:50:10.000000 multigifview-0.2.7/multigifview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-06-24 10:50:11.000000 multigifview-0.2.7/multigifview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 10:50:10.000000 multigifview-0.2.7/multigifview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-24 10:50:10.000000 multigifview-0.2.7/multigifview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-24 10:50:11.000000 multigifview-0.2.7/multigifview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-24 10:50:11.000000 multigifview-0.2.7/multigifview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-24 10:49:36.000000 multigifview-0.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:50:11.322320 multigifview-0.2.7/qtdesignerfiles/
--rw-r--r--   0 runner    (1001) docker     (121)     7193 2022-06-24 10:49:36.000000 multigifview-0.2.7/qtdesignerfiles/mainwindow.ui
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-06-24 10:50:11.322320 multigifview-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-06-24 10:49:36.000000 multigifview-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:01.016082 multigifview-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 12:50:16.000000 multigifview-0.2.8/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 12:50:16.000000 multigifview-0.2.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:01.012082 multigifview-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:01.016082 multigifview-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-13 12:50:16.000000 multigifview-0.2.8/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-13 12:50:16.000000 multigifview-0.2.8/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-13 12:50:16.000000 multigifview-0.2.8/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-13 12:50:16.000000 multigifview-0.2.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-13 12:51:01.016082 multigifview-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-13 12:50:16.000000 multigifview-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:01.016082 multigifview-0.2.8/man/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 12:50:57.000000 multigifview-0.2.8/man/multigifview.1
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-13 12:50:16.000000 multigifview-0.2.8/man/multigifview.1.dev-stub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:01.016082 multigifview-0.2.8/multigifview/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-13 12:50:16.000000 multigifview-0.2.8/multigifview/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-07-13 12:50:16.000000 multigifview-0.2.8/multigifview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-13 12:50:16.000000 multigifview-0.2.8/multigifview/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-13 12:50:16.000000 multigifview-0.2.8/multigifview/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:01.016082 multigifview-0.2.8/multigifview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-13 12:51:00.000000 multigifview-0.2.8/multigifview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-13 12:51:00.000000 multigifview-0.2.8/multigifview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:51:00.000000 multigifview-0.2.8/multigifview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 12:51:00.000000 multigifview-0.2.8/multigifview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 12:51:00.000000 multigifview-0.2.8/multigifview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 12:51:00.000000 multigifview-0.2.8/multigifview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 12:50:16.000000 multigifview-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:01.016082 multigifview-0.2.8/qtdesignerfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-13 12:50:16.000000 multigifview-0.2.8/qtdesignerfiles/mainwindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-13 12:51:01.016082 multigifview-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 12:50:16.000000 multigifview-0.2.8/setup.py
```

### Comparing `multigifview-0.2.7/.github/workflows/pythonpackage.yml` & `multigifview-0.2.8/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/.github/workflows/pythonpublish.yml` & `multigifview-0.2.8/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/DEVELOPMENT.md` & `multigifview-0.2.8/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/LICENCE` & `multigifview-0.2.8/LICENCE`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/PKG-INFO` & `multigifview-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multigifview
-Version: 0.2.7
+Version: 0.2.8
 Summary: View multiple gif files
 Home-page: https://github.com/johnomotani/multigifview
 Author: John Omotani
 Author-email: john.omotani@ukaea.uk
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
```

### Comparing `multigifview-0.2.7/README.md` & `multigifview-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/multigifview/__main__.py` & `multigifview-0.2.8/multigifview/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from Qt.QtWidgets import QApplication
 import sys
 
 from .core import MultiGifView
 
 
-def show_gifs(*filenames, max_columns=2, titles=True, zoom=None):
+def show_gifs(*filenames, max_columns=2, titles=True, step=1, zoom=None):
     """Show gifs in a Qt window
 
     Any number of gifs can be opened. Each will be in a new column until there are
     max_columns columns. After that new rows will be created and filled until all the
     gifs are shown.
 
     Parameters
@@ -22,15 +22,15 @@
     max_columns : int, default 2
         Maximum number of columns to use
     zoom : float, optional
         Set the initial zoom level of the gifs (in %)
     """
     app = QApplication(sys.argv)
     window = MultiGifView(
-        filenames, max_columns=max_columns, titles=titles, initial_zoom=zoom
+        filenames, max_columns=max_columns, titles=titles, step=step, initial_zoom=zoom
     )
     window.show()
     window.reset_minimum_size()
 
     return app.exec_()
 
 
@@ -65,14 +65,21 @@
     parser.add_argument(
         "-n",
         "--no-titles",
         action="store_true",
         default=False,
         help="Disable titles above gifs",
     )
+    parser.add_argument(
+        "-s",
+        "--step",
+        type=int,
+        default=1,
+        help="Number of frames to step by when going to next frame",
+    )
     from multigifview import __version__
 
     parser.add_argument(
         "-v", "--version", action="version", version="%(prog)s {}".format(__version__)
     )
     parser.add_argument(
         "-z",
@@ -83,14 +90,15 @@
     )
     args = parser.parse_args()
 
     exit_code = show_gifs(
         *args.file,
         max_columns=args.max_columns,
         titles=not args.no_titles,
+        step=args.step,
         zoom=args.zoom
     )
 
     sys.exit(exit_code)
 
 
 if __name__ == "__main__":
```

### Comparing `multigifview-0.2.7/multigifview/core.py` & `multigifview-0.2.8/multigifview/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from Qt.QtCore import QSize
 from Qt.QtCore import Qt as QtCoreQt
 
 
 class MultiGifView(QMainWindow, Ui_MainWindow):
     """A program for viewing .gif files"""
 
-    def __init__(self, filenames, *, max_columns, titles, initial_zoom=None):
+    def __init__(self, filenames, *, max_columns, titles, step, initial_zoom=None):
         super().__init__(None)
         self.setupUi(self)
 
         # extra keyboard shortcuts
         quit_shortcut = QShortcut(QKeySequence("Q"), self)
         quit_shortcut.activated.connect(QApplication.instance().quit)
         quit_shortcut = QShortcut(QKeySequence("Ctrl+Q"), self)
@@ -58,14 +58,23 @@
         set_clicked(self.zoom_in_button, self.zoom_in_action)
         set_clicked(self.zoom_reset_button, self.zoom_reset_action)
         self.zoom_box.editingFinished.connect(self.zoom_changed_action)
         self.zoom_box.setToolTip(self.zoom_changed_action.__doc__.strip())
 
         self.zoom = 100.0
 
+        # self.step sets the number of frames to change by when moving to the next
+        # frame. Defaults to 1.
+        if step < 1:
+            raise ValueError(
+                "The step passed to `-s`/`--step` must be a positive integer. Got "
+                f"{step}."
+            )
+        self.step = step
+
         if max_columns < 1:
             raise ValueError(f"Number of columns must be positive, got {max_columns}")
         n_columns = min(max_columns, len(filenames))
         self.columns = [self.column0]
         for i in range(n_columns)[1:]:
             # Create column
             column = QVBoxLayout()
@@ -108,20 +117,22 @@
             self.extra_movies.append(movie)
             self.extra_gif_widgets.append(gif_widget)
 
         # want the longest-running gif to be the one that's directly controlled, so that
         # it can play all the way to the end, not have to stop when the first movie
         # reaches its last frame
         frame_counts = [m.frameCount() for m in self.extra_movies]
-        self.total_frames = max(frame_counts)
-        ind_longest = frame_counts.index(self.total_frames)
+        # Ensure total_frames is a multiple of self.step so that when we loop between
+        # beginning/end we get the same set of frames
+        self.total_frames = max(frame_counts) - max(frame_counts) % self.step
+        ind_longest = frame_counts.index(max(frame_counts))
         self.movie = self.extra_movies.pop(ind_longest)
 
         # Set initial text for frame counter
-        self.frameCounter.setText(f"0 / {self.total_frames}")
+        self.frameCounter.setText(f"0 / {self.total_frames // self.step}")
 
         # Create actions so extra movies follow self.movie
         self.movie.frameChanged.connect(self.change_frames)
 
         if initial_zoom is not None:
             self.set_zoom(initial_zoom)
 
@@ -186,45 +197,49 @@
             self.movie.start()
 
     def previous_action(self):
         """<html><head/><body><p><b>Back one frame</b><br>
         p, left</p></body></html>
         """
         self.movie.jumpToFrame(
-            (self.movie.currentFrameNumber() - 1) % self.movie.frameCount()
+            (self.movie.currentFrameNumber() - self.step) % self.total_frames
         )
 
     def next_action(self):
         """<html><head/><body><p><b>Forward one frame</b><br>
         n, right</p></body></html>
         """
-        self.movie.jumpToNextFrame()
+        self.movie.jumpToFrame(
+            (self.movie.currentFrameNumber() + self.step) % self.total_frames
+        )
 
     def beginning_action(self):
         """<html><head/><body><p><b>Back to beginning</b><br>
         b, up</p></body></html>
         """
         self.movie.jumpToFrame(0)
 
     def end_action(self):
         """<html><head/><body><p><b>Forward to end</b><br>
         e, down</p></body></html>
         """
-        self.movie.jumpToFrame(self.movie.frameCount() - 1)
+        self.movie.jumpToFrame(self.total_frames - 1)
 
     def quit_action(self):
         """<html><head/><body><p><b>Quit</b><br>
         q, Ctrl-q, Ctrl-w, Ctrl-x</p></body></html>
         """
         QApplication.instance().quit
 
     def change_frames(self, new_frame):
         """Change all the frames in step"""
         # Update text in frame counter
-        self.frameCounter.setText(f"{new_frame} / {self.total_frames}")
+        self.frameCounter.setText(
+            f"{new_frame // self.step} / {self.total_frames // self.step}"
+        )
 
         for movie in self.extra_movies:
             length = movie.frameCount()
             if new_frame < length:
                 movie.jumpToFrame(new_frame)
             else:
                 movie.jumpToFrame(length - 1)
@@ -245,23 +260,23 @@
         self.zoom_box.setText(str(int(round(self.zoom))))
 
         current_frame = self.movie.currentFrameNumber()
         scale_factor = self.zoom / 100.0
 
         self.movie.setScaledSize(
             QSize(
-                scale_factor * self.movie.unscaled_width,
-                scale_factor * self.movie.unscaled_height,
+                round(scale_factor * self.movie.unscaled_width),
+                round(scale_factor * self.movie.unscaled_height),
             )
         )
         for movie in self.extra_movies:
             movie.setScaledSize(
                 QSize(
-                    scale_factor * movie.unscaled_width,
-                    scale_factor * movie.unscaled_height,
+                    round(scale_factor * movie.unscaled_width),
+                    round(scale_factor * movie.unscaled_height),
                 )
             )
 
         # change frame to make the image re-draw
         self.movie.jumpToFrame(0 if current_frame > 0 else 1)
         self.movie.jumpToFrame(current_frame)
```

### Comparing `multigifview-0.2.7/multigifview/mainwindow.py` & `multigifview-0.2.8/multigifview/mainwindow.py`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/multigifview.egg-info/PKG-INFO` & `multigifview-0.2.8/multigifview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multigifview
-Version: 0.2.7
+Version: 0.2.8
 Summary: View multiple gif files
 Home-page: https://github.com/johnomotani/multigifview
 Author: John Omotani
 Author-email: john.omotani@ukaea.uk
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
```

### Comparing `multigifview-0.2.7/multigifview.egg-info/SOURCES.txt` & `multigifview-0.2.8/multigifview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/qtdesignerfiles/mainwindow.ui` & `multigifview-0.2.8/qtdesignerfiles/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `multigifview-0.2.7/setup.cfg` & `multigifview-0.2.8/setup.cfg`

 * *Files identical despite different names*


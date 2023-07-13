# Comparing `tmp/sd_prompt_reader-1.3.2.post2.tar.gz` & `tmp/sd_prompt_reader-1.3.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_prompt_reader-1.3.2.post2.tar", max compression
+gzip compressed data, was "sd_prompt_reader-1.3.2.post3.tar", max compression
```

## Comparing `sd_prompt_reader-1.3.2.post2.tar` & `sd_prompt_reader-1.3.2.post3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1066 2023-04-09 14:16:43.184257 sd_prompt_reader-1.3.2.post2/LICENSE
--rw-r--r--   0        0        0    10121 2023-07-11 19:57:13.658064 sd_prompt_reader-1.3.2.post2/README.md
--rw-r--r--   0        0        0     1315 2023-07-11 19:59:40.364474 sd_prompt_reader-1.3.2.post2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-09 15:23:08.438879 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/.DS_Store
--rw-r--r--   0        0        0      144 2023-05-23 18:26:36.425241 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/__init__.py
--rw-r--r--   0        0        0       18 2023-07-08 12:39:03.680219 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/__version__.py
--rw-r--r--   0        0        0    38697 2023-07-08 12:39:03.680936 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/app.py
--rw-r--r--   0        0        0     4783 2023-05-27 18:27:20.241032 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/button.py
--rw-r--r--   0        0        0     4564 2023-07-11 19:08:57.263868 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/constants.py
--rw-r--r--   0        0        0     6256 2023-05-23 18:26:36.427298 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/ctk_tooltip.py
--rw-r--r--   0        0        0      399 2023-05-23 18:26:36.427755 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/ctkdnd.py
--rw-r--r--   0        0        0    26318 2023-07-08 12:39:03.681961 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/image_data_reader.py
--rw-r--r--   0        0        0     5465 2023-05-23 18:41:27.184337 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/parameter_viewer.py
--rw-r--r--   0        0        0     6148 2023-05-24 22:13:15.896086 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/.DS_Store
--rw-r--r--   0        0        0      144 2023-07-11 19:08:57.264228 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/__init__.py
--rw-r--r--   0        0        0      334 2023-07-11 17:12:14.136304 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3239 2023-07-11 19:08:57.264493 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/check_circle_24.png
--rw-r--r--   0        0        0     2076 2023-07-11 19:08:57.264800 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/check_circle_24_alpha.png
--rw-r--r--   0        0        0     1293 2023-07-11 19:08:57.265065 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/cleaning_services_24.png
--rw-r--r--   0        0        0     1036 2023-07-11 19:08:57.265362 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/cleaning_services_24_alpha.png
--rw-r--r--   0        0        0      602 2023-07-11 19:08:57.265675 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_20.png
--rw-r--r--   0        0        0      550 2023-07-11 19:08:57.265918 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_20_alpha.png
--rw-r--r--   0        0        0      739 2023-07-11 19:08:57.266148 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_24.png
--rw-r--r--   0        0        0      621 2023-07-11 19:08:57.266360 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_24_alpha.png
--rw-r--r--   0        0        0      751 2023-07-11 19:08:57.266701 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/description_24.png
--rw-r--r--   0        0        0      637 2023-07-11 19:08:57.266948 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/description_24_alpha.png
--rw-r--r--   0        0        0     1226 2023-07-11 19:08:57.267176 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_24.png
--rw-r--r--   0        0        0      905 2023-07-11 19:08:57.267391 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_24_alpha.png
--rw-r--r--   0        0        0     2016 2023-07-11 19:08:57.267672 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_off_24.png
--rw-r--r--   0        0        0     1368 2023-07-11 19:08:57.267885 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_off_24_alpha.png
--rw-r--r--   0        0        0     3062 2023-07-11 19:08:57.268109 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/error_24.png
--rw-r--r--   0        0        0     1964 2023-07-11 19:08:57.268350 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/error_24_alpha.png
--rw-r--r--   0        0        0      589 2023-07-11 19:08:57.268575 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/expand_more_24.png
--rw-r--r--   0        0        0      585 2023-07-11 19:08:57.268797 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/expand_more_24_alpha.png
--rw-r--r--   0        0        0     4510 2023-07-11 19:08:57.269090 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/gray.json
--rw-r--r--   0        0        0  1377264 2023-07-11 19:08:57.272293 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/icon.icns
--rw-r--r--   0        0        0   612157 2023-07-11 19:08:57.275238 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/icon.ico
--rw-r--r--   0        0        0   810239 2023-07-11 19:08:57.277029 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/icon.png
--rw-r--r--   0        0        0     3042 2023-07-11 19:08:57.277848 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/info_24.png
--rw-r--r--   0        0        0     1966 2023-07-11 19:08:57.278399 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/info_24_alpha.png
--rw-r--r--   0        0        0     1683 2023-07-11 19:08:57.278742 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/lightbulb_20.png
--rw-r--r--   0        0        0     1453 2023-07-11 19:08:57.278984 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/lightbulb_20_alpha.png
--rw-r--r--   0        0        0     1426 2023-07-11 19:08:57.279266 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/mop_24.png
--rw-r--r--   0        0        0     1109 2023-07-11 19:08:57.279480 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/mop_24_alpha.png
--rw-r--r--   0        0        0     1740 2023-07-11 19:08:57.279698 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/place_item_48.png
--rw-r--r--   0        0        0     1334 2023-07-11 19:08:57.279912 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/place_item_48_alpha.png
--rw-r--r--   0        0        0     1241 2023-07-11 19:08:57.280112 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/save_24.png
--rw-r--r--   0        0        0      946 2023-07-11 19:08:57.280306 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/save_24_alpha.png
--rw-r--r--   0        0        0     1619 2023-07-11 19:08:57.280516 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/sort_by_alpha_20.png
--rw-r--r--   0        0        0     1377 2023-07-11 19:08:57.280727 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png
--rw-r--r--   0        0        0     2732 2023-07-11 19:08:57.281015 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/update_24.png
--rw-r--r--   0        0        0     1937 2023-07-11 19:08:57.281230 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/update_24_alpha.png
--rw-r--r--   0        0        0     2258 2023-07-11 19:08:57.281426 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/warning_24.png
--rw-r--r--   0        0        0     1658 2023-07-11 19:08:57.281645 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/warning_24_alpha.png
--rw-r--r--   0        0        0     3021 2023-06-22 18:31:25.212601 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/status_bar.py
--rw-r--r--   0        0        0     4112 2023-05-25 14:00:16.911110 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/textbox.py
--rw-r--r--   0        0        0     1224 2023-05-23 18:26:36.430070 sd_prompt_reader-1.3.2.post2/sd_prompt_reader/update_checker.py
--rw-r--r--   0        0        0    11502 1970-01-01 00:00:00.000000 sd_prompt_reader-1.3.2.post2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-09 14:16:43.184257 sd_prompt_reader-1.3.2.post3/LICENSE
+-rw-r--r--   0        0        0    10121 2023-07-13 12:18:51.987624 sd_prompt_reader-1.3.2.post3/README.md
+-rw-r--r--   0        0        0     1315 2023-07-13 14:48:19.456471 sd_prompt_reader-1.3.2.post3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-09 15:23:08.438879 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/.DS_Store
+-rw-r--r--   0        0        0      144 2023-05-23 18:26:36.425241 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-13 14:30:25.872232 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/__version__.py
+-rw-r--r--   0        0        0    38697 2023-07-13 12:25:14.209944 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/app.py
+-rw-r--r--   0        0        0     4783 2023-05-27 18:27:20.241032 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/button.py
+-rw-r--r--   0        0        0     4564 2023-07-11 19:08:57.263868 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/constants.py
+-rw-r--r--   0        0        0     6256 2023-05-23 18:26:36.427298 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/ctk_tooltip.py
+-rw-r--r--   0        0        0      399 2023-05-23 18:26:36.427755 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/ctkdnd.py
+-rw-r--r--   0        0        0    26310 2023-07-13 13:35:33.409125 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/image_data_reader.py
+-rw-r--r--   0        0        0     5465 2023-05-23 18:41:27.184337 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/parameter_viewer.py
+-rw-r--r--   0        0        0     6148 2023-05-24 22:13:15.896086 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/.DS_Store
+-rw-r--r--   0        0        0      144 2023-07-11 19:08:57.264228 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-13 12:21:42.956440 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3239 2023-07-11 19:08:57.264493 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/check_circle_24.png
+-rw-r--r--   0        0        0     2076 2023-07-11 19:08:57.264800 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/check_circle_24_alpha.png
+-rw-r--r--   0        0        0     1293 2023-07-11 19:08:57.265065 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/cleaning_services_24.png
+-rw-r--r--   0        0        0     1036 2023-07-11 19:08:57.265362 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/cleaning_services_24_alpha.png
+-rw-r--r--   0        0        0      602 2023-07-11 19:08:57.265675 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_20.png
+-rw-r--r--   0        0        0      550 2023-07-11 19:08:57.265918 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_20_alpha.png
+-rw-r--r--   0        0        0      739 2023-07-11 19:08:57.266148 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_24.png
+-rw-r--r--   0        0        0      621 2023-07-11 19:08:57.266360 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_24_alpha.png
+-rw-r--r--   0        0        0      751 2023-07-11 19:08:57.266701 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/description_24.png
+-rw-r--r--   0        0        0      637 2023-07-11 19:08:57.266948 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/description_24_alpha.png
+-rw-r--r--   0        0        0     1226 2023-07-11 19:08:57.267176 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_24.png
+-rw-r--r--   0        0        0      905 2023-07-11 19:08:57.267391 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_24_alpha.png
+-rw-r--r--   0        0        0     2016 2023-07-11 19:08:57.267672 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_off_24.png
+-rw-r--r--   0        0        0     1368 2023-07-11 19:08:57.267885 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_off_24_alpha.png
+-rw-r--r--   0        0        0     3062 2023-07-11 19:08:57.268109 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/error_24.png
+-rw-r--r--   0        0        0     1964 2023-07-11 19:08:57.268350 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/error_24_alpha.png
+-rw-r--r--   0        0        0      589 2023-07-11 19:08:57.268575 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/expand_more_24.png
+-rw-r--r--   0        0        0      585 2023-07-11 19:08:57.268797 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/expand_more_24_alpha.png
+-rw-r--r--   0        0        0     4510 2023-07-11 19:08:57.269090 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/gray.json
+-rw-r--r--   0        0        0  1377264 2023-07-11 19:08:57.272293 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/icon.icns
+-rw-r--r--   0        0        0   612157 2023-07-11 19:08:57.275238 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/icon.ico
+-rw-r--r--   0        0        0   810239 2023-07-11 19:08:57.277029 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/icon.png
+-rw-r--r--   0        0        0     3042 2023-07-11 19:08:57.277848 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/info_24.png
+-rw-r--r--   0        0        0     1966 2023-07-11 19:08:57.278399 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/info_24_alpha.png
+-rw-r--r--   0        0        0     1683 2023-07-11 19:08:57.278742 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/lightbulb_20.png
+-rw-r--r--   0        0        0     1453 2023-07-11 19:08:57.278984 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/lightbulb_20_alpha.png
+-rw-r--r--   0        0        0     1426 2023-07-11 19:08:57.279266 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/mop_24.png
+-rw-r--r--   0        0        0     1109 2023-07-11 19:08:57.279480 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/mop_24_alpha.png
+-rw-r--r--   0        0        0     1740 2023-07-11 19:08:57.279698 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/place_item_48.png
+-rw-r--r--   0        0        0     1334 2023-07-11 19:08:57.279912 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/place_item_48_alpha.png
+-rw-r--r--   0        0        0     1241 2023-07-11 19:08:57.280112 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/save_24.png
+-rw-r--r--   0        0        0      946 2023-07-11 19:08:57.280306 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/save_24_alpha.png
+-rw-r--r--   0        0        0     1619 2023-07-11 19:08:57.280516 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/sort_by_alpha_20.png
+-rw-r--r--   0        0        0     1377 2023-07-11 19:08:57.280727 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png
+-rw-r--r--   0        0        0     2732 2023-07-11 19:08:57.281015 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/update_24.png
+-rw-r--r--   0        0        0     1937 2023-07-11 19:08:57.281230 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/update_24_alpha.png
+-rw-r--r--   0        0        0     2258 2023-07-11 19:08:57.281426 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/warning_24.png
+-rw-r--r--   0        0        0     1658 2023-07-11 19:08:57.281645 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/warning_24_alpha.png
+-rw-r--r--   0        0        0     3021 2023-06-22 18:31:25.212601 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/status_bar.py
+-rw-r--r--   0        0        0     4112 2023-05-25 14:00:16.911110 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/textbox.py
+-rw-r--r--   0        0        0     1224 2023-05-23 18:26:36.430070 sd_prompt_reader-1.3.2.post3/sd_prompt_reader/update_checker.py
+-rw-r--r--   0        0        0    11502 1970-01-01 00:00:00.000000 sd_prompt_reader-1.3.2.post3/PKG-INFO
```

### Comparing `sd_prompt_reader-1.3.2.post2/LICENSE` & `sd_prompt_reader-1.3.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/README.md` & `sd_prompt_reader-1.3.2.post3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     <a href="#features">Features</a> •
     <a href="#supported-formats">Supported Formats</a> •
     <a href="#download">Download</a> •
     <a href="#usage">Usage</a> •
     <a href="#faq">FAQ</a> •
     <a href="#credits">Credits</a>
   </p>
-    <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v130.png">
+    <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v132.png">
 </div>
 
 ## Features
 - Support macOS, Windows and Linux.
 - Simple drag and drop interaction.
 - Copy prompt to clipboard.
 - Remove prompt from image.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 [ç®ä½ä¸­æ](https://github.com/receyuki/stable-diffusion-prompt-reader/blob/
    master/README.zh-Hans.md) | [English](https://github.com/receyuki/stable-
  diffusion-prompt-reader/blob/master/README.md) A simple standalone viewer for
    reading prompt from Stable Diffusion generated image outside the webui.
    Features â¢ Supported_Formats â¢ Download â¢ Usage â¢ FAQ â¢ Credits
 [https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
-                             screenshot_v130.png]
+                             screenshot_v132.png]
 ## Features - Support macOS, Windows and Linux. - Simple drag and drop
 interaction. - Copy prompt to clipboard. - Remove prompt from image. - Export
 prompt to text file. - Edit or import prompt to images - Vertical orientation
 display and sorting by alphabet - Detect generation tool. - Multiple formats
 support. - Dark and light mode support. ## Supported Formats | | PNG | JPEG |
 WEBP | TXT* | |----------------|:---:|:----:|:----:|:----:| | A1111's webUI |
 â | â | â | â | | Easy Diffusion | â | â | â | | | InvokeAI | â
```

### Comparing `sd_prompt_reader-1.3.2.post2/pyproject.toml` & `sd_prompt_reader-1.3.2.post3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sd-prompt-reader"
-version = "1.3.2.post2"
+version = "1.3.2.post3"
 description = "A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui."
 authors = ["receyuki <receyuki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/receyuki/stable-diffusion-prompt-reader"
 repository = "https://github.com/receyuki/stable-diffusion-prompt-reader"
 documentation = "https://github.com/receyuki/stable-diffusion-prompt-reader"
```

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/.DS_Store` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/.DS_Store`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/app.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/app.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/button.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/button.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/constants.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/constants.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/ctk_tooltip.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/image_data_reader.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/image_data_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
                     self._nai_png()
                 # comfyui format
                 elif "prompt" in self._info:
                     self._tool = "ComfyUI"
                     self._comfy_png()
                 # drawthings format
                 elif "XML:com.adobe.xmp" in self._info:
-                    self._tool = "Draw Things"
                     self._dt_format()
             elif f.format == "JPEG" or f.format == "WEBP":
                 try:
                     exif = piexif.load(self._info.get("exif")) or {}
                     self._raw = piexif.helper.UserComment.load(exif.get("Exif").get(piexif.ExifIFD.UserComment))
                 except TypeError:
                     print("empty jpeg")
@@ -316,14 +315,15 @@
         try:
             data = minidom.parseString(self._info.get("XML:com.adobe.xmp"))
             data_json = json.loads(data.getElementsByTagName("exif:UserComment")[0]
                                    .childNodes[1].childNodes[1].childNodes[0].data)
         except:
             print("Draw things format error")
         else:
+            self._tool = "Draw Things"
             self._positive = data_json.get("c")
             self._negative = data_json.get("uc")
             self._raw = "\n".join([self._positive, self._negative, str(data_json)])
             data_json.pop("c")
             data_json.pop("uc")
             self._setting = self.remove_quotes(str(data_json)[1:-1])
```

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/parameter_viewer.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/parameter_viewer.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/.DS_Store` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/.DS_Store`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/check_circle_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/check_circle_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/check_circle_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/check_circle_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/cleaning_services_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/cleaning_services_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/cleaning_services_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/cleaning_services_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_20.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_20_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/content_copy_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/content_copy_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/description_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/description_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/description_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/description_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_off_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_off_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/edit_off_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/edit_off_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/error_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/error_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/error_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/error_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/expand_more_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/expand_more_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/expand_more_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/expand_more_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/gray.json` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/gray.json`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/icon.icns` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/icon.icns`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/icon.ico` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/icon.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/icon.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/info_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/info_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/info_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/info_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/lightbulb_20.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/lightbulb_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/lightbulb_20_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/lightbulb_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/mop_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/mop_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/mop_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/mop_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/place_item_48.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/place_item_48.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/place_item_48_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/place_item_48_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/save_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/save_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/save_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/save_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/sort_by_alpha_20.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/sort_by_alpha_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/update_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/update_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/update_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/update_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/warning_24.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/warning_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/resources/warning_24_alpha.png` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/resources/warning_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/status_bar.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/status_bar.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/textbox.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/textbox.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/sd_prompt_reader/update_checker.py` & `sd_prompt_reader-1.3.2.post3/sd_prompt_reader/update_checker.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.2.post2/PKG-INFO` & `sd_prompt_reader-1.3.2.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-prompt-reader
-Version: 1.3.2.post2
+Version: 1.3.2.post3
 Summary: A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui.
 Home-page: https://github.com/receyuki/stable-diffusion-prompt-reader
 License: MIT
 Author: receyuki
 Author-email: receyuki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -49,15 +49,15 @@
     <a href="#features">Features</a> •
     <a href="#supported-formats">Supported Formats</a> •
     <a href="#download">Download</a> •
     <a href="#usage">Usage</a> •
     <a href="#faq">FAQ</a> •
     <a href="#credits">Credits</a>
   </p>
-    <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v130.png">
+    <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v132.png">
 </div>
 
 ## Features
 - Support macOS, Windows and Linux.
 - Simple drag and drop interaction.
 - Copy prompt to clipboard.
 - Remove prompt from image.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sd-prompt-reader Version: 1.3.2.post2 Summary: A
+Metadata-Version: 2.1 Name: sd-prompt-reader Version: 1.3.2.post3 Summary: A
 simple standalone viewer for reading prompt from Stable Diffusion generated
 image outside the webui. Home-page: https://github.com/receyuki/stable-
 diffusion-prompt-reader License: MIT Author: receyuki Author-email:
 receyuki@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,15 @@
 
 [ç®ä½ä¸­æ](https://github.com/receyuki/stable-diffusion-prompt-reader/blob/
    master/README.zh-Hans.md) | [English](https://github.com/receyuki/stable-
  diffusion-prompt-reader/blob/master/README.md) A simple standalone viewer for
    reading prompt from Stable Diffusion generated image outside the webui.
    Features â¢ Supported_Formats â¢ Download â¢ Usage â¢ FAQ â¢ Credits
 [https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
-                             screenshot_v130.png]
+                             screenshot_v132.png]
 ## Features - Support macOS, Windows and Linux. - Simple drag and drop
 interaction. - Copy prompt to clipboard. - Remove prompt from image. - Export
 prompt to text file. - Edit or import prompt to images - Vertical orientation
 display and sorting by alphabet - Detect generation tool. - Multiple formats
 support. - Dark and light mode support. ## Supported Formats | | PNG | JPEG |
 WEBP | TXT* | |----------------|:---:|:----:|:----:|:----:| | A1111's webUI |
 â | â | â | â | | Easy Diffusion | â | â | â | | | InvokeAI | â
```


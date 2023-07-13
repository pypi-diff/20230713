# Comparing `tmp/media-processing-lib-0.61.tar.gz` & `tmp/media-processing-lib-0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media-processing-lib-0.61.tar", last modified: Wed Jan 11 08:56:42 2023, max compression
+gzip compressed data, was "media-processing-lib-0.62.tar", last modified: Thu Jul 13 11:33:19 2023, max compression
```

## Comparing `media-processing-lib-0.61.tar` & `media-processing-lib-0.62.tar`

### file list

```diff
@@ -1,106 +1,97 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2022-01-11 12:02:48.000000 media-processing-lib-0.61/LICENSE.TXT
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2022-07-06 05:52:12.000000 media-processing-lib-0.61/MANIFEST.in
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      482 2023-01-11 08:56:42.287435 media-processing-lib-0.61/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      161 2021-01-03 08:03:04.000000 media-processing-lib-0.61/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.275435 media-processing-lib-0.61/media_processing_lib/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2020-11-06 12:18:35.000000 media-processing-lib-0.61/media_processing_lib/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.275435 media-processing-lib-0.61/media_processing_lib/audio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2022-07-06 07:05:04.000000 media-processing-lib-0.61/media_processing_lib/audio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1169 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/audio/audio_reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/audio/audio_resample.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      669 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/audio/audio_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.275435 media-processing-lib-0.61/media_processing_lib/audio/libs/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2021-05-20 08:20:07.000000 media-processing-lib-0.61/media_processing_lib/audio/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.275435 media-processing-lib-0.61/media_processing_lib/audio/libs/librosa/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2022-07-06 06:39:54.000000 media-processing-lib-0.61/media_processing_lib/audio/libs/librosa/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      375 2022-07-06 06:40:22.000000 media-processing-lib-0.61/media_processing_lib/audio/libs/librosa/reader.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.275435 media-processing-lib-0.61/media_processing_lib/audio/libs/soundfile/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2022-07-06 06:39:59.000000 media-processing-lib-0.61/media_processing_lib/audio/libs/soundfile/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      311 2022-07-06 07:19:31.000000 media-processing-lib-0.61/media_processing_lib/audio/libs/soundfile/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.279435 media-processing-lib-0.61/media_processing_lib/audio/melspectrogram/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       59 2022-07-06 06:41:28.000000 media-processing-lib-0.61/media_processing_lib/audio/melspectrogram/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3384 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/audio/melspectrogram/melspectrogram.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3457 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/audio/mpl_audio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1706 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/audio/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.279435 media-processing-lib-0.61/media_processing_lib/collage_maker/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2022-07-06 07:15:25.000000 media-processing-lib-0.61/media_processing_lib/collage_maker/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4785 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/collage_maker/collage_maker.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2725 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/collage_maker/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.279435 media-processing-lib-0.61/media_processing_lib/image/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      167 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1333 2022-10-03 06:57:42.000000 media-processing-lib-0.61/media_processing_lib/image/image_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1319 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/image_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.279435 media-processing-lib-0.61/media_processing_lib/image/libs/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2021-05-20 08:19:55.000000 media-processing-lib-0.61/media_processing_lib/image/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.279435 media-processing-lib-0.61/media_processing_lib/image/libs/lycon/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2022-07-06 06:56:19.000000 media-processing-lib-0.61/media_processing_lib/image/libs/lycon/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      203 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/lycon/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1192 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/lycon/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      243 2022-07-06 06:55:32.000000 media-processing-lib-0.61/media_processing_lib/image/libs/lycon/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.279435 media-processing-lib-0.61/media_processing_lib/image/libs/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      363 2023-01-11 08:54:47.000000 media-processing-lib-0.61/media_processing_lib/image/libs/opencv/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/opencv/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      272 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/opencv/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.283435 media-processing-lib-0.61/media_processing_lib/image/libs/pil/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2022-07-06 06:55:07.000000 media-processing-lib-0.61/media_processing_lib/image/libs/pil/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      217 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/pil/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      782 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/pil/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      262 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/pil/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.283435 media-processing-lib-0.61/media_processing_lib/image/libs/skimage/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/skimage/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/skimage/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/skimage/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/libs/skimage/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.283435 media-processing-lib-0.61/media_processing_lib/image/resize/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2022-07-06 06:56:43.000000 media-processing-lib-0.61/media_processing_lib/image/resize/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4318 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/resize/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2197 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/resize/resize_black_bars.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1434 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/resize/resize_stretch.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.283435 media-processing-lib-0.61/media_processing_lib/image/utils/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/utils/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2023-01-11 08:54:47.000000 media-processing-lib-0.61/media_processing_lib/image/utils/text.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1443 2023-01-11 08:54:47.000000 media-processing-lib-0.61/media_processing_lib/image/utils/title.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1033 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/utils/to_image.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      818 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/image/utils/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2479 2021-11-12 12:30:12.000000 media-processing-lib-0.61/media_processing_lib/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      781 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/media_processing_lib/video/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/media_processing_lib/video/libs/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2021-01-02 03:36:03.000000 media-processing-lib-0.61/media_processing_lib/video/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/media_processing_lib/video/libs/imageio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/libs/imageio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      377 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/libs/imageio/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/media_processing_lib/video/libs/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/libs/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      526 2022-07-16 00:32:37.000000 media-processing-lib-0.61/media_processing_lib/video/libs/opencv/writer.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4847 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/mpl_video.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1848 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/mpl_video_apply.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/media_processing_lib/video/reader/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      392 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/reader/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1642 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/reader/decord.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2215 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/reader/imageio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1753 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/reader/images_path.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      995 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/reader/mpl_video_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1724 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/reader/numpy_path.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2121 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/reader/opencv.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1405 2022-07-20 12:52:44.000000 media-processing-lib-0.61/media_processing_lib/video/reader/pims.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1057 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/reader/raw_data.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2943 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/utils.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      805 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/video_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      696 2022-12-08 09:18:26.000000 media-processing-lib-0.61/media_processing_lib/video/video_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.275435 media-processing-lib-0.61/media_processing_lib.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      482 2023-01-11 08:56:42.000000 media-processing-lib-0.61/media_processing_lib.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3455 2023-01-11 08:56:42.000000 media-processing-lib-0.61/media_processing_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-01-11 08:56:42.000000 media-processing-lib-0.61/media_processing_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      126 2023-01-11 08:56:42.000000 media-processing-lib-0.61/media_processing_lib.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2023-01-11 08:56:42.000000 media-processing-lib-0.61/media_processing_lib.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      126 2022-07-20 12:52:44.000000 media-processing-lib-0.61/requirements.txt
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/resources/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2022-02-03 13:25:22.000000 media-processing-lib-0.61/resources/OpenSans-Bold.ttf
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2023-01-11 08:56:42.287435 media-processing-lib-0.61/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1784 2023-01-11 08:56:39.000000 media-processing-lib-0.61/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-11 08:56:42.287435 media-processing-lib-0.61/test/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      996 2022-07-16 00:32:37.000000 media-processing-lib-0.61/test/test_collage_maker.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2023-03-26 06:25:47.000000 media-processing-lib-0.62/LICENSE.TXT
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2023-03-26 06:25:47.000000 media-processing-lib-0.62/MANIFEST.in
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2023-07-13 11:33:19.511968 media-processing-lib-0.62/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2023-03-26 06:25:47.000000 media-processing-lib-0.62/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.503968 media-processing-lib-0.62/media_processing_lib/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1166 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/audio_reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/audio_resample.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      646 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/audio_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/libs/librosa/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/librosa/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      376 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/librosa/reader.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/libs/soundfile/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/soundfile/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/soundfile/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       59 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3397 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/melspectrogram.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3488 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/mpl_audio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2457 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/collage_maker/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/collage_maker/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5034 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/collage_maker/collage_maker.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3951 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/collage_maker/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      167 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      704 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/image/image_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      636 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/image_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      418 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      260 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/pil/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      443 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1359 2023-05-01 06:22:34.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      263 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/resize/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     3677 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2199 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/resize_black_bars.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1435 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/resize_stretch.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/utils/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/utils/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/utils/text.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1473 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/utils/title.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1030 2023-05-28 19:19:53.000000 media-processing-lib-0.62/media_processing_lib/image/utils/to_image.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2916 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/image/utils/utils.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3281 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      495 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/video/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/backends/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      436 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1712 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/decord.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4140 2023-05-28 19:58:05.000000 media-processing-lib-0.62/media_processing_lib/video/backends/disk_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2017 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/imageio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      984 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/backends/memory_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1101 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/backends/mpl_video_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2165 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/opencv.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1526 2023-05-31 16:16:07.000000 media-processing-lib-0.62/media_processing_lib/video/backends/pims.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7220 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/mpl_video.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4125 2023-05-29 09:32:03.000000 media-processing-lib-0.62/media_processing_lib/video/utils.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      583 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/video_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      902 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/video_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/writer/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/writer/imageio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/imageio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      372 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/imageio/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/writer/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      521 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3173 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2023-05-31 15:49:33.000000 media-processing-lib-0.62/requirements.txt
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/resources/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2023-03-26 06:25:47.000000 media-processing-lib-0.62/resources/OpenSans-Bold.ttf
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2023-07-13 11:33:19.511968 media-processing-lib-0.62/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1831 2023-07-13 11:33:17.000000 media-processing-lib-0.62/setup.py
```

### Comparing `media-processing-lib-0.61/media_processing_lib/audio/audio_reader.py` & `media-processing-lib-0.62/media_processing_lib/audio/audio_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import warnings
 
 from .utils import get_wav_from_video, build_reader
 from .mpl_audio import MPLAudio
 from ..logger import logger, logging
 
 # pylint: disable=broad-except
-def audio_read(path: str, audio_lib: str = "librosa", force_wav: bool=True, **kwargs):
+def audio_read(path: str, audio_lib: str = None, force_wav: bool = True, **kwargs):
     """
     audio_read implementation from a path
     FUN FACT: Reading mp4 (videos in general?) will yield different results every time, so we can convert data to wav
         first if mp4
     """
     if logger.getEffectiveLevel() < logging.DEBUG:
         warnings.filterwarnings("ignore")
```

### Comparing `media-processing-lib-0.61/media_processing_lib/audio/audio_writer.py` & `media-processing-lib-0.62/media_processing_lib/audio/audio_writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pathlib import Path
 import numpy as np
 
 # from .utils import build_writer
 from .mpl_audio import MPLAudio
 
 # pylint: disable=import-outside-toplevel, broad-except, cyclic-import
-def audio_write(audio: Union["MPLAudio", np.ndarray, List], path: Union[str, Path],
-                audio_lib: str = "soundfile", **kwargs):
+def audio_write(audio: Union["MPLAudio", np.ndarray, List], path: Union[str, Path], audio_lib: str = None, **kwargs):
     """Audio writer implementation from a MPLAudio/numpy array or data"""
     if isinstance(audio, (np.ndarray, List)):
         assert "sample_rate" in kwargs
         sample_rate = kwargs.pop("sample_rate")
         audio = MPLAudio(audio, sample_rate)
     audio.write(path, audio_lib, **kwargs)
```

### Comparing `media-processing-lib-0.61/media_processing_lib/audio/melspectrogram/melspectrogram.py` & `media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/melspectrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,82 +9,92 @@
     "n_fft": 800,  # Extra window size is filled with 0 paddings to match this parameter
     "hop_size": 200,  # For 16000Hz, 200 = 12.5 ms (0.0125 * sample_rate)
     "win_size": 800,  # For 16000Hz, 800 = 50 ms (If None, win_size = n_fft) (0.05 * sample_rate)
     "sample_rate": 16000,  # 16000Hz (corresponding to librispeech) (sox --i <filename>)
     "frame_shift_ms": None,  # Can replace hop_size parameter. (Recommended: 12.5)
     "min_level_db": -100,
     "num_mels": 80,  # Number of mel-spectrogram channels and local conditioning dimensionality
-    "fmin": 55, # 55 male, 95 female. Pitch info: male~[65, 260], female~[100, 525])
+    "fmin": 55,  # 55 male, 95 female. Pitch info: male~[65, 260], female~[100, 525])
     "fmax": 7600,  # To be increased/reduced depending on data.
     "ref_level_db": 20,
     "signal_normalization": True,
     "allow_clipping_in_normalization": True,  # Only relevant if mel_normalization = True
     "symmetric_mels": True,
     "max_abs_value": 4.0,
     "preemphasize": True,  # whether to apply filter
     "preemphasis": 0.97,  # filter coefficient.
 }
 hp = make_dataclass("hp", list(hp.keys()))(*hp.values())
 
+
 def get_hop_size():
     """Get hop size"""
     hop_size = hp.hop_size
     if hop_size is None:
         assert hp.frame_shift_ms is not None
         hop_size = int(hp.frame_shift_ms / 1000 * hp.sample_rate)
     return hop_size
 
+
 def _stft(y):
     """sfft call"""
     # if hp.use_lws:
     # 	return _lws_processor(hp).stft(y).T
     # else:
     return librosa.stft(y=y, n_fft=hp.n_fft, hop_length=get_hop_size(), win_length=hp.win_size)
 
+
 def preemphasis(wav, k, preemphasize=True):
     """Preemphasis"""
     if preemphasize:
         return signal.lfilter([1, -k], [1], wav)
     return wav
 
+
 def _amp_to_db(x):
     """Amplitude to db"""
     min_level = np.exp(hp.min_level_db / 20 * np.log(10))
     return 20 * np.log10(np.maximum(min_level, x))
 
+
 # Conversions
 _MEL_BASIS = None
 
+
 def _linear_to_mel(spectogram):
     global _MEL_BASIS
     if _MEL_BASIS is None:
         _MEL_BASIS = _build_mel_basis()
     return np.dot(_MEL_BASIS, spectogram)
 
+
 def _build_mel_basis():
     assert hp.fmax <= hp.sample_rate // 2
-    return librosa.filters.mel(hp.sample_rate, hp.n_fft, n_mels=hp.num_mels,
-                               fmin=hp.fmin, fmax=hp.fmax)
+    return librosa.filters.mel(hp.sample_rate, hp.n_fft, n_mels=hp.num_mels, fmin=hp.fmin, fmax=hp.fmax)
 
 
 # pylint: disable=no-else-return, chained-comparison
 def _normalize(S):
     if hp.allow_clipping_in_normalization:
         if hp.symmetric_mels:
-            return np.clip((2 * hp.max_abs_value) * ((S - hp.min_level_db) / (-hp.min_level_db)) - hp.max_abs_value,
-                            -hp.max_abs_value, hp.max_abs_value)
+            return np.clip(
+                (2 * hp.max_abs_value) * ((S - hp.min_level_db) / (-hp.min_level_db)) - hp.max_abs_value,
+                -hp.max_abs_value,
+                hp.max_abs_value,
+            )
         else:
             return np.clip(hp.max_abs_value * ((S - hp.min_level_db) / (-hp.min_level_db)), 0, hp.max_abs_value)
 
     assert S.max() <= 0 and S.min() - hp.min_level_db >= 0
     if hp.symmetric_mels:
         return (2 * hp.max_abs_value) * ((S - hp.min_level_db) / (-hp.min_level_db)) - hp.max_abs_value
     else:
         return hp.max_abs_value * ((S - hp.min_level_db) / (-hp.min_level_db))
 
+
 def melspectrogram(wav):
     """The main call"""
     D = _stft(preemphasis(wav, hp.preemphasis, hp.preemphasize))
     S = _amp_to_db(_linear_to_mel(np.abs(D))) - hp.ref_level_db
 
     if hp.signal_normalization:
         return _normalize(S)
```

### Comparing `media-processing-lib-0.61/media_processing_lib/audio/mpl_audio.py` & `media-processing-lib-0.62/media_processing_lib/audio/mpl_audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from typing import Any
 from copy import copy
 import numpy as np
 
 from .audio_resample import audio_resample
 from .utils import build_writer
 
+
 class MPLAudio(ABC):
     """MPLAudio implementation"""
-    def __init__(self, data:Any, sample_rate: int):
+
+    def __init__(self, data: Any, sample_rate: int):
         self.data = data
         self.sample_rate = sample_rate
         self.shape = self.data.shape
 
     def resample(self, sample_rate: int) -> MPLAudio:
         """
         Resamples this audio object to a new sample rate
@@ -26,15 +28,15 @@
     def save(self, *args, **kwargs):
         """
         Saves the current audio to the desired path. Calls audio_write with it's desired params, such as audio_lib
         Parameters: path A path where to save this current file
         """
         self.write(*args, **kwargs)
 
-    def write(self, path: str, audio_lib: str = "soundfile", **kwargs):
+    def write(self, path: str, audio_lib: str = None, **kwargs):
         """
         Saves the current audio to the desired path. Calls audio_write with it's desired params, such as audio_lib
         Parameters: path A path where to save this current file
         """
 
         path = str(path) if not isinstance(path, str) else path
         f_write = build_writer(audio_lib)
@@ -60,16 +62,19 @@
         f_str = "[MPLAudio]"
         f_str += f"\n - Shape: {self.shape}"
         f_str += f"\n-  Sample rate: {self.sample_rate}"
         return f_str
 
     def __eq__(self, other: MPLAudio):
         # Close enough equality
-        return (self.sample_rate == other.sample_rate) and (self.shape == other.shape) \
+        return (
+            (self.sample_rate == other.sample_rate)
+            and (self.shape == other.shape)
             and np.median(np.abs(self.data - other.data)) < 1e-4
+        )
 
     # # @brief Applies a function to each frame of the self video and creates a new video with the applied function.
     # #  The callable prototype is (video, timestep) and must return a modified frame of video[timestep]
     # # @return A new video where each frame is updates according to the provided callback
     # def apply(self, applyFn:Callable[[MPLVideo, int], np.ndarray]) -> MPLVideo:
     # 	N = len(self)
     # 	firstFrame = applyFn(self, 0)
@@ -79,11 +84,12 @@
     # 		newFrame = applyFn(self, i)
     # 		newData[i] = newFrame
     # 	return MPLVideo(newData, self.fps, self.shape, self.nFrames)
     # def saveApply(self, path:str, applyFn:Callable[[MPLVideo, int], np.ndarray], **kwargs):
     # 	from .video_writer import tryWriteVideoApply
     # 	tryWriteVideoApply(self, path, applyFn, **kwargs)
 
+
 # def save_wav(wav, path, sr):
 # 	wav *= 32767 / max(0.01, np.max(np.abs(wav)))
 # 	#proposed by @dsmiller
 # 	wavfile.write(path, sr, wav.astype(np.int16))
```

### Comparing `media-processing-lib-0.61/media_processing_lib/audio/utils.py` & `media-processing-lib-0.62/media_processing_lib/audio/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,77 @@
 """Utils for audio"""
 from typing import Tuple, Set
+import os
 import tempfile
 import subprocess
 
 from .libs.soundfile import audio_write as audio_write_soundfile
 from .libs.librosa import audio_read as audio_read_librosa
 from ..logger import logger
 
+
 def build_reader(audio_lib: str):
     """Build the reader function"""
+    audio_lib = get_default_audio_read_lib() if audio_lib is None else audio_lib
     assert audio_lib in get_available_audio_libs().intersection(["librosa"])
     if audio_lib == "librosa":
         return audio_read_librosa
     return None
 
+
+def get_default_audio_read_lib():
+    """gets the default audio read lib"""
+    backend = os.getenv("MPL_AUDIO_READ_BACKEND")
+    if not backend:
+        backend = "librosa"
+        logger.debug(f"MPL_AUDIO_READ_BACKEND not set. Defaulting to '{backend}' backend")
+    return backend
+
+
 # pylint: disable=import-outside-toplevel, unused-import
 def get_available_audio_libs() -> Set[str]:
     """Returns a set with all the available audio libraries used for reading/writing"""
     res = set()
     try:
         import librosa
+
         res.add("librosa")
     except ModuleNotFoundError:
         pass
 
     try:
         import soundfile
+
         res.add("soundfile")
     except ModuleNotFoundError:
         pass
 
     if len(res) == 0:
         logger.info("Warning! No image libraries available. Use 'pip install -r requirements.txt'")
     return res
 
+
 def get_wav_from_video(path: str) -> Tuple[int, str]:
     """Given a video path, use ffmpeg under the hood to extract the audio, and return the audio fd and path."""
     fd, tmp_path = tempfile.mkstemp(suffix=".wav")
     logger.debug2(f"Extracting audio from '{path}'. Will be stored at '{tmp_path}'.")
     command = f"ffmpeg -loglevel panic -y -i {path} -strict -2 {tmp_path}"
     subprocess.call(command, shell=True)
     return fd, tmp_path
 
+
 def build_writer(audio_lib: str):
     """Builds the writer function"""
+    audio_lib = get_default_audio_write_lib() if audio_lib is None else audio_lib
     assert audio_lib in get_available_audio_libs().intersection(["soundfile"])
     if audio_lib == "soundfile":
         return audio_write_soundfile
     return None
+
+
+def get_default_audio_write_lib():
+    """gets the default audio write lib"""
+    backend = os.getenv("MPL_AUDIO_WRITE_BACKEND")
+    if not backend:
+        backend = "soundfile"
+        logger.debug(f"MPL_VIDEO_BACKEND not set. Defaulting to '{backend}' backend")
+    return backend
```

### Comparing `media-processing-lib-0.61/media_processing_lib/collage_maker/collage_maker.py` & `media-processing-lib-0.62/media_processing_lib/collage_maker/collage_maker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,106 +1,118 @@
 """Collage maker module"""
 from pathlib import Path
 from multiprocessing import Pool
-from typing import List, Callable, Tuple
+from typing import List, Callable, Tuple, Dict
 import numpy as np
 from tqdm import trange, tqdm
 
 from .utils import get_closest_square, auto_load_fn, collage_fn
 from ..image import image_write, image_resize
 from ..logger import logger
 
+
 class CollageMaker:
     """Collage maker class implementation"""
-    def __init__(self, files: List[List[Path]], plot_fns: List[Callable], output_dir: Path, \
-            load_fns: List[Callable] = None, names: List[str] = None, \
-            rows_cols: Tuple[int, int] = None, resolution: Tuple[int, int] = None,
-            n_cores: int = 0):
+
+    def __init__(
+        self,
+        files: List[List[Path]],
+        plot_fns: List[Callable],
+        output_dir: Path,
+        load_fns: List[Callable] = None,
+        resolution: Tuple[int, int] = None,
+        n_cores: int = 0,
+        collage_fn_kwargs: Dict = None,
+    ):
         assert isinstance(files, List)
         self.files = np.array([[Path(x) for x in y] for y in files])
         self.lens = [len(x) for x in self.files]
         self.output_dir = Path(output_dir)
-        self.names = names
-        self.rows_cols = get_closest_square(len(self.files)) if rows_cols is None else rows_cols
+        self.collage_fn_kwargs = collage_fn_kwargs if collage_fn_kwargs is not None else {}
+        self.titles = self.collage_fn_kwargs.get("titles", None)
+        self.rows_cols = self.collage_fn_kwargs.get("rows_cols", None)
+        if self.rows_cols is None:
+            self.rows_cols = get_closest_square(len(self.files))
         self.n_cores = n_cores
-        n_outputs = len(self.files)
 
         # Bravely assuming all items can be plotted the same
+        n_outputs = len(self.files)
         if isinstance(plot_fns, Callable):
             plot_fns = n_outputs * [plot_fns]
         self.plot_fns = plot_fns
         # Bravely assuming we can infer the load fn based on suffixes
         if load_fns is None:
             load_fns = [auto_load_fn(x[0]) for x in self.files]
         # Bravely assuming all items can be loaded the same
         if isinstance(load_fns, Callable):
             load_fns = n_outputs * [load_fns]
         self.load_fns = load_fns
 
         assert np.std(self.lens) == 0, self.lens
         assert len(self.plot_fns) == n_outputs, f"{len(self.plot_fns)} vs. {n_outputs}"
-        if self.names is not None:
-            assert len(self.names) == n_outputs, f"{len(self.names)} vs {n_outputs}"
+        if self.titles is not None:
+            assert len(self.titles) == n_outputs, f"{len(self.titles)} vs {n_outputs}"
         if self.rows_cols is not None:
-            assert self.rows_cols[0] * self.rows_cols[1] >= n_outputs, \
-                f"Rows ({self.rows_cols[0]}) * Cols ({self.rows_cols[1]}) < Outputs ({n_outputs})"
+            assert (
+                self.rows_cols[0] * self.rows_cols[1] >= n_outputs
+            ), f"Rows ({self.rows_cols[0]}) * Cols ({self.rows_cols[1]}) < Outputs ({n_outputs})"
         if resolution is None:
             resolution = self._get_resolution()
         self.resolution = resolution
 
-    def _get_resolution(self):
-        """Gets the resolution based on first iteration"""
-        this_paths = self.files[:, 0]
-        items = [load_fn(x) for load_fn, x in zip(self.load_fns, this_paths)]
-        images = [plot_fn(x) for plot_fn, x in zip(self.plot_fns, items)]
-        result = collage_fn(images, self.rows_cols, self.names)
-        return tuple(result.shape[0: 2])
-
-    @staticmethod
-    def _do_one(items):
-        in_paths, load_fns, plot_fns, out_path, rows_cols, names, resolution = items
-        if Path(out_path).exists():
-            logger.debug2(f"Out path '{out_path}' exists. Skipping.")
-            return
-        loaded_items = [load_fn(x) for load_fn, x in zip(load_fns, in_paths)]
-        images = [plot_fn(x) for plot_fn, x in zip(plot_fns, loaded_items)]
-        collage = collage_fn(images, rows_cols, names)
-        collage_resized = image_resize(collage, height=resolution[0], width=resolution[1])
-        image_write(collage_resized, out_path)
-
     def make_collage(self, start_ix: int = None, end_ix: int = None) -> np.ndarray:
         """Function that is called to create the collage"""
         start_ix = start_ix if not start_ix is None else 0
         end_ix = end_ix if not end_ix is None else len(self.files[0])
         assert start_ix < end_ix
         assert end_ix <= len(self.files[0]), f"{end_ix} vs {len(self.files[0])}"
         self.output_dir.mkdir(parents=True, exist_ok=True)
 
         items = []
         for i in range(start_ix, end_ix):
             in_paths = self.files[:, i]
             out_path = f"{self.output_dir}/{i}.png"
-            item = [in_paths, self.load_fns, self.plot_fns, out_path, self.rows_cols, self.names, self.resolution]
+            item = [in_paths, self.load_fns, self.plot_fns, out_path, self.rows_cols, self.titles, self.resolution]
             items.append(item)
 
         if self.n_cores == 0:
             _ = [CollageMaker._do_one(items[i]) for i in trange(len(items))]
         else:
             pool = Pool(min(self.n_cores, len(items)))
             pbar = tqdm(total=len(items))
             for _ in pool.imap(CollageMaker._do_one, items):
                 pbar.update()
 
+    def _get_resolution(self):
+        """Gets the resolution based on first iteration"""
+        this_paths = self.files[:, 0]
+        items = [load_fn(x) for load_fn, x in zip(self.load_fns, this_paths)]
+        images = [plot_fn(x) for plot_fn, x in zip(self.plot_fns, items)]
+        result = collage_fn(images, **self.collage_fn_kwargs)
+        return tuple(result.shape[0:2])
+
+    @staticmethod
+    def _do_one(items):
+        in_paths, load_fns, plot_fns, out_path, rows_cols, names, resolution = items
+        if Path(out_path).exists():
+            logger.debug2(f"Out path '{out_path}' exists. Skipping.")
+            return
+        loaded_items = [load_fn(x) for load_fn, x in zip(load_fns, in_paths)]
+        images = [plot_fn(x) for plot_fn, x in zip(plot_fns, loaded_items)]
+        collage = collage_fn(images, rows_cols=rows_cols, titles=names)
+        collage_resized = image_resize(collage, height=resolution[0], width=resolution[1])
+        image_write(collage_resized, out_path)
+
     def __call__(self, *args, **kwargs):
         return self.make_collage(*args, **kwargs)
 
     def __str__(self) -> str:
         f_str = "[Collage Maker]"
         f_str += f"\n - Num outputs: {len(self.files)}"
         f_str += f"\n - Rows x Cols: {self.rows_cols}"
         f_str += f"\n - Lens: {self.lens}"
         f_str += f"\n - Resolution: {self.resolution}"
-        if self.names is not None:
-            f_str += f"\n - Names: {self.names}"
+        if self.titles is not None:
+            f_str += f"\n - Names: {self.titles}"
         f_str += f"\n - Output dir: '{self.output_dir}'"
         f_str += f"\n - N cores: {self.n_cores}"
         return f_str
```

### Comparing `media-processing-lib-0.61/media_processing_lib/collage_maker/utils.py` & `media-processing-lib-0.62/media_processing_lib/collage_maker/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """Utils for collage maker"""
 from typing import Callable, Tuple, List
 from pathlib import Path
 import numpy as np
 
 from ..image import image_read, image_add_title
+from ..logger import logger
 
 def auto_load_fn(file_path: Path) -> Callable[[Path], np.ndarray]:
     """Tries to autoload a file"""
     suffix = file_path.suffix[1:]
     if suffix in ("png", "jpg"):
         return image_read
     if suffix == "npy":
         return np.load
     if suffix == "npz":
+
         def f(x):
             X = np.load(x, allow_pickle=True)["arr_0"]
             try:
                 _ = X.shape
             except Exception as _:
                 X = X.item()
             return X
+
         return f
     assert False, f"Suffix unknown: '{suffix}'. Path: '{file_path}'"
 
 def get_closest_square(N: int) -> Tuple[int, int]:
     """
-    Objective:
-
     Given a stack of N images
     Find the closest square X>=N*N and then remove rows 1 by 1 until it still fits X
 
     Example: 9: 3*3; 12 -> 3*3 -> 3*4 (3 rows). 65 -> 8*8 -> 8*9. 73 -> 8*8 -> 8*9 -> 9*9
     """
 
     x = int(np.sqrt(N))
@@ -40,35 +41,56 @@
     if c * r < N:
         c += 1
     if c * r < N:
         r += 1
     assert (c + 1) * r > N and c * (r + 1) > N
     return r, c
 
-def collage_fn(images: List[np.ndarray], rows_cols: Tuple[int, int] = None,
-               titles: List[str] = None, **kwargs) -> np.ndarray:
+def collage_fn(images: List[np.ndarray], rows_cols: Tuple[int, int] = None, pad_bottom: int = 0,
+               pad_right: int = 0, titles: List[str] = None, **kwargs,) -> np.ndarray:
     """
     Make a concatenated collage based on the desired r,c format
-    Parameters
-    images A stack of images
-    rows_cols Tuple for number of rows and columns
-    titles Titles for each image. Optional.
-    kwargs are used for image_add_title method
+    Parameters:
+    - images A stack of images
+    - rows_cols Tuple for number of rows and columns
+    - pad_bottom An integer to pad the images on top, only valid in rows [2: n_rows]. TODO: what is this measured in?
+    - pad_right An integer to pad images on right, only valid on columns [2: n_cols]. TODO: what is this measured in?
+    - titles Titles for each image. Optional.
+    - kwargs are used for image_add_title method
 
     Return: A numpy array of stacked images according to (rows, cols) inputs.
     """
+    assert len(images) > 1, "Must give at least two images to the collage"
+    if rows_cols is None:
+        rows_cols = get_closest_square(len(images))
+        logger.debug(f"row_cols was not set. Setting automatically to {rows_cols} based on number of images")
+    assert len(rows_cols) == 2, f"rows_cols must be a tuple with 2 numbers, got: {rows_cols}"
+    if np.prod(rows_cols) > len(images):
+        logger.warning(f"rows_cols: {rows_cols} greater than n images: {len(images)}. Padding with black images!")
+
     shapes = [x.shape for x in images]
-    rows_cols = get_closest_square(len(images)) if rows_cols is None else rows_cols
-    assert rows_cols[0] * rows_cols[1] >= len(images), \
-        f"Rows ({rows_cols[0]}) * Cols ({rows_cols[1]}) < Images ({len(images)})"
+    # np.pad uses [(0, 0), (0, 0), (0, 0)] to pad (a, b) on each channge of H,W,C. Our images may be H,W or H,W,C
+    # If they are H, W, C then we care about [(0, pad_bottom), (0, pad_right), (0, 0)]
+    pad = np.zeros((len(shapes[0]), 2), dtype=int)
+    pad[0, 1] = pad_bottom
+    pad[1, 1] = pad_right
+
+    if pad.sum() != 0:
+        images = [np.pad(image, pad) for image in images]
+        shapes = [x.shape for x in images]
 
     if titles is not None:
         images = [image_add_title(image, title, **kwargs) for (image, title) in zip(images, titles)]
         shapes = [x.shape for x in images]
     assert np.std(shapes, axis=0).sum() == 0, f"Shapes not equal: {shapes}"
 
     # Put all the results in a new array
     result = np.zeros((rows_cols[0] * rows_cols[1], *shapes[0]), dtype=np.uint8)
     result[0 : len(images)] = np.array(images)
     result = result.reshape((rows_cols[0], rows_cols[1], *shapes[0]))
     result = np.concatenate(np.concatenate(result, axis=1), axis=1)
+    # remove pad right from last image
+    if pad_right != 0:
+        result = result[:, 0 : result.shape[1] - pad_right]
+    if pad_bottom != 0:
+        result = result[0 : result.shape[0] - pad_bottom]
     return result
```

### Comparing `media-processing-lib-0.61/media_processing_lib/image/libs/opencv/resize.py` & `media-processing-lib-0.62/media_processing_lib/image/libs/opencv/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.61/media_processing_lib/image/libs/skimage/resize.py` & `media-processing-lib-0.62/media_processing_lib/image/libs/skimage/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.61/media_processing_lib/image/resize/resize.py` & `media-processing-lib-0.62/media_processing_lib/image/resize/resize.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 """Resize module for images"""
-from typing import Callable
 import numpy as np
 from ...logger import logger
-from ..utils import get_available_image_libs
-from ..libs.skimage import image_resize as image_resize_skimage
-from ..libs.pil import image_resize as image_resize_pil
-from ..libs.lycon import image_resize as image_resize_lycon
-from ..libs.opencv import image_resize as image_resize_opencv
+from ..utils import build_resize_fn
 from .resize_stretch import image_resize_stretch
 from .resize_black_bars import image_resize_black_bars
 
-def build_resize_fn(resize_lib) -> Callable:
-    """Builds the resize fn"""
-    assert resize_lib in get_available_image_libs(), \
-        f"Image library '{resize_lib}' not in {get_available_image_libs()}"
-    if resize_lib == "skimage":
-        return image_resize_skimage
-    if resize_lib == "lycon":
-        return image_resize_lycon
-    if resize_lib == "PIL":
-        return image_resize_pil
-    if resize_lib == "opencv":
-        return image_resize_opencv
-    return None
 
 def build_resize_mode_fn(mode):
     """builds the resize mode fn"""
     assert mode in ("stretch", "black_bars")
     if mode == "stretch":
         return image_resize_stretch
     if mode == "black_bars":
         return image_resize_black_bars
     return None
 
-def image_resize(data: np.ndarray, height: int, width: int, interpolation: str = "bilinear",
-                 mode: str = "stretch", resize_lib: str = "opencv", only_uint8: bool = True, **kwargs) -> np.ndarray:
+
+def image_resize(
+    data: np.ndarray,
+    height: int,
+    width: int,
+    interpolation: str = "bilinear",
+    mode: str = "stretch",
+    resize_lib: str = None,
+    only_uint8: bool = True,
+    **kwargs,
+) -> np.ndarray:
     """
     Image resize function
     Generic function to resize ONE 2D image of shape (H, W) or 3D of shape (H, W, D) into (height, width [, D])
     Parameters:
         data Image (or any 2D/3D array)
         height Desired resulting height
         width Desired resulting width
@@ -56,17 +47,25 @@
         assert data.dtype == np.uint8, f"Data dtype: {data.dtype}. Use only_uint8=False."
 
     f_resize_mode = build_resize_mode_fn(mode)
     f_resize = build_resize_fn(resize_lib)
     resized_data = f_resize_mode(data, height, width, interpolation, f_resize, **kwargs)
     return resized_data
 
-def image_resize_batch(data: np.ndarray, height: int, width: int, interpolation: str = "bilinear",
-                       mode: str = "stretch", resize_lib: str="opencv",
-                       only_uint8: bool = True, **kwargs) -> np.ndarray:
+
+def image_resize_batch(
+    data: np.ndarray,
+    height: int,
+    width: int,
+    interpolation: str = "bilinear",
+    mode: str = "stretch",
+    resize_lib: str = None,
+    only_uint8: bool = True,
+    **kwargs,
+) -> np.ndarray:
     """
     Batch version of image_reisze
     Generic function to resize a batch of images of shape BxHxW(xD) to a desired shape of BxdWxdH(xD)
     Paramaeters
         data batch of images (or any 2D/3D array)
         height Desired resulting height
         width Desired resulting width
@@ -76,16 +75,32 @@
         only_uint8 If true, only [0-255] images are allowed. Otherwise, let the resize_lib work the provided dtype.
     Returns: Resized batch of image.
     """
     N = len(data)
     assert N > 0
 
     # Let the img_resize infer the height/width if not provided (i.e. autosclaing for img_resize)
-    first_result = image_resize(data[0], height=height, width=width, interpolation=interpolation,
-                                mode=mode, resize_lib=resize_lib, only_uint8=only_uint8, **kwargs)
+    first_result = image_resize(
+        data[0],
+        height=height,
+        width=width,
+        interpolation=interpolation,
+        mode=mode,
+        resize_lib=resize_lib,
+        only_uint8=only_uint8,
+        **kwargs,
+    )
     new_data = np.zeros((N, *first_result.shape), dtype=data[0].dtype)
     new_data[0] = first_result
     for i in range(1, N):
-        result = image_resize(data[i], height=height, width=width, interpolation=interpolation,
-                              mode=mode, resize_lib=resize_lib, only_uint8=only_uint8, **kwargs)
+        result = image_resize(
+            data[i],
+            height=height,
+            width=width,
+            interpolation=interpolation,
+            mode=mode,
+            resize_lib=resize_lib,
+            only_uint8=only_uint8,
+            **kwargs,
+        )
         new_data[i] = result
     return new_data
```

### Comparing `media-processing-lib-0.61/media_processing_lib/image/resize/resize_black_bars.py` & `media-processing-lib-0.62/media_processing_lib/image/resize/resize_black_bars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """Resize black bars mode"""
 from typing import Callable
 import numpy as np
 
-def image_resize_black_bars(data: np.ndarray, height: int, width: int, interpolation: str,
-                            resize_fn: Callable, return_coordinates: bool=False, **kwargs) -> np.ndarray:
+
+def image_resize_black_bars(
+    data: np.ndarray,
+    height: int,
+    width: int,
+    interpolation: str,
+    resize_fn: Callable,
+    return_coordinates: bool = False,
+    **kwargs,
+) -> np.ndarray:
     """
     Resize black bars mode
     Parameters:
         data Image (or any 2D/3D array)
         height Desired resulting height
         width Desired resulting width
         interpolation Interpolation method. Valid choices are specific to the library used for the resizing.
         resize_fn The library specific resize function
         return_coordinates If true, will return the coordinates where the black bars start
     Return: The resized image and, optionally, the black bars coordinates
 
     """
     desired_shape = (height, width) if len(data.shape) == 2 else (height, width, data.shape[-1])
 
-    img_h, img_w = data.shape[0 : 2]
-    desired_h, desired_w = desired_shape[0 : 2]
+    img_h, img_w = data.shape[0:2]
+    desired_h, desired_w = desired_shape[0:2]
 
     # Find the rapports between the img_h/desired_h and img_w/desired_w
     r_h, r_w = img_h / desired_h, img_w / desired_w
 
     # Find which one is the highest, that one will be used
     max_rapp = max(r_h, r_w)
     assert max_rapp != 0, f"Cannot convert data of shape {data.shape} to ({height}, {width})"
```

### Comparing `media-processing-lib-0.61/media_processing_lib/image/resize/resize_stretch.py` & `media-processing-lib-0.62/media_processing_lib/image/resize/resize_stretch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Resize stretch mode"""
 from typing import Callable
 import numpy as np
 from ...logger import logger
 
+
 def image_resize_stretch(data: np.ndarray, height: int, width: int, interpolation: str, resize_fn: Callable, **kwargs):
     """
     Resize stretch mode
     Parameters:
         data Image (or any 2D/3D array)
         height Desired resulting height
         width Desired resulting width
```

### Comparing `media-processing-lib-0.61/media_processing_lib/image/utils/text.py` & `media-processing-lib-0.62/media_processing_lib/image/utils/text.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.61/media_processing_lib/image/utils/title.py` & `media-processing-lib-0.62/media_processing_lib/image/utils/title.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 
     # Expand the image with (left=0, top=top_padding, right=0, bottom=0)
     border = (0, top_padding, 0, 0)
     expanded_image = ImageOps.expand(pil_image, border=border, fill=background_color)
     expanded_image = np.array(expanded_image)
     text_width, text_height = draw.textsize(text, font)
     position = -text_height // 4.8, (expanded_image.shape[1] - text_width) // 2
-    return image_add_text(expanded_image, text, position, font, font_color)
+    return image_add_text(expanded_image, text=text, position=position, font=font, font_color=font_color)
```

### Comparing `media-processing-lib-0.61/media_processing_lib/image/utils/to_image.py` & `media-processing-lib-0.62/media_processing_lib/image/utils/to_image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """to image module"""
 import numpy as np
 
 def to_image(x: np.ndarray) -> np.ndarray:
     """
     To image
-    Generic NumPy to plottable image uint8 [0 : 255] image. Basically, turns the image in [0:1] and float32,
-    applies minMax, does some stuff about potential shapes being wrong, converts image to [0:255] and to uint8.
+    Generic NumPy to plottable image uint8 [0:255] image. Basically, turns the image in [0:1] and float32,
+    applies min_max, does some stuff about potential shapes being wrong, converts image to [0:255] and to uint8.
+
     Parameters:
-        x A NumPy array that is to be converted to [0 : 255] image
-    Returns: A numpy array that is the image version of the original array
+    - x A NumPy array that is to be converted to [0:255] image
 
+    Returns: A numpy array that is the image version of the original array
     """
+
     x = np.array(x)
     x = x.astype(np.float32)
     img_min, img_max = x.min(), x.max()
     x = (x - img_min) / (img_max - img_min + np.spacing(1))
     x = x.squeeze()
     if len(x.shape) == 2:
         x = np.expand_dims(x, axis=-1)
```

### Comparing `media-processing-lib-0.61/media_processing_lib/logger.py` & `media-processing-lib-0.62/media_processing_lib/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,101 @@
-"""Python logger settings."""
+"""
+Python logger settings.
+Uses ENv variables to control the log level:
+
+YOUR_KEY_LOGLEVEL=4 python blabla.py
+and logger.debug4("message")
+
+"""
 
 import os
+import sys
 import logging
-from tqdm import trange
+from colorama import Fore, Back, Style
 
 KEY = "MPL"
-logging.DEBUG2 = 3
 ENV_KEY = f"{KEY}_LOGLEVEL"
-env_var = int(os.environ[ENV_KEY]) if ENV_KEY in os.environ else 2
+# defaults to -1 (no logger!).
+env_var = int(os.environ[ENV_KEY]) if ENV_KEY in os.environ else -1
 
-# Usage: loglevel=0 (none), loglevel=1 (info), loglevel=2 (debug), loglevel=3 (debug verbose)
+# we need numbers below 5 (last logging module used number)
 logging.DEBUG2 = 3
-loglevel = {0: logging.NOTSET, 1: logging.INFO, 2: logging.DEBUG, 3: logging.DEBUG2}[env_var]
-logging.addLevelName(logging.DEBUG2, "DEBUG-VERBOSE")
-
-# instantiate logger and set log level
-logger = logging.getLogger(KEY)
-logger.setLevel(loglevel)
-logger.debug2 = lambda msg: logger.log(logging.DEBUG2, msg)
-
-class drange:
-    """Use `drange` instead of `range` and `tqdm.trange`.
-    If {Key}_TQDM is set to 1, `drange` will call `trange`, otherwise will call `range`.
-    """
-
-    def __init__(self, *args, **kwargs):
-        tqdm_key = f"{KEY}_TQDM"
-        self.env_var = bool(int(os.environ[tqdm_key])) if tqdm_key in os.environ else True
-        self.range = trange(*args, **kwargs) if self.env_var else range(*args)
-
-    def __iter__(self):
-        return self.range.__iter__()
-
-    def set_description(self, *args, **kwargs):
-        """Set description."""
-        if self.env_var:
-            self.range.set_description(*args, **kwargs)
+logging.DEBUG3 = 2
+logging.DEBUG4 = 1
+try:
+    loglevel = {
+        -1: logging.NOTSET,
+        0: logging.INFO,
+        1: logging.DEBUG,
+        2: logging.DEBUG2,
+        3: logging.DEBUG3,
+        4: logging.DEBUG4,
+    }[env_var]
+except KeyError:
+    sys.stderr.write(f"You tried to use {KEY}_LOGLEVEL={env_var}. You need to set it between -1 and 4\n")
+    sys.exit(1)
+# add the custom ones in the logger
+logging.addLevelName(logging.DEBUG2, "DGB2")
+logging.addLevelName(logging.DEBUG3, "DGB3")
+logging.addLevelName(logging.DEBUG4, "DGB4")
 
 
 class CustomFormatter(logging.Formatter):
     """Custom formatting for logger."""
 
-    yellow = "\x1b[33;20m"
-    green = "\x1b[32;20m"
-    cyan = "\x1b[36;20m"
-    red = "\x1b[31;20m"
-    bold_red = "\x1b[31;1m"
-    reset = "\x1b[0m"
-
+    reset = Style.RESET_ALL
     pre = "[%(asctime)s-%(name)s-%(levelname)s]"
     post = "(%(filename)s:%(funcName)s:%(lineno)d)"
 
-    # Example [TIME:LEVEL:NAME] Message [FILE:FUNC:LINE]
+    # Example [TIME:LEVEL:NAME] Message [FILE:FUNC:LINE]. We can update some other format here easily
     FORMATS = {
-        logging.DEBUG: f"{cyan}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.DEBUG2: f"{cyan}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.INFO: f"{green}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.WARNING: f"{yellow}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.ERROR: f"{red}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.CRITICAL: f"{bold_red}{pre}{reset} %(message)s {yellow}{post}{reset}",
+        logging.DEBUG: f"{Fore.CYAN}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.DEBUG2: f"{Fore.CYAN}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.DEBUG3: f"{Fore.MAGENTA}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.DEBUG4: f"{Back.RED}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.INFO: f"{Fore.GREEN}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.WARNING: f"{Fore.YELLOW}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.ERROR: f"{Fore.RED}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.CRITICAL: f"{Back.RED}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
     }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt)
+        formatter.formatTime = self.formatTime
         return formatter.format(record)
 
+    # here we define the time format.
+    def formatTime(self, record, datefmt=None):
+        return super().formatTime(record, "%Y%m%d %H:%M:%S")
+
+
+# instantiate logger and set log level
+
+# pylint: disable=protected-access
+def _debug2(self, message, *args, **kws):
+    if self.isEnabledFor(logging.DEBUG2):
+        self._log(logging.DEBUG2, message, args, **kws)
+
+
+# pylint: disable=protected-access
+def _debug3(self, message, *args, **kws):
+    if self.isEnabledFor(logging.DEBUG3):
+        self._log(logging.DEBUG3, message, args, **kws)
+
+
+# pylint: disable=protected-access
+def _debug4(self, message, *args, **kws):
+    if self.isEnabledFor(logging.DEBUG4):
+        self._log(logging.DEBUG4, message, args, **kws)
+
+
+logger = logging.getLogger(KEY)
+logger.setLevel(loglevel)
+logging.Logger.debug2 = _debug2
+logging.Logger.debug3 = _debug3
+logging.Logger.debug4 = _debug4
+
 # add custom formatter to logger
 handler = logging.StreamHandler()
 handler.setFormatter(CustomFormatter())
 logger.addHandler(handler)
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/libs/opencv/writer.py` & `media-processing-lib-0.62/media_processing_lib/video/writer/opencv/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """OpenCV video writer"""
 import cv2
-from ....logger import drange
+from tqdm import trange
+
 
 def video_write(video: "MPLVideo", path: str, **kwargs):
     """OpenCV video writer"""
     width, height = video.shape[2], video.shape[1]
     fourcc = kwargs["fourcc"] if "fourcc" in kwargs else "mp4v"
     writer = cv2.VideoWriter(path, cv2.VideoWriter_fourcc(*fourcc), video.fps, (width, height))
 
     N = len(video)
-    for i in drange(N, desc="[OpenCV::video_write]"):
+    for i in trange(N, desc="[OpenCV::video_write]"):
         frame = video[i]
         frame = frame[..., ::-1]
         writer.write(frame)
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/reader/decord.py` & `media-processing-lib-0.62/media_processing_lib/video/backends/imageio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,55 @@
-"""Decord video reader"""
+"""ImageIO video reader"""
 from typing import Tuple, List, Union
+import math
 from overrides import overrides
 import numpy as np
-from decord import VideoReader, cpu, gpu
+import imageio.v3 as iio
 
 from .mpl_video_backend import MPLVideoBackend, MPLFrame
 from ...logger import logger
 
 ReadReturnType = Tuple[np.ndarray, int, List[int], int]
 
-class MPLDecordBackend(MPLVideoBackend):
-    """MPLDecordBackend implementation"""
-    def __init__(self, path: str, n_frames: int = None, device: str = "cpu"):
+
+class MPLImageIOBackend(MPLVideoBackend):
+    """MPLImageIOBackend implementation"""
+
+    def __init__(self, path: str, n_frames: int = None):
         super().__init__(path)
-        assert device in ("cpu", "gpu"), f"Got {device}"
-        self.device = device
-        self._video = VideoReader(str(self.path), ctx={"cpu": cpu(), "gpu": gpu()}[device])
-        self._raw_n_frames = len(self._video)
-        self.fps = self._video.get_avg_fps()
+        self._iter_reader = iio.imiter(path, plugin="pyav")
+        self.metadata = iio.immeta(path, plugin="pyav")
 
+        self.fps = self.metadata["fps"]
+        # Accumulate all frames in this buffer
+        self._raw_data = []
+        self._raw_n_frames = math.ceil(self.metadata["duration"] * self.metadata["fps"])
         self.n_frames = self._raw_n_frames if n_frames is None else n_frames
-        assert self.n_frames <= self._raw_n_frames, \
-            f"Requested {self.n_frames}. Raw number of frames from video: {self._raw_n_frames}"
+        assert (
+            self.n_frames <= self._raw_n_frames
+        ), f"Requested {self.n_frames}. Raw number of frames from metadata: {self._raw_n_frames}"
 
         # Read all frames if none are provided. We need a better way to do this perhaps.
-        logger.debug(f"Decord MPLBackend. Path: {path}. N frames: {self.n_frames}. Raw FPS: {self.fps}. "
-                     f"Device: {self.device}")
+        logger.debug(f"ImageIO MPLBackend. Path: {path}. N frames: {self.n_frames}. FPS: {self.fps}")
 
-    @staticmethod
+    @property
     @overrides
-    def supported_formats() -> List[str]:
-        return [".mp4", ".avi", ".gif"]
+    def is_supported_format(self) -> bool:
+        return self.path.suffix in  [".mp4", ".avi", ".gif"], f"Got {self.path.suffix}"
 
     @overrides
     def __getitem__(self, key: Union[int, slice]) -> Union[MPLFrame, List[MPLFrame]]:
         assert isinstance(key, int), f"Got {type(key)}"
-        res = self._video[key].asnumpy()
-        return res
+        assert key < self.n_frames, f"Out of bounds: frame {key} >= {self.n_frames}"
+        if key < len(self._raw_data):
+            return self._raw_data[key]
+
+        n_left = key - len(self._raw_data) + 1
+        while n_left > 0:
+            new_frame = next(self._iter_reader)[..., 0:3]
+            self._raw_data.append(new_frame)
+            n_left -= 1
+        return self._raw_data[-1]
 
     @overrides
     def __len__(self) -> int:
         return self.n_frames
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/reader/imageio.py` & `media-processing-lib-0.62/media_processing_lib/video/backends/pims.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,44 @@
-"""ImageIO video reader"""
+"""PIMS video reader"""
 from typing import Tuple, List, Union
-import math
 from overrides import overrides
+import pims
 import numpy as np
-from imageio import get_reader
 
 from .mpl_video_backend import MPLVideoBackend, MPLFrame
 from ...logger import logger
 
 ReadReturnType = Tuple[np.ndarray, int, List[int], int]
 
-class MPLImageIOBackend(MPLVideoBackend):
-    """MPLImageIOBackend implementation"""
+
+class MPLPimsBackend(MPLVideoBackend):
+    """MPLPimsBackend backend implmenetation"""
 
     def __init__(self, path: str, n_frames: int = None):
         super().__init__(path)
-        self.reader = get_reader(path)
-        self.metadata = self.reader.get_meta_data()
-        self.fps = self.metadata["fps"]
-        # Accumulate all frames in this buffer
-        self._raw_data = []
-        self._raw_n_frames = math.floor(self.metadata["duration"] * self.metadata["fps"]) - 1 # TODO: more checks
-        self._iter_reader = iter(self.reader)
+        self._video = pims.Video(path)
+        self._raw_n_frames = len(self._video)
+        self.fps = self._video.frame_rate
+
         self.n_frames = self._raw_n_frames if n_frames is None else n_frames
         assert self.n_frames <= self._raw_n_frames, \
-            f"Requested {self.n_frames}. Raw number of frames from metadata: {self._raw_n_frames}"
+            f"Requested {self.n_frames}. Raw number of frames from video: {self._raw_n_frames}"
 
         # Read all frames if none are provided. We need a better way to do this perhaps.
-        logger.debug(f"ImageIO MPLBackend. Path: {path}. N frames: {self.n_frames}. FPS: {self.fps}")
+        logger.debug(f"PIMS MPLBackend. Path: {path}. N frames: {self.n_frames}. Raw FPS: {self.fps:.2f}. ")
 
-    @staticmethod
+    @property
     @overrides
-    def supported_formats() -> List[str]:
-        return [".mp4", ".avi", ".gif"]
+    def is_supported_format(self) -> bool:
+        return self.path.suffix in  [".mp4", ".avi", ".gif"], f"Got {self.path.suffix}"
 
     @overrides
     def __getitem__(self, key: Union[int, slice]) -> Union[MPLFrame, List[MPLFrame]]:
+        if isinstance(key, slice):
+            return self._video[key]
         assert isinstance(key, int), f"Got {type(key)}"
-        assert key < self.n_frames, f"Out of bounds: frame {key} >= {self.n_frames}"
-        if len(self._raw_data) > key:
-            return self._raw_data[key]
-
-        n_left = key - len(self._raw_data) + 1
-        while n_left > 0:
-            try:
-                new_frame = next(self._iter_reader)[..., 0 : 3]
-            except StopIteration:
-                logger.info(f"Got StopIteration at frame {len(self._raw_data)}")
-                self.n_frames = len(self._raw_data)
-                break
-            self._raw_data.append(new_frame)
-            n_left -= 1
-        return self[key]
+        res = np.array(self._video[key])
+        return res
 
     @overrides
     def __len__(self) -> int:
         return self.n_frames
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/reader/mpl_video_backend.py` & `media-processing-lib-0.62/media_processing_lib/video/backends/mpl_video_backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 """MPLVideo backend -- module that defines a backend suitable for MPLVideo data reader"""
 from abc import ABC, abstractmethod
-from typing import Union, List
+from typing import Union, List, overload, Optional
 from pathlib import Path
 import numpy as np
 
 MPLFrame = np.ndarray
 
+
 class MPLVideoBackend(ABC):
     """MPLVideo backend implmenetation"""
 
-    def __init__(self, path: Path):
-        self.path = Path(path)
-        assert self.path_in_supported_format
+    def __init__(self, path: Optional[Path]):
+        self.path = Path(path) if path is not None else None
+        assert self.is_supported_format, f"Path '{path}' not a supported format"
 
-    @staticmethod
+    @property
     @abstractmethod
-    def supported_formats() -> List[str]:
-        """Supported formats"""
+    def is_supported_format(self) -> bool:
+        """Returns if the path is a valid video according to this backend"""
 
     @abstractmethod
     def __len__(self) -> int:
         """Gets the length of the backend"""
 
+    @overload
+    @abstractmethod
+    def __getitem__(self, key: int) -> MPLFrame:
+        ...
+
+    @overload
+    @abstractmethod
+    def __getitem__(self, key: slice) -> List[MPLFrame]:
+        ...
+
     @abstractmethod
     def __getitem__(self, key: Union[int, slice]) -> Union[MPLFrame, List[MPLFrame]]:
         """Gets the item(s) at key"""
-
-    @property
-    def path_in_supported_format(self) -> bool:
-        """Returns if the path is a valid video according to this backend"""
-        return self.path.suffix in type(self).supported_formats(), f"Got {self.path.suffix}"
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/reader/numpy_path.py` & `media-processing-lib-0.62/media_processing_lib/video/backends/decord.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-"""MPLNumpyPathBackend video reader"""
-from functools import lru_cache
+"""Decord video reader"""
 from typing import Tuple, List, Union
-from pathlib import Path
 from overrides import overrides
 import numpy as np
-from natsort import natsorted
+from decord import VideoReader, cpu, gpu
 
 from .mpl_video_backend import MPLVideoBackend, MPLFrame
 from ...logger import logger
 
 ReadReturnType = Tuple[np.ndarray, int, List[int], int]
 
-class MPLNumpyPathBackend(MPLVideoBackend):
-    """MPLNumpyPathBackend backend implmenetation"""
 
-    def __init__(self, path: str, pattern: str = "*"):
-        self.files = [Path(x).absolute() for x in natsorted([str(x) for x in Path(path).glob(pattern)])]
-        assert len(self.files) > 0, f"Found no files in '{path}' for pattern '{pattern}'"
-        super().__init__(path)
+class MPLDecordBackend(MPLVideoBackend):
+    """MPLDecordBackend implementation"""
 
-    @staticmethod
-    @overrides
-    def supported_formats() -> List[str]:
-        return [".npy", ".npz"]
+    def __init__(self, path: str, n_frames: int = None, device: str = "cpu"):
+        super().__init__(path)
+        assert device in ("cpu", "gpu"), f"Got {device}"
+        self.device = device
+        self._video = VideoReader(str(self.path), ctx={"cpu": cpu(), "gpu": gpu()}[device])
+        self._raw_n_frames = len(self._video)
+        self.fps = self._video.get_avg_fps()
+
+        self.n_frames = self._raw_n_frames if n_frames is None else n_frames
+        assert (
+            self.n_frames <= self._raw_n_frames
+        ), f"Requested {self.n_frames}. Raw number of frames from video: {self._raw_n_frames}"
+
+        # Read all frames if none are provided. We need a better way to do this perhaps.
+        logger.debug(
+            f"Decord MPLBackend. Path: {path}. N frames: {self.n_frames}. Raw FPS: {self.fps}. "
+            f"Device: {self.device}"
+        )
 
     @property
     @overrides
-    def path_in_supported_format(self) -> bool:
-        if not self.path.is_dir():
-            logger.info(f"Expected directory, found '{self.path}'")
-            return False
-        for file in self.files:
-            if file.suffix not in self.supported_formats():
-                logger.info(f"Expected a numpy file, found '{file}'")
-                return False
-        return True
+    def is_supported_format(self) -> bool:
+        return self.path.suffix in  [".mp4", ".avi", ".gif"], f"Got {self.path.suffix}"
 
-    @lru_cache
     @overrides
     def __getitem__(self, key: Union[int, slice]) -> Union[MPLFrame, List[MPLFrame]]:
         assert isinstance(key, int), f"Got {type(key)}"
-        assert key < len(self), f"Out of bounds: frame {key} >= {len(self)}"
-        res = np.load(self.files[key])
-        if not isinstance(res, np.ndarray):
-            res = res["arr_0"]
+        res = self._video[key].asnumpy()
         return res
 
     @overrides
     def __len__(self) -> int:
-        return len(self.files)
+        return self.n_frames
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/reader/opencv.py` & `media-processing-lib-0.62/media_processing_lib/video/backends/opencv.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,36 @@
 import numpy as np
 
 from .mpl_video_backend import MPLVideoBackend, MPLFrame
 from ...logger import logger
 
 ReadReturnType = Tuple[np.ndarray, int, List[int], int]
 
+
 class MPLOpenCVBackend(MPLVideoBackend):
     """MPLOpenCVBackend backend implmenetation"""
 
     def __init__(self, path: str, n_frames: int = None):
         super().__init__(path)
         self._video = cv2.VideoCapture(str(path))
-        self._raw_n_frames =  int(self._video.get(cv2.CAP_PROP_FRAME_COUNT))
+        self._raw_n_frames = int(self._video.get(cv2.CAP_PROP_FRAME_COUNT))
         self.fps = self._video.get(cv2.CAP_PROP_FPS)
         self._raw_data = []
 
         self.n_frames = self._raw_n_frames if n_frames is None else n_frames
         assert self.n_frames <= self._raw_n_frames, \
             f"Requested {self.n_frames}. Raw number of frames from video: {self._raw_n_frames}"
 
         # Read all frames if none are provided. We need a better way to do this perhaps.
         logger.debug(f"OpenCV MPLBackend. Path: {path}. N frames: {self.n_frames}. Raw FPS: {self.fps}.")
 
-    @staticmethod
+    @property
     @overrides
-    def supported_formats() -> List[str]:
-        return [".mp4", ".avi", ".gif"]
+    def is_supported_format(self) -> bool:
+        return self.path.suffix in  [".mp4", ".avi", ".gif"], f"Got {self.path.suffix}"
 
     @overrides
     def __getitem__(self, key: Union[int, slice]) -> Union[MPLFrame, List[MPLFrame]]:
         assert isinstance(key, int), f"Got {type(key)}"
         assert key < self.n_frames, f"Out of bounds: frame {key} >= {self.n_frames}"
         if len(self._raw_data) > key:
             return self._raw_data[key]
@@ -43,15 +44,15 @@
             ret, new_frame = self._video.read()
             if not ret:
                 logger.info(f"Got None (StopIteration of OpenCV) at frame {len(self._raw_data)}")
                 self.n_frames = len(self._raw_data)
                 break
             # BGR to RGB
             new_frame = new_frame[..., ::-1]
-            new_frame = new_frame[..., 0: 3]
+            new_frame = new_frame[..., 0:3]
             self._raw_data.append(new_frame)
             n_left -= 1
         return self[key]
 
     @overrides
     def __len__(self) -> int:
         return self.n_frames
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/reader/raw_data.py` & `media-processing-lib-0.62/media_processing_lib/video/backends/memory_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,28 @@
 import numpy as np
 
 from .mpl_video_backend import MPLVideoBackend, MPLFrame
 
 ReadReturnType = Tuple[np.ndarray, int, List[int], int]
 
 # pylint: disable=super-init-not-called
-class MPLRawDataBackend(MPLVideoBackend):
+class MemoryBackend(MPLVideoBackend):
     """MPLRawData backend implmenetation"""
 
     def __init__(self, raw_data: Union[List, np.ndarray]):
+        super().__init__(None)
         assert isinstance(raw_data, (List, np.ndarray))
         assert len(raw_data) > 0
         self.raw_data = np.array(raw_data).astype(np.uint8)
         assert len(self.raw_data.shape) == 4 and self.raw_data.shape[-1] == 3
 
-    @staticmethod
-    @overrides
-    def supported_formats() -> List[str]:
-        return []
-
     @property
     @overrides
-    def path_in_supported_format(self) -> bool:
-        return False
+    def is_supported_format(self) -> bool:
+        return True
 
     @overrides
     def __getitem__(self, key: Union[int, slice]) -> Union[MPLFrame, List[MPLFrame]]:
         return self.raw_data[key]
 
     @overrides
     def __len__(self) -> int:
```

### Comparing `media-processing-lib-0.61/media_processing_lib/video/utils.py` & `media-processing-lib-0.62/media_processing_lib/video/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,136 @@
 """Generic utility file for videos"""
 from typing import Set, Callable
+from collections import OrderedDict
+import os
 from ..logger import logger
-from .reader import MPLImageIOBackend, MPLImagesPathBackend, MPLDecordBackend, MPLPimsBackend, \
-    MPLOpenCVBackend, MPLNumpyPathBackend
-from .libs.imageio import video_write as video_write_imageio
-from .libs.opencv import video_write as video_write_opencv
+from .backends import MPLImageIOBackend, DiskBackend, MPLDecordBackend, MPLPimsBackend, MPLOpenCVBackend
+from .writer.imageio import video_write as video_write_imageio
+from .writer.opencv import video_write as video_write_opencv
 
 # pylint: disable=import-outside-toplevel, unused-import
 def get_available_video_read_libs() -> Set[str]:
     """Returns a set with all the available video libraries used for reading"""
     # TODO: perhaps use importlib and make this better
     res = set()
     try:
         import decord
+
         res.add("decord")
     except ModuleNotFoundError:
         pass
 
     try:
         import pims
+
         res.add("pims")
     except ModuleNotFoundError:
         pass
 
     try:
         import cv2
+
         res.add("opencv")
     except ModuleNotFoundError:
         pass
 
     try:
         import imageio
+
         res.add("imageio")
     except ModuleNotFoundError:
         pass
 
-    res.add("images_path")
-    res.add("numpy_path")
+    res.add("disk")
 
-    if len(res) == 0:
-        logger.info("Warning! No video libraries available. Use 'pip install -r requirements.txt'")
+    if len(res) == 1:
+        logger.warning("Warning! No video libraries available. Use 'pip install -r requirements.txt'")
     return res
 
+
 # pylint: disable=import-outside-toplevel, unused-import
 def get_available_video_write_libs() -> Set[str]:
     """Returns a set with all the available video libraries used for writing"""
     # TODO: perhaps use importlib and make this better
     res = set()
     try:
         import cv2
+
         res.add("opencv")
     except ModuleNotFoundError:
         pass
 
     try:
         import imageio
+
         res.add("imageio")
     except ModuleNotFoundError:
         pass
 
     if len(res) == 0:
         logger.info("Warning! No video libraries available. Use 'pip install -r requirements.txt'")
     return res
 
-def build_video_read_fn(video_lib: str) -> Callable:
+
+def build_video_read_fn(video_lib: str) -> Callable[[int], "MPLFrame"]:
     """Builds the video read function"""
-    assert video_lib in get_available_video_read_libs()
+    video_lib = get_default_video_read_lib() if video_lib is None else video_lib
+    assert video_lib in get_available_video_read_libs(), video_lib
     if video_lib == "pims":
         return MPLPimsBackend
     if video_lib == "imageio":
         return MPLImageIOBackend
-    if video_lib == "images_path":
-        return MPLImagesPathBackend
-    if video_lib == "numpy_path":
-        return MPLNumpyPathBackend
+    if video_lib == "disk":
+        return DiskBackend
     if video_lib == "opencv":
         return MPLOpenCVBackend
     if video_lib == "decord":
         return MPLDecordBackend
     assert False, "Unknown video lib: '{video_lib}'"
 
-def build_video_write_fn(video_lib: str) -> Callable:
+
+def build_video_write_fn(video_lib: str) -> Callable[["MPLVideo", str], None]:
     """Builds the video write fn"""
-    assert video_lib in get_available_video_write_libs(), \
-        f"Video library '{video_lib}' not in '{get_available_video_write_libs()}'"
+    video_lib = get_default_video_write_lib() if video_lib is None else video_lib
+    assert (
+        video_lib in get_available_video_write_libs()
+    ), f"Video library '{video_lib}' not in '{get_available_video_write_libs()}'"
     if video_lib == "imageio":
         return video_write_imageio
     if video_lib == "opencv":
         return video_write_opencv
     assert False, f"Unknown video lib: '{video_lib}'"
 
+
 def default_frame_apply_fn(frame, _, __) -> "MPLFrame":
     """Identity function for MPLVideoApply"""
     return frame
+
+
+def get_default_video_read_lib() -> str:
+    """get the default video read lib"""
+    backend = os.getenv("MPL_VIDEO_READ_BACKEND")
+    if not backend:
+        backend = "pims"
+        logger.debug(f"MPL_VIDEO_READ_BACKEND not set. Defaulting to '{backend}' backend")
+    return backend
+
+
+def get_default_video_write_lib() -> str:
+    """get the default video write lib"""
+    backend = os.getenv("MPL_VIDEO_WRITE_BACKEND")
+    if not backend:
+        backend = "imageio"
+        logger.debug(f"MPL_VIDEO_WRITE_BACKEND not set. Defaulting to '{backend}' backend")
+    return backend
+
+class FixSizeOrderedDict(OrderedDict):
+    """Fixed sized ordered dict, nicely borrowed from: https://stackoverflow.com/a/49274421/2086583"""
+    def __init__(self, *args, max_len: int = 0, **kwargs):
+        self._max = max_len
+        super().__init__(*args, **kwargs)
+
+    def __setitem__(self, key, value):
+        OrderedDict.__setitem__(self, key, value)
+        if self._max > 0:
+            if len(self) > self._max:
+                self.popitem(False)
```

### Comparing `media-processing-lib-0.61/media_processing_lib.egg-info/SOURCES.txt` & `media-processing-lib-0.62/media_processing_lib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 media_processing_lib/collage_maker/__init__.py
 media_processing_lib/collage_maker/collage_maker.py
 media_processing_lib/collage_maker/utils.py
 media_processing_lib/image/__init__.py
 media_processing_lib/image/image_reader.py
 media_processing_lib/image/image_writer.py
 media_processing_lib/image/libs/__init__.py
-media_processing_lib/image/libs/lycon/__init__.py
-media_processing_lib/image/libs/lycon/reader.py
-media_processing_lib/image/libs/lycon/resize.py
-media_processing_lib/image/libs/lycon/writer.py
 media_processing_lib/image/libs/opencv/__init__.py
 media_processing_lib/image/libs/opencv/reader.py
 media_processing_lib/image/libs/opencv/resize.py
 media_processing_lib/image/libs/opencv/writer.py
 media_processing_lib/image/libs/pil/__init__.py
 media_processing_lib/image/libs/pil/reader.py
 media_processing_lib/image/libs/pil/resize.py
@@ -54,27 +50,24 @@
 media_processing_lib/image/utils/__init__.py
 media_processing_lib/image/utils/text.py
 media_processing_lib/image/utils/title.py
 media_processing_lib/image/utils/to_image.py
 media_processing_lib/image/utils/utils.py
 media_processing_lib/video/__init__.py
 media_processing_lib/video/mpl_video.py
-media_processing_lib/video/mpl_video_apply.py
 media_processing_lib/video/utils.py
 media_processing_lib/video/video_reader.py
 media_processing_lib/video/video_writer.py
-media_processing_lib/video/libs/__init__.py
-media_processing_lib/video/libs/imageio/__init__.py
-media_processing_lib/video/libs/imageio/writer.py
-media_processing_lib/video/libs/opencv/__init__.py
-media_processing_lib/video/libs/opencv/writer.py
-media_processing_lib/video/reader/__init__.py
-media_processing_lib/video/reader/decord.py
-media_processing_lib/video/reader/imageio.py
-media_processing_lib/video/reader/images_path.py
-media_processing_lib/video/reader/mpl_video_backend.py
-media_processing_lib/video/reader/numpy_path.py
-media_processing_lib/video/reader/opencv.py
-media_processing_lib/video/reader/pims.py
-media_processing_lib/video/reader/raw_data.py
-resources/OpenSans-Bold.ttf
-test/test_collage_maker.py
+media_processing_lib/video/backends/__init__.py
+media_processing_lib/video/backends/decord.py
+media_processing_lib/video/backends/disk_backend.py
+media_processing_lib/video/backends/imageio.py
+media_processing_lib/video/backends/memory_backend.py
+media_processing_lib/video/backends/mpl_video_backend.py
+media_processing_lib/video/backends/opencv.py
+media_processing_lib/video/backends/pims.py
+media_processing_lib/video/writer/__init__.py
+media_processing_lib/video/writer/imageio/__init__.py
+media_processing_lib/video/writer/imageio/writer.py
+media_processing_lib/video/writer/opencv/__init__.py
+media_processing_lib/video/writer/opencv/writer.py
+resources/OpenSans-Bold.ttf
```

### Comparing `media-processing-lib-0.61/resources/OpenSans-Bold.ttf` & `media-processing-lib-0.62/resources/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.61/setup.py` & `media-processing-lib-0.62/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from setuptools import setup, find_packages
 from os import path
 
+
 def get_reqs(requirements):
     # Do not add to required lines pointing to Git repositories
     required, dependency_links = [], []
     EGG_MARK = "#egg="
     for line in requirements:
-        if line.startswith("-e git:") or line.startswith("-e git+") or \
-                line.startswith("git:") or line.startswith("git+"):
+        if (
+            line.startswith("-e git:")
+            or line.startswith("-e git+")
+            or line.startswith("git:")
+            or line.startswith("git+")
+        ):
             line = line.lstrip("-e ")  # in case that is using "-e"
             if EGG_MARK in line:
-                package_name = line[line.find(EGG_MARK) + len(EGG_MARK):]
-                repository = line[:line.find(EGG_MARK)]
+                package_name = line[line.find(EGG_MARK) + len(EGG_MARK) :]
+                repository = line[: line.find(EGG_MARK)]
                 required.append(f"{package_name} @ {repository}")
                 dependency_links.append(line)
             else:
                 print("Dependency to a git repository should have the format:")
                 print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
         else:
             required.append(line)
     return required, dependency_links
 
+
 name = "media-processing-lib"
-version = "0.61"
+version = "0.62"
 description = "Media processing library for video, audio and images."
 url = "https://gitlab.com/mihaicristianpirvu/media-processing-lib"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
@@ -41,9 +47,9 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=url,
     packages=find_packages(),
     install_requires=required,
     dependency_links=dependency_links,
     license="WTFPL",
-    python_requires=">=3.8"
+    python_requires=">=3.9",
 )
```


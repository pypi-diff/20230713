# Comparing `tmp/pymovie-3.7.7.tar.gz` & `tmp/pymovie-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymovie-3.7.7.tar", last modified: Fri Jun 30 16:03:40 2023, max compression
+gzip compressed data, was "pymovie-3.7.9.tar", last modified: Thu Jul 13 14:35:39 2023, max compression
```

## Comparing `pymovie-3.7.7.tar` & `pymovie-3.7.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 16:03:39.989101 pymovie-3.7.7/
--rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.7.7/LICENSE
--rw-rw-rw-   0        0        0     1474 2023-06-30 16:03:39.989101 pymovie-3.7.7/PKG-INFO
--rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.7.7/README.rst
--rw-rw-rw-   0        0        0       80 2023-06-30 16:03:39.989101 pymovie-3.7.7/setup.cfg
--rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:03:39.957962 pymovie-3.7.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:03:39.989101 pymovie-3.7.7/src/pymovie/
--rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.7.7/src/pymovie/NE3Lut.p
--rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.7.7/src/pymovie/PyMovie-doc.pdf
--rw-rw-rw-   0        0        0   628881 2023-06-30 14:44:27.000000 pymovie-3.7.7/src/pymovie/PyMovie-info.pdf
--rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.7.7/src/pymovie/PyMovie.bat
--rw-rw-rw-   0        0        0     6283 2023-05-12 20:27:48.000000 pymovie-3.7.7/src/pymovie/SER.py
--rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.7.7/src/pymovie/__init__.py
--rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.7.7/src/pymovie/alias_lnk_resolver.py
--rw-rw-rw-   0        0        0     6094 2023-05-18 11:24:11.000000 pymovie-3.7.7/src/pymovie/aperture.py
--rw-rw-rw-   0        0        0    15254 2023-06-27 02:54:33.000000 pymovie-3.7.7/src/pymovie/apertureEdit.py
--rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.7.7/src/pymovie/apertureEditDialog.py
--rw-rw-rw-   0        0        0     3962 2023-06-26 17:44:10.000000 pymovie-3.7.7/src/pymovie/apertureNameDialog.py
--rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.7.7/src/pymovie/aperturesFileTagDialog.py
--rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.7.7/src/pymovie/astrometry_client.py
--rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.7.7/src/pymovie/checkForNewerVersion.py
--rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.7.7/src/pymovie/gammaUtils.py
--rw-rw-rw-   0        0        0   233704 2023-06-26 17:44:13.000000 pymovie-3.7.7/src/pymovie/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-24 18:07:02.000000 pymovie-3.7.7/src/pymovie/helpDialog.py
--rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.7.7/src/pymovie/hotPixelDialog.py
--rw-rw-rw-   0        0        0   455131 2023-06-29 21:03:12.000000 pymovie-3.7.7/src/pymovie/main.py
--rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.7.7/src/pymovie/ocr.py
--rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.7.7/src/pymovie/ocrCharacterBox.py
--rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.7.7/src/pymovie/ocrProfileNameDialog.py
--rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.7.7/src/pymovie/play-Temp.py
--rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.7.7/src/pymovie/play-introspection.py
--rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.7.7/src/pymovie/run-pymovie-mac.bat
--rw-rw-rw-   0        0        0     4271 2023-05-31 13:21:53.000000 pymovie-3.7.7/src/pymovie/selectHotPixelProfile.py
--rw-rw-rw-   0        0        0     3675 2023-05-31 04:05:11.000000 pymovie-3.7.7/src/pymovie/selectProfile.py
--rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.7.7/src/pymovie/stacker.py
--rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.7.7/src/pymovie/starPositionDialog.py
--rw-rw-rw-   0        0        0       36 2023-06-30 15:52:51.000000 pymovie-3.7.7/src/pymovie/version.py
--rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.7.7/src/pymovie/wcs_helper_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:03:39.989101 pymovie-3.7.7/src/pymovie.egg-info/
--rw-rw-rw-   0        0        0     1474 2023-06-30 16:03:39.000000 pymovie-3.7.7/src/pymovie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2023-06-30 16:03:39.000000 pymovie-3.7.7/src/pymovie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 16:03:39.000000 pymovie-3.7.7/src/pymovie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.7.7/src/pymovie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      247 2023-06-30 16:03:39.000000 pymovie-3.7.7/src/pymovie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 16:03:39.000000 pymovie-3.7.7/src/pymovie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.421261 pymovie-3.7.9/
+-rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.7.9/LICENSE
+-rw-rw-rw-   0        0        0     1474 2023-07-13 14:35:39.421261 pymovie-3.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.7.9/README.rst
+-rw-rw-rw-   0        0        0       80 2023-07-13 14:35:39.422269 pymovie-3.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.273163 pymovie-3.7.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.417270 pymovie-3.7.9/src/pymovie/
+-rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.7.9/src/pymovie/NE3Lut.p
+-rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.7.9/src/pymovie/PyMovie-doc.pdf
+-rw-rw-rw-   0        0        0   631051 2023-07-13 14:33:12.000000 pymovie-3.7.9/src/pymovie/PyMovie-info.pdf
+-rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.7.9/src/pymovie/PyMovie.bat
+-rw-rw-rw-   0        0        0     6283 2023-05-12 20:27:48.000000 pymovie-3.7.9/src/pymovie/SER.py
+-rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.7.9/src/pymovie/__init__.py
+-rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.7.9/src/pymovie/alias_lnk_resolver.py
+-rw-rw-rw-   0        0        0     6094 2023-05-18 11:24:11.000000 pymovie-3.7.9/src/pymovie/aperture.py
+-rw-rw-rw-   0        0        0    15254 2023-06-27 02:54:33.000000 pymovie-3.7.9/src/pymovie/apertureEdit.py
+-rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.7.9/src/pymovie/apertureEditDialog.py
+-rw-rw-rw-   0        0        0     3962 2023-06-26 17:44:10.000000 pymovie-3.7.9/src/pymovie/apertureNameDialog.py
+-rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.7.9/src/pymovie/aperturesFileTagDialog.py
+-rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.7.9/src/pymovie/astrometry_client.py
+-rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.7.9/src/pymovie/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.7.9/src/pymovie/gammaUtils.py
+-rw-rw-rw-   0        0        0   233704 2023-06-26 17:44:13.000000 pymovie-3.7.9/src/pymovie/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-24 18:07:02.000000 pymovie-3.7.9/src/pymovie/helpDialog.py
+-rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.7.9/src/pymovie/hotPixelDialog.py
+-rw-rw-rw-   0        0        0   456486 2023-07-13 14:26:39.000000 pymovie-3.7.9/src/pymovie/main.py
+-rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.7.9/src/pymovie/ocr.py
+-rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.7.9/src/pymovie/ocrCharacterBox.py
+-rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.7.9/src/pymovie/ocrProfileNameDialog.py
+-rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.7.9/src/pymovie/play-Temp.py
+-rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.7.9/src/pymovie/play-introspection.py
+-rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.7.9/src/pymovie/run-pymovie-mac.bat
+-rw-rw-rw-   0        0        0     4271 2023-05-31 13:21:53.000000 pymovie-3.7.9/src/pymovie/selectHotPixelProfile.py
+-rw-rw-rw-   0        0        0     3675 2023-05-31 04:05:11.000000 pymovie-3.7.9/src/pymovie/selectProfile.py
+-rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.7.9/src/pymovie/stacker.py
+-rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.7.9/src/pymovie/starPositionDialog.py
+-rw-rw-rw-   0        0        0       36 2023-07-07 20:58:41.000000 pymovie-3.7.9/src/pymovie/version.py
+-rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.7.9/src/pymovie/wcs_helper_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.421261 pymovie-3.7.9/src/pymovie.egg-info/
+-rw-rw-rw-   0        0        0     1474 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.7.9/src/pymovie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      247 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/top_level.txt
```

### Comparing `pymovie-3.7.7/LICENSE` & `pymovie-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/PKG-INFO` & `pymovie-3.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.7.7
+Version: 3.7.9
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.7.7/setup.py` & `pymovie-3.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/PyMovie-doc.pdf` & `pymovie-3.7.9/src/pymovie/PyMovie-doc.pdf`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/PyMovie-info.pdf` & `pymovie-3.7.9/src/pymovie/PyMovie-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -3,14 +3,26 @@
 For general information about the program (with usage tips), click on the
 Documentation button that is in the Help tab panel. A pdf will be launched – it
 is out-of-date, but still a bit useful.
 Note: there is a series of (grossly out-of-date and nearly useless and possibly
 confusing) YouTube tutorials available. Go to
 http://occultations.org/observing/software/pymovie for access to these videos.
 PyMovie version history
+Version 3.7.9
+13 July 2023
+• Fixed a bug that caused 3.7.8 to fail with message PyMovie has no attribute
+extractionMethod
+Version 3.7.8
+6 July 2023
+• Added ‘best practices’ message popup when a user attempts to add a non-static mask
+aperture or a dynamic aperture stack to a “finder” image. This is done because
+dynamic mask apertures require a background calculation to set the appropriate
+threshold, and the background of a “finder” image is noise-reduced and hence the
+wrong value to use.
+Adding a static mask aperture set is okay as is an NRE aperture.
 Version 3.7.7
 30 June 2023
 • Changed the centering/tracking of fixed radius masks (in static apertures) from
 centering on the single brightest pixel (introduced in version 3.7.0) to a mass centroid
 calculated using the nThBrightPixel algorithm conceived and tested by A. G. Basden
 (reported in Centroids using Brightest Pixel Algorithm by A. G. Basden, et al, MNRAS,
 2011)
@@ -23,27 +35,27 @@
 R. Astron. Soc. 296, 339-346 (1998)].
 Naylor's algorithm utilizes a two-dimensional gaussian as an approximation to the psf
 of stars in the image and demonstrates that this is an effective approximation in practice. Using this analytic psf, the paper describes how to calculate a weighted mask that
 lowers the noise in a star intensity measurement by giving a larger weight to those
 pixel that have a higher SNR and a lower weight to dimmer, noisier pixels - this is the
 core idea in all optimal extraction schemes.
 
-•
+•
 
 PyMovie uses the Naylor algorithm in the form that is optimal for sky-limited observations - i.e., dim targets - and can be used for occultations where the target completely
 disappears.
 
 •
 
 Added an item to the aperture placement menu to add a nest of 12 static apertures of
 steadily increasing size. This is to support the common practice of testing extraction
 metrics for very small to quite large fixed circular masks, an old time-tested technique.
 PyOTE 5.2.6 introduced a set of tools to make processing multiple lightcurves and recording the fit-metrics easy.
 
-•
+•
 
 Added an item to the aperture placement menu to add a nest of 6 dynamic mask apertures of increasing threshold levels with the smallest threshold and threshold step settable in a simple dialog. This is a good practice, like that mentioned in the bullet item
 above. PyOTE 5.2.6 introduced a set of tools to make processing multiple lightcurves
 and recording the fit-metrics easy.
 
 Version 3.7.5
 12 May 2023
@@ -69,26 +81,26 @@
 
 Version 3.7.0 7 February 2023
 • Added an additional tracking feature to static apertures. In previous versions, the fixed
 radius circular sampling mask was always centered inside a static aperture. Tracking
 the enclosed star image was indirect, depending on some other ‘tracking aperture’
 placed elsewhere in the frame on a tracking star. But the position of the target star
 relative to the tracking star is not constant but jitters due to atmospheric turbulence, so
-a relatively large circular mask had to be used around the target star so that the
+
+a relatively large circular mask had to be used around the target star so that the
 jittering target star remained inside the circular mask. This version adds tracking to the
 fixed circular mask inside the aperture itself. It operates by finding the brightest pixel
 visible in a centered mask, then recentering the mask around that bright pixel. (A
 ‘bright pixel is defined as being at or above 1 std deviation above background.)
 It is now possible to more effectively lower the noise in an extracted target star
 lightcurve by using smaller and smaller circular masks to find the one that improves the
 noise best. This was possible in the past, but because positional jitter was not adjusted
 for static masks, the size of the smallest useful radius was often rather large. Now
 quite small radius values remain effective.
-
-This is a reliable form of ‘optimal extraction’ because it is robust during an occultation
+This is a reliable form of ‘optimal extraction’ because it is robust during an occultation
 where the target star image diminishes and shrinks (maybe disappearing) during the
 event. Other forms of ‘optimal extraction’ depend on a star image that is relatively
 bright with a well-defined and positionally stable point-spread-function. When those
 conditions are not met, as they often are not during the D and R transitions of an
 occultation, the lightcurve is at risk of being distorted by the extraction process, right at
 moments where we want it to be most reliable.
 Version 3.6.8 1 February 2023
@@ -109,24 +121,27 @@
 Version 3.6.2 7 August 2022
 • At one point in time (see version 3.2.0 and 3.2.1 discussion) a ‘hack’ was introduced to
 get Windows to preserve any image scaling and positioning during frame changes. The
 hack was to expand and contract the width of the image by 1 pixel. This ‘dance’ is
 sometime apparent. This version removes that ‘hack’ as it appears no longer
 necessary on Win10 or Win11.
 Version 3.6.1 7 August 2022
-• During timestamp OCR setup, frame 0 is often messed up during recording and so
+
+•
+
+During timestamp OCR setup, frame 0 is often messed up during recording and so
 should not be used for sampling timestamp characters. This version detects that
 situation and automatically advances to frame 1 with a pop-up message alerting the
 user that this action has been performed.
+
 Version 3.6.0 29 July 2022
 • fixes OCR context menu and plots
 Version 3.5.6 26 July 2022
 • fixes aperture context menu. OCR context menu still broken
-
-Version 3.5.1 23 July 2022
+Version 3.5.1 23 July 2022
 • it appears that the PyPI JSON API is no longer useful for getting the latest version of a
 package due to an announced breaking change on the part of the PyPI support team.
 This version utilizes a work-around so that we can continue to be alerted to the
 availability of a newer version than the one that is currently installed.
 Version 3.4.8 23 July 2022
 • fixed float/int problem in stacker.py that exhibits only in Win11 os, not Win10
 Version 3.4.7 22 July 2022
@@ -148,24 +163,24 @@
 Version 3.4.2 9Jul2022
 • fixes QMenu() reference issue (created by Qt programmers changing where the
 QMenu() item is found
 Version 3.4.1 22Jun2022
 • cleans up some issues involving the color scale for the thumbnails.
 Version 3.4.0 18Jun2022
 • For some reason, I thought that 16 bit FITS file images should be scaled (divided by)
-by 16 because all current A/D are 12 bits. I now think that this is a bad idea and have
+
+by 16 because all current A/D are 12 bits. I now think that this is a bad idea and have
 returned to displaying 16 bit FITS image as 0 to 65535 pixel values.
 Version 3.3.9
 • adds display of WCS RA and DEC info (if available) in a popup box whenever
 the key w is pressed while the mouse cursor is pointing to a star.
 Version 3.3.7
 • enable cursor-over-image wcs annotation whenever a WCS solution has been
 obtained, even when the target is not in the field
-
-Version 3.3.5
+Version 3.3.5
 • fixes 'skimage has no transform' when processing image with non-square pixels for
 submission to nove.astrometry.net
 •
 
 changes from horizontal bars to vertical bars in CMOS pixel tool
 
 •
@@ -193,25 +208,24 @@
 • The CMOS Pixels Tool tab is now fully functional.
 There is too much in this tab to explain in this forum – start your education with the
 Click me for help/info button. Then do right clicks on the other controls, starting at the upper
 left and procedding down the column, then move to the upper right.
 •
 
 I removed the 3x3 and 5x5 median filter options from the CCD Hot Pixels tab – they
-were not useful in any meaningful context and mostly just corrupted (smeared) the
-images that they were applied to.
 
+were not useful in any meaningful context and mostly just corrupted (smeared) the
+images that they were applied to.
 Version 3.2.6
 • improves help messages to give better guidance during use of the hot-pixel removal
 tab functions
 Presages the CMOS hot pixel tab functions to be added soon.
 Version 3.2.5
 • at the suggestion of a user, the version adds the name of the fits file that contains the
-
-currently displayed image to the file-in-use text box at the upper left. Of course this
+currently displayed image to the file-in-use text box at the upper left. Of course this
 only happens when a FITS folder has been selected.
 •
 
 Also changed is the treatment of fits image data in float32 or float64 format that may
 contain negative values. Negative values do not come from a camera but rather from
 some post-processing code. The new code clips the values so that they have a min
 value of 1 and a max value of 65535 so that the image data can be safely converted to
@@ -239,28 +253,25 @@
 days to find this 'hack' and still I hate that it's necessary.
 Version 3.2.0
 • has changed so that Zoom/Pan state of main image is preserved when switching back
 and forth between a 'finder' image and a frame image
 Version 3.1.6
 • fixes a bug that kept the use of yellow aperture mask (for windshake files) from
 displaying properly in Thumbnail Two
-Version 3.1.5
+
+Version 3.1.5
 • added code for converting FITS files that are in 64 bit float format to uint16. If the
 image pixels contained negative values (because they didn't actually come from a
 camera but some post-processing procedure), then frame by frame the image will have
 an amount added to it so that the smallest pixel value will become 1.0
 Version 3.1.4
 • fixed a typo introduced while reverting to the non-scrollable GUI.
 Version 3.1.3
-
-•
-
-added print of version number to console output (your command window) on startup as
+• added print of version number to console output (your command window) on startup as
 a diagnostic aid.
-
 Version 3.1.2
 • removed the scrolling GUI (for size-limited displays) introduced in version 2.9.8
 because it constrained the splitters too much and so inhibited panel resizing preferred
 by many users.
 This will return those users with small screens to a GUI that does have scroll bars,
 unless they always use version 3.1.1 and don't accept new updates.
 Version 3.1.1
@@ -282,25 +293,25 @@
 • adds clearing of line filter checkbox when new file is loaded. The display of the median
 plot is now a one-time event, as there was a need to clear that data in preparation of a
 new 'run'. This avoids duplicated and overlaid data in that array.
 Version 3.0.7
 • adds a median filter to reduce/eliminate 'line pattern noise' that some cameras exhibit.
 Such 'patterning' appears as row to row differences in brightness – streaks – that are
 consistently there. The median filter adjust each row indiviudally so that all rows and up
-having having the same median, and the 'line patterning' disappears.
+
+having having the same median, and the 'line patterning' disappears.
 This new feature can be found in the Misc. tab.
 Version 3.0.5
 • Adds a warning message if a user starts an analysis when there is already data
 present from a previous analysis run. This is an allowed condition (it allows running an
 analysis backwards or some part forward and the rest backwards to deal with a difficult
 tracking situation) but may cause some frames to be processed more than once. If that
 happens, attempts to write a csv file file with a duplicated frame message. With this
 new warning message, it should be clearer as to the cause and cure.
-
-Version 3.0.4
+Version 3.0.4
 • Found one more place where QtGui had to be replaced with PyQt5.QtWidgets
 Version 3.0.3
 • Changed QtGui.QApplication.setStyle('fusion') to
 PyQt5.QtWidgets.QApplication.setStyle('fusion') to fix the same issue covered by
 version 3.0.2
 Version 3.0.2
 • Changed the way QMainWindow is referenced from QtGui.QMainWindow to
@@ -326,24 +337,23 @@
 •
 
 The GUI has been changed so that scroll bars will appear when the standard GUI size
 exceeds your screen dimensions. THIS IS EXPERIMENTAL BECAUSE I DO NOT
 HAVE SUCH A SMALL SCREEN TO TEST WITH. If this does not work for you, please
 let me know immediately!
 
-Version 2.9.7
+Version 2.9.7
 • adds interlock so that use of yellow mask as the default mask cannot be enabled
 unless there is a yellow aperture present.
 Version 2.9.6
 • cures a ThumbNailTwo coloring issue when the default mask is set to Yellow Mask
 (FYI: the selection box for this option is in the Misc tab)
 Version 2.9.5
 • this change affects ONLY videos processed in field mode. Field mode processing is
-
-required when processing videos from the RunCam (and Mallincam) which incorrectly
+required when processing videos from the RunCam (and Mallincam) which incorrectly
 frame fields such that fields that belong together appear in two frames. In this version,
 the background mean calculations are done separately for each field and used for that
 fields background subtraction – prior to this, the background mean was computed once
 using the pixels from the whole frame (i.e., both fields) and that single mean was used
 to perform the background subtraction for both fields. Without this correction,
 processing a raw RunCam video and then the same video, but with corrected framing,
 produced slightly different lightcurves – that is no longer the case with this version.
@@ -374,25 +384,28 @@
 ‘sticky file’ whenever a new folder is opened (to solve the issue where ‘save dialogs’
 sometimes have a previous folder path rather than the current folder path and so
 tricking the unwary user into storing a file unintentionally into the wrong folder)
 Version 2.9.2
 • added forced install of version 4.1.2.30 of opencv-python to (hopefully) eliminate the qt
 plugin errors that occur on Mac installations.
 Version 2.9.1
-• added auto-install of opencv-python-headless and numpy>=1.17.0 in hopes of better
+
+•
+
+added auto-install of opencv-python-headless and numpy>=1.17.0 in hopes of better
 dealing with older installations on Anaconda3
+
 Version 2.9.0
 • red colorization has been added to pixels displayed in the Thumbnails that are at or
 above a value specified by the user (there is a place to enter this value just below the
 Show image contrast control check box.
 There is a new meaning to the values of minpx and maxpx (reported in the text box at
 the lower left) --- previously, these reported the min and max pixel values from the
 entire aperture; now they are the min and max pixel values of the pixels that have been
-
-selected by the 'mask'.
+selected by the 'mask'.
 The Thumbnail Two display now lets the actual pixels selected by the mask to be seen
 (the mask is transparent) and the surround of the mask is shown in yellow so that it is
 easy to visualize the mask selection.
 Version 2.8.9
 • adds frame number to the aperture report when the .csv file is written to allow a
 reviewer to place apertures that match those used to generate the .csv file. Note: the
 frame number will be that of the final frame recorded in the .csv file!
@@ -414,25 +427,25 @@
 special case. This change will be completely transparent – it will not affect QHY frames
 that have a GPS Locked status.
 Version 2.8.4
 • fixed issue that caused the initial display of a help message that was too big for the
 panel to be scrolled to the bottom (obscuring the first few lines) rather than the top.
 Version 2.8.3
 • adds an explicit Timestamp setup help button in the Timestamp tabbed panel. While
-help was available by right-clicking the Select VTI: label, that's not an obvious thing to
+
+help was available by right-clicking the Select VTI: label, that's not an obvious thing to
 do, hence the added button.
 Version 2.8.2
 • adds a color change to OCR selection boxes based on their ability to be jogged. A red
 selection box (which can't be jogged by the arrow keys) turns yellow whenever it is
 enabled for arrow key jogging. I added some clarification to the Kiwi instructions
 regarding selection box placement.
 A major aid in adjusting the selection boxes to center on the timestamp characters has
 been added: position your mouse cursor on a selection box and press the j key on the
-
-keyboard to make that box joggable. Next, move to the arrow keys and use them to
+keyboard to make that box joggable. Next, move to the arrow keys and use them to
 center the character, watching the thumbnail (which is now a live display --- no need to
 mouse out and back in as it had been). Once the character is well centered, press the j
 key again once again to make the box non-joggable. Move your cursor to the next
 character, rinse, and repeat. Training is unchanged --- right-click on a character and tell
 PyMovie what the character is.
 Version 2.8.1
 • adds documentation of aperture settings, lunar background usage, and yellow aperture
@@ -455,25 +468,25 @@
 The problem with a restricted search however is that if an error is made such that the
 target star is actually not in the image submitted, the search will simply fail quietly (and
 use a lot of computer time at nova to reach this conclusion!) without giving the user any
 clue as to why no solution could be found.
 With this version, I do a blind-search and if a solution is returned, I check to see if the
 target star is within the image and alert the user if the target star is not visible in the
 image.
-Version 2.7.8
+
+Version 2.7.8
 • Added a test for duplicated frames during the writing of a csv file and now abort the csv
 write should there be a duplicated frame found (caused by the user doing multiple
 overlapping analysis runs by accident).
 Version 2.7.7
 • Added an automatic 'Clear Data' at conclusion of 'finder image' generation do get rid of
 the aperture data that is collected during that operation.
 Version 2.7.6
 • Fixed a bug introduced by the addition of size 71 and 91 apertures. The bug appears
-
-only when a saved aperture group is restored --- it gets the aperture size wrong.
+only when a saved aperture group is restored --- it gets the aperture size wrong.
 Anyway, it's fixed.
 Version 2.7.5
 • Added the option of selecting extra large apertures of 71 or 91. These values are NOT
 included in the 'preferences' list (too little usage to justify the work required on my part)
 so those sizes will always have to be selected deliberately from the drop-down
 aperture size list.
 Version 2.7.4
@@ -498,26 +511,26 @@
 integer values).
 Version 2.6.9
 • Changed the 'help/info' for the Plot Robust Mean button to better explain the algorithm.
 Version 2.6.8
 • Changed the algorithm for calculating the average value of background pixels. This
 new algorithm replaced one that was excellent when background noise had a gaussian
 distribution, but had about a 1% error (too small by 1%) when the noise distribution
-was skewed. The histogram of a skewed distribution has a longer tail on one side than
+
+was skewed. The histogram of a skewed distribution has a longer tail on one side than
 the other. It is common to find recordings that have background noise that is skewed,
 usually with a longer tail on the right (toward higher values). Sometime, perhaps due
 to a camera setting, background levels are 'clipped' and so appear skewed, sometimes
 without a left tail at all. One other effect is frequently seen in 8 bit avi from a composite
 video camera --- missing values. These 'missing' values appear when a video with a
 range of pixel values from 10 to 235 is remapped (stretched) to a 0 to 255 range.
 When that process is present, every eighth value is missing and never appears as a
 pixel value.
 This new algorithm is insensitive to skew, clipping, and missing values.
-
-Version 2.6.7
+Version 2.6.7
 • Very minor change – set the default state of the checkbox that controls the display of
 frame metadata for ADV/AAV frames.
 One reason for this change is that this information is rarely needed.
 Another reason is that for AAV files, the first frame tag is named Error: and is usually
 empty, but as it heads a list of other tags, it is easy to thing that an error has actually
 occurred. But if the user had to check a box to see this data display, it will be clearer
 that no error has occurred.
@@ -537,29 +550,30 @@
 Version 2.6.1
 • Working with Hristo Pavlov, I have added support for reading Version 2 ADV files (Astro
 Digital Video files) to PyMovie.
 A side effect of our collaborative effort is that there is now a publicly available Python
 package on PyPI.org for reading .adv files (Version 2) --- the package is called Adv2
 and is available to any Python programmer by the usual pip install Adv2. The
 project and its documentation can be viewed at https://pypi.org/project/Adv2/
-While being able to read .adv files is a pre-requisite to reading AAV files, it is likely that
+
+While being able to read .adv files is a pre-requisite to reading AAV files, it is likely that
 some additional capabilities will need to be added to PyMovie to deal smoothly with
 such files. If the demand is there for such support and is made known to me, I will
 undertake adding the missing pieces.
 •
 
 Added an option to apply either a 3x3 or a 5x5 median filter to frames as they are
 being read --- this has the effect of removing hot-pixels automatically, provided the 'hotpixels' are isolated pixels or in very small groups. This is a much easier option than
 placing apertures on all the hot-pixel groups and asking PyMovie to record the
 coordinates of the enclosed hot-pixels for later 'erasure'. This simple method of
 removing hot-pixels has allowed me to generate very well defined “finder” images from
-
-a video that had too many hot-pixels to deal with by placing apertures on them
+a video that had too many hot-pixels to deal with by placing apertures on them
 individually. Fortunately, these hot-pixels were all single isolated pixels, so the 3x3
 median filter easily suppressed them during the “finder” image generation.
+
 Version 2.6.0
 • Added the change of 2.5.9 to .avi files. (Version 2.5.9 only applied to .ser files.)
 Version 2.5.9
 • Added the 100 nanosecond digit to the SER timestamps so that there now is no
 difference between the SharpCap timestamp and that of PyMovie. Timestamps to a
 resolution 0f 100 nanoseconds have little use, but this eliminates a discrepancy that
 might be unsettling to some.
@@ -581,41 +595,42 @@
 Version 2.5.6
 • In version 2.5.4 we switched to using a filename dialog that provided a list of alreadyused .csv file names, a useful convenience on occassion. Unfortunately, another
 characteristic of that file dialog is that it allowed the user to specify a filename that did
 not have a .csv extension. This version adds code to append a .csv extension to any
 filename the user provides that does not already have such an extension.
 Version 2.5.5
 • Squashed bug that kept avi files recorded with a dvsd codec from being read.
-Version 2.5.4
+
+Version 2.5.4
 • When writing a csv file or saving an aperture group, the dialogs now let you see what
 names you have used in the past.
 •
 
 CAUTION: the use of a computed mask (i.e., a snap-to-blob aperture) for the sole
 aperture that contains the target star, particularly if the target intensity drops
 significantly during the occultation, is not recommended! If you use a single
 aperture on the target star, it should be a static aperture with a fixed radius
 circular mask!
 The problem is that, as the target intensity drops, there may be a point, just before the
-
-default mask comes into use, that a very small computed mask gets used and that
+default mask comes into use, that a very small computed mask gets used and that
 mask fails to include all the pixels from the star image, thus creating an artificial drop
 that can/will affect where the D or R edge appears to occur. This is exacerbated by the
 use of the 2 sigma level for mask computation, a practice that, while good for tracking
 and reference stars, is hazardous for target stars.
 If you want to use a computed mask on such a target in hopes of achieving an
 improved snr, ALWAYS overlay that aperture with another aperture that uses a fixed
 circular mask. The composite lightcurve for the target will then make it clear whether
 or not the computed mask results should be used for timing as it will show two overlaid
 lightcurves: one with a computed mask and one with the standard (and reliable) fixed
 circular mask.
 The computed mask has proven to be most helpful in providing robust tracking. If you
 have a 12 or 16 bit camera and windshake, you will also get cleaner lightcurves by
 using computed masks. But for 8 bit videos with little windshake, the computed mask
 is best relegated to tracking and reference stars.
+
 Version 2.5.3
 • Fixed: during preparation of image for submission to nova.astrometry.net, I was forcing
 conversion of the image to uint16 for display purposes --- normally this would be ok,
 but FITS files can be float64 (signed) and cannot always be converted to uint16. I
 doubt any users will have noticed this, but one of my test data sets is a video of the
 Pluto occultation that was greatly 'massaged' and as a result came to me as a signed
 float64 file.
@@ -629,34 +644,35 @@
 affect your workflow if you were in the habit of running an analysis, plotting the results,
 and running a changed analysis expecting to be able to generate another set of plots
 without losing the first set. If this was your practice, now you will be required to
 explicitly save plots that you want to use for comparison studies.
 
 Version 2.5.1
 • Fixed: SER file folder selection was not enabling ‘save aperture group’ button.
-• Fixed: Initial ‘save’ of aperture group was not enabling ‘restore aperture group’ button
-• Changed: default aperture name from app00 to ap00
+
+•
+•
+
+Fixed: Initial ‘save’ of aperture group was not enabling ‘restore aperture group’ button
+Changed: default aperture name from app00 to ap00
+
 Version 2.5.0
 • Removed asinh scaling and normalization to 0...255 range in “finder” images. This will
 preserve star intensities and (hopefully) make “finder” images look more like the star
 chart. In addition, with this change, the contrast settings that are useful for an individual
 frame are also applicable to the “finder” image, so I make that setting ‘sticky’ during
 changes to and from a “finder” image.
 Version 2.4.9
-
-•
-
-This version provides a solution to the following problem: if snap-to-blob apertures are
+• This version provides a solution to the following problem: if snap-to-blob apertures are
 placed on a “finder” image, the thresh value (used for calculating sampling masks) will
 be correct for the “finder” image, but not for the frames of the video --- the average
 background will different and the noise will lower. The solution incorporated in this
 version is to detect when the display changes from a “finder” image back to the normal
 frames. When this change is detected, we now automatically recalculate thresh for all
 snap-to-blob apertures that are present.
-
 Version 2.4.8
 • Removed the requirement when reading a “finder” file that it reside in an avi/ser or fits
 folder to make it easier to use “finder” images from an external source (like RegiStax)
 Version 2.4.7
 • Dragging tabs to new positions to reflect a preferred work flow is now ‘sticky’ between
 session.
 Version 2.4.5
@@ -673,32 +689,29 @@
 computers.
 Version 2.4.3
 • Solves another problem reading large SER files --- again unique to Win10
 environment.
 Version 2.4.2
 • Solves problem reading large SER files that was unique to Win10 --- reading large
 SER files on Mac was no problem.
-Version 2.4.1
+
+Version 2.4.1
 • Adds timestamp extraction from SharpCap 8 bit avi captures. SharpCap embeds a 64
 bit timestamp (from Windows computer clock --- number of 100ns ticks since midnight
 on 1 Jan 0001) in the first 8 bytes of each frame (upper left corner). With this version,
 there is an addition to the VTI drop-down list that allows this form of avi to enjoy
 automatic timestamp extraction.
 Version 2.3.9
 • Fixed font issue on Preferences tab and radio button behavior
 Version 2.3.6
-
-•
-
-Adds initial support for GHS VTI. I have only a single sample to test with. It was a 720
+• Adds initial support for GHS VTI. I have only a single sample to test with. It was a 720
 x 480 avi running at 30 fps. The sample was provided by Hiroyuki Watanabe with the
 timestamp positioning he preferred. If the template extracted from that sample doesn’t
 fit your GHS setup very well, send me a sample. Sometimes a 640 x 480 (or other
 shape) needs its own template.
-
 Version 2.3.5
 • GUI changes: moved Plot Robust Mean back to main page --- because I use this a lot
 and don’t want the extra click on the Misc. tab. Moved Show contrast control to more
 readily accessible position.
 •
 
 Added a text box at top of form that displays the name of the file/folder currently being
@@ -729,33 +742,29 @@
 Version 2.3.1
 • Added test for astrometry.net failing to accept upload of image --- a failed upload
 happened once when astrometry.net was having some trouble --- so that a clear
 message to the user is produced.
 •
 
 Changed default mask radius from 5.3 (nearly always too big to be useful) to 3.2
-(which makes a smallish and roundish default mask of more useful size).
 
+(which makes a smallish and roundish default mask of more useful size).
 •
 
 Tracked down and solved some mysterious behavior associated with FITS files. After
 a deep dive, I discovered that all FITS files are written with data bytes ordered for a
 big-endian computer. We run on Intel, which is little-endian. Nearly all of my code did
 operations on image data using numpy, which detects and properly operates on either
 big or little-endian data. BUT, in my mask calculation, a routine is used that was ported
 from c++ code which did NOT adapt gracefully to big-endian image data. A test for bigendian data has been put in that routine and does an endian swap when necessary.
 
 Version 2.3.0
-
-•
-
-Fixed a bug involving saved aperture groups that did not contain a tracking path --- the
+• Fixed a bug involving saved aperture groups that did not contain a tracking path --- the
 code had been requiring the presence of a tracking path definition in a saved aperture
 group --- clearly that needs to be optional.
-
 •
 
 Added some additional ‘help’ info
 
 •
 
 Moved Version info button back to its original position, never to be moved again.
@@ -779,26 +788,26 @@
 When the Save aperture group button is clicked, a dialog will appear requesting that a
 ‘tag’ be supplied to give the 2 or 3 files that are used to record a saved aperture group
 a unique name. The tag is appended to a root name and when the Restore aperture
 group button is clicked, a list of available aperture groups will be presented for
 selection.
 Version 2.2.6
 • Many significant changes to finder image usage:
-It is now possible to generate and save multiple finder images. This is particularly
+
+It is now possible to generate and save multiple finder images. This is particularly
 helpful in the context of setting up for 2 point tracking. The procedure would be to
 generate a finder image at frame 10 (say) and another at frame 2500 (say). These will
 be saved as enhanced-image-10.fit and enhanced-image-2500.fit and can be restored
 by clicking the load finder image button --- there you can select the appropriate
 enhanced-image-nnn.fit file (or .bmp --- that’s still available so that RegiStax can be
 used as well). The appropriate frame number to position the video to will be extracted
 from the image name. These two finder images will be of assistance in positioning a
 yellow aperture and recording the 2 points needed for determining the tracking
 equation.
-
-It is now possible to place multiple apertures on a finder image. This can be useful to
+It is now possible to place multiple apertures on a finder image. This can be useful to
 ‘find’ which of several stars is the occulted one when a sky chart is not available or
 does not resolve the uncertainty. Pick the likely candidates with apertures --- run an
 analysis --- look for the occultation.
 Note: because of the change above, we no longer treat any particular aperture as a
 target aperture and do not record a ‘target xy’ as we had been in previous versions.
 Previous versions would only allow a single aperture to be placed on a finder image
 and assumed that this was the ‘target’ and recorded its coordinates in a special txt file.
@@ -824,25 +833,25 @@
 
 Version 2.2.4
 • On lightcurve plots: the composite light curve is back on top. I didn’t like it on the
 bottom so it is back to the top where it will stay. I did ensure that the order of adding
 curves to the composite lightcurve plot is based on the column order. In this way, if the
 target lightcurve is the first column in the csv plot, it will be the last added to the
 composite plot so its ‘dots’ will be on top.
-Version 2.2.3
+
+Version 2.2.3
 • When the lightcurves are plotted, the z-order of the composite light curve plot has been
 changed so that it is now the bottom-most plot rather than the topmost plot. In addition,
 the individual light curves will appear in the order specified by the order number of the
 aperture (this will match the column order in the csv file). So an aperture with order
 number 4 will be plotted on top of an aperture with order number 7. So the user now
 has complete control of the plot order for the individual lightcurves through judicious
 use of the aperture edit table invoked by clicking on the Examine/change aperture
 settings button.
-
-Version 2.2.2
+Version 2.2.2
 • Made change to 2.2.1 so that my name change is no longer a breaking change. This
 version accepts either form upon read, looking first for the new form, and then for the
 old form. It always writes the new form.
 Version 2.2.1
 • NOTE: this is a breaking change. When an aperture group is saved, the filenames that
 appear in the folder have been changed as shown below:
 markedApertures.p
@@ -867,23 +876,23 @@
 sunlit lunar limb for a lunar occultation.
 This is experimental: until this point, PyMovie has focussed on asteroid occultations
 only --- this is a deviation from that focus.
 When this box is checked, it signals the Robust Mean extraction routine to statistically
 separate sky pixels from lunar limb and star pixels for use in background calculations.
 This emulates what Limovie does when a properly oriented ‘Avoid Sunlit Face’ aperture
 is utilized and so should produce comparable lightcurves. Time will tell.
-Version 2.1.8
+
+Version 2.1.8
 • I now save tracking path data when an aperture group is saved.
 Version 2.1.7
 • Added the ability to set a ‘tracking path’ by specifying two points, one early in the video
 and one late in the video. This feature is primarily useful in processing difficult driftthrough videos where no other good options for tracking are present.
 To learn a bit more, right-click on a non-yellow aperture and then click one of the menu
 items involving ‘track path’. That will cause a help panel to appear.
-
-Version 2.1.6
+Version 2.1.6
 • Robust Mean extractor changed so that when processing a ‘clipped’ background, star
 pixels will be excluded from the calculation by not including pixels with values that are
 are more than 3 sigma from the mean.
 Version 2.1.5
 • Modified Robust Mean extractor to detect ‘clipped’ backgrounds and employ a different
 algorithm for the determination of mean and standard deviation.
 Version 2.1.4
@@ -898,32 +907,34 @@
 before this version --- that feature speeds up the initial sampling of the digits. The
 change made in this version is that, if all digits have been sampled, a complete menu
 of digits to record will be produced when a digit is right-clicked so that any poorly
 sampled digit can be re-recorded without the need to start over from scratch.
 version 2.1.2
 • Added ability to correct pixel response curve for non-unity gamma setting of camera
 version 2.1.1
-• Modified the robust mean estimator to deal with videos that have ‘clipped’
+
+•
+
+Modified the robust mean estimator to deal with videos that have ‘clipped’
 backgrounds, a situation that is surprisingly common.
 
-Here is a ‘normal’ RobustMean plot:
+Here is a ‘normal’ RobustMean plot:
 It shows the usual gaussian background noise in a 51x51 pixel aperture with some stars in
 the aperture as well.
 But sometimes we see that somewhere in the processing chain (could be a camera setting --could be in the recording software) that some sort of 'clipping' has occurred. It exhibits as a
 'one-sided' noise distribution with many of the background pixel values equal to a fixed value.
 This is illustrated in the plot below:
 
-The problem now is how to calculate something that approximates a standard deviation for
+The problem now is how to calculate something that approximates a standard deviation for
 the background noise. This is an important value because PyMovie uses that number to set
 an initial threshold value which is used in the calculation of the sampling mask. But the
 presence of very many constant values causes the current computation to produce a very
 small (often 0.0) value for the estimated std and that causes mask threshold values to be set
 unreasonably low.
-
-The changed robust mean estimator, applied to the same 51x51 aperture produces:
+The changed robust mean estimator, applied to the same 51x51 aperture produces:
 
 and the resulting standard deviation is much more realistic and produces a useful initial value
 for the mask threshold.
 Note: such clipping has an effect on photometry. It appears small, so can often be ignored,
 but if you can set your processing chain to avoid such clipping, that would be the
 recommended way to go.
 version 2.1.0
@@ -935,21 +946,25 @@
 have any affect on properly recorded backgrounds, but stay alert!
 version 2.0.8
 • Added ability to redact images from top and bottom simultaneously.
 • Modified IOTA timestamp ocr parser to allow for a 3 digit milliseconds field (fourth entry
 blank). This makes ocr timestamp reading possible for the smopiVTI by treating it as
 an IOTA VTI with repositioned character boxes.
 version 2.0.7
-• Fixed 3D Thumbnail display (it got broken in version 2.0.2 when left to right image
+
+•
+•
+
+Fixed 3D Thumbnail display (it got broken in version 2.0.2 when left to right image
 flipping was added)
-• Changed Open AVI file button label to Open AVI/SER file.
+Changed Open AVI file button label to Open AVI/SER file.
+
 version 2.0.6
 • Added PAL mode Kiwi OCR timestamp recognition. In PAL mode, Kiwi timestamp
-
-characters are vertical. In NTSC mode, the characters are slanted.
+characters are vertical. In NTSC mode, the characters are slanted.
 version 2.0.5
 • Adds the ability to read 8 and 16 bit gray-scale (not color) SER files
 NOTE !!!! Quite a few changes were made to the code to add this capability.
 NOTE !!!! Although changes were carefully isolated and made specific to SER files,
 NOTE !!!! the possibility that a bug was introduced is high.
 PLEASE: email me immediately if you find such a breakage
 (bob.anderson.ok@gmail.com)
@@ -975,22 +990,22 @@
 creating ‘finder’ images. This is necessary so that the stacker aligns to star features
 rather than background features/texture.
 version 1.9.9
 • Major rewrite of manual WCS calibration code. Biggest change was to solve for the
 rotation angle between the RA/Dec and x/y coordinate systems numerically rather than
 with trig. This numerical solution tolerates all possible orientations. The change was
 necessitated when an alt-az example showed that the trig solution was too
-temperamental --- and there were problems earlier with inverted or flipped images that
+
+temperamental --- and there were problems earlier with inverted or flipped images that
 were dealt with as special cases and now can be treated without special code. The
 other change was to use a 2 x 2 rotation matrix to calculate the target x/y coordinates.
 The rotation matrix values depend only on the rotation angle between the RA/Dec and
 x/y coordinate systems, determined robustly by the numerical ‘search’ referred to
 earlier.
-
-version 1.9.8
+version 1.9.8
 • IF you have enabled a SINGLE ocr selection box for jogging, jogging that box will
 automatically show you the expanded view in the Thumbnails. This feature is
 automatically suppressed if more than one box is being jogged (which box should be
 displayed??). This change will not affect anyone that has gotten used to jogging
 groups of boxes, but for people electing to jog each box individually into place, this will
 be more intuitive and save the extra right-click to ‘show properties’.
 version 1.9.7
@@ -1016,21 +1031,24 @@
 prompting (rudely) for an aperture name when a static aperture was being placed.
 Fixed it --- we’re back to prompting for an aperture name when a single static aperture
 is placed, but don’t prompt for names when a stack of 5 is placed.
 version 1.9.0
 • Updated the right-click help message for the Examine/change aperture settings button
 to reflect the new functionality of using the thumbnails to show aperture contents and
 either computed mask or default mask.
-• It is expected that this will be the version released for public use --- end of Beta testing
+
+•
+
+It is expected that this will be the version released for public use --- end of Beta testing
 --- start of production testing.
+
 version 1.8.9
 • Added a menu item to add a stack of 5 static apertures.
 • Also allow red apertures to ‘snap’ as their threshold is changed from the Aperture Edit
-
-list. Previously, on a ‘green’ aperture would snap.
+list. Previously, on a ‘green’ aperture would snap.
 version 1.8.8
 • Made a ‘live’ connection between the Aperture List Dialog and the thumbnails so that is
 is easy to set default mask sizes and thresholds with a ‘live’ view of the effects. Also
 eliminated the need for a ‘write’ button by making any change take effect immediately
 when enter key pressed, cell focus changed (by tab or arrow key or mouse click), or
 dialog closed.
 • Fixed csv write routine so that is uses the correct folder location (AVI-WCS or FITS) as
@@ -1057,23 +1075,27 @@
 workflow-order.
 version 1.8.2
 • Added the ability to save an aperture configuration between 'runs'. Preserved is the
 frame showing when the Save aperture group button was clicked and the apertures
 showing at that time, including all of their properties. The configuration can be
 retrieved by clicking the Restore aperture group button.
 version 1.8.1
-• Added +/- 1 frame buttons and removed the the up/down buttons on the current frame
+
+•
+•
+
+Added +/- 1 frame buttons and removed the the up/down buttons on the current frame
 and stop frame spinners.
-• Made it easy to change pixel dimensions during WCS operations. This is normally a
+Made it easy to change pixel dimensions during WCS operations. This is normally a
 set-and-forget operation --- please do not experiment with dimensions to 'guess' at
 pixel dimensions --- that would be an abuse of nova.astrometry.net. A single test to
 prove that it does matter is ok. Figure out what your pixel dimensions are from camera
-
-specs/sensor chip manufacturer, not from inducing nova.astrometry.net to 'fail', which
+specs/sensor chip manufacturer, not from inducing nova.astrometry.net to 'fail', which
 slows down the service for everyone world-wide.
+
 version 1.8.0
 • 'play' was not initializing tracking --- added the needed initialization so that 'play' will
 show exactly what would happen during an analysis.
 version 1.7.9
 • Fixed indexing problem with lightcurve plots in field mode that was causing incorrect
 frame numbers to be displayed as hairline was moved.
 version 1.7.8
@@ -1098,29 +1120,30 @@
 
 This compensation is NOT YET incorporated in manual WCS calibration.
 
 version 1.7.2
 • Moved all the major operational buttons (clear data, write csv, plot curves) to the
 transport button complex.
 version 1.7.1
-• Rearranged transport buttons to allow more flexibility in splitter placement and also to
-bring the current frame spinner to a more accessible place.
-• Begun adding the elements needed to deal with non-square pixels during WCS
-calibrations --- GUI elements only at the moment.
-version 1.7.0
 
 •
+•
+
+Rearranged transport buttons to allow more flexibility in splitter placement and also to
+bring the current frame spinner to a more accessible place.
+Begun adding the elements needed to deal with non-square pixels during WCS
+calibrations --- GUI elements only at the moment.
 
-Implements the save/restore state feature. Only the number of apertures and their
+version 1.7.0
+• Implements the save/restore state feature. Only the number of apertures and their
 positions are 'marked'. The frame number is 'marked' as well. This 'mark' is placed
 automatically when the first analysis is initiated on a newly loaded video. However,
 there is a button that can be utilized to override this 'mark' if the automatic 'mark' was
 somehow incorrect (or you just changed your mind about where to stat an analysis or
 how many apertures to use, etc).
-
 version 1.6.9
 • Transport buttons fully functional.
 • Save and restore state buttons added to GUI, but not yet implemented.
 version 1.6.8
 • Added additional entries to the OCR profile dictionary to accommodate the need for
 four sets of character selection boxes for Kiwi. That need became apparent when it
 was determined that the left-right shift of Kiwi characters was not a constant but
@@ -1144,21 +1167,21 @@
 where it won't be the accidentally invoked by a user intending to click the mskth
 spinner.
 version 1.6.5
 • Made some small changes to documentation pdf suggested by Tony
 • Relabeled the angle printed at completion of manual WCS calibration from fieldrotation (incorrect) to ref1-to-target. This angle is a diagnostic printout, useful to me,
 but not to the user. To interpret it, you need to know that the coordinate systems in use
 are: x increases to right, y increases down, RA has East to the right, DEC has North
-down, and angles in the x-y plane (the image) are always positive and are the number
+
+down, and angles in the x-y plane (the image) are always positive and are the number
 of degrees in the ccw direction needed to rotate a vector until it lines up with the
 positive (i.e., down) y axis. So ref1-to-target means the origin is ref1, and we are
 rotating the vector from ref1 to target around ref1 ccw until it is aligned with the positive
 y axis.
-
-version 1.6.4
+version 1.6.4
 • Updated documentation pdf
 version 1.6.3
 • Added units to the plate scale that is printed at completion of manual WCS calibration.
 • Added field rotation angle printout at completion of manual WCS calibration.
 version 1.6.2
 • For manual WCS calibration: automatically adjusts to star fields that are flipped left-toright and/or top-to-bottom.
 version 1.6.1
@@ -1183,30 +1206,25 @@
 t2 on a timestamp line --- either left or right. After that, the other digits (t1) wilnot be
 used. This will reduce the number of times an ocr error occurs because of a misrecognition of a digit in a part of the timestamp that should not have been used.
 version 1.5.4
 • Changed blank detection for Kiwi to reflect the new 'normalized' model characters.
 • Added (Kiwi) 8 versus 9 secondary test to resolve confusions (same thing as is being
 done for 6 versus 8)
 • The logic to allow a Kiwi profile to be saved from other than a frame where the
-characters are in their training position was too tortuous to implement. Now we just
+
+characters are in their training position was too tortuous to implement. Now we just
 reposition to frame 1 before doing the save. This means that all training needs to be
 accomplished while the characters are in the position of those in frame 1.
 version 1.5.2
-
-•
-•
-•
-
-When starting from empty folder to train Kiwi, the selection boxes initially were being
+• When starting from empty folder to train Kiwi, the selection boxes initially were being
 displayed as red rectangles instead of yellow slanted selection boxes --- that's fixed
-At completion of choosing model digits, we now start timestamp reading.
-If a Kiwi training is done and a trial run is made that ends with boxes in the alternate
+• At completion of choosing model digits, we now start timestamp reading.
+• If a Kiwi training is done and a trial run is made that ends with boxes in the alternate
 position, we now detect the new position so that if the ocr profile is saved from this
 position, it will be saved with the current box positions as well as the model digits.
-
 version 1.5.1
 • Major change to Kiwi digit processing: trapezoidal boxes for selection (matching the
 'lean' of the font); removal of blank lines in font; removing 'lean' from the characters; no
 longer use Gaussian blur.
 Initial tests show that it is much easier to place ocr selection boxes and recognition
 error rate is no longer so sensitive to the precise box placement.
 version 1.5.0
@@ -1232,20 +1250,20 @@
 character positions.)
 • Squashed the bug that was causing crash when training an OCR profile from an empty
 folder and not providing a star location when prompted.
 •
 
 Very high quality (low error rates) OCR for Kiwi timestamps is available IF and ONLY IF
 you take the time to jog the character selection boxes into good positions. A good
-position has the character right-justified in the box. Use 'show property' to get a view
+
+position has the character right-justified in the box. Use 'show property' to get a view
 of EVERY character box placement and adjust accordingly before saving the model
 digit. It's fiddly, but I routinely get 100% recognition rates on Kiwi timestamps by
 following this advice.
-
-•
+•
 
 Changed the name of the users' list of custom profiles from pymovie-ocr-profiles<username>.p to simply pymovie-ocr-profiles.p What this implies is that we no longer
 support the presence (and automatic merging) of multiple custom profile dictionaries in
 the users' home directory. This feature was highly unlikely to be useful and greatly
 complicated the editing (deleting) of profiles from the custom directories. That is much
 easier to implement when there is but a single dictionary. This will be done in the next
 version.
@@ -1275,20 +1293,20 @@
 positions
 You will therefore need to choose the correct ocr box set when setting up the ocr
 profile
 Subsequently, whenever the minute field changes, the other position is applied and
 remains
 active until the next minute change.
 As a consequence of this, you must make sure that any initial 'training' (model digit
-recording) never crosses a minute boundary. This is not usually hard to do as the
+
+recording) never crosses a minute boundary. This is not usually hard to do as the
 complete digit set is usually present in the first 3 or 4 frames.
 In addition, take care not to adjust (jog) Kiwi ocr boxes unless the character position is
 the same as frame 1.
-
-version 1.4.0
+version 1.4.0
 • Added automatic opening of the newly created AVI-WCS folder after it has been
 created by by clicking the Create AVI-WCS folder from avi file button. So the workflow
 instructions that came with 1.3.9 are no longer needed.
 version 1.3.9
 • Removed the message inadvertently left in place that said only partial support for
 Windows for creation of AVI-WCS folders. It wasn't true.
 • When an AVI-WCS folder is created from an open avi file, I make that folder be the
@@ -1317,25 +1335,22 @@
 • Fixed bug where adding a custom profile was not removing existing ocr selection
 boxes.
 • Gui change to keep 'cascade' label from disappearing on some displays.
 • Started adding ability to create an AVI-WCS folder from an already open avi file. Just
 the gui and a stub where the code will go.
 version 1.3.6
 • Fixed bug that required AVI-WCS folder to be reopened in order for a newly selected
-custom ocr profile to take effect. Now timestamp reading starts up as soon as a
+
+custom ocr profile to take effect. Now timestamp reading starts up as soon as a
 custom profile is selected.
 version 1.3.5
 • Added printing of the 'confusion matrix' (correlation scores of each model digit against
-
-•
-
 all the others) when 'show model digits' is invoked.
-Fixed the spurious exception that was occurring when FITS folder was in use (caused
+• Fixed the spurious exception that was occurring when FITS folder was in use (caused
 by trying to do timestamp extraction as though a VTI were in use)
-
 version 1.3.4
 • Fixed BoxSprite 'start-from-scratch' specifying None instead of boxsprite as timestamp
 formatter.
 version 1.3.3
 • Fixed BoxSprite 'start-from-scratch' specifying iota instead of boxsprite as timestamp
 formatter.
 version 1.3.2
@@ -1364,21 +1379,25 @@
 version 1.3.1
 • Added to ocr box right-click menu: retrain model digits, enable/disable upper/lower
 boxes.
 • Added automatic switch to frame view if field view was selected and then Start analysis
 was clicked. It is possible to Pause analysis and then switch to field view without loss
 of data.
 • Removed threshold spinner as that mechanism is no longer used for OCR --- switched
+
+•
+•
+
 to custom model digits per AVI-WCS folder instead.
-• Fixed problem that kept ocr box changes and model digits from being properly
+Fixed problem that kept ocr box changes and model digits from being properly
 preserved and restored from an AVI-WCS folder.
-• Laid some framework in place for saving and reusing custom profiles (i.e., ocr boxes
+Laid some framework in place for saving and reusing custom profiles (i.e., ocr boxes
 and model digits from an AVI-WCS folder)
 
-version 1.3.0
+version 1.3.0
 • We now require that an avi --- for which timestamp OCR extraction is wanted --- be
 placed in an AVI-WCS folder. This allows completely custom ocr box placement and
 modelDigit training. This need only be done once. When that folder is reopened, it will
 snap to frame 1 with ocr boxes placed and the correct vti selected. The value of
 training for each file is that the highest OCR accuracy will always be obtained.
 version 1.2.9
 • Made the cascading of lightcurve plots optional (and sticky)
@@ -1409,23 +1428,23 @@
 being set to match the detected fps; that is fixed.
 •
 
 Timestamp OCR is now functional for the IOTA VTI. Model 3 is directly supported.
 Model 2 (which interchanges the position of the early millisecond characters (VTI3:
 early on left; VTI2: early on right) can be decoded as well if one takes the time to
 reposition the ocr selection boxes. Such a change is 'sticky'. This is useful when there
-is a single tool chain (camera/VTI/frame-grabber) because, once set for your
-equipment setup, it will be ready to go next time.
 
+is a single tool chain (camera/VTI/frame-grabber) because, once set for your
+equipment setup, it will be ready to go next time.
 •
 
 Recommended work flow: open avi, select VTI, click the appropriate radio button that
 tells PyMovie which field (top or bottom) is first in time, adjust ocr selection boxes (if
+needed), leave field display mode and place measurement apertures as usual.
 
-needed), leave field display mode and place measurement apertures as usual.
 version 1.1.8
 • Changed the titling on the frame navigation buttons to use time units for ntsc/pal
 recordings --- fits still uses frame units as there is no set correlation between frames
 and time for fits recordings.
 • Lightcurve plots now cascade (don't overlap) from the upper left corner of your screen
 down and to the right (rather than be plotted on top of each other in the center of your
 screen).
@@ -1454,39 +1473,33 @@
 panel.
 version 1.1.2
 • Implements output of csv aperture data in the order specified by the user rather than
 the default order based on the order of adding apertures to the image. For now,
 PyOTE accepts only up to the first four light curves, so when multiple apertures are in
 use, this re-ordering will make sure that you will be able to use PyOTE on the relevant
 lightcurves. It is possible (in the future) that PyOTE will be modified so that more than
-4 lightcuves can be processed at the same time. Until then, be judicious in
+
+4 lightcuves can be processed at the same time. Until then, be judicious in
 selecting/ordering the apertures.
 version 1.1.1
 • Removed the log scaling checkbox. Log scaling rarely used and the image control is
-
-•
-•
-•
-•
-
 an adequate and flexible tool for image clipping and scaling to better see stars in an
 image
-Added an Edit Aperture tool that pops up a list of all aperture with their properties and
+• Added an Edit Aperture tool that pops up a list of all aperture with their properties and
 provides a central place to modify same. This will make it easier to deal with stacked
 (overlapping) apertures.
-Added a default mask radius setting for each aperture rather than the one-size-fits-all
+• Added a default mask radius setting for each aperture rather than the one-size-fits-all
 of prior versions to better support the use of multiple sampling aperture/masks.
-Removed the spinner previously used for setting a global default mask.
-Changed status bar display when mouse is hovered over an aperture to simply show a
+• Removed the spinner previously used for setting a global default mask.
+• Changed status bar display when mouse is hovered over an aperture to simply show a
 list of any apertures that are under the cursor (again in support of stacked/overlapping
 apertures). Previously all the special properties of the topmost aperture were output to
 the status bar. That was not helpful when apertures were stacked on top of each other.
 Now the Edit Aperture list lets one see all the properties of all the apertures, so it's
 more important to to be able to locate apertures via mouse hover, hence this change.
-
 version 1.1.0
 • Added a check on the validity of RA Dec strings on a program path that was missed in
 1.0.9.
 version 1.0.9
 • Tests the validity of RA Dec strings at the point of entry --- shows errors in textOut
 panel.
 • Returns the aperture jogging capability that was inadvertently suppressed in 1.0.8 by
@@ -1502,23 +1515,20 @@
 subsequent right-click-for-help events. The user is encouraged to position and size the
 help dialog box to suit his preferences and to not worry if it gets hidden because a new
 right-click-for-help will pop it right back up at the previous size and position.
 This help system is much easier to use to quickly explore the help available for each
 gui control.
 version 1.0.4
 • Hover is now properly disabled so that help only appears with a right-click
-version 1.0.3
+
+version 1.0.3
 • Changed the 'help' system from a 'hover to get help' to a right-click to get help.
 version 1.0.2
-
-•
-
-Fixed conversion of color image to grayscale image for avis: now processes YUV color
+• Fixed conversion of color image to grayscale image for avis: now processes YUV color
 space correctly.
-
 version 1.0.0
 • Added documentation: PyMovie-doc.pdf
 • Pushed source code to git-hub for the first time
 • Updated Windows PyMovie.bat file to require the user to press the Enter key to close
 the script. This keeps the prompt window open so that if anything went wrong, the
 diagnostic messages will remain visible. This file is created in C:\Anaconda3 the first
 time PyMovie is run. However, we do not over-write an existing PyMovie.bat file, so if
@@ -1547,20 +1557,20 @@
 version 0.9.3
 • the calculations for manual WCS calibration have definitely been 'fixed' .
 • Miscellaneous small changes to GUI: labels on edit boxes for redact lines and plate
 scale; clear the VizieR response as soon as a change is made in UCAC4 box.
 version 0.9.2
 • the calculations for manual WCS calibration have been 'fixed' (we hope).
 • added the ability to specify a plate scale to use for the manual WCS calibration. Any
-value entered in the box to the right of the the Manual WCS calibration button will used
+
+value entered in the box to the right of the the Manual WCS calibration button will used
 as the plate scale. But be sure to leave this box empty if you want the maths behind
 manual WCS calibration to estimate the plate scale from the calibration points
 provided; this is the normal expected use.
-
-version 0.9.0
+version 0.9.0
 • same as 0.8.9 but added astroquery as a required package. This is used to make
 VizieR calls but is not a standard part of an Anaconda installation.
 version 0.8.9
 • this version adds manual WCS calibration. It is not yet very accurate likely due to the
 assumption that the RA Dec coordinate system covers a small enough area that the
 curvature of RA/Dec grid lines could be ignored --- this may not a good assumption.
 Currently a target aperture may be placed 2 to 4 pixels from the correct location (per
@@ -1588,25 +1598,22 @@
 • removed the self.pointed_at_aperture = None statement in removeAperture method.
 Just trying stuff.
 version 0.8.3
 • still working on avoiding crashes while deleting apertures under win7. Added manual
 disconnect of slot/signals for the aperture before deleting it.
 version 0.8.2
 • another variation on deleting apertures, this time without the aperture.deleteLater() call.
-version 0.8.1
+
+version 0.8.1
 • another attempt to squash the win7 crash-on-delete-then-run bug.
 version 0.8.0
-
-•
-
-added self.pointed_at_aperture = None when an aperture is deleted. This is a possible
+• added self.pointed_at_aperture = None when an aperture is deleted. This is a possible
 cause of referring to an aperture that has been deleted and thus causing a memory
 violation exception. Crossing our fingers on this one that it finally solves the win7
 crash-sometimes-when-aperture-is-deleted problem.
-
 version 0.7.9
 • in another attempt to find a solution to the occasional crash that a beta tester has
 experienced when deleting an aperture, I changed from the use of
 removeItem(aperture) to aperture.deleteLater(). Their was some chatter on the internet
 that this is a better/safer procedure.
 version 0.7.8
 • restored the automatic green property for a newly added aperture.
@@ -1632,25 +1639,22 @@
 one) that is used to place a target aperture 'blind' on frame 0. This folder will be the
 default location for csv files and (in the future) png dumps of lightcurve plots.
 • finally found bug that was causing confusing thumbnail updates. Should be better now.
 version 0.6.8
 • tightened up the spacing between GUI elements to provide more vertical space for text
 box
 • changed labelling of mask threshold spinner
-version 0.6.7
+
+version 0.6.7
 • rearrange items on GUI to allow for large Clear plot data button
 • added 'hooks' for experimenting with WCS/astrometry.net
 • fixed issue where Thumbnail One was not always synchronized with Thumbnail Two
-
-•
-
 (probably)
-made thumbnail display policy the same whether stepping through or running an
+• made thumbnail display policy the same whether stepping through or running an
 analysis
-
 version 0.6.6
 • new policy: all newly created apertures default to having auto-display enabled.
 • to control which of a group of apertures, all with auto-display ON, has its thumbnail
 dynamically updated during an analysis run, a property was added to make a
 specifically chosen aperture be the source for Thumbnail One. There will be either one
 or no apertures with this property set, enforced by the program. Should there already
 be an aperture with this property set and you choose a different aperture as the
@@ -1679,29 +1683,25 @@
 as to what is going and avoids the 'complaints' from within the pyqtgraph histogram
 widget when all pixels have the same value
 • added a 3D display (rotatable and zoomable by left and right mouse drag) for the
 Thumbnail One image.
 version 0.4.8
 • now, if you put your cursor on an aperture, the name and major properties of the
 aperture appear in the status bar in the very bottom left corner of the GUI
-version 0.4.6
+
+version 0.4.6
 • added the name of aperture to its context menu --- appears at the top of the right-click
 menu
 • added ability to use arrow keys to jog apertures. Each aperture has a flag to enable it
-
-•
-•
-
 to respond to an arrow key, so apertures could be manually jogged as a group should
 that be useful. When an aperture is added, it is born 'joggable' and with 'auto-display'
-Eliminated the 'green' mode for an aperture. Now each aperture can request that its
+• Eliminated the 'green' mode for an aperture. Now each aperture can request that its
 stats be printed at each frame change. There is only one thumbnail display however
 so only the last aperture in a group that gets printed will have its thumbnail displayed.
-Added cross hairs to thumbnail One to aid in manual positioning of apertures.
-
+• Added cross hairs to thumbnail One to aid in manual positioning of apertures.
 version 0.4.5
 • removed debug printout from Demo Robust
 • added auto-naming to no-snap aperture creation (just overlooked it earlier)
 • ThumbNailOne no longer uses log scaling. Instead, it uses whatever scaling is in force
 for the frame image.
 version 0.4.4
 • added button to read a bmp file, assumed to be a star locator. Any apertures
@@ -1724,24 +1724,28 @@
 • added an image range control to give user complete control over image 'stretching'.
 This is a visual effect only as an aid to identifying stars --- it does not affect any
 underlying data values.
 • Added an 'invert images' checkbox to make it easy to switch between avi and fits files
 with their differing convention of the image origin (fits: lower left corner; avi: upper left
 corner)
 version 0.3.9
-• added fast navigate buttons to speed going forward and backward through images
-• now the text box gets cleared when a new image file is successfully opened
-• changed the way apertures are deleted in support of chasing a pesky sporadic crash
-when apertures are deleted
-• add a spinbox to allow the user to select the plot symbol size --- it's set by a spinbox
 
 •
 •
 •
+•
+•
+•
+•
 
+added fast navigate buttons to speed going forward and backward through images
+now the text box gets cleared when a new image file is successfully opened
+changed the way apertures are deleted in support of chasing a pesky sporadic crash
+when apertures are deleted
+add a spinbox to allow the user to select the plot symbol size --- it's set by a spinbox
 that is 'sticky'
 some rearranging of GUI elements
 changed label on threshold box to help user understand better what a value in this box
 means
 added a legend to the composite lightcurve plot to identify the curves
 
 version 0.3.8
@@ -1770,21 +1774,25 @@
 version 0.3.1
 • field processing of avi files now operational
 version 0.3.0
 • fixed tracking during wind shake (accidentally broken in 0.2.9)
 • now we enable/disable controls that are specific to avi versus fits file processing
 • added printout of frames per second read from avi files
 • added ability to view both fields of an avi frame
-• added update of default mask when aperture size is changed to solve the
+
+•
+•
+
+added update of default mask when aperture size is changed to solve the
 mask/thumbnail shape mis-match exception from occurring
-• added aperture constellation tracking during manual (frame spinbox) changing of
+added aperture constellation tracking during manual (frame spinbox) changing of
 frame. It was confusing to have aperture constellation tracking only active during a
 'run'
 
-version 0.2.9
+version 0.2.9
 • added the printing of the FOURCC codec ID extracted from avi files that could be
 opened. This may have diagnostic value in some case where an unusual codec was
 employed. PyMovie handles Lagarith compressed files without issue and without the
 need for the user to separately find and install a Lagarith codec.
 • Added the controls for dealing with field level avi stuff --- no code behind the controls
 yet
 • found a way to do random access reading of an avi file so it is no longer necessary to
@@ -1814,10 +1822,13 @@
 • added opencv-python to the required packages list so that Anaconda installations that
 lack this package (known as cv2) will have it automatically added
 • increased the allowed distance of computed masks from aperture center from 4 pixels
 to 6 pixels (this only comes into effect when there is a yellow aperture present
 • set thresh = 0 when aperture is created rather than None to deal with cases where an
 aperture is added where there is no image
 version 0.2.5
-• Initial Beta release – no timestamp OCR – functional for lightcurve extraction
+
+•
+
+Initial Beta release – no timestamp OCR – functional for lightcurve extraction
```

### Comparing `pymovie-3.7.7/src/pymovie/SER.py` & `pymovie-3.7.9/src/pymovie/SER.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/alias_lnk_resolver.py` & `pymovie-3.7.9/src/pymovie/alias_lnk_resolver.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/aperture.py` & `pymovie-3.7.9/src/pymovie/aperture.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/apertureEdit.py` & `pymovie-3.7.9/src/pymovie/apertureEdit.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/apertureEditDialog.py` & `pymovie-3.7.9/src/pymovie/apertureEditDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/apertureNameDialog.py` & `pymovie-3.7.9/src/pymovie/apertureNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/aperturesFileTagDialog.py` & `pymovie-3.7.9/src/pymovie/aperturesFileTagDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/astrometry_client.py` & `pymovie-3.7.9/src/pymovie/astrometry_client.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/checkForNewerVersion.py` & `pymovie-3.7.9/src/pymovie/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/gammaUtils.py` & `pymovie-3.7.9/src/pymovie/gammaUtils.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/gui.py` & `pymovie-3.7.9/src/pymovie/gui.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/helpDialog.py` & `pymovie-3.7.9/src/pymovie/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/hotPixelDialog.py` & `pymovie-3.7.9/src/pymovie/hotPixelDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/main.py` & `pymovie-3.7.9/src/pymovie/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,20 +426,22 @@
         self.ocrDigitsDir = self.homeDir
 
         self.firstYellowApertureX = None
         self.firstYellowApertureY = None
         self.secondYellowApertureX = None
         self.secondYellowApertureY = None
 
-        # self.pixel_sums = []
+        self.thumbTwoScaleFactor = 1.0
 
         self.sorted_masked_data = None
 
         self.naylorInShiftedPositions = None
 
+        self.extractionMode = 'Aperture Photometry'
+
         self.target_psf = None
         self.psf_radius_in_use = None
         self.fractional_weights = None
         self.sum_fractional_weights = None
         self.target_psf_number_accumulated = np.int64
         self.recordPsf = False
         self.target_psf_gathering_in_progress = False
@@ -2423,14 +2425,22 @@
             self.showMsgPopup('psf-stars require a minimum aperture size of 21')
             return
 
         self.addStaticAperture(askForName=False, name='psf-star-for-NRE', radius=8.0)
         self.testForConsistentPsfStarFixedMasks()
 
     def addApertureStack(self):
+        # It's ok to add a static mask aperture stack to a "finder" frame
+        # if self.finderFrameBeingDisplayed:
+        #     self.showMsgPopup(f'Aperture stacks cannot be added to "finder" images.\n\n'
+        #                       f'Best practice is to add a single static aperture at the target star position,\n'
+        #                       f'then advance 1 frame to exit the "finder" frame and add any\n'
+        #                       f'additional apertures.')
+        #     return
+
         nest_number = 1
         for app in self.getApertureList():
             if app.name.startswith('static-nest2'):
                 self.showMsgPopup(f'There are already two static nests in place - that is the limit.')
                 return
         for app in self.getApertureList():
             if app.name.startswith('static-nest'):
@@ -2443,14 +2453,21 @@
             if app.color == 'green':
                 app.setRed()
 
     def addDynamicApertureStack(self):
         if self.image is None:  # Don't add an aperture if there is no image showing yet.
             return
 
+        if self.finderFrameBeingDisplayed:
+            self.showMsgPopup(f'Aperture stacks cannot be added to "finder" images.\n\n'
+                              f'Best practice is to add a single static aperture at the target star position,\n'
+                              f'then advance 1 frame to exit the "finder" frame and add any\n'
+                              f'additional apertures.')
+            return
+
         for app in self.getApertureList():
             if app.name.startswith('dynamic-nest2'):
                 self.showMsgPopup(f'There are already two dynamic nests in place - that is the limit.')
                 return
 
         nest_number = 1
         for app in self.getApertureList():
@@ -6240,14 +6257,20 @@
         self.threshValueEdit.setValue(self.big_thresh)  # Causes call to self.changeThreshold()
         return
 
     def addSnapAperture(self):
         if self.image is None:  # Don't add an aperture if there is no image showing yet.
             return
 
+        if self.finderFrameBeingDisplayed:
+            self.showMsgPopup(f'Dynamic mask apertures cannot be added to "finder" images.\n\n'
+                              f'Best practice is to add a single static aperture at the target star position,\n'
+                              f'then advance 1 frame to exit the "finder" frame and add any\n'
+                              f'additional apertures.')
+            return
         self.one_time_suppress_stats = True
         aperture = self.addGenericAperture()  # Just calls addApertureAtPosition() with mouse coords
 
         self.nameAperture(aperture)
 
         if not 'psf-star' in aperture.name:
             self.computeInitialThreshold(aperture)
@@ -6389,15 +6412,15 @@
         if not self.showMissingModelDigits():
             self.acceptAviFolderDirectoryWithoutUserIntervention = True
             self.startTimestampReading()
             self.showMsg(f'Training completed.')
             self.showFrame()
 
     def addApertureAtPosition(self, x, y, custom_default_mask_radius=None):
-        # custom_default_mask_radius is used for 'add stack of 5 apertures' to generate 'russian doll' mask set
+        # custom_default_mask_radius is used for 'add stack of 12 apertures' to generate 'russian doll' mask set
 
         x0 = x - self.roi_center
         y0 = y - self.roi_center
         xsize = self.roi_size
         ysize = self.roi_size
         bbox = (x0, y0, xsize, ysize)
 
@@ -9519,15 +9542,15 @@
         # good_mean, sigma, sorted_data, hist_data, window, data_size, left, right = robustMeanStd(self.thumbOneImage)
         # calced_mean, bkgnd_sigma, sorted_data, my_hist, data.size / 2, data.size, 0, clip_point + 1, bkgnd_values
         good_mean, sigma, _, hist_data, _, _, _, local_right, *_ = newRobustMeanStd(
             self.thumbOneImage, lunar=self.lunarCheckBox.isChecked()
         )
         # self.showMsg(f'{good_mean} {sigma} {window} {data_size} {left}  {right}')
 
-        # TODO This was put here just for testing/development - it is used in newRobustMean()
+        # Version 3.7.8
         max_area, _, negative_mask, *_ = remove_stars(
             img=self.thumbOneImage,
             cut=good_mean + 1 * sigma
         )
 
         # Start a new plot
         self.plots.append(pg.GraphicsLayoutWidget(title="Robust Mean Calculation"))
```

### Comparing `pymovie-3.7.7/src/pymovie/ocr.py` & `pymovie-3.7.9/src/pymovie/ocr.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/ocrCharacterBox.py` & `pymovie-3.7.9/src/pymovie/ocrCharacterBox.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/ocrProfileNameDialog.py` & `pymovie-3.7.9/src/pymovie/ocrProfileNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/play-Temp.py` & `pymovie-3.7.9/src/pymovie/play-Temp.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/play-introspection.py` & `pymovie-3.7.9/src/pymovie/play-introspection.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/selectHotPixelProfile.py` & `pymovie-3.7.9/src/pymovie/selectHotPixelProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/selectProfile.py` & `pymovie-3.7.9/src/pymovie/selectProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/stacker.py` & `pymovie-3.7.9/src/pymovie/stacker.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/starPositionDialog.py` & `pymovie-3.7.9/src/pymovie/starPositionDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie/wcs_helper_functions.py` & `pymovie-3.7.9/src/pymovie/wcs_helper_functions.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.7/src/pymovie.egg-info/PKG-INFO` & `pymovie-3.7.9/src/pymovie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.7.7
+Version: 3.7.9
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.7.7/src/pymovie.egg-info/SOURCES.txt` & `pymovie-3.7.9/src/pymovie.egg-info/SOURCES.txt`

 * *Files identical despite different names*


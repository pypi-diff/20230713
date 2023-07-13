# Comparing `tmp/pymovie-3.7.9.tar.gz` & `tmp/pymovie-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymovie-3.7.9.tar", last modified: Thu Jul 13 14:35:39 2023, max compression
+gzip compressed data, was "pymovie-3.8.0.tar", last modified: Thu Jul 13 21:33:04 2023, max compression
```

## Comparing `pymovie-3.7.9.tar` & `pymovie-3.8.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.421261 pymovie-3.7.9/
--rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.7.9/LICENSE
--rw-rw-rw-   0        0        0     1474 2023-07-13 14:35:39.421261 pymovie-3.7.9/PKG-INFO
--rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.7.9/README.rst
--rw-rw-rw-   0        0        0       80 2023-07-13 14:35:39.422269 pymovie-3.7.9/setup.cfg
--rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.273163 pymovie-3.7.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.417270 pymovie-3.7.9/src/pymovie/
--rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.7.9/src/pymovie/NE3Lut.p
--rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.7.9/src/pymovie/PyMovie-doc.pdf
--rw-rw-rw-   0        0        0   631051 2023-07-13 14:33:12.000000 pymovie-3.7.9/src/pymovie/PyMovie-info.pdf
--rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.7.9/src/pymovie/PyMovie.bat
--rw-rw-rw-   0        0        0     6283 2023-05-12 20:27:48.000000 pymovie-3.7.9/src/pymovie/SER.py
--rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.7.9/src/pymovie/__init__.py
--rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.7.9/src/pymovie/alias_lnk_resolver.py
--rw-rw-rw-   0        0        0     6094 2023-05-18 11:24:11.000000 pymovie-3.7.9/src/pymovie/aperture.py
--rw-rw-rw-   0        0        0    15254 2023-06-27 02:54:33.000000 pymovie-3.7.9/src/pymovie/apertureEdit.py
--rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.7.9/src/pymovie/apertureEditDialog.py
--rw-rw-rw-   0        0        0     3962 2023-06-26 17:44:10.000000 pymovie-3.7.9/src/pymovie/apertureNameDialog.py
--rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.7.9/src/pymovie/aperturesFileTagDialog.py
--rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.7.9/src/pymovie/astrometry_client.py
--rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.7.9/src/pymovie/checkForNewerVersion.py
--rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.7.9/src/pymovie/gammaUtils.py
--rw-rw-rw-   0        0        0   233704 2023-06-26 17:44:13.000000 pymovie-3.7.9/src/pymovie/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-24 18:07:02.000000 pymovie-3.7.9/src/pymovie/helpDialog.py
--rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.7.9/src/pymovie/hotPixelDialog.py
--rw-rw-rw-   0        0        0   456486 2023-07-13 14:26:39.000000 pymovie-3.7.9/src/pymovie/main.py
--rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.7.9/src/pymovie/ocr.py
--rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.7.9/src/pymovie/ocrCharacterBox.py
--rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.7.9/src/pymovie/ocrProfileNameDialog.py
--rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.7.9/src/pymovie/play-Temp.py
--rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.7.9/src/pymovie/play-introspection.py
--rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.7.9/src/pymovie/run-pymovie-mac.bat
--rw-rw-rw-   0        0        0     4271 2023-05-31 13:21:53.000000 pymovie-3.7.9/src/pymovie/selectHotPixelProfile.py
--rw-rw-rw-   0        0        0     3675 2023-05-31 04:05:11.000000 pymovie-3.7.9/src/pymovie/selectProfile.py
--rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.7.9/src/pymovie/stacker.py
--rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.7.9/src/pymovie/starPositionDialog.py
--rw-rw-rw-   0        0        0       36 2023-07-07 20:58:41.000000 pymovie-3.7.9/src/pymovie/version.py
--rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.7.9/src/pymovie/wcs_helper_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:35:39.421261 pymovie-3.7.9/src/pymovie.egg-info/
--rw-rw-rw-   0        0        0     1474 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.7.9/src/pymovie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      247 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 14:35:38.000000 pymovie-3.7.9/src/pymovie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 21:33:04.007579 pymovie-3.8.0/
+-rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.8.0/LICENSE
+-rw-rw-rw-   0        0        0     1474 2023-07-13 21:33:04.007579 pymovie-3.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.8.0/README.rst
+-rw-rw-rw-   0        0        0       80 2023-07-13 21:33:04.012588 pymovie-3.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:33:03.974509 pymovie-3.8.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:33:03.998579 pymovie-3.8.0/src/pymovie/
+-rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.8.0/src/pymovie/NE3Lut.p
+-rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.8.0/src/pymovie/PyMovie-doc.pdf
+-rw-rw-rw-   0        0        0   633433 2023-07-13 21:31:24.000000 pymovie-3.8.0/src/pymovie/PyMovie-info.pdf
+-rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.8.0/src/pymovie/PyMovie.bat
+-rw-rw-rw-   0        0        0     6283 2023-05-12 20:27:48.000000 pymovie-3.8.0/src/pymovie/SER.py
+-rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.8.0/src/pymovie/__init__.py
+-rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.8.0/src/pymovie/alias_lnk_resolver.py
+-rw-rw-rw-   0        0        0     6094 2023-05-18 11:24:11.000000 pymovie-3.8.0/src/pymovie/aperture.py
+-rw-rw-rw-   0        0        0    15254 2023-06-27 02:54:33.000000 pymovie-3.8.0/src/pymovie/apertureEdit.py
+-rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.8.0/src/pymovie/apertureEditDialog.py
+-rw-rw-rw-   0        0        0     3962 2023-06-26 17:44:10.000000 pymovie-3.8.0/src/pymovie/apertureNameDialog.py
+-rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.8.0/src/pymovie/aperturesFileTagDialog.py
+-rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.8.0/src/pymovie/astrometry_client.py
+-rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.8.0/src/pymovie/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.8.0/src/pymovie/gammaUtils.py
+-rw-rw-rw-   0        0        0   233704 2023-06-26 17:44:13.000000 pymovie-3.8.0/src/pymovie/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-24 18:07:02.000000 pymovie-3.8.0/src/pymovie/helpDialog.py
+-rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.8.0/src/pymovie/hotPixelDialog.py
+-rw-rw-rw-   0        0        0   456966 2023-07-13 21:23:15.000000 pymovie-3.8.0/src/pymovie/main.py
+-rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.8.0/src/pymovie/ocr.py
+-rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.8.0/src/pymovie/ocrCharacterBox.py
+-rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.8.0/src/pymovie/ocrProfileNameDialog.py
+-rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.8.0/src/pymovie/play-Temp.py
+-rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.8.0/src/pymovie/play-introspection.py
+-rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.8.0/src/pymovie/run-pymovie-mac.bat
+-rw-rw-rw-   0        0        0     4271 2023-05-31 13:21:53.000000 pymovie-3.8.0/src/pymovie/selectHotPixelProfile.py
+-rw-rw-rw-   0        0        0     3675 2023-05-31 04:05:11.000000 pymovie-3.8.0/src/pymovie/selectProfile.py
+-rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.8.0/src/pymovie/stacker.py
+-rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.8.0/src/pymovie/starPositionDialog.py
+-rw-rw-rw-   0        0        0       36 2023-07-13 20:33:37.000000 pymovie-3.8.0/src/pymovie/version.py
+-rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.8.0/src/pymovie/wcs_helper_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:33:04.006580 pymovie-3.8.0/src/pymovie.egg-info/
+-rw-rw-rw-   0        0        0     1474 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.8.0/src/pymovie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      247 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/top_level.txt
```

### Comparing `pymovie-3.7.9/LICENSE` & `pymovie-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/PKG-INFO` & `pymovie-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.7.9
+Version: 3.8.0
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.7.9/setup.py` & `pymovie-3.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/PyMovie-doc.pdf` & `pymovie-3.8.0/src/pymovie/PyMovie-doc.pdf`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/PyMovie-info.pdf` & `pymovie-3.8.0/src/pymovie/PyMovie-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -3,14 +3,25 @@
 For general information about the program (with usage tips), click on the
 Documentation button that is in the Help tab panel. A pdf will be launched – it
 is out-of-date, but still a bit useful.
 Note: there is a series of (grossly out-of-date and nearly useless and possibly
 confusing) YouTube tutorials available. Go to
 http://occultations.org/observing/software/pymovie for access to these videos.
 PyMovie version history
+Version 3.8.0
+13 July 2023
+• If data was already gathered, then an aperture was renamed to psf-star, the NRE
+analysis would not run UNLESS the user manually cleared the already gathered data.
+This version detects that case and starts the psf gathering process as expected.
+•
+
+If a long analysis was started and the program closed, the analysis continued to run in
+a background thread. This version detects that case and stops the background thread
+whenever the program is closed.
+
 Version 3.7.9
 13 July 2023
 • Fixed a bug that caused 3.7.8 to fail with message PyMovie has no attribute
 extractionMethod
 Version 3.7.8
 6 July 2023
 • Added ‘best practices’ message popup when a user attempts to add a non-static mask
@@ -24,26 +35,27 @@
 • Changed the centering/tracking of fixed radius masks (in static apertures) from
 centering on the single brightest pixel (introduced in version 3.7.0) to a mass centroid
 calculated using the nThBrightPixel algorithm conceived and tested by A. G. Basden
 (reported in Centroids using Brightest Pixel Algorithm by A. G. Basden, et al, MNRAS,
 2011)
 This operates by finding the n brightest pixels in the mask, setting all other pixel values
 to zero, and calculating the x,y centroid of the remaining ‘mass’.
-•
+
+•
 
 Optimal extraction for imaging photometry was introduced by Tim Naylor in his 1998
 paper titled: An optimal extraction algorithm for imaging photometry.[ Mon. Not.
 R. Astron. Soc. 296, 339-346 (1998)].
 Naylor's algorithm utilizes a two-dimensional gaussian as an approximation to the psf
 of stars in the image and demonstrates that this is an effective approximation in practice. Using this analytic psf, the paper describes how to calculate a weighted mask that
 lowers the noise in a star intensity measurement by giving a larger weight to those
 pixel that have a higher SNR and a lower weight to dimmer, noisier pixels - this is the
 core idea in all optimal extraction schemes.
 
-•
+•
 
 PyMovie uses the Naylor algorithm in the form that is optimal for sky-limited observations - i.e., dim targets - and can be used for occultations where the target completely
 disappears.
 
 •
 
 Added an item to the aperture placement menu to add a nest of 12 static apertures of
@@ -70,27 +82,27 @@
 an aperture placement that ‘worked’ so I found no problem.
 It is also the case that the problem is only visually identifiable for very short events that
 have a good snr, so it is easily overlooked.
 I believe that this bug has always been present – just undetected and confirmed until
 now.
 Version 3.7.3 11 February 2023
 • Restored the font size of the text box (lower left) that had inadvertently been increased
-to 13 back to 9
+
+to 13 back to 9
 •
 
 Restored use of pyqtgraph 0.12.4
 
 Version 3.7.0 7 February 2023
 • Added an additional tracking feature to static apertures. In previous versions, the fixed
 radius circular sampling mask was always centered inside a static aperture. Tracking
 the enclosed star image was indirect, depending on some other ‘tracking aperture’
 placed elsewhere in the frame on a tracking star. But the position of the target star
 relative to the tracking star is not constant but jitters due to atmospheric turbulence, so
-
-a relatively large circular mask had to be used around the target star so that the
+a relatively large circular mask had to be used around the target star so that the
 jittering target star remained inside the circular mask. This version adds tracking to the
 fixed circular mask inside the aperture itself. It operates by finding the brightest pixel
 visible in a centered mask, then recentering the mask around that bright pixel. (A
 ‘bright pixel is defined as being at or above 1 std deviation above background.)
 It is now possible to more effectively lower the noise in an extracted target star
 lightcurve by using smaller and smaller circular masks to find the one that improves the
 noise best. This was possible in the past, but because positional jitter was not adjusted
@@ -113,30 +125,27 @@
 • Removed instructions for pipenv installations (we have killed that project before it is
 actually born)
 Version 3.6.5 5 September 2022
 • No code changes. Added ‘wheel’ to required packages to better support pure Python
 installations (no Anaconda3).
 Version 3.6.3 7 August 2022
 • Added messages upon app closing indicating normal program shutdown with advice to
-user to ignore any subsequent messages about QBasic timers as they are harmless.
+
+user to ignore any subsequent messages about QBasic timers as they are harmless.
 Version 3.6.2 7 August 2022
 • At one point in time (see version 3.2.0 and 3.2.1 discussion) a ‘hack’ was introduced to
 get Windows to preserve any image scaling and positioning during frame changes. The
 hack was to expand and contract the width of the image by 1 pixel. This ‘dance’ is
 sometime apparent. This version removes that ‘hack’ as it appears no longer
 necessary on Win10 or Win11.
 Version 3.6.1 7 August 2022
-
-•
-
-During timestamp OCR setup, frame 0 is often messed up during recording and so
+• During timestamp OCR setup, frame 0 is often messed up during recording and so
 should not be used for sampling timestamp characters. This version detects that
 situation and automatically advances to frame 1 with a pop-up message alerting the
 user that this action has been performed.
-
 Version 3.6.0 29 July 2022
 • fixes OCR context menu and plots
 Version 3.5.6 26 July 2022
 • fixes aperture context menu. OCR context menu still broken
 Version 3.5.1 23 July 2022
 • it appears that the PyPI JSON API is no longer useful for getting the latest version of a
 package due to an announced breaking change on the part of the PyPI support team.
@@ -155,24 +164,24 @@
 Version 3.4.3 21 July 2022
 • removed option to download new version when found. This was done in part to remove
 a sometimes-annoying nag and to pave the way for a new installation procedure that
 does not require an Anaconda3 installation.
 The usual pip install pymovie==x.y.z remains available for the user to install any new
 version at a time of her choosing for the current installation procedure. For the new
 installation procedure, a batch file is provided that prompts for the new version number
-– one no longer hs to remember the magic incantation.
+
+– one no longer hs to remember the magic incantation.
 Version 3.4.2 9Jul2022
 • fixes QMenu() reference issue (created by Qt programmers changing where the
 QMenu() item is found
 Version 3.4.1 22Jun2022
 • cleans up some issues involving the color scale for the thumbnails.
 Version 3.4.0 18Jun2022
 • For some reason, I thought that 16 bit FITS file images should be scaled (divided by)
-
-by 16 because all current A/D are 12 bits. I now think that this is a bad idea and have
+by 16 because all current A/D are 12 bits. I now think that this is a bad idea and have
 returned to displaying 16 bit FITS image as 0 to 65535 pixel values.
 Version 3.3.9
 • adds display of WCS RA and DEC info (if available) in a popup box whenever
 the key w is pressed while the mouse cursor is pointing to a star.
 Version 3.3.7
 • enable cursor-over-image wcs annotation whenever a WCS solution has been
 obtained, even when the target is not in the field
@@ -198,27 +207,31 @@
 assumed recorded with gamma 0.75, be linearized. When this box is checked, the
 'gamma' response curve of the Night Eagle 3 will be inverted so that the response
 becomes very close to linear.
 Version 3.3.0
 • removes the requirement for a specific version of opencv-python – this was causing
 problems with new Anaconda installs of Python 3.9
 Version 3.2.9
-• fixes bug where meta-data from adv file was being placed in csv file without leading #
+
+•
+
+fixes bug where meta-data from adv file was being placed in csv file without leading #
 character
+
 Version 3.2.7
 • The CMOS Pixels Tool tab is now fully functional.
 There is too much in this tab to explain in this forum – start your education with the
 Click me for help/info button. Then do right clicks on the other controls, starting at the upper
 left and procedding down the column, then move to the upper right.
 •
 
 I removed the 3x3 and 5x5 median filter options from the CCD Hot Pixels tab – they
-
-were not useful in any meaningful context and mostly just corrupted (smeared) the
+were not useful in any meaningful context and mostly just corrupted (smeared) the
 images that they were applied to.
+
 Version 3.2.6
 • improves help messages to give better guidance during use of the hot-pixel removal
 tab functions
 Presages the CMOS hot pixel tab functions to be added soon.
 Version 3.2.5
 • at the suggestion of a user, the version adds the name of the fits file that contains the
 currently displayed image to the file-in-use text box at the upper left. Of course this
@@ -244,25 +257,28 @@
 • fixed issue where contrast level settings were not being preserved when an analysis
 was started
 •
 
 reduced 'blinking' of thumbnail One image during image changes.
 
 Version 3.2.1
-• added an ugly hack to the Windows version in order to make what worked so easily in
+
+•
+
+added an ugly hack to the Windows version in order to make what worked so easily in
 version 3.2.0 on Mac hardware also work on Windows machine – it took me two full
 days to find this 'hack' and still I hate that it's necessary.
+
 Version 3.2.0
 • has changed so that Zoom/Pan state of main image is preserved when switching back
 and forth between a 'finder' image and a frame image
 Version 3.1.6
 • fixes a bug that kept the use of yellow aperture mask (for windshake files) from
 displaying properly in Thumbnail Two
-
-Version 3.1.5
+Version 3.1.5
 • added code for converting FITS files that are in 64 bit float format to uint16. If the
 image pixels contained negative values (because they didn't actually come from a
 camera but some post-processing procedure), then frame by frame the image will have
 an amount added to it so that the smallest pixel value will become 1.0
 Version 3.1.4
 • fixed a typo introduced while reverting to the non-scrollable GUI.
 Version 3.1.3
@@ -284,25 +300,25 @@
 • changed median filter to adjust all horizontal lines to have a median equal the median
 of the row-by-row medians (previously I was adjusting all lines to the maximum of the
 row-by-row medians). This will make the brightness adjustments less radical.
 Version 3.0.9
 • adds options for the user when she starts an analysis and there is already data
 present: she can ignore the warning and continue because her settings will not
 produce duplicate frames; she clear the data and proceed into the analysis; she can
-stop the analysis.
+
+stop the analysis.
 Version 3.0.8
 • adds clearing of line filter checkbox when new file is loaded. The display of the median
 plot is now a one-time event, as there was a need to clear that data in preparation of a
 new 'run'. This avoids duplicated and overlaid data in that array.
 Version 3.0.7
 • adds a median filter to reduce/eliminate 'line pattern noise' that some cameras exhibit.
 Such 'patterning' appears as row to row differences in brightness – streaks – that are
 consistently there. The median filter adjust each row indiviudally so that all rows and up
-
-having having the same median, and the 'line patterning' disappears.
+having having the same median, and the 'line patterning' disappears.
 This new feature can be found in the Misc. tab.
 Version 3.0.5
 • Adds a warning message if a user starts an analysis when there is already data
 present from a previous analysis run. This is an allowed condition (it allows running an
 analysis backwards or some part forward and the rest backwards to deal with a difficult
 tracking situation) but may cause some frames to be processed more than once. If that
 happens, attempts to write a csv file file with a duplicated frame message. With this
@@ -324,28 +340,29 @@
 • same as version 2.9.8 but the new scrollable area now scales with the size of the main
 window as it always did before.
 Version 2.9.8
 • changes the routine that looks for the latest version of PyMovie to one provided by Kia
 Getrost. His version contacts the PyPI repository via a json query and is the officially
 supported way to get version info. My version was based on a 'hack' that depended on
 a special feature of pip (the loader that get programs from the PyPI repository) that
-was marked as 'unsupported'. That worked for many years until the pip programmers
+
+was marked as 'unsupported'. That worked for many years until the pip programmers
 removed the 'special feature' as was their right (and promise, I guess). This caused
 several users to always get a message that they were not running the most recent
 version of PyMovie, even though they were. Again: thanks to Kia Getrost for
 researching the problem and even supplying correct code (worked first time!) for me to
 use.
 •
 
 The GUI has been changed so that scroll bars will appear when the standard GUI size
 exceeds your screen dimensions. THIS IS EXPERIMENTAL BECAUSE I DO NOT
 HAVE SUCH A SMALL SCREEN TO TEST WITH. If this does not work for you, please
 let me know immediately!
 
-Version 2.9.7
+Version 2.9.7
 • adds interlock so that use of yellow mask as the default mask cannot be enabled
 unless there is a yellow aperture present.
 Version 2.9.6
 • cures a ThumbNailTwo coloring issue when the default mask is set to Yellow Mask
 (FYI: the selection box for this option is in the Misc tab)
 Version 2.9.5
 • this change affects ONLY videos processed in field mode. Field mode processing is
@@ -375,29 +392,25 @@
 created, OCR will be ready to go.
 
 ◦
 
 If you have a need for more than one OCR profile, you can still use the save/load
 OCR profile mechanism, which remains untouched.
 
-Version 2.9.3
+Version 2.9.3
 • changed the handling of ‘sticky values’ (like folder paths) to force the update of the
 ‘sticky file’ whenever a new folder is opened (to solve the issue where ‘save dialogs’
 sometimes have a previous folder path rather than the current folder path and so
 tricking the unwary user into storing a file unintentionally into the wrong folder)
 Version 2.9.2
 • added forced install of version 4.1.2.30 of opencv-python to (hopefully) eliminate the qt
 plugin errors that occur on Mac installations.
 Version 2.9.1
-
-•
-
-added auto-install of opencv-python-headless and numpy>=1.17.0 in hopes of better
+• added auto-install of opencv-python-headless and numpy>=1.17.0 in hopes of better
 dealing with older installations on Anaconda3
-
 Version 2.9.0
 • red colorization has been added to pixels displayed in the Thumbnails that are at or
 above a value specified by the user (there is a place to enter this value just below the
 Show image contrast control check box.
 There is a new meaning to the values of minpx and maxpx (reported in the text box at
 the lower left) --- previously, these reported the min and max pixel values from the
 entire aperture; now they are the min and max pixel values of the pixels that have been
@@ -418,25 +431,25 @@
 • changed the meta-tag that is examined for the QHY174M GPS status from GPS_STAT
 to GPSSTAT
 Version 2.8.5
 • adds special detection for FITS files from QHY174M cameras that have a GPS status
 of PartialData. In this case the normal timestamp meta-data tag (DATE-OBS) is invalid,
 but there is a belief that a timestamp can be computed from two other meta-data tags
 that do get filled in: GPS_ST and GPS_SU. Such a timestamp will almost certainly
-contain errors, but the observer may be able to figure out a common offset to apply to
+
+contain errors, but the observer may be able to figure out a common offset to apply to
 make them correct, so we are outputting GPS_ST + (GPS_SU / 1,000,000) in this
 special case. This change will be completely transparent – it will not affect QHY frames
 that have a GPS Locked status.
 Version 2.8.4
 • fixed issue that caused the initial display of a help message that was too big for the
 panel to be scrolled to the bottom (obscuring the first few lines) rather than the top.
 Version 2.8.3
 • adds an explicit Timestamp setup help button in the Timestamp tabbed panel. While
-
-help was available by right-clicking the Select VTI: label, that's not an obvious thing to
+help was available by right-clicking the Select VTI: label, that's not an obvious thing to
 do, hence the added button.
 Version 2.8.2
 • adds a color change to OCR selection boxes based on their ability to be jogged. A red
 selection box (which can't be jogged by the arrow keys) turns yellow whenever it is
 enabled for arrow key jogging. I added some clarification to the Kiwi instructions
 regarding selection box placement.
 A major aid in adjusting the selection boxes to center on the timestamp characters has
@@ -460,24 +473,24 @@
 Version 2.7.9
 • changes the way the WCS procedure submits a request to nova.astrometry.net. Where
 previously, the submission to nova deliberately restricted the search to a 1 degree
 radius around the target star location, I now allow a full blind-search.
 Restricting the search to a small region was done to give nova.astrometry.net a much
 more limited selection of catalogs to search in the interest of speed. In my latest test
 case, a restricted search took 0.43 seconds of computer time at nova, while a blind
-search took 4.5 seconds of computer time.
+
+search took 4.5 seconds of computer time.
 The problem with a restricted search however is that if an error is made such that the
 target star is actually not in the image submitted, the search will simply fail quietly (and
 use a lot of computer time at nova to reach this conclusion!) without giving the user any
 clue as to why no solution could be found.
 With this version, I do a blind-search and if a solution is returned, I check to see if the
 target star is within the image and alert the user if the target star is not visible in the
 image.
-
-Version 2.7.8
+Version 2.7.8
 • Added a test for duplicated frames during the writing of a csv file and now abort the csv
 write should there be a duplicated frame found (caused by the user doing multiple
 overlapping analysis runs by accident).
 Version 2.7.7
 • Added an automatic 'Clear Data' at conclusion of 'finder image' generation do get rid of
 the aperture data that is collected during that operation.
 Version 2.7.6
@@ -502,25 +515,28 @@
 shape may be.
 •
 
 Changed the default threshold for static aperture from 9999 to 99999 to better
 accommodate 12 and 16 bit videos.
 
 Version 2.7.0
-• A small change to the Robust Mean algorithm so that it can be used on “finder” images
+
+•
+
+A small change to the Robust Mean algorithm so that it can be used on “finder” images
 (which have floating point values) as well as single-frame images (which have only
 integer values).
+
 Version 2.6.9
 • Changed the 'help/info' for the Plot Robust Mean button to better explain the algorithm.
 Version 2.6.8
 • Changed the algorithm for calculating the average value of background pixels. This
 new algorithm replaced one that was excellent when background noise had a gaussian
 distribution, but had about a 1% error (too small by 1%) when the noise distribution
-
-was skewed. The histogram of a skewed distribution has a longer tail on one side than
+was skewed. The histogram of a skewed distribution has a longer tail on one side than
 the other. It is common to find recordings that have background noise that is skewed,
 usually with a longer tail on the right (toward higher values). Sometime, perhaps due
 to a camera setting, background levels are 'clipped' and so appear skewed, sometimes
 without a left tail at all. One other effect is frequently seen in 8 bit avi from a composite
 video camera --- missing values. These 'missing' values appear when a video with a
 range of pixel values from 10 to 235 is remapped (stretched) to a 0 to 255 range.
 When that process is present, every eighth value is missing and never appears as a
@@ -542,24 +558,24 @@
 • With this version, the case of a non-version 2 ADV file is treated more gracefully --- just
 printing a message in the text box rather than a session-ending exception.
 Version 2.6.2
 • Added requirement that top/bottom redact values be entered (in the “finder” tab panel)
 before hot-pixel suppression via median filter will take place. This is needed for the
 case where a timestamp overlay is present that requires OCR. The median filter
 process has to bypass the region where such timestamps are located, otherwise poor
-OCR will be a result.
+
+OCR will be a result.
 Version 2.6.1
 • Working with Hristo Pavlov, I have added support for reading Version 2 ADV files (Astro
 Digital Video files) to PyMovie.
 A side effect of our collaborative effort is that there is now a publicly available Python
 package on PyPI.org for reading .adv files (Version 2) --- the package is called Adv2
 and is available to any Python programmer by the usual pip install Adv2. The
 project and its documentation can be viewed at https://pypi.org/project/Adv2/
-
-While being able to read .adv files is a pre-requisite to reading AAV files, it is likely that
+While being able to read .adv files is a pre-requisite to reading AAV files, it is likely that
 some additional capabilities will need to be added to PyMovie to deal smoothly with
 such files. If the demand is there for such support and is made known to me, I will
 undertake adding the missing pieces.
 •
 
 Added an option to apply either a 3x3 or a 5x5 median filter to frames as they are
 being read --- this has the effect of removing hot-pixels automatically, provided the 'hotpixels' are isolated pixels or in very small groups. This is a much easier option than
@@ -588,23 +604,22 @@
 mechanism. It was finicky, had no benefits over the simple to use and understand
 stacking using a single tracking star, and fails on images without dominant features.
 •
 
 Also made the name of the aperture to be used for stacking case-insensitive. It must
 still start with the character string 'stack', but 'StAcK' will work just as well.
 
-Version 2.5.6
+Version 2.5.6
 • In version 2.5.4 we switched to using a filename dialog that provided a list of alreadyused .csv file names, a useful convenience on occassion. Unfortunately, another
 characteristic of that file dialog is that it allowed the user to specify a filename that did
 not have a .csv extension. This version adds code to append a .csv extension to any
 filename the user provides that does not already have such an extension.
 Version 2.5.5
 • Squashed bug that kept avi files recorded with a dvsd codec from being read.
-
-Version 2.5.4
+Version 2.5.4
 • When writing a csv file or saving an aperture group, the dialogs now let you see what
 names you have used in the past.
 •
 
 CAUTION: the use of a computed mask (i.e., a snap-to-blob aperture) for the sole
 aperture that contains the target star, particularly if the target intensity drops
 significantly during the occultation, is not recommended! If you use a single
@@ -633,32 +648,27 @@
 but FITS files can be float64 (signed) and cannot always be converted to uint16. I
 doubt any users will have noticed this, but one of my test data sets is a video of the
 Pluto occultation that was greatly 'massaged' and as a result came to me as a signed
 float64 file.
 •
 
 Fixed: memory leak associated with plots --- some users (and me during testing) found
-that pymovie memory usage increased with time, eventually crashing --- I have traced
+
+that pymovie memory usage increased with time, eventually crashing --- I have traced
 that behavior down to the plot lightcurves function and eliminated the problem. A side
 effect of the 'fix' is that plots from a previous will no longer persist but rather will be
 automatically deleted, closed, and replaced by new plots. For some users, this may
 affect your workflow if you were in the habit of running an analysis, plotting the results,
 and running a changed analysis expecting to be able to generate another set of plots
 without losing the first set. If this was your practice, now you will be required to
 explicitly save plots that you want to use for comparison studies.
-
 Version 2.5.1
 • Fixed: SER file folder selection was not enabling ‘save aperture group’ button.
-
-•
-•
-
-Fixed: Initial ‘save’ of aperture group was not enabling ‘restore aperture group’ button
-Changed: default aperture name from app00 to ap00
-
+• Fixed: Initial ‘save’ of aperture group was not enabling ‘restore aperture group’ button
+• Changed: default aperture name from app00 to ap00
 Version 2.5.0
 • Removed asinh scaling and normalization to 0...255 range in “finder” images. This will
 preserve star intensities and (hopefully) make “finder” images look more like the star
 chart. In addition, with this change, the contrast settings that are useful for an individual
 frame are also applicable to the “finder” image, so I make that setting ‘sticky’ during
 changes to and from a “finder” image.
 Version 2.4.9
@@ -681,24 +691,24 @@
 and used by me for reading SER files, timestamp conversion involved first converting
 to Julian date and then to an ISO timestamp. For some reason, the Julian date version
 was always exactly one day earlier than the value from my SharpCap routine. Since
 the SharpCap interpretation matches what is shown visually, I’m electing to use that
 method of timestamp calculation.
 Version 2.4.4
 • Solves a problem extracting SharpCap embedded timestamps on some Win10
-systems, which can have a default 32 bit integer rather than the 64 bit integer on Mac
+
+systems, which can have a default 32 bit integer rather than the 64 bit integer on Mac
 computers.
 Version 2.4.3
 • Solves another problem reading large SER files --- again unique to Win10
 environment.
 Version 2.4.2
 • Solves problem reading large SER files that was unique to Win10 --- reading large
 SER files on Mac was no problem.
-
-Version 2.4.1
+Version 2.4.1
 • Adds timestamp extraction from SharpCap 8 bit avi captures. SharpCap embeds a 64
 bit timestamp (from Windows computer clock --- number of 100ns ticks since midnight
 on 1 Jan 0001) in the first 8 bytes of each frame (upper left corner). With this version,
 there is an addition to the VTI drop-down list that allows this form of avi to enjoy
 automatic timestamp extraction.
 Version 2.3.9
 • Fixed font issue on Preferences tab and radio button behavior
@@ -728,30 +738,30 @@
 or 3) can be specified. They will be ‘saved’ when PyMovie is closed and applied when
 next PyMovie is started up.
 Version 2.3.3
 • Major rearranging of GUI elements to reduce clutter. Uses Tabs.
 •
 
 Note: the tabs can be dragged to rearrange (but won’t be sticky --- I may do that when I
-implement ‘preferences’)
 
+implement ‘preferences’)
 •
 
 Changed to use of 2 sigma(std) in automatic setting of threshold in snap-to-blob
 apertures.
 
 Version 2.3.1
 • Added test for astrometry.net failing to accept upload of image --- a failed upload
 happened once when astrometry.net was having some trouble --- so that a clear
 message to the user is produced.
 •
 
 Changed default mask radius from 5.3 (nearly always too big to be useful) to 3.2
+(which makes a smallish and roundish default mask of more useful size).
 
-(which makes a smallish and roundish default mask of more useful size).
 •
 
 Tracked down and solved some mysterious behavior associated with FITS files. After
 a deep dive, I discovered that all FITS files are written with data bytes ordered for a
 big-endian computer. We run on Intel, which is little-endian. Nearly all of my code did
 operations on image data using numpy, which detects and properly operates on either
 big or little-endian data. BUT, in my mask calculation, a routine is used that was ported
@@ -779,25 +789,25 @@
 To activate this type of stacking, place a snap-to-blob aperture with a name that starts
 with stack That’s the only change needed. This is the easiest and most reliable stack
 alignment algorithm and will follow windshake (which 2 point tracking does not).
 The priority of frame stacking algorithms is:
 1. ‘stack’ aperture
 2. 2 point tracking path
 3. Fourier Correlation
-Version 2.2.7
+
+Version 2.2.7
 • Adds the ability to save multiple sets of apertures (and any associated tracking path).
 When the Save aperture group button is clicked, a dialog will appear requesting that a
 ‘tag’ be supplied to give the 2 or 3 files that are used to record a saved aperture group
 a unique name. The tag is appended to a root name and when the Restore aperture
 group button is clicked, a list of available aperture groups will be presented for
 selection.
 Version 2.2.6
 • Many significant changes to finder image usage:
-
-It is now possible to generate and save multiple finder images. This is particularly
+It is now possible to generate and save multiple finder images. This is particularly
 helpful in the context of setting up for 2 point tracking. The procedure would be to
 generate a finder image at frame 10 (say) and another at frame 2500 (say). These will
 be saved as enhanced-image-10.fit and enhanced-image-2500.fit and can be restored
 by clicking the load finder image button --- there you can select the appropriate
 enhanced-image-nnn.fit file (or .bmp --- that’s still available so that RegiStax can be
 used as well). The appropriate frame number to position the video to will be extracted
 from the image name. These two finder images will be of assistance in positioning a
@@ -823,26 +833,25 @@
 keys is enabled. At the same time, jogging is disabled on all apertures. This change
 was made to make the process of positioning apertures on hot-pixels easier.
 It is still possible to individually enable/disable jogging on more than one aperture. The
 only change is when an aperture is first created.
 •
 
 Added hot-pixel removal from finder images. This is a user guided process --- the user
-must place small apertures on hot-pixel groups, set a threshold for identifying hotpixels, and clicking on a button that invokes a program looks through all of the
+
+must place small apertures on hot-pixel groups, set a threshold for identifying hotpixels, and clicking on a button that invokes a program looks through all of the
 apertures, prepares a list of the coordinates of all hot-pixels, and substitutes the
 average background for all hot-pixels.
-
 Version 2.2.4
 • On lightcurve plots: the composite light curve is back on top. I didn’t like it on the
 bottom so it is back to the top where it will stay. I did ensure that the order of adding
 curves to the composite lightcurve plot is based on the column order. In this way, if the
 target lightcurve is the first column in the csv plot, it will be the last added to the
 composite plot so its ‘dots’ will be on top.
-
-Version 2.2.3
+Version 2.2.3
 • When the lightcurves are plotted, the z-order of the composite light curve plot has been
 changed so that it is now the bottom-most plot rather than the topmost plot. In addition,
 the individual light curves will appear in the order specified by the order number of the
 aperture (this will match the column order in the csv file). So an aperture with order
 number 4 will be plotted on top of an aperture with order number 7. So the user now
 has complete control of the plot order for the individual lightcurves through judicious
 use of the aperture edit table invoked by clicking on the Examine/change aperture
@@ -868,24 +877,27 @@
 over’ and, without this change, if you click Restore aperture group, then Mark, then
 Restore aperture group again you got a duplicate set of apertures.
 
 Version 2.2.0
 • Made the ‘help’ text come up whenever the lunar box is checked. It serves as a
 warning.
 Version 2.1.9
-• Added a ‘lunar’ checkbox which should ONLY be used when an aperture is placed on a
+
+•
+
+Added a ‘lunar’ checkbox which should ONLY be used when an aperture is placed on a
 sunlit lunar limb for a lunar occultation.
 This is experimental: until this point, PyMovie has focussed on asteroid occultations
 only --- this is a deviation from that focus.
 When this box is checked, it signals the Robust Mean extraction routine to statistically
 separate sky pixels from lunar limb and star pixels for use in background calculations.
 This emulates what Limovie does when a properly oriented ‘Avoid Sunlit Face’ aperture
 is utilized and so should produce comparable lightcurves. Time will tell.
 
-Version 2.1.8
+Version 2.1.8
 • I now save tracking path data when an aperture group is saved.
 Version 2.1.7
 • Added the ability to set a ‘tracking path’ by specifying two points, one early in the video
 and one late in the video. This feature is primarily useful in processing difficult driftthrough videos where no other good options for tracking are present.
 To learn a bit more, right-click on a non-yellow aperture and then click one of the menu
 items involving ‘track path’. That will cause a help panel to appear.
 Version 2.1.6
@@ -906,19 +918,17 @@
 the menu of characters to record will show those that remain to be sampled, as it was
 before this version --- that feature speeds up the initial sampling of the digits. The
 change made in this version is that, if all digits have been sampled, a complete menu
 of digits to record will be produced when a digit is right-clicked so that any poorly
 sampled digit can be re-recorded without the need to start over from scratch.
 version 2.1.2
 • Added ability to correct pixel response curve for non-unity gamma setting of camera
-version 2.1.1
 
-•
-
-Modified the robust mean estimator to deal with videos that have ‘clipped’
+version 2.1.1
+• Modified the robust mean estimator to deal with videos that have ‘clipped’
 backgrounds, a situation that is surprisingly common.
 
 Here is a ‘normal’ RobustMean plot:
 It shows the usual gaussian background noise in a 51x51 pixel aperture with some stars in
 the aperture as well.
 But sometimes we see that somewhere in the processing chain (could be a camera setting --could be in the recording software) that some sort of 'clipping' has occurred. It exhibits as a
 'one-sided' noise distribution with many of the background pixel values equal to a fixed value.
@@ -931,37 +941,33 @@
 small (often 0.0) value for the estimated std and that causes mask threshold values to be set
 unreasonably low.
 The changed robust mean estimator, applied to the same 51x51 aperture produces:
 
 and the resulting standard deviation is much more realistic and produces a useful initial value
 for the mask threshold.
 Note: such clipping has an effect on photometry. It appears small, so can often be ignored,
-but if you can set your processing chain to avoid such clipping, that would be the
+
+but if you can set your processing chain to avoid such clipping, that would be the
 recommended way to go.
 version 2.1.0
 • Fixed math problem in robust mean estimator when 16 bit uints are involved (QHY
 FITS)
 version 2.0.9
 • Made a change to the ‘robust mean estimator’ to better deal with videos that have
 been (artificially) clipped so that the background has many 0 values. This shouldn’t
 have any affect on properly recorded backgrounds, but stay alert!
 version 2.0.8
 • Added ability to redact images from top and bottom simultaneously.
 • Modified IOTA timestamp ocr parser to allow for a 3 digit milliseconds field (fourth entry
 blank). This makes ocr timestamp reading possible for the smopiVTI by treating it as
 an IOTA VTI with repositioned character boxes.
 version 2.0.7
-
-•
-•
-
-Fixed 3D Thumbnail display (it got broken in version 2.0.2 when left to right image
+• Fixed 3D Thumbnail display (it got broken in version 2.0.2 when left to right image
 flipping was added)
-Changed Open AVI file button label to Open AVI/SER file.
-
+• Changed Open AVI file button label to Open AVI/SER file.
 version 2.0.6
 • Added PAL mode Kiwi OCR timestamp recognition. In PAL mode, Kiwi timestamp
 characters are vertical. In NTSC mode, the characters are slanted.
 version 2.0.5
 • Adds the ability to read 8 and 16 bit gray-scale (not color) SER files
 NOTE !!!! Quite a few changes were made to the code to add this capability.
 NOTE !!!! Although changes were carefully isolated and made specific to SER files,
@@ -974,32 +980,35 @@
 version 2.0.3
 • When in field mode and ocr selection boxes are present, moving the cursor into a
 character box automatically displays that character in the Thumbnails. This probably
 eliminates the need for the Show property menu item in the context menu, but we’ll
 leave that in place until we’re certain there is no longer a need for it.
 version 2.0.2
 • Added ability to use “finder” image as submission to nova.astrometry.net. This has
+
+•
+
 helped in at least one case, but use sparingly.
-• Added check box to allow flip of images left to right (around y axis)
+Added check box to allow flip of images left to right (around y axis)
+
 version 2.0.1
 • Negative values for line redaction was not working when used for an astrometry.net
 calibration. This oversight has been corrected.
 version 2.0.0
 • Fixed reading of FITS files --- had been reading as int16 --- should have been uint16
 • For “finder” image generation: added setting of background to zero (controlled by a
 threshold value that can be set by the user or automatically by the program) for
 creating ‘finder’ images. This is necessary so that the stacker aligns to star features
 rather than background features/texture.
 version 1.9.9
 • Major rewrite of manual WCS calibration code. Biggest change was to solve for the
 rotation angle between the RA/Dec and x/y coordinate systems numerically rather than
 with trig. This numerical solution tolerates all possible orientations. The change was
 necessitated when an alt-az example showed that the trig solution was too
-
-temperamental --- and there were problems earlier with inverted or flipped images that
+temperamental --- and there were problems earlier with inverted or flipped images that
 were dealt with as special cases and now can be treated without special code. The
 other change was to use a 2 x 2 rotation matrix to calculate the target x/y coordinates.
 The rotation matrix values depend only on the rotation angle between the RA/Dec and
 x/y coordinate systems, determined robustly by the numerical ‘search’ referred to
 earlier.
 version 1.9.8
 • IF you have enabled a SINGLE ocr selection box for jogging, jogging that box will
@@ -1015,15 +1024,16 @@
 This capability was added when one user encountered difficulty getting their arrow
 keys to be recognized. But if one user has a problem, others may follow.
 version 1.9.4
 • Made some GUI changes specific to Windows operation to deal with font differences
 between Mac and Windows platforms.
 version 1.9.3
 • Thanks to Christopher Bennett: he found and fixed some issues related to using
-PyMovie on Linux and posted his proposed changes as a pull-request in my GitHub
+
+PyMovie on Linux and posted his proposed changes as a pull-request in my GitHub
 pymovie repository. I have accepted and merged his changes --- AVI-WCS folders
 should now work properly on Linux systems.
 version 1.9.2
 • Fixed bug where retraining digits deleted template digits but was failing to allow
 retraining menu list to appear until the folder was reopened.
 version 1.9.1
 • When, in version 1.8.9, we added the option for an aperture stack, we decided to
@@ -1031,20 +1041,16 @@
 prompting (rudely) for an aperture name when a static aperture was being placed.
 Fixed it --- we’re back to prompting for an aperture name when a single static aperture
 is placed, but don’t prompt for names when a stack of 5 is placed.
 version 1.9.0
 • Updated the right-click help message for the Examine/change aperture settings button
 to reflect the new functionality of using the thumbnails to show aperture contents and
 either computed mask or default mask.
-
-•
-
-It is expected that this will be the version released for public use --- end of Beta testing
+• It is expected that this will be the version released for public use --- end of Beta testing
 --- start of production testing.
-
 version 1.8.9
 • Added a menu item to add a stack of 5 static apertures.
 • Also allow red apertures to ‘snap’ as their threshold is changed from the Aperture Edit
 list. Previously, on a ‘green’ aperture would snap.
 version 1.8.8
 • Made a ‘live’ connection between the Aperture List Dialog and the thumbnails so that is
 is easy to set default mask sizes and thresholds with a ‘live’ view of the effects. Also
@@ -1059,15 +1065,16 @@
 • Added message in textOut panel that PyOTE is starting up --- that process takes a few
 seconds and the user needs to know to be patient.
 • Updated the main documentation file to add a table of contents, hyperlinks, and an
 acronym list.
 version 1.8.5
 • Added automatic startup of PyOTE when a csv file is written. PyOTE will open and
 load that csv file.
-version 1.8.4
+
+version 1.8.4
 • Defaulted the lightcurve plot 'zoom' (drag with right button) to affect x axis only rather
 than both x and y at the same. There is a right-click context menu for each plot that
 let's you change how the right button drag is applied to x and y axis --- it is called
 Mouse Enabled and is individually settable for each axis.
 • Added a bit more text to the lower row of transport buttons to make them a little less
 cryptic at the expense of a little more real estate.
 version 1.8.3
@@ -1075,27 +1082,22 @@
 workflow-order.
 version 1.8.2
 • Added the ability to save an aperture configuration between 'runs'. Preserved is the
 frame showing when the Save aperture group button was clicked and the apertures
 showing at that time, including all of their properties. The configuration can be
 retrieved by clicking the Restore aperture group button.
 version 1.8.1
-
-•
-•
-
-Added +/- 1 frame buttons and removed the the up/down buttons on the current frame
+• Added +/- 1 frame buttons and removed the the up/down buttons on the current frame
 and stop frame spinners.
-Made it easy to change pixel dimensions during WCS operations. This is normally a
+• Made it easy to change pixel dimensions during WCS operations. This is normally a
 set-and-forget operation --- please do not experiment with dimensions to 'guess' at
 pixel dimensions --- that would be an abuse of nova.astrometry.net. A single test to
 prove that it does matter is ok. Figure out what your pixel dimensions are from camera
 specs/sensor chip manufacturer, not from inducing nova.astrometry.net to 'fail', which
 slows down the service for everyone world-wide.
-
 version 1.8.0
 • 'play' was not initializing tracking --- added the needed initialization so that 'play' will
 show exactly what would happen during an analysis.
 version 1.7.9
 • Fixed indexing problem with lightcurve plots in field mode that was causing incorrect
 frame numbers to be displayed as hairline was moved.
 version 1.7.8
@@ -1103,15 +1105,17 @@
 version 1.7.7
 • Added timestamp to data displayed as hairline is dragged across a lightcurve plot.
 version 1.7.6
 • During manual WCS calibration, adjusted assignment of RA DEC values to reflect the
 center of the pixel, rather than the upper left corner.
 version 1.7.5
 • Corrected the display of WCS coordinates that appear in the status bar (when
-astrometry.net solution is active in a frame) when the cursor is inside the image --these values needed to take into account pixel aspect ratio.
+astrometry.net solution is active in a frame) when the cursor is inside the image ---
+
+these values needed to take into account pixel aspect ratio.
 version 1.7.4
 • Added non-square camera pixel compensation to manual WCS calibration. That
 compensation is now in place for both WCS calibration methods: nova.astrometry.net
 and 2-star manual
 version 1.7.3
 • Added compensation for pixel aspect ratio (W/H) for submissions to astrometry.net.
 This deals properly with non-square camera pixels by resizing the image submitted to
@@ -1120,23 +1124,18 @@
 
 This compensation is NOT YET incorporated in manual WCS calibration.
 
 version 1.7.2
 • Moved all the major operational buttons (clear data, write csv, plot curves) to the
 transport button complex.
 version 1.7.1
-
-•
-•
-
-Rearranged transport buttons to allow more flexibility in splitter placement and also to
+• Rearranged transport buttons to allow more flexibility in splitter placement and also to
 bring the current frame spinner to a more accessible place.
-Begun adding the elements needed to deal with non-square pixels during WCS
+• Begun adding the elements needed to deal with non-square pixels during WCS
 calibrations --- GUI elements only at the moment.
-
 version 1.7.0
 • Implements the save/restore state feature. Only the number of apertures and their
 positions are 'marked'. The frame number is 'marked' as well. This 'mark' is placed
 automatically when the first analysis is initiated on a newly loaded video. However,
 there is a button that can be utilized to override this 'mark' if the automatic 'mark' was
 somehow incorrect (or you just changed your mind about where to stat an analysis or
 how many apertures to use, etc).
@@ -1152,31 +1151,30 @@
 your list must be deleted. Just open the list, delete each saved profile, then restore
 them from relevant AVI-WCS folder(s) as required. It's not often that I make a breaking
 change, but this was unavoidable.
 •
 
 Do not get too excited about the transport buttons. They are conceptual/visual only --no functionality yet.
 
-version 1.6.7
+version 1.6.7
 • Fixed breakage caused by incomplete removal of default mask radius spinner.
 version 1.6.6
 • When an AVI-WCS folder is created by clicking the Create AVI-WCS folder from AVI file
 button, a help panel is popped showing the location and name of the newly created
 folder. (I actually had been printing that info to the textOut panel, but there was an
 automatic opening of the new folder that was erasing that panel.)
 • An experimental GUI change has relocated the Plot symbol size spinner to a place
 where it won't be the accidentally invoked by a user intending to click the mskth
 spinner.
 version 1.6.5
 • Made some small changes to documentation pdf suggested by Tony
 • Relabeled the angle printed at completion of manual WCS calibration from fieldrotation (incorrect) to ref1-to-target. This angle is a diagnostic printout, useful to me,
 but not to the user. To interpret it, you need to know that the coordinate systems in use
 are: x increases to right, y increases down, RA has East to the right, DEC has North
-
-down, and angles in the x-y plane (the image) are always positive and are the number
+down, and angles in the x-y plane (the image) are always positive and are the number
 of degrees in the ccw direction needed to rotate a vector until it lines up with the
 positive (i.e., down) y axis. So ref1-to-target means the origin is ref1, and we are
 rotating the vector from ref1 to target around ref1 ccw until it is aligned with the positive
 y axis.
 version 1.6.4
 • Updated documentation pdf
 version 1.6.3
@@ -1190,15 +1188,16 @@
 Version 1.6.0
 • Added the ability for PyMovie to check for more recent versions on startup and allow
 the user to choose whether to accept or not.
 version 1.5.7
 • select VTI dropdown list is disabled unless there are missing model digits.
 • Suppressed the star location dialog --- now only appears when an astrometry.net
 calibration is requested.
-version 1.5.6
+
+version 1.5.6
 • Adds full edit capability for saved ocr profiles. A single dialog box allows for: the
 naming and saving of the current ocr profile; the deletion of a saved profile; the
 renaming of a saved profile; the loading of a saved profile.
 • Item 3 in version 1.5.4 notes refer to the too tortuous logic to implement. Well, it has
 been implemented anyway so training can be done from any position in the avi where
 the upper and lower box positions are the same.
 version 1.5.5
@@ -1206,16 +1205,15 @@
 t2 on a timestamp line --- either left or right. After that, the other digits (t1) wilnot be
 used. This will reduce the number of times an ocr error occurs because of a misrecognition of a digit in a part of the timestamp that should not have been used.
 version 1.5.4
 • Changed blank detection for Kiwi to reflect the new 'normalized' model characters.
 • Added (Kiwi) 8 versus 9 secondary test to resolve confusions (same thing as is being
 done for 6 versus 8)
 • The logic to allow a Kiwi profile to be saved from other than a frame where the
-
-characters are in their training position was too tortuous to implement. Now we just
+characters are in their training position was too tortuous to implement. Now we just
 reposition to frame 1 before doing the save. This means that all training needs to be
 accomplished while the characters are in the position of those in frame 1.
 version 1.5.2
 • When starting from empty folder to train Kiwi, the selection boxes initially were being
 displayed as red rectangles instead of yellow slanted selection boxes --- that's fixed
 • At completion of choosing model digits, we now start timestamp reading.
 • If a Kiwi training is done and a trial run is made that ends with boxes in the alternate
@@ -1232,15 +1230,16 @@
 whenever an analysis (data recording) was started and then paused, the frame where
 the pause took effect was being recorded again if the analysis was restarted from that
 point. That caused duplicated frames to appear in the csv that were not present in the
 avi whenever multiple start/pause/look-around/start-again sequences were performed
 by the user (a common practice).
 The 'fix' was to set a flag when an analysis is started for the first time after either a
 program start or aperture data has been cleared. The start-at frame is recorded if this
-flag is not set, and then the flag is set to inhibit the recording of the start-at frame
+
+flag is not set, and then the flag is set to inhibit the recording of the start-at frame
 should a pause/restart occur.
 A side effect of this new flag is that if one uses the 'run backward' --- 100 down to 50
 (which stops at 51) then 1 to 50 to complete the analysis, frame 1 will not be recorded;
 only 2...100 will be present. A small price to pay for the ability to freely interrupt an
 analysis, check some things, and restart as many times as needed.
 version 1.4.9
 • Improved Kiwi timestamp recognition capability by adding second stage testing to
@@ -1250,19 +1249,19 @@
 character positions.)
 • Squashed the bug that was causing crash when training an OCR profile from an empty
 folder and not providing a star location when prompted.
 •
 
 Very high quality (low error rates) OCR for Kiwi timestamps is available IF and ONLY IF
 you take the time to jog the character selection boxes into good positions. A good
-
-position has the character right-justified in the box. Use 'show property' to get a view
+position has the character right-justified in the box. Use 'show property' to get a view
 of EVERY character box placement and adjust accordingly before saving the model
 digit. It's fiddly, but I routinely get 100% recognition rates on Kiwi timestamps by
 following this advice.
+
 •
 
 Changed the name of the users' list of custom profiles from pymovie-ocr-profiles<username>.p to simply pymovie-ocr-profiles.p What this implies is that we no longer
 support the presence (and automatic merging) of multiple custom profile dictionaries in
 the users' home directory. This feature was highly unlikely to be useful and greatly
 complicated the editing (deleting) of profiles from the custom directories. That is much
 easier to implement when there is but a single dictionary. This will be done in the next
@@ -1277,15 +1276,16 @@
 • Memory usage is back to normal.
 • Better detection and correction of Kiwi timestamps at seconds rollover.
 version 1.4.6
 • Experimental. Probably fixes the garbage collection delay at the end of Kiwi runs. But
 each analysis run causes PyMovie to claim more and more memory.
 version 1.4.2
 • Found a way to deal with the odd timestamp that results when there is a minutes rollover in a Kiwi timestamp. As a result, Kiwi timestamp ocr errors are almost always just
-the 'confusion' between the character 6 and the character 8 (check the confusion
+
+the 'confusion' between the character 6 and the character 8 (check the confusion
 matrix that prints whenever the model digits are viewed to see what I mean), an
 unfortunate result of the Kiwi font for which (as far as I know) nothing can be done.
 version 1.4.1
 • Kiwi timestamp extraction is now (maybe) working. The 'maybe' is because the
 implementation for dealing with the, unique to Kiwi, character position change when
 minutes change is:
 There is a left position and a right position (differing by 11 pixels)
@@ -1293,16 +1293,15 @@
 positions
 You will therefore need to choose the correct ocr box set when setting up the ocr
 profile
 Subsequently, whenever the minute field changes, the other position is applied and
 remains
 active until the next minute change.
 As a consequence of this, you must make sure that any initial 'training' (model digit
-
-recording) never crosses a minute boundary. This is not usually hard to do as the
+recording) never crosses a minute boundary. This is not usually hard to do as the
 complete digit set is usually present in the first 3 or 4 frames.
 In addition, take care not to adjust (jog) Kiwi ocr boxes unless the character position is
 the same as frame 1.
 version 1.4.0
 • Added automatic opening of the newly created AVI-WCS folder after it has been
 created by by clicking the Create AVI-WCS folder from avi file button. So the workflow
 instructions that came with 1.3.9 are no longer needed.
@@ -1319,15 +1318,16 @@
 will be created to be changed by the user. It defaults to the directory that holds the avi.
 Work flow:
 open an avi (this will enable the Create AVI-WCS folder from avi file button)
 click the Create AVI-WCS folder from avi file button
 use the Directory dialog to select (or create a new folder) the directory
 that is to hold the AVI-WCS folder or just accept the default (directory of the
 avi)
-the folder will be created (if necessary) and populated with an alias (for mac
+
+the folder will be created (if necessary) and populated with an alias (for mac
 users)
 or a Shortcut (for Windows users)
 This button has been added because of the decision to perform timestamp OCR only on avi
 files that live in an AVI-WCS folder. That is a good way to collect the (many) files that result
 from OCR, PyMovie, and PyOTE operations in one logical place, but there are likely to be
 users that have opted for a flat(ter) directory structure. This button will ease (hopefully) the
 transition to an alternate file organization.
@@ -1335,16 +1335,15 @@
 • Fixed bug where adding a custom profile was not removing existing ocr selection
 boxes.
 • Gui change to keep 'cascade' label from disappearing on some displays.
 • Started adding ability to create an AVI-WCS folder from an already open avi file. Just
 the gui and a stub where the code will go.
 version 1.3.6
 • Fixed bug that required AVI-WCS folder to be reopened in order for a newly selected
-
-custom ocr profile to take effect. Now timestamp reading starts up as soon as a
+custom ocr profile to take effect. Now timestamp reading starts up as soon as a
 custom profile is selected.
 version 1.3.5
 • Added printing of the 'confusion matrix' (correlation scores of each model digit against
 all the others) when 'show model digits' is invoked.
 • Fixed the spurious exception that was occurring when FITS folder was in use (caused
 by trying to do timestamp extraction as though a VTI were in use)
 version 1.3.4
@@ -1361,42 +1360,41 @@
 pymovie-ocr-profiles-bob.p
 It is possible to share your complete list of custom ocr profiles with another user. For
 instance, I have another custom profile list in my home directory named
 pymovie-ocr-profiles-tony.p
 That ocr profile list came from Tony George (and implements profiles that allow the
 reading of 4 line BoxSprite timestamps). All lists of the form pymovie-ocr-profiles*.p in
 a users home directory are available as custom ocr profiles.
-• Sharing a complete list of profiles is probably not the way to go most times as there
+
+•
+
+Sharing a complete list of profiles is probably not the way to go most times as there
 would be too many entries from someone like Tony (who has to deal with many
 recording chains, each requiring slightly different ocr profiles). Instead, you could
 share the four files (in an AVI-WCS folder) that comprise the ocr profile:
 custom-boxes-upper.p
 custom-boxes-lower.p
 custom-digits.p
 formatter.txt
 Sharing just those files is all that is required. Put them in your AVI-WCS folder and
 then click on the Save OCR profile button to save that profile with a name of your
 choosing in your personal list of custom ocr profiles.
+
 version 1.3.1
 • Added to ocr box right-click menu: retrain model digits, enable/disable upper/lower
 boxes.
 • Added automatic switch to frame view if field view was selected and then Start analysis
 was clicked. It is possible to Pause analysis and then switch to field view without loss
 of data.
 • Removed threshold spinner as that mechanism is no longer used for OCR --- switched
-
-•
-•
-
 to custom model digits per AVI-WCS folder instead.
-Fixed problem that kept ocr box changes and model digits from being properly
+• Fixed problem that kept ocr box changes and model digits from being properly
 preserved and restored from an AVI-WCS folder.
-Laid some framework in place for saving and reusing custom profiles (i.e., ocr boxes
+• Laid some framework in place for saving and reusing custom profiles (i.e., ocr boxes
 and model digits from an AVI-WCS folder)
-
 version 1.3.0
 • We now require that an avi --- for which timestamp OCR extraction is wanted --- be
 placed in an AVI-WCS folder. This allows completely custom ocr box placement and
 modelDigit training. This need only be done once. When that folder is reopened, it will
 snap to frame 1 with ocr boxes placed and the correct vti selected. The value of
 training for each file is that the highest OCR accuracy will always be obtained.
 version 1.2.9
@@ -1411,15 +1409,16 @@
 affecting the preset (optimized) model digits.
 version 1.2.8
 • Timestamp OCR for IOTA VTI models 2 and 3 are functional and useable.
 • Timestamp OCR for BoxSprite is useable, but a little tedious as it requires 're-training'
 at every run in order to deal with the lack of well-formed and reproducible characters.
 • Timestamp OCR for Kiwi is not useable (except to demonstrate and play with the
 challenges of the Kiwi timestamp quirks.
-version 1.2.5
+
+version 1.2.5
 • Adds both lefthand and righthand ocr selection boxes to the IOTA VTI to deal with the
 ambiguity that arises when some cameras emit the odd field first in time while others
 emit the even field first in time.
 version 1.2.4
 • Removed the main gui buttons that jogged the ocr selection box constellation
 up/down/left/right. That function has been taken over by a new right-click context
 menu item that allows all ocr boxes to become joggable by use of arrow keys.
@@ -1428,17 +1427,17 @@
 being set to match the detected fps; that is fixed.
 •
 
 Timestamp OCR is now functional for the IOTA VTI. Model 3 is directly supported.
 Model 2 (which interchanges the position of the early millisecond characters (VTI3:
 early on left; VTI2: early on right) can be decoded as well if one takes the time to
 reposition the ocr selection boxes. Such a change is 'sticky'. This is useful when there
-
-is a single tool chain (camera/VTI/frame-grabber) because, once set for your
+is a single tool chain (camera/VTI/frame-grabber) because, once set for your
 equipment setup, it will be ready to go next time.
+
 •
 
 Recommended work flow: open avi, select VTI, click the appropriate radio button that
 tells PyMovie which field (top or bottom) is first in time, adjust ocr selection boxes (if
 needed), leave field display mode and place measurement apertures as usual.
 
 version 1.1.8
@@ -1457,32 +1456,35 @@
 that widget to make changes take effect. Closing the widget still makes changes take
 effect --- that remains unchanged.
 • It is now possible to change the x,y value of an aperture from the Edit Aperture widget.
 This will make it easy to stack apertures by a simple copy and paste operation of the
 (x,y) data.
 version 1.1.5
 • Added spinner to change default mask radius of any 'green' aperture present.
-• Added linkage from the aperture edit table to the default mask radius spinner and
+
+•
+
+Added linkage from the aperture edit table to the default mask radius spinner and
 threshold spinner so that when the color of an aperture is set to 'green' (even if it
 already was 'green'), the def mask radius and thresh are copied into the spinners on
 the main gui..
+
 version 1.1.4
 • Fixed the aperture position limit issue that occurs when the aperture size is changed
 AFTER the image has been loaded.
 version 1.1.3
 • Removed some no longer needed diagnostic messages being printed in the textOut
 panel.
 version 1.1.2
 • Implements output of csv aperture data in the order specified by the user rather than
 the default order based on the order of adding apertures to the image. For now,
 PyOTE accepts only up to the first four light curves, so when multiple apertures are in
 use, this re-ordering will make sure that you will be able to use PyOTE on the relevant
 lightcurves. It is possible (in the future) that PyOTE will be modified so that more than
-
-4 lightcuves can be processed at the same time. Until then, be judicious in
+4 lightcuves can be processed at the same time. Until then, be judicious in
 selecting/ordering the apertures.
 version 1.1.1
 • Removed the log scaling checkbox. Log scaling rarely used and the image control is
 an adequate and flexible tool for image clipping and scaling to better see stars in an
 image
 • Added an Edit Aperture tool that pops up a list of all aperture with their properties and
 provides a central place to modify same. This will make it easier to deal with stacked
@@ -1500,31 +1502,31 @@
 • Added a check on the validity of RA Dec strings on a program path that was missed in
 1.0.9.
 version 1.0.9
 • Tests the validity of RA Dec strings at the point of entry --- shows errors in textOut
 panel.
 • Returns the aperture jogging capability that was inadvertently suppressed in 1.0.8 by
 the new right-click-for-help system
-version 1.0.8
+
+version 1.0.8
 • Made splitter settings 'sticky' so that user choices as to how much gui real estate to
 give to buttons versus image and textOut versus Thumbnails is preserved between
 sessions.
 • Fixed the tooltip/help info re UCAC4 format to say XXX-XXXXXX (had been XXXXXXXX)
 version 1.0.6
 • Polished the right-click help system. Now the help dialog box can be sized and placed
 by the user and it will be reused (as it was in the original hover-for-help system) for
 subsequent right-click-for-help events. The user is encouraged to position and size the
 help dialog box to suit his preferences and to not worry if it gets hidden because a new
 right-click-for-help will pop it right back up at the previous size and position.
 This help system is much easier to use to quickly explore the help available for each
 gui control.
 version 1.0.4
 • Hover is now properly disabled so that help only appears with a right-click
-
-version 1.0.3
+version 1.0.3
 • Changed the 'help' system from a 'hover to get help' to a right-click to get help.
 version 1.0.2
 • Fixed conversion of color image to grayscale image for avis: now processes YUV color
 space correctly.
 version 1.0.0
 • Added documentation: PyMovie-doc.pdf
 • Pushed source code to git-hub for the first time
@@ -1540,33 +1542,40 @@
 changes to 8 pts if you run on Windows
 version 0.9.8
 • modified the setup.py file so that scikit-image >= 0.15.0 will be automatically installed
 by pip if it is not already present in the Anaconda installation when PyMovie is installed.
 • Added messages to the user that appear if the redact lines and/or num frames boxes
 associated with the Generate “finder” image button are left empty.
 version 0.9.6
-• added the ability (when working in the context of an AVI-WCS folder) to generate a
+
+•
+
+•
+
+•
+
+added the ability (when working in the context of an AVI-WCS folder) to generate a
 “finder” image formed by registering and summing several hundred frames. An
 aperture placed on this image remains when the user switches to the avi. The user
 then adds a 'tracker' aperture, adjusts its threshold, and runs the analysis.
-• to facilitate the use of 'finder' images (produced by stacking images), when a static
+to facilitate the use of 'finder' images (produced by stacking images), when a static
 aperture is added, its threshold is set very high so that it will be forced to use a default
 mask. An aperture that uses a default mask will not move on its own. So switching from
 the 'finder' image to the avi can be done without concern that your careful placement
 will change when the avi comes up.
-• added crosshairs to all apertures, a nice visual aid, particularly in zoomed mode.
+added crosshairs to all apertures, a nice visual aid, particularly in zoomed mode.
+
 version 0.9.3
 • the calculations for manual WCS calibration have definitely been 'fixed' .
 • Miscellaneous small changes to GUI: labels on edit boxes for redact lines and plate
 scale; clear the VizieR response as soon as a change is made in UCAC4 box.
 version 0.9.2
 • the calculations for manual WCS calibration have been 'fixed' (we hope).
 • added the ability to specify a plate scale to use for the manual WCS calibration. Any
-
-value entered in the box to the right of the the Manual WCS calibration button will used
+value entered in the box to the right of the the Manual WCS calibration button will used
 as the plate scale. But be sure to leave this box empty if you want the maths behind
 manual WCS calibration to estimate the plate scale from the calibration points
 provided; this is the normal expected use.
 version 0.9.0
 • same as 0.8.9 but added astroquery as a required package. This is used to make
 VizieR calls but is not a standard part of an Anaconda installation.
 version 0.8.9
@@ -1584,30 +1593,30 @@
 the analysis, frames 0 up to and including the stop-at-frame will be processed. Both the
 plotting routines and the csv write routine will reorder the data based on frame number
 so the section of data that has frame numbers counting down will be restored to its
 normal ordering. This somewhat unusual capability make it easier to deal with an video
 recording that has but a single star (no companion that can used for tracking) that is
 occulted strongly enough that it is only visible (and so can self-track) before D and after
 R. In this case, the R side can be better handled by running the analysis in reverse.
-version 0.8.7
+
+version 0.8.7
 • WCS calibration through nova.astrometry.net now works for both AVI-WCS folders and
 FITS folders.
 version 0.8.5
 • adds an option for WCS calibration when AVI-WCS folder is used to hold observation
 video (or a link to one) through an on-connection to nova.astrometry.net
 version 0.8.4
 • removed the self.pointed_at_aperture = None statement in removeAperture method.
 Just trying stuff.
 version 0.8.3
 • still working on avoiding crashes while deleting apertures under win7. Added manual
 disconnect of slot/signals for the aperture before deleting it.
 version 0.8.2
 • another variation on deleting apertures, this time without the aperture.deleteLater() call.
-
-version 0.8.1
+version 0.8.1
 • another attempt to squash the win7 crash-on-delete-then-run bug.
 version 0.8.0
 • added self.pointed_at_aperture = None when an aperture is deleted. This is a possible
 cause of referring to an aperture that has been deleted and thus causing a memory
 violation exception. Crossing our fingers on this one that it finally solves the win7
 crash-sometimes-when-aperture-is-deleted problem.
 version 0.7.9
@@ -1622,15 +1631,16 @@
 use.
 version 0.7.4
 • added code to ensure that when the yellow aperture mask is being used as the default
 mask that it is evaluated first whenever a there is a frame change.
 version 0.7.3
 • returned the option of simply opening an avi file --- use the Open AVI file button.
 • Now there is a new button labelled Select AVI/WCS folder for when the user wants to
-utilize the WCS calibration capability of PyMovie. They will need to create a folder
+
+utilize the WCS calibration capability of PyMovie. They will need to create a folder
 specifically for that purpose. In that folder they will need to place either the avi file to be
 processed or a shortcut (Windows) or alias (Mac) to that file (so the user does not have
 to relocate his avi just to satisfy PyMovie). This folder will hold star position and wcs
 calibration data unique to frame 0 of the avi. As before, this folder will be the default
 location for csv files and (in the future) png dumps of lightcurve plots.
 version 0.6.9
 • changed to requiring the use of a folder per observation. In that folder must be exactly
@@ -1639,16 +1649,15 @@
 one) that is used to place a target aperture 'blind' on frame 0. This folder will be the
 default location for csv files and (in the future) png dumps of lightcurve plots.
 • finally found bug that was causing confusing thumbnail updates. Should be better now.
 version 0.6.8
 • tightened up the spacing between GUI elements to provide more vertical space for text
 box
 • changed labelling of mask threshold spinner
-
-version 0.6.7
+version 0.6.7
 • rearrange items on GUI to allow for large Clear plot data button
 • added 'hooks' for experimenting with WCS/astrometry.net
 • fixed issue where Thumbnail One was not always synchronized with Thumbnail Two
 (probably)
 • made thumbnail display policy the same whether stepping through or running an
 analysis
 version 0.6.6
@@ -1667,15 +1676,16 @@
 yellow aperture in the set which locks the apertures together in a rigid constellation.
 version 0.6.4
 • with the success of 'dynamic' aperture display, we have adopted a policy when creating
 an aperture of setting all its special properties (jogging and auto-display) OFF and NOT
 touching the properties of any already-in-place apertures. In the previous version,
 adding an aperture caused all special properties in existing apertures to be cleared
 (quietly --- this adds to confusion --- didn't I just set that?) and the new aperture came
-preset with jogging and auto-display ON. In this version, it is up to the user to set the
+
+preset with jogging and auto-display ON. In this version, it is up to the user to set the
 special properties and they will never be quietly changed.
 version 0.6.3
 • added 'dynamic' aperture display. If the mouse cursor is placed over/in an aperture, its
 stats and thumbnail are displayed, regardless of its auto-display setting. This is active
 during an analysis as well so that any aperture can be examined/viewed during a 'run'
 simply by pointing at it.
 version 0.6.2
@@ -1683,16 +1693,15 @@
 as to what is going and avoids the 'complaints' from within the pyqtgraph histogram
 widget when all pixels have the same value
 • added a 3D display (rotatable and zoomable by left and right mouse drag) for the
 Thumbnail One image.
 version 0.4.8
 • now, if you put your cursor on an aperture, the name and major properties of the
 aperture appear in the status bar in the very bottom left corner of the GUI
-
-version 0.4.6
+version 0.4.6
 • added the name of aperture to its context menu --- appears at the top of the right-click
 menu
 • added ability to use arrow keys to jog apertures. Each aperture has a flag to enable it
 to respond to an arrow key, so apertures could be manually jogged as a group should
 that be useful. When an aperture is added, it is born 'joggable' and with 'auto-display'
 • Eliminated the 'green' mode for an aperture. Now each aperture can request that its
 stats be printed at each frame change. There is only one thumbnail display however
@@ -1708,15 +1717,16 @@
 positioned on this image will be preserved when the avi file is opened.
 version 0.4.3
 • made it unnecessary to close the image range control for level changes to be reflected
 in subsequent frame changes
 version 0.4.2
 • the 'no snap' aperture was actually 'snapping' --- that's been fixed
 • added a demonstration plot to let the user see visually what the robust mean and std
-calculations are doing.
+
+calculations are doing.
 version 0.4.1
 • made the changes in image display through use of the image range control 'sticky' so
 that any changes made apply to all images going forward
 • changed the number of pixels plot to use lines only (no circles at the data points) and
 show the negative values (from a default aperture) as positive. It's easier to look at
 and the data plot above clearly identifies data points that were obtained using a default
 mask. The redundancy was not needed or useful
@@ -1724,49 +1734,40 @@
 • added an image range control to give user complete control over image 'stretching'.
 This is a visual effect only as an aid to identifying stars --- it does not affect any
 underlying data values.
 • Added an 'invert images' checkbox to make it easy to switch between avi and fits files
 with their differing convention of the image origin (fits: lower left corner; avi: upper left
 corner)
 version 0.3.9
-
-•
-•
-•
-•
-•
-•
-•
-
-added fast navigate buttons to speed going forward and backward through images
-now the text box gets cleared when a new image file is successfully opened
-changed the way apertures are deleted in support of chasing a pesky sporadic crash
+• added fast navigate buttons to speed going forward and backward through images
+• now the text box gets cleared when a new image file is successfully opened
+• changed the way apertures are deleted in support of chasing a pesky sporadic crash
 when apertures are deleted
-add a spinbox to allow the user to select the plot symbol size --- it's set by a spinbox
+• add a spinbox to allow the user to select the plot symbol size --- it's set by a spinbox
 that is 'sticky'
-some rearranging of GUI elements
-changed label on threshold box to help user understand better what a value in this box
+• some rearranging of GUI elements
+• changed label on threshold box to help user understand better what a value in this box
 means
-added a legend to the composite lightcurve plot to identify the curves
-
+• added a legend to the composite lightcurve plot to identify the curves
 version 0.3.8
 • added a try/except block around aperture delete code to see if we can track down
 crashes that are occurring sporadically under Win 7 OS (but not Mac or Win 10)
 version 0.3.6
 • made the log scale image checkbox 'sticky' so that PyMovie can 'adapt' to your
 preferred image view.
 • removed white apertures from the aperture constellation during tracking so that it/they
 will remain fixed on the image wherever you originally placed it/them.
 version 0.3.5
 • fixed double yellow tracking that was accidentally broken by a change introduced in
 0.3.4
 version 0.3.4
 • added timestamp printout when running fits files with DATE-OBS in fits metadata
 • initialized timestamp correctly
-version 0.3.3
+
+version 0.3.3
 • added timestamp extraction from 'fits files under the assumption that they came from a
 QHY-174M-GPS. This completes PyMovie for users of the QHY-174 that record in
 int16 fits files.
 version 0.3.2
 • added the option of a 'white' aperture to be used when flash-tags have been recorded
 in the video. The special thing about a white aperture is that all the pixels in the
 aperture are summed (without background subtraction) and output as the 'signal' for
@@ -1774,24 +1775,19 @@
 version 0.3.1
 • field processing of avi files now operational
 version 0.3.0
 • fixed tracking during wind shake (accidentally broken in 0.2.9)
 • now we enable/disable controls that are specific to avi versus fits file processing
 • added printout of frames per second read from avi files
 • added ability to view both fields of an avi frame
-
-•
-•
-
-added update of default mask when aperture size is changed to solve the
+• added update of default mask when aperture size is changed to solve the
 mask/thumbnail shape mis-match exception from occurring
-added aperture constellation tracking during manual (frame spinbox) changing of
+• added aperture constellation tracking during manual (frame spinbox) changing of
 frame. It was confusing to have aperture constellation tracking only active during a
 'run'
-
 version 0.2.9
 • added the printing of the FOURCC codec ID extracted from avi files that could be
 opened. This may have diagnostic value in some case where an unusual codec was
 employed. PyMovie handles Lagarith compressed files without issue and without the
 need for the user to separately find and install a Lagarith codec.
 • Added the controls for dealing with field level avi stuff --- no code behind the controls
 yet
@@ -1805,30 +1801,33 @@
 version 0.2.7
 • changed the snap-to-blob function to require user to place cursor on/near star of
 interest. Previously, snap-to-blob snapped to the brightest star in the entire aperture
 UNLESS there was already a yellow aperture defined. This seemed overly
 complicated, hard to explain, and causes the behavior to be sometimes mysterious,
 particularly if one forgets whether or not there is a yellow aperture. Requiring cursor
 placement within 6 pixels of the star-of-interest at all times is easier to get used to and
+
+•
+•
+•
+
 allows a dim star that has bright neighbors to be easily singled out.
-• The aperture name dialog now pops up whenever an aperture is created. This save
+The aperture name dialog now pops up whenever an aperture is created. This save
 mouse clicks and encourages good practices.
-• The title on the Number of pixels plot has been expanded to clarify the meaning of
+The title on the Number of pixels plot has been expanded to clarify the meaning of
 negative mask pixel counts.
-• Removed Inc threshold and Dec threshold menu items from the aperture specific
+Removed Inc threshold and Dec threshold menu items from the aperture specific
 context menu. The Inc and Dec functions are more clearly handled by the spinbox on
 the main GUI window.
+
 version 0.2.6
 • added PyMovie-info.pdf to the distribution (to make the About button work)
 • added opencv-python to the required packages list so that Anaconda installations that
 lack this package (known as cv2) will have it automatically added
 • increased the allowed distance of computed masks from aperture center from 4 pixels
 to 6 pixels (this only comes into effect when there is a yellow aperture present
 • set thresh = 0 when aperture is created rather than None to deal with cases where an
 aperture is added where there is no image
 version 0.2.5
-
-•
-
-Initial Beta release – no timestamp OCR – functional for lightcurve extraction
+• Initial Beta release – no timestamp OCR – functional for lightcurve extraction
```

### Comparing `pymovie-3.7.9/src/pymovie/SER.py` & `pymovie-3.8.0/src/pymovie/SER.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/alias_lnk_resolver.py` & `pymovie-3.8.0/src/pymovie/alias_lnk_resolver.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/aperture.py` & `pymovie-3.8.0/src/pymovie/aperture.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/apertureEdit.py` & `pymovie-3.8.0/src/pymovie/apertureEdit.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/apertureEditDialog.py` & `pymovie-3.8.0/src/pymovie/apertureEditDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/apertureNameDialog.py` & `pymovie-3.8.0/src/pymovie/apertureNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/aperturesFileTagDialog.py` & `pymovie-3.8.0/src/pymovie/aperturesFileTagDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/astrometry_client.py` & `pymovie-3.8.0/src/pymovie/astrometry_client.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/checkForNewerVersion.py` & `pymovie-3.8.0/src/pymovie/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/gammaUtils.py` & `pymovie-3.8.0/src/pymovie/gammaUtils.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/gui.py` & `pymovie-3.8.0/src/pymovie/gui.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/helpDialog.py` & `pymovie-3.8.0/src/pymovie/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/hotPixelDialog.py` & `pymovie-3.8.0/src/pymovie/hotPixelDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/main.py` & `pymovie-3.8.0/src/pymovie/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -3193,27 +3193,33 @@
         if psf_star_found:
             return True, f'All psf-stars have fixed and equal masks.', pixel_count  # noqa
         else:
             return False, 'No apertures with a name containing "psf-star" were found', None
 
     def startAnalysisWithNRE(self):
 
-        if not self.checkForDataAlreadyPresent():
+        if not self.checkForDataAlreadyPresent():  # Returns True if data is already present
+            # If no data collected yet, set default mode to aperture photometry
             self.extractionCode = 'AP'
             self.extractionMode = 'Aperture Photometry'
 
         for app in self.getApertureList():
             if app.name.startswith('psf-star'):
                 ok, msg, _ = self.testForConsistentPsfStarFixedMasks()
 
                 if not ok:
                     self.showMsgPopup(msg)
                     return
 
-                if not self.checkForDataAlreadyPresent():
+                self.extractionCode = 'NRE'
+                self.extractionMode = 'Naylor Noise Reduction Extraction'
+
+
+                if not self.checkForDataAlreadyPresent() or self.naylorInShiftedPositions is None:
+                    # If there is no data present, or naylor weights have not been calculated, we start the psf gathering process
                     self.showMsg(f'Gathering data for psf estimation.')
                     # Save the stop frame
                     saved_stop_frame = self.stopAtFrameSpinBox.value()
                     self.stopAtFrameSpinBox.setValue(self.currentFrameSpinBox.value() + self.psfFrameCountSpinBox.value() - 1)
                     self.startPsfGathering()
                     self.stopAtFrameSpinBox.setValue(saved_stop_frame)
                     self.extractionCode = 'NRE'
@@ -5426,16 +5432,14 @@
         for app in self.getApertureList():
             if app.data:
                 dataAlreadyPresent = True
         return dataAlreadyPresent
 
     def clearApertureData(self):
         self.analysisInProgress = False
-        # self.transportCalcBackgroundCheckBox.setChecked(False)
-        # self.transportCalcBackgroundCheckBox.setEnabled(False)
         self.transportClearData.setEnabled(False)
         for app in self.getApertureList():
             app.data = []
             app.last_theta = None
         self.showMsg(f'All aperture data has been removed.')
         self.stackXtrack = []
         self.stackYtrack = []
@@ -7568,14 +7572,15 @@
 
         if dir_path:
 
             self.clearOptimalExtractionVariables()
 
             self.firstFrameInApertureData = None
             self.lastFrameInApertureData = None
+            self.naylorInShiftedPositions = None
 
             self.disableCmosPixelFilterControls()
             self.activateTimestampRemovalButton.setEnabled(True)
 
             _, fn = os.path.split(dir_path)
             self.fileInUseEdit.setText(fn)
 
@@ -7889,14 +7894,15 @@
 
         if self.filename:
 
             self.clearOptimalExtractionVariables()
 
             self.firstFrameInApertureData = None
             self.lastFrameInApertureData = None
+            self.naylorInShiftedPositions = None
 
             self.disableCmosPixelFilterControls()
             self.activateTimestampRemovalButton.setEnabled(True)
 
             self.useYellowMaskCheckBox.setChecked(False)
             self.lunarCheckBox.setChecked(False)
 
@@ -8120,14 +8126,15 @@
 
         if dir_path:
 
             self.clearOptimalExtractionVariables()
 
             self.firstFrameInApertureData = None
             self.lastFrameInApertureData = None
+            self.naylorInShiftedPositions = None
 
             self.disableCmosPixelFilterControls()
             self.activateTimestampRemovalButton.setEnabled(True)
 
             self.useYellowMaskCheckBox.setChecked(False)
             self.setGammaToUnity()
 
@@ -10038,14 +10045,16 @@
             self.textOut.append("")
             self.textOut.moveCursor(QtGui.QTextCursor.End)  # noqa
 
         self.textOut.ensureCursorVisible()
 
     def closeEvent(self, event):
 
+        self.analysisRequested = False
+
         tabOrderList = []
         numTabs = self.tabWidget.count()
         # print(f'numTabs: {numTabs}')
         for i in range(numTabs):
             tabName = self.tabWidget.tabText(i)
             # print(f'{i}: |{tabName}|')
             tabOrderList.append(tabName)
```

### Comparing `pymovie-3.7.9/src/pymovie/ocr.py` & `pymovie-3.8.0/src/pymovie/ocr.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/ocrCharacterBox.py` & `pymovie-3.8.0/src/pymovie/ocrCharacterBox.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/ocrProfileNameDialog.py` & `pymovie-3.8.0/src/pymovie/ocrProfileNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/play-Temp.py` & `pymovie-3.8.0/src/pymovie/play-Temp.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/play-introspection.py` & `pymovie-3.8.0/src/pymovie/play-introspection.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/selectHotPixelProfile.py` & `pymovie-3.8.0/src/pymovie/selectHotPixelProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/selectProfile.py` & `pymovie-3.8.0/src/pymovie/selectProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/stacker.py` & `pymovie-3.8.0/src/pymovie/stacker.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/starPositionDialog.py` & `pymovie-3.8.0/src/pymovie/starPositionDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie/wcs_helper_functions.py` & `pymovie-3.8.0/src/pymovie/wcs_helper_functions.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.9/src/pymovie.egg-info/PKG-INFO` & `pymovie-3.8.0/src/pymovie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.7.9
+Version: 3.8.0
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.7.9/src/pymovie.egg-info/SOURCES.txt` & `pymovie-3.8.0/src/pymovie.egg-info/SOURCES.txt`

 * *Files identical despite different names*


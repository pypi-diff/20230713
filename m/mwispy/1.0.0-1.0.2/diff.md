# Comparing `tmp/mwispy-1.0.0.tar.gz` & `tmp/mwispy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shaobo/Work/script/mwisp_package/dist/.tmp-2qmg9ipf/mwispy-1.0.0.tar", last modified: Wed Jul 12 13:12:42 2023, max compression
+gzip compressed data, was "/Users/shaobo/Work/script/mwisp_package/dist/.tmp-iptdcmjp/mwispy-1.0.2.tar", last modified: Thu Jul 13 01:09:32 2023, max compression
```

## Comparing `mwispy-1.0.0.tar` & `mwispy-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-12 13:12:42.601572 mwispy-1.0.0/
--rw-r--r--   0 shaobo     (501) staff       (20)     1054 2023-07-12 05:35:20.000000 mwispy-1.0.0/LICENSE
--rw-r--r--   0 shaobo     (501) staff       (20)     7950 2023-07-12 13:12:42.601270 mwispy-1.0.0/PKG-INFO
--rw-r--r--   0 shaobo     (501) staff       (20)     7520 2023-07-12 12:07:04.000000 mwispy-1.0.0/README.md
--rw-r--r--   0 shaobo     (501) staff       (20)      511 2023-07-12 05:31:35.000000 mwispy-1.0.0/pyproject.toml
--rw-r--r--   0 shaobo     (501) staff       (20)       38 2023-07-12 13:12:42.601655 mwispy-1.0.0/setup.cfg
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-12 13:12:42.595021 mwispy-1.0.0/src/
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-12 13:12:42.599537 mwispy-1.0.0/src/mwispy/
--rw-r--r--   0 shaobo     (501) staff       (20)      279 2023-07-12 05:27:10.000000 mwispy-1.0.0/src/mwispy/__init__.py
--rw-r--r--   0 shaobo     (501) staff       (20)     2503 2023-07-12 03:35:10.000000 mwispy-1.0.0/src/mwispy/converter.py
--rw-r--r--   0 shaobo     (501) staff       (20)    14269 2023-07-12 05:26:23.000000 mwispy-1.0.0/src/mwispy/cubemoment.py
--rw-r--r--   0 shaobo     (501) staff       (20)    42688 2023-07-12 12:07:10.000000 mwispy-1.0.0/src/mwispy/datacube.py
--rw-r--r--   0 shaobo     (501) staff       (20)    17017 2023-07-12 05:19:20.000000 mwispy-1.0.0/src/mwispy/mosaic.py
--rw-r--r--   0 shaobo     (501) staff       (20)     8765 2023-07-12 07:51:26.000000 mwispy-1.0.0/src/mwispy/pvslice.py
--rw-r--r--   0 shaobo     (501) staff       (20)     1841 2023-07-12 08:26:23.000000 mwispy-1.0.0/src/mwispy/tile.py
-drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-12 13:12:42.600922 mwispy-1.0.0/src/mwispy.egg-info/
--rw-r--r--   0 shaobo     (501) staff       (20)     7950 2023-07-12 13:12:42.000000 mwispy-1.0.0/src/mwispy.egg-info/PKG-INFO
--rw-r--r--   0 shaobo     (501) staff       (20)      325 2023-07-12 13:12:42.000000 mwispy-1.0.0/src/mwispy.egg-info/SOURCES.txt
--rw-r--r--   0 shaobo     (501) staff       (20)        1 2023-07-12 13:12:42.000000 mwispy-1.0.0/src/mwispy.egg-info/dependency_links.txt
--rw-r--r--   0 shaobo     (501) staff       (20)        7 2023-07-12 13:12:42.000000 mwispy-1.0.0/src/mwispy.egg-info/top_level.txt
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:09:32.578835 mwispy-1.0.2/
+-rw-r--r--   0 shaobo     (501) staff       (20)     1054 2023-07-12 05:35:20.000000 mwispy-1.0.2/LICENSE
+-rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 01:09:32.578560 mwispy-1.0.2/PKG-INFO
+-rw-r--r--   0 shaobo     (501) staff       (20)     7666 2023-07-12 15:07:16.000000 mwispy-1.0.2/README.md
+-rw-r--r--   0 shaobo     (501) staff       (20)      713 2023-07-13 01:09:10.000000 mwispy-1.0.2/pyproject.toml
+-rw-r--r--   0 shaobo     (501) staff       (20)       38 2023-07-13 01:09:32.578925 mwispy-1.0.2/setup.cfg
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:09:32.573632 mwispy-1.0.2/src/
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:09:32.576995 mwispy-1.0.2/src/mwispy/
+-rw-r--r--   0 shaobo     (501) staff       (20)      279 2023-07-12 05:27:10.000000 mwispy-1.0.2/src/mwispy/__init__.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     2503 2023-07-12 03:35:10.000000 mwispy-1.0.2/src/mwispy/converter.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    14270 2023-07-13 00:43:04.000000 mwispy-1.0.2/src/mwispy/cubemoment.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    42692 2023-07-13 00:44:47.000000 mwispy-1.0.2/src/mwispy/datacube.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    17025 2023-07-13 00:42:45.000000 mwispy-1.0.2/src/mwispy/mosaic.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     8870 2023-07-13 00:47:35.000000 mwispy-1.0.2/src/mwispy/pvslice.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     1841 2023-07-12 08:26:23.000000 mwispy-1.0.2/src/mwispy/tile.py
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 01:09:32.578228 mwispy-1.0.2/src/mwispy.egg-info/
+-rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 01:09:32.000000 mwispy-1.0.2/src/mwispy.egg-info/PKG-INFO
+-rw-r--r--   0 shaobo     (501) staff       (20)      325 2023-07-13 01:09:32.000000 mwispy-1.0.2/src/mwispy.egg-info/SOURCES.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)        1 2023-07-13 01:09:32.000000 mwispy-1.0.2/src/mwispy.egg-info/dependency_links.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)        7 2023-07-13 01:09:32.000000 mwispy-1.0.2/src/mwispy.egg-info/top_level.txt
```

### Comparing `mwispy-1.0.0/LICENSE` & `mwispy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.0/PKG-INFO` & `mwispy-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mwispy
-Version: 1.0.0
+Version: 1.0.2
 Summary: Tools for MWISP data reduction.
 Author-email: Shaobo Zhang <shbzhang@pmo.ac.cn>
 Project-URL: Homepage, https://github.com/shbzhang/mwispy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mwispy
 ``mwispy`` derives from the [Milky Way Imaging Scroll Painting (MWISP) project](https://ui.adsabs.harvard.edu/abs/2019ApJS..240....9S).
 
 > The MWISP project is an unbiased Galactic plane CO survey for mapping region of l=-10° to +250° and |b|<=5.°2 with the 13.7 m telescope of the Purple Mountain Observatory.
@@ -60,15 +60,15 @@
 ### Moment
 To calculate the moment of a datacube:
 ```python
 from mwispy import cubemoment
 cubemoment('datacube.fits', crange=[-15, 15], direction='v')
 ```
 * _``crange`` is the velocity range in the unit of km/s._
-* _``cubemoment`` contains a ``goodlooking`` mode which will filter the noise and make the result looking better.
+* _``cubemoment`` contains a ``goodlooking`` mode which will filter the noise and make the result looking better._
 * _See more keywords available for ``cubemoment`` in its help._
 
 To derive a longitude-velocity (LV) map:
 ```python
 from mwispy import cubemoment
 cubemoment('datacube.fits', crange=[-1.5, 2.5], direction='b')
 ```
@@ -204,52 +204,58 @@
 pvhdu.write('pvslice.fits')
 ```
 
 ### Baseline fitting
 ```python
 #set mode and window
 fittedCube = cube.with_window(-60, -40, -20, 20, modex = [-200, 200], vunit='km/s')
+
 #do the baseline fitting
 fittedCube.baseline(deg=1)
+
 #calculate new RMS
-rms = fittedCube.rms()
+rms = fittedCube.get_rms()
 ```
 
 ### Average spectra
 ```python
 #average with equal weighting
 avsp1 = cube.average()
 #average with noise weighting
 avsp2 = cube.with_rms('datacube_rms.fits').average()
+
 #plot spectra
 import matplotlib.pyplot as plt
 plt.step(cube.velocity(), avsp1._data, label='Equal weighting')
 plt.step(cube.velocity(), avsp2._data, label='RMS weighting')
 plt.show()
 ```
 
 ### Rebin velocity
 Smooth and rebin the velocity.
 ```python
 #use rebinvelocity
 rebinnedCube = cube.rebinvelocity(-10, 10, 21, vunit='km/s', largecube=True)
 
 #use resample to align with another header
-ResampleDataCube = cube.resample(referenceheader, vunit='km/s')
+resampledCube = cube.resample(referenceheader, vunit='km/s')
 #use resample with values (NumC, RefC, RefV, IncV)
-ResampleDataCube = cube.resample(201, 100, 0.0, 1.0, vunit='km/s')
+resampledCube = cube.resample(201, 100, 0.0, 1.0, vunit='km/s')
 ```
 
 ### Plot channel map
+
+This method is similar as the ``SpectralCube.plot_channel_maps``, 
+but it adjusts figure size automatically, and provide more keyword options.
 ```python
 #rebin velocity first
 cube = cube.rebinvelocity(-10, 10, 21, vunit='km/s', largecube=True)
 
 #plot
-fig, ax = cube.channelmap(nrows=3, ncols=7, vunit='km/s', figureheight=8, \
+fig, ax = cube.channelmap(nrows=4, ncols=6, vunit='km/s', figureheight=8, \
 	imshow_kws = dict(vmin=-0.1, vmax=5, cmap='rainbow'),\
 	contour_kws = dict(levels=[1,2,3,4,5,6]),\
 	text_kws = dict(x=0.1, y=0.1, size=5),\
 	tick_kws = dict(size=10, direction='in'),\
 	colorbar_kws = None)
 
 #ax[-1,0] is the lower left pannel with tick labels
```

### Comparing `mwispy-1.0.0/README.md` & `mwispy-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ### Moment
 To calculate the moment of a datacube:
 ```python
 from mwispy import cubemoment
 cubemoment('datacube.fits', crange=[-15, 15], direction='v')
 ```
 * _``crange`` is the velocity range in the unit of km/s._
-* _``cubemoment`` contains a ``goodlooking`` mode which will filter the noise and make the result looking better.
+* _``cubemoment`` contains a ``goodlooking`` mode which will filter the noise and make the result looking better._
 * _See more keywords available for ``cubemoment`` in its help._
 
 To derive a longitude-velocity (LV) map:
 ```python
 from mwispy import cubemoment
 cubemoment('datacube.fits', crange=[-1.5, 2.5], direction='b')
 ```
@@ -191,52 +191,58 @@
 pvhdu.write('pvslice.fits')
 ```
 
 ### Baseline fitting
 ```python
 #set mode and window
 fittedCube = cube.with_window(-60, -40, -20, 20, modex = [-200, 200], vunit='km/s')
+
 #do the baseline fitting
 fittedCube.baseline(deg=1)
+
 #calculate new RMS
-rms = fittedCube.rms()
+rms = fittedCube.get_rms()
 ```
 
 ### Average spectra
 ```python
 #average with equal weighting
 avsp1 = cube.average()
 #average with noise weighting
 avsp2 = cube.with_rms('datacube_rms.fits').average()
+
 #plot spectra
 import matplotlib.pyplot as plt
 plt.step(cube.velocity(), avsp1._data, label='Equal weighting')
 plt.step(cube.velocity(), avsp2._data, label='RMS weighting')
 plt.show()
 ```
 
 ### Rebin velocity
 Smooth and rebin the velocity.
 ```python
 #use rebinvelocity
 rebinnedCube = cube.rebinvelocity(-10, 10, 21, vunit='km/s', largecube=True)
 
 #use resample to align with another header
-ResampleDataCube = cube.resample(referenceheader, vunit='km/s')
+resampledCube = cube.resample(referenceheader, vunit='km/s')
 #use resample with values (NumC, RefC, RefV, IncV)
-ResampleDataCube = cube.resample(201, 100, 0.0, 1.0, vunit='km/s')
+resampledCube = cube.resample(201, 100, 0.0, 1.0, vunit='km/s')
 ```
 
 ### Plot channel map
+
+This method is similar as the ``SpectralCube.plot_channel_maps``, 
+but it adjusts figure size automatically, and provide more keyword options.
 ```python
 #rebin velocity first
 cube = cube.rebinvelocity(-10, 10, 21, vunit='km/s', largecube=True)
 
 #plot
-fig, ax = cube.channelmap(nrows=3, ncols=7, vunit='km/s', figureheight=8, \
+fig, ax = cube.channelmap(nrows=4, ncols=6, vunit='km/s', figureheight=8, \
 	imshow_kws = dict(vmin=-0.1, vmax=5, cmap='rainbow'),\
 	contour_kws = dict(levels=[1,2,3,4,5,6]),\
 	text_kws = dict(x=0.1, y=0.1, size=5),\
 	tick_kws = dict(size=10, direction='in'),\
 	colorbar_kws = None)
 
 #ax[-1,0] is the lower left pannel with tick labels
```

### Comparing `mwispy-1.0.0/src/mwispy/converter.py` & `mwispy-1.0.2/src/mwispy/converter.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.0/src/mwispy/cubemoment.py` & `mwispy-1.0.2/src/mwispy/cubemoment.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     >>> cubemoment('cube.fits', [-10,10], goodlooking=True, rmsfile='rms.fits', coveragefile='coverage.fits')
     For mosaiced PMO survey data produce by mosaic.pro
     >>> cubemoment, 'mosaic_U.fits', [-10,10], /goodlooking
     '''
 
     #standardize and test input
     if (cubefile == None) or (crange == None):
-        print("Syntax - mwisp.cubemoment(cubefile, crange, direction='v', threshold=-inf, zeroth_only=False,")
+        print("Syntax - mwispy.cubemoment(cubefile, crange, direction='v', threshold=-inf, zeroth_only=False,")
         print("             coveragefile=None, goodlooking=False, rmsfile=None, outname=None)")
         return
 
     time_start = time.time()
     print('Parameters\n----------')
 
     #cubefile
```

### Comparing `mwispy-1.0.0/src/mwispy/datacube.py` & `mwispy-1.0.2/src/mwispy/datacube.py`

 * *Files 0% similar despite different names*

```diff
@@ -818,15 +818,15 @@
 		Examples
 		--------
 		>>> #set mode and window
 		>>> fittedCube = cube.with_window(-60, -40, -20, 20, modex = [-200, 200], vunit='km/s')
 		>>> #do the baseline fitting
 		>>> fittedCube.baseline(deg=1)
 		>>> #calculate RMS
-		>>> rms = fittedCube.rms()
+		>>> rms = fittedCube.get_rms()
 		'''
 		if deg == 0:
 			p0 = self.mean(axis=0)._data
 			self._data -= p0
 		else:
 			channel = self.channel()
 			p = np.ndarray((deg+1, self.shape[1], self.shape[2]))
```

### Comparing `mwispy-1.0.0/src/mwispy/mosaic.py` & `mwispy-1.0.2/src/mwispy/mosaic.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,20 +95,20 @@
 		correct the CDELT1 error when MWISP-2 data are involving.
 		add keyword "prefix", "suffix" to mosaic cleaned datacubes.
 
 
 	Examples
 	--------
 	>>> pa = ['./', '/share/data/mwisp/G020+00', '/share/data/mwisp/G030+00']
-	>>> mwisp.mosaic(29, 32.5, -1, 1.2, -30, 30, sb='L', path=pa, output='Test', silent=True)
+	>>> mwispy.mosaic(29, 32.5, -1, 1.2, -30, 30, sb='L', path=pa, output='Test', silent=True)
 	'''
 
 	###Syntax prompt
 	if len(crange) != 6 and undone is None:
-		print("Syntax - mosaic(l1, l2, b1, b2, v1, v2, sb='U', path='./', prefix='', suffix='.fits', \n\
+		print("Syntax - mwispy.mosaic(l1, l2, b1, b2, v1, v2, sb='U', path='./', prefix='', suffix='.fits', \n\
 			undone=None, output='mosaic', weightcube=False, display=False, silent=False)")
 		return
 
 	###log file config
 	logging.basicConfig(filename=_getMosaicLogName(output, sb), filemode='w', \
 		level=logging.INFO, format='%(asctime)s %(message)s')
 	def _prompt(message):
```

### Comparing `mwispy-1.0.0/src/mwispy/pvslice.py` & `mwispy-1.0.2/src/mwispy/pvslice.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,28 +78,33 @@
 		rewrite the procedure to accept arbitary path with WIDTH
 		correct the path resampling error
 	Nov,02,2018,v2.1
 		rewrite in python3
 
 	Examples
 	--------
+	>>> #path from array
 	>>> pvslice('XXX.fits', [[l1,l2,l3],[b1,b2,b3]], width=5, step=0.2)
+	>>>
+	>>> #path from file
 	>>> pvslice('XXX.fits', 'path.cat', pathgal=False, spline=True)
-	>>> from mwisp.mosaic import gauss2d
+	>>>
+	>>> #slice with gaussian kernel
+	>>> g2d = lambda dx,dy: np.exp(-(dx**2+dy**2)/2/2**2)
 	>>> pvslice('XXX.fits', 'path.cat', kernel=gauss2d)
 
 	Todo list
 	---------
 	give position with emission more weight when averaging
 	multi-kernel
 	'''
 
 	if (fitsfile == None) | (path_coord == None):
-		print('Syntax - mwisp.pvslice(fitsfile, catalog, width=1, step=0.5, pathgal=True, spline=False, kernel=None)')
-		print('Syntax - mwisp.pvslice(fitsfile, [a, d], width=1, step=0.5, pathgal=True, spline=False, kernel=None)')
+		print('Syntax - mwispy.pvslice(fitsfile, catalog, width=1, step=0.5, pathgal=True, spline=False, kernel=None)')
+		print('Syntax - mwispy.pvslice(fitsfile, [a, d], width=1, step=0.5, pathgal=True, spline=False, kernel=None)')
 		return
 
 	if not os.path.exists(fitsfile):
 		print('Error - fits file does not exist.')
 		return
 	
 	if step <= 0:
```

### Comparing `mwispy-1.0.0/src/mwispy/tile.py` & `mwispy-1.0.2/src/mwispy/tile.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.0/src/mwispy.egg-info/PKG-INFO` & `mwispy-1.0.2/src/mwispy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mwispy
-Version: 1.0.0
+Version: 1.0.2
 Summary: Tools for MWISP data reduction.
 Author-email: Shaobo Zhang <shbzhang@pmo.ac.cn>
 Project-URL: Homepage, https://github.com/shbzhang/mwispy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mwispy
 ``mwispy`` derives from the [Milky Way Imaging Scroll Painting (MWISP) project](https://ui.adsabs.harvard.edu/abs/2019ApJS..240....9S).
 
 > The MWISP project is an unbiased Galactic plane CO survey for mapping region of l=-10° to +250° and |b|<=5.°2 with the 13.7 m telescope of the Purple Mountain Observatory.
@@ -60,15 +60,15 @@
 ### Moment
 To calculate the moment of a datacube:
 ```python
 from mwispy import cubemoment
 cubemoment('datacube.fits', crange=[-15, 15], direction='v')
 ```
 * _``crange`` is the velocity range in the unit of km/s._
-* _``cubemoment`` contains a ``goodlooking`` mode which will filter the noise and make the result looking better.
+* _``cubemoment`` contains a ``goodlooking`` mode which will filter the noise and make the result looking better._
 * _See more keywords available for ``cubemoment`` in its help._
 
 To derive a longitude-velocity (LV) map:
 ```python
 from mwispy import cubemoment
 cubemoment('datacube.fits', crange=[-1.5, 2.5], direction='b')
 ```
@@ -204,52 +204,58 @@
 pvhdu.write('pvslice.fits')
 ```
 
 ### Baseline fitting
 ```python
 #set mode and window
 fittedCube = cube.with_window(-60, -40, -20, 20, modex = [-200, 200], vunit='km/s')
+
 #do the baseline fitting
 fittedCube.baseline(deg=1)
+
 #calculate new RMS
-rms = fittedCube.rms()
+rms = fittedCube.get_rms()
 ```
 
 ### Average spectra
 ```python
 #average with equal weighting
 avsp1 = cube.average()
 #average with noise weighting
 avsp2 = cube.with_rms('datacube_rms.fits').average()
+
 #plot spectra
 import matplotlib.pyplot as plt
 plt.step(cube.velocity(), avsp1._data, label='Equal weighting')
 plt.step(cube.velocity(), avsp2._data, label='RMS weighting')
 plt.show()
 ```
 
 ### Rebin velocity
 Smooth and rebin the velocity.
 ```python
 #use rebinvelocity
 rebinnedCube = cube.rebinvelocity(-10, 10, 21, vunit='km/s', largecube=True)
 
 #use resample to align with another header
-ResampleDataCube = cube.resample(referenceheader, vunit='km/s')
+resampledCube = cube.resample(referenceheader, vunit='km/s')
 #use resample with values (NumC, RefC, RefV, IncV)
-ResampleDataCube = cube.resample(201, 100, 0.0, 1.0, vunit='km/s')
+resampledCube = cube.resample(201, 100, 0.0, 1.0, vunit='km/s')
 ```
 
 ### Plot channel map
+
+This method is similar as the ``SpectralCube.plot_channel_maps``, 
+but it adjusts figure size automatically, and provide more keyword options.
 ```python
 #rebin velocity first
 cube = cube.rebinvelocity(-10, 10, 21, vunit='km/s', largecube=True)
 
 #plot
-fig, ax = cube.channelmap(nrows=3, ncols=7, vunit='km/s', figureheight=8, \
+fig, ax = cube.channelmap(nrows=4, ncols=6, vunit='km/s', figureheight=8, \
 	imshow_kws = dict(vmin=-0.1, vmax=5, cmap='rainbow'),\
 	contour_kws = dict(levels=[1,2,3,4,5,6]),\
 	text_kws = dict(x=0.1, y=0.1, size=5),\
 	tick_kws = dict(size=10, direction='in'),\
 	colorbar_kws = None)
 
 #ax[-1,0] is the lower left pannel with tick labels
```


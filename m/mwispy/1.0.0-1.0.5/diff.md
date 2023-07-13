# Comparing `tmp/mwispy-1.0.0.tar.gz` & `tmp/mwispy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shaobo/Work/script/mwisp_package/dist/.tmp-2qmg9ipf/mwispy-1.0.0.tar", last modified: Wed Jul 12 13:12:42 2023, max compression
+gzip compressed data, was "/Users/shaobo/Work/script/mwisp_package/dist/.tmp-kmw2j5ii/mwispy-1.0.5.tar", last modified: Thu Jul 13 03:06:41 2023, max compression
```

## Comparing `mwispy-1.0.0.tar` & `mwispy-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
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
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 03:06:41.110467 mwispy-1.0.5/
+-rw-r--r--   0 shaobo     (501) staff       (20)     1054 2023-07-12 05:35:20.000000 mwispy-1.0.5/LICENSE
+-rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 03:06:41.110098 mwispy-1.0.5/PKG-INFO
+-rw-r--r--   0 shaobo     (501) staff       (20)     7666 2023-07-13 01:26:25.000000 mwispy-1.0.5/README.md
+-rw-r--r--   0 shaobo     (501) staff       (20)      676 2023-07-13 03:05:56.000000 mwispy-1.0.5/pyproject.toml
+-rw-r--r--   0 shaobo     (501) staff       (20)       38 2023-07-13 03:06:41.110598 mwispy-1.0.5/setup.cfg
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 03:06:41.103005 mwispy-1.0.5/src/
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 03:06:41.107882 mwispy-1.0.5/src/mwispy/
+-rw-r--r--   0 shaobo     (501) staff       (20)      279 2023-07-12 05:27:10.000000 mwispy-1.0.5/src/mwispy/__init__.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     2503 2023-07-12 03:35:10.000000 mwispy-1.0.5/src/mwispy/converter.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    14270 2023-07-13 00:43:04.000000 mwispy-1.0.5/src/mwispy/cubemoment.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    42777 2023-07-13 03:05:16.000000 mwispy-1.0.5/src/mwispy/datacube.py
+-rw-r--r--   0 shaobo     (501) staff       (20)    17025 2023-07-13 00:42:45.000000 mwispy-1.0.5/src/mwispy/mosaic.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     8870 2023-07-13 00:47:35.000000 mwispy-1.0.5/src/mwispy/pvslice.py
+-rw-r--r--   0 shaobo     (501) staff       (20)     1841 2023-07-12 08:26:23.000000 mwispy-1.0.5/src/mwispy/tile.py
+drwxr-xr-x   0 shaobo     (501) staff       (20)        0 2023-07-13 03:06:41.109736 mwispy-1.0.5/src/mwispy.egg-info/
+-rw-r--r--   0 shaobo     (501) staff       (20)     8096 2023-07-13 03:06:41.000000 mwispy-1.0.5/src/mwispy.egg-info/PKG-INFO
+-rw-r--r--   0 shaobo     (501) staff       (20)      358 2023-07-13 03:06:41.000000 mwispy-1.0.5/src/mwispy.egg-info/SOURCES.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)        1 2023-07-13 03:06:41.000000 mwispy-1.0.5/src/mwispy.egg-info/dependency_links.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)       92 2023-07-13 03:06:41.000000 mwispy-1.0.5/src/mwispy.egg-info/requires.txt
+-rw-r--r--   0 shaobo     (501) staff       (20)        7 2023-07-13 03:06:41.000000 mwispy-1.0.5/src/mwispy.egg-info/top_level.txt
```

### Comparing `mwispy-1.0.0/LICENSE` & `mwispy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.0/PKG-INFO` & `mwispy-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwispy
-Version: 1.0.0
+Version: 1.0.5
 Summary: Tools for MWISP data reduction.
 Author-email: Shaobo Zhang <shbzhang@pmo.ac.cn>
 Project-URL: Homepage, https://github.com/shbzhang/mwispy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
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

### Comparing `mwispy-1.0.0/README.md` & `mwispy-1.0.5/README.md`

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

### Comparing `mwispy-1.0.0/src/mwispy/converter.py` & `mwispy-1.0.5/src/mwispy/converter.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.0/src/mwispy/cubemoment.py` & `mwispy-1.0.5/src/mwispy/cubemoment.py`

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

### Comparing `mwispy-1.0.0/src/mwispy/datacube.py` & `mwispy-1.0.5/src/mwispy/datacube.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,22 @@
 
 ###use spectral
 import copy, warnings
 import numpy as np
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 
-import radio_beam
 from astropy.io import fits
+import astropy.units as u
 from astropy.units.quantity import Quantity
 from spectral_cube import SpectralCube, OneDSpectrum
 from spectral_cube.lower_dimensional_structures import Projection
 from astropy.convolution import Gaussian1DKernel, Box1DKernel
 from astropy.coordinates import SkyCoord
 from astropy.wcs import WCS
-from reproject import reproject_interp
-import astropy.units as u
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 
 
 def openMWISP(file):
 	return DataCube.openMWISP(file)
 
 
@@ -89,14 +87,15 @@
 	>>> newcube = cube.subcube(xlo=84*u.deg, xhi=86*u.deg, ylo=-2*u.deg, yhi=1*u.deg, zlo=-5*u.km/u.s, zhi=5*u.km/u.s) 
 
 	Spatial Reprojection (cf. SpectralCube.reproject)
 	>>> newcube = cube.reproject(referenceheader, order='bilinear', use_memmap=False, filled=True)
 
 	Spatial Smooth (cf. SpectralCube.convolve_to)
 	if cube has no beam info:
+	>>> import radio_beam
 	>>> beam = radio_beam.Beam(major=52*u.arcsec, minor=52*u.arcsec, pa=0*u.deg)
 	>>> cube = cube.with_beam(beam)
 	then smoothing:
 	>>> newbeam = radio_beam.Beam(major=4*u.arcmin, minor=4*u.arcmin, pa=0*u.deg)
 	>>> newcube = cube.with_beam(beam).convolve_to(newbeam)
 	
 	Cube Moment (cf. SpectralCube.moment)
@@ -818,29 +817,29 @@
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
-			it = np.nditer(self._data[0], flags=['multi_index'])
-			while not it.finished:
-				spectrum = self._data[:, it.multi_index[0], it.multi_index[1]]
-				mask = self.mask.include()[:, it.multi_index[0], it.multi_index[1]] & np.isfinite(spectrum)
-				if mask.sum()>5:
-					p[:, it.multi_index[0], it.multi_index[1]] = np.polyfit(channel[mask], spectrum[mask], deg)
-				it.iternext()
+			for ix in tqdm(range(self.shape[2])):
+				for iy in range(self.shape[1]):
+					spectrum = self._data[:,iy,ix].copy()
+					mask = self.mask.include()[:,iy,ix] & np.isfinite(spectrum)
+					if mask.sum()>5:
+						p[:, iy, ix] = np.polyfit(channel[mask], spectrum[mask], deg)
+
 			for d in range(deg+1):
 				self._data -= p[-d-1,:,:]*self.channel()[:,np.newaxis,np.newaxis]**d
 
 
 	def get_rms(self):
 		'''
 		return a RMS map in current mask
@@ -1264,19 +1263,19 @@
 		rgbwcs = self.wcs.sub(2)
 		return rgbdata, rgbwcs
 
 
 
 if __name__ == '__main__':
 	#init
-	old = 'example/old.fits'
-	ref = 'example/ref.fits'
-	rms = 'example/rms.fits'
-	cxy = 'example/cxy.fits'
-	ycx = 'example/ycx.fits'
+	old = '/Users/shaobo/Work/script/mwisp_package_test/example/old.fits'
+	ref = '/Users/shaobo/Work/script/mwisp_package_test/example/ref.fits'
+	rms = '/Users/shaobo/Work/script/mwisp_package_test/example/rms.fits'
+	cxy = '/Users/shaobo/Work/script/mwisp_package_test/example/cxy.fits'
+	ycx = '/Users/shaobo/Work/script/mwisp_package_test/example/ycx.fits'
 	cube = DataCube.openMWISP(old)
 	print(cube,'\n')
 	#print(help(cube))
 
 	###test rms
 	if 0:
 		print('new and old are using the same data')
@@ -1362,20 +1361,20 @@
 		###show v_mask
 		cube.moment(order=0).quicklook()
 		cube.with_rms(rms).with_mask(cube.v_mask(threshold=5, consecutive=5)).moment(order=0).quicklook()
 		plt.show()
 
 	#test baseline
 	if 0:
-		new = cube[:,100:110, 120: 135].with_window(-1, 13, modex=[-19, 19])
+		new = cube[:,100:110, 120:135].with_window(-1, 13, modex=[-19, 19])
 
 		plt.step(new.velocity(), new._data[:,5,-2], 'k-')
 		plt.step(new.velocity(), new.mask.include()[:,5,-2])
 		
-		new.baseline(deg=0)
+		new.baseline(deg=2)
 		plt.step(new.velocity(), new._data[:,5,-2], 'r-')
 		plt.plot(new.velocity(), np.zeros(new.velocity().size))
 		plt.show()
 
 		new.get_rms().quicklook()
 		plt.show()
```

### Comparing `mwispy-1.0.0/src/mwispy/mosaic.py` & `mwispy-1.0.5/src/mwispy/mosaic.py`

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

### Comparing `mwispy-1.0.0/src/mwispy/pvslice.py` & `mwispy-1.0.5/src/mwispy/pvslice.py`

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

### Comparing `mwispy-1.0.0/src/mwispy/tile.py` & `mwispy-1.0.5/src/mwispy/tile.py`

 * *Files identical despite different names*

### Comparing `mwispy-1.0.0/src/mwispy.egg-info/PKG-INFO` & `mwispy-1.0.5/src/mwispy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwispy
-Version: 1.0.0
+Version: 1.0.5
 Summary: Tools for MWISP data reduction.
 Author-email: Shaobo Zhang <shbzhang@pmo.ac.cn>
 Project-URL: Homepage, https://github.com/shbzhang/mwispy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
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


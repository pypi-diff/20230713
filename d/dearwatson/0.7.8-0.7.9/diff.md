# Comparing `tmp/dearwatson-0.7.8.tar.gz` & `tmp/dearwatson-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.7.8.tar", last modified: Tue Jun 20 09:37:04 2023, max compression
+gzip compressed data, was "dearwatson-0.7.9.tar", last modified: Tue Jul  4 21:51:37 2023, max compression
```

## Comparing `dearwatson-0.7.8.tar` & `dearwatson-0.7.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 09:36:50.000000 dearwatson-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 09:36:50.000000 dearwatson-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-20 09:37:04.547575 dearwatson-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-20 09:36:50.000000 dearwatson-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:37:04.547575 dearwatson-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-20 09:36:51.000000 dearwatson-0.7.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 09:36:51.000000 dearwatson-0.7.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:36:52.000000 dearwatson-0.7.8/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-06-20 09:36:52.000000 dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-06-20 09:36:52.000000 dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   107007 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.929850 dearwatson-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 21:51:22.000000 dearwatson-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 21:51:22.000000 dearwatson-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-04 21:51:37.929850 dearwatson-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-04 21:51:22.000000 dearwatson-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.925850 dearwatson-0.7.9/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-04 21:51:37.000000 dearwatson-0.7.9/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-04 21:51:37.000000 dearwatson-0.7.9/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:51:37.000000 dearwatson-0.7.9/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-04 21:51:37.000000 dearwatson-0.7.9/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 21:51:37.000000 dearwatson-0.7.9/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:51:37.929850 dearwatson-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-04 21:51:22.000000 dearwatson-0.7.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 21:51:22.000000 dearwatson-0.7.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.925850 dearwatson-0.7.9/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.925850 dearwatson-0.7.9/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.921850 dearwatson-0.7.9/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.925850 dearwatson-0.7.9/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-07-04 21:51:22.000000 dearwatson-0.7.9/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.929850 dearwatson-0.7.9/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:23.000000 dearwatson-0.7.9/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-04 21:51:23.000000 dearwatson-0.7.9/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:51:37.929850 dearwatson-0.7.9/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:51:24.000000 dearwatson-0.7.9/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-07-04 21:51:24.000000 dearwatson-0.7.9/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-07-04 21:51:24.000000 dearwatson-0.7.9/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107106 2023-07-04 21:51:23.000000 dearwatson-0.7.9/watson/watson.py
```

### Comparing `dearwatson-0.7.8/LICENSE` & `dearwatson-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/PKG-INFO` & `dearwatson-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.8
+Version: 0.7.9
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.8/README.md` & `dearwatson-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.7.9/dearwatson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.8
+Version: 0.7.9
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.8/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.7.9/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/setup.py` & `dearwatson-0.7.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.7.8"
+version = "0.7.9"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
@@ -23,15 +23,16 @@
     python_requires='>=3.8',
     install_requires=[
                         "bokeh==2.4.2", # TPFPlotter dependency
                         'configparser==5.0.1',
                         "cython==0.29.21",
                         "extension-helpers==0.1",
                         "imageio==2.9.0",
-                        "lcbuilder==0.12.6",
+                        "lcbuilder==0.12.7",
                         "matplotlib==3.5.2",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "pyyaml==5.4.1",
+                        "pillow==9.5.0",
                         "reportlab==3.5.59",
                         'setuptools>=41.0.0'
     ]
 )
```

### Comparing `dearwatson-0.7.8/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.7.9/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/watson/neighbours.py` & `dearwatson-0.7.9/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/watson/report.py` & `dearwatson-0.7.9/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/watson/resources/images/sherlock3.png` & `dearwatson-0.7.9/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/watson/resources/images/watson.png` & `dearwatson-0.7.9/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/watson/tests/test_watson.py` & `dearwatson-0.7.9/watson/tests/test_watson.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def test_vetting_by_params(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
         vetting_dir = object_dir + "/vetting_0/"
         try:
             Watson(object_dir, vetting_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
                                        cadence=120, cpus=multiprocessing.cpu_count() // 2, clean=False)
             files_in_dir = os.listdir(vetting_dir)
-            assert len(files_in_dir) == 34
+            assert len(files_in_dir) == 33
         finally:
             if os.path.exists(vetting_dir):
                 shutil.rmtree(vetting_dir, ignore_errors=False)
 
     def test_vetting_by_files(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
         vetting_dir = object_dir + "/vetting_0/"
```

### Comparing `dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.7.9/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.7.9/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.8/watson/watson.py` & `dearwatson-0.7.9/watson/watson.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         lc_builder = LcBuilder()
         if transits_mask is None:
             transits_mask = []
         if rp_rstar is None:
             rp_rstar = np.sqrt(depth / 1000)
         lc_build = None
         if lc_file is None or lc_data_file is None:
-            lc_build = lc_builder.build(MissionObjectInfo(sectors, id, cadence=cadence,
+            lc_build = lc_builder.build(MissionObjectInfo(sectors, id, cadence=cadence, high_rms_enabled=False,
                                                           initial_transit_mask=transits_mask), self.data_dir)
             lc_build.lc_data.to_csv(self.object_dir + "/lc_data.csv")
             lc_file = self.object_dir + "/lc.csv"
             lc_data_file = self.object_dir + "/lc_data.csv"
         if a_rstar is None and lc_build is None:
             raise ValueError("You need to define a_rstar if you are providing the lc_file and lc_data_file")
         if a_rstar is None:
@@ -1122,34 +1122,34 @@
         plt.clf()
         # phot_source_offset_ra = ra + (centroid_coords_df_oot['centroids_ra'].median() * ra / 3600 - \
         #                         (1 / depth - 1) * centroid_coords_df_it['centroids_ra'].median() * ra / 3600) * np.cos(np.deg2rad(dec))
         # phot_source_offset_dec = dec + (centroid_coords_df_oot['centroids_dec'].median() * dec / 3600 - \
         #                         (1 / depth - 1) * centroid_coords_df_it['centroids_dec'].median() * dec / 3600)
         source_offset_diggimg_ra = np.nanmedian(np.array(source_offsets_diffimg)[:, 0])
         source_offset_diggimg_dec = np.nanmedian(np.array(source_offsets_diffimg)[:, 1])
-        source_offset_diggimg_ra_err = np.nanstd(np.array(source_offsets_diffimg)[:, 0])
-        source_offset_diggimg_dec_err = np.nanstd(np.array(source_offsets_diffimg)[:, 1])
+        source_offset_diggimg_ra_err = 3 * np.nanstd(np.array(source_offsets_diffimg)[:, 0])
+        source_offset_diggimg_dec_err = 3 * np.nanstd(np.array(source_offsets_diffimg)[:, 1])
         source_offset_bls_ra = np.nanmedian(np.array(source_offsets_bls)[:, 0])
         source_offset_bls_dec = np.nanmedian(np.array(source_offsets_bls)[:, 1])
-        source_offset_bls_ra_err = np.nanstd(np.array(source_offsets_bls)[:, 0])
-        source_offset_bls_dec_err = np.nanstd(np.array(source_offsets_bls)[:, 1])
+        source_offset_bls_ra_err = 3 * np.nanstd(np.array(source_offsets_bls)[:, 0])
+        source_offset_bls_dec_err = 3 * np.nanstd(np.array(source_offsets_bls)[:, 1])
         offset_ra = np.mean([source_offset_bls_ra, source_offset_diggimg_ra])
         offset_dec = np.mean([source_offset_bls_dec, source_offset_diggimg_dec])
-        offset_ra_err = 1/2 * np.sqrt(source_offset_bls_ra_err ** 2 + source_offset_diggimg_ra_err ** 2)
-        offset_dec_err = 1/2 * np.sqrt(source_offset_bls_dec_err ** 2 + source_offset_diggimg_dec_err ** 2)
+        offset_ra_err = np.sqrt((1/2 * source_offset_bls_ra_err) ** 2 + (1/2 * source_offset_diggimg_ra_err) ** 2)
+        offset_dec_err = np.sqrt((1/2 * source_offset_bls_dec_err) ** 2 + (1/2 * source_offset_diggimg_dec_err) ** 2)
         if np.isnan(offset_ra_err) or offset_ra_err == 0.0:
             offset_ra_err = 3 * np.nanstd([source_offset_bls_ra, source_offset_diggimg_ra])
         if np.isnan(offset_dec_err) or offset_dec_err == 0.0:
             offset_dec_err = 3 * np.nanstd([source_offset_bls_dec, source_offset_diggimg_dec])
         offsets_df = pd.DataFrame(columns=['name', 'ra', 'dec', 'ra_err', 'dec_err'])
-        offsets_df.append({'name': 'diff_img', 'ra': source_offset_diggimg_ra, 'dec': source_offset_diggimg_dec,
+        offsets_df = offsets_df.append({'name': 'diff_img', 'ra': source_offset_diggimg_ra, 'dec': source_offset_diggimg_dec,
                            'ra_err': source_offset_diggimg_ra_err, 'dec_err': source_offset_diggimg_dec_err}, ignore_index=True)
-        offsets_df.append({'name': 'px_bls', 'ra': source_offset_bls_ra, 'dec': source_offset_bls_dec,
+        offsets_df = offsets_df.append({'name': 'px_bls', 'ra': source_offset_bls_ra, 'dec': source_offset_bls_dec,
                            'ra_err': source_offset_bls_ra_err, 'dec_err': source_offset_bls_dec_err}, ignore_index=True)
-        offsets_df.append({'name': 'mean', 'ra': offset_ra, 'dec': offset_dec,
+        offsets_df = offsets_df.append({'name': 'mean', 'ra': offset_ra, 'dec': offset_dec,
                            'ra_err': offset_ra_err, 'dec_err': offset_dec_err}, ignore_index=True)
         offsets_df.to_csv(file_dir + '/source_offsets.csv')
         tpf = tpfs[0]
         hdu = tpf.hdu[2].header
         wcs = WCS(hdu)
         offset_px = wcs.all_world2pix(offset_ra, offset_dec, 0)
         light_centroids_sub_offset_px = wcs.all_world2pix(source_offset_diggimg_ra, source_offset_diggimg_dec, 0)
```


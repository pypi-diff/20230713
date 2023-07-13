# Comparing `tmp/antspyt1w-0.8.9.tar.gz` & `tmp/antspyt1w-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspyt1w-0.8.9.tar", last modified: Tue Mar 14 13:29:16 2023, max compression
+gzip compressed data, was "antspyt1w-0.9.0.tar", last modified: Thu Jul 13 15:44:41 2023, max compression
```

## Comparing `antspyt1w-0.8.9.tar` & `antspyt1w-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-14 13:29:16.995547 antspyt1w-0.8.9/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-17 22:27:29.000000 antspyt1w-0.8.9/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)     3228 2023-03-14 13:29:16.995353 antspyt1w-0.8.9/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     2897 2021-12-05 17:08:27.000000 antspyt1w-0.8.9/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-14 13:29:16.992076 antspyt1w-0.8.9/antspyt1w/
--rw-r--r--   0 stnava     (501) staff       (20)     1573 2023-03-14 13:16:41.000000 antspyt1w-0.8.9/antspyt1w/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   132166 2023-03-14 13:25:36.000000 antspyt1w-0.8.9/antspyt1w/get_data.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-14 13:29:16.993265 antspyt1w-0.8.9/antspyt1w.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)     3228 2023-03-14 13:29:16.000000 antspyt1w-0.8.9/antspyt1w.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      364 2023-03-14 13:29:16.000000 antspyt1w-0.8.9/antspyt1w.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-03-14 13:29:16.000000 antspyt1w-0.8.9/antspyt1w.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2022-10-05 13:41:34.000000 antspyt1w-0.8.9/antspyt1w.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)       10 2023-03-14 13:29:16.000000 antspyt1w-0.8.9/antspyt1w.egg-info/top_level.txt
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-03-14 13:29:16.995602 antspyt1w-0.8.9/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      522 2023-03-14 13:24:01.000000 antspyt1w-0.8.9/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-14 13:29:16.995021 antspyt1w-0.8.9/tests/
--rw-r--r--   0 stnava     (501) staff       (20)      987 2022-03-11 22:33:25.000000 antspyt1w-0.8.9/tests/test_deep_hipp.py
--rw-r--r--   0 stnava     (501) staff       (20)      948 2022-03-12 15:08:32.000000 antspyt1w-0.8.9/tests/test_mtl.py
--rw-r--r--   0 stnava     (501) staff       (20)      675 2022-01-11 18:52:31.000000 antspyt1w-0.8.9/tests/test_rbp.py
--rw-r--r--   0 stnava     (501) staff       (20)     1382 2022-03-18 13:56:41.000000 antspyt1w-0.8.9/tests/test_reference_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      541 2022-01-09 15:31:19.000000 antspyt1w-0.8.9/tests/test_tissueseg.py
--rw-r--r--   0 stnava     (501) staff       (20)     1143 2022-01-04 12:49:35.000000 antspyt1w-0.8.9/tests/test_wmh.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:44:41.149325 antspyt1w-0.9.0/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-17 22:27:29.000000 antspyt1w-0.9.0/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)     3228 2023-07-13 15:44:41.149148 antspyt1w-0.9.0/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     2897 2021-12-05 17:08:27.000000 antspyt1w-0.9.0/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:44:41.146600 antspyt1w-0.9.0/antspyt1w/
+-rw-r--r--   0 stnava     (501) staff       (20)     1573 2023-03-14 13:16:41.000000 antspyt1w-0.9.0/antspyt1w/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   134081 2023-07-13 15:42:38.000000 antspyt1w-0.9.0/antspyt1w/get_data.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:44:41.147631 antspyt1w-0.9.0/antspyt1w.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)     3228 2023-07-13 15:44:41.000000 antspyt1w-0.9.0/antspyt1w.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      364 2023-07-13 15:44:41.000000 antspyt1w-0.9.0/antspyt1w.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-07-13 15:44:41.000000 antspyt1w-0.9.0/antspyt1w.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2022-10-05 13:41:34.000000 antspyt1w-0.9.0/antspyt1w.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)       10 2023-07-13 15:44:41.000000 antspyt1w-0.9.0/antspyt1w.egg-info/top_level.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-07-13 15:44:41.149373 antspyt1w-0.9.0/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      522 2023-07-13 14:58:47.000000 antspyt1w-0.9.0/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:44:41.148901 antspyt1w-0.9.0/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)      987 2022-03-11 22:33:25.000000 antspyt1w-0.9.0/tests/test_deep_hipp.py
+-rw-r--r--   0 stnava     (501) staff       (20)      948 2022-03-12 15:08:32.000000 antspyt1w-0.9.0/tests/test_mtl.py
+-rw-r--r--   0 stnava     (501) staff       (20)      675 2022-01-11 18:52:31.000000 antspyt1w-0.9.0/tests/test_rbp.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1382 2022-03-18 13:56:41.000000 antspyt1w-0.9.0/tests/test_reference_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      541 2022-01-09 15:31:19.000000 antspyt1w-0.9.0/tests/test_tissueseg.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1143 2022-01-04 12:49:35.000000 antspyt1w-0.9.0/tests/test_wmh.py
```

### Comparing `antspyt1w-0.8.9/LICENSE` & `antspyt1w-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/PKG-INFO` & `antspyt1w-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspyt1w
-Version: 0.8.9
+Version: 0.9.0
 Summary: T1w human neuroimage processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyT1w
 Author: Avants, Gosselin, Tustison
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspyt1w-0.8.9/README.md` & `antspyt1w-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/antspyt1w/__init__.py` & `antspyt1w-0.9.0/antspyt1w/__init__.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/antspyt1w/get_data.py` & `antspyt1w-0.9.0/antspyt1w/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import antspynet
 import tensorflow as tf
 
 from multiprocessing import Pool
 
 DATA_PATH = os.path.expanduser('~/.antspyt1w/')
 
-def get_data( name=None, force_download=False, version=45, target_extension='.csv' ):
+def get_data( name=None, force_download=False, version=46, target_extension='.csv' ):
     """
     Get ANTsPyT1w data filename
 
     The first time this is called, it will download data to ~/.antspyt1w.
     After, it will just read data from disk.  The ~/.antspyt1w may need to
     be periodically deleted in order to ensure data is current.
 
@@ -544,18 +544,18 @@
 
     """
 
     if x.dimension != 3:
         raise ValueError('inspect_raw_t1: input image should be 3-dimensional')
 
     x = ants.iMath( x, "Normalize" )
-    csvfn = output_prefix + "_head.csv"
-    pngfn = output_prefix + "_head.png"
-    csvfnb = output_prefix + "_brain.csv"
-    pngfnb = output_prefix + "_brain.png"
+    csvfn = output_prefix + "head.csv"
+    pngfn = output_prefix + "head.png"
+    csvfnb = output_prefix + "brain.csv"
+    pngfnb = output_prefix + "brain.png"
 
     # reference bases
     rbh = pd.read_csv( get_data( "refbasis_head", target_extension=".csv" ) )
     rbb = pd.read_csv( get_data( "refbasis_brain", target_extension=".csv" ) )
 
     # whole head outlierness
     rbp=None
@@ -2549,14 +2549,16 @@
     cit168lab = None
     cit168reg = None
     cit168lab_desc = None
     cit168adni = get_data( "CIT168_T1w_700um_pad_adni",target_extension='.nii.gz')
     cit168adni = ants.image_read( cit168adni ).iMath("Normalize")
     cit168labT = get_data( "det_atlas_25_pad_LR_adni", target_extension='.nii.gz' )
     cit168labT = ants.image_read( cit168labT )
+    cit168labStem = get_data( "CIT168_T1w_700um_pad_adni_brainstem", target_extension='.nii.gz' )
+    cit168labStem = ants.image_read( cit168labStem )
 
     if verbose:
         print("cit168")
 
     cit168reg = region_reg(
             input_image = img,
             input_image_tissue_segmentation=myparc['tissue_segmentation'],
@@ -2616,14 +2618,34 @@
         padding = 4, is_test=False )['synL']
     tbinseg = ants.mask_image( cit168labT, cit168labT, [7,9,23,25,33,34], binarize=False)
     snseg = ants.apply_transforms( img, tbinseg,
         snreg['invtransforms'], interpolator = 'genericLabel' )
     snseg = snseg * ants.threshold_image( myparc['tissue_segmentation'], 2, 6 )
     snseg_desc = map_segmentation_to_dataframe( 'CIT168_Reinf_Learn_v1_label_descriptions_pad', snseg ).dropna(axis=0)
 
+    if verbose:
+        print( "brainstem and cerebellar segmentation" )
+    # midbrain/brainstem
+    brainstemseg = ants.apply_transforms( img, cit168labStem,
+                cit168reg['invtransforms'], interpolator = 'genericLabel' )
+    brainstemseg = brainstemseg * braintissuemask
+    brainstem_desc = map_segmentation_to_dataframe( 'CIT168_T1w_700um_pad_adni_brainstem', brainstemseg )
+    brainstem_desc = brainstem_desc.loc[:, ~brainstem_desc.columns.str.contains('^Side')]
+
+
+    # cerebellum
+    cereb = antspynet.cerebellum_morphology( ants.iMath( x, "Normalize" ), compute_thickness_image=False, verbose=False, do_preprocessing=True )
+    # refinement with cerebellum estimate (comment out since it's not needed for this image).
+    maskc = ants.threshold_image(cereb['cerebellum_probability_image'], 0.5, 1, 1, 0)
+    cereb = antspynet.cerebellum_morphology( ants.iMath( x, "Normalize" ), cerebellum_mask=maskc, compute_thickness_image=False, verbose=False, do_preprocessing=True )
+    cereb_desc = map_segmentation_to_dataframe( 'cerebellum', cereb['parcellation_segmentation_image'] ).dropna(axis=0)
+
+    if verbose:
+        print( "antspyt1w.hierarchical complete" )
+
     mydataframes = {
         "rbp": myqc['brain'],
         "hemispheres":hemi,
         "tissues":tissue,
         "dktlobes":dktl,
         "dktregions":dktp,
         "dktcortex":dktc,
@@ -2632,14 +2654,16 @@
 #        "wmh":myhypo['wmh_summary'],
         "mtl":deep_flash['mtl_description'],
         "bf":deep_bf['description'],
         "cit168":cit168lab_desc,
         "deep_cit168":deep_cit['description'],
         "snseg":snseg_desc,
         "hippLR":hippLR['description'],
+        "brainstem": brainstem_desc,
+        "cerebellum": cereb_desc
         }
 
     outputs = {
         "brain_n4_dnz": img,
         "brain_n4_dnz_png": myqc['brain_image'],
         "brain_extraction": imgbxt,
         "tissue_seg_png": tissue_seg_png,
@@ -2653,14 +2677,16 @@
         "mtl":deep_flash['mtl_segmentation'],
         "bf":deep_bf['segmentation'],
         "deep_cit168lab":  deep_cit['segmentation'],
         "cit168lab":  cit168lab,
         "cit168reg":  cit168reg,
         "snseg":snseg,
         "snreg":snreg,
+        "brainstem": brainstemseg,
+        "cerebellum":cereb['parcellation_segmentation_image'],
         "dataframes": mydataframes
     }
 
     return outputs
 
 
 def trim_segmentation_by_distance( segmentation, which_label, distance ):
@@ -2790,14 +2816,16 @@
     #        "wmh":myhypo['wmh_summary'],
             "mtl":None,
             "bf":None,
             "cit168":None,
             "deep_cit168":None,
             "snseg":None,
             "hippLR":None,
+            "cerebellum":None,
+            "brainstem":None
             }
 
     dkt_parc = {
         "tissue_segmentation":None,
         "tissue_probabilities":None,
         "dkt_parcellation":None,
         "dkt_lobes":None,
@@ -2821,14 +2849,16 @@
             "mtl":None,
             "bf":None,
             "deep_cit168lab":  None,
             "cit168lab":  None,
             "cit168reg":  None,
             "snseg":None,
             "snreg":None,
+            "cerebellum":None,
+            "brainstem":None,
             "dataframes": mydataframes
         }
 
     for myvar in hierarchical_object['dataframes'].keys():
         if hierarchical_object['dataframes'][myvar] is None and exists( output_prefix + myvar + ".csv"):
             hierarchical_object['dataframes'][myvar] = pd.read_csv(output_prefix + myvar + ".csv")
 
@@ -2849,58 +2879,66 @@
 
 
     return hierarchical_object
 
 
 
 
-def write_hierarchical( hierarchical_object, output_prefix ):
+def write_hierarchical( hierarchical_object, output_prefix, verbose=False ):
     """
     standardized writing of output for hierarchical function
 
     Arguments
     ---------
     hierarchical_object : output of antspyt1w.hierarchical
 
     output_prefix : string path including directory and file prefix that will
         be applied to all output, both csv and images.
 
+    verbose: boolean
+
     Returns
     -------
     None
 
     """
 
     # write extant dataframes
     for myvar in hierarchical_object['dataframes'].keys():
         if hierarchical_object['dataframes'][myvar] is not None:
+            if verbose:
+                print( myvar )
             hierarchical_object['dataframes'][myvar].dropna(axis=0).to_csv(output_prefix + myvar + ".csv")
 
     myvarlist = hierarchical_object.keys()
     r16img = ants.image_read( ants.get_data( "r16" ))
     for myvar in myvarlist:
         if hierarchical_object[myvar] is not None and type(hierarchical_object[myvar]) == type( r16img ):
+            if verbose:
+                print( output_prefix + myvar )
             ants.image_write( hierarchical_object[myvar], output_prefix + myvar + '.nii.gz' )
 
     myvarlist = [
         'tissue_segmentation',
         'dkt_parcellation',
         'dkt_lobes',
         'dkt_cortex',
         'hemisphere_labels' ]
     for myvar in myvarlist:
         if hierarchical_object['dkt_parc'][myvar] is not None:
+            if verbose:
+                print( output_prefix + myvar )
             ants.image_write( hierarchical_object['dkt_parc'][myvar], output_prefix + myvar + '.nii.gz' )
 
     return
 
 
 
 
-def merge_hierarchical_csvs_to_wide_format( hierarchical_dataframes, col_names = None , identifier=None, identifier_name='u_hier_id' ):
+def merge_hierarchical_csvs_to_wide_format( hierarchical_dataframes, col_names = None , identifier=None, identifier_name='u_hier_id', verbose=False ):
     """
     standardized merging of output for dataframes produced by hierarchical function.
 
     Arguments
     ---------
     hierarchical_dataframes : output of antspyt1w.hierarchical
 
@@ -2913,14 +2951,16 @@
     data frame in wide format
 
     """
     if identifier is None:
         identifier='A'
     wide_df = pd.DataFrame( )
     for myvar in hierarchical_dataframes.keys():
+        if verbose:
+            print( myvar )
         if hierarchical_dataframes[myvar] is not None:
             jdf = hierarchical_dataframes[myvar].dropna(axis=0)
             jdf = jdf.loc[:, ~jdf.columns.str.contains('^Unnamed')]
             if col_names is not None :
                 for col_name in col_names :
                     if jdf.shape[0] > 1 and any( jdf.columns.str.contains(col_name)):
                         varsofinterest = ["Description", col_name]
```

### Comparing `antspyt1w-0.8.9/antspyt1w.egg-info/PKG-INFO` & `antspyt1w-0.9.0/antspyt1w.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspyt1w
-Version: 0.8.9
+Version: 0.9.0
 Summary: T1w human neuroimage processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyT1w
 Author: Avants, Gosselin, Tustison
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspyt1w-0.8.9/setup.py` & `antspyt1w-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup
 
 long_description = open("README.md").read()
 
 setup(name='antspyt1w',
-      version='0.8.9',
+      version='0.9.0',
       description='T1w human neuroimage processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyT1w',
       author='Avants, Gosselin, Tustison',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspyt1w-0.8.9/tests/test_deep_hipp.py` & `antspyt1w-0.9.0/tests/test_deep_hipp.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/tests/test_mtl.py` & `antspyt1w-0.9.0/tests/test_mtl.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/tests/test_rbp.py` & `antspyt1w-0.9.0/tests/test_rbp.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/tests/test_reference_run.py` & `antspyt1w-0.9.0/tests/test_reference_run.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/tests/test_tissueseg.py` & `antspyt1w-0.9.0/tests/test_tissueseg.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.8.9/tests/test_wmh.py` & `antspyt1w-0.9.0/tests/test_wmh.py`

 * *Files identical despite different names*


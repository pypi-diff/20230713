# Comparing `tmp/GDAL-3.7.0.tar.gz` & `tmp/GDAL-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GDAL-3.7.0.tar", last modified: Wed May 10 15:24:27 2023, max compression
+gzip compressed data, was "GDAL-3.7.1.tar", last modified: Thu Jul 13 17:06:31 2023, max compression
```

## Comparing `GDAL-3.7.0.tar` & `GDAL-3.7.1.tar`

### file list

```diff
@@ -1,143 +1,127 @@
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.177897 GDAL-3.7.0/
--rw-rw-r--   0 even      (1000) even      (1000)     6325 2023-05-10 15:24:27.177897 GDAL-3.7.0/PKG-INFO
--rw-rw-r--   0 even      (1000) even      (1000)     5463 2023-05-10 15:18:45.000000 GDAL-3.7.0/README.rst
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.157897 GDAL-3.7.0/extensions/
--rw-rw-r--   0 even      (1000) even      (1000)   246829 2023-05-10 15:19:00.000000 GDAL-3.7.0/extensions/gdal_array_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)  1797680 2023-05-10 15:19:00.000000 GDAL-3.7.0/extensions/gdal_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)   126161 2023-05-10 15:18:58.000000 GDAL-3.7.0/extensions/gdalconst_wrap.c
--rw-rw-r--   0 even      (1000) even      (1000)   224308 2023-05-10 15:18:59.000000 GDAL-3.7.0/extensions/gnm_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)  1388574 2023-05-10 15:19:00.000000 GDAL-3.7.0/extensions/ogr_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)   761303 2023-05-10 15:19:00.000000 GDAL-3.7.0/extensions/osr_wrap.cpp
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.153897 GDAL-3.7.0/gdal-utils/
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.157897 GDAL-3.7.0/gdal-utils/GDAL.egg-info/
--rw-rw-r--   0 even      (1000) even      (1000)     6325 2023-05-10 15:24:27.000000 GDAL-3.7.0/gdal-utils/GDAL.egg-info/PKG-INFO
--rw-rw-r--   0 even      (1000) even      (1000)     5228 2023-05-10 15:24:27.000000 GDAL-3.7.0/gdal-utils/GDAL.egg-info/SOURCES.txt
--rw-rw-r--   0 even      (1000) even      (1000)        1 2023-05-10 15:24:27.000000 GDAL-3.7.0/gdal-utils/GDAL.egg-info/dependency_links.txt
--rw-rw-r--   0 even      (1000) even      (1000)        1 2023-05-10 15:24:27.000000 GDAL-3.7.0/gdal-utils/GDAL.egg-info/not-zip-safe
--rw-rw-r--   0 even      (1000) even      (1000)       21 2023-05-10 15:24:27.000000 GDAL-3.7.0/gdal-utils/GDAL.egg-info/requires.txt
--rw-rw-r--   0 even      (1000) even      (1000)       18 2023-05-10 15:24:27.000000 GDAL-3.7.0/gdal-utils/GDAL.egg-info/top_level.txt
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.161897 GDAL-3.7.0/gdal-utils/osgeo_utils/
--rw-rw-r--   0 even      (1000) even      (1000)      432 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/__init__.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.165897 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/
--rw-rw-r--   0 even      (1000) even      (1000)        0 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)     2635 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/array_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     4044 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/base.py
--rw-rw-r--   0 even      (1000) even      (1000)     3447 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/batch_creator.py
--rw-rw-r--   0 even      (1000) even      (1000)    15215 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/color_palette.py
--rw-rw-r--   0 even      (1000) even      (1000)     5649 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/color_table.py
--rw-rw-r--   0 even      (1000) even      (1000)     5384 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/extent_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     6566 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py
--rw-rw-r--   0 even      (1000) even      (1000)     2891 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/numpy_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     5467 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/osr_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     3340 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/progress.py
--rw-rw-r--   0 even      (1000) even      (1000)     6671 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/raster_creation.py
--rw-rw-r--   0 even      (1000) even      (1000)     8828 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/rectangle.py
--rw-rw-r--   0 even      (1000) even      (1000)    16651 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/util.py
--rw-rw-r--   0 even      (1000) even      (1000)   166280 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal2tiles.py
--rw-rw-r--   0 even      (1000) even      (1000)    15776 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal2xyz.py
--rw-rw-r--   0 even      (1000) even      (1000)    36237 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_calc.py
--rw-rw-r--   0 even      (1000) even      (1000)    15155 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_edit.py
--rw-rw-r--   0 even      (1000) even      (1000)     9085 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_fillnodata.py
--rw-rw-r--   0 even      (1000) even      (1000)    18296 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_merge.py
--rw-rw-r--   0 even      (1000) even      (1000)    11772 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_pansharpen.py
--rw-rw-r--   0 even      (1000) even      (1000)    11088 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_polygonize.py
--rw-rw-r--   0 even      (1000) even      (1000)     7052 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_proximity.py
--rw-rw-r--   0 even      (1000) even      (1000)    35621 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_retile.py
--rw-rw-r--   0 even      (1000) even      (1000)     6441 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_sieve.py
--rw-rw-r--   0 even      (1000) even      (1000)     4794 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdalattachpct.py
--rw-rw-r--   0 even      (1000) even      (1000)    11855 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdalcompare.py
--rw-rw-r--   0 even      (1000) even      (1000)     9796 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/gdalmove.py
--rw-rw-r--   0 even      (1000) even      (1000)    18278 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/ogr_layer_algebra.py
--rw-rw-r--   0 even      (1000) even      (1000)    42925 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/ogrmerge.py
--rw-rw-r--   0 even      (1000) even      (1000)     7664 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/pct2rgb.py
--rw-rw-r--   0 even      (1000) even      (1000)     7145 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/rgb2pct.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.173897 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/
--rw-rw-r--   0 even      (1000) even      (1000)        0 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)     4632 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/assemblepoly.py
--rw-rw-r--   0 even      (1000) even      (1000)    17347 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py
--rw-rw-r--   0 even      (1000) even      (1000)     2828 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/classify.py
--rw-rw-r--   0 even      (1000) even      (1000)    12326 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/crs2crs2grid.py
--rw-rw-r--   0 even      (1000) even      (1000)    16769 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/densify.py
--rw-rw-r--   0 even      (1000) even      (1000)     8126 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/dump_jp2.py
--rw-rw-r--   0 even      (1000) even      (1000)     9915 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/epsg_tr.py
--rw-rw-r--   0 even      (1000) even      (1000)     3238 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/esri2wkt.py
--rw-rw-r--   0 even      (1000) even      (1000)     4274 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/fft.py
--rw-rw-r--   0 even      (1000) even      (1000)     3008 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/fix_gpkg.py
--rw-rw-r--   0 even      (1000) even      (1000)     3193 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gcps2ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)     5419 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gcps2vec.py
--rw-rw-r--   0 even      (1000) even      (1000)     2580 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gcps2wld.py
--rw-rw-r--   0 even      (1000) even      (1000)     5281 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal2grd.py
--rw-rw-r--   0 even      (1000) even      (1000)     4451 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_auth.py
--rw-rw-r--   0 even      (1000) even      (1000)     8460 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_cp.py
--rw-rw-r--   0 even      (1000) even      (1000)     2561 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py
--rw-rw-r--   0 even      (1000) even      (1000)     8693 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_ls.py
--rw-rw-r--   0 even      (1000) even      (1000)     6668 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_lut.py
--rw-rw-r--   0 even      (1000) even      (1000)     2403 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_mkdir.py
--rw-rw-r--   0 even      (1000) even      (1000)     4426 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py
--rw-rw-r--   0 even      (1000) even      (1000)     4035 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_rm.py
--rw-rw-r--   0 even      (1000) even      (1000)     2538 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_rmdir.py
--rw-rw-r--   0 even      (1000) even      (1000)    11900 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py
--rw-rw-r--   0 even      (1000) even      (1000)     4069 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_zip.py
--rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalchksum.py
--rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalcopyproj.py
--rw-rw-r--   0 even      (1000) even      (1000)     6067 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalfilter.py
--rw-rw-r--   0 even      (1000) even      (1000)     3021 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalident.py
--rw-rw-r--   0 even      (1000) even      (1000)     3036 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalimport.py
--rw-rw-r--   0 even      (1000) even      (1000)    22278 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)    20066 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdallocationinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)     4095 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/get_soundg.py
--rw-rw-r--   0 even      (1000) even      (1000)     3374 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/histrep.py
--rw-rw-r--   0 even      (1000) even      (1000)     8150 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/hsv_merge.py
--rw-rw-r--   0 even      (1000) even      (1000)    10510 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py
--rw-rw-r--   0 even      (1000) even      (1000)     6440 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/load2odbc.py
--rw-rw-r--   0 even      (1000) even      (1000)     8847 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/loslas2ntv2.py
--rw-rw-r--   0 even      (1000) even      (1000)     2739 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/magphase.py
--rw-rw-r--   0 even      (1000) even      (1000)     2167 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py
--rw-rw-r--   0 even      (1000) even      (1000)     7547 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/mkgraticule.py
--rw-rw-r--   0 even      (1000) even      (1000)    70440 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr2ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)    12810 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr2vrt.py
--rw-rw-r--   0 even      (1000) even      (1000)     7567 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py
--rw-rw-r--   0 even      (1000) even      (1000)    14345 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr_dispatch.py
--rw-rw-r--   0 even      (1000) even      (1000)    21229 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogrinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)    19843 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogrupdate.py
--rw-rw-r--   0 even      (1000) even      (1000)     7724 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/rel.py
--rw-rw-r--   0 even      (1000) even      (1000)     7578 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/tigerpoly.py
--rw-rw-r--   0 even      (1000) even      (1000)     4368 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py
--rw-rw-r--   0 even      (1000) even      (1000)     4055 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/tolatlong.py
--rw-rw-r--   0 even      (1000) even      (1000)     4344 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/val_repl.py
--rw-rw-r--   0 even      (1000) even      (1000)    18476 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py
--rw-rw-r--   0 even      (1000) even      (1000)   109775 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/validate_gpkg.py
--rw-rw-r--   0 even      (1000) even      (1000)    70659 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/validate_jp2.py
--rw-rw-r--   0 even      (1000) even      (1000)     4768 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/vec_tr.py
--rw-rw-r--   0 even      (1000) even      (1000)     4843 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/vec_tr_spat.py
--rw-rw-r--   0 even      (1000) even      (1000)     7103 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.177897 GDAL-3.7.0/gdal-utils/scripts/
--rwxrwxr-x   0 even      (1000) even      (1000)      579 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal2tiles.py
--rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal2xyz.py
--rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_calc.py
--rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_edit.py
--rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_fillnodata.py
--rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_merge.py
--rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_pansharpen.py
--rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_polygonize.py
--rwxrwxr-x   0 even      (1000) even      (1000)      335 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_proximity.py
--rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_retile.py
--rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdal_sieve.py
--rwxrwxr-x   0 even      (1000) even      (1000)      331 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdalattachpct.py
--rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdalcompare.py
--rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/gdalmove.py
--rwxrwxr-x   0 even      (1000) even      (1000)      347 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/ogr_layer_algebra.py
--rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/ogrmerge.py
--rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/pct2rgb.py
--rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-05-02 13:04:13.000000 GDAL-3.7.0/gdal-utils/scripts/rgb2pct.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-05-10 15:24:27.177897 GDAL-3.7.0/osgeo/
--rw-rw-r--   0 even      (1000) even      (1000)     4758 2023-05-10 15:19:01.000000 GDAL-3.7.0/osgeo/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)   230510 2023-05-10 15:19:03.000000 GDAL-3.7.0/osgeo/gdal.py
--rw-rw-r--   0 even      (1000) even      (1000)    27867 2023-05-10 15:19:02.000000 GDAL-3.7.0/osgeo/gdal_array.py
--rw-rw-r--   0 even      (1000) even      (1000)    12438 2023-05-10 15:19:02.000000 GDAL-3.7.0/osgeo/gdalconst.py
--rw-rw-r--   0 even      (1000) even      (1000)      214 2023-05-10 15:19:00.000000 GDAL-3.7.0/osgeo/gdalnumeric.py
--rw-rw-r--   0 even      (1000) even      (1000)    13622 2023-05-10 15:19:02.000000 GDAL-3.7.0/osgeo/gnm.py
--rw-rw-r--   0 even      (1000) even      (1000)   227576 2023-05-10 15:19:02.000000 GDAL-3.7.0/osgeo/ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)    58831 2023-05-10 15:19:02.000000 GDAL-3.7.0/osgeo/osr.py
--rw-rw-r--   0 even      (1000) even      (1000)       38 2023-05-10 15:24:27.177897 GDAL-3.7.0/setup.cfg
--rw-rw-r--   0 even      (1000) even      (1000)    13847 2023-05-10 15:18:45.000000 GDAL-3.7.0/setup.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-07-13 17:06:31.713241 GDAL-3.7.1/
+-rw-rw-r--   0 even      (1000) even      (1000)     6325 2023-07-13 17:06:31.713241 GDAL-3.7.1/PKG-INFO
+-rw-rw-r--   0 even      (1000) even      (1000)     5463 2023-07-13 17:04:03.000000 GDAL-3.7.1/README.rst
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-07-13 17:06:31.701240 GDAL-3.7.1/gdal-utils/
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-07-13 17:06:31.705240 GDAL-3.7.1/gdal-utils/GDAL.egg-info/
+-rw-rw-r--   0 even      (1000) even      (1000)     6325 2023-07-13 17:06:31.000000 GDAL-3.7.1/gdal-utils/GDAL.egg-info/PKG-INFO
+-rw-rw-r--   0 even      (1000) even      (1000)     4941 2023-07-13 17:06:31.000000 GDAL-3.7.1/gdal-utils/GDAL.egg-info/SOURCES.txt
+-rw-rw-r--   0 even      (1000) even      (1000)        1 2023-07-13 17:06:31.000000 GDAL-3.7.1/gdal-utils/GDAL.egg-info/dependency_links.txt
+-rw-rw-r--   0 even      (1000) even      (1000)        1 2023-05-10 15:24:27.000000 GDAL-3.7.1/gdal-utils/GDAL.egg-info/not-zip-safe
+-rw-rw-r--   0 even      (1000) even      (1000)       21 2023-07-13 17:06:31.000000 GDAL-3.7.1/gdal-utils/GDAL.egg-info/requires.txt
+-rw-rw-r--   0 even      (1000) even      (1000)       18 2023-07-13 17:06:31.000000 GDAL-3.7.1/gdal-utils/GDAL.egg-info/top_level.txt
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-07-13 17:06:31.705240 GDAL-3.7.1/gdal-utils/osgeo_utils/
+-rw-rw-r--   0 even      (1000) even      (1000)      432 2023-07-06 11:09:16.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/__init__.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-07-13 17:06:31.705240 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/
+-rw-rw-r--   0 even      (1000) even      (1000)        0 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2635 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/array_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4044 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/base.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3447 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/batch_creator.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15215 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/color_palette.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5649 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/color_table.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5384 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/extent_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6566 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2891 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/numpy_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5467 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/osr_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3340 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/progress.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6671 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/raster_creation.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8828 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/rectangle.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16651 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/util.py
+-rw-rw-r--   0 even      (1000) even      (1000)   166280 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal2tiles.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15776 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal2xyz.py
+-rw-rw-r--   0 even      (1000) even      (1000)    36560 2023-07-05 11:52:07.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_calc.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15155 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_edit.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9085 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_fillnodata.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18296 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_merge.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11772 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_pansharpen.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11088 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_polygonize.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7052 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_proximity.py
+-rw-rw-r--   0 even      (1000) even      (1000)    35621 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_retile.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6441 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_sieve.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4794 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdalattachpct.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11855 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdalcompare.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9796 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/gdalmove.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18278 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/ogr_layer_algebra.py
+-rw-rw-r--   0 even      (1000) even      (1000)    42925 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/ogrmerge.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7664 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/pct2rgb.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7145 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/rgb2pct.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-07-13 17:06:31.709241 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/
+-rw-rw-r--   0 even      (1000) even      (1000)        0 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4632 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/assemblepoly.py
+-rw-rw-r--   0 even      (1000) even      (1000)    17347 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2828 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/classify.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12326 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/crs2crs2grid.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16769 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/densify.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8126 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/dump_jp2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9915 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/epsg_tr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3238 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/esri2wkt.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4274 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/fft.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3008 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/fix_gpkg.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3193 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gcps2ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5419 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gcps2vec.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2580 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gcps2wld.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5281 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal2grd.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4451 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_auth.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8460 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_cp.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2561 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8693 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_ls.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6668 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_lut.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2403 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_mkdir.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4426 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4035 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_rm.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2538 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_rmdir.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11900 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4069 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_zip.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalchksum.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalcopyproj.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6067 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalfilter.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3021 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalident.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3036 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalimport.py
+-rw-rw-r--   0 even      (1000) even      (1000)    22278 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)    20066 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdallocationinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4095 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/get_soundg.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3374 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/histrep.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8150 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/hsv_merge.py
+-rw-rw-r--   0 even      (1000) even      (1000)    10510 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6440 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/load2odbc.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8847 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/loslas2ntv2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2739 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/magphase.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2167 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7547 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/mkgraticule.py
+-rw-rw-r--   0 even      (1000) even      (1000)    70440 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr2ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12810 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr2vrt.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7567 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py
+-rw-rw-r--   0 even      (1000) even      (1000)    14345 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr_dispatch.py
+-rw-rw-r--   0 even      (1000) even      (1000)    21229 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogrinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)    19843 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogrupdate.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7724 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/rel.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7578 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/tigerpoly.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4368 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4055 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/tolatlong.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4344 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/val_repl.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18476 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py
+-rw-rw-r--   0 even      (1000) even      (1000)   112045 2023-06-24 14:56:05.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/validate_gpkg.py
+-rw-rw-r--   0 even      (1000) even      (1000)    70659 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/validate_jp2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4768 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/vec_tr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4843 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/vec_tr_spat.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7103 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-07-13 17:06:31.713241 GDAL-3.7.1/gdal-utils/scripts/
+-rwxrwxr-x   0 even      (1000) even      (1000)      579 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal2tiles.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal2xyz.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_calc.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_edit.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_fillnodata.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_merge.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_pansharpen.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_polygonize.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      335 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_proximity.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_retile.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdal_sieve.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      331 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdalattachpct.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdalcompare.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/gdalmove.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      347 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/ogr_layer_algebra.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/ogrmerge.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/pct2rgb.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-05-02 13:04:13.000000 GDAL-3.7.1/gdal-utils/scripts/rgb2pct.py
+-rw-rw-r--   0 even      (1000) even      (1000)       38 2023-07-13 17:06:31.713241 GDAL-3.7.1/setup.cfg
+-rw-rw-r--   0 even      (1000) even      (1000)    13847 2023-07-13 17:04:03.000000 GDAL-3.7.1/setup.py
```

### Comparing `GDAL-3.7.0/PKG-INFO` & `GDAL-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GDAL
-Version: 3.7.0
+Version: 3.7.1
 Summary: GDAL: Geospatial Data Abstraction Library
 Home-page: http://www.gdal.org
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Howard Butler
 Maintainer-email: hobu.inc@gmail.com
 License: MIT
@@ -37,15 +37,15 @@
 bindings for GDAL and OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the `GDAL API Tutorial`_ includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.7.0 or greater) and header files (gdal-devel)
+ * libgdal (3.7.1 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.7.0/README.rst` & `GDAL-3.7.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 bindings for GDAL and OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the `GDAL API Tutorial`_ includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.7.0 or greater) and header files (gdal-devel)
+ * libgdal (3.7.1 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.7.0/gdal-utils/GDAL.egg-info/PKG-INFO` & `GDAL-3.7.1/gdal-utils/GDAL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GDAL
-Version: 3.7.0
+Version: 3.7.1
 Summary: GDAL: Geospatial Data Abstraction Library
 Home-page: http://www.gdal.org
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Howard Butler
 Maintainer-email: hobu.inc@gmail.com
 License: MIT
@@ -37,15 +37,15 @@
 bindings for GDAL and OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the `GDAL API Tutorial`_ includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.7.0 or greater) and header files (gdal-devel)
+ * libgdal (3.7.1 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.7.0/gdal-utils/GDAL.egg-info/SOURCES.txt` & `GDAL-3.7.1/gdal-utils/GDAL.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 README.rst
 setup.py
-extensions/gdal_array_wrap.cpp
-extensions/gdal_wrap.cpp
-extensions/gdalconst_wrap.c
-extensions/gnm_wrap.cpp
-extensions/ogr_wrap.cpp
-extensions/osr_wrap.cpp
 gdal-utils/GDAL.egg-info/PKG-INFO
 gdal-utils/GDAL.egg-info/SOURCES.txt
 gdal-utils/GDAL.egg-info/dependency_links.txt
 gdal-utils/GDAL.egg-info/not-zip-safe
 gdal-utils/GDAL.egg-info/requires.txt
 gdal-utils/GDAL.egg-info/top_level.txt
 gdal-utils/osgeo_utils/__init__.py
@@ -117,16 +111,8 @@
 gdal-utils/scripts/gdal_sieve.py
 gdal-utils/scripts/gdalattachpct.py
 gdal-utils/scripts/gdalcompare.py
 gdal-utils/scripts/gdalmove.py
 gdal-utils/scripts/ogr_layer_algebra.py
 gdal-utils/scripts/ogrmerge.py
 gdal-utils/scripts/pct2rgb.py
-gdal-utils/scripts/rgb2pct.py
-osgeo/__init__.py
-osgeo/gdal.py
-osgeo/gdal_array.py
-osgeo/gdalconst.py
-osgeo/gdalnumeric.py
-osgeo/gnm.py
-osgeo/ogr.py
-osgeo/osr.py
+gdal-utils/scripts/rgb2pct.py
```

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/array_util.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/array_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/base.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/base.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/batch_creator.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/batch_creator.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/color_palette.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/color_palette.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/color_table.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/color_table.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/extent_util.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/extent_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/numpy_util.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/numpy_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/osr_util.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/osr_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/progress.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/progress.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/raster_creation.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/raster_creation.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/rectangle.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/rectangle.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/auxiliary/util.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/auxiliary/util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal2tiles.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal2tiles.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal2xyz.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal2xyz.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_calc.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
             myOut.SetGeoTransform(GeoTransformCheck)
 
         if not ProjectionCheck:
             ProjectionCheck = myFiles[0].GetProjection()
         if ProjectionCheck:
             myOut.SetProjection(ProjectionCheck)
 
-        if NoDataValue is None:
+        if NoDataValue is None and not hideNoData:
             myOutNDV = DefaultNDVLookup[
                 myOutType
             ]  # use the default noDataValue for this datatype
         elif isinstance(NoDataValue, str) and NoDataValue.lower() == "none":
             myOutNDV = None  # not to set any noDataValue
         else:
             myOutNDV = NoDataValue  # use the given noDataValue
@@ -461,17 +461,14 @@
                 if is_path_like(color_table):
                     color_table = get_color_table(color_table)
                 myOutB.SetRasterColorTable(color_table)
                 myOutB.SetRasterColorInterpretation(gdal.GCI_PaletteIndex)
 
             myOutB = None  # write to band
 
-        if hideNoData:
-            myOutNDV = None
-
     myOutTypeName = gdal.GetDataTypeName(myOutType)
     if debug:
         print(
             f"output file: {outfile}, dimensions: {myOut.RasterXSize}, {myOut.RasterYSize}, type: {myOutTypeName}"
         )
 
     ################################################################
@@ -750,14 +747,24 @@
                     type=int,
                     help=f"number of raster band for file {alpha} (default 1)",
                     metavar="n",
                 )
             except argparse.ArgumentError:
                 pass
 
+    def float_or_none(self, NoDataValue: str) -> Union[float, str]:
+        if NoDataValue.lower() == "none":
+            return NoDataValue
+
+        try:
+            return float(NoDataValue)
+        except ValueError:
+            msg = f"Invalid float value for NoDataValue: {NoDataValue}"
+            raise argparse.ArgumentTypeError(msg)
+
     def get_parser(self, argv) -> GDALArgumentParser:
         parser = self.parser
         parser.add_argument(
             "--calc",
             dest="calc",
             type=str,
             required=True,
@@ -777,15 +784,15 @@
             required=True,
             metavar="filename",
             help="output file to generate or fill",
         )
         parser.add_argument(
             "--NoDataValue",
             dest="NoDataValue",
-            type=float,
+            type=self.float_or_none,
             metavar="value",
             help="output nodata value (default datatype specific value)",
         )
         parser.add_argument(
             "--hideNoData",
             dest="hideNoData",
             action="store_true",
```

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_edit.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_edit.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_fillnodata.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_fillnodata.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_merge.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_merge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_pansharpen.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_pansharpen.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_polygonize.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_polygonize.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_proximity.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_proximity.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_retile.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_retile.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdal_sieve.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdal_sieve.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdalattachpct.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdalattachpct.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdalcompare.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdalcompare.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/gdalmove.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/gdalmove.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/ogr_layer_algebra.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/ogr_layer_algebra.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/ogrmerge.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/ogrmerge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/pct2rgb.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/pct2rgb.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/rgb2pct.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/rgb2pct.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/assemblepoly.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/assemblepoly.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/classify.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/classify.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/crs2crs2grid.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/crs2crs2grid.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/densify.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/densify.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/dump_jp2.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/dump_jp2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/epsg_tr.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/epsg_tr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/esri2wkt.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/esri2wkt.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/fft.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/fft.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/fix_gpkg.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/fix_gpkg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gcps2ogr.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gcps2ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gcps2vec.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gcps2vec.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gcps2wld.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gcps2wld.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal2grd.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal2grd.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_auth.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_auth.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_cp.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_cp.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_ls.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_ls.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_lut.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_lut.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_mkdir.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_mkdir.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_rm.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_rm.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_rmdir.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_rmdir.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdal_zip.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdal_zip.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalchksum.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalchksum.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalcopyproj.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalcopyproj.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalfilter.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalfilter.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalident.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalident.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalimport.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalimport.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdalinfo.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdalinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/gdallocationinfo.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/gdallocationinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/get_soundg.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/get_soundg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/histrep.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/histrep.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/hsv_merge.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/hsv_merge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/load2odbc.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/load2odbc.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/loslas2ntv2.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/loslas2ntv2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/magphase.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/magphase.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/mkgraticule.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/mkgraticule.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr2ogr.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr2ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr2vrt.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr2vrt.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogr_dispatch.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogr_dispatch.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogrinfo.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogrinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/ogrupdate.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/ogrupdate.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/rel.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/rel.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/tigerpoly.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/tigerpoly.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/tolatlong.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/tolatlong.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/val_repl.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/val_repl.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/validate_gpkg.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/validate_gpkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,16 @@
         abort_at_first_error=True,
         extra_checks=False,
         log_msg=False,
         warning_msg=True,
         warning_as_error=False,
     ):
         self.filename = filename
+        self.conn = None
+        self.has_tried_spatialite = False
         self.extended_pragma_info = False
         self.abort_at_first_error = abort_at_first_error
         self.extra_checks = extra_checks
         self.log_msg = log_msg
         self.warning_msg = warning_msg
         self.warning_as_error = warning_as_error
         self.errors = []
@@ -665,39 +667,72 @@
         )
         geom_column_name = rows_gpkg_geometry_columns[0][0]
         z = rows_gpkg_geometry_columns[0][1]
         m = rows_gpkg_geometry_columns[0][2]
         geometry_type_name = rows_gpkg_geometry_columns[0][3]
         srs_id = rows_gpkg_geometry_columns[0][4]
 
-        c.execute("PRAGMA table_info(%s)" % _esc_id(table_name))
+        c.execute(
+            "SELECT 1 FROM sqlite_master WHERE name = ? and type = 'view'",
+            (table_name,),
+        )
+        is_view = c.fetchone() is not None
+        is_spatialite_computed_column = False
+        if is_view:
+            c.execute("SELECT 1 FROM sqlite_master WHERE name = 'gpkg_extensions'")
+            if c.fetchone() is not None:
+                c.execute(
+                    "SELECT 1 FROM gpkg_extensions WHERE table_name = ? AND column_name = ? AND extension_name = 'gdal_spatialite_computed_geom_column'",
+                    (table_name, geom_column_name),
+                )
+                if c.fetchone() is not None:
+                    is_spatialite_computed_column = True
+
+        try:
+            c.execute("PRAGMA table_info(%s)" % _esc_id(table_name))
+        except sqlite3.OperationalError as e:
+            if not self.has_tried_spatialite:
+                self.has_tried_spatialite = True
+                spatialite_loaded = False
+                try:
+                    self.conn.enable_load_extension(True)
+                    self.conn.execute('SELECT load_extension("mod_spatialite")')
+                    spatialite_loaded = True
+                except Exception:
+                    pass
+                if not spatialite_loaded:
+                    raise e
+                c.execute("PRAGMA table_info(%s)" % _esc_id(table_name))
+
         cols = c.fetchall()
+
         found_geom = False
         count_pkid = 0
         pkid_column_name = None
         for (_, name, typ, notnull, default, pk) in cols:
             if name.lower() == geom_column_name.lower():
                 found_geom = True
-                self._assert(
-                    typ in GPKGChecker.BASE_GEOM_TYPES
-                    or typ in GPKGChecker.EXT_GEOM_TYPES,
-                    25,
-                    ("invalid type (%s) for geometry " + "column of table %s")
-                    % (typ, table_name),
-                )
-                self._assert(
-                    typ == geometry_type_name,
-                    31,
-                    (
-                        "table %s has geometry column of type %s in "
-                        + "SQL and %s in geometry_type_name of "
-                        + "gpkg_geometry_columns"
+                if not is_spatialite_computed_column:
+                    self._assert(
+                        typ in GPKGChecker.BASE_GEOM_TYPES
+                        or typ in GPKGChecker.EXT_GEOM_TYPES,
+                        25,
+                        ("invalid type (%s) for geometry " + "column of table %s")
+                        % (typ, table_name),
+                    )
+                    self._assert(
+                        typ == geometry_type_name,
+                        31,
+                        (
+                            "table %s has geometry column of type %s in "
+                            + "SQL and %s in geometry_type_name of "
+                            + "gpkg_geometry_columns"
+                        )
+                        % (table_name, typ, geometry_type_name),
                     )
-                    % (table_name, typ, geometry_type_name),
-                )
 
             elif pk == 1:
                 if pkid_column_name is None:
                     pkid_column_name = name
                 count_pkid += 1
                 self._assert(
                     typ == "INTEGER",
@@ -1013,24 +1048,36 @@
                 "SELECT 1 FROM sqlite_master WHERE type = 'trigger' "
                 + "AND name = '%s_insert'" % _esc_literal(rtree_name)
             )
             self._assert(
                 c.fetchone() is not None, 75, "%s_insert trigger missing" % rtree_name
             )
 
-            for i in range(4):
-                c.execute(
-                    "SELECT 1 FROM sqlite_master WHERE "
-                    + "type = 'trigger' "
-                    + "AND name = '%s_update%d'" % (_esc_literal(rtree_name), i + 1)
-                )
+            if self.version < (1, 4):
+                expected_update_triggers_numbers = (1, 2, 3, 4)
+            else:
+                expected_update_triggers_numbers = (2, 4, 5, 6, 7)
+
+            c.execute(
+                "SELECT name FROM sqlite_master WHERE "
+                + "type = 'trigger' "
+                + "AND name LIKE '%s_update%%'" % (_esc_literal(rtree_name))
+            )
+            trigger_names = c.fetchall()
+            found_numbers = set()
+            for (name,) in trigger_names:
+                number = int(name[len(_esc_literal(rtree_name)) + len("_update") :])
+                if number not in expected_update_triggers_numbers:
+                    self._assert(False, 75, f"{name} trigger unexpected")
+                found_numbers.add(number)
+            for expected_number in expected_update_triggers_numbers:
                 self._assert(
-                    c.fetchone() is not None,
+                    expected_number in found_numbers,
                     75,
-                    "%s_update%d trigger missing" % (rtree_name, i + 1),
+                    "%s_update%d trigger missing" % (rtree_name, expected_number),
                 )
 
             c.execute(
                 "SELECT 1 FROM sqlite_master WHERE type = 'trigger' "
                 + "AND name = '%s_delete'" % _esc_literal(rtree_name)
             )
             self._assert(
@@ -2793,18 +2840,20 @@
                 self._assert(
                     user_version >= expected_version,
                     2,
                     "Wrong user_version: %d. Expected >= %d"
                     % (user_version, expected_version),
                 )
                 self.version = (
-                    expected_version // 10000,
-                    (expected_version % 10000) // 100,
-                    expected_version % 100,
+                    user_version // 10000,
+                    (user_version % 10000) // 100,
+                    user_version % 100,
                 )
+                if self.version >= (1, 5, 0):
+                    self._warn(f"Version {self.version} not handled by this script")
             else:
                 self.version = (99, 99)
 
         conn = sqlite3.connect(":memory:")
         c = conn.cursor()
         c.execute(
             "CREATE TABLE foo(one TEXT, two TEXT, "
@@ -2814,14 +2863,15 @@
         rows = c.fetchall()
         if rows[1][5] == 2:
             self.extended_pragma_info = True
         c.close()
         conn.close()
 
         conn = sqlite3.connect(self.filename)
+        self.conn = conn
         c = conn.cursor()
         try:
             try:
                 c.execute("SELECT 1 FROM sqlite_master")
                 c.fetchone()
             except Exception:
                 self._assert(False, 1, "not a sqlite3 database")
```

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/validate_jp2.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/validate_jp2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/vec_tr.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/vec_tr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/vec_tr_spat.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/vec_tr_spat.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py` & `GDAL-3.7.1/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/gdal-utils/scripts/gdal2tiles.py` & `GDAL-3.7.1/gdal-utils/scripts/gdal2tiles.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.7.0/setup.py` & `GDAL-3.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 packages = find_packages(utils_package_root)
 packages = ['osgeo'] + packages
 package_dir = {'osgeo': 'osgeo', '': utils_package_root}
 
 readme = open('README.rst', encoding="utf-8").read()
 
 name = 'GDAL'
-version = '3.7.0'
+version = '3.7.1'
 author = "Frank Warmerdam"
 author_email = "warmerdam@pobox.com"
 maintainer = "Howard Butler"
 maintainer_email = "hobu.inc@gmail.com"
 description = "GDAL: Geospatial Data Abstraction Library"
 license_type = "MIT"
 url = "http://www.gdal.org"
```


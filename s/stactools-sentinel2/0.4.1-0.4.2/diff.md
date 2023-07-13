# Comparing `tmp/stactools-sentinel2-0.4.1.tar.gz` & `tmp/stactools-sentinel2-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-sentinel2-0.4.1.tar", last modified: Fri Apr 28 11:34:52 2023, max compression
+gzip compressed data, was "stactools-sentinel2-0.4.2.tar", last modified: Thu Jul 13 20:38:47 2023, max compression
```

## Comparing `stactools-sentinel2-0.4.1.tar` & `stactools-sentinel2-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.754932 stactools-sentinel2-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.754932 stactools-sentinel2-0.4.1/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/src/stactools/sentinel2/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/granule_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/mgrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/product_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/safe_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22081 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/tileinfo_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-28 11:34:41.000000 stactools-sentinel2-0.4.1/src/stactools/sentinel2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:34:52.758932 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 11:34:52.000000 stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:38:47.800556 stactools-sentinel2-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 20:38:47.800556 stactools-sentinel2-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-13 20:38:47.800556 stactools-sentinel2-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:38:47.796556 stactools-sentinel2-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:38:47.796556 stactools-sentinel2-0.4.2/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:38:47.800556 stactools-sentinel2-0.4.2/src/stactools/sentinel2/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/granule_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/mgrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/product_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/safe_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/tileinfo_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-13 20:38:35.000000 stactools-sentinel2-0.4.2/src/stactools/sentinel2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:38:47.800556 stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 20:38:47.000000 stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 20:38:47.000000 stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:38:47.000000 stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 20:38:47.000000 stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 20:38:47.000000 stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/top_level.txt
```

### Comparing `stactools-sentinel2-0.4.1/LICENSE` & `stactools-sentinel2-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/PKG-INFO` & `stactools-sentinel2-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel2
-Version: 0.4.1
+Version: 0.4.2
 Summary: Create STAC Items from Sentinel-2 metadata
 Home-page: https://github.com/stactools-sentinel2/stactools-sentinel2
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Issues, https://github.com/stactools-sentinel2s/stactools-sentinel2/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-sentinel2-0.4.1/README.md` & `stactools-sentinel2-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/setup.cfg` & `stactools-sentinel2-0.4.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 [options]
 python_requires = >=3.8
 package_dir = 
 	= src
 packages = find_namespace:
 install_requires = 
-	stactools >= 0.4.2
+	antimeridian >= 0.3.1
+	stactools >= 0.4.8
 	pystac >= 1.7.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/cog.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/cog.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/commands.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/constants.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/granule_metadata.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/granule_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/mgrs.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/mgrs.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/product_metadata.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/product_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/safe_manifest.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/safe_manifest.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/stac.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/stac.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import math
 import os
 import re
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import chain
 from typing import Any, Dict, Final, List, Optional, Pattern, Tuple
 
@@ -10,14 +11,17 @@
 import shapely
 from pystac.extensions.eo import Band, EOExtension
 from pystac.extensions.grid import GridExtension
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.raster import DataType, RasterBand, RasterExtension
 from pystac.extensions.sat import OrbitState, SatExtension
 from pystac.extensions.view import ViewExtension
+from shapely.geometry import mapping as shapely_mapping
+from shapely.geometry import shape as shapely_shape
+from shapely.validation import make_valid
 from stactools.core.io import ReadHrefModifier
 from stactools.core.projection import reproject_geom, transform_from_bbox
 from stactools.core.utils import antimeridian
 from stactools.core.utils.antimeridian import Strategy
 
 from stactools.sentinel2.constants import (
     BANDS_TO_ASSET_NAME,
@@ -126,17 +130,20 @@
         metadata = metadata_from_safe_manifest(granule_href, read_href_modifier)
     else:
         metadata = metadata_from_granule_metadata(
             granule_href, read_href_modifier, tolerance
         )
     created = datetime.now().strftime("%Y-%m-%dT%H:%MZ")
 
+    # ensure that we have a valid geometry
+    geometry = shapely_mapping(make_valid(shapely_shape(metadata.geometry)))
+
     item = pystac.Item(
         id=metadata.scene_id,
-        geometry=metadata.geometry,
+        geometry=geometry,
         bbox=metadata.bbox,
         datetime=metadata.datetime,
         properties={"created": created},
     )
 
     # Handle antimeridian if necessary
     antimeridian.fix_item(item, antimeridian_strategy)
@@ -170,16 +177,46 @@
     # Projection Extension
     projection = ProjectionExtension.ext(item, add_if_missing=True)
     projection.epsg = metadata.epsg
     if projection.epsg is None:
         raise ValueError(
             f"Could not determine EPSG code for {granule_href}; which is required."
         )
-    centroid = shapely.geometry.shape(item.geometry).centroid
-    projection.centroid = {"lat": round(centroid.y, 5), "lon": round(centroid.x, 5)}
+
+    # It is assumed that any MultiPolygon is an antimeridian-crossing scene.
+    # If we used split, the code below "normalizes" the polygon with negative longitude to
+    # have positive longitude greater than 180, then takes the centroid of this new
+    # MultiPolygon, and the un-normalize it back to within (-180,180).
+    if (
+        antimeridian_strategy == Strategy.SPLIT
+        and item.geometry
+        and item.geometry.get("type") == "MultiPolygon"
+    ):
+        shapely_geometry = shapely_shape(item.geometry)
+        # force all positive lons so we can merge on an antimeridian split
+        polys = list(shapely_geometry.geoms)
+        for index, poly in enumerate(polys):
+            coords = list(poly.exterior.coords)
+            lons = [coord[0] for coord in coords]
+            if min(lons) < 0:
+                polys[index] = shapely.affinity.translate(poly, xoff=+360)
+
+        # make_valid merges the normalized MultiPolygon into a single normalized Polygon
+        # and removes any line artifacts that may exist.
+        normalized_geometry = make_valid(shapely.geometry.MultiPolygon(polys))
+
+        centroid = normalized_geometry.centroid
+        lon = centroid.x
+        if lon > 180:
+            lon = lon - 360
+    else:
+        centroid = shapely_shape(item.geometry).centroid
+        lon = centroid.x
+
+    projection.centroid = {"lat": round(centroid.y, 5), "lon": round(lon, 5)}
 
     # MGRS and Grid Extension
     mgrs_match = MGRS_PATTERN.search(metadata.scene_id)
     if mgrs_match and len(mgrs_groups := mgrs_match.groups()) == 3:
         mgrs = MgrsExtension.ext(item, add_if_missing=True)
         mgrs.utm_zone = int(mgrs_groups[0])
         mgrs.latitude_band = mgrs_groups[1]
@@ -188,27 +225,34 @@
         grid.code = f"MGRS-{mgrs.utm_zone}{mgrs.latitude_band}{mgrs.grid_square}"
     else:
         logger.error(
             f"Error populating MGRS and Grid Extensions fields from ID: {metadata.scene_id}"
         )
 
     # View Extension
-    view = ViewExtension.ext(item, add_if_missing=True)
-    view.sun_azimuth = metadata.sun_azimuth
-    if msz := metadata.sun_zenith:
+
+    # both sun_azimuth and sun_zenith can be NaN, so don't set
+    # when that is the case
+    if (msa := metadata.sun_azimuth) and not math.isnan(msa):
+        view = ViewExtension.ext(item, add_if_missing=True)
+        view.sun_azimuth = msa
+
+    if (msz := metadata.sun_zenith) and not math.isnan(msz):
+        view = ViewExtension.ext(item, add_if_missing=True)
         view.sun_elevation = 90 - msz
 
     # s2 properties
     item.properties.update(metadata.metadata_dict)
 
     # --Assets--
 
     image_assets = dict(
         [
             image_asset_from_href(
+                item=item,
                 asset_href=os.path.join(asset_href_prefix or granule_href, image_path),
                 resolution_to_shape=metadata.resolution_to_shape,
                 proj_bbox=metadata.proj_bbox,
                 media_type=metadata.image_media_type,
                 processing_baseline=metadata.processing_baseline,
                 viewing_angles=metadata.viewing_angles,
                 boa_add_offsets=metadata.boa_add_offsets,
@@ -225,14 +269,15 @@
 
     item.links.append(SENTINEL_LICENSE)
 
     return item
 
 
 def image_asset_from_href(
+    item: pystac.Item,
     asset_href: str,
     resolution_to_shape: Dict[int, Tuple[int, int]],
     proj_bbox: List[float],
     media_type: Optional[str],
     processing_baseline: str,
     viewing_angles: Dict[str, ViewingAngle],
     boa_add_offsets: Optional[Dict[str, int]] = None,
@@ -331,16 +376,25 @@
             media_type=asset_media_type,
             title=f"{band.description} - {asset_res}m",
             roles=["data", "reflectance"],
         )
         viewing_angle = viewing_angles[band_id]
         # We can't use the ViewExtension here until
         # https://github.com/stac-utils/pystac/issues/793 is fixed
-        asset.extra_fields["view:azimuth"] = viewing_angle.azimuth
-        asset.extra_fields["view:incidence_angle"] = viewing_angle.zenith
+        if not math.isnan(viewing_angle.azimuth):
+            # View Extension doesn't specify fields in Assets,
+            # but if it does, this should be uncommented
+            # ViewExtension.ext(item, add_if_missing=True)
+            asset.extra_fields["view:azimuth"] = viewing_angle.azimuth
+
+        if not math.isnan(viewing_angle.zenith):
+            # View Extension doesn't specify fields in Assets,
+            # but if it does, this should be uncommented
+            # ViewExtension.ext(item, add_if_missing=True)
+            asset.extra_fields["view:incidence_angle"] = viewing_angle.zenith
 
         asset_eo = EOExtension.ext(asset)
         asset_eo.bands = [band_from_band_id(band_id)]
         set_asset_properties(asset, band_gsd)
 
         RasterExtension.ext(asset).bands = raster_bands(
             boa_add_offsets, processing_baseline, band_id, resolution
@@ -536,15 +590,15 @@
         f = (
             granule_metadata_href.split("tiles/")[0]
             + tileinfo_metadata.product_path
             + "/metadata.xml"
         )
         product_metadata = ProductMetadata(f, read_href_modifier)
 
-    geometry = shapely.geometry.shape(
+    geometry = shapely_shape(
         reproject_geom(
             f"epsg:{granule_metadata.epsg}", "epsg:4326", tileinfo_metadata.geometry
         )
     ).simplify(tolerance)
 
     extra_assets = dict(
         [
@@ -569,15 +623,15 @@
         scene_id=granule_metadata.scene_id,
         extra_assets=extra_assets,
         metadata_dict=metadata_dict,
         cloudiness_percentage=granule_metadata.cloudiness_percentage,
         epsg=granule_metadata.epsg,
         proj_bbox=granule_metadata.proj_bbox,
         resolution_to_shape=granule_metadata.resolution_to_shape,
-        geometry=shapely.geometry.mapping(geometry),
+        geometry=shapely_mapping(geometry),
         bbox=geometry.bounds,
         datetime=tileinfo_metadata.datetime,
         platform=granule_metadata.platform,
         image_media_type=pystac.MediaType.JPEG2000,
         image_paths=image_paths,
         sun_zenith=granule_metadata.mean_solar_zenith,
         sun_azimuth=granule_metadata.mean_solar_azimuth,
```

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/tileinfo_metadata.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/tileinfo_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools/sentinel2/utils.py` & `stactools-sentinel2-0.4.2/src/stactools/sentinel2/utils.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/PKG-INFO` & `stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel2
-Version: 0.4.1
+Version: 0.4.2
 Summary: Create STAC Items from Sentinel-2 metadata
 Home-page: https://github.com/stactools-sentinel2/stactools-sentinel2
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Issues, https://github.com/stactools-sentinel2s/stactools-sentinel2/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-sentinel2-0.4.1/src/stactools_sentinel2.egg-info/SOURCES.txt` & `stactools-sentinel2-0.4.2/src/stactools_sentinel2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


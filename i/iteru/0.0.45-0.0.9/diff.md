# Comparing `tmp/iteru-0.0.45.tar.gz` & `tmp/iteru-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iteru-0.0.45.tar", last modified: Thu Jul 13 09:45:25 2023, max compression
+gzip compressed data, was "iteru-0.0.9.tar", last modified: Wed Mar 16 11:23:27 2022, max compression
```

## Comparing `iteru-0.0.45.tar` & `iteru-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:25.204504 iteru-0.0.45/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 09:45:15.000000 iteru-0.0.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-13 09:45:15.000000 iteru-0.0.45/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-13 09:45:25.204504 iteru-0.0.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-13 09:45:15.000000 iteru-0.0.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:25.200504 iteru-0.0.45/iteru/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 09:45:15.000000 iteru-0.0.45/iteru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-13 09:45:15.000000 iteru-0.0.45/iteru/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    26763 2023-07-13 09:45:15.000000 iteru-0.0.45/iteru/iterugee.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-13 09:45:15.000000 iteru-0.0.45/iteru/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:45:25.204504 iteru-0.0.45/iteru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-13 09:45:25.000000 iteru-0.0.45/iteru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-13 09:45:25.000000 iteru-0.0.45/iteru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 09:45:25.000000 iteru-0.0.45/iteru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:45:25.000000 iteru-0.0.45/iteru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 09:45:25.000000 iteru-0.0.45/iteru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 09:45:25.000000 iteru-0.0.45/iteru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 09:45:15.000000 iteru-0.0.45/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 09:45:25.204504 iteru-0.0.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-13 09:45:15.000000 iteru-0.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 11:23:27.397113 iteru-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-03-16 11:23:08.000000 iteru-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-03-16 11:23:08.000000 iteru-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-03-16 11:23:27.397113 iteru-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-03-16 11:23:08.000000 iteru-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 11:23:27.397113 iteru-0.0.9/iteru/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-03-16 11:23:08.000000 iteru-0.0.9/iteru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-03-16 11:23:08.000000 iteru-0.0.9/iteru/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-03-16 11:23:08.000000 iteru-0.0.9/iteru/gui_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35305 2022-03-16 11:23:08.000000 iteru-0.0.9/iteru/iteru.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 11:23:27.397113 iteru-0.0.9/iteru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-03-16 11:23:27.000000 iteru-0.0.9/iteru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-03-16 11:23:27.000000 iteru-0.0.9/iteru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-03-16 11:23:27.000000 iteru-0.0.9/iteru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 11:23:27.000000 iteru-0.0.9/iteru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-03-16 11:23:27.000000 iteru-0.0.9/iteru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-16 11:23:27.000000 iteru-0.0.9/iteru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-03-16 11:23:08.000000 iteru-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-16 11:23:27.397113 iteru-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-03-16 11:23:08.000000 iteru-0.0.9/setup.py
```

### Comparing `iteru-0.0.45/LICENSE` & `iteru-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iteru-0.0.45/iteru/iterugee.py` & `iteru-0.0.9/iteru/iteru.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,280 @@
-""" A Main Module for Google Earth Engine Python API Functions """
+"""The main module for the interactive mapping based on Google Earth Enigne Python API and Ipyleaflet Package """
 
-import ee
+
+from IPython.display import display
+from .common import *
+from .gui_widgets import *
 from ipywidgets import *
 import ipyleaflet
-from IPython.display import display
+import geemap
+import ee
 import datetime
-from .common import *
-from statistics import mode
+import matplotlib.pyplot as plt
+
+
+class Map(geemap.Map):
+    """ Inherting the Map class from Ipyleaflet with the all its methods and attributes
+
+    """
+
+    def __init__(self, **kwargs):
+        
+        Map.zoom_control = False
+        
+        if 'center' not in kwargs:
+            kwargs['center'] = [27, 31]
+
+        if 'zoom' not in kwargs:
+            kwargs['zoom'] = 5
+
+        if 'scroll_wheel_zoom' not in kwargs:
+            kwargs['scroll_wheel_zoom'] = True
+
+        if 'height' not in kwargs:
+            self.layout.height = '500px'
+        else:
+            self.layout.height = kwargs['height']
+
+        super().__init__(**kwargs)
+        
+        
+        self.clear_controls()
+        self.add_control(ipyleaflet.SearchControl(
+
+            position="topleft",
+            url='https://nominatim.openstreetmap.org/search?format=json&q={s}',
+            zoom=10,
+            marker=ipyleaflet.Marker(
+                icon=ipyleaflet.AwesomeIcon(name="check",
+                                            marker_color='green', icon_color='darkgreen')
+            )
+        )
+        )
+
+        self.add_control(ipyleaflet.ScaleControl(position='bottomleft'))
+
+        self.add_control(ipyleaflet.LayersControl(position='topleft'))
+
+        self.add_control(ipyleaflet.ZoomControl(position='topright'))
+
+        self.add_control(ipyleaflet.FullScreenControl(position='topright'))
+
+        draw_control = ipyleaflet.DrawControl(position='topright')
+
+        draw_control.polyline = {
+            "shapeOptions": {
+                "color": "blue",
+                "weight": 8,
+                "opacity": 0.5
+            }
+        }
+        draw_control.polygon = {
+            "shapeOptions": {
+                "fillColor": "blue",
+                "color": "red",
+                "fillOpacity": 0.1
+            },
+            "drawError": {
+                "color": "#dd253b",
+                "message": "Oups!"
+            },
+            "allowIntersection": False
+        }
+        draw_control.circle = {
+            "shapeOptions": {
+                "fillColor": "blue",
+                "color": "red",
+                "fillOpacity": 0.1
+            }
+        }
+        draw_control.rectangle = {
+            "shapeOptions": {
+                "fillColor": "blue",
+                "color": "red",
+                "fillOpacity": 0.1
+            }
+        }
+
+        self.add_control(draw_control)
+        self.draw_control = draw_control
+        self.last_draw = draw_control.last_draw
+        self.last_action = draw_control.last_action
+
+        def handle_draw(target, action, geo_json):
+            self.last_draw = geo_json
+            self.last_action = action
+            if self.last_draw['geometry']['type'] == 'Polygon':
+                self.aoi = ee.Geometry.Polygon(
+                    self.last_draw['geometry']['coordinates'])
+            elif self.last_draw['geometry']['type'] == 'Point':
+                self.aoi = ee.Geometry.Point(
+                    self.last_draw['geometry']['coordinates'])
+            elif self.last_draw['geometry']['type'] == 'LineString':
+                self.aoi = ee.Geometry.LineString(
+                    self.last_draw['geometry']['coordinates'])
+
+        self.draw_control.on_draw(handle_draw)
+
+        measure = ipyleaflet.MeasureControl(
+            position='topright',
+            active_color='orange',
+            primary_length_unit='kilometers',
+            secondary_length_unit=('miles'),
+            secondary_area_unit=('acres')
+        )
+
+        measure.add_area_unit('Sq Kilometers', 1e-6, 4)
+        measure.primary_area_unit = ('Sq Kilometers')
+        self.add_control(measure)
+
+        self.add_control(TOC_widget)
+
+        def add_to_map(change):
+            if change.new:
+                self.add_layer_widgets(change.new)
+
+        # add coordinates of the mousemove to the map
+        def from_decimal_to_degree(angle):
+            degrees = int(angle)
+            minutes = (angle - degrees)*60
+            seconds = (minutes - int(minutes)) * 60
+            return f"{degrees}°{int(minutes)}'{seconds:.4f}”"
+
+        coordinates = HTML()
+
+        def handle_interaction(**kwargs):
+            if kwargs.get('type') == 'mousemove':
+                coordinates.value = f"""
+                                    <b>Lat</b>: {from_decimal_to_degree(float(str(kwargs.get('coordinates')[0])))}
+                                    <br>
+                                    <b>Long</b>: {from_decimal_to_degree(float(str(kwargs.get('coordinates')[1])))}
+                                    <br>
+                                    <b>Zoom Level</b>: {int(self.zoom)}
+                                    """
+            if kwargs.get('type') == 'click':
+                JAXA = ee.ImageCollection(
+                    'JAXA/ALOS/AW3D30/V3_2').select('DSM').median()
+                lat = float(str(kwargs.get('coordinates')[0]))
+                long = float(str(kwargs.get('coordinates')[1]))
+                point_elevation = JAXA.reduceRegion(
+                    reducer=ee.Reducer.mean(),
+                    geometry=ee.Geometry.Point(long, lat),
+                    scale=10,).getInfo()
+                coordinates.value = f"""
+                                    <b>Lat</b>: {from_decimal_to_degree(float(str(kwargs.get('coordinates')[0])))}
+                                    <br>
+                                    <b>Long</b>: {from_decimal_to_degree(float(str(kwargs.get('coordinates')[1])))}
+                                    <br>
+                                    <b>Zoom Level</b>: {int(self.zoom)}
+                                    <br>
+                                    <b>Elevation</b>:{point_elevation['DSM']}
+                                    """
+
+        self.on_interaction(handle_interaction)
+        coordinates_widget = WidgetControl(
+            widget=coordinates, position='bottomleft')
+        self.add_control(coordinates_widget)
+
+    def add_layer_widgets(self, object, vis_params=None, name=None):
+        try:
+            if isinstance(object, ee.Image) or isinstance(object, ee.ImageCollection) or (object, ee.FeatureCollection):
+                layer = ee_tilelayer(object, vis_params)
+                if name is None:
+                    name = object.getInfo()['id']
+
+            elif isinstance(object, ipyleaflet.TileLayer):
+                layer = object
+                if name is None:
+                    name = object.name
+        except:
+            print('input layer is not supported ')
+
+        try:
+            self.add_layer(layer)
+
+            close_button = Button(
+                value=False,
+                tooltip='Remove This Layer',
+                icon='window-close',
+                layout=Layout(width='32px', height='28px'),
+            )
+
+            layer_visibility = Checkbox(
+                value=True,
+                indent=False,
+                layout=Layout(width='15px')
+            )
+
+            layer_name = Label(
+                value=name,
+                layout=Layout(width='150px', height='28px'),
+                tooltip=name
+            )
+            opacity = FloatSlider(
+                value=1,
+                min=0,
+                max=1,
+                step=0.1,
+                indent=False,
+            )
+
+            def change_layer_visibility(show_hide):
+                layer.visible = show_hide
+
+            def change_layer_opacity(Opacity):
+                layer.opacity = Opacity
+
+            def remove_layer(b):
+                self.remove_layer(layer)
+                close_button.close()
+                opacity.close()
+                layer_name.close()
+                layer_visibility.close()
+
+            opacity_slider = interactive(change_layer_opacity, Opacity=opacity)
+
+            visibility_checkbox = interactive(
+                change_layer_visibility, show_hide=layer_visibility)
+
+            with TOC_out:
+                display(
+                    HBox([layer_visibility, layer_name, opacity, close_button]))
+
+            close_button.on_click(remove_layer)
+
+        except Exception:
+            pass
+            #print(f'layer already on the map: {layer}')
+
+    def zoom_to(self, ee_object, zoom=8):
+
+        try:
+            lat = ee_object.geometry().centroid().getInfo()['coordinates'][1]
+            long = ee_object.geometry().centroid().getInfo()['coordinates'][0]
+            self.center = (lat, long)
+            self.zoom = zoom
+        except:
+            self.center = (27, 31)
+            self.zoom = 5
+            print('Error: can not get the centroid of the Object')
+
+    def add_ee_layer(self, ee_object, vis_params=None, name=''):
+
+        map_id_dict = ee_object.getMapId(vis_params)
+
+        ee_object_tile = ipyleaflet.TileLayer(
+
+            url=map_id_dict['tile_fetcher'].url_format,
+            attr='Map Data &copy; <a href="https://earthengine.google.com/">Google Earth Engine</a>',
+            name=name,
+            overlay=True,
+            control=True
+        )
+        self.add_layer(ee_object_tile)
 
 
 def ee_tilelayer(ee_object, vis_params=None, name=''):
 
     ee_object_id = ee_object.getMapId(vis_params)
 
     ee_object_tile = ipyleaflet.TileLayer(
@@ -27,15 +291,15 @@
 def get_vis_params(collection):
     """A fucntion to get the visualiztions paramters of GEE ImageCollection Feature
 
     Args:
         collection ([ImageCollection]): [GEE ImageColelction]
 
     Returns:
-        [dict]: [Visualization paramters]
+        [dict]: [Visualization paramters ]
     """
     min = float(collection.getInfo()['properties']['visualization_0_min'])
     max = float(collection.getInfo()['properties']['visualization_0_max'])
     bands = collection.getInfo(
     )['properties']['visualization_0_bands'].split(',')
     return {'min': min, 'max': max, 'bands': bands}
 
@@ -45,20 +309,98 @@
 
 
 def get_imgCol_dates(col):
     col = col.map(add_dates_to_imgcol)
     return col.aggregate_array('DATE').getInfo()
 
 
-def get_imgCol_dates_dict(col):
+def get_gif(url):
 
-    dates_dict = {formated_date: date for formated_date, date in zip(
-        get_imgCol_dates(col), col.aggregate_array('system:time_start').getInfo())}
+    import requests
+    import os
 
-    return dates_dict
+    r = requests.get(url, stream=True)
+    out_dir = os.path.join(os.path.expanduser("~"), "Downloads")
+    filename = "TimeSeries_" + random_string() + ".gif"
+    out_gif = os.path.join(out_dir, filename)
+
+    with open(out_gif, 'wb') as file:
+        for chunk in r.iter_content(chunk_size=1024):
+            file.write(chunk)
+
+    return out_gif
+
+
+def random_string(string_length=4):
+    import random
+    import string
+
+    letters = string.ascii_uppercase
+    return "".join(random.choice(letters) for i in range(string_length))
+
+
+def add_text_to_gif(out_gif, dates_list,
+                    dates_font_size=25,
+                    copywrite_font_size=15,
+                    dates_font_color='red',
+                    copywrite_font_color='black',
+                    framesPerSecond=4):
+
+    from PIL import Image, ImageDraw, ImageFont, ImageSequence
+    import io
+
+    gif = Image.open(out_gif)
+    count = gif.n_frames
+
+    width, height = gif.size
+    dates_text_xy = (int(0.001 * width), int(0.001 * height))
+    copywrite_xy = (int(0.001 * width), int(0.98 * height))
+
+    dates_text = dates_list
+    copywrite = '©Muhammed Abdelaal, 2022'
+    dates_text_font = ImageFont.truetype(
+        r'C:\Users\muham\Downloads\News 705 Italic BT\News 705 Italic BT.ttf', dates_font_size)
+    copywrite_font = ImageFont.truetype(
+        r'C:\Users\muham\Downloads\News 705 Italic BT\News 705 Italic BT.ttf', copywrite_font_size)
+
+    frames = []
+
+    for index, frame in enumerate(ImageSequence.Iterator(gif)):
+        frame = frame.convert("RGB")
+        draw = ImageDraw.Draw(frame)
+        draw.text(dates_text_xy, dates_text[index],
+                  fill=dates_font_color, font=dates_text_font)
+        draw.text(copywrite_xy, copywrite,
+                  fill=copywrite_font_color, font=copywrite_font)
+        b = io.BytesIO()
+        frame.save(b, format="GIF")
+        frame = Image.open(b)
+        frames.append(frame)
+
+    frames[0].save(
+        out_gif,
+        save_all=True,
+        append_images=frames[1:],
+        duration=int(1000/framesPerSecond),
+        loop=0,
+        optimize=True,
+    )
+
+
+def display_gif(out_gif):
+
+    from ipywidgets import Image
+
+    out = Output()
+    out.clear_output(wait=True)
+    display(out)
+    with out:
+        with open(out_gif, 'rb') as file:
+            image = file.read()
+        display(Image(value=image))
 
 
 def dates_params(startYear=2020, startMonth=6, startDay=1, endYear=2022, endMonth=3, endDay=1):
 
     if all(isinstance(i, int) for i in [startYear, startMonth, startDay, endYear, endMonth, endDay]):
 
         valid_startDate = datetime.date(2020, 1, 1)
@@ -116,47 +458,66 @@
         days.pop()
 
     days_dates = [f'{date.year}-{date.month}-{date.day}' for date in days]
 
     return days_dates
 
 
+GERD_aoi = ee.Geometry.Polygon([[[
+    35.008243,
+    10.522199
+],
+    [
+    35.008243,
+    11.266588
+],
+    [
+    35.387092,
+    11.266588
+],
+    [
+    35.387092,
+    10.522199
+],
+    [
+    35.008243,
+    10.522199
+]]])
+
+
 def addRatioBand(img):
     ratio_band = img.select('VV').divide(img.select('VH')).rename('VV/VH')
 
     return img.addBands(ratio_band)
 
 
 def filterSpeckles(img):
 
     VH_smooth = img.select('VH').focal_median(
         100, 'circle', 'meters').rename('VH_Filtered')
 
     return img.addBands(VH_smooth)
 
 
-def water_classify_threshold(col, threshold):
+water_threshold = -25
 
-    def water_classify(img):
 
-        VH_Filtered = img.select('VH_Filtered')
-        water = VH_Filtered.lt(threshold).rename('water')
-        water_mask = water.updateMask(water).rename('water_mask')
-
-        return img.addBands([water, water_mask])
-
-    return col.map(water_classify)
+def water_classify(img):
+    vv = img.select('VH_Filtered')
+    water = vv.lt(water_threshold).rename('Water')
+    water_mask = water.updateMask(water).rename('Water_mask')
+    return img.addBands([water_mask])
 
 
 def rgb_water_mosaic(img):
 
     img_rgb = img.visualize(
-        **{'min': [-40, -40, -3], 'max': [5, 5, 5], 'bands': ['VV', 'VH', 'VV/VH']})
+        **{'min': [-35, -35, 0], 'max': [0, 0, 5], 'bands': ['VV', 'VH', 'VV/VH']})
 
-    water_vis = img.select('water_mask').visualize(
+    water_vis = img.select('Water_mask').visualize(
         **{'min': 0.5, 'max': 1, 'palette': ['00FFFF', '0000FF']})
 
     mosaic = ee.ImageCollection([img_rgb, water_vis]).mosaic()
 
     return mosaic.copyProperties(img, img.propertyNames())
 
 
@@ -254,15 +615,15 @@
                                 get_images_sequence)
 
                             SAR = ee.ImageCollection.fromImages(images)
 
                             return [SAR, dates_sequence]
 
 
-def SAR_timeseries_url(col, aoi, vis_method='rgb', water_threshold=-25, frame_per_second=2, crs='EPSG:3857', dimensions=900):
+def SAR_timeseries_url(col, aoi, vis_method='rgb', frame_per_second=2, crs='EPSG:3857', dimensions=900):
 
     try:
         if isinstance(col, ee.ImageCollection):
             pass
         else:
             raise Exception('The input should be ee.ImageCollection')
 
@@ -281,54 +642,42 @@
     palette = None
     vis_min = -35,
     vis_max = 5,
 
     try:
         if vis_method == 'rgb':
 
-            vis_min = [-40, -40, -3]
-            vis_max = [5, 5, 5]
+            vis_min = [-35, -35, 0]
+            vis_max = [0, 0, 5]
             bands = ['VV', 'VH', 'VV/VH']
 
         elif vis_method == 'single_band_VV':
             bands = ['VV']
-            palette = ['#000000', '#FFFFFF']
-
-        elif vis_method == 'single_band_VV_R':
-            bands = ['VV']
-            palette = ['#FFFFFF', '#000000']
 
         elif vis_method == 'single_band_VH':
-            bands = ['VH']
-            palette = ['#000000', '#FFFFFF']
-
-        elif vis_method == 'single_band_VH_R':
 
             bands = ['VH']
-            palette = ['#FFFFFF', '#000000']
 
-        elif vis_method == 'water_mask':
+        elif vis_method == 'water_mask_only':
 
-            col = col.map(filterSpeckles)
-            col = water_classify_threshold(col, water_threshold)
-            bands = ['water_mask']
+            col = col.map(filterSpeckles).map(water_classify)
+            bands = ['Water_mask']
             palette = ['00FFFF', '0000FF']
 
         elif vis_method == 'rgb_water_mosaic':
 
-            col = col.map(filterSpeckles)
-            col = water_classify_threshold(col, water_threshold)
-            col = col.map(rgb_water_mosaic)
+            col = col.map(filterSpeckles).map(
+                water_classify).map(rgb_water_mosaic)
 
             bands = ['vis-red', 'vis-green', 'vis-blue']
             vis_min = 0
             vis_max = 255
         else:
             raise Exception('Invalid visualization method input. The visualization method should be'
-                            '"rgb","singl_band_VV","single_band_VH","single_band_VH_R","single_band_VH_R","water_mask" or "rgb_water_mosaic"')
+                            '"rgb","singl_band_VV","single_band_VH","water_mask_only" or "rgb_water_mosaic"')
 
     except Exception as e:
         print(e)
         return
     else:
 
         videoArgs = {
@@ -361,15 +710,15 @@
     area = feature.geometry().area(maxError=1)
 
     return feature.set({'Area': area})
 
 
 def water_to_vector(img):
 
-    water_mask = img.select('water_mask').clip(GERD_aoi)
+    water_mask = img.select('Water_mask').clip(GERD_aoi)
 
     feature = ee.Image(1).updateMask(water_mask).reduceToVectors(
         geometry=water_mask.geometry(),
         crs='EPSG:32636',
         scale=10,
         geometryType='polygon',
         eightConnected=False,
@@ -383,14 +732,22 @@
     lake_area = lake_feature.geometry().area(maxError=1)
 
     return ee.FeatureCollection(lake_feature).set({'Area': lake_area})\
         .copyProperties(img, img.propertyNames())\
         .copyProperties(lake_feature, lake_feature.propertyNames())
 
 
+elevation_dataset = ee.ImageCollection('JAXA/ALOS/AW3D30/V3_2')\
+    .filter(ee.Filter.bounds(GERD_aoi))\
+    .select('DSM')\
+    .median()\
+    .clip(GERD_aoi)\
+    .reproject(crs='EPSG:32636', scale=30)
+
+
 def max_water_ele(feature):
 
     lake_dem = elevation_dataset.clip(feature)
 
     max_ele = lake_dem.reduceRegion(
         reducer=ee.Reducer.max(),
         geometry=lake_dem.geometry(),
@@ -428,16 +785,14 @@
 
 def toNatural(img):
     return ee.Image(10.0).pow(img.select(0).divide(10.0))
 
 
 def RefinedLee(img):
 
-    # ©2018 Guido Lemoine, European Commission, Joint Research Centre
-
     weights3 = ee.List.repeat(ee.List.repeat(1, 3), 3)
     kernel3 = ee.Kernel.fixed(3, 3, weights3, 1, 1, False)
 
     mean3 = img.reduceNeighborhood(ee.Reducer.mean(), kernel3)
     variance3 = img.reduceNeighborhood(ee.Reducer.variance(), kernel3)
 
     sample_weights = ee.List([[0, 0, 0, 0, 0, 0, 0], [0, 1, 0, 1, 0, 1, 0], [0, 0, 0, 0, 0, 0, 0],
@@ -529,16 +884,14 @@
         toDB(RefinedLee(toNatural(img.select(['VH']))))).rename('VH_Filtered')
 
     return img.addBands(VH_Filtered)
 
 
 def otsu(histogram):
 
-    # ©2017, Nicholas Clinton, Developer Advocate, Google Earth Engine
-
     counts = ee.Array(ee.Dictionary(histogram).get('histogram'))
     means = ee.Array(ee.Dictionary(histogram).get('bucketMeans'))
     size = means.length().get([0])
     total = counts.reduce(ee.Reducer.sum(), [0]).get([0])
     sum = means.multiply(counts).reduce(ee.Reducer.sum(), [0]).get([0])
     mean = sum.divide(total)
 
@@ -581,29 +934,26 @@
     return water.set({"otsu_threshold": otsu_threshold})
 
 
 def GERD_SAR_timelaspe(aoi=GERD_aoi,
                        startYear=2020,
                        startMonth=6,
                        startDay=1,
-                       endYear=2022,
-                       endMonth=3,
-                       endDay=19,
+                       endYear=2020,
+                       endMonth=6,
+                       endDay=10,
                        temp_freq=None,
                        vis_method='rgb',
-                       water_threshold=-25,
                        crs='EPSG:3857',
                        dimensions=900,
                        dates_font_size=25,
                        copywrite_font_size=15,
                        dates_font_color='red',
                        copywrite_font_color='black',
                        framesPerSecond=2,
-                       zoom_level='Zoom Level: 14',
-                       zoom_level_font_size=20
                        ):
     try:
         SAR_col = S1_SAR_col(aoi, startYear, startMonth,
                              startDay, endYear, endMonth, endDay, temp_freq)
 
     except Exception as e:
         print(e)
@@ -612,46 +962,69 @@
         if isinstance(SAR_col, list):
             SAR = SAR_col[0]
             dates_sequences = SAR_col[1]
 
             try:
 
                 url = SAR_timeseries_url(
-                    SAR, aoi, vis_method, water_threshold, framesPerSecond, crs, dimensions)
+                    SAR, aoi, vis_method, framesPerSecond, crs, dimensions)
 
             except Exception as e:
                 print(e)
                 return
 
             else:
                 if url:
 
                     out_gif = get_gif(url)
 
-                    out_gif = add_text_to_gif(out_gif, dates_sequences,
-                                              dates_font_size,
-                                              copywrite_font_size,
-                                              dates_font_color,
-                                              copywrite_font_color,
-                                              framesPerSecond,
-                                              zoom_level,
-                                              zoom_level_font_size)
-
-                    return out_gif
+                    add_text_to_gif(out_gif, dates_sequences,
+                                    dates_font_size,
+                                    copywrite_font_size,
+                                    dates_font_color,
+                                    copywrite_font_color,
+                                    framesPerSecond)
+
+                    display_gif(out_gif)
+
+
+def show_plot(x, y,
+              x_label, y_label,
+              xlabel_fontsize=15,
+              ylabel_fontsize=18,
+              xticks_rotation=90,
+              figwitdth=10,
+              figheight=7,
+              style='fivethirtyeight',
+              grid_status=True,
+              legend_label=None
+              ):
+
+    import matplotlib.pyplot as plt
+    plt.style.use(style)
+    f = plt.figure()
+    f.set_figwidth(figwitdth)
+    f.set_figheight(figheight)
+    plt.xlabel(x_label, fontsize=xlabel_fontsize)
+    plt.ylabel(y_label, fontsize=ylabel_fontsize)
+    plt.grid(grid_status)
+    plt.xticks(rotation=xticks_rotation)
+    plt.plot(x, y, label=legend_label)
+    plt.legend()
+    plt.gcf().set_size_inches(18.5, 10.5)
 
 
 def GERD_water_stats(aoi=GERD_aoi,
                      startYear=2020,
                      startMonth=6,
                      startDay=1,
                      endYear=2022,
                      endMonth=3,
                      endDay=15,
                      temp_freq='monthly',
-                     water_threshold=-25,
                      water_area=True,
                      water_level=False,
                      water_volume=False,
                      ):
 
     try:
         SAR_col = S1_SAR_col(aoi, startYear, startMonth,
@@ -678,41 +1051,36 @@
 
         else:
 
             try:
                 water_stats = {}
                 water_stats['image_date'] = dates_sequences
                 if water_area:
-                    SAR = SAR.map(filterSpeckles)
-                    SAR = water_classify_threshold(SAR, water_threshold)
-                    water_vectors = SAR.map(water_to_vector)
-
+                    water_vectors = SAR.map(filterSpeckles).map(
+                        water_classify).map(water_to_vector)
                     water_area = [
                         area / (1e6) for area in water_vectors.aggregate_array('Area').getInfo()]
                     water_stats['water_surface_area'] = water_area
 
                 if water_level:
                     if not water_area:
-
-                        SAR = SAR.map(filterSpeckles)
-                        SAR = water_classify_threshold(SAR, water_threshold)
-                        water_vectors = SAR.map(water_to_vector)
+                        water_vectors = SAR.map(filterSpeckles).map(
+                            water_classify).map(water_to_vector)
 
                     dems = water_vectors.map(max_water_ele)
 
                     max_elev = [elev for elev in dems.aggregate_array(
                         'Maximum_water_elevation').getInfo()]
                     water_stats['maximum_elevation'] = max_elev
 
                 if water_volume:
 
                     if not water_area:
-                        SAR = SAR.map(filterSpeckles)
-                        SAR = water_classify_threshold(SAR, water_threshold)
-                        water_vectors = SAR.map(water_to_vector)
+                        water_vectors = SAR.map(filterSpeckles).map(
+                            water_classify).map(water_to_vector)
                     if not water_level:
                         dems = water_vectors.map(max_water_ele)
                         max_elev = [elev for elev in dems.aggregate_array(
                             'Maximum_water_elevation').getInfo()]
 
                     volume_stats = dems.map(water_vol)
                     ele_sum = volume_stats.aggregate_array(
@@ -723,90 +1091,7 @@
                               for water_level, elevations_sum, pixles_count in zip(max_elev, ele_sum, pixel_num)]
                     water_stats['water_volume'] = volume
 
                 return water_stats
 
             except:
                 print('Error! Memory Limit Exceeded.')
-
-
-def SAR_VV_stats_single_img(system_start_time, aoi):
-
-    SAR = ee.ImageCollection('COPERNICUS/S1_GRD')\
-        .filter(ee.Filter.equals('relativeOrbitNumber_start', 50))\
-        .filter(ee.Filter.eq('instrumentMode', 'IW'))\
-        .filter(ee.Filter.eq('orbitProperties_pass', 'DESCENDING'))\
-        .filter(ee.Filter.listContains('transmitterReceiverPolarisation', 'VH'))\
-        .filter(ee.Filter.listContains('transmitterReceiverPolarisation', 'VV'))\
-        .filter(ee.Filter.eq('resolution_meters', 10))\
-        .filterBounds(aoi)\
-        .filter(ee.Filter.eq('system:time_start', system_start_time))\
-        .select(['VV'])\
-        .median()
-
-    VV_smooth = ee.Image(
-        toDB(RefinedLee(toNatural(SAR.select(['VV']))))).rename('VV_Filtered')
-
-    histogram_VV = VV_smooth.select('VV_Filtered').reduceRegion(
-        reducer=ee.Reducer.histogram().combine(
-            'mean', None, True).combine('variance', None, True),
-        geometry=aoi,
-        scale=10,
-        bestEffort=True)
-
-    otsu_threshold_VV = otsu(histogram_VV.get('VV_Filtered_histogram'))
-
-    water_mask_VV = VV_smooth.select('VV_Filtered').lt(
-        otsu_threshold_VV).selfMask().rename('water_mask')
-
-    water_mask_VV = water_mask_VV.select('water_mask').clip(aoi)
-
-    feature_VV = ee.Image(1).updateMask(water_mask_VV).reduceToVectors(
-        geometry=water_mask_VV.geometry(),
-        crs='EPSG:32636',
-        scale=30,
-        geometryType='polygon',
-        eightConnected=False,
-        labelProperty='water_cover',
-        bestEffort=True
-    )
-
-    feature_VV = feature_VV.map(calc_area)
-
-    lake_feature_VV = feature_VV.sort('Area', False).first()
-
-    lake_area_VV = lake_feature_VV.geometry().area(maxError=1)
-
-    pix_num = lake_area_VV.getInfo()/1e5
-
-    lake_dem_VV = fabdem.clip(lake_feature_VV)
-
-    elevations_VV = lake_dem_VV.reduceRegion(
-        reducer=ee.Reducer.toList(),
-        geometry=lake_dem_VV.geometry(),
-        maxPixels=1e11,
-        scale=30,
-        crs='EPSG:32636',
-        bestEffort=True
-    ).get('b1')
-
-    elevations_list_VV = ee.List(elevations_VV).getInfo()
-
-    elevations_desc_VV = sorted(elevations_list_VV, reverse=True)
-
-    water_level_VV = mode(elevations_desc_VV[100:round(0.5*pix_num)])
-
-    volume_VV = ((water_level_VV*len(elevations_desc_VV) -
-                 sum(elevations_desc_VV))*900)/1e9
-
-    stats = {'Otsu_threshold': otsu_threshold_VV.getInfo(),
-             'Area': lake_area_VV.getInfo()/1e6,
-             'Level': water_level_VV,
-             'Volume': volume_VV
-             }
-
-    layers = {'SAR_VV': VV_smooth,
-
-              'Waterbody': lake_feature_VV
-              }
-
-    return (stats, layers)
```

### Comparing `iteru-0.0.45/setup.py` & `iteru-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,10 +50,10 @@
     keywords='iteru',
     name='iteru',
     packages=find_packages(include=['iteru', 'iteru.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MuhammedM294/iteru',
-    version='0.0.45',
+    version='0.0.9',
     zip_safe=False,
 )
```


# Comparing `tmp/chartspy-2.0.9.tar.gz` & `tmp/chartspy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/chartspy/chartspy/dist/.tmp-3c0daihl/chartspy-2.0.9.tar", last modified: Sun Feb 19 10:13:13 2023, max compression
+gzip compressed data, was "chartspy-2.1.1.tar", last modified: Thu Jul 13 02:49:34 2023, max compression
```

## Comparing `chartspy-2.0.9.tar` & `chartspy-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-19 10:13:13.000000 chartspy-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2023-02-19 10:13:04.000000 chartspy-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      755 2023-02-19 10:13:13.000000 chartspy-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3572 2023-02-19 10:13:04.000000 chartspy-2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy/
--rw-r--r--   0 runner    (1001) docker     (116)      563 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9218 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/base.py
--rw-r--r--   0 runner    (1001) docker     (116)   168433 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/charts.py
--rw-r--r--   0 runner    (1001) docker     (116)    20470 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/echarts.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy/express/
--rw-r--r--   0 runner    (1001) docker     (116)       71 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/express/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83768 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/express/echarts.py
--rw-r--r--   0 runner    (1001) docker     (116)    13521 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/express/g2plot.py
--rw-r--r--   0 runner    (1001) docker     (116)     3047 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/express/highcharts.py
--rw-r--r--   0 runner    (1001) docker     (116)     7151 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/g2plot.py
--rw-r--r--   0 runner    (1001) docker     (116)    10496 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/highcharts.py
--rw-r--r--   0 runner    (1001) docker     (116)     8119 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/klinecharts.py
--rw-r--r--   0 runner    (1001) docker     (116)    13416 2023-02-19 10:13:04.000000 chartspy-2.0.9/chartspy/tabulator.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      755 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      496 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-19 10:13:12.000000 chartspy-2.0.9/chartspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2023-02-19 10:13:13.000000 chartspy-2.0.9/chartspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-19 10:13:13.000000 chartspy-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1501 2023-02-19 10:13:04.000000 chartspy-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:49:34.831700 chartspy-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 02:49:26.000000 chartspy-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 02:49:34.831700 chartspy-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-13 02:49:26.000000 chartspy-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:49:34.831700 chartspy-2.1.1/chartspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168433 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20470 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/echarts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:49:34.831700 chartspy-2.1.1/chartspy/express/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/express/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84234 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/express/echarts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/express/g2plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/express/highcharts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/g2plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/highcharts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/klinecharts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-07-13 02:49:26.000000 chartspy-2.1.1/chartspy/tabulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:49:34.831700 chartspy-2.1.1/chartspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 02:49:34.000000 chartspy-2.1.1/chartspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 02:49:34.000000 chartspy-2.1.1/chartspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:49:34.000000 chartspy-2.1.1/chartspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:49:34.000000 chartspy-2.1.1/chartspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 02:49:34.000000 chartspy-2.1.1/chartspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 02:49:34.000000 chartspy-2.1.1/chartspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 02:49:34.831700 chartspy-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-13 02:49:26.000000 chartspy-2.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chartspy-2.0.9/LICENSE` & `chartspy-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/PKG-INFO` & `chartspy-2.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartspy
-Version: 2.0.9
+Version: 2.1.1
 Summary: echarts g2plot klinechart highcharts tabulator python wrapper
 Home-page: https://chartspy.icopy.site/
 Author: yiliuyan
 Author-email: yiliuyan161@126.com
 Maintainer: yiliuyan
 Maintainer-email: yiliuyan161@126.com
 Keywords: echarts g2plot klinechart highcharts tabulator python
```

### Comparing `chartspy-2.0.9/README.md` & `chartspy-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/__init__.py` & `chartspy-2.1.1/chartspy/__init__.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/base.py` & `chartspy-2.1.1/chartspy/base.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/charts.py` & `chartspy-2.1.1/chartspy/charts.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/echarts.py` & `chartspy-2.1.1/chartspy/echarts.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/express/echarts.py` & `chartspy-2.1.1/chartspy/express/echarts.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,14 +297,15 @@
         }
     }
     return Echarts(options=options, width=width, height=height)
 
 
 def line_echarts(data_frame: pd.DataFrame, x_field: str = None, y_field: str = None, series_field: str = None,
                  tooltip_trigger="axis",
+                 y_scale=True,
                  title: str = "",
                  width: str = "100%", height: str = "500px") -> Echarts:
     """
     绘制线图
     :param data_frame: 必填 DataFrame
     :param x_field: 必填 x轴映射的列
     :param y_field: 必填 y轴映射的列
@@ -320,14 +321,15 @@
     df = data_frame.copy()
     if x_field is None:
         df["x_col_echartspy"] = df.index
         x_field = "x_col_echartspy"
     options['title'] = {"text": title}
     if "date" in str(df[x_field].dtype) or "object" in str(df[x_field].dtype):
         options['xAxis']['type'] = 'category'
+    options['yAxis']['scale'] = y_scale
     if series_field is not None:
         series_list = list(df[series_field].unique())
         for s in series_list:
             series = {'name': s, 'type': 'line', 'dimensions': [x_field, y_field],
                       'data': df[df[series_field] == s][[x_field, y_field]].values.tolist()}
             options['legend']['data'].append(s)
             options['series'].append(series)
@@ -407,14 +409,15 @@
 
     return Echarts(options=options, width=width, height=height)
 
 
 def bar_echarts(data_frame: pd.DataFrame, x_field: str = None, y_field: str = None, series_field: str = None,
                 stack: str = "all",
                 tooltip_trigger="axis",
+                y_scale=True,
                 title: str = "",
                 width: str = "100%", height: str = "500px") -> Echarts:
     """
 
     :param data_frame: 必填 DataFrame
     :param x_field: 必填 x轴映射的列
     :param y_field: 必填 y轴映射的列
@@ -431,14 +434,15 @@
     title = y_field if title == '' else title
     if x_field is None:
         df["x_col_echartspy"] = df.index
         x_field = "x_col_echartspy"
     options['title'] = {"text": title}
     if "date" in str(df[x_field].dtype) or "object" in str(df[x_field].dtype):
         options['xAxis']['type'] = 'category'
+    options['yAxis']['scale'] = y_scale
     if series_field is not None:
         series_list = list(df[series_field].unique())
         for s in series_list:
             series = {'name': s, 'type': 'bar', 'stack': stack, 'dimensions': [x_field, y_field], 'sampling': 'lttb',
                       'data': df[df[series_field] == s][[x_field, y_field]].values.tolist(), 'emphasis': {
                     'itemStyle': {
                         'borderColor': "#333",
@@ -608,17 +612,22 @@
     df = data_frame.copy()
     if time_field not in data_frame.columns:  # 使用index作为时间
         df[time_field] = df.index
     df[close_field] = df[close_field].fillna(method="ffill")
     df[open_field] = df[open_field].fillna(df[close_field])
     df[high_field] = df[high_field].fillna(df[close_field])
     df[low_field] = df[low_field].fillna(df[close_field])
+    df['uplimit'] = df[close_field] > df[close_field].shift(1) * 1.098
+    df['dnlimit'] = df[close_field] < df[close_field].shift(1) * 0.902
+    bars = [{'value': [row[open_field], row[close_field], row[low_field], row[high_field]],
+             'itemStyle': ({"borderWidth": 4} if (row['uplimit'] or row['dnlimit']) else {})} for row in
+            df.to_dict(orient="records")]
     df[volume_field] = df[volume_field].fillna(0)
     volumes = (df[volume_field]).round(2).tolist()
-    vol_filter = (df[volume_field]).quantile([0.05, 0.95]).values
+    vol_filter = (df[volume_field]).quantile([0.10, 0.90]).values
     bar_items = [({"value": vol} if vol >= vol_filter[0] and vol <= vol_filter[1] else (
         {"value": vol, "itemStyle": {"color": "red"}} if vol > vol_filter[1] else {"value": vol,
                                                                                    "itemStyle": {"color": "green"}}))
                  for vol in volumes]
 
     options = {
         'animation': False,
@@ -657,20 +666,20 @@
                                         }
                                     }else{
                                         label.push("<div style='max-width:15em;word-break:break-all;white-space: normal;'>"+dimensionNames[j]+':&nbsp;'+value+"</div>");
                                     }
                             }
                         }else if(param['seriesType']=="candlestick"){
                                 label.push("<br/>");
-                                label.push("<span>open:&nbsp;"+param['data'][1].toFixed(2)+"</span><br/>");
-                                label.push("<span>close:&nbsp;"+param['data'][2].toFixed(2)+"</span><br/>");
-                                label.push("<span>high:&nbsp;"+param['data'][4].toFixed(2)+"</span><br/>");
-                                label.push("<span>low:&nbsp;"+param['data'][3].toFixed(2)+"</span><br/>");   
-                                label.push("<span>change:&nbsp;"+((param['data'][2]/param['data'][1]-1)*100).toFixed(2)+"</span><br/>");
-                                label.push("<span>range:&nbsp;"+((param['data'][4]/param['data'][3]-1)*100).toFixed(2)+"</span><br/>");   
+                                label.push("<span>open:&nbsp;"+param['value'][1].toFixed(2)+"</span><br/>");
+                                label.push("<span>close:&nbsp;"+param['value'][2].toFixed(2)+"</span><br/>");
+                                label.push("<span>high:&nbsp;"+param['value'][4].toFixed(2)+"</span><br/>");
+                                label.push("<span>low:&nbsp;"+param['value'][3].toFixed(2)+"</span><br/>");   
+                                label.push("<span>change:&nbsp;"+((param['value'][2]/param['value'][1]-1)*100).toFixed(2)+"</span><br/>");
+                                label.push("<span>range:&nbsp;"+((param['value'][4]/param['value'][3]-1)*100).toFixed(2)+"</span><br/>");   
                         }else if(typeof(param['value'])=='number'){
                             if (param['value']%1==0){
                                 label.push("<span>"+param['value'].toFixed(0)+"</span><br/>");
                             }else{
                                 label.push("<span>"+param['value'].toFixed(2)+"</span><br/>");
                             }
                         }else if(param['value']){
@@ -803,15 +812,15 @@
                 'height': 20
             }
         ],
         'series': [
             {
                 'name': title,
                 'type': 'candlestick',
-                'data': df[[open_field, close_field, low_field, high_field]].values.tolist(),
+                'data': bars,
             },
             {
                 'name': 'Volume',
                 'type': 'bar',
                 'xAxisIndex': 1,
                 'yAxisIndex': 1,
                 'data': bar_items
```

### Comparing `chartspy-2.0.9/chartspy/express/g2plot.py` & `chartspy-2.1.1/chartspy/express/g2plot.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/express/highcharts.py` & `chartspy-2.1.1/chartspy/express/highcharts.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/g2plot.py` & `chartspy-2.1.1/chartspy/g2plot.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/highcharts.py` & `chartspy-2.1.1/chartspy/highcharts.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/klinecharts.py` & `chartspy-2.1.1/chartspy/klinecharts.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy/tabulator.py` & `chartspy-2.1.1/chartspy/tabulator.py`

 * *Files identical despite different names*

### Comparing `chartspy-2.0.9/chartspy.egg-info/PKG-INFO` & `chartspy-2.1.1/chartspy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartspy
-Version: 2.0.9
+Version: 2.1.1
 Summary: echarts g2plot klinechart highcharts tabulator python wrapper
 Home-page: https://chartspy.icopy.site/
 Author: yiliuyan
 Author-email: yiliuyan161@126.com
 Maintainer: yiliuyan
 Maintainer-email: yiliuyan161@126.com
 Keywords: echarts g2plot klinechart highcharts tabulator python
```

### Comparing `chartspy-2.0.9/setup.py` & `chartspy-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def get_install_requires():
     requirement_file = os.path.join(THIS_FOLDER, "requirements.txt")
     return _parse_requirement_file(requirement_file)
 
 
 setup(
     name="chartspy",
-    version="2.0.9",
+    version="2.1.1",
     url="https://chartspy.icopy.site/",
     description="echarts g2plot klinechart highcharts tabulator python wrapper",
     keywords='echarts g2plot klinechart highcharts tabulator python ',
     packages=find_packages(exclude=("tests", "tests.*")),
     author="yiliuyan",
     author_email="yiliuyan161@126.com",
     maintainer="yiliuyan",
@@ -44,7 +44,8 @@
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ],
 )
+
```


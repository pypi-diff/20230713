# Comparing `tmp/imschrm-1.1.0b1.tar.gz` & `tmp/imschrm-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Z:\projects\imsc-hrm\imschrm-repo\dist\.tmp-wztb7eka\imschrm-1.1.0b1.tar", last modified: Thu Jun 22 15:52:51 2023, max compression
+gzip compressed data, was "Z:\projects\imsc-hrm\imschrm-repo\dist\.tmp-4ob2aoh1\imschrm-1.1.0b2.tar", last modified: Thu Jul 13 21:55:11 2023, max compression
```

## Comparing `imschrm-1.1.0b1.tar` & `imschrm-1.1.0b2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.843247 imschrm-1.1.0b1/
--rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.1.0b1/LICENSE.txt
--rw-rw-rw-   0        0        0     2981 2023-06-22 15:52:51.837227 imschrm-1.1.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     2068 2023-06-22 15:26:04.000000 imschrm-1.1.0b1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 15:52:51.846256 imschrm-1.1.0b1/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-06-22 15:24:41.000000 imschrm-1.1.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.126332 imschrm-1.1.0b1/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.132368 imschrm-1.1.0b1/src/main/
-drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.138361 imschrm-1.1.0b1/src/main/python/
-drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.659756 imschrm-1.1.0b1/src/main/python/imschrm/
--rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.1.0b1/src/main/python/imschrm/__init__.py
--rw-rw-rw-   0        0        0     3640 2021-07-22 05:14:45.000000 imschrm-1.1.0b1/src/main/python/imschrm/cli.py
--rw-rw-rw-   0        0        0   366016 2022-04-06 16:51:28.000000 imschrm-1.1.0b1/src/main/python/imschrm/codepoint_sets.py
--rw-rw-rw-   0        0        0     3394 2021-06-02 18:29:37.000000 imschrm-1.1.0b1/src/main/python/imschrm/doc_sequence.py
--rw-rw-rw-   0        0        0    11595 2023-06-22 15:09:58.000000 imschrm-1.1.0b1/src/main/python/imschrm/hrm.py
-drwxrwxrwx   0        0        0        0 2023-06-22 15:52:51.417122 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/
--rw-rw-rw-   0        0        0     2981 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 15:52:51.000000 imschrm-1.1.0b1/src/main/python/imschrm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.118954 imschrm-1.1.0b2/
+-rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.1.0b2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2981 2023-07-13 21:55:12.583696 imschrm-1.1.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     2068 2023-06-22 15:26:04.000000 imschrm-1.1.0b2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 21:55:12.589709 imschrm-1.1.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-07-13 21:54:13.000000 imschrm-1.1.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.043732 imschrm-1.1.0b2/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.049764 imschrm-1.1.0b2/src/main/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.053793 imschrm-1.1.0b2/src/main/python/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.351091 imschrm-1.1.0b2/src/main/python/imschrm/
+-rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.1.0b2/src/main/python/imschrm/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-07-13 17:28:11.000000 imschrm-1.1.0b2/src/main/python/imschrm/cli.py
+-rw-rw-rw-   0        0        0   366016 2022-04-06 16:51:28.000000 imschrm-1.1.0b2/src/main/python/imschrm/codepoint_sets.py
+-rw-rw-rw-   0        0        0     3394 2021-06-02 18:29:37.000000 imschrm-1.1.0b2/src/main/python/imschrm/doc_sequence.py
+-rw-rw-rw-   0        0        0    12174 2023-07-13 17:28:31.000000 imschrm-1.1.0b2/src/main/python/imschrm/hrm.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.222209 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-07-13 21:55:12.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/top_level.txt
```

### Comparing `imschrm-1.1.0b1/LICENSE.txt` & `imschrm-1.1.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b1/PKG-INFO` & `imschrm-1.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imschrm
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Validates IMSC documents against the IMSC HRM
 Home-page: https://www.sandflow.com
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/imscHRM/issues
 Project-URL: Source, https://github.com/sandflow/imscHRM
 Keywords: ttml,imsc,smpte-tt,hrm,complexity
```

### Comparing `imschrm-1.1.0b1/README.md` & `imschrm-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b1/setup.py` & `imschrm-1.1.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setup(
   name='imschrm', 
-  version='1.1.0b1',
+  version='1.1.0b2',
   description='Validates IMSC documents against the IMSC HRM',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Sandflow Consulting LLC',
   author_email='info@sandflow.com',
   url='https://www.sandflow.com',
   project_urls={
```

### Comparing `imschrm-1.1.0b1/src/main/python/imschrm/cli.py` & `imschrm-1.1.0b2/src/main/python/imschrm/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
   if args.verbose:
     logging.basicConfig(level=logging.DEBUG)
   else:
     logging.basicConfig(level=logging.WARNING)
 
 
-  imschrm.hrm.validate(imschrm.doc_sequence.iter_isd(doc_sequence), ev)
+  imschrm.hrm.validate(imschrm.doc_sequence.iter_isd(doc_sequence), ev, 0)
 
   if ev.failed:
     print("Validation failed")
     sys.exit(1)
 
 if __name__ == "__main__":
   main()
```

### Comparing `imschrm-1.1.0b1/src/main/python/imschrm/codepoint_sets.py` & `imschrm-1.1.0b2/src/main/python/imschrm/codepoint_sets.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b1/src/main/python/imschrm/doc_sequence.py` & `imschrm-1.1.0b2/src/main/python/imschrm/doc_sequence.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b1/src/main/python/imschrm/hrm.py` & `imschrm-1.1.0b2/src/main/python/imschrm/hrm.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,22 +65,29 @@
   is_empty: bool = False # Does the ISD contain any content
 
 
 class EventHandler:
   '''Allows a callee to inform the caller of events that occur during processing. Typically
   overridden by the caller.
   '''
-  
+
   @staticmethod
   def _format_message(msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
-    return (
-      f"{msg} at {float(time_offset):.3f}s (doc #{doc_index})\n"
-      f"  available time: {float(available_time):.3f}s | HRM time: {float(stats.dur):.3f}\n"
-      f"  Glyph copy count: {stats.gcpy_count} | render count: {stats.gren_count} | Background draw count: {stats.nbg_total} | Clear: {stats.clear}\n"
-    )
+    if stats.is_empty:
+      return (
+        f"{msg} at {float(time_offset):.3f}s (doc #{doc_index})\n"
+        f"  available time: {float(available_time):.3f}s | HRM time: 0 (Empty ISD)\n"
+      )
+    else:
+      return (
+        f"{msg} at {float(time_offset):.3f}s (doc #{doc_index})\n"
+        f"  available time: {float(available_time):.3f}s | HRM time: {float(stats.dur):.3f}\n"
+        f"  ngra_t: {float(stats.ngra_t):.3f}\n"
+        f"  Glyph copy count: {stats.gcpy_count} | render count: {stats.gren_count} | Background draw count: {stats.nbg_total} | Clear: {stats.clear}\n"
+      )
 
 
   def info(self, msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
     LOGGER.info(EventHandler._format_message(msg, doc_index, time_offset, available_time, stats))
 
   def warn(self, msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
     LOGGER.warning(EventHandler._format_message(msg, doc_index, time_offset, available_time, stats))
@@ -88,15 +95,15 @@
   def error(self, msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
     LOGGER.error(EventHandler._format_message(msg, doc_index, time_offset, available_time, stats))
 
   def debug(self, msg: str, doc_index: int, time_offset: Fraction, available_time: Fraction, stats: ISDStatistics):
     LOGGER.debug(EventHandler._format_message(msg, doc_index, time_offset, available_time, stats))
 
 
-def validate(isd_iterator: typing.Iterator[typing.Tuple[Fraction, ttconv.isd.ISD]], event_handler: typing.Type[EventHandler]=EventHandler()):
+def validate(isd_iterator: typing.Iterator[typing.Tuple[Fraction, ttconv.isd.ISD]], event_handler: typing.Type[EventHandler]=EventHandler(), tolerance: float=0):
   '''Determines whether the sequence of ISDs returned by `isd_iterator` conform to the IMSC HRM.
   `isd_iterator` returns a sequence of tuplets `(begin, ISD)`, where `ISD` is an ISD instance whose
   active interval starts at `begin` seconds and ends immediately before the `begin` value of the next 
   ISD. Errors, warnings and info messages are signalled through callbacks on the `event_handler`.
   '''
 
   hrm = HRM()
@@ -111,18 +118,18 @@
     stats = hrm.next_isd(isd)
 
     avail_render_time = min(_IPD, time_offset - last_render_time)
 
     event_handler.debug("Processed document", doc_index, time_offset, avail_render_time, stats)
 
     if not stats.is_empty:
-      if stats.dur > avail_render_time:
+      if stats.dur - avail_render_time > tolerance:
         event_handler.error("Rendering time exceeded", doc_index, time_offset, avail_render_time, stats)
 
-      if stats.ngra_t > _NGBS:
+      if stats.ngra_t - _NGBS > tolerance:
         event_handler.error("NGBS exceeded", doc_index, time_offset, avail_render_time, stats)
 
       last_render_time = time_offset
 
 
 @dataclass(frozen=True)
 class _Glyph:
@@ -146,19 +153,31 @@
   def next_isd(
     self,
     isd: typing.Type[ttconv.isd.ISD]
     ) -> ISDStatistics:
 
     self.isd_stats = ISDStatistics()
 
-    self._compute_dur_t(isd)
+    self.isd_stats.is_empty = True
+
+    if isd is not None:
+      for region in isd.iter_regions():
+
+        if not _is_presented_region(region):
+          continue
+
+        self.isd_stats.is_empty = False
+
+    if not self.isd_stats.is_empty:
+
+      self._compute_dur_t(isd)
 
-    self._compute_dur_d(isd)
+      self._compute_dur_d(isd)
 
-    self.isd_stats.dur = self.isd_stats.dur_t + self.isd_stats.dur_d
+      self.isd_stats.dur = self.isd_stats.dur_t + self.isd_stats.dur_d
 
     return self.isd_stats
 
   def _compute_dur_d(
     self,
     isd: typing.Type[ttconv.isd.ISD]
     ):
```

### Comparing `imschrm-1.1.0b1/src/main/python/imschrm.egg-info/PKG-INFO` & `imschrm-1.1.0b2/src/main/python/imschrm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imschrm
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Validates IMSC documents against the IMSC HRM
 Home-page: https://www.sandflow.com
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/imscHRM/issues
 Project-URL: Source, https://github.com/sandflow/imscHRM
 Keywords: ttml,imsc,smpte-tt,hrm,complexity
```

### Comparing `imschrm-1.1.0b1/src/main/python/imschrm.egg-info/SOURCES.txt` & `imschrm-1.1.0b2/src/main/python/imschrm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


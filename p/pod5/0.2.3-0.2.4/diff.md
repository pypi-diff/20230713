# Comparing `tmp/pod5-0.2.3.tar.gz` & `tmp/pod5-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pod5-0.2.3.tar", last modified: Wed Jun 28 15:57:45 2023, max compression
+gzip compressed data, was "pod5-0.2.4.tar", last modified: Thu Jul 13 13:15:56 2023, max compression
```

## Comparing `pod5-0.2.3.tar` & `pod5-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.433904 pod5-0.2.3/
--rw-r--r--   0 root         (0) root         (0)    19530 2023-06-28 15:57:45.433904 pod5-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    18873 2023-06-26 10:25:34.000000 pod5-0.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-28 15:57:36.000000 pod5-0.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 15:57:45.433904 pod5-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-06-26 10:25:34.000000 pod5-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.369899 pod5-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.373899 pod5-0.2.3/src/pod5/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-28 15:57:24.000000 pod5-0.2.3/src/pod5/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/api_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13092 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/pod5_types.py
--rw-rw-rw-   0 root         (0) root         (0)    36471 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     7675 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/repack.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/signal_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.429904 pod5-0.2.3/src/pod5/tools/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/main.py
--rw-rw-rw-   0 root         (0) root         (0)    20644 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)    27286 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_convert_from_fast5.py
--rw-rw-rw-   0 root         (0) root         (0)    10005 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_convert_to_fast5.py
--rw-rw-rw-   0 root         (0) root         (0)     4779 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     6822 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_recover.py
--rw-rw-rw-   0 root         (0) root         (0)     2723 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_repack.py
--rw-rw-rw-   0 root         (0) root         (0)    18541 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_subset.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_update.py
--rw-rw-rw-   0 root         (0) root         (0)    16686 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_view.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/polars_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6105 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12952 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.377899 pod5-0.2.3/src/pod5.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19530 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:15:56.167003 pod5-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)    19530 2023-07-13 13:15:56.167003 pod5-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    18873 2023-07-13 13:15:38.000000 pod5-0.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-07-13 13:15:46.000000 pod5-0.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 13:15:56.167003 pod5-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-07-13 13:15:38.000000 pod5-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:15:56.163003 pod5-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:15:56.163003 pod5-0.2.4/src/pod5/
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-13 13:15:26.000000 pod5-0.2.4/src/pod5/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/api_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13092 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/pod5_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    36471 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6212 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/repack.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/signal_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:15:56.167003 pod5-0.2.4/src/pod5/tools/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    20644 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)    27286 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_convert_from_fast5.py
+-rw-rw-rw-   0 root         (0) root         (0)    10005 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_convert_to_fast5.py
+-rw-rw-rw-   0 root         (0) root         (0)     4767 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6822 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     3400 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     3304 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_recover.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_repack.py
+-rw-rw-rw-   0 root         (0) root         (0)    18562 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_update.py
+-rw-rw-rw-   0 root         (0) root         (0)    16686 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/pod5_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/polars_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6105 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/tools/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12952 2023-07-13 13:15:38.000000 pod5-0.2.4/src/pod5/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:15:56.163003 pod5-0.2.4/src/pod5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19530 2023-07-13 13:15:56.000000 pod5-0.2.4/src/pod5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2023-07-13 13:15:56.000000 pod5-0.2.4/src/pod5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 13:15:56.000000 pod5-0.2.4/src/pod5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-13 13:15:56.000000 pod5-0.2.4/src/pod5.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      318 2023-07-13 13:15:56.000000 pod5-0.2.4/src/pod5.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-13 13:15:56.000000 pod5-0.2.4/src/pod5.egg-info/top_level.txt
```

### Comparing `pod5-0.2.3/PKG-INFO` & `pod5-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pod5
-Version: 0.2.3
+Version: 0.2.4
 Summary: Oxford Nanopore Technologies Pod5 File Format Python API and Tools
 Author-email: Oxford Nanopore Technologies plc <support@nanoporetech.com>
 Keywords: nanopore
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pod5-0.2.3/README.md` & `pod5-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/pyproject.toml` & `pod5-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 
 
 [project]
 name = "pod5"
 authors = [{name="Oxford Nanopore Technologies plc", email="support@nanoporetech.com"}]
 readme = "README.md"
 requires-python = "~= 3.7"
-dynamic = ["version"]
 description="Oxford Nanopore Technologies Pod5 File Format Python API and Tools"
-
+dynamic = ["version"]
 keywords = ['nanopore']
-
 classifiers=[
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 
 dependencies = [
-    'lib_pod5 == 0.2.3',
+    'lib_pod5 == 0.2.4',
     "iso8601",
     'importlib-metadata; python_version<"3.8"',
     "more_itertools",
-    "numpy >= 1.20.0",
+    "numpy >= 1.21.0",
+    'typing-extensions; python_version<"3.8"',
     "pyarrow ~= 11.0.0",
     "pytz",
     "packaging",
     "polars~=0.17.12",
     "h5py~=3.8.0",
     "vbz_h5py_plugin",
     "tqdm"
```

### Comparing `pod5-0.2.3/src/pod5/__init__.py` & `pod5-0.2.4/src/pod5/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,7 +33,30 @@
 from .signal_tools import (
     vbz_compress_signal,
     vbz_decompress_signal,
     vbz_decompress_signal_chunked,
     vbz_decompress_signal_into,
 )
 from .writer import Writer
+
+__all__ = (
+    "__version__",
+    "format_read_id_to_str",
+    "format_read_ids",
+    "load_read_id_iterable",
+    "pack_read_ids",
+    "Calibration",
+    "CompressedRead",
+    "EndReason",
+    "EndReasonEnum",
+    "Pore",
+    "Read",
+    "RunInfo",
+    "Reader",
+    "ReadRecord",
+    "ReadRecordBatch",
+    "vbz_compress_signal",
+    "vbz_decompress_signal",
+    "vbz_decompress_signal_chunked",
+    "vbz_decompress_signal_into",
+    "Writer",
+)
```

### Comparing `pod5-0.2.3/src/pod5/api_utils.py` & `pod5-0.2.4/src/pod5/api_utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/pod5_types.py` & `pod5-0.2.4/src/pod5/pod5_types.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/reader.py` & `pod5-0.2.4/src/pod5/reader.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/repack.py` & `pod5-0.2.4/src/pod5/repack.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 """
 Tools to assist repacking pod5 data into other pod5 files
 """
-import time
-from typing import Collection, Generator, Optional
-from venv import logger
+from typing import Collection, Generator
+import warnings
 
 import lib_pod5 as p5b
 
 import pod5 as p5
-from pod5.tools.utils import PBAR_DEFAULTS, logged_all
-from tqdm.auto import tqdm
-
-# The default interval in seconds to check for completion
-DEFAULT_INTERVAL = 0.5
+from pod5.tools.utils import logged_all
 
 
 class Repacker:
     """Wrapper class around native pod5 tools to repack data"""
 
     def __init__(self):
         self._repacker = p5b.Repacker()
         self._reads_requested = 0
 
     @property
     def is_complete(self) -> bool:
         """Find if the requested repack operations are complete"""
-        # is_complete can be initialised to true before work starts
-        # this gives a short time to allow the value to be set
-        if self._repacker.is_complete:
-            for _ in range(100):
-                time.sleep(0.02)
-                if not self._repacker.is_complete:
-                    break
-
         return self._repacker.is_complete
 
     @property
     def reads_sample_bytes_completed(self) -> int:
         """Find the number of bytes for sample data repacked"""
         return self._repacker.reads_sample_bytes_completed
 
@@ -123,14 +110,15 @@
             )
 
         self._reads_requested += successful_finds
         self._repacker.add_selected_reads_to_output(
             output_ref, reader.inner_file_reader, per_batch_counts, all_batch_rows
         )
 
+    @logged_all
     def add_all_reads_to_output(
         self, output_ref: p5b.Pod5RepackerOutput, reader: p5.Reader
     ) -> None:
         """
         Copy the every read from the given :py:class:`Reader` into the
         Repacker output reference which was returned by :py:meth:`add_output`
 
@@ -141,98 +129,65 @@
         reader : :py:class:`Reader`
             The Pod5 file reader to copy reads from
         """
         self._reads_requested += reader.num_reads
         self._repacker.add_all_reads_to_output(output_ref, reader.inner_file_reader)
 
     @logged_all
-    def wait(
-        self,
-        finish: bool = True,
-        interval: float = DEFAULT_INTERVAL,
-        desc: str = "",
-        total_reads: Optional[int] = None,
-        offset: int = 0,
-    ) -> int:
-        """
-        Wait for the repacker (blocking) until it is done checking every `interval`
-        seconds. Shows a progress bar at the current process index with desc string
-        as the description.
+    def wait(self, finish: bool = True, **kwargs) -> int:
+        """
+        Wait for the repacker (blocking) until it is done. Returning the number of reads
+        completed.
 
         Parameters
         ----------
         finish : bool
             Flag to toggle an optional final call to :py:meth:`finish` to
             close the repacker and free resources
-        interval : float
-            The interval (in seconds) between checks to :py:meth:`is_complete`
-        desc : str
-            Progressbar description string
-        total_reads : int
-            Overwrites the total number of reads expected
-        offset : int
-            Sets the progress bar position offset
 
         Returns
         -------
         num_reads_completed: int
             The number of reads written
         """
-        logger.info(f"pos: {offset}")
-
-        if total_reads is not None:
-            total = total_reads
-        else:
-            total = self.reads_requested
-
-        pbar = tqdm(
-            total=total,
-            desc=desc,
-            leave=False,
-            unit="Read",
-            position=offset,
-            **PBAR_DEFAULTS,
-        )
+        if kwargs:
+            warnings.warn(
+                f"pod5.repack.Repacker.wait: {kwargs.keys()} parameters are "
+                "deprecated and have no effect",
+                FutureWarning,
+            )
 
-        last_reads = 0
         while not self.is_complete:
-            time.sleep(interval)
-
-            # Update pbar - total / reads_requested might change if user adds more
-            if total_reads is None:
-                pbar.total = self.reads_requested
-            pbar.update(self.reads_completed - last_reads)
-            last_reads = self.reads_completed
+            continue
 
         if finish:
             self.finish()
 
-        return last_reads
+        return self.reads_completed
 
-    def waiter(
-        self,
-        interval: float = DEFAULT_INTERVAL,
-    ) -> Generator[int, None, None]:
+    @logged_all
+    def waiter(self, **kwargs) -> Generator[int, None, None]:
         """
-        Wait for the repacker (blocking) until it is done checking every `interval`
-        seconds. Yields number of reads completed .
-
-        Parameters
-        ----------
-        interval : float
-            The interval (in seconds) between checks to :py:meth:`is_complete`
+        Generate number of reads completed while waiting for the repacker to return
+        `is_complete==True`.
 
         Returns
         -------
-        num_reads_completed: int
-            The number of reads written
+        reads_completed: int
+            The number of reads completed
         """
-        # Sleep to ensure `is_complete` state correctly set
+        if kwargs:
+            warnings.warn(
+                f"pod5.repack.Repacker.waiter: {kwargs.keys()} parameters are "
+                "deprecated and have no effect",
+                FutureWarning,
+            )
+
         while not self.is_complete:
             yield self.reads_completed
-            time.sleep(interval)
 
     def finish(self) -> None:
         """
-        Call finish on the underlying c_api repacker instance to free resources
+        Call finish on the underlying c_api repacker instance to write the footer
+        completing the file and freeing resources
         """
         return self._repacker.finish()
```

### Comparing `pod5-0.2.3/src/pod5/signal_tools.py` & `pod5-0.2.4/src/pod5/signal_tools.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/main.py` & `pod5-0.2.4/src/pod5/tools/main.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/parsers.py` & `pod5-0.2.4/src/pod5/tools/parsers.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_convert_from_fast5.py` & `pod5-0.2.4/src/pod5/tools/pod5_convert_from_fast5.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_convert_to_fast5.py` & `pod5-0.2.4/src/pod5/tools/pod5_convert_to_fast5.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_filter.py` & `pod5-0.2.4/src/pod5/tools/pod5_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
             if len(read_ids) == 0:
                 logger.debug(f"Skipping: {src}")
                 continue
 
             with p5.Reader(src) as reader:
                 repacker.add_selected_reads_to_output(output, reader, read_ids)
-                for n_written in repacker.waiter(interval=0.1):
+                for n_written in repacker.waiter():
                     pbar.update(n_written - prev)
                     prev = n_written
 
         pbar.update(total_reads - prev)
         pbar.close()
         # Finish the pod5 file and close source handles
         repacker.finish()
```

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_inspect.py` & `pod5-0.2.4/src/pod5/tools/pod5_inspect.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_merge.py` & `pod5-0.2.4/src/pod5/tools/pod5_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             with p5.Reader(path) as reader:
                 pbar2 = tqdm(
                     total=reader.num_reads,
                     desc=reader.path.name,
                     unit="Reads",
                     leave=False,
                     position=1,
+                    delay=10,
                     **PBAR_DEFAULTS,
                 )
 
                 repacker.add_all_reads_to_output(repacker_output, reader)
                 for n_written in repacker.waiter():
                     pbar2.update(n_written - prev)
                     prev = n_written
```

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_recover.py` & `pod5-0.2.4/src/pod5/tools/pod5_recover.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_repack.py` & `pod5-0.2.4/src/pod5/tools/pod5_repack.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_subset.py` & `pod5-0.2.4/src/pod5/tools/pod5_subset.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,15 @@
 
         pbar = tqdm(
             total=total_reads,
             desc=dest.name,
             unit="Reads",
             leave=False,
             position=process,
+            delay=2,
             **PBAR_DEFAULTS,
         )
 
         prev = 0
         # Copy selected reads from one file at a time
         for source, reads in sources.groupby(PL_SRC_FNAME):
             with p5.Reader(Path(source)) as reader:
```

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_update.py` & `pod5-0.2.4/src/pod5/tools/pod5_update.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/pod5_view.py` & `pod5-0.2.4/src/pod5/tools/pod5_view.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/polars_utils.py` & `pod5-0.2.4/src/pod5/tools/polars_utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/tools/utils.py` & `pod5-0.2.4/src/pod5/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5/writer.py` & `pod5-0.2.4/src/pod5/writer.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.3/src/pod5.egg-info/PKG-INFO` & `pod5-0.2.4/src/pod5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pod5
-Version: 0.2.3
+Version: 0.2.4
 Summary: Oxford Nanopore Technologies Pod5 File Format Python API and Tools
 Author-email: Oxford Nanopore Technologies plc <support@nanoporetech.com>
 Keywords: nanopore
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pod5-0.2.3/src/pod5.egg-info/SOURCES.txt` & `pod5-0.2.4/src/pod5.egg-info/SOURCES.txt`

 * *Files identical despite different names*


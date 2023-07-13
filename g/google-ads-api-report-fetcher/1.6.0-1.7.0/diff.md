# Comparing `tmp/google-ads-api-report-fetcher-1.6.0.tar.gz` & `tmp/google-ads-api-report-fetcher-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ads-api-report-fetcher-1.6.0.tar", last modified: Thu Jun  8 13:13:24 2023, max compression
+gzip compressed data, was "google-ads-api-report-fetcher-1.7.0.tar", last modified: Thu Jul 13 06:28:54 2023, max compression
```

## Comparing `google-ads-api-report-fetcher-1.6.0.tar` & `google-ads-api-report-fetcher-1.7.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.6.0/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.347265 google-ads-api-report-fetcher-1.6.0/gaarf/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.6.0/gaarf/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-04-13 10:50:21.000000 google-ads-api-report-fetcher-1.6.0/gaarf/api_clients.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.6.0/gaarf/base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2717 2023-06-06 14:22:27.000000 google-ads-api-report-fetcher-1.6.0/gaarf/bq_executor.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/gaarf/cli/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3188 2023-06-07 14:43:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/bq.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7494 2023-06-07 14:43:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/gaarf.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4210 2023-06-07 13:55:49.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/postprocessor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3586 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/simulator.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3099 2023-06-07 14:43:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/sql.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    13434 2023-06-07 14:43:52.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/utils.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/gaarf/io/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/formatter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9991 2023-03-16 19:54:17.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/writer.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10596 2023-05-29 10:48:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9680 2023-03-10 13:35:15.000000 google-ads-api-report-fetcher-1.6.0/gaarf/query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11597 2023-06-07 20:34:00.000000 google-ads-api-report-fetcher-1.6.0/gaarf/query_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2399 2023-06-06 14:27:05.000000 google-ads-api-report-fetcher-1.6.0/gaarf/query_post_processor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5655 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.6.0/gaarf/report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-03-06 16:43:36.000000 google-ads-api-report-fetcher-1.6.0/gaarf/simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1275 2023-06-07 14:38:11.000000 google-ads-api-report-fetcher-1.6.0/gaarf/sql_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.6.0/gaarf/utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.6.0/gaarf/wip.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1169 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      214 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1723 2023-06-07 14:40:20.000000 google-ads-api-report-fetcher-1.6.0/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      423 2023-06-06 14:22:27.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_bq_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10945 2023-04-07 06:54:54.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_cli_utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7168 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3890 2023-02-24 15:33:44.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3982 2023-06-08 13:13:05.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_query_post_processor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6927 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3882 2023-06-06 14:23:09.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_writer.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:28:54.693833 google-ads-api-report-fetcher-1.7.0/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-07-13 06:28:54.693833 google-ads-api-report-fetcher-1.7.0/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.7.0/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:28:54.689833 google-ads-api-report-fetcher-1.7.0/gaarf/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.7.0/gaarf/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-07-13 06:28:11.000000 google-ads-api-report-fetcher-1.7.0/gaarf/api_clients.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.7.0/gaarf/base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2717 2023-07-07 14:27:09.000000 google-ads-api-report-fetcher-1.7.0/gaarf/bq_executor.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:28:54.689833 google-ads-api-report-fetcher-1.7.0/gaarf/cli/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.7.0/gaarf/cli/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3959 2023-06-19 15:45:10.000000 google-ads-api-report-fetcher-1.7.0/gaarf/cli/bq.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7649 2023-07-13 06:28:11.000000 google-ads-api-report-fetcher-1.7.0/gaarf/cli/gaarf.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4210 2023-06-07 13:55:49.000000 google-ads-api-report-fetcher-1.7.0/gaarf/cli/postprocessor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2967 2023-07-13 06:28:11.000000 google-ads-api-report-fetcher-1.7.0/gaarf/cli/simulator.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3859 2023-06-19 15:45:10.000000 google-ads-api-report-fetcher-1.7.0/gaarf/cli/sql.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    13434 2023-06-21 17:43:19.000000 google-ads-api-report-fetcher-1.7.0/gaarf/cli/utils.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:28:54.693833 google-ads-api-report-fetcher-1.7.0/gaarf/io/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.7.0/gaarf/io/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.7.0/gaarf/io/formatter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.7.0/gaarf/io/reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10370 2023-07-13 06:28:11.000000 google-ads-api-report-fetcher-1.7.0/gaarf/io/writer.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10596 2023-05-29 10:48:19.000000 google-ads-api-report-fetcher-1.7.0/gaarf/parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11869 2023-07-07 09:02:33.000000 google-ads-api-report-fetcher-1.7.0/gaarf/query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11681 2023-07-12 20:43:36.000000 google-ads-api-report-fetcher-1.7.0/gaarf/query_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2642 2023-07-13 06:28:11.000000 google-ads-api-report-fetcher-1.7.0/gaarf/query_post_processor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5774 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.7.0/gaarf/report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-06-16 18:39:22.000000 google-ads-api-report-fetcher-1.7.0/gaarf/simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1275 2023-06-07 14:38:11.000000 google-ads-api-report-fetcher-1.7.0/gaarf/sql_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-07-12 20:43:36.000000 google-ads-api-report-fetcher-1.7.0/gaarf/utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.7.0/gaarf/wip.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:28:54.693833 google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-07-13 06:28:54.000000 google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1169 2023-07-13 06:28:54.000000 google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-07-13 06:28:54.000000 google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      214 2023-07-13 06:28:54.000000 google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-07-13 06:28:54.000000 google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-07-13 06:28:54.000000 google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-07-13 06:28:54.693833 google-ads-api-report-fetcher-1.7.0/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1723 2023-07-13 06:28:22.000000 google-ads-api-report-fetcher-1.7.0/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:28:54.693833 google-ads-api-report-fetcher-1.7.0/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.7.0/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:28:54.693833 google-ads-api-report-fetcher-1.7.0/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      423 2023-06-06 14:22:27.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_bq_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11446 2023-06-21 17:43:19.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_cli_utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7233 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4835 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4771 2023-06-16 12:21:00.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_query_post_processor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7620 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3784 2023-07-13 06:28:11.000000 google-ads-api-report-fetcher-1.7.0/tests/unit/test_writer.py
```

### Comparing `google-ads-api-report-fetcher-1.6.0/PKG-INFO` & `google-ads-api-report-fetcher-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.6.0
+Version: 1.7.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `google-ads-api-report-fetcher-1.6.0/README.md` & `google-ads-api-report-fetcher-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/api_clients.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/api_clients.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/base_query.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/bq_executor.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/bq_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/cli/bq.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/cli/bq.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 from concurrent import futures
+import functools
 
 from gaarf.io import reader  # type: ignore
 from gaarf.bq_executor import BigQueryExecutor
 from .utils import (GaarfBqConfigBuilder, ConfigSaver,
                     initialize_runtime_parameters, postprocessor_runner,
                     init_logging)
 
@@ -38,16 +39,23 @@
                         action="store_false")
     parser.add_argument("--config-destination",
                         dest="save_config_dest",
                         default="config.yaml")
     parser.add_argument("--log", "--loglevel", dest="loglevel", default="info")
     parser.add_argument("--logger", dest="logger", default="local")
     parser.add_argument("--dry-run", dest="dry_run", action="store_true")
+    parser.add_argument("--parallel-queries",
+                        dest="parallel_queries",
+                        action="store_true")
+    parser.add_argument("--no-parallel-queries",
+                        dest="parallel_queries",
+                        action="store_false")
     parser.set_defaults(save_config=False)
     parser.set_defaults(dry_run=False)
+    parser.set_defaults(parallel_queries=True)
     args = parser.parse_known_args()
     main_args = args[0]
 
     logger = init_logging(loglevel=main_args.loglevel.upper(),
                           logger_type=main_args.logger)
     config = GaarfBqConfigBuilder(args).build()
     logger.debug("config: %s", config)
@@ -61,20 +69,28 @@
 
     bq_executor = BigQueryExecutor(project_id=config.project,
                                    location=config.dataset_location)
     bq_executor.create_datasets(config.params.get("macro"))
 
     reader_client = reader.FileReader()
 
-    with futures.ThreadPoolExecutor() as executor:
-        future_to_query = {
-            executor.submit(bq_executor.execute, query,
-                            reader_client.read(query), config.params): query
-            for query in main_args.query
-        }
-        for future in futures.as_completed(future_to_query):
-            query = future_to_query[future]
-            postprocessor_runner(query, future.result, logger)
+    if main_args.parallel_queries:
+        logger.info("Running queries in parallel")
+        with futures.ThreadPoolExecutor() as executor:
+            future_to_query = {
+                executor.submit(bq_executor.execute, query,
+                                reader_client.read(query), config.params): query
+                for query in sorted(main_args.query)
+            }
+            for future in futures.as_completed(future_to_query):
+                query = future_to_query[future]
+                postprocessor_runner(query, future.result, logger)
+    else:
+        logger.info("Running queries sequentially")
+        for query in sorted(main_args.query):
+            callback = functools.partial(bq_executor.execute, query,
+                reader_client.read(query), config.params)
+            postprocessor_runner(query, callback, logger)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/cli/gaarf.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/cli/gaarf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys
+import argparse
 from collections.abc import MutableSequence
 from concurrent import futures
-import argparse
-from pathlib import Path
+import functools
 import logging
+from pathlib import Path
+import sys
 from rich.logging import RichHandler
 from smart_open import open
 import yaml
 
 from gaarf import api_clients, utils, query_executor
 from gaarf.io import writer, reader  # type: ignore
 from .utils import (GaarfConfigBuilder, ConfigSaver,
@@ -156,18 +157,19 @@
                 }
                 for future in futures.as_completed(future_to_query):
                     query = future_to_query[future]
                     gaarf_runner(query, future.result, logger)
         else:
             logger.info("Running queries sequentially")
             for query in main_args.query:
-                callback = ads_query_executor.execute(
-                    reader_client.read(query), query, customer_ids,
-                    writer_client, config.params,
-                    main_args._optimize_performance)
+                callback = functools.partial(ads_query_executor.execute,
+                                             reader_client.read(query), query,
+                                             customer_ids, writer_client,
+                                             config.params,
+                                             main_args._optimize_performance)
                 gaarf_runner(query, callback, logger)
     else:
         logger.warning(
             "Not a single under MCC %s is found that satisfies the following customer_id query: '%s'",
             config.account, customer_ids_query)
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/cli/postprocessor.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/cli/postprocessor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/cli/sql.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/cli/sql.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 from concurrent import futures
+import functools
 import sqlalchemy
 
 from gaarf.io import reader  # type: ignore
 from gaarf.sql_executor import SqlAlchemyQueryExecutor
 from .utils import (GaarfSqlConfigBuilder, ConfigSaver,
                     initialize_runtime_parameters, postprocessor_runner,
                     init_logging)
@@ -38,16 +39,23 @@
                         action="store_false")
     parser.add_argument("--config-destination",
                         dest="save_config_dest",
                         default="config.yaml")
     parser.add_argument("--log", "--loglevel", dest="loglevel", default="info")
     parser.add_argument("--logger", dest="logger", default="local")
     parser.add_argument("--dry-run", dest="dry_run", action="store_true")
+    parser.add_argument("--parallel-queries",
+                        dest="parallel_queries",
+                        action="store_true")
+    parser.add_argument("--no-parallel-queries",
+                        dest="parallel_queries",
+                        action="store_false")
     parser.set_defaults(save_config=False)
     parser.set_defaults(dry_run=False)
+    parser.set_defaults(parallel_queries=True)
     args = parser.parse_known_args()
     main_args = args[0]
 
     logger = init_logging(loglevel=main_args.loglevel.upper(),
                           logger_type=main_args.logger)
 
     config = GaarfSqlConfigBuilder(args).build()
@@ -61,21 +69,28 @@
     logger.debug("initialized config: %s", config)
 
     engine = sqlalchemy.create_engine(config.connection_string)
     sql_executor = SqlAlchemyQueryExecutor(engine)
 
     reader_client = reader.FileReader()
 
-    with futures.ThreadPoolExecutor() as executor:
-        future_to_query = {
-            executor.submit(sql_executor.execute, query,
-                            reader_client.read(query), config.params):
-            query
-            for query in main_args.query
-        }
-        for future in futures.as_completed(future_to_query):
-            query = future_to_query[future]
-            postprocessor_runner(query, future.result, logger)
+    if main_args.parallel_queries:
+        logger.info("Running queries in parallel")
+        with futures.ThreadPoolExecutor() as executor:
+            future_to_query = {
+                executor.submit(sql_executor.execute, query,
+                                reader_client.read(query), config.params): query
+                for query in sorted(main_args.query)
+            }
+            for future in futures.as_completed(future_to_query):
+                query = future_to_query[future]
+                postprocessor_runner(query, future.result, logger)
+    else:
+        logger.info("Running queries sequentially")
+        for query in sorted(main_args.query):
+            callback = functools.partial(sql_executor.execute, query,
+                reader_client.read(query), config.params)
+            postprocessor_runner(query, callback, logger)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/cli/utils.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from smart_open import open
 from dateutil.relativedelta import relativedelta
 import yaml
 from google.ads.googleads.errors import GoogleAdsException  # type: ignore
 import traceback
 
 from gaarf.io.writer import ZeroRowException
+from gaarf.query_editor import CommonParametersMixin
 
 
 @dataclass
 class GaarfConfig:
     output: str
     api_version: str
     account: str
@@ -175,17 +176,15 @@
         params = ParamsParser(["macro", "sql", "template"]).parse(query_args)
         return GaarfSqlConfig(
             connection_string=main_args.connection_string.format(
                 **dict(os.environ.items())),
             params=params)
 
 
-class ParamsParser:
-
-    common_params = {"date_iso": datetime.date.today().strftime("%Y%m%d")}
+class ParamsParser(CommonParametersMixin):
 
     def __init__(self, identifiers: Sequence[str]):
         self.identifiers = identifiers
 
     def parse(self,
               params: Sequence[Any]) -> Dict[str, Optional[Dict[str, Any]]]:
         return {
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/io/formatter.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/io/formatter.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/io/reader.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/io/reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/io/writer.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/io/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.import csv
+# limitations under the License.
 
-from typing import Any, Dict, Sequence, Tuple
+from typing import Any, Dict, List, Sequence, Tuple
 import logging
 import abc
 import os
 import proto  # type: ignore
 from google.cloud import bigquery  # type: ignore
 from google.cloud.exceptions import NotFound  # type: ignore
 from pathlib import Path
@@ -102,31 +102,34 @@
 class BigQueryWriter(AbsWriter):
 
     def __init__(self,
                  project: str,
                  dataset: str,
                  location: str = "US",
                  **kwargs):
-        self.client = bigquery.Client(project)
+        self.project = project
         self.dataset_id = f"{project}.{dataset}"
         self.location = location
+        self.client = None
 
     def __str__(self):
         return f"[BigQuery] - {self.dataset_id} at {self.location} location."
 
     def create_or_get_dataset(self):
+        self._init_client()
         try:
             bq_dataset = self.client.get_dataset(self.dataset_id)
         except NotFound:
             bq_dataset = bigquery.Dataset(self.dataset_id)
             bq_dataset.location = self.location
             bq_dataset = self.client.create_dataset(bq_dataset, timeout=30)
         return bq_dataset
 
     def write(self, results, destination) -> str:
+        self._init_client()
         fake_report = results.is_fake
         column_names, results = self.get_columns_results(results)
         schema = self._define_schema(results, column_names)
         destination = DestinationFormatter.format_extension(destination)
         table = self._create_or_get_table(f"{self.dataset_id}.{destination}",
                                           schema)
         job_config = bigquery.LoadJobConfig(
@@ -142,20 +145,22 @@
                                                   destination=table,
                                                   job_config=job_config)
             logger.debug("Writing to %s is completed", destination)
         except Exception as e:
             raise ValueError(f"Unable to save data to BigQuery! {str(e)}")
         return f"[BigQuery] - at {self.dataset_id}.{destination}"
 
-    def _define_schema(self, results, header):
-        result_types = self._get_result_types(results, header)
-        return self._get_bq_schema(result_types)
+    @staticmethod
+    def _define_schema(results, header) -> List[bigquery.SchemaField]:
+        result_types = BigQueryWriter._get_result_types(results, header)
+        return BigQueryWriter._get_bq_schema(result_types)
 
+    @staticmethod
     def _get_result_types(
-            self, elements: Sequence[Any],
+            elements: Sequence[Any],
             column_names: Sequence[str]) -> Dict[str, Dict[str, Any]]:
         result_types = {}
         for i, element in enumerate(elements[0]):
             element_type = type(element)
             if element_type in [
                     list, proto.marshal.collections.repeated.RepeatedComposite,
                     proto.marshal.collections.repeated.Repeated
@@ -170,36 +175,42 @@
                 repeated = False
             result_types[column_names[i]] = {
                 "element_type": element_type,
                 "repeated": repeated
             }
         return result_types
 
-    def _get_bq_schema(self, types):
+    @staticmethod
+    def _get_bq_schema(types) -> List[bigquery.SchemaField]:
         TYPE_MAPPING = {
             list: "REPEATED",
             str: "STRING",
             int: "INT64",
             float: "FLOAT64",
             bool: "BOOL",
             proto.marshal.collections.repeated.RepeatedComposite: "REPEATED",
             proto.marshal.collections.repeated.Repeated: "REPEATED"
         }
 
-        schema = []
+        schema: List[bigquery.SchemaField] = []
         for key, value in types.items():
             element_type = TYPE_MAPPING.get(value.get("element_type"))
             schema.append(
                 bigquery.SchemaField(
                     name=key,
                     field_type="STRING" if not element_type else element_type,
                     mode="REPEATED" if value.get("repeated") else "NULLABLE"))
         return schema
 
-    def _create_or_get_table(self, table_name, schema):
+    def _init_client(self) -> None:
+        if not self.client:
+            self.client = bigquery.Client(self.project)
+
+    def _create_or_get_table(self, table_name: str, schema) -> bigquery.Table:
+        self._init_client()
         try:
             table = self.client.get_table(table_name)
         except NotFound:
             table_ref = bigquery.Table(table_name, schema=schema)
             table = self.client.create_table(table_ref)
             table = self.client.get_table(table_name)
         return table
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/parsers.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/query_editor.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/query_editor.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Dict, List, Optional, Tuple
+import datetime
 import dataclasses
 import re
 from .api_clients import BaseClient
 from operator import attrgetter
 
 
 @dataclasses.dataclass(frozen=True)
@@ -24,15 +25,23 @@
     type: str
     value: str
     fields: Optional[List[str]] = None
     substitute_expression: Optional[str] = None
 
 
 class VirtualColumnError(Exception):
-    pass
+    ...
+
+
+class FieldError(Exception):
+    ...
+
+
+class MacroError(Exception):
+    ...
 
 
 @dataclasses.dataclass
 class QueryElements:
     """Contains raw query and parsed elements.
 
     Attributes:
@@ -48,26 +57,44 @@
     column_names: List[str]
     customizers: Optional[Dict[str, Dict[str, str]]]
     virtual_columns: Optional[Dict[str, VirtualColumn]]
     resource_name: str
     is_constant_resource: bool
 
 
-class QuerySpecification:
+class CommonParametersMixin:
+    common_params = {
+        "date_iso": datetime.date.today().strftime("%Y%m%d"),
+        "current_date": datetime.date.today().strftime("%Y-%m-%d"),
+        "current_datetime":
+        datetime.datetime.today().strftime("%Y-%m-%d %H:%M:%S")
+    }
+
+
+class QuerySpecification(CommonParametersMixin):
 
     def __init__(self,
                  text: str,
-                 title: str = None,
-                 args: Dict[Any, Any] = None,
-                 api_version: str = "v12"):
+                 title: Optional[str] = None,
+                 args: Optional[Dict[Any, Any]] = None,
+                 api_version: str = "v12") -> None:
         self.text = text
         self.title = title
         self.args = args
+        self.macros = self._init_macros()
         self.base_client = BaseClient(api_version)
 
+    def _init_macros(self) -> Dict[str, str]:
+        if not self.args:
+            return self.common_params
+        if macros := self.args.get("macro"):
+            macros.update(self.common_params)
+            return macros
+        return self.common_params
+
     def generate(self) -> QueryElements:
         """Reads query from a file and returns different elements of a query.
 
         Args:
             path: Path to a file with a query.
 
         Returns:
@@ -75,50 +102,56 @@
             column_names, etc).
         """
 
         query_lines = self.cleanup_query_text(self.text)
         resource_name = self.extract_resource_from_query(self.text)
         is_constant_resource = bool(resource_name.endswith("_constant"))
         query_text = " ".join(query_lines)
-        if self.args:
-            if (macros := self.args.get("macro")):
-                query_text = query_text.format(**macros)
+        try:
+            query_text = query_text.format(**self.macros)
+        except KeyError as e:
+            raise MacroError(
+                f"No value provided for macro {str(e)}.")
         fields = []
         column_names = []
         customizers = {}
         virtual_columns = {}
 
         query_lines = self.extract_query_lines(" ".join(query_lines))
         for line in query_lines:
             field_name = None
             customizer_type = None
             field_elements, alias, virtual_column = self.extract_fields_and_aliases(
-                line)
+                line, self.macros)
             if field_elements:
                 for field_element in field_elements:
                     field_name, customizer_type, customizer_value = \
                         self.extract_fields_and_customizers(field_element)
                     field_name = field_name.strip().replace(",", "")
                     fields.append(self.format_type_field_name(field_name))
             if not alias and not field_name:
-                raise ValueError("Virtual attributes should be aliased")
+                raise VirtualColumnError(
+                    "Virtual attributes should be aliased")
             else:
                 column_name = alias.strip().replace(
                     ",", "") if alias else field_name
                 column_names.append(self.normalize_column_name(column_name))
 
             if virtual_column:
                 virtual_columns[column_name] = virtual_column
             if customizer_type:
                 customizers[column_name] = {
                     "type": customizer_type,
                     "value": customizer_value
                 }
         query_text = self.create_query_text(fields, virtual_columns,
                                             query_text)
+        for name, column in virtual_columns.items():
+            if not isinstance(virtual_columns[name].value, (int, float)):
+                virtual_columns[name].value.format(**self.macros)
         return QueryElements(query_title=self.title,
                              query_text=query_text,
                              fields=fields,
                              column_names=column_names,
                              customizers=customizers,
                              virtual_columns=virtual_columns,
                              resource_name=resource_name,
@@ -132,15 +165,15 @@
             if column.type == "expression" for field in column.fields
         ]
         if virtual_fields:
             fields = fields + virtual_fields
         query_text = f"SELECT {', '.join(fields)} {self.extract_from_statement(query_text)}"
         query_text = self._remove_traling_comma(query_text)
         query_text = self._unformat_type_field_name(query_text)
-        query_text = re.sub("\s+", " ", query_text).strip()
+        query_text = re.sub(r"\s+", " ", query_text).strip()
         return query_text
 
     def cleanup_query_text(self, query: str) -> List[str]:
         query_lines = query.split("\n")
         result = []
         for line in query_lines:
             if re.match("^(#|--|//)", line):
@@ -159,25 +192,33 @@
                                  flags=re.IGNORECASE).split(",")
         return [field.strip() for field in selected_fields if field != " "]
 
     def extract_from_statement(self, query_text: str) -> str:
         return re.search(" FROM .+", query_text, re.IGNORECASE).group(0)
 
     def extract_fields_and_aliases(
-        self, query_line: str
+        self, query_line: str, macros
     ) -> Tuple[Optional[List[str]], Optional[str], Optional[VirtualColumn]]:
         fields = []
         virtual_column = None
         field_raw, *alias = re.split(" [Aa][Ss] ", query_line)
-        field_raw = field_raw.replace("\s+", "").strip()
+        field_raw = field_raw.replace(r"\s+", "").strip()
         virtual_field, _, _ = self.extract_fields_and_customizers(field_raw)
         try:
             _ = attrgetter(virtual_field)(self.base_client.google_ads_row)
         except AttributeError:
-            operators = ("/", "\*", "\+", "-")
+            if virtual_field.isdigit():
+                virtual_field = int(virtual_field)
+            else:
+                try:
+                    virtual_field = float(virtual_field)
+                except ValueError:
+                    pass
+
+            operators = ("/", r"\*", r"\+", " - ")
             if len(expressions := re.split("|".join(operators),
                                            field_raw)) > 1:
                 virtual_column_fields = []
                 substitute_expression = virtual_field
                 for element in expressions:
                     element = element.strip()
                     try:
@@ -186,20 +227,31 @@
                         virtual_column_fields.append(element)
                         substitute_expression = substitute_expression.replace(
                             element, f"{{{element}}}")
                     except AttributeError:
                         pass
                 virtual_column = VirtualColumn(
                     type="expression",
-                    value=virtual_field,
+                    value=virtual_field.format(
+                        **macros) if macros else virtual_field,
                     fields=virtual_column_fields,
-                    substitute_expression=substitute_expression.replace(".", "_"))
+                    substitute_expression=substitute_expression.replace(
+                        ".", "_"))
             else:
+                if not isinstance(virtual_field, (int, float)):
+                    if not self._not_a_quoted_string(virtual_field):
+                        raise FieldError(
+                            f"Incorrect field '{virtual_field}' in the query '{self.title}'."
+                        )
+                    virtual_field = virtual_field.replace("'",
+                                                          "").replace('"', '')
+                    virtual_field = virtual_field.format(
+                        **macros) if macros else virtual_field
                 virtual_column = VirtualColumn(type="built-in",
-                                                     value=virtual_field)
+                                               value=virtual_field)
         if not virtual_column and field_raw:
             fields = [field_raw]
         else:
             fields = None
         return fields, alias[0] if alias else None, virtual_column
 
     def extract_fields_and_customizers(self, line_elements: str):
@@ -233,7 +285,13 @@
         return re.sub(r"\.", "_", column_name)
 
     def _remove_traling_comma(self, query: str) -> str:
         return re.sub(r",\s+from", " FROM", query, re.IGNORECASE)
 
     def _unformat_type_field_name(self, query: str) -> str:
         return re.sub(r"\.type_", ".type", query)
+
+    def _not_a_quoted_string(self, field_name: str) -> bool:
+        if ((field_name.startswith("'") and field_name.endswith("'"))
+                or (field_name.startswith('"') and field_name.endswith('"'))):
+            return True
+        return False
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/query_executor.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/query_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,17 +94,18 @@
                 logger.error(str(e))
                 raise
         if not total_results:
             row = self.api_client.google_ads_row
             results = [parser.parse_ads_row(row)]
             total_results.extend(results)
             is_fake_report = True
-            logger.warning(
-                "Query %s generated zero results, using placeholders to infer schema",
-                query_specification.query_title)
+            if not isinstance(self.api_client, api_clients.BaseClient):
+                logger.warning(
+                    "Query %s generated zero results, using placeholders to infer schema",
+                    query_specification.query_title)
         return GaarfReport(results=total_results,
                            column_names=query_specification.column_names,
                            is_fake=is_fake_report)
 
     def _parse_ads_response(
         self,
         query_specification: QueryElements,
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/query_post_processor.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/query_post_processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,18 +32,24 @@
                     name: value
                     for name, value in templates.items() if name in query_text
                 }
                 if query_templates:
                     query_text = self.expand_jinja(query_text, query_templates)
                     logger.debug("Query text after jinja expansion:\n%s",
                                  query_text)
+                else:
+                    query_text = self.expand_jinja(query_text, {})
+            else:
+                query_text = self.expand_jinja(query_text, {})
             if (macros := params.get("macro")):
                 query_text = query_text.format(**macros)
                 logger.debug("Query text after macro substitution:\n%s",
                              query_text)
+        else:
+            query_text = self.expand_jinja(query_text, {})
         return query_text
 
     def expand_jinja(self, query_text: str, template_params: Optional[Dict[str,
                                                                   Any]] = None) -> str:
         if not template_params:
             return Template(query_text).render()
         for key, value in template_params.items():
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/report.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,18 @@
         raise IndexError(f"cannot find {element} element!")
 
     def __setattr__(self, name: str, value: Union[str, int]) -> None:
         self.__setitem__(name, value)
 
     def __setitem__(self, name: str, value: Union[str, int]) -> None:
         if name in self.column_names:
-            self.data[self.column_names.index(name)] = value
+            if len(self.column_names) == len(self.data):
+                self.data[self.column_names.index(name)] = value
+            else:
+                self.data.append(value)
         else:
             self.data.append(value)
             self.column_names.append(name)
 
     def get(self, item: str) -> Any:
         return self.__getattr__(item)
```

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/simulation.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/sql_executor.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/sql_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/gaarf/utils.py` & `google-ads-api-report-fetcher-1.7.0/gaarf/utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/PKG-INFO` & `google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.6.0
+Version: 1.7.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt` & `google-ads-api-report-fetcher-1.7.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/setup.py` & `google-ads-api-report-fetcher-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "sqlalchemy": ["sqlalchemy"],
     "simulator": ["Faker"]
 }
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     name="google-ads-api-report-fetcher",
-    version="1.6.0",
+    version="1.7.0",
     description=
     "Library for fetching reports from Google Ads API and saving them locally / BigQuery.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/google/ads-api-reports-fetcher",
     author="Google Inc. (gTech gPS CSE team)",
     author_email="no-reply@google.com",
```

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_base_query.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_cli_utils.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_cli_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
+from unittest import mock
 
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
 import gaarf.cli.utils as utils
+from gaarf.query_editor import CommonParametersMixin
 
 
 def test_convert_date():
     current_date = datetime.today()
     current_year = datetime(current_date.year, 1, 1)
     current_month = datetime(current_date.year, current_date.month, 1)
     last_year = current_year - relativedelta(years=1)
@@ -47,16 +49,18 @@
 @pytest.fixture
 def param_parser():
     return utils.ParamsParser(["macro", "sql", "template"])
 
 
 def test_if_incorrect_param_is_provided(param_parser):
     with pytest.raises(utils.GaarfParamsException):
-        parsed_params = param_parser.parse(
-            ["--macros.start_date=2022-01-01", "--fake_param.end_date=2022-12-31"])
+        parsed_params = param_parser.parse([
+            "--macros.start_date=2022-01-01",
+            "--fake_param.end_date=2022-12-31"
+        ])
 
 
 def test_identify_param_pair_existing(param_parser):
     param_pair = param_parser._identify_param_pair(
         "macro", ["--macro.start_date", "2022-01-01"])
     assert param_pair == {"start_date": "2022-01-01"}
 
@@ -69,30 +73,25 @@
 
 def test_identify_param_pair_raises_error(param_parser):
     with pytest.raises(utils.GaarfParamsException):
         param_parser._identify_param_pair(
             "macro", ["--macro.start_date", ":YYYYMMDD", "extra_element"])
 
 
-@pytest.fixture
-def current_date_iso():
-    return datetime.today().strftime("%Y%m%d")
-
-
-def test_parse_params(param_parser, current_date_iso):
+def test_parse_params(param_parser):
     parsed_params = param_parser._parse_params(
         "macro",
         ["--macro.start_date=2022-01-01", "--macro.end_date=2022-12-31"])
     assert parsed_params == {
         "start_date": "2022-01-01",
         "end_date": "2022-12-31"
     }
 
 
-def test_parse(param_parser, current_date_iso):
+def test_parse(param_parser):
     parsed_params = param_parser.parse(
         ["--macro.start_date=2022-01-01", "--macro.end_date=2022-12-31"])
     assert parsed_params == {
         "macro": {
             "start_date": "2022-01-01",
             "end_date": "2022-12-31"
         },
@@ -152,23 +151,24 @@
             "output": "console",
             "api_version": "10",
         }
     }
 
 
 def test_gaarf_config_saver_gaarf_dont_save_inner_empty_values(config_saver):
-    gaarf_config = utils.GaarfConfig(output="console",
-                                     api_version="10",
-                                     account="1",
-                                     params={"macro": {
-                                         "start_date": ":YYYYMMDD"
-                                     }},
-                                     writer_params={},
-                                     customer_ids_query="",
-                                     customer_ids_query_file="")
+    gaarf_config = utils.GaarfConfig(
+        output="console",
+        api_version="10",
+        account="1",
+        params={"macro": {
+            "start_date": ":YYYYMMDD"
+        }},
+        writer_params={},
+        customer_ids_query="",
+        customer_ids_query_file="")
 
     config = config_saver.prepare_config({}, gaarf_config)
     assert config == {
         "gaarf": {
             "account": ["1"],
             "output": "console",
             "api_version": "10",
@@ -178,21 +178,22 @@
                 }
             }
         }
     }
 
 
 def test_config_saver_gaarf_save_customer_ids_query_values(config_saver):
-    gaarf_config = utils.GaarfConfig(output="console",
-                                     api_version="10",
-                                     account="1",
-                                     params={},
-                                     writer_params={},
-                                     customer_ids_query="SELECT",
-                                     customer_ids_query_file="path/to/file.sql")
+    gaarf_config = utils.GaarfConfig(
+        output="console",
+        api_version="10",
+        account="1",
+        params={},
+        writer_params={},
+        customer_ids_query="SELECT",
+        customer_ids_query_file="path/to/file.sql")
 
     config = config_saver.prepare_config({}, gaarf_config)
     assert config == {
         "gaarf": {
             "account": ["1"],
             "output": "console",
             "api_version": "10",
@@ -202,15 +203,17 @@
     }
 
 
 def test_config_saver_gaarf_bq(config_saver):
     gaarf_bq_config = utils.GaarfBqConfig(
         project="fake-project",
         dataset_location="fake-location",
-        params={"macro": {"bq_project": "another-fake-project"}})
+        params={"macro": {
+            "bq_project": "another-fake-project"
+        }})
     config = config_saver.prepare_config({}, gaarf_bq_config)
     assert config == {
         "gaarf-bq": {
             "project": "fake-project",
             "dataset_location": "fake-location",
             "params": {
                 "macro": {
@@ -218,32 +221,36 @@
                 }
             }
         }
     }
 
 
 def test_config_saver_does_not_save_empty_params(config_saver):
-    gaarf_bq_config = utils.GaarfBqConfig(
-        project="fake-project",
-        dataset_location="fake-location",
-        params={})
+    gaarf_bq_config = utils.GaarfBqConfig(project="fake-project",
+                                          dataset_location="fake-location",
+                                          params={})
     config = config_saver.prepare_config({}, gaarf_bq_config)
     assert config == {
         "gaarf-bq": {
             "project": "fake-project",
             "dataset_location": "fake-location"
         }
     }
 
 
 def test_config_saver_does_not_save_empty_nested_params(config_saver):
-    gaarf_bq_config = utils.GaarfBqConfig(
-        project="fake-project",
-        dataset_location="fake-location",
-        params={"macro": {"bq_project": "another-fake-project"}, "sql": {}})
+    gaarf_bq_config = utils.GaarfBqConfig(project="fake-project",
+                                          dataset_location="fake-location",
+                                          params={
+                                              "macro": {
+                                                  "bq_project":
+                                                  "another-fake-project"
+                                              },
+                                              "sql": {}
+                                          })
     config = config_saver.prepare_config({}, gaarf_bq_config)
     assert config == {
         "gaarf-bq": {
             "project": "fake-project",
             "dataset_location": "fake-location",
             "params": {
                 "macro": {
@@ -276,44 +283,58 @@
                                  "start_date": "2022-01-01"
                              }},
                              writer_params={},
                              customer_ids_query=None,
                              customer_ids_query_file=None)
 
 
-def test_initialize_config_with_runtime_parameters(config_with_runtime_params,
-                                                   current_date_iso):
-    initialized_config = utils.initialize_runtime_parameters(
-        config_with_runtime_params)
-    expected_config = utils.GaarfConfig(
-        output="console",
-        api_version="10",
-        account="1",
-        params={
-            "macro": {
-                "start_date": datetime.today().strftime("%Y-%m-%d"),
-                "date_iso": current_date_iso
-            }
-        },
-        writer_params={},
-        customer_ids_query=None,
-        customer_ids_query_file=None)
-    assert initialized_config == expected_config
+def test_initialize_config_with_runtime_parameters(config_with_runtime_params):
+    with mock.patch.object(CommonParametersMixin,
+                           "common_params", {
+                               "date_iso": "19700101",
+                               "current_date": "1970-01-01",
+                               "current_datetime": "1970-01-01 00-00-00" }):
+        initialized_config = utils.initialize_runtime_parameters(
+            config_with_runtime_params)
+        expected_config = utils.GaarfConfig(
+            output="console",
+            api_version="10",
+            account="1",
+            params={
+                "macro": {
+                    "start_date": datetime.today().strftime("%Y-%m-%d"),
+                    "date_iso": "19700101",
+                    "current_date": "1970-01-01",
+                    "current_datetime": "1970-01-01 00-00-00"
+                }
+            },
+            writer_params={},
+            customer_ids_query=None,
+            customer_ids_query_file=None)
+        assert initialized_config == expected_config
 
 
 def test_initialize_config_without_runtime_parameters(
-        config_without_runtime_params, current_date_iso):
-    initialized_config = utils.initialize_runtime_parameters(
-        config_without_runtime_params)
-    expected_config = utils.GaarfConfig(output="console",
-                                        api_version="10",
-                                        account="1",
-                                        params={
-                                            "macro": {
-                                                "start_date": "2022-01-01",
-                                                "date_iso": current_date_iso
-                                            }
-                                        },
-                                        writer_params={},
-                                        customer_ids_query=None,
-                                        customer_ids_query_file=None)
-    assert initialized_config == expected_config
+        config_without_runtime_params):
+    with mock.patch.object(CommonParametersMixin,
+                           "common_params", {
+                               "date_iso": "19700101",
+                               "current_date": "1970-01-01",
+                               "current_datetime": "1970-01-01 00-00-00" }):
+        initialized_config = utils.initialize_runtime_parameters(
+            config_without_runtime_params)
+        expected_config = utils.GaarfConfig(
+            output="console",
+            api_version="10",
+            account="1",
+            params={
+                "macro": {
+                    "start_date": "2022-01-01",
+                    "date_iso": "19700101",
+                    "current_date": "1970-01-01",
+                    "current_datetime": "1970-01-01 00-00-00"
+                }
+            },
+            writer_params={},
+            customer_ids_query=None,
+            customer_ids_query_file=None)
+        assert initialized_config == expected_config
```

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_parsers.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from typing import Any, Dict, List
 from dataclasses import dataclass
-from proto import Message
+import proto
 import gaarf.parsers as parsers
 from gaarf.query_editor import VirtualColumn, VirtualColumnError
 
 
 @dataclass
 class FakeGoogleAdsRowElement:
     value: int
@@ -77,14 +77,17 @@
 
 
 @pytest.fixture
 def google_ads_row_parser(fake_query_specification):
     return parsers.GoogleAdsRowParser(fake_query_specification)
 
 
+class TestMessage(proto.Message):
+    message = proto.Field(proto.STRING, number=1)
+
 def test_google_ads_row_parser_return_last_parser_in_chain(
         google_ads_row_parser):
     assert type(google_ads_row_parser.parser) == parsers.RepeatedParser
 
 
 def test_google_ads_row_parser_chooses_correct_element_parser(
         google_ads_row_parser, fake_google_ads_row_element):
@@ -141,19 +144,18 @@
     attribute_parser = parsers.AttributeParser(base_parser)
     assert attribute_parser.parse("") == None
     assert attribute_parser.parse(name_attribute) == "some-name"
     assert attribute_parser.parse(text_attribute) == "some-text"
     assert attribute_parser.parse(value_attribute) == 1
 
 
-@pytest.mark.skip("WIP")
 def test_empty_attribute_parser(base_parser):
     empty_attribute_parser = parsers.EmptyAttributeParser(base_parser)
     assert empty_attribute_parser.parse("") == None
-    message = Message()
+    message = TestMessage(message="test")
     assert empty_attribute_parser.parse(message) == "Not set"
 
 
 def test_google_ads_row_parser(google_ads_row_parser, text_attribute,
                                name_attribute, value_attribute):
     assert isinstance(google_ads_row_parser.parser, parsers.RepeatedParser)
     assert google_ads_row_parser.parse(name_attribute) == "some-name"
```

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_query_editor.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_query_editor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import pytest
+import datetime
 import gaarf.query_editor as query_editor
 
 
 @pytest.fixture
 def query_specification():
     query = """
 -- Comment
 # Comment
 // Comment
 
 SELECT
-    '20230101' AS date,
+    1 AS constant,
+    '2023-01-01' AS date,
+    '{current_date}' AS current_date,
     metrics.clicks / metrics.impressions AS ctr,
     customer.id, --customer_id
     campaign.bidding_strategy_type AS campaign_type, campaign.id:nested AS campaign,
     ad_group.id~1 AS ad_group,
     ad_group_ad.ad.id->asset AS ad,
     metrics.cost_micros * 1e6 AS cost,
     campaign.selective_optimization AS selective_optimization,
@@ -26,42 +29,29 @@
 
 
 @pytest.fixture
 def sample_query(query_specification):
     return query_specification.generate()
 
 
-@pytest.fixture
-def incorrect_query_specification():
-    query = """
-SELECT
-    "${custom_field}",
-    ad_group.id AS ad_group_id
-FROM ad_group_id
-"""
-    return query_editor.QuerySpecification(title="sample_query",
-                                           text=query,
-                                           args=None)
-
-
 def test_correct_title(sample_query):
     assert sample_query.query_title == "sample_query"
 
 
 def test_extract_correct_fields(sample_query):
     assert sample_query.fields == [
         "customer.id", "campaign.bidding_strategy_type", "campaign.id",
         "ad_group.id", "ad_group_ad.ad.id", "campaign.selective_optimization"
     ]
 
 
 def test_extract_correct_aliases(sample_query):
     assert sample_query.column_names == [
-        "date", "ctr", "customer_id", "campaign_type", "campaign", "ad_group",
-        "ad", "cost", "selective_optimization"
+        "constant", "date", "current_date", "ctr", "customer_id", "campaign_type",
+        "campaign", "ad_group", "ad", "cost", "selective_optimization"
     ]
 
 
 def test_extract_correct_text(sample_query):
     assert sample_query.query_text.lower(
     ) == "select customer.id, campaign.bidding_strategy_type, campaign.id, ad_group.id, ad_group_ad.ad.id, campaign.selective_optimization, metrics.clicks, metrics.impressions, metrics.cost_micros from ad_group_ad"
 
@@ -99,16 +89,21 @@
 
 def test_is_constant_resource(sample_query):
     assert sample_query.is_constant_resource == False
 
 
 def test_has_virtual_columns(sample_query):
     assert sample_query.virtual_columns == {
+        "constant":
+        query_editor.VirtualColumn(type="built-in", value=1),
         "date":
-        query_editor.VirtualColumn(type="built-in", value="'20230101'"),
+        query_editor.VirtualColumn(type="built-in", value="2023-01-01"),
+        "current_date":
+        query_editor.VirtualColumn(
+            type="built-in", value=datetime.date.today().strftime("%Y-%m-%d")),
         "ctr":
         query_editor.VirtualColumn(
             type="expression",
             value="metrics.clicks / metrics.impressions",
             fields=["metrics.clicks", "metrics.impressions"],
             substitute_expression="{metrics_clicks} / {metrics_impressions}"),
         "cost":
@@ -116,11 +111,31 @@
             type="expression",
             value="metrics.cost_micros * 1e6",
             fields=["metrics.cost_micros"],
             substitute_expression="{metrics_cost_micros} * 1e6")
     }
 
 
-def test_incorrect_specification_raises_value_error(
-        incorrect_query_specification):
-    with pytest.raises(ValueError):
-        incorrect_query_specification.generate()
+def test_incorrect_specification_raises_macro_error():
+    query = "SELECT '${custom_field}', ad_group.id FROM ad_group_id"
+    spec = query_editor.QuerySpecification(title="sample_query",
+                                           text=query,
+                                           args=None)
+    with pytest.raises(query_editor.MacroError):
+        spec.generate()
+
+
+def test_incorrect_specification_raises_virtual_column_error():
+    query = "SELECT 1, ad_group.id AS ad_group_id FROM ad_group_id"
+    spec = query_editor.QuerySpecification(title="sample_query",
+                                           text=query,
+                                           args=None)
+    with pytest.raises(query_editor.VirtualColumnError):
+        spec.generate()
+
+def test_incorrect_field_raises_value_error():
+    query = "SELECT metric.impressions, ad_group.id FROM ad_group_id"
+    spec = query_editor.QuerySpecification(title="sample_query",
+                                           text=query,
+                                           args=None)
+    with pytest.raises(query_editor.FieldError):
+        spec.generate()
```

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_query_post_processor.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_query_post_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,7 +90,25 @@
                 "field_2": "field_two"
             },
             "template": {
                 "cohort_days": "1,2"
             }
         })
     assert rendered_query.replace("  ", " ") == expected_query
+
+def test_replace_params_empty_template_is_ignored(macro_template_query_with_for_loop):
+    expected_query = "SELECT field_one, field_two AS field_two, FROM some_table"
+    rendered_query = PostProcessorMixin().replace_params_template(
+        macro_template_query_with_for_loop,
+        params={
+            "macro": {
+                "field_2": "field_two"
+            }
+        })
+    assert rendered_query.replace("  ", " ") == expected_query
+
+def test_replace_empty_params(macro_template_query_with_for_loop):
+    expected_query = "SELECT field_one, {field_2} AS field_two, FROM some_table"
+    rendered_query = PostProcessorMixin().replace_params_template(
+        macro_template_query_with_for_loop,
+        params={})
+    assert rendered_query.replace("  ", " ") == expected_query
```

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_reader.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_report.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -194,12 +194,30 @@
     row = multi_column_report[0]
     row.campaign_id_new = row.campaign_id * 100
     assert row == GaarfRow(
         data=[1, 2, 100],
         column_names=["campaign_id", "ad_group_id", "campaign_id_new"])
 
 
+def test_set_non_existing_attribute_gaarf_rows_get_new_columns(
+        multi_column_report):
+    for row in multi_column_report:
+        row.campaign_id_new = row.campaign_id * 100
+    assert multi_column_report == GaarfReport(
+        results=[[1, 2, 100], [2, 3, 200], [3, 4, 300]],
+        column_names=["campaign_id", "ad_group_id", "campaign_id_new"])
+
+
 def test_set_existing_attribute_gaarf_row_updates_column(multi_column_report):
     row = multi_column_report[0]
     row.campaign_id = row.campaign_id * 100
     assert row == GaarfRow(data=[100, 2],
                            column_names=["campaign_id", "ad_group_id"])
+
+
+def test_set_existing_attribute_gaarf_multiple_rows_updates_columns(
+        multi_column_report):
+    for row in multi_column_report:
+        row.campaign_id = row.campaign_id * 100
+    assert multi_column_report == GaarfReport(
+        results=[[100, 2], [200, 3], [300, 4]],
+        column_names=["campaign_id", "ad_group_id"])
```

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_simulation.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.6.0/tests/unit/test_writer.py` & `google-ads-api-report-fetcher-1.7.0/tests/unit/test_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 
 @pytest.fixture
 def csv_writer():
     return writer.CsvWriter("/tmp")
 
 
 @pytest.fixture
-def bq_writer():
-    return writer.BigQueryWriter("fake_project", "fake_dataset")
-
-
-@pytest.fixture
 def single_column_data():
     results = [1, 2, 3]
     columns = ["column_1"]
     return GaarfReport(results, columns)
 
 
 @pytest.fixture
@@ -42,17 +37,17 @@
     expected = ["column_1,column_2,column_3", '1,two,3|4']
     csv_writer.write(sample_data, "test.csv")
     with open(tmp_file, "r") as f:
         file = f.readlines()
     assert [row.strip() for row in file] == expected
 
 
-def test_bq_get_results_types(bq_writer, sample_data):
+def test_bq_get_results_types(sample_data):
     results, columns = sample_data.results, sample_data.column_names
-    result_types = bq_writer._get_result_types(results, columns)
+    result_types = writer.BigQueryWriter._get_result_types(results, columns)
     assert result_types == {
         'column_1': {
             'element_type': int,
             'repeated': False
         },
         'column_2': {
             'element_type': str,
@@ -61,17 +56,17 @@
         'column_3': {
             'element_type': int,
             'repeated': True
         }
     }
 
 
-def test_bq_get_correct_schema(bq_writer, sample_data):
+def test_bq_get_correct_schema(sample_data):
     results, columns = sample_data.results, sample_data.column_names
-    schema = bq_writer._define_schema(results, columns)
+    schema = writer.BigQueryWriter._define_schema(results, columns)
     assert schema == [
         SchemaField('column_1', 'INT64', 'NULLABLE', None, None, (), None),
         SchemaField('column_2', 'STRING', 'NULLABLE', None, None, (), None),
         SchemaField('column_3', 'INT64', 'REPEATED', None, None, (), None)
     ]
```


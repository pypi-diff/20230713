# Comparing `tmp/fbn-0.1.1-py3-none-any.whl.zip` & `tmp/fbn-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8554 bytes, number of entries: 12
--rw-r--r--  2.0 unx       81 b- defN 23-Jul-09 20:55 fbn/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jul-09 20:55 fbn/__main__.py
--rw-r--r--  2.0 unx     2686 b- defN 23-Jul-09 20:55 fbn/cli.py
--rw-r--r--  2.0 unx       78 b- defN 23-Jul-09 20:55 fbn/constants.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jul-09 20:55 fbn/exceptions.py
--rw-r--r--  2.0 unx     7374 b- defN 23-Jul-09 20:55 fbn/fb.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5020 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/RECORD
-12 files, 17782 bytes uncompressed, 7106 bytes compressed:  60.0%
+Zip file size: 8844 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       81 b- defN 23-Jul-13 04:16 fbn/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jul-13 04:16 fbn/__main__.py
+-rw-r--r--  2.0 unx     3064 b- defN 23-Jul-13 04:16 fbn/cli.py
+-rw-r--r--  2.0 unx       78 b- defN 23-Jul-13 04:16 fbn/constants.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jul-13 04:16 fbn/exceptions.py
+-rw-r--r--  2.0 unx     7533 b- defN 23-Jul-13 04:16 fbn/fb.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-13 04:17 fbn-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5405 b- defN 23-Jul-13 04:17 fbn-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 04:17 fbn-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-13 04:17 fbn-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-13 04:17 fbn-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 23-Jul-13 04:17 fbn-0.1.2.dist-info/RECORD
+12 files, 18704 bytes uncompressed, 7396 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: fbn/exceptions.py
 Comment: 
 
 Filename: fbn/fb.py
 Comment: 
 
-Filename: fbn-0.1.1.dist-info/LICENSE
+Filename: fbn-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: fbn-0.1.1.dist-info/METADATA
+Filename: fbn-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: fbn-0.1.1.dist-info/WHEEL
+Filename: fbn-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: fbn-0.1.1.dist-info/entry_points.txt
+Filename: fbn-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: fbn-0.1.1.dist-info/top_level.txt
+Filename: fbn-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fbn-0.1.1.dist-info/RECORD
+Filename: fbn-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbn/__init__.py

```diff
@@ -1,3 +1,3 @@
 __author__ = "Visesh Prasad"
 __email__ = "visesh@live.com"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## fbn/cli.py

```diff
@@ -65,18 +65,29 @@
     default=10,
     show_default=True,
     help="Number of posts to sample",
 )
 @click.option(
     "-e",
     "--every",
-    "frequency",
+    "every",
     type=str,
     required=False,
-    help="Monitor frequency",
+    help="Monitor frequency. Of the form <int><m/h/d/w>. "
+         "Eg: --every 2m. Will check every 2 minutes.",
+)
+@click.option(
+    "-t",
+    "--to",
+    "to",
+    type=str,
+    required=False,
+    help="Monitor randomization frequency. Requires --every. Same form as --every. "
+         "Both units must match. "
+         "Eg: --every 1h --to 2h. Will randomize checks every 1 to 2 hours. "
 )
 @click.option(
     "-a",
     "--apprise-url",
     type=str,
     required=True,
     envvar="FBN_APPRISE_URL",
@@ -92,15 +103,16 @@
 def main(
     target_id,
     username,
     password,
     cookies_file,
     user_agent,
     sample_count,
-    frequency,
+    every,
+    to,
     apprise_url,
     on_error,
     verbose,
 ):
     """
     Simple CLI tool to look for new posts in a Facebook group and
     then send you a notification. Public groups do not require authentication information.
@@ -115,15 +127,16 @@
         check_and_notify(
             target_id,
             username,
             password,
             cookies_file,
             user_agent,
             sample_count,
-            frequency,
+            every,
+            to,
             apprise_url,
             on_error,
             verbose,
         )
     except Exception as e:
         # all other exceptions
         click.echo(e)
```

## fbn/fb.py

```diff
@@ -151,15 +151,16 @@
 def check_and_notify(
     target_id,
     username,
     password,
     cookies_file,
     user_agent,
     sample_count,
-    frequency,
+    every,
+    to,
     apprise_url,
     on_error,
     verbose,
 ):
     if verbose:
         # fbn logging
         level = logging.DEBUG
@@ -200,20 +201,24 @@
             raise NoAuthInfoException(
                 "Please provide your Facebook username/password or a cookies file."
             )
 
     logger.debug(f"Running for the first time...")
     check_fb(**kwargs)
     logger.debug("Creating schedule...")
-    if frequency:
-        interval, unit = parse_frequency(frequency)
+    if every:
+        interval, unit = parse_frequency(every)
         schedule_unit = SCHEDULE_UNIT_MAP[unit]
-        getattr(schedule.every(int(interval)), schedule_unit).do(check_fb, **kwargs)
+        every_schedule = schedule.every(int(interval))
+        if to:
+            interval, _ = parse_frequency(to)
+            every_schedule = every_schedule.to(int(interval))
+        getattr(every_schedule, schedule_unit).do(check_fb, **kwargs)
     else:  # randomize as the default
-        schedule.every(2).to(4).hours.do(check_fb, **kwargs)
+        schedule.every(1).to(3).hours.do(check_fb, **kwargs)
     # run
     while True:
         logger.debug(f"Next check at {schedule.next_run()}...")
         n = schedule.idle_seconds()
         if n > 0:
             # sleep exactly the right amount of time
             time.sleep(n)
```

## Comparing `fbn-0.1.1.dist-info/LICENSE` & `fbn-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fbn-0.1.1.dist-info/METADATA` & `fbn-0.1.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbn
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool to monitor fb groups and notify
 Home-page: https://github.com/viseshrp/fbn
 Author: Visesh Prasad
 Author-email: visesh@live.com
 Maintainer: Visesh Prasad
 Maintainer-email: visesh@live.com
 License: MIT license
@@ -63,15 +63,20 @@
   -u, --username TEXT         Your Facebook username  [env var:
                               FBN_FB_USERNAME]
   -p, --password TEXT         Your Facebook password  [env var:
                               FBN_FB_PASSWORD]
   -c, --cookies-file FILE     Path to the Facebook cookies file
   -g, --user-agent TEXT       User agent to use for scraping
   -s, --sample-count INTEGER  Number of posts to sample  [default: 10]
-  -e, --every TEXT            Monitor frequency
+  -e, --every TEXT            Monitor frequency. Of the form <int><m/h/d/w>.
+                              Eg: --every 2m. Will check every 2 minutes.
+  -t, --to TEXT               Monitor randomization frequency. Requires
+                              --every. Same form as --every. Both units must
+                              match. Eg: --every 1h --to 2h. Will randomize
+                              checks every 1 to 2 hours.
   -a, --apprise-url TEXT      The apprise URL to notify  [env var:
                               FBN_APPRISE_URL; required]
   --include-errors            Notify of errors as well.
   -v, --verbose               Enable debug logging.
   -h, --help                  Show this message and exit.
 ```
```

## Comparing `fbn-0.1.1.dist-info/RECORD` & `fbn-0.1.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-fbn/__init__.py,sha256=n_RcprRToTC1WU4QumeFXWop6H7YvKMc4uSUey_ou7Q,81
+fbn/__init__.py,sha256=xVqyqVADQP-dcLEC8hXPS8rPReXm6PsEH-WA-6cXC7k,81
 fbn/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
-fbn/cli.py,sha256=Hg0l2gxOrO_TT_RjdjU4iQnjLcIuaXLKXM3qPYDZp3Y,2686
+fbn/cli.py,sha256=HezMRsS_KK-ko0gs3mPJrmGNUliwbW3GHtA6N6UDuwc,3064
 fbn/constants.py,sha256=cMQzDOJVV3vm3P1UqY1DKpB5OfhLdT5fbLEM6tAu6l8,78
 fbn/exceptions.py,sha256=8yan1cmPUJEbiTW12adRoyWF48zb3L2SCKEW1trobyA,406
-fbn/fb.py,sha256=A5F-TSLKuramGwsMAYLGOB-zgyzNeO_tvHnrq58kkWA,7374
-fbn-0.1.1.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
-fbn-0.1.1.dist-info/METADATA,sha256=TlRmL8O9sdFe5OIU3pNCgfuHQuZrELjUgPf-afCmiZA,5020
-fbn-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fbn-0.1.1.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
-fbn-0.1.1.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
-fbn-0.1.1.dist-info/RECORD,,
+fbn/fb.py,sha256=ojjtq4FfRWUv1YILCzG3tFxtKUtCRaUh9Ka-P5z0tdA,7533
+fbn-0.1.2.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
+fbn-0.1.2.dist-info/METADATA,sha256=8iezr2yb_g-3aLC4zgrhloustZchVQlFeLQxzEJv9_Y,5405
+fbn-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fbn-0.1.2.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
+fbn-0.1.2.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
+fbn-0.1.2.dist-info/RECORD,,
```


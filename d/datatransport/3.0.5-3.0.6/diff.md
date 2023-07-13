# Comparing `tmp/datatransport-3.0.5.tar.gz` & `tmp/datatransport-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransport-3.0.5.tar", last modified: Mon Jul 10 06:31:27 2023, max compression
+gzip compressed data, was "datatransport-3.0.6.tar", last modified: Thu Jul 13 20:00:21 2023, max compression
```

## Comparing `datatransport-3.0.5.tar` & `datatransport-3.0.6.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/
--rw-rw-r--   0 valentic   (500) valentic   (500)    49591 2023-07-09 19:59:41.000000 datatransport-3.0.5/CHANGES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.5/INSTALL
--rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.5/LICENSE
--rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.5/MANIFEST.in
--rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.5/MIGRATION
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-10 06:31:27.000000 datatransport-3.0.5/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.5/README.rst
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/
--rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/.coverage
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2351 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/archivegroups/archivegroups.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2340 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/component/component.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1759 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/environ/environ.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1098 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/environ/environ.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.5/contrib/examples/examples.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/filewatch/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1654 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/getbytes/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      896 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/hello/
--rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.5/contrib/examples/hello/hello.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      799 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/hello/helloworld.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/init/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      973 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/init/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/init/init.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/messagebox/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/messagebox/messagebox.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/messagebox/poll_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/messagebox/poll_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/messagebox/post_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/messagebox/post_text.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/postpoll/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1009 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/postpoll/poll_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      836 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/postpoll/poll_text.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1125 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/postpoll/post_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      957 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/postpoll/post_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/postpoll/postpoll.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/rotatelogs/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      861 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/service/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1175 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/service/client.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/service/directory.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/service/echo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/service/service.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/spawn/spawn.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1284 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples/watchdog/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1054 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/watchdog/crasher.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/watchdog/init_crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/README
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/archivegroups/archivegroups.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/component/component.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/config/config.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/config/config.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/diskmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/diskmonitor/diskmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/environ/environ.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/environ/environ.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/eventmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/eventmonitor/eventmonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/eventmonitor/serverstate.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/filewatch/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/getbytes/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/instrumentstatus/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/instrumentstatus/plugin.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/instrumentstatus/postdata
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/multipoll/
--rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/multipoll/README
--rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/multipoll/multipoll.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/multipoll/reader.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/multipoll/writer.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/newsgroupmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/plottool/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/plottool/datasource.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/plottool/plottool.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/postdatafiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/postdatafiles/checkdate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/postdatafiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/postdatafiles/postdatafiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/resourcemonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/rotatelogs/
--rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/spawn/spawn.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/splitfiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/splitfiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/splitfiles/splitfiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/syncpoller/
--rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/syncpoller/poller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/syncpoller/source.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/syncpoller/syncpoller.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/test.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/wait/
--rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/wait/timer.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/wait/wait.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/examples.v2/watchdog/
--rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/watchdog/crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/examples.v2/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/contrib/utils/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/utils/createnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/utils/getarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/utils/postarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/utils/rebuilddatabase
--rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/utils/relaynewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/utils/rmnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.5/contrib/utils/watchtransport
--rw-rw-r--   0 valentic   (500) valentic   (500)     2611 2023-07-10 06:31:17.000000 datatransport-3.0.5/pyproject.toml
--rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-10 06:31:27.000000 datatransport-3.0.5/setup.cfg
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/
--rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1584 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/accessmixin.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/commands/
--rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/cancelnewsgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/console.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/listnewsgroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/transport_create_app.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/transportctl.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/transportd.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/commands/transportps.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7860 2023-07-08 23:10:13.000000 datatransport-3.0.5/src/datatransport/commands/viewlog.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/components/
--rw-rw-r--   0 valentic   (500) valentic   (500)    50983 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/ArchiveGroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2405 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/DirectoryService.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5325 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/DiskMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     6212 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/EventMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4130 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/FilePost.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     9573 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/FileStore.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5460 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/FileWatch.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5213 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/GroupControl.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/InstrumentStatus.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4364 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/NewsGateway.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7859 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/NewsgroupMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/PageKit.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/PlotTool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    12588 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/PostDataFiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/RealTimeFeed.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/ResourceMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     6851 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/Scheduler.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/SyncPoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11920 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/WatchURL.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      645 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/components/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1335 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/configcomponent.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3058 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/directory.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-09 20:00:49.000000 datatransport-3.0.5/src/datatransport/metadata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10437 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/newspoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7928 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/newsposter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    33842 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/newstool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    15514 2023-07-09 19:28:31.000000 datatransport-3.0.5/src/datatransport/processclient.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    13288 2023-07-09 19:27:51.000000 datatransport-3.0.5/src/datatransport/processgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/root.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/templates/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/templates/etc/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/templates/etc/transportd.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/templates/groups/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/templates/groups/ServerMonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4679 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/templates/groups/ServerMonitor/watchdog.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.5/src/datatransport/transportconfig.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/transportlogger.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/transportmanager.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/transportserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport/utilities/
--rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/utilities/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/utilities/datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/utilities/makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4012 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/utilities/patterntemplate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/utilities/removefile.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/utilities/sizedesc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/utilities/xmlrpcdeferred.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4498 2023-07-07 20:20:45.000000 datatransport-3.0.5/src/datatransport/xmlrpcserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport.egg-info/
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport.egg-info/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)     6282 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport.egg-info/SOURCES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport.egg-info/dependency_links.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)     1330 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport.egg-info/entry_points.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport.egg-info/requires.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-10 06:31:27.000000 datatransport-3.0.5/src/datatransport.egg-info/top_level.txt
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-10 06:31:27.000000 datatransport-3.0.5/tests/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.5/tests/test_utilities_datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.5/tests/test_utilities_makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1443 2023-07-07 20:20:45.000000 datatransport-3.0.5/tests/test_utilities_pattern.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.5/tests/test_utilities_removefiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.5/tests/test_utilities_sizedesc.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    49678 2023-07-12 23:31:21.000000 datatransport-3.0.6/CHANGES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.6/INSTALL
+-rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.6/LICENSE
+-rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.6/MANIFEST.in
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.6/MIGRATION
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-13 20:00:21.000000 datatransport-3.0.6/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.6/README.rst
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/.coverage
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2351 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/archivegroups/archivegroups.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2340 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/component/component.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1759 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/environ/environ.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1098 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/environ/environ.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.6/contrib/examples/examples.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/filewatch/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1654 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/getbytes/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      896 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/hello/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.6/contrib/examples/hello/hello.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      799 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/hello/helloworld.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/init/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      973 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/init/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/init/init.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/messagebox/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/messagebox.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/poll_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/poll_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/post_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/post_text.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/postpoll/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1009 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/poll_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      836 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/poll_text.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1125 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/post_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      957 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/post_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/postpoll.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/rotatelogs/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      861 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/service/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1175 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/client.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/directory.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/echo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/service.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/spawn/spawn.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1284 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/watchdog/
+-rwxr-xr-x   0 valentic   (500) valentic   (500)     1054 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/watchdog/crasher.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/watchdog/init_crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/README
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/archivegroups/archivegroups.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/component/component.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/config/config.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/config/config.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/diskmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/diskmonitor/diskmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/environ/environ.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/environ/environ.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/eventmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/eventmonitor/eventmonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/eventmonitor/serverstate.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/filewatch/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/getbytes/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/plugin.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/postdata
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/README
+-rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/multipoll.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/reader.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/writer.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/newsgroupmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/plottool/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/plottool/datasource.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/plottool/plottool.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/checkdate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/postdatafiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/resourcemonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/rotatelogs/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/spawn/spawn.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/splitfiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/splitfiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/splitfiles/splitfiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/poller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/source.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/syncpoller.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/test.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/wait/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/wait/timer.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/wait/wait.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/watchdog/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/watchdog/crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/utils/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/createnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/getarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/postarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/rebuilddatabase
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/relaynewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/rmnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/watchtransport
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2611 2023-07-10 06:31:17.000000 datatransport-3.0.6/pyproject.toml
+-rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-13 20:00:21.000000 datatransport-3.0.6/setup.cfg
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1584 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/accessmixin.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/commands/
+-rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/cancelnewsgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/console.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/listnewsgroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transport_create_app.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transportctl.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transportd.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transportps.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7918 2023-07-12 23:39:58.000000 datatransport-3.0.6/src/datatransport/commands/viewlog.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/components/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    50983 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/ArchiveGroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2405 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/DirectoryService.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5325 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/DiskMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6212 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/EventMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4130 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/FilePost.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     9573 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/FileStore.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5460 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/FileWatch.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5213 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/GroupControl.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/InstrumentStatus.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4364 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/NewsGateway.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7859 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/NewsgroupMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/PageKit.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/PlotTool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    12588 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/PostDataFiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/RealTimeFeed.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/ResourceMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6851 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/Scheduler.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/SyncPoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11920 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/WatchURL.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      645 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1335 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/configcomponent.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3058 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/directory.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-12 23:30:41.000000 datatransport-3.0.6/src/datatransport/metadata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10437 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/newspoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7928 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/newsposter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    33842 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/newstool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    15514 2023-07-09 19:28:31.000000 datatransport-3.0.6/src/datatransport/processclient.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    13288 2023-07-09 19:27:51.000000 datatransport-3.0.6/src/datatransport/processgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/root.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/etc/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/templates/etc/transportd.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/groups/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4679 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/watchdog.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.6/src/datatransport/transportconfig.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/transportlogger.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/transportmanager.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/transportserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/utilities/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4012 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/patterntemplate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/removefile.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/sizedesc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/xmlrpcdeferred.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4498 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/xmlrpcserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6282 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1330 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/entry_points.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/requires.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/top_level.txt
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/tests/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1443 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_pattern.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_removefiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_sizedesc.py
```

### Comparing `datatransport-3.0.5/CHANGES.txt` & `datatransport-3.0.6/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+2023-07-12  Todd Valentic
+    - Make sure viewlog opens new files
+    - Release 3.0.6
+
 2023-07-09  Todd Valentic
     - Add find_config_files() method to TransportConfig()
     - Allow hostname config files now on all configs
     - ProcessClient - use TransportConfig find_config_files 
     - ProcessGroup - use TransportConfig find_config_files 
-    - RElease 3.0.5
+    - Release 3.0.5
 
 2023-07-08  Todd Valentic
     - Major update to viewlog (parents and recursive views) 
     - Release 3.0.4
 
 2023-07-07  Todd Valentic
     - Initial public release of transport3
```

### Comparing `datatransport-3.0.5/INSTALL` & `datatransport-3.0.6/INSTALL`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/LICENSE` & `datatransport-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/MIGRATION` & `datatransport-3.0.6/MIGRATION`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/PKG-INFO` & `datatransport-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.5
+Version: 3.0.6
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.5/contrib/examples/.coverage` & `datatransport-3.0.6/contrib/examples/.coverage`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/archivegroups/archivegroups.conf` & `datatransport-3.0.6/contrib/examples/archivegroups/archivegroups.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/archivegroups/postdata.py` & `datatransport-3.0.6/contrib/examples/archivegroups/postdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/component/component.conf` & `datatransport-3.0.6/contrib/examples/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/component/demo.py` & `datatransport-3.0.6/contrib/examples/component/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/environ/environ.py` & `datatransport-3.0.6/contrib/examples/environ/environ.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/filewatch/createdata.py` & `datatransport-3.0.6/contrib/examples/filewatch/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/getbytes/demo.py` & `datatransport-3.0.6/contrib/examples/getbytes/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/getbytes/getbytes.conf` & `datatransport-3.0.6/contrib/examples/getbytes/getbytes.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/hello/helloworld.py` & `datatransport-3.0.6/contrib/examples/hello/helloworld.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/init/demo.py` & `datatransport-3.0.6/contrib/examples/init/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/messagebox/messagebox.conf` & `datatransport-3.0.6/contrib/examples/messagebox/messagebox.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/messagebox/poll_file.py` & `datatransport-3.0.6/contrib/examples/messagebox/poll_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/messagebox/poll_text.py` & `datatransport-3.0.6/contrib/examples/messagebox/poll_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/messagebox/post_file.py` & `datatransport-3.0.6/contrib/examples/messagebox/post_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/messagebox/post_text.py` & `datatransport-3.0.6/contrib/examples/messagebox/post_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/postpoll/poll_file.py` & `datatransport-3.0.6/contrib/examples/postpoll/poll_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/postpoll/poll_text.py` & `datatransport-3.0.6/contrib/examples/postpoll/poll_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/postpoll/post_file.py` & `datatransport-3.0.6/contrib/examples/postpoll/post_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/postpoll/post_text.py` & `datatransport-3.0.6/contrib/examples/postpoll/post_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/postpoll/postpoll.conf` & `datatransport-3.0.6/contrib/examples/postpoll/postpoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/rotatelogs/counter.py` & `datatransport-3.0.6/contrib/examples/rotatelogs/counter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/service/client.py` & `datatransport-3.0.6/contrib/examples/service/client.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/service/echo.py` & `datatransport-3.0.6/contrib/examples/service/echo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/service/service.conf` & `datatransport-3.0.6/contrib/examples/service/service.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/spawn/spawner.py` & `datatransport-3.0.6/contrib/examples/spawn/spawner.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/watchdog/crasher.py` & `datatransport-3.0.6/contrib/examples/watchdog/crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples/watchdog/init_crasher.py` & `datatransport-3.0.6/contrib/examples/watchdog/init_crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/README` & `datatransport-3.0.6/contrib/examples.v2/README`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/archivegroups/archivegroups.conf` & `datatransport-3.0.6/contrib/examples.v2/archivegroups/archivegroups.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/archivegroups/postdata.py` & `datatransport-3.0.6/contrib/examples.v2/archivegroups/postdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/component/component.conf` & `datatransport-3.0.6/contrib/examples.v2/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/component/demo.py` & `datatransport-3.0.6/contrib/examples.v2/component/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/config/config.py` & `datatransport-3.0.6/contrib/examples.v2/config/config.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/environ/environ.py` & `datatransport-3.0.6/contrib/examples.v2/environ/environ.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/eventmonitor/eventmonitor.conf` & `datatransport-3.0.6/contrib/examples.v2/eventmonitor/eventmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/eventmonitor/serverstate.py` & `datatransport-3.0.6/contrib/examples.v2/eventmonitor/serverstate.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/filewatch/createdata.py` & `datatransport-3.0.6/contrib/examples.v2/filewatch/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/getbytes/demo.py` & `datatransport-3.0.6/contrib/examples.v2/getbytes/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/instrumentstatus/instrumentstatus.conf` & `datatransport-3.0.6/contrib/examples.v2/instrumentstatus/instrumentstatus.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/instrumentstatus/postdata` & `datatransport-3.0.6/contrib/examples.v2/instrumentstatus/postdata`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/multipoll/multipoll.conf` & `datatransport-3.0.6/contrib/examples.v2/multipoll/multipoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/multipoll/writer.py` & `datatransport-3.0.6/contrib/examples.v2/multipoll/writer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf` & `datatransport-3.0.6/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/plottool/datasource.py` & `datatransport-3.0.6/contrib/examples.v2/plottool/datasource.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/plottool/plottool.conf` & `datatransport-3.0.6/contrib/examples.v2/plottool/plottool.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/postdatafiles/createfiles.py` & `datatransport-3.0.6/contrib/examples.v2/postdatafiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/postdatafiles/postdatafiles.conf` & `datatransport-3.0.6/contrib/examples.v2/postdatafiles/postdatafiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/rotatelogs/counter.py` & `datatransport-3.0.6/contrib/examples.v2/rotatelogs/counter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/spawn/spawner.py` & `datatransport-3.0.6/contrib/examples.v2/spawn/spawner.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/splitfiles/createfiles.py` & `datatransport-3.0.6/contrib/examples.v2/splitfiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/splitfiles/splitfiles.conf` & `datatransport-3.0.6/contrib/examples.v2/splitfiles/splitfiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/syncpoller/source.py` & `datatransport-3.0.6/contrib/examples.v2/syncpoller/source.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/syncpoller/syncpoller.conf` & `datatransport-3.0.6/contrib/examples.v2/syncpoller/syncpoller.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/wait/timer.py` & `datatransport-3.0.6/contrib/examples.v2/wait/timer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/examples.v2/watchdog/crasher.py` & `datatransport-3.0.6/contrib/examples.v2/watchdog/crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/utils/createnewsgroup` & `datatransport-3.0.6/contrib/utils/createnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/utils/getarticle` & `datatransport-3.0.6/contrib/utils/getarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/utils/postarticle` & `datatransport-3.0.6/contrib/utils/postarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/utils/rebuilddatabase` & `datatransport-3.0.6/contrib/utils/rebuilddatabase`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/utils/relaynewsgroup` & `datatransport-3.0.6/contrib/utils/relaynewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/utils/rmnewsgroup` & `datatransport-3.0.6/contrib/utils/rmnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/contrib/utils/watchtransport` & `datatransport-3.0.6/contrib/utils/watchtransport`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/pyproject.toml` & `datatransport-3.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/__init__.py` & `datatransport-3.0.6/src/datatransport/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/accessmixin.py` & `datatransport-3.0.6/src/datatransport/accessmixin.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/cancelnewsgroup.py` & `datatransport-3.0.6/src/datatransport/commands/cancelnewsgroup.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/console.py` & `datatransport-3.0.6/src/datatransport/commands/console.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/listnewsgroups.py` & `datatransport-3.0.6/src/datatransport/commands/listnewsgroups.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/transport_create_app.py` & `datatransport-3.0.6/src/datatransport/commands/transport_create_app.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/transportctl.py` & `datatransport-3.0.6/src/datatransport/commands/transportctl.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/transportd.py` & `datatransport-3.0.6/src/datatransport/commands/transportd.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/transportps.py` & `datatransport-3.0.6/src/datatransport/commands/transportps.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/commands/viewlog.py` & `datatransport-3.0.6/src/datatransport/commands/viewlog.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,31 +209,32 @@
             result[key] = tracker
 
         return result
 
     def run(self):
         """Print the last 10 lines of each file, sort by time"""
 
-        paths = self.scan_groups(self.specs)
-
         if self.verbose:
+            paths = self.scan_groups(self.specs)
+
             print("=" * 75)
             print(f"Looking in {self.specs}")
             if self.args.parents is None:
                 print("Parents: all")
             else:
                 print(f"Parents: {self.args.parents}")
-            print(f"Total lots: {len(paths)}")
+            print(f"Total log files: {len(paths)}")
             for path in paths:
                 print(path)
             print("=" * 75)
 
         # Tail forever
 
         while True:
+            paths = self.scan_groups(self.specs)
             self.trackers = self.update_trackers(self.trackers, paths)
 
             lines = []
             for tracker in self.trackers.values():
                 output = tracker.poll()
                 if not output:
                     continue
```

### Comparing `datatransport-3.0.5/src/datatransport/components/ArchiveGroups.py` & `datatransport-3.0.6/src/datatransport/components/ArchiveGroups.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/DirectoryService.py` & `datatransport-3.0.6/src/datatransport/components/DirectoryService.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/DiskMonitor.py` & `datatransport-3.0.6/src/datatransport/components/DiskMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/EventMonitor.py` & `datatransport-3.0.6/src/datatransport/components/EventMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/FilePost.py` & `datatransport-3.0.6/src/datatransport/components/FilePost.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/FileStore.py` & `datatransport-3.0.6/src/datatransport/components/FileStore.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/FileWatch.py` & `datatransport-3.0.6/src/datatransport/components/FileWatch.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/GroupControl.py` & `datatransport-3.0.6/src/datatransport/components/GroupControl.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/InstrumentStatus.py` & `datatransport-3.0.6/src/datatransport/components/InstrumentStatus.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/NewsGateway.py` & `datatransport-3.0.6/src/datatransport/components/NewsGateway.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/NewsgroupMonitor.py` & `datatransport-3.0.6/src/datatransport/components/NewsgroupMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/PageKit.py` & `datatransport-3.0.6/src/datatransport/components/PageKit.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/PlotTool.py` & `datatransport-3.0.6/src/datatransport/components/PlotTool.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/PostDataFiles.py` & `datatransport-3.0.6/src/datatransport/components/PostDataFiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/RealTimeFeed.py` & `datatransport-3.0.6/src/datatransport/components/RealTimeFeed.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/ResourceMonitor.py` & `datatransport-3.0.6/src/datatransport/components/ResourceMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/Scheduler.py` & `datatransport-3.0.6/src/datatransport/components/Scheduler.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/SyncPoller.py` & `datatransport-3.0.6/src/datatransport/components/SyncPoller.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/WatchURL.py` & `datatransport-3.0.6/src/datatransport/components/WatchURL.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/components/__init__.py` & `datatransport-3.0.6/src/datatransport/components/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/configcomponent.py` & `datatransport-3.0.6/src/datatransport/configcomponent.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/directory.py` & `datatransport-3.0.6/src/datatransport/directory.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/newspoller.py` & `datatransport-3.0.6/src/datatransport/newspoller.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/newsposter.py` & `datatransport-3.0.6/src/datatransport/newsposter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/newstool.py` & `datatransport-3.0.6/src/datatransport/newstool.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/processclient.py` & `datatransport-3.0.6/src/datatransport/processclient.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/processgroup.py` & `datatransport-3.0.6/src/datatransport/processgroup.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/templates/etc/transportd.conf` & `datatransport-3.0.6/src/datatransport/templates/etc/transportd.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/templates/groups/ServerMonitor/watchdog.py` & `datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/watchdog.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/transportconfig.py` & `datatransport-3.0.6/src/datatransport/transportconfig.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/transportlogger.py` & `datatransport-3.0.6/src/datatransport/transportlogger.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/transportmanager.py` & `datatransport-3.0.6/src/datatransport/transportmanager.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/transportserver.py` & `datatransport-3.0.6/src/datatransport/transportserver.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/utilities/datefunc.py` & `datatransport-3.0.6/src/datatransport/utilities/datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/utilities/makepath.py` & `datatransport-3.0.6/src/datatransport/utilities/makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/utilities/patterntemplate.py` & `datatransport-3.0.6/src/datatransport/utilities/patterntemplate.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/utilities/removefile.py` & `datatransport-3.0.6/src/datatransport/utilities/removefile.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/utilities/sizedesc.py` & `datatransport-3.0.6/src/datatransport/utilities/sizedesc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/utilities/xmlrpcdeferred.py` & `datatransport-3.0.6/src/datatransport/utilities/xmlrpcdeferred.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport/xmlrpcserver.py` & `datatransport-3.0.6/src/datatransport/xmlrpcserver.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport.egg-info/PKG-INFO` & `datatransport-3.0.6/src/datatransport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.5
+Version: 3.0.6
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.5/src/datatransport.egg-info/SOURCES.txt` & `datatransport-3.0.6/src/datatransport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/src/datatransport.egg-info/entry_points.txt` & `datatransport-3.0.6/src/datatransport.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/tests/test_utilities_datefunc.py` & `datatransport-3.0.6/tests/test_utilities_datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/tests/test_utilities_makepath.py` & `datatransport-3.0.6/tests/test_utilities_makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/tests/test_utilities_pattern.py` & `datatransport-3.0.6/tests/test_utilities_pattern.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/tests/test_utilities_removefiles.py` & `datatransport-3.0.6/tests/test_utilities_removefiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.5/tests/test_utilities_sizedesc.py` & `datatransport-3.0.6/tests/test_utilities_sizedesc.py`

 * *Files identical despite different names*


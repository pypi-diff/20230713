# Comparing `tmp/trio-0.8.0.tar.gz` & `tmp/trio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trio-0.8.0.tar", last modified: Mon Oct  1 02:57:15 2018, max compression
+gzip compressed data, was "dist/trio-0.9.0.tar", last modified: Sat Oct 13 07:14:15 2018, max compression
```

## Comparing `trio-0.8.0.tar` & `trio-0.9.0.tar`

### file list

```diff
@@ -1,166 +1,238 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/
--rw-r--r--   0 smurf      (501) smurf      (501)     1046 2018-04-23 11:56:26.000000 trio-0.8.0/LICENSE.MIT
--rw-r--r--   0 smurf      (501) smurf      (501)    10050 2018-09-04 11:49:29.000000 trio-0.8.0/README.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1748 2018-10-01 01:19:41.000000 trio-0.8.0/test-requirements.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       38 2018-10-01 02:57:15.000000 trio-0.8.0/setup.cfg
--rw-r--r--   0 smurf      (501) smurf      (501)    11358 2018-04-23 11:56:26.000000 trio-0.8.0/LICENSE.APACHE2
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/docs/
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/docs/source/
--rw-r--r--   0 smurf      (501) smurf      (501)     1203 2018-09-12 19:13:14.000000 trio-0.8.0/docs/source/releasing.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      449 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/glossary.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/docs/source/reference-testing/
--rw-r--r--   0 smurf      (501) smurf      (501)     1628 2018-10-01 01:19:41.000000 trio-0.8.0/docs/source/reference-testing/across-realtime.py
--rw-r--r--   0 smurf      (501) smurf      (501)      832 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/reference-testing/across-realtime.out
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/docs/source/tutorial/
--rw-r--r--   0 smurf      (501) smurf      (501)     1949 2018-04-30 12:36:22.000000 trio-0.8.0/docs/source/tutorial/echo-server.py
--rw-r--r--   0 smurf      (501) smurf      (501)      693 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/tutorial/tasks-intro.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2021 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/tutorial/tasks-with-trace.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1370 2018-04-30 12:36:22.000000 trio-0.8.0/docs/source/tutorial/echo-client.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/docs/source/_templates/
--rw-r--r--   0 smurf      (501) smurf      (501)      848 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_templates/layout.html
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_templates/.gitkeep
--rw-r--r--   0 smurf      (501) smurf      (501)     7134 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/reference-testing.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/docs/source/reference-core/
--rw-r--r--   0 smurf      (501) smurf      (501)     1285 2018-04-30 12:36:22.000000 trio-0.8.0/docs/source/reference-core/contextvar-example.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7161 2018-07-04 02:55:04.000000 trio-0.8.0/docs/source/conf.py
--rw-r--r--   0 smurf      (501) smurf      (501)    60697 2018-10-01 01:19:41.000000 trio-0.8.0/docs/source/reference-core.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    24376 2018-10-01 01:20:41.000000 trio-0.8.0/docs/source/history.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    23321 2018-10-01 01:19:41.000000 trio-0.8.0/docs/source/reference-io.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      646 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/local_customization.py
--rw-r--r--   0 smurf      (501) smurf      (501)    20586 2018-10-01 01:19:41.000000 trio-0.8.0/docs/source/reference-hazmat.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/docs/source/_static/
--rw-r--r--   0 smurf      (501) smurf      (501)     4286 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_static/favicon-32.ico
--rw-r--r--   0 smurf      (501) smurf      (501)    10895 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_static/ornament.svg
--rw-r--r--   0 smurf      (501) smurf      (501)     9962 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_static/favicon.svg
--rw-r--r--   0 smurf      (501) smurf      (501)     1834 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_static/favicon-32.png
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_static/.gitkeep
--rw-r--r--   0 smurf      (501) smurf      (501)     3437 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/_static/hackrtd.css
--rw-r--r--   0 smurf      (501) smurf      (501)     3521 2018-09-04 11:49:29.000000 trio-0.8.0/docs/source/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    25245 2018-09-04 11:49:29.000000 trio-0.8.0/docs/source/design.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    23683 2018-09-04 11:49:29.000000 trio-0.8.0/docs/source/contributing.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    10903 2018-04-23 11:56:26.000000 trio-0.8.0/docs/source/code-of-conduct.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    48056 2018-10-01 01:19:41.000000 trio-0.8.0/docs/source/tutorial.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      647 2018-04-23 11:56:26.000000 trio-0.8.0/docs/notes.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      812 2018-04-23 11:56:26.000000 trio-0.8.0/docs/make.bat
--rw-r--r--   0 smurf      (501) smurf      (501)      605 2018-04-23 11:56:26.000000 trio-0.8.0/docs/Makefile
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)      134 2018-10-01 02:57:15.000000 trio-0.8.0/trio.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     4208 2018-10-01 02:57:15.000000 trio-0.8.0/trio.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        5 2018-10-01 02:57:15.000000 trio-0.8.0/trio.egg-info/top_level.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2018-10-01 02:57:15.000000 trio-0.8.0/trio.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     4354 2018-10-01 02:57:15.000000 trio-0.8.0/trio.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)      228 2018-04-23 11:56:26.000000 trio-0.8.0/MANIFEST.in
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/
--rw-r--r--   0 smurf      (501) smurf      (501)     5569 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_path.py
--rw-r--r--   0 smurf      (501) smurf      (501)    33295 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_sync.py
--rw-r--r--   0 smurf      (501) smurf      (501)    16326 2018-07-04 02:55:04.000000 trio-0.8.0/trio/_threads.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6137 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_highlevel_ssl_helpers.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1240 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_highlevel_open_unix_stream.py
--rw-r--r--   0 smurf      (501) smurf      (501)    14209 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_highlevel_open_tcp_stream.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2079 2018-10-01 01:19:41.000000 trio-0.8.0/trio/socket.py
--rw-r--r--   0 smurf      (501) smurf      (501)    14379 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_highlevel_socket.py
--rw-r--r--   0 smurf      (501) smurf      (501)    18910 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_abc.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4175 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_subprocess.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3972 2018-07-04 02:55:04.000000 trio-0.8.0/trio/_timeouts.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2073 2018-09-04 11:49:29.000000 trio-0.8.0/trio/hazmat.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3936 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_highlevel_generic.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4814 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_file_io.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4645 2018-09-12 19:13:23.000000 trio-0.8.0/trio/_deprecate.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8208 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_util.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4326 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_highlevel_serve_listeners.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4070 2018-10-01 01:19:41.000000 trio-0.8.0/trio/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2197 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_wait_for_object.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)     1337 2018-04-30 12:36:22.000000 trio-0.8.0/trio/tests/test_highlevel_open_unix_stream.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4466 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_highlevel_serve_listeners.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8092 2018-08-30 17:25:25.000000 trio-0.8.0/trio/tests/test_wait_for_object.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5198 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_path.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7744 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_signals.py
--rw-r--r--   0 smurf      (501) smurf      (501)    15025 2018-04-23 11:56:26.000000 trio-0.8.0/trio/tests/test_threads.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8831 2018-09-04 11:49:29.000000 trio-0.8.0/trio/tests/test_highlevel_socket.py
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.8.0/trio/tests/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/tests/subprocess/
--rw-r--r--   0 smurf      (501) smurf      (501)     1140 2018-09-12 19:13:23.000000 trio-0.8.0/trio/tests/subprocess/test_waitpid_linux.py
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-09-04 11:49:29.000000 trio-0.8.0/trio/tests/subprocess/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3839 2018-09-04 11:49:29.000000 trio-0.8.0/trio/tests/subprocess/test_unix_pipes.py
--rw-r--r--   0 smurf      (501) smurf      (501)      985 2018-04-23 11:56:26.000000 trio-0.8.0/trio/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5047 2018-04-23 11:56:26.000000 trio-0.8.0/trio/tests/test_file_io.py
--rw-r--r--   0 smurf      (501) smurf      (501)    24726 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_testing.py
--rw-r--r--   0 smurf      (501) smurf      (501)      447 2018-04-23 11:56:26.000000 trio-0.8.0/trio/tests/test_abc.py
--rw-r--r--   0 smurf      (501) smurf      (501)      708 2018-04-23 11:56:26.000000 trio-0.8.0/trio/tests/module_with_deprecations.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6388 2018-04-30 12:36:22.000000 trio-0.8.0/trio/tests/test_deprecate.py
--rw-r--r--   0 smurf      (501) smurf      (501)    13928 2018-09-04 11:49:29.000000 trio-0.8.0/trio/tests/test_highlevel_open_tcp_stream.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8383 2018-07-04 02:55:04.000000 trio-0.8.0/trio/tests/test_highlevel_open_tcp_listeners.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3335 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_timeouts.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2674 2018-04-23 11:56:26.000000 trio-0.8.0/trio/tests/test_highlevel_generic.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1667 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_exports.py
--rw-r--r--   0 smurf      (501) smurf      (501)    31391 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_socket.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3791 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_highlevel_ssl_helpers.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5143 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_util.py
--rw-r--r--   0 smurf      (501) smurf      (501)    20183 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_sync.py
--rw-r--r--   0 smurf      (501) smurf      (501)    43122 2018-10-01 01:19:41.000000 trio-0.8.0/trio/tests/test_ssl.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/_subprocess/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_subprocess/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1303 2018-09-12 19:13:23.000000 trio-0.8.0/trio/_subprocess/linux_waitpid.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3762 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_subprocess/unix_pipes.py
--rw-r--r--   0 smurf      (501) smurf      (501)      425 2018-04-23 11:56:26.000000 trio-0.8.0/trio/abc.py
--rw-r--r--   0 smurf      (501) smurf      (501)    28356 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_socket.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/_core/
--rw-r--r--   0 smurf      (501) smurf      (501)     7898 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/_ki.py
--rw-r--r--   0 smurf      (501) smurf      (501)    61906 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/_run.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5054 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/_io_epoll.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1283 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      769 2018-07-04 02:55:04.000000 trio-0.8.0/trio/_core/_result.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/_core/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)     1993 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_epoll.py
--rw-r--r--   0 smurf      (501) smurf      (501)      451 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_tutil.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/_core/tests/test_multierror_scripts/
--rw-r--r--   0 smurf      (501) smurf      (501)      364 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_multierror_scripts/custom_excepthook.py
--rw-r--r--   0 smurf      (501) smurf      (501)      155 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_multierror_scripts/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      342 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_multierror_scripts/simple_excepthook.py
--rw-r--r--   0 smurf      (501) smurf      (501)      172 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_multierror_scripts/simple_excepthook_IPython.py
--rw-r--r--   0 smurf      (501) smurf      (501)      171 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_multierror_scripts/_common.py
--rw-r--r--   0 smurf      (501) smurf      (501)      727 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_multierror_scripts/ipython_custom_exc.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2623 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_core/tests/test_local.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3986 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/tests/test_unbounded_queue.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1446 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/tutil.py
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)    18959 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/tests/test_ki.py
--rw-r--r--   0 smurf      (501) smurf      (501)      703 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)    64709 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/tests/test_run.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2638 2018-07-04 02:55:04.000000 trio-0.8.0/trio/_core/tests/test_result.py
--rw-r--r--   0 smurf      (501) smurf      (501)    18670 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/tests/test_multierror.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1350 2018-08-30 17:25:25.000000 trio-0.8.0/trio/_core/tests/test_windows.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8230 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/tests/test_io.py
--rw-r--r--   0 smurf      (501) smurf      (501)       14 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_util.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5853 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/tests/test_parking_lot.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4526 2018-04-23 11:56:26.000000 trio-0.8.0/trio/_core/_unbounded_queue.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6861 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_core/_traps.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2832 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_core/_local.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5410 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/_io_kqueue.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8331 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_core/_entry_queue.py
--rw-r--r--   0 smurf      (501) smurf      (501)    16141 2018-09-12 19:13:23.000000 trio-0.8.0/trio/_core/_multierror.py
--rw-r--r--   0 smurf      (501) smurf      (501)    15359 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/_io_windows.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1635 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_core/_wakeup_socketpair.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4531 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_core/_exceptions.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8485 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_core/_parking_lot.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4307 2018-08-30 17:25:25.000000 trio-0.8.0/trio/_core/_windows_cffi.py
--rw-r--r--   0 smurf      (501) smurf      (501)      425 2018-04-23 11:56:26.000000 trio-0.8.0/trio/ssl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6963 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_signals.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8448 2018-09-04 11:49:29.000000 trio-0.8.0/trio/_highlevel_open_tcp_listeners.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-01 02:57:15.000000 trio-0.8.0/trio/testing/
--rw-r--r--   0 smurf      (501) smurf      (501)     1178 2018-04-23 11:56:26.000000 trio-0.8.0/trio/testing/_network.py
--rw-r--r--   0 smurf      (501) smurf      (501)      875 2018-07-04 02:55:04.000000 trio-0.8.0/trio/testing/_trio_test.py
--rw-r--r--   0 smurf      (501) smurf      (501)      763 2018-09-12 19:13:23.000000 trio-0.8.0/trio/testing/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)    19671 2018-10-01 01:19:41.000000 trio-0.8.0/trio/testing/_check_streams.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8465 2018-10-01 01:19:41.000000 trio-0.8.0/trio/testing/_mock_clock.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2804 2018-09-12 19:13:23.000000 trio-0.8.0/trio/testing/_sequencer.py
--rw-r--r--   0 smurf      (501) smurf      (501)    21557 2018-10-01 01:19:41.000000 trio-0.8.0/trio/testing/_memory_streams.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1885 2018-09-12 19:13:23.000000 trio-0.8.0/trio/testing/_checkpoints.py
--rw-r--r--   0 smurf      (501) smurf      (501)       89 2018-10-01 02:57:02.000000 trio-0.8.0/trio/_version.py
--rw-r--r--   0 smurf      (501) smurf      (501)    41934 2018-10-01 01:19:41.000000 trio-0.8.0/trio/_ssl.py
--rw-r--r--   0 smurf      (501) smurf      (501)      190 2018-04-23 11:56:26.000000 trio-0.8.0/LICENSE
--rw-r--r--   0 smurf      (501) smurf      (501)       98 2018-04-23 11:56:26.000000 trio-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 smurf      (501) smurf      (501)       98 2018-04-23 11:56:26.000000 trio-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 smurf      (501) smurf      (501)     4354 2018-10-01 02:57:15.000000 trio-0.8.0/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     5004 2018-09-12 19:13:14.000000 trio-0.8.0/setup.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1046 2018-04-23 11:56:26.000000 trio-0.9.0/LICENSE.MIT
+-rw-r--r--   0 smurf      (501) smurf      (501)      905 2018-10-12 16:32:47.000000 trio-0.9.0/appveyor.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)     5501 2018-10-01 01:19:41.000000 trio-0.9.0/.style.yapf
+-rw-r--r--   0 smurf      (501) smurf      (501)    10050 2018-09-04 11:49:29.000000 trio-0.9.0/README.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1748 2018-10-12 16:32:47.000000 trio-0.9.0/test-requirements.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       38 2018-10-13 07:14:15.000000 trio-0.9.0/setup.cfg
+-rw-r--r--   0 smurf      (501) smurf      (501)    11358 2018-04-23 11:56:26.000000 trio-0.9.0/LICENSE.APACHE2
+-rw-r--r--   0 smurf      (501) smurf      (501)      692 2018-09-12 19:13:23.000000 trio-0.9.0/.gitignore
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/docs/
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/docs/source/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1203 2018-09-12 19:13:14.000000 trio-0.9.0/docs/source/releasing.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      449 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/glossary.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/docs/source/reference-testing/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1628 2018-10-01 01:19:41.000000 trio-0.9.0/docs/source/reference-testing/across-realtime.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      832 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/reference-testing/across-realtime.out
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/docs/source/tutorial/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1949 2018-04-30 12:36:22.000000 trio-0.9.0/docs/source/tutorial/echo-server.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      693 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/tutorial/tasks-intro.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2021 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/tutorial/tasks-with-trace.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1370 2018-04-30 12:36:22.000000 trio-0.9.0/docs/source/tutorial/echo-client.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/docs/source/_templates/
+-rw-r--r--   0 smurf      (501) smurf      (501)      848 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_templates/layout.html
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_templates/.gitkeep
+-rw-r--r--   0 smurf      (501) smurf      (501)     7134 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/reference-testing.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/docs/source/reference-core/
+-rw-r--r--   0 smurf      (501) smurf      (501)      924 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-core/channels-backpressure.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1285 2018-04-30 12:36:22.000000 trio-0.9.0/docs/source/reference-core/contextvar-example.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1226 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-core/channels-mpmc-fixed.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1426 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-core/blocking-trio-portal-example.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      797 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-core/channels-simple.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1083 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-core/channels-mpmc-broken.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      582 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-core/channels-shutdown.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7037 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/conf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    70417 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-core.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    25535 2018-10-12 16:35:23.000000 trio-0.9.0/docs/source/history.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    23867 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-io.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      646 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/local_customization.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    19123 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/reference-hazmat.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/docs/source/_static/
+-rw-r--r--   0 smurf      (501) smurf      (501)     4286 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_static/favicon-32.ico
+-rw-r--r--   0 smurf      (501) smurf      (501)    10895 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_static/ornament.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)     9962 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_static/favicon.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)     1834 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_static/favicon-32.png
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_static/.gitkeep
+-rw-r--r--   0 smurf      (501) smurf      (501)     3437 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/_static/hackrtd.css
+-rw-r--r--   0 smurf      (501) smurf      (501)     3521 2018-09-04 11:49:29.000000 trio-0.9.0/docs/source/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    25011 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/design.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    23683 2018-09-04 11:49:29.000000 trio-0.9.0/docs/source/contributing.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    10903 2018-04-23 11:56:26.000000 trio-0.9.0/docs/source/code-of-conduct.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    48004 2018-10-12 16:32:47.000000 trio-0.9.0/docs/source/tutorial.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      647 2018-04-23 11:56:26.000000 trio-0.9.0/docs/notes.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      812 2018-04-23 11:56:26.000000 trio-0.9.0/docs/make.bat
+-rw-r--r--   0 smurf      (501) smurf      (501)      605 2018-04-23 11:56:26.000000 trio-0.9.0/docs/Makefile
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)      142 2018-10-13 07:14:15.000000 trio-0.9.0/trio.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     6263 2018-10-13 07:14:15.000000 trio-0.9.0/trio.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        5 2018-10-13 07:14:15.000000 trio-0.9.0/trio.egg-info/top_level.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2018-10-13 07:14:15.000000 trio-0.9.0/trio.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     4354 2018-10-13 07:14:15.000000 trio-0.9.0/trio.egg-info/PKG-INFO
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/logo/
+-rw-r--r--   0 smurf      (501) smurf      (501)    14685 2018-04-23 11:56:26.000000 trio-0.9.0/logo/logo-with-background.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)    13938 2018-04-23 11:56:26.000000 trio-0.9.0/logo/logo-transparent-with-text.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)    12093 2018-04-23 11:56:26.000000 trio-0.9.0/logo/wordmark-with-background.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)    10002 2018-04-23 11:56:26.000000 trio-0.9.0/logo/logo-transparent-no-text.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)    24942 2018-04-23 11:56:26.000000 trio-0.9.0/logo/editable.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)    11268 2018-04-23 11:56:26.000000 trio-0.9.0/logo/wordmark-transparent.svg
+-rw-r--r--   0 smurf      (501) smurf      (501)     3224 2018-08-30 17:25:25.000000 trio-0.9.0/Jenkinsfile
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/notes-to-self/
+-rw-r--r--   0 smurf      (501) smurf      (501)     2053 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/time-wait-windows-exclusiveaddruse.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      737 2018-10-12 16:32:47.000000 trio-0.9.0/notes-to-self/thread-dispatch-bench.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1675 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/server.key
+-rw-r--r--   0 smurf      (501) smurf      (501)     1084 2018-09-04 11:49:29.000000 trio-0.9.0/notes-to-self/socketpair-buffering.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      938 2018-10-01 01:19:41.000000 trio-0.9.0/notes-to-self/file-read-latency.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3383 2018-07-04 02:55:04.000000 trio-0.9.0/notes-to-self/ntp-example.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1722 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/sslobject.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      987 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/measure-listen-backlog.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2064 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/reopen-pipe.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1449 2018-07-04 02:55:04.000000 trio-0.9.0/notes-to-self/blocking-read-hack.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      529 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/trivial-err.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      234 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/lots-of-tasks.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      104 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/trivial.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4183 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/tiny-thread-pool.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/notes-to-self/ssl-close-notify/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1989 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/ssl-close-notify/ssl2.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2576 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/ssl-close-notify/ssl-close-notify.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3808 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/ssl-close-notify/trio-test-1.pem
+-rw-r--r--   0 smurf      (501) smurf      (501)     1111 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/ssl-close-notify/trio-test-CA.pem
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/notes-to-self/ssl-handshake/
+-rw-r--r--   0 smurf      (501) smurf      (501)     3808 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/ssl-handshake/trio-test-1.pem
+-rw-r--r--   0 smurf      (501) smurf      (501)     1111 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/ssl-handshake/trio-test-CA.pem
+-rw-r--r--   0 smurf      (501) smurf      (501)     4250 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/ssl-handshake/ssl-handshake.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      809 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/atomic-local.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      925 2018-10-01 01:19:41.000000 trio-0.9.0/notes-to-self/schedule-timing.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      759 2018-10-12 16:32:47.000000 trio-0.9.0/notes-to-self/estimate-task-size.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1679 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/thread-closure-bug-demo.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3041 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/print-task-tree.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2279 2018-10-12 16:32:47.000000 trio-0.9.0/notes-to-self/graceful-shutdown-idea.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1743 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/server.orig.key
+-rw-r--r--   0 smurf      (501) smurf      (501)      956 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/server.csr
+-rw-r--r--   0 smurf      (501) smurf      (501)      615 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/windows-vm-notes.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      578 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/manual-signal-handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3709 2018-10-01 01:19:41.000000 trio-0.9.0/notes-to-self/proxy-benchmarks.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3424 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/time-wait.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      369 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/loopy.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1111 2018-04-23 11:56:26.000000 trio-0.9.0/notes-to-self/server.crt
+-rw-r--r--   0 smurf      (501) smurf      (501)     3095 2018-10-01 01:19:41.000000 trio-0.9.0/notes-to-self/wakeup-fd-racer.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      722 2018-09-12 19:13:23.000000 trio-0.9.0/mypy.ini
+-rw-r--r--   0 smurf      (501) smurf      (501)      228 2018-04-23 11:56:26.000000 trio-0.9.0/MANIFEST.in
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/
+-rw-r--r--   0 smurf      (501) smurf      (501)     5569 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_path.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    33460 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_sync.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    16326 2018-07-04 02:55:04.000000 trio-0.9.0/trio/_threads.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6137 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_highlevel_ssl_helpers.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1240 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_highlevel_open_unix_stream.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    14209 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_highlevel_open_tcp_stream.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2079 2018-10-01 01:19:41.000000 trio-0.9.0/trio/socket.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    14379 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_highlevel_socket.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    25986 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_abc.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4175 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_subprocess.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3972 2018-07-04 02:55:04.000000 trio-0.9.0/trio/_timeouts.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2073 2018-09-04 11:49:29.000000 trio-0.9.0/trio/hazmat.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3936 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_highlevel_generic.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4814 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_file_io.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4645 2018-09-12 19:13:23.000000 trio-0.9.0/trio/_deprecate.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8208 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_util.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4326 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_highlevel_serve_listeners.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4127 2018-10-12 16:32:47.000000 trio-0.9.0/trio/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2197 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_wait_for_object.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1337 2018-04-30 12:36:22.000000 trio-0.9.0/trio/tests/test_highlevel_open_unix_stream.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4465 2018-10-12 16:32:47.000000 trio-0.9.0/trio/tests/test_highlevel_serve_listeners.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8092 2018-08-30 17:25:25.000000 trio-0.9.0/trio/tests/test_wait_for_object.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5198 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_path.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7744 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_signals.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    15025 2018-04-23 11:56:26.000000 trio-0.9.0/trio/tests/test_threads.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8831 2018-09-04 11:49:29.000000 trio-0.9.0/trio/tests/test_highlevel_socket.py
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.9.0/trio/tests/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/tests/subprocess/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1140 2018-09-12 19:13:23.000000 trio-0.9.0/trio/tests/subprocess/test_waitpid_linux.py
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-09-04 11:49:29.000000 trio-0.9.0/trio/tests/subprocess/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3839 2018-09-04 11:49:29.000000 trio-0.9.0/trio/tests/subprocess/test_unix_pipes.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      985 2018-04-23 11:56:26.000000 trio-0.9.0/trio/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5047 2018-04-23 11:56:26.000000 trio-0.9.0/trio/tests/test_file_io.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    24726 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_testing.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      447 2018-04-23 11:56:26.000000 trio-0.9.0/trio/tests/test_abc.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      708 2018-04-23 11:56:26.000000 trio-0.9.0/trio/tests/module_with_deprecations.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    10477 2018-10-12 16:32:47.000000 trio-0.9.0/trio/tests/test_channel.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6388 2018-04-30 12:36:22.000000 trio-0.9.0/trio/tests/test_deprecate.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    13928 2018-09-04 11:49:29.000000 trio-0.9.0/trio/tests/test_highlevel_open_tcp_stream.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8383 2018-07-04 02:55:04.000000 trio-0.9.0/trio/tests/test_highlevel_open_tcp_listeners.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3335 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_timeouts.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2674 2018-04-23 11:56:26.000000 trio-0.9.0/trio/tests/test_highlevel_generic.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1667 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_exports.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    31391 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_socket.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3791 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_highlevel_ssl_helpers.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5143 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_util.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    22070 2018-10-12 16:32:47.000000 trio-0.9.0/trio/tests/test_sync.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    43122 2018-10-01 01:19:41.000000 trio-0.9.0/trio/tests/test_ssl.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/_subprocess/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_subprocess/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1303 2018-09-12 19:13:23.000000 trio-0.9.0/trio/_subprocess/linux_waitpid.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3762 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_subprocess/unix_pipes.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      425 2018-04-23 11:56:26.000000 trio-0.9.0/trio/abc.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    28356 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_socket.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/_core/
+-rw-r--r--   0 smurf      (501) smurf      (501)     7898 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/_ki.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    61906 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/_run.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5054 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/_io_epoll.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1297 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_core/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      769 2018-07-04 02:55:04.000000 trio-0.9.0/trio/_core/_result.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/_core/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1993 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_epoll.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      451 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_tutil.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/_core/tests/test_multierror_scripts/
+-rw-r--r--   0 smurf      (501) smurf      (501)      364 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_multierror_scripts/custom_excepthook.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      155 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_multierror_scripts/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      342 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_multierror_scripts/simple_excepthook.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      172 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_multierror_scripts/simple_excepthook_IPython.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      171 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_multierror_scripts/_common.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      727 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_multierror_scripts/ipython_custom_exc.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2623 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_core/tests/test_local.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4088 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_core/tests/test_unbounded_queue.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1446 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/tutil.py
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    18961 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_core/tests/test_ki.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      703 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    64709 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/tests/test_run.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2638 2018-07-04 02:55:04.000000 trio-0.9.0/trio/_core/tests/test_result.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    18670 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/tests/test_multierror.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1625 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_core/tests/test_windows.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8230 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/tests/test_io.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       14 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_util.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5853 2018-04-23 11:56:26.000000 trio-0.9.0/trio/_core/tests/test_parking_lot.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4718 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_core/_unbounded_queue.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6861 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_core/_traps.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2832 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_core/_local.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5410 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/_io_kqueue.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8331 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_core/_entry_queue.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    16141 2018-09-12 19:13:23.000000 trio-0.9.0/trio/_core/_multierror.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    15359 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_core/_io_windows.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1635 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_core/_wakeup_socketpair.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4760 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_core/_exceptions.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8485 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_core/_parking_lot.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4307 2018-08-30 17:25:25.000000 trio-0.9.0/trio/_core/_windows_cffi.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      425 2018-04-23 11:56:26.000000 trio-0.9.0/trio/ssl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     9510 2018-10-12 16:32:47.000000 trio-0.9.0/trio/_channel.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6963 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_signals.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8448 2018-09-04 11:49:29.000000 trio-0.9.0/trio/_highlevel_open_tcp_listeners.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/trio/testing/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1178 2018-04-23 11:56:26.000000 trio-0.9.0/trio/testing/_network.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      875 2018-07-04 02:55:04.000000 trio-0.9.0/trio/testing/_trio_test.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      763 2018-09-12 19:13:23.000000 trio-0.9.0/trio/testing/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    19671 2018-10-01 01:19:41.000000 trio-0.9.0/trio/testing/_check_streams.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8465 2018-10-01 01:19:41.000000 trio-0.9.0/trio/testing/_mock_clock.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2804 2018-09-12 19:13:23.000000 trio-0.9.0/trio/testing/_sequencer.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    21557 2018-10-01 01:19:41.000000 trio-0.9.0/trio/testing/_memory_streams.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1885 2018-09-12 19:13:23.000000 trio-0.9.0/trio/testing/_checkpoints.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       89 2018-10-13 07:13:54.000000 trio-0.9.0/trio/_version.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    41934 2018-10-01 01:19:41.000000 trio-0.9.0/trio/_ssl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      190 2018-04-23 11:56:26.000000 trio-0.9.0/LICENSE
+-rw-r--r--   0 smurf      (501) smurf      (501)       98 2018-04-23 11:56:26.000000 trio-0.9.0/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/newsfragments/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1065 2018-04-23 11:56:26.000000 trio-0.9.0/newsfragments/README.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-04-23 11:56:26.000000 trio-0.9.0/newsfragments/.gitkeep
+-rw-r--r--   0 smurf      (501) smurf      (501)      921 2018-10-01 01:19:41.000000 trio-0.9.0/check.sh
+-rw-r--r--   0 smurf      (501) smurf      (501)       98 2018-04-23 11:56:26.000000 trio-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 smurf      (501) smurf      (501)      505 2018-10-01 01:19:41.000000 trio-0.9.0/test-requirements.in
+-rw-r--r--   0 smurf      (501) smurf      (501)     1030 2018-05-25 01:53:55.000000 trio-0.9.0/pyproject.toml
+-rw-r--r--   0 smurf      (501) smurf      (501)      175 2018-04-23 11:56:26.000000 trio-0.9.0/.readthedocs.yml
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-10-13 07:14:15.000000 trio-0.9.0/ci/
+-rw-r--r--   0 smurf      (501) smurf      (501)      133 2018-10-01 01:19:41.000000 trio-0.9.0/ci/rtd-requirements.in
+-rwxr-xr-x   0 smurf      (501) smurf      (501)     2977 2018-10-12 16:32:47.000000 trio-0.9.0/ci/travis.sh
+-rw-r--r--   0 smurf      (501) smurf      (501)     1089 2018-10-12 16:32:47.000000 trio-0.9.0/ci/rtd-requirements.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     4354 2018-10-13 07:14:15.000000 trio-0.9.0/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     5042 2018-10-12 16:32:47.000000 trio-0.9.0/setup.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      916 2018-10-12 16:32:47.000000 trio-0.9.0/.travis.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      385 2018-04-23 11:56:26.000000 trio-0.9.0/.coveragerc
```

### Comparing `trio-0.8.0/LICENSE.MIT` & `trio-0.9.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/README.rst` & `trio-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/test-requirements.txt` & `trio-0.9.0/test-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,34 +14,34 @@
 cryptography==2.3.1       # via pyopenssl, trustme
 decorator==4.3.0          # via ipython, traitlets
 flake8==3.5.0
 idna==2.7                 # via cryptography, trustme
 ipython-genutils==0.2.0   # via traitlets
 ipython==7.0.1
 isort==4.3.4              # via pylint
-jedi==0.12.1
+jedi==0.13.1
 lazy-object-proxy==1.3.1  # via astroid
 mccabe==0.6.1             # via flake8, pylint
 more-itertools==4.3.0     # via pytest
 parso==0.3.1              # via jedi
 pexpect==4.6.0            # via ipython
 pickleshare==0.7.5        # via ipython
 pluggy==0.7.1             # via pytest
-prompt-toolkit==2.0.4     # via ipython
+prompt-toolkit==2.0.5     # via ipython
 ptyprocess==0.6.0         # via pexpect
 py==1.6.0                 # via pytest
 pycodestyle==2.3.1        # via flake8
 pycparser==2.19           # via cffi
 pyflakes==1.6.0           # via flake8
 pygments==2.2.0           # via ipython
 pylint==2.1.1
 pyopenssl==18.0.0
 pytest-cov==2.6.0
 pytest-faulthandler==1.5.0
-pytest==3.8.1
+pytest==3.8.2
 simplegeneric==0.8.1      # via ipython
 six==1.11.0               # via astroid, cryptography, more-itertools, prompt-toolkit, pyopenssl, pytest, traitlets
 traitlets==4.3.2          # via ipython
 trustme==0.4.0
 typed-ast==1.1.0 ; python_version < "3.7" and implementation_name == "cpython"
 wcwidth==0.1.7            # via prompt-toolkit
 wrapt==1.10.11            # via astroid
```

### Comparing `trio-0.8.0/LICENSE.APACHE2` & `trio-0.9.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/releasing.rst` & `trio-0.9.0/docs/source/releasing.rst`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/reference-testing/across-realtime.py` & `trio-0.9.0/docs/source/reference-testing/across-realtime.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/reference-testing/across-realtime.out` & `trio-0.9.0/docs/source/reference-testing/across-realtime.out`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/tutorial/echo-server.py` & `trio-0.9.0/docs/source/tutorial/echo-server.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/tutorial/tasks-intro.py` & `trio-0.9.0/docs/source/tutorial/tasks-intro.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/tutorial/tasks-with-trace.py` & `trio-0.9.0/docs/source/tutorial/tasks-with-trace.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/tutorial/echo-client.py` & `trio-0.9.0/docs/source/tutorial/echo-client.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/_templates/layout.html` & `trio-0.9.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/reference-testing.rst` & `trio-0.9.0/docs/source/reference-testing.rst`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/reference-core/contextvar-example.py` & `trio-0.9.0/docs/source/reference-core/contextvar-example.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/conf.py` & `trio-0.9.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,15 @@
     ("py:class", "CapacityLimiter-like object"),
     ("py:class", "bytes-like"),
     ("py:class", "None"),
     # Was removed but still shows up in changelog
     ("py:class", "trio.hazmat.RunLocal"),
     # trio.abc is documented at random places scattered throughout the docs
     ("py:mod", "trio.abc"),
-    # contextvars is added in 3.7, but the docs point to 3.6
-    # these two entries can be removed after 3.7 is released
-    ("py:mod", "contextvars"),
-    ("py:class", "contextvars.Context"),
+    ("py:class", "math.inf"),
 ]
 autodoc_inherit_docstrings = False
 
 # XX hack the RTD theme until
 #   https://github.com/rtfd/sphinx_rtd_theme/pull/382
 # is shipped (should be in the release after 0.2.4)
 # ...note that this has since grown to contain a bunch of other CSS hacks too
@@ -66,15 +63,15 @@
     'sphinx.ext.napoleon',
     'sphinxcontrib_trio',
     'local_customization',
 ]
 
 intersphinx_mapping = {
     "python": ('https://docs.python.org/3', None),
-    "outcome": ('https://outcome.readthedocs.org/en/latest/', None),
+    "outcome": ('https://outcome.readthedocs.io/en/latest/', None),
 }
 
 autodoc_member_order = "bysource"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
@@ -156,14 +153,15 @@
     # default is 2
     # show deeper nesting in the RTD theme's sidebar TOC
     # https://stackoverflow.com/questions/27669376/
     # I'm not 100% sure this actually does anything with our current
     # versions/settings...
     "navigation_depth": 4,
     "logo_only": True,
+    'prev_next_buttons_location': 'both'
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
```

### Comparing `trio-0.8.0/docs/source/reference-core.rst` & `trio-0.9.0/docs/source/reference-core.rst`

 * *Files 11% similar despite different names*

```diff
@@ -826,31 +826,31 @@
 them all concurrently, and returns the result from the one that
 finishes first::
 
    async def race(*async_fns):
        if not async_fns:
            raise ValueError("must pass at least one argument")
 
-       q = trio.Queue(1)
+       send_channel, receive_channel = trio.open_memory_channel(0)
 
        async def jockey(async_fn):
-           await q.put(await async_fn())
+           await send_channel.send(await async_fn())
 
        async with trio.open_nursery() as nursery:
            for async_fn in async_fns:
                nursery.start_soon(jockey, async_fn)
-           winner = await q.get()
+           winner = await receive_channel.receive()
            nursery.cancel_scope.cancel()
            return winner
 
 This works by starting a set of tasks which each try to run their
 function, and then report back the value it returns. The main task
-uses ``q.get()`` to wait for one to finish; as soon as the first task
-crosses the finish line, it cancels the rest, and then returns the
-winning value.
+uses ``receive_channel.receive`` to wait for one to finish; as soon as
+the first task crosses the finish line, it cancels the rest, and then
+returns the winning value.
 
 Here if one or more of the racing functions raises an unhandled
 exception then Trio's normal handling kicks in: it cancels the others
 and then propagates the exception. If you want different behavior, you
 can get that by adding a ``try`` block to the ``jockey`` function to
 catch exceptions and handle them however you like.
 
@@ -1187,19 +1187,19 @@
 * For operations that have a non-blocking variant, the blocking and
   non-blocking variants are different methods with names like ``X``
   and ``X_nowait``, respectively. (This is similar to
   :class:`queue.Queue`, but unlike most of the classes in
   :mod:`threading`.) We like this approach because it allows us to
   make the blocking version async and the non-blocking version sync.
 
-* When a non-blocking method cannot succeed (the queue is empty, the
-  lock is already held, etc.), then it raises
-  :exc:`trio.WouldBlock`. There's no equivalent to the
-  :exc:`queue.Empty` versus :exc:`queue.Full` distinction – we just
-  have the one exception that we use consistently.
+* When a non-blocking method cannot succeed (the channel is empty, the
+  lock is already held, etc.), then it raises :exc:`trio.WouldBlock`.
+  There's no equivalent to the :exc:`queue.Empty` versus
+  :exc:`queue.Full` distinction – we just have the one exception that
+  we use consistently.
 
 
 Fairness
 ~~~~~~~~
 
 These classes are all guaranteed to be "fair", meaning that when it
 comes time to choose who will be next to acquire a lock, get an item
@@ -1241,72 +1241,334 @@
 Broadcasting an event with :class:`Event`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: Event
    :members:
 
 
-.. _queue:
+.. _channels:
 
-Passing messages with :class:`Queue`
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Using channels to pass values between tasks
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-You can use :class:`Queue` objects to safely pass objects between
-tasks. Trio :class:`Queue` objects always have a bounded size. Here's
-a toy example to demonstrate why this is important. Suppose we have a
-queue with two producers and one consumer::
+*Channels* allow you to safely and conveniently send objects between
+different tasks. They're particularly useful for implementing
+producer/consumer patterns.
 
-   async def producer(queue):
-       while True:
-           await queue.put(1)
+The channel API is defined by the abstract base classes
+:class:`trio.abc.SendChannel` and :class:`trio.abc.ReceiveChannel`.
+You can use these to implement your own custom channels, that do
+things like pass objects between processes or over the network. But in
+many cases, you just want to pass objects between different tasks
+inside a single process, and for that you can use
+:func:`trio.open_memory_channel`:
 
-   async def consumer(queue):
-       while True:
-           print(await queue.get())
+.. autofunction:: open_memory_channel
 
-   async def main():
-       # This example won't work with Trio's actual Queue class, so
-       # imagine we have some sort of platonic ideal of an unbounded
-       # queue here:
-       queue = trio.HypotheticalQueue()
-       async with trio.open_nursery() as nursery:
-           # Two producers
-           nursery.start_soon(producer, queue)
-           nursery.start_soon(producer, queue)
-           # One consumer
-           nursery.start_soon(consumer, queue)
+.. note:: If you've used the :mod:`threading` or :mod:`asyncio`
+   modules, you may be familiar with :class:`queue.Queue` or
+   :class:`asyncio.Queue`. In Trio, :func:`open_memory_channel` is
+   what you use when you're looking for a queue. The main difference
+   is that Trio splits the classic queue interface up into two
+   objects. The advantage of this is that it makes it possible to put
+   the two ends in different processes, and that we can close the two
+   sides separately.
 
-   trio.run(main)
 
-If we naively cycle between these three tasks in round-robin style,
-then we put an item, then put an item, then get an item, then put an
-item, then put an item, then get an item, ... and since on each cycle
-we add two items to the queue but only remove one, then over time the
-queue size grows arbitrarily large, our latency is terrible, we run
-out of memory, it's just generally bad news all around.
-
-By placing an upper bound on our queue's size, we avoid this problem.
-If the queue gets too big, then it applies *backpressure*: ``put``
-blocks and forces the producers to slow down and wait until the
-consumer calls ``get``.
-
-You can also create a :class:`Queue` with size 0. In that case any
-task that calls ``put`` on the queue will wait until another task
-calls ``get`` on the same queue, and vice versa. This is similar to
-the behavior of `channels as described in the CSP model
-<https://en.wikipedia.org/wiki/Channel_(programming)>`__.
+A simple channel example
+++++++++++++++++++++++++
 
-.. autoclass:: Queue
-   :members:
+Here's a simple example of how to use channels:
+
+.. literalinclude:: reference-core/channels-simple.py
+
+If you run this, it prints:
+
+.. code-block:: none
+
+   got value "message 0"
+   got value "message 1"
+   got value "message 2"
+
+And then it hangs forever. (Use control-C to quit.)
+
+
+.. _channel-shutdown:
+
+Clean shutdown with channels
+++++++++++++++++++++++++++++
+
+Of course we don't generally like it when programs hang. What
+happened? The problem is that the producer sent 3 messages and then
+exited, but the consumer has no way to tell that the producer is gone:
+for all it knows, another message might be coming along any moment. So
+it hangs forever waiting for the 4th message.
+
+Here's a new version that fixes this: it produces the same output as
+the previous version, and then exits cleanly. The only change is the
+addition of ``async with`` blocks inside the producer and consumer:
+
+.. literalinclude:: reference-core/channels-shutdown.py
+   :emphasize-lines: 10,15
+
+The really important thing here is the producer's ``async with`` .
+When the producer exits, this closes the ``send_channel``, and that
+tells the consumer that no more messages are coming, so it can cleanly
+exit its ``async for`` loop. Then the program shuts down because both
+tasks have exited.
+
+We also added an ``async with`` to the consumer. This isn't as
+important, but can it help us catch mistakes or other problems. For
+example, suppose that the consumer exited early for some reason –
+maybe because of a bug. Then the producer would be sending messages
+into the void, and might get stuck indefinitely. But, if the consumer
+closes its ``receive_channel``, then the producer will get a
+:exc:`BrokenResourceError` to alert it that it should stop sending
+messages because no-one is listening.
+
+If you want to see the effect of the consumer exiting early, try
+adding a ``break`` statement to the ``async for`` loop – you should
+see a :exc:`BrokenResourceError` from the producer.
+
+
+.. _channel-mpmc:
+
+Managing multiple producers and/or multiple consumers
++++++++++++++++++++++++++++++++++++++++++++++++++++++
+
+You can also have multiple producers, and multiple consumers, all
+sharing the same channel. However, this makes shutdown a little more
+complicated.
+
+For example, consider this naive extension of our previous example,
+now with two producers and two consumers:
+
+.. literalinclude:: reference-core/channels-mpmc-broken.py
+
+The two producers, A and B, send 3 messages apiece. These are then
+randomly distributed between the two producers, X and Y. So we're
+hoping to see some output like:
+
+.. code-block:: none
+
+   consumer Y got value '0 from producer B'
+   consumer X got value '0 from producer A'
+   consumer Y got value '1 from producer A'
+   consumer Y got value '1 from producer B'
+   consumer X got value '2 from producer B'
+   consumer X got value '2 from producer A'
+
+However, on most runs, that's not what happens – the first part of the
+output is OK, and then when we get to the end the program crashes with
+:exc:`ClosedResourceError`. If you run the program a few times, you'll
+see that sometimes the traceback shows ``send`` crashing, and other
+times it shows ``receive`` crashing, and you might even find that on
+some runs it doesn't crash at all.
+
+Here's what's happening: suppose that producer A finishes first. It
+exits, and its ``async with`` block closes the ``send_channel``. But
+wait! Producer B was still using that ``send_channel``... so the next
+time B calls ``send``, it gets a :exc:`ClosedResourceError`.
+
+Sometimes, though if we're lucky, the two producers might finish at
+the same time (or close enough), so they both make their last ``send``
+before either of them closes the ``send_channel``.
+
+But, even if that happens, we're not out of the woods yet! After the
+producers exit, the two consumers race to be the first to notice that
+the ``send_channel`` has closed. Suppose that X wins the race. It
+exits its ``async for`` loop, then exits the ``async with`` block...
+and closes the ``receive_channel``, while Y is still using it. Again,
+this causes a crash.
+
+We could avoid this by using some complicated bookkeeping to make sure
+that only the *last* producer and the *last* consumer close their
+channel endpoints... but that would be tiresome and fragile.
+Fortunately, there's a better way! Here's a fixed version of our
+program above:
+
+.. literalinclude:: reference-core/channels-mpmc-fixed.py
+   :emphasize-lines: 7, 9, 10, 12, 13
+
+This example demonstrates using the :meth:`SendChannel.clone
+<trio.abc.SendChannel.clone>` and :meth:`ReceiveChannel.clone
+<trio.abc.ReceiveChannel.clone>` methods. What these do is create
+copies of our endpoints, that act just like the original – except that
+they can be closed independently. And the underlying channel is only
+closed after *all* the clones have been closed. So this completely
+solves our problem with shutdown, and if you run this program, you'll
+see it print its six lines of output and then exits cleanly.
+
+Notice a small trick we use: the code in ``main`` creates clone
+objects to pass into all the child tasks, and then closes the original
+objects using ``async with``. Another option is to pass clones into
+all-but-one of the child tasks, and then pass the original object into
+the last task, like::
+
+   # Also works, but is more finicky:
+   send_channel, receive_channel = trio.open_memory_channel(0)
+   nursery.start_soon(producer, "A", send_channel.clone())
+   nursery.start_soon(producer, "B", send_channel)
+   nursery.start_soon(consumer, "X", receive_channel.clone())
+   nursery.start_soon(consumer, "Y", receive_channel)
+
+But this is more error-prone, especially if you use a loop to spawn
+the producers/consumers.
+
+Just make sure that you don't write::
+
+   # Broken, will cause program to hang:
+   send_channel, receive_channel = trio.open_memory_channel(0)
+   nursery.start_soon(producer, "A", send_channel.clone())
+   nursery.start_soon(producer, "B", send_channel.clone())
+   nursery.start_soon(consumer, "X", receive_channel.clone())
+   nursery.start_soon(consumer, "Y", receive_channel.clone())
+
+Here we pass clones into the tasks, but never close the original
+objects. That means we have 3 send channel objects (the original + two
+clones), but we only close 2 of them, so the consumers will hang
+around forever waiting for that last one to be closed.
+
+
+.. _channel-buffering:
+
+Buffering in channels
++++++++++++++++++++++
+
+When you call :func:`open_memory_channel`, you have to specify how
+many values can be buffered internally in the channel. If the buffer
+is full, then any task that calls :meth:`~trio.abc.SendChannel.send`
+will stop and wait for another task to call
+:meth:`~trio.abc.ReceiveChannel.receive`. This is useful because it
+produces *backpressure*: if the channel producers are running faster
+than the consumers, then it forces the producers to slow down.
+
+You can disable buffering entirely, by doing
+``open_memory_channel(0)``. In that case any task calls
+:meth:`~trio.abc.SendChannel.send` will wait until another task calls
+:meth:`~trio.abc.ReceiveChannel.receive`, and vice versa. This is similar to
+how channels work in the `classic Communicating Sequential Processes
+model <https://en.wikipedia.org/wiki/Channel_(programming)>`__, and is
+a reasonable default if you aren't sure what size buffer to use.
+(That's why we used it in the examples above.)
+
+At the other extreme, you can make the buffer unbounded by using
+``open_memory_channel(math.inf)``. In this case,
+:meth:`~trio.abc.SendChannel.send` *always* returns immediately.
+Normally, this is a bad idea. To see why, consider a program where the
+producer runs more quickly than the consumer:
+
+.. literalinclude:: reference-core/channels-backpressure.py
+
+If you run this program, you'll see output like:
+
+.. code-block:: none
+
+   Sent message: 0
+   Received message: 0
+   Sent message: 1
+   Sent message: 2
+   Sent message: 3
+   Sent message: 4
+   Sent message: 5
+   Sent message: 6
+   Sent message: 7
+   Sent message: 8
+   Sent message: 9
+   Received message: 1
+   Sent message: 10
+   Sent message: 11
+   Sent message: 12
+   ...
+
+On average, the producer sends ten messages per second, but the
+consumer only calls ``receive`` once per second. That means that each
+second, the channel's internal buffer has to grow to hold an extra
+nine items. After a minute, the buffer will have ~540 items in it;
+after an hour, that grows to ~32,400. Eventually, the program will run
+out of memory. And well before we run out of memory, our latency on
+handling individual messages will become abysmal. For example, at the
+one minute mark, the producer is sending message ~600, but the
+producer is still processing message ~60. Message 600 will have to sit
+in the channel for ~9 minutes before the consumer catches up and
+processes it.
+
+Now try replacing ``open_memory_channel(math.inf)`` with
+``open_memory_channel(0)``, and run it again. We get output like:
+
+.. code-block:: none
+
+   Sent message: 0
+   Received message: 0
+   Received message: 1
+   Sent message: 1
+   Received message: 2
+   Sent message: 2
+   Sent message: 3
+   Received message: 3
+   ...
+
+Now the ``send`` calls wait for the ``receive`` calls to finish, which
+forces the producer to slow down to match the consumer's speed. (It
+might look strange that some values are reported as "Received" before
+they're reported as "Sent"; this happens because the actual
+send/receive happen at the same time, so which line gets printed first
+is random.)
+
+Now, let's try setting a small but nonzero buffer size, like
+``open_memory_channel(3)``. what do you think will happen?
+
+I get:
+
+.. code-block:: none
+
+   Sent message: 0
+   Received message: 0
+   Sent message: 1
+   Sent message: 2
+   Sent message: 3
+   Received message: 1
+   Sent message: 4
+   Received message: 2
+   Sent message: 5
+   ...
+
+So you can see that the producer runs ahead by 3 messages, and then
+stops to wait: when the consumer reads message 1, it sends message 4,
+then when the consumer reads message 2, it sends message 5, and so on.
+Once it reaches the steady state, this version acts just like our
+previous version where we set the buffer size to 0, except that it
+uses a bit more memory and each message sits in the buffer for a bit
+longer before being processed (i.e., the message latency is higher).
+
+Of course real producers and consumers are usually more complicated
+than this, and in some situations, a modest amount of buffering might
+improve throughput. But too much buffering wastes memory and increases
+latency, so if you want to tune your application you should experiment
+to see what value works best for you.
+
+**Why do we even support unbounded buffers then?** Good question!
+Despite everything we saw above, there are times when you actually do
+need an unbounded buffer. For example, consider a web crawler that
+uses a channel to keep track of all the URLs it still wants to crawl.
+Each crawler runs a loop where it takes a URL from the channel,
+fetches it, checks the HTML for outgoing links, and then adds the new
+URLs to the channel. This creates a *circular flow*, where each
+consumer is also a producer. In this case, if your channel buffer gets
+full, then the crawlers will block when they try to add new URLs to
+the channel, and if all the crawlers got blocked, then they aren't
+taking any URLs out of the channel, so they're stuck forever in a
+deadlock. Using an unbounded channel avoids this, because it means
+that :meth:`~trio.abc.SendChannel.send` never blocks.
 
 
 Lower-level synchronization primitives
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Personally, I find that events and queues are usually enough to
+Personally, I find that events and channels are usually enough to
 implement most things I care about, and lead to easier to read code
 than the lower-level primitives discussed in this section. But if you
 need them, they're here. (If you find yourself reaching for these
 because you're trying to implement a new higher-level synchronization
 primitive, then you might also want to check out the facilities in
 :mod:`trio.hazmat` for a more direct exposure of trio's underlying
 synchronization logic. All of classes discussed in this section are
@@ -1486,68 +1748,31 @@
 Getting back into the trio thread from another thread
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: BlockingTrioPortal
    :members:
 
 This will probably be clearer with an example. Here we demonstrate how
-to spawn a child thread, and then use a :class:`trio.Queue` to send
-messages between the thread and a trio task::
+to spawn a child thread, and then use a :ref:`memory channel
+<channels>` to send messages between the thread and a trio task:
 
-   import trio
-   import threading
-
-   def thread_fn(portal, request_queue, response_queue):
-       while True:
-           # Since we're in a thread, we can't call trio.Queue methods
-           # directly -- so we use our portal to call them.
-           request = portal.run(request_queue.get)
-           # We use 'None' as a request to quit
-           if request is not None:
-               response = request + 1
-               portal.run(response_queue.put, response)
-           else:
-               # acknowledge that we're shutting down, and then do it
-               portal.run(response_queue.put, None)
-               return
-
-   async def main():
-       portal = trio.BlockingTrioPortal()
-       request_queue = trio.Queue(1)
-       response_queue = trio.Queue(1)
-       thread = threading.Thread(
-           target=thread_fn,
-           args=(portal, request_queue, response_queue))
-       thread.start()
-
-       # prints "1"
-       await request_queue.put(0)
-       print(await response_queue.get())
-
-       # prints "2"
-       await request_queue.put(1)
-       print(await response_queue.get())
-
-       # prints "None"
-       await request_queue.put(None)
-       print(await response_queue.get())
-       thread.join()
-
-   trio.run(main)
+.. literalinclude:: reference-core/blocking-trio-portal-example.py
 
 
 Exceptions and warnings
 -----------------------
 
 .. autoexception:: Cancelled
 
 .. autoexception:: TooSlowError
 
 .. autoexception:: WouldBlock
 
+.. autoexception:: EndOfChannel
+
 .. autoexception:: BusyResourceError
 
 .. autoexception:: ClosedResourceError
 
 .. autoexception:: BrokenResourceError
 
 .. autoexception:: RunFinishedError
```

### Comparing `trio-0.8.0/docs/source/history.rst` & `trio-0.9.0/docs/source/history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,42 @@
 Release history
 ===============
 
 .. currentmodule:: trio
 
 .. towncrier release notes start
 
+Trio 0.9.0 (2018-10-12)
+-----------------------
+
+Features
+~~~~~~~~
+
+- New and improved APIs for inter-task communication:
+  :class:`trio.abc.SendChannel`, :class:`trio.abc.ReceiveChannel`, and
+  :func:`trio.open_memory_channel` (which replaces ``trio.Queue``). This
+  interface uses separate "send" and "receive" methods, for consistency with
+  other communication interfaces like :class:`~trio.abc.Stream`. Also, the two
+  objects can now be closed individually, making it much easier to gracefully
+  shut down a channel. Also, check out the nifty ``clone`` API to make it easy
+  to manage fan-in scenarios. Also, the API has been written to allow for
+  future channel-like objects that send objects across process boundaries.
+  Also, it supports unbounded buffering if you really need it. Also, help I
+  can't stop writing also. See :ref:`channels` for more details. (`#497
+  <https://github.com/python-trio/trio/issues/497>`__)
+
+
+Deprecations and Removals
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- ``trio.Queue`` and ``trio.hazmat.UnboundedQueue`` have been deprecated, in
+  favor of :func:`trio.open_memory_channel`. (`#497
+  <https://github.com/python-trio/trio/issues/497>`__)
+
+
 Trio 0.8.0 (2018-10-01)
 -----------------------
 
 Features
 ~~~~~~~~
 
 - Trio's default internal clock is now based on :func:`time.perf_counter`
@@ -135,15 +163,15 @@
   :func:`trio.hazmat.wait_readable`, you should make sure to call these
   functions at appropriate times. (`#36
   <https://github.com/python-trio/trio/issues/36>`__)
 - Tasks created by :func:`~trio.hazmat.spawn_system_task` now no longer inherit
   the creator's :mod:`contextvars` context, instead using one created at
   :func:`~trio.run`. (`#289
   <https://github.com/python-trio/trio/issues/289>`__)
-- Add support for :class:`trio.Queue` with `capacity=0`. Queue's implementation
+- Add support for ``trio.Queue`` with ``capacity=0``. Queue's implementation
   is also faster now. (`#473
   <https://github.com/python-trio/trio/issues/473>`__)
 - Switch to using standalone `Outcome
   <https://github.com/python-trio/outcome>`__ library for Result objects.
   (`#494 <https://github.com/python-trio/trio/issues/494>`__)
 
 Deprecations and Removals
@@ -393,15 +421,15 @@
 
   * The hazmat function ``current_call_soon_thread_and_signal_safe``
     is being replaced by :class:`trio.hazmat.TrioToken`
 
   See `#68 <https://github.com/python-trio/trio/issues/68>`__ for
   details.
 
-* :class:`trio.Queue`\'s ``join`` and ``task_done`` methods are
+* ``trio.Queue``\'s ``join`` and ``task_done`` methods are
   deprecated without replacement (`#321
   <https://github.com/python-trio/trio/issues/321>`__)
 
 * Trio 0.1.0 provided a set of built-in mechanisms for waiting for and
   tracking the result of individual tasks. We haven't yet found any
   cases where using this actually led to simpler code, though, and
   this feature is blocking useful improvements, so the following are
@@ -420,15 +448,15 @@
   main :mod:`trio` namespace and into :mod:`trio.hazmat`:
 
   * ``trio.Task`` → :class:`trio.hazmat.Task`
   * ``trio.current_task`` → :func:`trio.hazmat.current_task`
   * ``trio.Result`` → ``trio.hazmat.Result``
   * ``trio.Value`` → ``trio.hazmat.Value``
   * ``trio.Error`` → ``trio.hazmat.Error``
-  * ``trio.UnboundedQueue`` → :class:`trio.hazmat.UnboundedQueue`
+  * ``trio.UnboundedQueue`` → ``trio.hazmat.UnboundedQueue``
 
   In addition, several introspection attributes are being renamed:
 
   * ``nursery.children`` → ``nursery.child_tasks``
   * ``task.parent_task`` → use ``task.parent_nursery.parent_task`` instead
 
   See `#136 <https://github.com/python-trio/trio/issues/136>`__ for
```

### Comparing `trio-0.8.0/docs/source/reference-io.rst` & `trio-0.9.0/docs/source/reference-io.rst`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,23 @@
 
      # Get a raw SocketStream connection to the proxy:
      s0 = await open_tcp_stream("proxy", 443)
 
      # Set up SSL connection to proxy:
      s1 = SSLStream(s0, proxy_ssl_context, server_hostname="proxy")
      # Request a connection to the website
-     await s1.send_all(b"CONNECT website:443 / HTTP/1.0\r\n")
+     await s1.send_all(b"CONNECT website:443 / HTTP/1.0\r\n\r\n")
      await check_CONNECT_response(s1)
 
      # Set up SSL connection to the real website. Notice that s1 is
      # already an SSLStream object, and here we're wrapping a second
      # SSLStream object around it.
      s2 = SSLStream(s1, website_ssl_context, server_hostname="website")
      # Make our request
-     await s2.send_all("GET /index.html HTTP/1.0\r\n")
+     await s2.send_all(b"GET /index.html HTTP/1.0\r\n\r\n")
      ...
 
 * The :mod:`trio.testing` module provides a set of :ref:`flexible
   in-memory stream object implementations <testing-streams>`, so if
   you have a protocol implementation to test then you can can start
   two tasks, set up a virtual "socket" connecting them, and then do
   things like inject random-but-repeatable delays into the connection.
@@ -114,14 +114,24 @@
      -
      - :class:`~trio.SocketStream`, :class:`~trio.StapledStream`
    * - :class:`Listener`
      - :class:`AsyncResource`
      - :meth:`~Listener.accept`
      -
      - :class:`~trio.SocketListener`, :class:`~trio.ssl.SSLListener`
+   * - :class:`SendChannel`
+     - :class:`AsyncResource`
+     - :meth:`~SendChannel.send`, :meth:`~SendChannel.send_nowait`
+     -
+     - :func:`~trio.open_memory_channel`
+   * - :class:`ReceiveChannel`
+     - :class:`AsyncResource`
+     - :meth:`~ReceiveChannel.receive`, :meth:`~ReceiveChannel.receive_nowait`
+     - ``__aiter__``, ``__anext__``
+     - :func:`~trio.open_memory_channel`
 
 .. autoclass:: trio.abc.AsyncResource
    :members:
 
 .. currentmodule:: trio
 
 .. autofunction:: aclose_forcefully
@@ -146,14 +156,22 @@
 
 .. currentmodule:: trio.abc
 
 .. autoclass:: trio.abc.Listener
    :members:
    :show-inheritance:
 
+.. autoclass:: trio.abc.SendChannel
+   :members:
+   :show-inheritance:
+
+.. autoclass:: trio.abc.ReceiveChannel
+   :members:
+   :show-inheritance:
+
 .. currentmodule:: trio
 
 
 Generic stream tools
 ~~~~~~~~~~~~~~~~~~~~
 
 Trio currently provides a generic helper for writing servers that
```

### Comparing `trio-0.8.0/docs/source/local_customization.py` & `trio-0.9.0/docs/source/local_customization.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/reference-hazmat.rst` & `trio-0.9.0/docs/source/reference-hazmat.rst`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 Debugging and instrumentation
 =============================
 
 Trio tries hard to provide useful hooks for debugging and
 instrumentation. Some are documented above (the nursery introspection
-attributes, :meth:`trio.Queue.statistics`, etc.). Here are some more.
+attributes, :meth:`trio.Lock.statistics`, etc.). Here are some more.
 
 
 Global statistics
 -----------------
 
 .. autofunction:: current_statistics
 
@@ -277,44 +277,14 @@
 
 .. function:: current_iocp()
 
 .. function:: monitor_completion_key()
    :with: queue
 
 
-Unbounded queues
-================
-
-In the section :ref:`queue`, we showed an example with two producers
-and one consumer using the same queue, where the queue size would grow
-without bound to produce unbounded latency and memory usage.
-:class:`trio.Queue` avoids this by placing an upper bound on how big
-the queue can get before ``put`` starts blocking. But what if you're
-in a situation where ``put`` can't block?
-
-There is another option: the queue consumer could get greedy. Each
-time it runs, it could eagerly consume all of the pending items before
-allowing another task to run. (In some other systems, this would
-happen automatically because their queue's ``get`` method doesn't
-invoke the scheduler unless it has to block. But :ref:`in trio, get is
-always a checkpoint <checkpoint-rule>`.) This works, but it's a bit
-risky: basically instead of applying backpressure to specifically the
-producer tasks, we're applying it to *all* the tasks in our system.
-The danger here is that if enough items have built up in the queue,
-then "stopping the world" to process them all may cause unacceptable
-latency spikes in unrelated tasks. Nonetheless, this is still the
-right choice in situations where it's impossible to apply backpressure
-more precisely. So this is the strategy implemented by
-:class:`UnboundedQueue`. The main time you should use this is when
-working with low-level APIs like :func:`monitor_kevent`.
-
-.. autoclass:: UnboundedQueue
-   :members:
-
-
 Global state: system tasks and run-local variables
 ==================================================
 
 .. autoclass:: RunVar
 
 .. autofunction:: spawn_system_task
```

### Comparing `trio-0.8.0/docs/source/_static/favicon-32.ico` & `trio-0.9.0/docs/source/_static/favicon-32.ico`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/_static/ornament.svg` & `trio-0.9.0/docs/source/_static/ornament.svg`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/_static/favicon.svg` & `trio-0.9.0/docs/source/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/_static/favicon-32.png` & `trio-0.9.0/docs/source/_static/favicon-32.png`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/_static/hackrtd.css` & `trio-0.9.0/docs/source/_static/hackrtd.css`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/index.rst` & `trio-0.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/design.rst` & `trio-0.9.0/docs/source/design.rst`

 * *Files 1% similar despite different names*

```diff
@@ -409,19 +409,14 @@
          ...
 
      def OPERATION_nowait(...):
          ...
 
   and the ``nowait`` version raises :exc:`trio.WouldBlock` if it would block.
 
-* The word ``monitor`` is used for APIs that involve an
-  :class:`trio.hazmat.UnboundedQueue` receiving some kind of events.
-  (Examples: nursery ``.monitor`` attribute, some of the low-level I/O
-  functions in :mod:`trio.hazmat`.)
-
 * ...we should, but currently don't, have a solid convention to
   distinguish between functions that take an async callable and those
   that take a sync callable. See `issue #68
   <https://github.com/python-trio/trio/issues/68>`__.
 
 
 A brief tour of trio's internals
@@ -443,15 +438,15 @@
 is to reach the point where we *can* declare the API stable. It's
 unlikely that we'll be able to quickly explore all possible corners of
 the design space and cover all possible types of I/O. So instead, our
 strategy is to make sure that it's possible for independent packages
 to add new features on top of trio. Enforcing the ``trio`` vs
 ``trio._core`` split is a way of `eating our own dogfood
 <https://en.wikipedia.org/wiki/Eating_your_own_dog_food>`__: basic
-functionality like :class:`trio.Queue` and :mod:`trio.socket` is
+functionality like :class:`trio.Lock` and :mod:`trio.socket` is
 actually implemented solely in terms of public APIs. And the hope is
 that by doing this, we increase the chances that someone who comes up
 with a better kind of queue or wants to add some new functionality
 like, say, file system change watching, will be able to do that on top
 of our public APIs without having to modify trio internals.
```

### Comparing `trio-0.8.0/docs/source/contributing.rst` & `trio-0.9.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/code-of-conduct.rst` & `trio-0.9.0/docs/source/code-of-conduct.rst`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/source/tutorial.rst` & `trio-0.9.0/docs/source/tutorial.rst`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
 unfortunately, if you forget an ``await``, you don't get that. What
 you actually get is:
 
 .. code-block:: none
 
    >>> trio.run(broken_double_sleep, 3)
    *yawn* Going to sleep
-   Woke up again after 0.00 seconds, feeling well rested!
+   Woke up after 0.00 seconds, feeling well rested!
    __main__:4: RuntimeWarning: coroutine 'sleep' was never awaited
    >>>
 
 This is clearly broken – 0.00 seconds is not long enough to feel well
 rested! Yet the code acts like it succeeded – no exception was
 raised. The only clue that something went wrong is that it prints
 ``RuntimeWarning: coroutine 'sleep' was never awaited``. Also, the
@@ -302,15 +302,15 @@
 runs:
 
 .. code-block:: none
 
    # On PyPy:
    >>>> trio.run(broken_double_sleep, 3)
    *yawn* Going to sleep
-   Woke up again after 0.00 seconds, feeling well rested!
+   Woke up after 0.00 seconds, feeling well rested!
    >>>> # what the ... ?? not even a warning!
 
    >>>> # but forcing a garbage collection gives us a warning:
    >>>> import gc
    >>>> gc.collect()
    /home/njs/pypy-3.5-nightly/lib-python/3/importlib/_bootstrap.py:191: RuntimeWarning: coroutine 'sleep' was never awaited
    if _module_locks.get(name) is wr:    # XXX PyPy fix?
@@ -473,21 +473,21 @@
      child1: started! sleeping now...
        [... 1 second passes ...]
      child1: exiting!
      child2: exiting!
    parent: all done!
 
 (Your output might have the order of the "started" and/or "exiting"
-lines swapped compared to to mine.)
+lines swapped compared to mine.)
 
 Notice that ``child1`` and ``child2`` both start together and then
-both exit together, and that the whole program only takes 1 second to
-run, even though we made two calls to ``trio.sleep(1)``, which should
-take two seconds in total. So it looks like ``child1`` and ``child2``
-really are running at the same time!
+both exit together. And, even though we made two calls to
+``trio.sleep(1)``, the program finished in just one second total.
+So it looks like ``child1`` and ``child2`` really are running at the
+same time!
 
 Now, if you're familiar with programming using threads, this might
 look familiar – and that's intentional. But it's important to realize
 that *there are no threads here*. All of this is happening in a single
 thread. To remind ourselves of this, we use slightly different
 terminology: instead of spawning two "threads", we say that we spawned
 two "tasks". There are two differences between tasks and threads: (1)
@@ -596,15 +596,15 @@
    <<< task step finished: __main__.child1
 
 Each task runs until it hits the call to :func:`trio.sleep`, and then
 suddenly we're back in :func:`trio.run` deciding what to run next. How
 does this happen? The secret is that :func:`trio.run` and
 :func:`trio.sleep` work together to make it happen: :func:`trio.sleep`
 has access to some special magic that lets it pause its entire
-callstack, so it sends a note to :func:`trio.run` requesting to be
+call stack, so it sends a note to :func:`trio.run` requesting to be
 woken again after 1 second, and then suspends the task. And once the
 task is suspended, Python gives control back to :func:`trio.run`,
 which decides what to do next. (If this sounds similar to the way that
 generators can suspend execution by doing a ``yield``, then that's not
 a coincidence: inside the Python interpreter, there's a lot of overlap
 between the implementation of generators and async functions.)
 
@@ -756,19 +756,19 @@
 this frustrating.
 
 But from trio's point of view, the problem with the GIL isn't that it
 restricts parallelism. Of course it would be nice if Python had better
 options for taking advantage of multiple cores, but that's an
 extremely difficult problem to solve, and in the meantime there are
 lots of problems where a single core is totally adequate – or where if
-it isn't, then process- or machine-level parallelism works fine.
+it isn't, then process-level or machine-level parallelism works fine.
 
 No, the problem with the GIL is that it's a *lousy deal*: we give up
 on using multiple cores, and in exchange we get... almost all the same
-challenges and mind bending bugs that come with real parallel
+challenges and mind-bending bugs that come with real parallel
 programming, and – to add insult to injury – `pretty poor scalability
 <https://twitter.com/hynek/status/771790449057132544>`__. Threads in
 Python just aren't that appealing.
 
 Trio doesn't make your code run on multiple cores; in fact, as we saw
 above, it's baked into trio's design that you never have two tasks
 running at the same time. We're not so much overcoming the GIL as
@@ -872,15 +872,15 @@
    :pyobject: parent
 
 First we call :func:`trio.open_tcp_stream` to make a TCP connection to
 the server. ``127.0.0.1`` is a magic `IP address
 <https://en.wikipedia.org/wiki/IP_address>`__ meaning "the computer
 I'm running on", so this connects us to whatever program on the local
 computer is using ``PORT`` as its contact point. This function returns
-a object implementing Trio's :class:`~trio.abc.Stream` interface,
+an object implementing Trio's :class:`~trio.abc.Stream` interface,
 which gives us methods to send and receive bytes, and to close the
 connection when we're done. We use an ``async with`` block to make
 sure that we do close the connection – not a big deal in a toy example
 like this, but it's a good habit to get into, and Trio is designed to
 make ``with`` and ``async with`` blocks easy to use.
 
 Finally, we start up two child tasks, and pass each of them a
@@ -982,15 +982,15 @@
 
 So what's that ``try`` block for? Remember that in trio, like Python
 in general, exceptions keep propagating until they're caught. Here we
 think it's plausible there might be unexpected exceptions, and we want
 to isolate that to making just this one task crash, without taking
 down the whole program. For example, if the client closes the
 connection at the wrong moment then it's possible this code will end
-up calling ``send_all`` on a closed connection and get an
+up calling ``send_all`` on a closed connection and get a
 :exc:`BrokenResourceError`; that's unfortunate, and in a more serious
 program we might want to handle it more explicitly, but it doesn't
 indicate a problem for any *other* connections. On the other hand, if
 the exception is something like a :exc:`KeyboardInterrupt`, we *do*
 want that to propagate out into the parent task and cause the whole
 program to exit. To express this, we use a ``try`` block with an
 ``except Exception:`` handler.
```

### Comparing `trio-0.8.0/docs/notes.txt` & `trio-0.9.0/docs/notes.txt`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/make.bat` & `trio-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/docs/Makefile` & `trio-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio.egg-info/PKG-INFO` & `trio-0.9.0/trio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: trio
-Version: 0.8.0
+Version: 0.9.0
 Summary: An async/await-native I/O library for humans and snake people
 Home-page: https://github.com/python-trio/trio
 Author: Nathaniel J. Smith
 Author-email: njs@pobox.com
 License: MIT -or- Apache License 2.0
 Description: .. image:: https://cdn.rawgit.com/python-trio/trio/9b0bec646a31e0d0f67b8b6ecc6939726faf3e17/logo/logo-with-background.svg
            :width: 200px
```

### Comparing `trio-0.8.0/trio/_path.py` & `trio-0.9.0/trio/_path.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_sync.py` & `trio-0.9.0/trio/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import deque, OrderedDict
 
 import attr
 import outcome
 
 from . import _core
 from ._util import aiter_compat
+from ._deprecate import deprecated
 
 __all__ = [
     "Event",
     "CapacityLimiter",
     "Semaphore",
     "Lock",
     "StrictFIFOLock",
@@ -839,14 +840,20 @@
       capacity (int): The maximum number of items allowed in the queue before
           :meth:`put` blocks. Choosing a sensible value here is important to
           ensure that backpressure is communicated promptly and avoid
           unnecessary latency. If in doubt, use 0.
 
     """
 
+    @deprecated(
+        "0.9.0",
+        issue=497,
+        thing="trio.Queue",
+        instead="trio.open_memory_channel"
+    )
     def __init__(self, capacity):
         if not isinstance(capacity, int):
             raise TypeError("capacity must be an integer")
         if capacity < 0:
             raise ValueError("capacity must be >= 0")
         self.capacity = operator.index(capacity)
         # {task: None} ordered set
```

### Comparing `trio-0.8.0/trio/_threads.py` & `trio-0.9.0/trio/_threads.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_highlevel_ssl_helpers.py` & `trio-0.9.0/trio/_highlevel_ssl_helpers.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_highlevel_open_unix_stream.py` & `trio-0.9.0/trio/_highlevel_open_unix_stream.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_highlevel_open_tcp_stream.py` & `trio-0.9.0/trio/_highlevel_open_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/socket.py` & `trio-0.9.0/trio/socket.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_highlevel_socket.py` & `trio-0.9.0/trio/_highlevel_socket.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_abc.py` & `trio-0.9.0/trio/_abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from abc import ABCMeta, abstractmethod
+from ._util import aiter_compat
 from . import _core
 
 __all__ = [
     "Clock",
     "Instrument",
     "AsyncResource",
     "SendStream",
     "ReceiveStream",
     "Stream",
     "HalfCloseableStream",
     "SocketFactory",
     "HostnameResolver",
     "Listener",
+    "SendChannel",
+    "ReceiveChannel",
 ]
 
 
 # We use ABCMeta instead of ABC, plus set __slots__=(), so as not to force a
 # __dict__ onto subclasses.
 class Clock(metaclass=ABCMeta):
     """The interface for custom run loop clocks.
@@ -278,16 +281,20 @@
 class SendStream(AsyncResource):
     """A standard interface for sending data on a byte stream.
 
     The underlying stream may be unidirectional, or bidirectional. If it's
     bidirectional, then you probably want to also implement
     :class:`ReceiveStream`, which makes your object a :class:`Stream`.
 
-    Every :class:`SendStream` also implements the :class:`AsyncResource`
-    interface.
+    :class:`SendStream` objects also implement the :class:`AsyncResource`
+    interface, so they can be closed by calling :meth:`~AsyncResource.aclose`
+    or using an ``async with`` block.
+
+    If you want to send Python objects rather than raw bytes, see
+    :class:`SendChannel`.
 
     """
     __slots__ = ()
 
     @abstractmethod
     async def send_all(self, data):
         """Sends the given data through the stream, blocking if necessary.
@@ -374,16 +381,20 @@
 class ReceiveStream(AsyncResource):
     """A standard interface for receiving data on a byte stream.
 
     The underlying stream may be unidirectional, or bidirectional. If it's
     bidirectional, then you probably want to also implement
     :class:`SendStream`, which makes your object a :class:`Stream`.
 
-    Every :class:`ReceiveStream` also implements the :class:`AsyncResource`
-    interface.
+    :class:`ReceiveStream` objects also implement the :class:`AsyncResource`
+    interface, so they can be closed by calling :meth:`~AsyncResource.aclose`
+    or using an ``async with`` block.
+
+    If you want to receive Python objects rather than raw bytes, see
+    :class:`ReceiveChannel`.
 
     """
     __slots__ = ()
 
     @abstractmethod
     async def receive_some(self, max_bytes):
         """Wait until there is data available on this stream, and then return
@@ -486,35 +497,215 @@
 
         """
 
 
 class Listener(AsyncResource):
     """A standard interface for listening for incoming connections.
 
+    :class:`Listener` objects also implement the :class:`AsyncResource`
+    interface, so they can be closed by calling :meth:`~AsyncResource.aclose`
+    or using an ``async with`` block.
+
     """
     __slots__ = ()
 
     @abstractmethod
     async def accept(self):
         """Wait until an incoming connection arrives, and then return it.
 
         Returns:
           AsyncResource: An object representing the incoming connection. In
-          practice this is almost always some variety of :class:`Stream`,
-          though in principle you could also use this interface with, say,
-          SOCK_SEQPACKET sockets or similar.
+          practice this is generally some kind of :class:`Stream`,
+          but in principle you could also define a :class:`Listener` that
+          returned, say, channel objects.
 
         Raises:
           trio.BusyResourceError: if two tasks attempt to call
               :meth:`accept` on the same listener at the same time.
           trio.ClosedResourceError: if you previously closed this listener
               object, or if another task closes this listener object while
               :meth:`accept` is running.
 
-        Note that there is no ``BrokenListenerError``, because for listeners
-        there is no general condition of "the network/remote peer broke the
-        connection" that can be handled in a generic way, like there is for
-        streams. Other errors *can* occur and be raised from :meth:`accept` –
-        for example, if you run out of file descriptors then you might get an
-        :class:`OSError` with its errno set to ``EMFILE``.
+        Listeners don't generally raise :exc:`~trio.BrokenResourceError`,
+        because for listeners there is no general condition of "the
+        network/remote peer broke the connection" that can be handled in a
+        generic way, like there is for streams. Other errors *can* occur and
+        be raised from :meth:`accept` – for example, if you run out of file
+        descriptors then you might get an :class:`OSError` with its errno set
+        to ``EMFILE``.
+
+        """
+
+
+class SendChannel(AsyncResource):
+    """A standard interface for sending Python objects to some receiver.
+
+    :class:`SendChannel` objects also implement the :class:`AsyncResource`
+    interface, so they can be closed by calling :meth:`~AsyncResource.aclose`
+    or using an ``async with`` block.
+
+    If you want to send raw bytes rather than Python objects, see
+    :class:`ReceiveStream`.
+
+    """
+    __slots__ = ()
+
+    @abstractmethod
+    def send_nowait(self, value):
+        """Attempt to send an object through the channel, without blocking.
+
+        Args:
+          value (object): The object to send.
+
+        Raises:
+          trio.WouldBlock: if the operation cannot be completed immediately
+              (for example, because the channel's internal buffer is full).
+          trio.BrokenResourceError: if something has gone wrong, and the
+              channel is broken. For example, you may get this if the receiver
+              has already been closed.
+          trio.ClosedResourceError: if you previously closed this
+              :class:`SendChannel` object.
+
+        """
+
+    @abstractmethod
+    async def send(self, value):
+        """Attempt to send an object through the channel, blocking if necessary.
+
+        Args:
+          value (object): The object to send.
+
+        Raises:
+          trio.BrokenResourceError: if something has gone wrong, and the
+              channel is broken. For example, you may get this if the receiver
+              has already been closed.
+          trio.ClosedResourceError: if you previously closed this
+              :class:`SendChannel` object, or if another task closes it while
+              :meth:`send` is running.
 
         """
+
+    @abstractmethod
+    def clone(self):
+        """Clone this send channel object.
+
+        This returns a new :class:`SendChannel` object, which acts as a
+        duplicate of the original: sending on the new object does exactly the
+        same thing as sending on the old object.
+
+        However, closing one of the objects does not close the other, and
+        receivers don't get :exc:`~trio.EndOfChannel` until *all* clones have
+        been closed.
+
+        This is useful for communication patterns that involve multiple
+        producers all sending objects to the same destination. If you give
+        each producer its own clone of the :class:`SendChannel`, and then make
+        sure to close each :class:`SendChannel` when it's finished, receivers
+        will automatically get notified when all producers are finished. See
+        :ref:`channel-mpmc` for examples.
+
+        Raises:
+          trio.ClosedResourceError: if you already closed this
+              :class:`SendChannel` object.
+
+        """
+
+
+class ReceiveChannel(AsyncResource):
+    """A standard interface for receiving Python objects from some sender.
+
+    You can iterate over a :class:`ReceiveChannel` using an ``async for``
+    loop::
+
+       async for value in receive_channel:
+           ...
+
+    This is equivalent to calling :meth:`receive` repeatedly. The loop exits
+    without error when :meth:`receive` raises :exc:`~trio.EndOfChannel`.
+
+    :class:`ReceiveChannel` objects also implement the :class:`AsyncResource`
+    interface, so they can be closed by calling :meth:`~AsyncResource.aclose`
+    or using an ``async with`` block.
+
+    If you want to receive raw bytes rather than Python objects, see
+    :class:`ReceiveStream`.
+
+    """
+    __slots__ = ()
+
+    @abstractmethod
+    def receive_nowait(self):
+        """Attempt to receive an incoming object, without blocking.
+
+        Returns:
+          object: Whatever object was received.
+
+        Raises:
+          trio.WouldBlock: if the operation cannot be completed immediately
+              (for example, because no object has been sent yet).
+          trio.EndOfChannel: if the sender has been closed cleanly, and no
+              more objects are coming. This is not an error condition.
+          trio.ClosedResourceError: if you previously closed this
+              :class:`ReceiveChannel` object.
+          trio.BrokenResourceError: if something has gone wrong, and the
+              channel is broken.
+
+        """
+
+    @abstractmethod
+    async def receive(self):
+        """Attempt to receive an incoming object, blocking if necessary.
+
+        It's legal for multiple tasks to call :meth:`receive` at the same
+        time. If this happens, then one task receives the first value sent,
+        another task receives the next value sent, and so on.
+
+        Returns:
+          object: Whatever object was received.
+
+        Raises:
+          trio.EndOfChannel: if the sender has been closed cleanly, and no
+              more objects are coming. This is not an error condition.
+          trio.ClosedResourceError: if you previously closed this
+              :class:`ReceiveChannel` object.
+          trio.BrokenResourceError: if something has gone wrong, and the
+              channel is broken.
+
+        """
+
+    @abstractmethod
+    def clone(self):
+        """Clone this receive channel object.
+
+        This returns a new :class:`ReceiveChannel` object, which acts as a
+        duplicate of the original: receiving on the new object does exactly
+        the same thing as receiving on the old object.
+
+        However, closing one of the objects does not close the other, and the
+        underlying channel is not closed until all clones are closed.
+
+        This is useful for communication patterns involving multiple consumers
+        all receiving objects from the same underlying channel. See
+        :ref:`channel-mpmc` for examples.
+
+        .. warning:: The clones all share the same underlying channel.
+           Whenever a clone :meth:`receive`\s a value, it is removed from the
+           channel and the other clones do *not* receive that value. If you
+           want to send multiple copies of the same stream of values to
+           multiple destinations, like :func:`itertools.tee`, then you need to
+           find some other solution; this method does *not* do that.
+
+        Raises:
+          trio.ClosedResourceError: if you already closed this
+              :class:`SendChannel` object.
+
+        """
+
+    @aiter_compat
+    def __aiter__(self):
+        return self
+
+    async def __anext__(self):
+        try:
+            return await self.receive()
+        except _core.EndOfChannel:
+            raise StopAsyncIteration
```

### Comparing `trio-0.8.0/trio/_subprocess.py` & `trio-0.9.0/trio/_subprocess.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_timeouts.py` & `trio-0.9.0/trio/_timeouts.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/hazmat.py` & `trio-0.9.0/trio/hazmat.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_highlevel_generic.py` & `trio-0.9.0/trio/_highlevel_generic.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_file_io.py` & `trio-0.9.0/trio/_file_io.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_deprecate.py` & `trio-0.9.0/trio/_deprecate.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_util.py` & `trio-0.9.0/trio/_util.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_highlevel_serve_listeners.py` & `trio-0.9.0/trio/_highlevel_serve_listeners.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/__init__.py` & `trio-0.9.0/trio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from ._version import __version__
 
 from ._core import (
     TrioInternalError, RunFinishedError, WouldBlock, Cancelled,
     BusyResourceError, ClosedResourceError, MultiError, run, open_nursery,
     open_cancel_scope, current_effective_deadline, TASK_STATUS_IGNORED,
-    current_time, BrokenResourceError
+    current_time, BrokenResourceError, EndOfChannel
 )
 
 from ._timeouts import (
     move_on_at, move_on_after, sleep_forever, sleep_until, sleep, fail_at,
     fail_after, TooSlowError
 )
 
@@ -34,14 +34,16 @@
 from ._threads import (
     run_sync_in_worker_thread, current_default_worker_thread_limiter,
     BlockingTrioPortal
 )
 
 from ._highlevel_generic import aclose_forcefully, StapledStream
 
+from ._channel import open_memory_channel
+
 from ._signals import catch_signals, open_signal_receiver
 
 from ._highlevel_socket import SocketStream, SocketListener
 
 from ._file_io import open_file, wrap_file
 
 from ._path import Path
```

### Comparing `trio-0.8.0/trio/_wait_for_object.py` & `trio-0.9.0/trio/_wait_for_object.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_highlevel_open_unix_stream.py` & `trio-0.9.0/trio/tests/test_highlevel_open_unix_stream.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_highlevel_serve_listeners.py` & `trio-0.9.0/trio/tests/test_highlevel_serve_listeners.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 import trio
 from trio.testing import memory_stream_pair, wait_all_tasks_blocked
 
 
 @attr.s(hash=False, cmp=False)
 class MemoryListener(trio.abc.Listener):
     closed = attr.ib(default=False)
-    accepted_streams = attr.ib(default=attr.Factory(list))
-    queued_streams = attr.ib(default=attr.Factory(lambda: trio.Queue(1)))
+    accepted_streams = attr.ib(factory=list)
+    queued_streams = attr.ib(factory=(lambda: trio.open_memory_channel(1)))
     accept_hook = attr.ib(default=None)
 
     async def connect(self):
         assert not self.closed
         client, server = memory_stream_pair()
-        await self.queued_streams.put(server)
+        await self.queued_streams[0].send(server)
         return client
 
     async def accept(self):
         await trio.hazmat.checkpoint()
         assert not self.closed
         if self.accept_hook is not None:
             await self.accept_hook()
-        stream = await self.queued_streams.get()
+        stream = await self.queued_streams[1].receive()
         self.accepted_streams.append(stream)
         return stream
 
     async def aclose(self):
         self.closed = True
         await trio.hazmat.checkpoint()
```

### Comparing `trio-0.8.0/trio/tests/test_wait_for_object.py` & `trio-0.9.0/trio/tests/test_wait_for_object.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_path.py` & `trio-0.9.0/trio/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_signals.py` & `trio-0.9.0/trio/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_threads.py` & `trio-0.9.0/trio/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_highlevel_socket.py` & `trio-0.9.0/trio/tests/test_highlevel_socket.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/subprocess/test_waitpid_linux.py` & `trio-0.9.0/trio/tests/subprocess/test_waitpid_linux.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/subprocess/test_unix_pipes.py` & `trio-0.9.0/trio/tests/subprocess/test_unix_pipes.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/conftest.py` & `trio-0.9.0/trio/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_file_io.py` & `trio-0.9.0/trio/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_testing.py` & `trio-0.9.0/trio/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/module_with_deprecations.py` & `trio-0.9.0/trio/tests/module_with_deprecations.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_deprecate.py` & `trio-0.9.0/trio/tests/test_deprecate.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_highlevel_open_tcp_stream.py` & `trio-0.9.0/trio/tests/test_highlevel_open_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_highlevel_open_tcp_listeners.py` & `trio-0.9.0/trio/tests/test_highlevel_open_tcp_listeners.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_timeouts.py` & `trio-0.9.0/trio/tests/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_highlevel_generic.py` & `trio-0.9.0/trio/tests/test_highlevel_generic.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_exports.py` & `trio-0.9.0/trio/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_socket.py` & `trio-0.9.0/trio/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_highlevel_ssl_helpers.py` & `trio-0.9.0/trio/tests/test_highlevel_ssl_helpers.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_util.py` & `trio-0.9.0/trio/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/tests/test_sync.py` & `trio-0.9.0/trio/tests/test_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from ..testing import wait_all_tasks_blocked, assert_checkpoints
 
 from .. import _core
 from .. import _timeouts
 from .._timeouts import sleep_forever, move_on_after
 from .._sync import *
 
+pytestmark = pytest.mark.filterwarnings(
+    "ignore:.*trio.Queue:trio.TrioDeprecationWarning"
+)
+
 
 async def test_Event():
     e = Event()
     assert not e.is_set()
     assert e.statistics().tasks_waiting == 0
 
     e.set()
@@ -554,18 +558,84 @@
         nursery.start_soon(do_put, q, 1)
         with assert_checkpoints():
             assert await q.get() == 1
     with pytest.raises(_core.WouldBlock):
         q.get_nowait()
 
 
-# Two ways of implementing a Lock in terms of a Queue. Used to let us put the
-# Queue through the generic lock tests.
-
 from .._sync import async_cm
+from .._channel import open_memory_channel
+
+# Three ways of implementing a Lock in terms of a channel. Used to let us put
+# the channel through the generic lock tests.
+
+
+@async_cm
+class ChannelLock1:
+    def __init__(self, capacity):
+        self.s, self.r = open_memory_channel(capacity)
+        for _ in range(capacity - 1):
+            self.s.send_nowait(None)
+
+    def acquire_nowait(self):
+        self.s.send_nowait(None)
+
+    async def acquire(self):
+        await self.s.send(None)
+
+    def release(self):
+        self.r.receive_nowait()
+
+
+@async_cm
+class ChannelLock2:
+    def __init__(self):
+        self.s, self.r = open_memory_channel(10)
+        self.s.send_nowait(None)
+
+    def acquire_nowait(self):
+        self.r.receive_nowait()
+
+    async def acquire(self):
+        await self.r.receive()
+
+    def release(self):
+        self.s.send_nowait(None)
+
+
+@async_cm
+class ChannelLock3:
+    def __init__(self):
+        self.s, self.r = open_memory_channel(0)
+        # self.acquired is true when one task acquires the lock and
+        # only becomes false when it's released and no tasks are
+        # waiting to acquire.
+        self.acquired = False
+
+    def acquire_nowait(self):
+        assert not self.acquired
+        self.acquired = True
+
+    async def acquire(self):
+        if self.acquired:
+            await self.s.send(None)
+        else:
+            self.acquired = True
+            await _core.checkpoint()
+
+    def release(self):
+        try:
+            self.r.receive_nowait()
+        except _core.WouldBlock:
+            assert self.acquired
+            self.acquired = False
+
+
+# Three ways of implementing a Lock in terms of a Queue. Used to let us put
+# the Queue through the generic lock tests.
 
 
 @async_cm
 class QueueLock1:
     def __init__(self, capacity):
         self.q = Queue(capacity)
         for _ in range(capacity - 1):
@@ -626,24 +696,32 @@
 
 
 lock_factories = [
     lambda: CapacityLimiter(1),
     lambda: Semaphore(1),
     Lock,
     StrictFIFOLock,
+    lambda: ChannelLock1(10),
+    lambda: ChannelLock1(1),
+    ChannelLock2,
+    ChannelLock3,
     lambda: QueueLock1(10),
     lambda: QueueLock1(1),
     QueueLock2,
     QueueLock3,
 ]
 lock_factory_names = [
     "CapacityLimiter(1)",
     "Semaphore(1)",
     "Lock",
     "StrictFIFOLock",
+    "ChannelLock1(10)",
+    "ChannelLock1(1)",
+    "ChannelLock2",
+    "ChannelLock3",
     "QueueLock1(10)",
     "QueueLock1(1)",
     "QueueLock2",
     "QueueLock3",
 ]
 
 generic_lock_test = pytest.mark.parametrize(
```

### Comparing `trio-0.8.0/trio/tests/test_ssl.py` & `trio-0.9.0/trio/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_subprocess/linux_waitpid.py` & `trio-0.9.0/trio/_subprocess/linux_waitpid.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_subprocess/unix_pipes.py` & `trio-0.9.0/trio/_subprocess/unix_pipes.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_socket.py` & `trio-0.9.0/trio/_socket.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_ki.py` & `trio-0.9.0/trio/_core/_ki.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_run.py` & `trio-0.9.0/trio/_core/_run.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_io_epoll.py` & `trio-0.9.0/trio/_core/_io_epoll.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/__init__.py` & `trio-0.9.0/trio/_core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # of _run.py for the wrapper implementation).
     fn._public = True
     return fn
 
 
 from ._exceptions import (
     TrioInternalError, RunFinishedError, WouldBlock, Cancelled,
-    BusyResourceError, ClosedResourceError, BrokenResourceError
+    BusyResourceError, ClosedResourceError, BrokenResourceError, EndOfChannel
 )
 
 from ._multierror import MultiError
 
 from ._traps import cancel_shielded_checkpoint, Abort, wait_task_rescheduled
 
 from ._ki import (
```

### Comparing `trio-0.8.0/trio/_core/_result.py` & `trio-0.9.0/trio/_core/_result.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_epoll.py` & `trio-0.9.0/trio/_core/tests/test_epoll.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_multierror_scripts/ipython_custom_exc.py` & `trio-0.9.0/trio/_core/tests/test_multierror_scripts/ipython_custom_exc.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_local.py` & `trio-0.9.0/trio/_core/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_unbounded_queue.py` & `trio-0.9.0/trio/_core/tests/test_unbounded_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import itertools
 
 import pytest
 
 from ... import _core
 from ...testing import assert_checkpoints, wait_all_tasks_blocked
 
+pytestmark = pytest.mark.filterwarnings(
+    "ignore:.*UnboundedQueue:trio.TrioDeprecationWarning"
+)
+
 
 async def test_UnboundedQueue_basic():
     q = _core.UnboundedQueue()
     q.put_nowait("hi")
     assert await q.get_batch() == ["hi"]
     with pytest.raises(_core.WouldBlock):
         q.get_batch_nowait()
```

### Comparing `trio-0.8.0/trio/_core/tests/tutil.py` & `trio-0.9.0/trio/_core/tests/tutil.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_ki.py` & `trio-0.9.0/trio/_core/tests/test_ki.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,15 +534,15 @@
     lock = threading.Lock()
 
     def kill_soon():
         # We want the signal to be raised after the main thread has entered
         # the IO manager blocking primitive. There really is no way to
         # deterministically interlock with that, so we have to use sleep and
         # hope it's long enough.
-        time.sleep(1)
+        time.sleep(1.1)
         with lock:
             print("thread doing ki_self()")
             ki_self()
             if buggy_wakeup_fd:
                 print("buggy_wakeup_fd =", buggy_wakeup_fd)
                 ki_self()
```

### Comparing `trio-0.8.0/trio/_core/tests/conftest.py` & `trio-0.9.0/trio/_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_run.py` & `trio-0.9.0/trio/_core/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_result.py` & `trio-0.9.0/trio/_core/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_multierror.py` & `trio-0.9.0/trio/_core/tests/test_multierror.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_io.py` & `trio-0.9.0/trio/_core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/tests/test_parking_lot.py` & `trio-0.9.0/trio/_core/tests/test_parking_lot.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_unbounded_queue.py` & `trio-0.9.0/trio/_core/_unbounded_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import deque
 import attr
 
 from .. import _core
 from .._util import aiter_compat
+from .._deprecate import deprecated
 
 __all__ = ["UnboundedQueue"]
 
 
 @attr.s(frozen=True)
 class _UnboundedQueueStats:
     qsize = attr.ib()
@@ -39,14 +40,20 @@
 
        while True:
            obj = await queue.get_batch()
            ...
 
     """
 
+    @deprecated(
+        "0.9.0",
+        issue=497,
+        thing="trio.hazmat.UnboundedQueue",
+        instead="trio.open_memory_channel(math.inf)"
+    )
     def __init__(self):
         self._lot = _core.ParkingLot()
         self._data = []
         # used to allow handoff from put to the first task in the lot
         self._can_get = False
 
     def __repr__(self):
```

### Comparing `trio-0.8.0/trio/_core/_traps.py` & `trio-0.9.0/trio/_core/_traps.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_local.py` & `trio-0.9.0/trio/_core/_local.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_io_kqueue.py` & `trio-0.9.0/trio/_core/_io_kqueue.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_entry_queue.py` & `trio-0.9.0/trio/_core/_entry_queue.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_multierror.py` & `trio-0.9.0/trio/_core/_multierror.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_io_windows.py` & `trio-0.9.0/trio/_core/_io_windows.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_wakeup_socketpair.py` & `trio-0.9.0/trio/_core/_wakeup_socketpair.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_exceptions.py` & `trio-0.9.0/trio/_core/_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,7 +119,16 @@
     You *don't* get this error if *you* closed the resource – in that case you
     get :class:`ClosedResourceError`.
 
     This exception's ``__cause__`` attribute will often contain more
     information about the underlying error.
 
     """
+
+
+class EndOfChannel(Exception):
+    """Raised when trying to receive from a :class:`trio.abc.ReceiveChannel`
+    that has no more data to receive.
+
+    This is analogous to an "end-of-file" condition, but for channels.
+
+    """
```

### Comparing `trio-0.8.0/trio/_core/_parking_lot.py` & `trio-0.9.0/trio/_core/_parking_lot.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_core/_windows_cffi.py` & `trio-0.9.0/trio/_core/_windows_cffi.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_signals.py` & `trio-0.9.0/trio/_signals.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_highlevel_open_tcp_listeners.py` & `trio-0.9.0/trio/_highlevel_open_tcp_listeners.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/_network.py` & `trio-0.9.0/trio/testing/_network.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/_trio_test.py` & `trio-0.9.0/trio/testing/_trio_test.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/__init__.py` & `trio-0.9.0/trio/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/_check_streams.py` & `trio-0.9.0/trio/testing/_check_streams.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/_mock_clock.py` & `trio-0.9.0/trio/testing/_mock_clock.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/_sequencer.py` & `trio-0.9.0/trio/testing/_sequencer.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/_memory_streams.py` & `trio-0.9.0/trio/testing/_memory_streams.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/testing/_checkpoints.py` & `trio-0.9.0/trio/testing/_checkpoints.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/trio/_ssl.py` & `trio-0.9.0/trio/_ssl.py`

 * *Files identical despite different names*

### Comparing `trio-0.8.0/PKG-INFO` & `trio-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: trio
-Version: 0.8.0
+Version: 0.9.0
 Summary: An async/await-native I/O library for humans and snake people
 Home-page: https://github.com/python-trio/trio
 Author: Nathaniel J. Smith
 Author-email: njs@pobox.com
 License: MIT -or- Apache License 2.0
 Description: .. image:: https://cdn.rawgit.com/python-trio/trio/9b0bec646a31e0d0f67b8b6ecc6939726faf3e17/logo/logo-with-background.svg
            :width: 200px
```

### Comparing `trio-0.8.0/setup.py` & `trio-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     long_description=LONG_DESC,
     author="Nathaniel J. Smith",
     author_email="njs@pobox.com",
     url="https://github.com/python-trio/trio",
     license="MIT -or- Apache License 2.0",
     packages=find_packages(),
     install_requires=[
-        "attrs",
+        "attrs >= 18.1.0",  # for attr.ib(factory=...)
         "sortedcontainers",
         "async_generator >= 1.9",
         "idna",
         "outcome",
         "sniffio",
         # PEP 508 style, but:
         # https://bitbucket.org/pypa/wheel/issues/181/bdist_wheel-silently-discards-pep-508
```


# Comparing `tmp/slapos.cookbook-1.0.9.tar.gz` & `tmp/slapos.cookbook-1.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slapos.cookbook-1.0.9.tar", last modified: Mon Aug 17 17:30:57 2015, max compression
+gzip compressed data, was "dist/slapos.cookbook-1.0.92.tar", last modified: Thu Feb 21 14:16:30 2019, max compression
```

## Comparing `slapos.cookbook-1.0.9.tar` & `slapos.cookbook-1.0.92.tar`

### file list

```diff
@@ -1,513 +1,353 @@
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       59 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/setup.cfg
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      277 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/MANIFEST.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    55869 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/PKG-INFO
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    26811 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/CHANGES.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)        1 2015-08-17 17:29:19.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/zip-safe
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)        7 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/top_level.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    15587 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/SOURCES.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       21 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/namespace_packages.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)        1 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/dependency_links.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    55869 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/PKG-INFO
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     7223 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/entry_points.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      137 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos.cookbook.egg-info/requires.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       61 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/README.txt
--rwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)    12183 2015-08-17 17:28:48.000000 slapos.cookbook-1.0.9/setup.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      244 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/test/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)        0 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/test/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      413 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/test/test_recipe.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2900 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/test/test_json_schema.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       52 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.cloudooo.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/proactive/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3302 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/proactive/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/proactive/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      422 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/proactive/template/ProActiveConfiguration.xml.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/configurationfile/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1677 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/configurationfile/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheperl/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2787 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheperl/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheperl/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2009 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheperl/template/apache.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       26 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.nosqltestbed.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3643 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/neoppod.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/nbdserver/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1948 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nbdserver/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/nbdserver/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      251 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nbdserver/template/nbdserver_run.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/davstorage/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4749 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/davstorage/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/davstorage/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      456 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/davstorage/template/php.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3792 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/davstorage/template/httpd.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3499 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/container.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       54 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.memcached.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    11080 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/vifib.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/xvfb/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2233 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xvfb/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/xvfb/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      202 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xvfb/template/xvfb_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      189 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xvfb/template/xwd_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4671 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/notifier.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4829 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/dcron.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/fontconfig/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3575 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/fontconfig/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/fontconfig/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      157 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/fontconfig/template/onetimedownload_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       32 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/fontconfig/template/fontconfig-snippet.cfg.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      153 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/fontconfig/template/fontconfig.cfg.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_test/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3301 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_test/test.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6241 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_test/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/reverse_proxy_nginx/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4094 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/reverse_proxy_nginx/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/reverse_proxy_nginx/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1280 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/reverse_proxy_nginx/template/nginx.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       48 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.kumofs.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1663 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/condor.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6459 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2497 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/configure.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3073 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/boinc.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/template/
--rwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)      687 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/template/machineinfo.sh.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2983 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/logrotate.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1939 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/simplelogger.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3077 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/genericslap.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    12378 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1980 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/inotify.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3307 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/execute.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     9528 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/generic.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      470 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/shlex.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3218 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/librecipe/filehash.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/firefox/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1975 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/firefox/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/firefox/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2244 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/firefox/template/prefs.js
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1425 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/firefox/template/firefox_run.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6056 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      732 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope/template/site.zcml
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       96 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope/template/zope.conf.promise.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1608 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope/template/zope.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      960 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.zero_knowledge.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3194 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      838 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm/template/kvm_controller_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     9664 2015-08-17 16:54:58.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm/template/kvm_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      189 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm/template/6to4.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/sphinx/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2257 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/sphinx/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/sphinx/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    61948 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/sphinx/template/sphinx.conf.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/postgres/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3910 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/postgres/backup.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     8552 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/postgres/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2508 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/publishurl.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4253 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      193 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/stunnel.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       97 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/stunnel.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      639 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/varnishlogd.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4173 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/default.vcl.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      112 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/varnishlog.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      549 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/varnishd.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/redis/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    72873 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/redis/MyRedis2410.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2723 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/redis/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      425 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/redis/promise.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/redis/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    23474 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/redis/template/redis.conf.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/memcached/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    10385 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/memcached/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/memcached/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      229 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/memcached/template/stunnel.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    10855 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/memcached/template/openssl.cnf.ca.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      100 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/memcached/template/memcached.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3425 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/memcached/certificate_authority.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/sheepdogtestbed/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5049 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/sheepdogtestbed/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/sheepdogtestbed/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      342 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/sheepdogtestbed/template/nosqltester_manager_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      206 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/sheepdogtestbed/template/nosqltester_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     9447 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/softwaretype.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2302 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/symbolic_link.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2108 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/duplicity.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4435 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/downloader.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_update/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3515 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_update/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    14521 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_update/erp5.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      567 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/jsondump.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/haproxy/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      426 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/haproxy/haproxy.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5371 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/haproxy/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/haproxy/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      125 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/haproxy/template/haproxy-server-snippet.cfg.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1205 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/haproxy/template/haproxy.cfg.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      147 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/haproxy/template/haproxy-listen-snippet.cfg.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     9572 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      970 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/innobackupex.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4972 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/mysql.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      265 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/template/initmysql.sql.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      199 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/template/mysql-init-function.sql.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1799 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/template/my.cnf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      244 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1741 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mkdirectory.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    12695 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pbs.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2374 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    13935 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      287 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/template/kumo_server_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      201 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/template/kumo_manager_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      205 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/template/memstrike_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      244 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/template/kumo_gateway_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      473 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/template/kumotester_manager_run.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      440 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/template/nosqltester_manager_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      260 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/template/nosqltester_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       48 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.xwiki.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/6tunnel/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2151 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/6tunnel/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/6tunnel/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      182 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/6tunnel/template/4to6.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      188 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/6tunnel/template/6to4.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/condor/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    12033 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/condor/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2350 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/condor/configure.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    11704 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      229 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/template/stunnel.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    10855 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/template/openssl.cnf.ca.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      159 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/template/kumo_gateway.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      111 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/template/kumo_manager.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      207 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/template/kumo_server.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3425 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kumofs/certificate_authority.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/squid/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3453 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/squid/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/squid/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      868 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/squid/template/squid.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      970 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.seleniumrunner.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/agent/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      300 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/agent/catdatefile.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2574 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/agent/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_kumofs/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3419 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_kumofs/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_kumofs/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      166 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_kumofs/template/kumo_gateway.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      118 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_kumofs/template/kumo_manager.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      214 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_kumofs/template/kumo_server.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5202 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      241 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/template/zope.zeo.entry.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      137 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/template/zope.conf.tidstorage.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      732 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/template/site.zcml
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       87 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/template/zope.conf.timeserver.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       96 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/template/zope.conf.promise.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1425 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_zope_zeo_client/template/zope.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2211 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.librecipe.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3691 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/generatepassword.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_page_content/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2008 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/check_page_content/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_page_content/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      360 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/check_page_content/template/check_page_content.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4684 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      875 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/template/erp5testnode.cfg.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2816 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/template/httpd.conf.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_memcached/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2160 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_memcached/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_memcached/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      107 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_memcached/template/memcached.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       20 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.nbdserver.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/certificate_authority/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5406 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/certificate_authority/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/certificate_authority/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    10855 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/certificate_authority/template/openssl.cnf.ca.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3706 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/certificate_authority/certificate_authority.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/re6stnet/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     8024 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/re6stnet/re6stnet.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     9773 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/re6stnet/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/re6stnet/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       68 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/re6stnet/template/registry-run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3872 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/shellinabox.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_parameter/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2186 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/check_parameter/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_parameter/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      268 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/check_parameter/template/check_ipv6.py.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      435 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/check_parameter/template/check_ipv4.py.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      447 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/check_parameter/template/check_parameter.py.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       46 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.mysql.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/novnc/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2106 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/novnc/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephp/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6730 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephp/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephp/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1883 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephp/template/apache.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      436 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephp/template/php.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       32 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.libcloudrequest.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1208 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.generic_varnish.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheproxy/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2687 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheproxy/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheproxy/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1477 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apacheproxy/template/apache.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    12373 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/ERP5TypeFunctionalTestCase.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1844 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6973 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/erp5functionaltestreporthandler.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5280 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/testrunner.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      159 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/template/xvfb_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       58 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.proactive.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    18592 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      970 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/innobackupex.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2840 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/mysql.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      229 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/stunnel.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       63 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc-core.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1984 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/apache.in.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    10855 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/openssl.cnf.ca.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc_conf/
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc_conf/agent/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1133 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc_conf/agent/config.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1285 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc_conf/mmc.ini.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc_conf/plugins/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      651 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc_conf/plugins/ppolicy.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6261 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mmc_conf/plugins/base.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      161 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/logrotate_entry.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      100 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/memcached.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      233 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/php.ini.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/atftpd/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      761 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/atftpd/pcre.conf.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/launchers/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      309 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/launchers/log_launcher_01.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4914 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/launchers/launchers.ini.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/package-server/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      387 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/package-server/plugin_terminal_type.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6285 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/package-server/package-server.ini.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/scheduler/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5116 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/scheduler/scheduler.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1184 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/p2ipc-windows.ini.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/imaging-server/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3196 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/imaging-server/imaging-server.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      302 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/p2ipc.ini.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/inventory-server/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1519 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/pulse2/inventory-server/inventory-server.ini.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      198 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/pulse2.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2544 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/inventory.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      735 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/dyngroup.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4439 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/msc.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1651 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/glpi.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      944 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/imaging.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      169 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/pulse2_conf/plugins/pkgs.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1521 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/my.cnf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      391 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/mysqlinit.sql.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3425 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/certificate_authority.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      559 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/pulse2/apache.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       26 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.erp5testnode.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       88 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.libcloud.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5scalabilitytestbed/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4678 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5scalabilitytestbed/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5scalabilitytestbed/template/
--rwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)      355 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5scalabilitytestbed/template/nosqltester_run.in
--rwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)      490 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5scalabilitytestbed/template/erp5tester_manager_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2088 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/_uuid.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    11082 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/request.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3601 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zero_knowledge.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3042 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/publish.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3110 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lockfile.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       24 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.zabbixagent.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2107 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/equeue.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/simplehttpserver/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3458 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/simplehttpserver/simplehttpserver.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2904 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/simplehttpserver/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2249 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/copyfilelist.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5709 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/sshkeys_authority.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       22 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.slaprunner.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_bootstrap/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2432 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_bootstrap/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_bootstrap/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      869 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_bootstrap/template/erp5_bootstrap.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     8693 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/trac.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4021 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      282 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/template/snippet.ssl.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1938 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/template/apache.zope.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      122 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/template/vhost.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      149 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/template/snippet.ssl.ca.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      559 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/apache.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/addresiliency/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2600 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/addresiliency/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3819 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/addresiliency/takeover.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/slapreport/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2107 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/slapreport/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2170 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/readline.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    12756 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      937 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/runner.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2854 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/mysql.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      170 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/template/stunnel.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2007 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/template/apache.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      438 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/template/php.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1536 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/template/my.cnf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      391 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/template/mysqlinit.sql.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      559 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lamp/apache.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2051 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/shell.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2011 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/_urlparse.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4725 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.kvm.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     9140 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/slapconfiguration.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_promise/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2295 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5_promise/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1633 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/signal_wrapper.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/boinc/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    17872 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/boinc/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    13192 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/boinc/configure.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/boinc/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      453 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/boinc/template/project_config.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      458 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/boinc/template/sed_update.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6964 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      129 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/initmysql.sql.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     7112 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/hibernate.cfg.xml.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       70 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/mysqld.bin
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1536 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/my.cnf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6832 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/tomcat-server.xml.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1754 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.kvm_frontend.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     8207 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      124 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/template/apache.zope.conf.path-protected.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       83 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/template/apache.zope.conf.path.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      270 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/template/apache.ssl-snippet.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1855 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/template/apache.zope.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      101 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/template/apache.location-snippet.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      559 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/erp5/apache.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/mioga/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)        0 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mioga/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)    11909 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mioga/instantiate.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       12 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.vifib.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2170 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generatemac.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4101 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.lamp.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2106 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/gitinit.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1753 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/waitfor.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephpconfigure/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5526 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephpconfigure/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      954 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/apachephpconfigure/runner.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/web_checker/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2692 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/web_checker/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/web_checker/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1056 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/web_checker/template/web_checker.cfg.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/tidstorage/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2232 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/tidstorage/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/tidstorage/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      344 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/tidstorage/template/tidstorage.py.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3312 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/publish_early.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/libcloud/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5060 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/libcloud/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      156 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/libcloud/run.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/libcloud/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)        0 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/libcloud/template/cloudmgr.cnf.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_port_listening/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1845 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/check_port_listening/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_port_listening/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      365 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/check_port_listening/template/socket_connection_attempt.py.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/zeo/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3668 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zeo/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/zeo/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       81 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zeo/template/zeo-filestorage-snippet.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      239 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zeo/template/zeo.conf.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/onetimeupload/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2037 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/onetimeupload/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/onetimeupload/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      187 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/onetimeupload/template/onetimeupload_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       20 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.siptester.txt
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4098 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      416 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/template/os_config.xml.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      512 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/template/accords.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      308 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/template/testos.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      500 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/template/coips.xml.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3581 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/accords/accords.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_cloudooo/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2835 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_cloudooo/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_cloudooo/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2027 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/generic_cloudooo/template/cloudooo.cfg.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/zimbra_kvm/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2632 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zimbra_kvm/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/zimbra_kvm/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      712 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zimbra_kvm/template/kvm_controller_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1452 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zimbra_kvm/template/kvm_run.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm_frontend/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5813 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm_frontend/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm_frontend/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     4592 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm_frontend/template/kvm-proxy.js
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      250 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/kvm_frontend/template/nodejs_run.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2812 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/switch_softwaretype.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/mysql/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       29 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mysql/backup.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     6538 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mysql/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2844 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mysql/mysql.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/mysql/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      256 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mysql/template/initmysql.sql.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1480 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mysql/template/my.cnf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      548 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/libcloudrequest.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/stunnel/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3397 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/stunnel/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/stunnel/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      187 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/stunnel/template/server.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      170 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/stunnel/template/client.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      622 2015-08-10 09:02:42.000000 slapos.cookbook-1.0.9/slapos/recipe/userinfo.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/lampgeneric/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3151 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lampgeneric/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/lampgeneric/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1883 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lampgeneric/template/apache.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      436 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/lampgeneric/template/php.ini.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     3323 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/mydumper.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1315 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/svcdaemon.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      300 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/catdatefile.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5686 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      117 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/template/logrotate_entry.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5934 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/template/zabbix_agentd.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      382 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.mkdirectory.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       39 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.erp5.txt
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     5921 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/dropbear.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/slapmonitor/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2248 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/slapmonitor/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/siptester/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2073 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/siptester/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/siptester/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      196 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/siptester/template/init_caller.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      442 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/siptester/template/pjsua_receiver.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      393 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/siptester/template/pjsua_caller.conf.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      173 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/siptester/template/init_receiver.in
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2650 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/wrapper.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_url_available/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     1970 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/check_url_available/__init__.py
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/check_url_available/template/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)      843 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/check_url_available/template/check_url.in
-drwxr-xr-x   0 slapuser19   (979) slapuser19  (1020)        0 2015-08-17 17:30:57.000000 slapos.cookbook-1.0.9/slapos/recipe/cloud9/
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)     2367 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/cloud9/__init__.py
--rw-r--r--   0 slapuser19   (979) slapuser19  (1020)       32 2015-05-19 14:09:52.000000 slapos.cookbook-1.0.9/slapos/recipe/README.sheepdogtestbed.txt
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/
+-rwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)    10909 2019-02-21 14:13:14.000000 slapos.cookbook-1.0.92/setup.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6243 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/entry_points.txt
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)        1 2019-02-06 16:01:44.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/zip-safe
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)        7 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/top_level.txt
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      131 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/requires.txt
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)        1 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/dependency_links.txt
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     9888 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/SOURCES.txt
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    30727 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/PKG-INFO
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       21 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos.cookbook.egg-info/namespace_packages.txt
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4856 2019-02-21 14:13:14.000000 slapos.cookbook-1.0.92/CHANGES.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      332 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/README.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       38 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/setup.cfg
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/reverse_proxy_nginx/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4064 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/reverse_proxy_nginx/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/reverse_proxy_nginx/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1280 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/reverse_proxy_nginx/template/nginx.conf.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_cloudooo/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5588 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_cloudooo/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_cloudooo/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1342 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_cloudooo/template/cloudooo.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3187 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mydumper.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      963 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/innobackupex.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     9591 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4957 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/mysql.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      199 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/template/mysql-init-function.sql.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      265 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/template/initmysql.sql.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1637 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/template/my.cnf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2736 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.generic_cloudooo.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       88 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.libcloud.rst
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/novnc/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2040 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/novnc/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/sheepdogtestbed/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5049 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/sheepdogtestbed/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/sheepdogtestbed/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      342 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/sheepdogtestbed/template/nosqltester_manager_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      206 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/sheepdogtestbed/template/nosqltester_run.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/check_page_content/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2008 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_page_content/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/check_page_content/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      360 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_page_content/template/check_page_content.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_memcached/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2160 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_memcached/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_memcached/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      107 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_memcached/template/memcached.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      960 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.zero_knowledge.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1788 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/shell.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/cloud9/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2220 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/cloud9/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2172 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_port_listening.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/stunnel/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3123 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/stunnel/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/stunnel/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      187 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/stunnel/template/server.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      170 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/stunnel/template/client.conf.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4573 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3177 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/template/httpd.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      907 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/template/erp5testnode.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    12384 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/pbs.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/lampgeneric/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3093 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lampgeneric/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/lampgeneric/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      436 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lampgeneric/template/php.ini.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1883 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lampgeneric/template/apache.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3942 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zero_knowledge.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5868 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/sshkeys_authority.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/nbdserver/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1948 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nbdserver/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/nbdserver/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      251 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nbdserver/template/nbdserver_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     8693 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/trac.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    12001 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/request.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5_promise/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2295 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5_promise/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      937 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/runner.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      559 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/apache.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    12771 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2854 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/mysql.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      391 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/template/mysqlinit.sql.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      170 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/template/stunnel.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      438 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/template/php.ini.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2007 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/template/apache.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1536 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/lamp/template/my.cnf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5106 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/notifier.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/web_checker/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2692 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/web_checker/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/web_checker/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1056 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/web_checker/template/web_checker.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3499 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/container.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2632 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      712 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/template/kvm_controller_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1452 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/template/kvm_run.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/mysql/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       29 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mysql/backup.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6498 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mysql/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2844 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mysql/mysql.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/mysql/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      256 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mysql/template/initmysql.sql.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1480 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mysql/template/my.cnf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2936 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/logrotate.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/simplehttpserver/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2890 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/simplehttpserver/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3442 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/simplehttpserver/simplehttpserver.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1663 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/condor.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2497 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/configure.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6348 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3073 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/boinc.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/template/
+-rwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)      687 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/template/machineinfo.sh.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    13935 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      201 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/template/kumo_manager_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      244 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/template/kumo_gateway_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      205 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/template/memstrike_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      473 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/template/kumotester_manager_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      287 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/template/kumo_server_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2374 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      440 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/template/nosqltester_manager_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      260 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/template/nosqltester_run.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/postgres/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3910 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/postgres/backup.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     8804 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/postgres/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    11068 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/softwaretype.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/check_parameter/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2186 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_parameter/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/check_parameter/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      453 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_parameter/template/check_parameter.py.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      435 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_parameter/template/check_ipv4.py.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      268 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_parameter/template/check_ipv6.py.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/addresiliency/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2461 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/addresiliency/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3084 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/addresiliency/takeover.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/haproxy/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      425 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/haproxy/haproxy.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5291 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/haproxy/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/haproxy/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1205 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/haproxy/template/haproxy.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      154 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/haproxy/template/haproxy-listen-snippet.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      125 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/haproxy/template/haproxy-server-snippet.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2011 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/_urlparse.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1956 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mkdirectory.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/zeo/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3603 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zeo/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/zeo/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      239 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zeo/template/zeo.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       81 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zeo/template/zeo-filestorage-snippet.conf.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/boinc/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    12711 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/boinc/configure.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    17476 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/boinc/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/boinc/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      458 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/boinc/template/sed_update.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      453 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/boinc/template/project_config.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      470 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/shlex.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3350 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/genericslap.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4083 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/execute.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1863 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/inotify.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3218 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/filehash.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    12378 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     9305 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/librecipe/generic.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5scalabilitytestbed/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4678 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5scalabilitytestbed/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5scalabilitytestbed/template/
+-rwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)      355 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5scalabilitytestbed/template/nosqltester_run.in
+-rwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)      490 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5scalabilitytestbed/template/erp5tester_manager_run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5406 2019-02-21 14:13:14.000000 slapos.cookbook-1.0.92/slapos/recipe/promise_plugin.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2106 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/gitinit.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      637 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/userinfo.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1970 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/equeue.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2249 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/copyfilelist.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/re6stnet/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     7343 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/re6stnet/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/re6stnet/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       68 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/re6stnet/template/registry-run.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6770 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/re6stnet/re6stnet.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1798 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/simplelogger.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/onetimeupload/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2037 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/onetimeupload/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/onetimeupload/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      187 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/onetimeupload/template/onetimeupload_run.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/libcloud/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      156 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/libcloud/run.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5060 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/libcloud/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/libcloud/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/libcloud/template/cloudmgr.cnf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3924 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/free_port.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephp/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6660 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephp/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephp/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      436 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephp/template/php.ini.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1883 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephp/template/apache.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      567 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/jsondump.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2211 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.librecipe.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2088 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/_uuid.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/condor/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2338 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/condor/configure.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    11780 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/condor/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1637 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/signal_wrapper.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/mioga/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    11747 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mioga/instantiate.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/mioga/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2812 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/switch_softwaretype.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/fontconfig/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2600 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/fontconfig/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/fontconfig/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       32 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/fontconfig/template/fontconfig-snippet.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      153 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/fontconfig/template/fontconfig.cfg.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    10960 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/slapconfiguration.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4678 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/dropbear.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1860 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.kvm_frontend.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3457 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/wrapper.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2302 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/symbolic_link.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/6tunnel/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2151 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/6tunnel/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/6tunnel/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      182 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/6tunnel/template/4to6.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      188 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/6tunnel/template/6to4.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4735 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.kvm.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2170 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/readline.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6140 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/random.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      244 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/kvm_frontend/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5813 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/kvm_frontend/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/kvm_frontend/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4592 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/kvm_frontend/template/kvm-proxy.js
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      250 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/kvm_frontend/template/nodejs_run.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/squid/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3231 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/squid/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/squid/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      868 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/squid/template/squid.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3228 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/publish.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2029 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/duplicity.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3312 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/publish_early.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3581 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/accords.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4099 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      512 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/template/accords.ini.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      500 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/template/coips.xml.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      308 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/template/testos.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      416 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/accords/template/os_config.xml.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheproxy/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2629 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheproxy/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheproxy/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1477 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheproxy/template/apache.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6964 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      129 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/initmysql.sql.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       70 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/mysqld.bin
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     7112 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/hibernate.cfg.xml.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6832 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/tomcat-server.xml.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1536 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/my.cnf.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/check_url_available/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2343 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_url_available/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/check_url_available/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1364 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/check_url_available/template/check_url.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1315 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/svcdaemon.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5720 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      117 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/template/logrotate_entry.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5934 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/template/zabbix_agentd.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      300 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/catdatefile.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4772 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/dcron.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_kumofs/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3419 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_kumofs/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_kumofs/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      214 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_kumofs/template/kumo_server.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      166 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_kumofs/template/kumo_gateway.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      118 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_kumofs/template/kumo_manager.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/proactive/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3302 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/proactive/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/proactive/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      422 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/proactive/template/ProActiveConfiguration.xml.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     1203 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.generic_varnish.rst
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      382 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.mkdirectory.rst
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/siptester/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2073 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/siptester/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/siptester/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      442 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/siptester/template/pjsua_receiver.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      196 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/siptester/template/init_caller.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      393 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/siptester/template/pjsua_caller.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      173 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/siptester/template/init_receiver.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/tidstorage/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2124 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/tidstorage/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/tidstorage/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      344 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/tidstorage/template/tidstorage.py.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      548 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/libcloudrequest.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4336 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/README.lamp.rst
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3574 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/certificate_authority.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     6218 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    10855 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/template/openssl.cnf.ca.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephpconfigure/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      791 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephpconfigure/runner.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     5526 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apachephpconfigure/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheperl/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2733 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheperl/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheperl/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2009 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/apacheperl/template/apache.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5_test/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2354 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5_test/test.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2177 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/erp5_test/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/sphinx/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2202 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/sphinx/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/sphinx/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    61948 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/sphinx/template/sphinx.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2508 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/publishurl.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4004 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/neoppod.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4253 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)       97 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/stunnel.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      193 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/stunnel.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      112 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/varnishlog.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      549 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/varnishd.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4173 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/default.vcl.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      639 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/varnishlogd.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/redis/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    72873 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/redis/MyRedis2410.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3182 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/redis/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/redis/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    36283 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/redis/template/redis.conf.in
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/davstorage/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4550 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/davstorage/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/recipe/davstorage/template/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     3792 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/davstorage/template/httpd.conf.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      456 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/recipe/davstorage/template/php.ini.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      244 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/__init__.py
+drwxr-xr-x   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/slapos/test/
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     4465 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/test/test_json_schema.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      413 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/test/test_recipe.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)        0 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/test/__init__.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)     2257 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/slapos/test/utils.py
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)      216 2019-02-05 15:37:10.000000 slapos.cookbook-1.0.92/MANIFEST.in
+-rw-r--r--   0 slapuser11   (987) slapuser11  (1012)    30727 2019-02-21 14:16:30.000000 slapos.cookbook-1.0.92/PKG-INFO
```

### Comparing `slapos.cookbook-1.0.9/slapos.cookbook.egg-info/SOURCES.txt` & `slapos.cookbook-1.0.92/slapos.cookbook.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,79 @@
-CHANGES.txt
+CHANGES.rst
 MANIFEST.in
-README.txt
+README.rst
 setup.py
 slapos/__init__.py
 slapos.cookbook.egg-info/PKG-INFO
 slapos.cookbook.egg-info/SOURCES.txt
 slapos.cookbook.egg-info/dependency_links.txt
 slapos.cookbook.egg-info/entry_points.txt
 slapos.cookbook.egg-info/namespace_packages.txt
 slapos.cookbook.egg-info/requires.txt
 slapos.cookbook.egg-info/top_level.txt
 slapos.cookbook.egg-info/zip-safe
-slapos/recipe/README.cloudooo.txt
-slapos/recipe/README.erp5.txt
-slapos/recipe/README.erp5testnode.txt
-slapos/recipe/README.generic_varnish.txt
-slapos/recipe/README.kumofs.txt
-slapos/recipe/README.kvm.txt
-slapos/recipe/README.kvm_frontend.txt
-slapos/recipe/README.lamp.txt
-slapos/recipe/README.libcloud.txt
-slapos/recipe/README.libcloudrequest.txt
-slapos/recipe/README.librecipe.txt
-slapos/recipe/README.memcached.txt
-slapos/recipe/README.mkdirectory.txt
-slapos/recipe/README.mysql.txt
-slapos/recipe/README.nbdserver.txt
-slapos/recipe/README.nosqltestbed.txt
-slapos/recipe/README.proactive.txt
-slapos/recipe/README.seleniumrunner.txt
-slapos/recipe/README.sheepdogtestbed.txt
-slapos/recipe/README.siptester.txt
-slapos/recipe/README.slaprunner.txt
-slapos/recipe/README.vifib.txt
-slapos/recipe/README.xwiki.txt
-slapos/recipe/README.zabbixagent.txt
-slapos/recipe/README.zero_knowledge.txt
+slapos/recipe/README.generic_cloudooo.rst
+slapos/recipe/README.generic_varnish.rst
+slapos/recipe/README.kvm.rst
+slapos/recipe/README.kvm_frontend.rst
+slapos/recipe/README.lamp.rst
+slapos/recipe/README.libcloud.rst
+slapos/recipe/README.librecipe.rst
+slapos/recipe/README.mkdirectory.rst
+slapos/recipe/README.zero_knowledge.rst
 slapos/recipe/__init__.py
 slapos/recipe/_urlparse.py
 slapos/recipe/_uuid.py
+slapos/recipe/check_port_listening.py
 slapos/recipe/container.py
 slapos/recipe/copyfilelist.py
 slapos/recipe/dcron.py
-slapos/recipe/downloader.py
 slapos/recipe/dropbear.py
 slapos/recipe/duplicity.py
 slapos/recipe/equeue.py
-slapos/recipe/generatemac.py
-slapos/recipe/generatepassword.py
+slapos/recipe/free_port.py
 slapos/recipe/gitinit.py
 slapos/recipe/jsondump.py
 slapos/recipe/libcloudrequest.py
-slapos/recipe/lockfile.py
 slapos/recipe/logrotate.py
 slapos/recipe/mkdirectory.py
 slapos/recipe/mydumper.py
 slapos/recipe/neoppod.py
 slapos/recipe/notifier.py
 slapos/recipe/pbs.py
+slapos/recipe/promise_plugin.py
 slapos/recipe/publish.py
 slapos/recipe/publish_early.py
 slapos/recipe/publishurl.py
+slapos/recipe/random.py
 slapos/recipe/readline.py
 slapos/recipe/request.py
 slapos/recipe/shell.py
-slapos/recipe/shellinabox.py
 slapos/recipe/signal_wrapper.py
 slapos/recipe/simplelogger.py
 slapos/recipe/slapconfiguration.py
 slapos/recipe/softwaretype.py
 slapos/recipe/sshkeys_authority.py
 slapos/recipe/switch_softwaretype.py
 slapos/recipe/symbolic_link.py
 slapos/recipe/trac.py
 slapos/recipe/userinfo.py
-slapos/recipe/vifib.py
-slapos/recipe/waitfor.py
 slapos/recipe/wrapper.py
 slapos/recipe/zero_knowledge.py
 slapos/recipe/6tunnel/__init__.py
 slapos/recipe/6tunnel/template/4to6.in
 slapos/recipe/6tunnel/template/6to4.in
 slapos/recipe/accords/__init__.py
 slapos/recipe/accords/accords.py
 slapos/recipe/accords/template/accords.ini.in
 slapos/recipe/accords/template/coips.xml.in
 slapos/recipe/accords/template/os_config.xml.in
 slapos/recipe/accords/template/testos.in
 slapos/recipe/addresiliency/__init__.py
 slapos/recipe/addresiliency/takeover.py
-slapos/recipe/agent/__init__.py
-slapos/recipe/agent/catdatefile.py
-slapos/recipe/apache_zope_backend/__init__.py
-slapos/recipe/apache_zope_backend/apache.py
-slapos/recipe/apache_zope_backend/template/apache.zope.conf.in
-slapos/recipe/apache_zope_backend/template/snippet.ssl.ca.in
-slapos/recipe/apache_zope_backend/template/snippet.ssl.in
-slapos/recipe/apache_zope_backend/template/vhost.in
 slapos/recipe/apacheperl/__init__.py
 slapos/recipe/apacheperl/template/apache.in
 slapos/recipe/apachephp/__init__.py
 slapos/recipe/apachephp/template/apache.in
 slapos/recipe/apachephp/template/php.ini.in
 slapos/recipe/apachephpconfigure/__init__.py
 slapos/recipe/apachephpconfigure/runner.py
@@ -120,52 +93,34 @@
 slapos/recipe/certificate_authority/template/openssl.cnf.ca.in
 slapos/recipe/check_page_content/__init__.py
 slapos/recipe/check_page_content/template/check_page_content.in
 slapos/recipe/check_parameter/__init__.py
 slapos/recipe/check_parameter/template/check_ipv4.py.in
 slapos/recipe/check_parameter/template/check_ipv6.py.in
 slapos/recipe/check_parameter/template/check_parameter.py.in
-slapos/recipe/check_port_listening/__init__.py
-slapos/recipe/check_port_listening/template/socket_connection_attempt.py.in
 slapos/recipe/check_url_available/__init__.py
 slapos/recipe/check_url_available/template/check_url.in
 slapos/recipe/cloud9/__init__.py
 slapos/recipe/condor/__init__.py
 slapos/recipe/condor/configure.py
-slapos/recipe/configurationfile/__init__.py
 slapos/recipe/davstorage/__init__.py
 slapos/recipe/davstorage/template/httpd.conf.in
 slapos/recipe/davstorage/template/php.ini.in
-slapos/recipe/erp5/__init__.py
-slapos/recipe/erp5/apache.py
-slapos/recipe/erp5/template/apache.location-snippet.conf.in
-slapos/recipe/erp5/template/apache.ssl-snippet.conf.in
-slapos/recipe/erp5/template/apache.zope.conf.in
-slapos/recipe/erp5/template/apache.zope.conf.path-protected.in
-slapos/recipe/erp5/template/apache.zope.conf.path.in
-slapos/recipe/erp5_bootstrap/__init__.py
-slapos/recipe/erp5_bootstrap/template/erp5_bootstrap.in
 slapos/recipe/erp5_promise/__init__.py
 slapos/recipe/erp5_test/__init__.py
 slapos/recipe/erp5_test/test.py
-slapos/recipe/erp5_update/__init__.py
-slapos/recipe/erp5_update/erp5.py
 slapos/recipe/erp5scalabilitytestbed/__init__.py
 slapos/recipe/erp5scalabilitytestbed/template/erp5tester_manager_run.in
 slapos/recipe/erp5scalabilitytestbed/template/nosqltester_run.in
 slapos/recipe/erp5testnode/__init__.py
 slapos/recipe/erp5testnode/template/erp5testnode.cfg.in
 slapos/recipe/erp5testnode/template/httpd.conf.in
-slapos/recipe/firefox/__init__.py
-slapos/recipe/firefox/template/firefox_run.in
-slapos/recipe/firefox/template/prefs.js
 slapos/recipe/fontconfig/__init__.py
 slapos/recipe/fontconfig/template/fontconfig-snippet.cfg.in
 slapos/recipe/fontconfig/template/fontconfig.cfg.in
-slapos/recipe/fontconfig/template/onetimedownload_run.in
 slapos/recipe/generic_cloudooo/__init__.py
 slapos/recipe/generic_cloudooo/template/cloudooo.cfg.in
 slapos/recipe/generic_kumofs/__init__.py
 slapos/recipe/generic_kumofs/template/kumo_gateway.in
 slapos/recipe/generic_kumofs/template/kumo_manager.in
 slapos/recipe/generic_kumofs/template/kumo_server.in
 slapos/recipe/generic_memcached/__init__.py
@@ -179,41 +134,19 @@
 slapos/recipe/generic_varnish/__init__.py
 slapos/recipe/generic_varnish/template/default.vcl.in
 slapos/recipe/generic_varnish/template/stunnel.conf.in
 slapos/recipe/generic_varnish/template/stunnel.in
 slapos/recipe/generic_varnish/template/varnishd.in
 slapos/recipe/generic_varnish/template/varnishlog.in
 slapos/recipe/generic_varnish/template/varnishlogd.in
-slapos/recipe/generic_zope/__init__.py
-slapos/recipe/generic_zope/template/site.zcml
-slapos/recipe/generic_zope/template/zope.conf.in
-slapos/recipe/generic_zope/template/zope.conf.promise.in
-slapos/recipe/generic_zope_zeo_client/__init__.py
-slapos/recipe/generic_zope_zeo_client/template/site.zcml
-slapos/recipe/generic_zope_zeo_client/template/zope.conf.in
-slapos/recipe/generic_zope_zeo_client/template/zope.conf.promise.in
-slapos/recipe/generic_zope_zeo_client/template/zope.conf.tidstorage.in
-slapos/recipe/generic_zope_zeo_client/template/zope.conf.timeserver.in
-slapos/recipe/generic_zope_zeo_client/template/zope.zeo.entry.conf.in
 slapos/recipe/haproxy/__init__.py
 slapos/recipe/haproxy/haproxy.py
 slapos/recipe/haproxy/template/haproxy-listen-snippet.cfg.in
 slapos/recipe/haproxy/template/haproxy-server-snippet.cfg.in
 slapos/recipe/haproxy/template/haproxy.cfg.in
-slapos/recipe/kumofs/__init__.py
-slapos/recipe/kumofs/certificate_authority.py
-slapos/recipe/kumofs/template/kumo_gateway.in
-slapos/recipe/kumofs/template/kumo_manager.in
-slapos/recipe/kumofs/template/kumo_server.in
-slapos/recipe/kumofs/template/openssl.cnf.ca.in
-slapos/recipe/kumofs/template/stunnel.conf.in
-slapos/recipe/kvm/__init__.py
-slapos/recipe/kvm/template/6to4.in
-slapos/recipe/kvm/template/kvm_controller_run.in
-slapos/recipe/kvm/template/kvm_run.in
 slapos/recipe/kvm_frontend/__init__.py
 slapos/recipe/kvm_frontend/template/kvm-proxy.js
 slapos/recipe/kvm_frontend/template/nodejs_run.in
 slapos/recipe/lamp/__init__.py
 slapos/recipe/lamp/apache.py
 slapos/recipe/lamp/mysql.py
 slapos/recipe/lamp/runner.py
@@ -231,19 +164,14 @@
 slapos/recipe/librecipe/__init__.py
 slapos/recipe/librecipe/execute.py
 slapos/recipe/librecipe/filehash.py
 slapos/recipe/librecipe/generic.py
 slapos/recipe/librecipe/genericslap.py
 slapos/recipe/librecipe/inotify.py
 slapos/recipe/librecipe/shlex.py
-slapos/recipe/memcached/__init__.py
-slapos/recipe/memcached/certificate_authority.py
-slapos/recipe/memcached/template/memcached.in
-slapos/recipe/memcached/template/openssl.cnf.ca.in
-slapos/recipe/memcached/template/stunnel.conf.in
 slapos/recipe/mioga/__init__.py
 slapos/recipe/mioga/instantiate.py
 slapos/recipe/mysql/__init__.py
 slapos/recipe/mysql/backup.py
 slapos/recipe/mysql/mysql.py
 slapos/recipe/mysql/template/initmysql.sql.in
 slapos/recipe/mysql/template/my.cnf.in
@@ -261,89 +189,43 @@
 slapos/recipe/novnc/__init__.py
 slapos/recipe/onetimeupload/__init__.py
 slapos/recipe/onetimeupload/template/onetimeupload_run.in
 slapos/recipe/postgres/__init__.py
 slapos/recipe/postgres/backup.py
 slapos/recipe/proactive/__init__.py
 slapos/recipe/proactive/template/ProActiveConfiguration.xml.in
-slapos/recipe/pulse2/__init__.py
-slapos/recipe/pulse2/apache.py
-slapos/recipe/pulse2/certificate_authority.py
-slapos/recipe/pulse2/innobackupex.py
-slapos/recipe/pulse2/mysql.py
-slapos/recipe/pulse2/template/apache.in.in
-slapos/recipe/pulse2/template/logrotate_entry.in
-slapos/recipe/pulse2/template/memcached.in
-slapos/recipe/pulse2/template/mmc-core.in
-slapos/recipe/pulse2/template/my.cnf.in
-slapos/recipe/pulse2/template/mysqlinit.sql.in
-slapos/recipe/pulse2/template/openssl.cnf.ca.in
-slapos/recipe/pulse2/template/php.ini.in
-slapos/recipe/pulse2/template/stunnel.conf.in
-slapos/recipe/pulse2/template/mmc_conf/mmc.ini.in
-slapos/recipe/pulse2/template/mmc_conf/agent/config.ini.in
-slapos/recipe/pulse2/template/mmc_conf/plugins/base.ini.in
-slapos/recipe/pulse2/template/mmc_conf/plugins/ppolicy.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/plugins/dyngroup.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/plugins/glpi.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/plugins/imaging.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/plugins/inventory.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/plugins/msc.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/plugins/pkgs.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/plugins/pulse2.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/p2ipc-windows.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/p2ipc.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/atftpd/pcre.conf.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/imaging-server/imaging-server.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/inventory-server/inventory-server.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/launchers/launchers.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/launchers/log_launcher_01.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/package-server/package-server.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/package-server/plugin_terminal_type.ini.in
-slapos/recipe/pulse2/template/pulse2_conf/pulse2/scheduler/scheduler.ini.in
 slapos/recipe/re6stnet/__init__.py
 slapos/recipe/re6stnet/re6stnet.py
 slapos/recipe/re6stnet/template/registry-run.in
 slapos/recipe/redis/MyRedis2410.py
 slapos/recipe/redis/__init__.py
-slapos/recipe/redis/promise.py
 slapos/recipe/redis/template/redis.conf.in
 slapos/recipe/reverse_proxy_nginx/__init__.py
 slapos/recipe/reverse_proxy_nginx/template/nginx.conf.in
-slapos/recipe/seleniumrunner/ERP5TypeFunctionalTestCase.py
-slapos/recipe/seleniumrunner/__init__.py
-slapos/recipe/seleniumrunner/erp5functionaltestreporthandler.py
-slapos/recipe/seleniumrunner/testrunner.py
-slapos/recipe/seleniumrunner/template/xvfb_run.in
 slapos/recipe/sheepdogtestbed/__init__.py
 slapos/recipe/sheepdogtestbed/template/nosqltester_manager_run.in
 slapos/recipe/sheepdogtestbed/template/nosqltester_run.in
 slapos/recipe/simplehttpserver/__init__.py
 slapos/recipe/simplehttpserver/simplehttpserver.py
 slapos/recipe/siptester/__init__.py
 slapos/recipe/siptester/template/init_caller.in
 slapos/recipe/siptester/template/init_receiver.in
 slapos/recipe/siptester/template/pjsua_caller.conf.in
 slapos/recipe/siptester/template/pjsua_receiver.conf.in
-slapos/recipe/slapmonitor/__init__.py
-slapos/recipe/slapreport/__init__.py
 slapos/recipe/sphinx/__init__.py
 slapos/recipe/sphinx/template/sphinx.conf.in
 slapos/recipe/squid/__init__.py
 slapos/recipe/squid/template/squid.conf.in
 slapos/recipe/stunnel/__init__.py
 slapos/recipe/stunnel/template/client.conf.in
 slapos/recipe/stunnel/template/server.conf.in
 slapos/recipe/tidstorage/__init__.py
 slapos/recipe/tidstorage/template/tidstorage.py.in
 slapos/recipe/web_checker/__init__.py
 slapos/recipe/web_checker/template/web_checker.cfg.in
-slapos/recipe/xvfb/__init__.py
-slapos/recipe/xvfb/template/xvfb_run.in
-slapos/recipe/xvfb/template/xwd_run.in
 slapos/recipe/xwiki/__init__.py
 slapos/recipe/xwiki/template/hibernate.cfg.xml.in
 slapos/recipe/xwiki/template/initmysql.sql.in
 slapos/recipe/xwiki/template/my.cnf.in
 slapos/recipe/xwiki/template/mysqld.bin
 slapos/recipe/xwiki/template/tomcat-server.xml.in
 slapos/recipe/zabbixagent/__init__.py
@@ -355,8 +237,9 @@
 slapos/recipe/zeo/template/zeo-filestorage-snippet.conf.in
 slapos/recipe/zeo/template/zeo.conf.in
 slapos/recipe/zimbra_kvm/__init__.py
 slapos/recipe/zimbra_kvm/template/kvm_controller_run.in
 slapos/recipe/zimbra_kvm/template/kvm_run.in
 slapos/test/__init__.py
 slapos/test/test_json_schema.py
-slapos/test/test_recipe.py
+slapos/test/test_recipe.py
+slapos/test/utils.py
```

### Comparing `slapos.cookbook-1.0.9/slapos.cookbook.egg-info/entry_points.txt` & `slapos.cookbook-1.0.92/slapos.cookbook.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,153 +1,131 @@
 [slapos.recipe.nosqltestbed.plugin]
 kumo = slapos.recipe.nosqltestbed.kumo:KumoTestBed
 
 [zc.buildout]
-equeue = slapos.recipe.equeue:Recipe
+accords = slapos.recipe.accords:Recipe
+addresiliency = slapos.recipe.addresiliency:Recipe
+apacheperl = slapos.recipe.apacheperl:Recipe
+apachephp = slapos.recipe.apachephp:Recipe
+apachephpconfigure = slapos.recipe.apachephpconfigure:Recipe
+apacheproxy = slapos.recipe.apacheproxy:Recipe
+boinc = slapos.recipe.boinc:Recipe
 boinc.app = slapos.recipe.boinc:App
-lamp.simple = slapos.recipe.lamp:Simple
-dumpmdb = slapos.recipe.dumpmdb:Recipe
-neoppod.master = slapos.recipe.neoppod:Master
-zimbra.kvm = slapos.recipe.zimbra_kvm:Recipe
-stunnel = slapos.recipe.stunnel:Recipe
-dropbear.add_authorized_key = slapos.recipe.dropbear:AddAuthorizedKey
-slapreport = slapos.recipe.slapreport:Recipe
-mysql = slapos.recipe.mysql:Recipe
-libcloud = slapos.recipe.libcloud:Recipe
-zero-knowledge.read = slapos.recipe.zero_knowledge:ReadRecipe
-generate.mac = slapos.recipe.generatemac:Recipe
-nbdserver = slapos.recipe.nbdserver:Recipe
-uuid = slapos.recipe._uuid:Recipe
-condor = slapos.recipe.condor:Recipe
-seleniumrunner = slapos.recipe.seleniumrunner:Recipe
+boinc.client = slapos.recipe.boinc:Client
+bonjourgrid = slapos.recipe.bonjourgrid:Recipe
+bonjourgrid.client = slapos.recipe.bonjourgrid:Client
+certificate_authority = slapos.recipe.certificate_authority:Recipe
+certificate_authority.request = slapos.recipe.certificate_authority:Request
+check_page_content = slapos.recipe.check_page_content:Recipe
+check_parameter = slapos.recipe.check_parameter:Recipe
+check_port_listening = slapos.recipe.check_port_listening:Recipe
 check_url_available = slapos.recipe.check_url_available:Recipe
 cloud9 = slapos.recipe.cloud9:Recipe
-fontconfig = slapos.recipe.fontconfig:Recipe
-dropbear = slapos.recipe.dropbear:Recipe
-shellinabox = slapos.recipe.shellinabox:Recipe
+cloudooo.test = slapos.recipe.erp5_test:CloudoooRecipe
+condor = slapos.recipe.condor:Recipe
+condor.submit = slapos.recipe.condor:AppSubmit
 copyfilelist = slapos.recipe.copyfilelist:Recipe
+cron = slapos.recipe.dcron:Recipe
+cron.d = slapos.recipe.dcron:Part
+davstorage = slapos.recipe.davstorage:Recipe
+dropbear = slapos.recipe.dropbear:Recipe
+dropbear.add_authorized_key = slapos.recipe.dropbear:AddAuthorizedKey
+dropbear.client = slapos.recipe.dropbear:Client
+duplicity = slapos.recipe.duplicity:Recipe
+equeue = slapos.recipe.equeue:Recipe
+erp5.promise = slapos.recipe.erp5_promise:Recipe
+erp5scalabilitytestbed = slapos.recipe.erp5scalabilitytestbed:Recipe
+erp5testnode = slapos.recipe.erp5testnode:Recipe
+fontconfig = slapos.recipe.fontconfig:Recipe
+free_port = slapos.recipe.free_port:Recipe
+generate.mac = slapos.recipe.random:Mac
+generate.password = slapos.recipe.random:Password
+generic.cloudooo = slapos.recipe.generic_cloudooo:Recipe
+generic.kumofs = slapos.recipe.generic_kumofs:Recipe
+generic.memcached = slapos.recipe.generic_memcached:Recipe
 generic.mysql = slapos.recipe.generic_mysql:Recipe
-mydumper = slapos.recipe.mydumper:Recipe
+generic.mysql.wrap_mysqld = slapos.recipe.generic_mysql:WrapMySQLd
+generic.mysql.wrap_update_mysql = slapos.recipe.generic_mysql:WrapUpdateMySQL
 generic.varnish = slapos.recipe.generic_varnish:Recipe
-zeo = slapos.recipe.zeo:Recipe
-cron.d = slapos.recipe.dcron:Part
-neoppod.storage = slapos.recipe.neoppod:Storage
-certificate_authority = slapos.recipe.certificate_authority:Recipe
-slapcontainer = slapos.recipe.container:Recipe
-notifier.callback = slapos.recipe.notifier:Callback
-pbs = slapos.recipe.pbs:Recipe
-mioga.instantiate = slapos.recipe.mioga.instantiate:Recipe
-helloworld = slapos.recipe.helloworld:Recipe
-lamp.generic = slapos.recipe.lampgeneric:Recipe
+gitinit = slapos.recipe.gitinit:Recipe
+haproxy = slapos.recipe.haproxy:Recipe
+ipv4toipv6 = slapos.recipe.6tunnel:FourToSix
+ipv6toipv4 = slapos.recipe.6tunnel:SixToFour
 jsondump = slapos.recipe.jsondump:Recipe
-erp5.test = slapos.recipe.erp5_test:Recipe
-apacheproxy = slapos.recipe.apacheproxy:Recipe
-re6stnet.registry = slapos.recipe.re6stnet:Recipe
+kvm.frontend = slapos.recipe.kvm_frontend:Recipe
+lamp = slapos.recipe.lamp:Request
+lamp.generic = slapos.recipe.lampgeneric:Recipe
+lamp.request = slapos.recipe.lamp:Request
+lamp.simple = slapos.recipe.lamp:Simple
+lamp.static = slapos.recipe.lamp:Static
+libcloud = slapos.recipe.libcloud:Recipe
+libcloudrequest = slapos.recipe.libcloudrequest:Recipe
+logrotate = slapos.recipe.logrotate:Recipe
+logrotate.d = slapos.recipe.logrotate:Part
+mioga.instantiate = slapos.recipe.mioga.instantiate:Recipe
+mkdirectory = slapos.recipe.mkdirectory:Recipe
+mydumper = slapos.recipe.mydumper:Recipe
+mysql = slapos.recipe.mysql:Recipe
+nbdserver = slapos.recipe.nbdserver:Recipe
+neoppod.admin = slapos.recipe.neoppod:Admin
+neoppod.master = slapos.recipe.neoppod:Master
+neoppod.storage = slapos.recipe.neoppod:Storage
 nosqltestbed = slapos.recipe.nosqltestbed:NoSQLTestBed
 notifier = slapos.recipe.notifier:Recipe
-generic.kumofs = slapos.recipe.generic_kumofs:Recipe
-cron = slapos.recipe.dcron:Recipe
-logrotate.d = slapos.recipe.logrotate:Part
-requestoptional = slapos.recipe.request:RequestOptional
-slapconfiguration.serialised = slapos.recipe.slapconfiguration:Serialised
-generic.mysql.wrap_update_mysql = slapos.recipe.generic_mysql:WrapUpdateMySQL
-symbolic.link = slapos.recipe.symbolic_link:Recipe
-publish = slapos.recipe.publish:Recipe
-request.edge = slapos.recipe.request:RequestEdge
-zero-knowledge.write = slapos.recipe.zero_knowledge:WriteRecipe
-memcached = slapos.recipe.memcached:Recipe
-slapconfiguration = slapos.recipe.slapconfiguration:Recipe
-check_parameter = slapos.recipe.check_parameter:Recipe
-webchecker = slapos.recipe.web_checker:Recipe
-bonjourgrid = slapos.recipe.bonjourgrid:Recipe
-downloader = slapos.recipe.downloader:Recipe
+notifier.callback = slapos.recipe.notifier:Callback
+notifier.notify = slapos.recipe.notifier:Notify
 novnc = slapos.recipe.novnc:Recipe
-sheepdogtestbed = slapos.recipe.sheepdogtestbed:SheepDogTestBed
-libcloudrequest = slapos.recipe.libcloudrequest:Recipe
-tidstorage = slapos.recipe.tidstorage:Recipe
-lockfile = slapos.recipe.lockfile:Recipe
-haproxy = slapos.recipe.haproxy:Recipe
 onetimeupload = slapos.recipe.onetimeupload:Recipe
-publish.serialised = slapos.recipe.publish:Serialised
-erp5testnode = slapos.recipe.erp5testnode:Recipe
-dropbear.client = slapos.recipe.dropbear:Client
-slapconfiguration.jsondump = slapos.recipe.slapconfiguration:JsonDump
-firefox = slapos.recipe.firefox:Recipe
-duplicity = slapos.recipe.duplicity:Recipe
-xwiki = slapos.recipe.xwiki:Recipe
-boinc.client = slapos.recipe.boinc:Client
-bonjourgrid.client = slapos.recipe.bonjourgrid:Client
-kumofs = slapos.recipe.kumofs:Recipe
-publishurl = slapos.recipe.publishurl:Recipe
-importmdb = slapos.recipe.importmdb:Recipe
-sshkeys_authority = slapos.recipe.sshkeys_authority:Recipe
-request.serialised = slapos.recipe.request:Serialised
-slapmonitor-xml = slapos.recipe.slapmonitor:MonitorXMLRecipe
-java = slapos.recipe.java:Recipe
-generic.memcached = slapos.recipe.generic_memcached:Recipe
-wrapper = slapos.recipe.wrapper:Recipe
-userinfo = slapos.recipe.userinfo:Recipe
-accords = slapos.recipe.accords:Recipe
-generic.zope.zeo.client = slapos.recipe.generic_zope_zeo_client:Recipe
-apachephpconfigure = slapos.recipe.apachephpconfigure:Recipe
-notifier.notify = slapos.recipe.notifier:Notify
-generate.password = slapos.recipe.generatepassword:Recipe
-ipv6toipv4 = slapos.recipe.6tunnel:SixToFour
+pbs = slapos.recipe.pbs:Recipe
+postgres = slapos.recipe.postgres:Recipe
 postgres.export = slapos.recipe.postgres.backup:ExportRecipe
-addresiliency = slapos.recipe.addresiliency:Recipe
-erp5.update = slapos.recipe.erp5_update:Recipe
-apacheperl = slapos.recipe.apacheperl:Recipe
-signalwrapper = slapos.recipe.signal_wrapper:Recipe
-xvfb = slapos.recipe.xvfb:Recipe
-vifib = slapos.recipe.vifib:Recipe
 postgres.import = slapos.recipe.postgres.backup:ImportRecipe
-ipv4toipv6 = slapos.recipe.6tunnel:FourToSix
-switch-softwaretype = slapos.recipe.switch_softwaretype:Recipe
-mkdirectory = slapos.recipe.mkdirectory:Recipe
-redis.server = slapos.recipe.redis:Recipe
-egg_test = slapos.recipe.erp5_test:EggTestRecipe
-neoppod.admin = slapos.recipe.neoppod:Admin
-kvm.frontend = slapos.recipe.kvm_frontend:Recipe
-siptester = slapos.recipe.siptester:SipTesterRecipe
-certificate_authority.request = slapos.recipe.certificate_authority:Request
-apachephp = slapos.recipe.apachephp:Recipe
 proactive = slapos.recipe.proactive:Recipe
-generic.zope = slapos.recipe.generic_zope:Recipe
-cloudooo.test = slapos.recipe.erp5_test:CloudoooRecipe
-simplehttpserver = slapos.recipe.simplehttpserver:Recipe
-check_port_listening = slapos.recipe.check_port_listening:Recipe
-apache.zope.backend = slapos.recipe.apache_zope_backend:Recipe
-squid = slapos.recipe.squid:Recipe
-agent = slapos.recipe.agent:Recipe
-generic.cloudooo = slapos.recipe.generic_cloudooo:Recipe
-generic.mysql.wrap_mysqld = slapos.recipe.generic_mysql:WrapMySQLd
-logrotate = slapos.recipe.logrotate:Recipe
-shell = slapos.recipe.shell:Recipe
-check_page_content = slapos.recipe.check_page_content:Recipe
-configurationfile = slapos.recipe.configurationfile:Recipe
-erp5.bootstrap = slapos.recipe.erp5_bootstrap:Recipe
-postgres = slapos.recipe.postgres:Recipe
-erp5.promise = slapos.recipe.erp5_promise:Recipe
+promise.plugin = slapos.recipe.promise_plugin:Recipe
+publish = slapos.recipe.publish:Recipe
 publish-early = slapos.recipe.publish_early:Recipe
-lamp = slapos.recipe.lamp:Request
-simplelogger = slapos.recipe.simplelogger:Recipe
-sshkeys_authority.request = slapos.recipe.sshkeys_authority:Request
-lamp.static = slapos.recipe.lamp:Static
-condor.submit = slapos.recipe.condor:AppSubmit
-kvm = slapos.recipe.kvm:Recipe
-zabbixagent = slapos.recipe.zabbixagent:Recipe
-trac = slapos.recipe.trac:Recipe
-boinc = slapos.recipe.boinc:Recipe
-gitinit = slapos.recipe.gitinit:Recipe
-reverseproxy.nginx = slapos.recipe.reverse_proxy_nginx:Recipe
+publish.serialised = slapos.recipe.publish:Serialised
 publishsection = slapos.recipe.publish:PublishSection
+publishurl = slapos.recipe.publishurl:Recipe
+random.integer = slapos.recipe.random:Integer
+random.time = slapos.recipe.random:Time
+re6stnet.registry = slapos.recipe.re6stnet:Recipe
 readline = slapos.recipe.readline:Recipe
+redis.server = slapos.recipe.redis:Recipe
+request = slapos.recipe.request:Recipe
+request.edge = slapos.recipe.request:RequestEdge
+request.serialised = slapos.recipe.request:RequestJSONEncoded
+requestoptional = slapos.recipe.request:RequestOptional
+requestoptional.serialised = slapos.recipe.request:RequestOptionalJSONEncoded
+reverseproxy.nginx = slapos.recipe.reverse_proxy_nginx:Recipe
+sheepdogtestbed = slapos.recipe.sheepdogtestbed:SheepDogTestBed
+shell = slapos.recipe.shell:Recipe
+signalwrapper = slapos.recipe.signal_wrapper:Recipe
+simplehttpserver = slapos.recipe.simplehttpserver:Recipe
+simplelogger = slapos.recipe.simplelogger:Recipe
+siptester = slapos.recipe.siptester:SipTesterRecipe
+slapconfiguration = slapos.recipe.slapconfiguration:Recipe
+slapconfiguration.jsondump = slapos.recipe.slapconfiguration:JsonDump
+slapconfiguration.serialised = slapos.recipe.slapconfiguration:Serialised
+slapcontainer = slapos.recipe.container:Recipe
 softwaretype = slapos.recipe.softwaretype:Recipe
 sphinx = slapos.recipe.sphinx:Recipe
-erp5scalabilitytestbed = slapos.recipe.erp5scalabilitytestbed:Recipe
-waitfor = slapos.recipe.waitfor:Recipe
-request = slapos.recipe.request:Recipe
+squid = slapos.recipe.squid:Recipe
+sshkeys_authority = slapos.recipe.sshkeys_authority:Recipe
+sshkeys_authority.request = slapos.recipe.sshkeys_authority:Request
+stunnel = slapos.recipe.stunnel:Recipe
+switch-softwaretype = slapos.recipe.switch_softwaretype:Recipe
+symbolic.link = slapos.recipe.symbolic_link:Recipe
+tidstorage = slapos.recipe.tidstorage:Recipe
+trac = slapos.recipe.trac:Recipe
 urlparse = slapos.recipe._urlparse:Recipe
-lamp.request = slapos.recipe.lamp:Request
-davstorage = slapos.recipe.davstorage:Recipe
-slapmonitor = slapos.recipe.slapmonitor:MonitorRecipe
+userinfo = slapos.recipe.userinfo:Recipe
+uuid = slapos.recipe._uuid:Recipe
+webchecker = slapos.recipe.web_checker:Recipe
+wrapper = slapos.recipe.wrapper:Recipe
+xwiki = slapos.recipe.xwiki:Recipe
+zabbixagent = slapos.recipe.zabbixagent:Recipe
+zeo = slapos.recipe.zeo:Recipe
+zero-knowledge.read = slapos.recipe.zero_knowledge:ReadRecipe
+zero-knowledge.write = slapos.recipe.zero_knowledge:WriteRecipe
+zimbra.kvm = slapos.recipe.zimbra_kvm:Recipe
```

### Comparing `slapos.cookbook-1.0.9/setup.py` & `slapos.cookbook-1.0.92/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,59 +24,58 @@
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 from setuptools import setup, find_packages
 import glob
 import os
 
-version = '1.0.9'
+version = '1.0.92'
 name = 'slapos.cookbook'
-long_description = open("README.txt").read() + "\n" + \
-    open("CHANGES.txt").read() + "\n"
+long_description = open("README.rst").read() + "\n" + \
+    open("CHANGES.rst").read() + "\n"
 
-for f in sorted(glob.glob(os.path.join('slapos', 'recipe', 'README.*.txt'))):
+for f in sorted(glob.glob(os.path.join('slapos', 'recipe', 'README.*.rst'))):
   long_description += '\n' + open(f).read() + '\n'
 
 # extras_requires are not used because of
 #   https://bugs.launchpad.net/zc.buildout/+bug/85604
 setup(name=name,
       version=version,
       description="SlapOS recipes.",
       long_description=long_description,
       classifiers=[
           "Framework :: Buildout :: Recipe",
           "Programming Language :: Python",
         ],
+      maintainer="Nexedi",
+      maintainer_email="info@nexedi.com",
+      url="https://lab.nexedi.com/nexedi/slapos",
       keywords='slapos recipe',
       license='GPLv3',
       namespace_packages=['slapos', 'slapos.recipe'],
       packages=find_packages(),
       include_package_data=True,
       install_requires=[
+        'enum34',  # for inotify-simple
         'jsonschema',
         'hexagonit.recipe.download',
-        'lxml', # for full blown python interpreter
         'netaddr', # to manipulate on IP addresses
         'setuptools', # namespaces
-        'inotifyx', # to watch filesystem changes (used in lockfile)
+        'inotify_simple',
         'lock_file', #another lockfile implementation for multiprocess
         'slapos.core', # uses internally
-#        'slapos.toolbox', # needed for libcloud, cloudmgr, disabled for now
-        'xml_marshaller', # need to communication with slapgrid
         'zc.buildout', # plays with buildout
         'zc.recipe.egg', # for scripts generation
         'pytz', # for timezone database
         ],
       zip_safe=True,
       entry_points={
         'zc.buildout': [
           'addresiliency = slapos.recipe.addresiliency:Recipe',
           'accords = slapos.recipe.accords:Recipe',
-          'agent = slapos.recipe.agent:Recipe',
-          'apache.zope.backend = slapos.recipe.apache_zope_backend:Recipe',
           'apacheperl = slapos.recipe.apacheperl:Recipe',
           'apachephp = slapos.recipe.apachephp:Recipe',
           'apachephpconfigure = slapos.recipe.apachephpconfigure:Recipe',
           'apacheproxy = slapos.recipe.apacheproxy:Recipe',
           'boinc = slapos.recipe.boinc:Recipe',
           'boinc.app = slapos.recipe.boinc:App',
           'boinc.client = slapos.recipe.boinc:Client',
@@ -88,68 +87,52 @@
           'check_port_listening = slapos.recipe.check_port_listening:Recipe',
           'check_url_available = slapos.recipe.check_url_available:Recipe',
           'check_parameter = slapos.recipe.check_parameter:Recipe',
           'cloud9 = slapos.recipe.cloud9:Recipe',
           'cloudooo.test = slapos.recipe.erp5_test:CloudoooRecipe',
           'condor = slapos.recipe.condor:Recipe',
           'condor.submit = slapos.recipe.condor:AppSubmit',
-          'configurationfile = slapos.recipe.configurationfile:Recipe',
           'copyfilelist = slapos.recipe.copyfilelist:Recipe',
           'cron = slapos.recipe.dcron:Recipe',
           'cron.d = slapos.recipe.dcron:Part',
           'davstorage = slapos.recipe.davstorage:Recipe',
-          'downloader = slapos.recipe.downloader:Recipe',
           'dropbear = slapos.recipe.dropbear:Recipe',
           'dropbear.add_authorized_key = slapos.recipe.dropbear:AddAuthorizedKey',
           'dropbear.client = slapos.recipe.dropbear:Client',
-          'dumpmdb = slapos.recipe.dumpmdb:Recipe',
           'duplicity = slapos.recipe.duplicity:Recipe',
-          'egg_test = slapos.recipe.erp5_test:EggTestRecipe',
           'equeue = slapos.recipe.equeue:Recipe',
-          'erp5.bootstrap = slapos.recipe.erp5_bootstrap:Recipe',
           'erp5.promise = slapos.recipe.erp5_promise:Recipe',
-          'erp5.test = slapos.recipe.erp5_test:Recipe',
-          'erp5.update = slapos.recipe.erp5_update:Recipe',
           'erp5scalabilitytestbed = slapos.recipe.erp5scalabilitytestbed:Recipe',
           'erp5testnode = slapos.recipe.erp5testnode:Recipe',
-          'firefox = slapos.recipe.firefox:Recipe',
           'fontconfig = slapos.recipe.fontconfig:Recipe',
-          'generate.mac = slapos.recipe.generatemac:Recipe',
-          'generate.password = slapos.recipe.generatepassword:Recipe',
+          'free_port = slapos.recipe.free_port:Recipe',
+          'generate.mac = slapos.recipe.random:Mac',
+          'generate.password = slapos.recipe.random:Password',
           'generic.cloudooo = slapos.recipe.generic_cloudooo:Recipe',
           'generic.kumofs = slapos.recipe.generic_kumofs:Recipe',
           'generic.memcached = slapos.recipe.generic_memcached:Recipe',
           'generic.mysql = slapos.recipe.generic_mysql:Recipe',
           'generic.mysql.wrap_update_mysql = slapos.recipe.generic_mysql:WrapUpdateMySQL',
           'generic.mysql.wrap_mysqld = slapos.recipe.generic_mysql:WrapMySQLd',
           'generic.varnish = slapos.recipe.generic_varnish:Recipe',
-          'generic.zope = slapos.recipe.generic_zope:Recipe',
-          'generic.zope.zeo.client = slapos.recipe.generic_zope_zeo_client:Recipe',
           'gitinit = slapos.recipe.gitinit:Recipe',
           'haproxy = slapos.recipe.haproxy:Recipe',
-          'helloworld = slapos.recipe.helloworld:Recipe',
-          'importmdb = slapos.recipe.importmdb:Recipe',
           'ipv4toipv6 = slapos.recipe.6tunnel:FourToSix',
           'ipv6toipv4 = slapos.recipe.6tunnel:SixToFour',
-          'java = slapos.recipe.java:Recipe',
           'jsondump = slapos.recipe.jsondump:Recipe',
-          'kumofs = slapos.recipe.kumofs:Recipe',
-          'kvm = slapos.recipe.kvm:Recipe',
           'kvm.frontend = slapos.recipe.kvm_frontend:Recipe',
           'lamp = slapos.recipe.lamp:Request',
           'lamp.generic = slapos.recipe.lampgeneric:Recipe',
           'lamp.request = slapos.recipe.lamp:Request',
           'lamp.simple = slapos.recipe.lamp:Simple',
           'lamp.static = slapos.recipe.lamp:Static',
           'libcloud = slapos.recipe.libcloud:Recipe',
           'libcloudrequest = slapos.recipe.libcloudrequest:Recipe',
-          'lockfile = slapos.recipe.lockfile:Recipe',
           'logrotate = slapos.recipe.logrotate:Recipe',
           'logrotate.d = slapos.recipe.logrotate:Part',
-          'memcached = slapos.recipe.memcached:Recipe',
           'mkdirectory = slapos.recipe.mkdirectory:Recipe',
           'mioga.instantiate = slapos.recipe.mioga.instantiate:Recipe',
           'mydumper = slapos.recipe.mydumper:Recipe',
           'mysql = slapos.recipe.mysql:Recipe',
           'nbdserver = slapos.recipe.nbdserver:Recipe',
           'neoppod.admin = slapos.recipe.neoppod:Admin',
           'neoppod.master = slapos.recipe.neoppod:Master',
@@ -161,67 +144,68 @@
           'novnc = slapos.recipe.novnc:Recipe',
           'onetimeupload = slapos.recipe.onetimeupload:Recipe',
           'pbs = slapos.recipe.pbs:Recipe',
           'postgres = slapos.recipe.postgres:Recipe',
           'postgres.export = slapos.recipe.postgres.backup:ExportRecipe',
           'postgres.import = slapos.recipe.postgres.backup:ImportRecipe',
           'proactive = slapos.recipe.proactive:Recipe',
+          'promise.plugin= slapos.recipe.promise_plugin:Recipe',
           'publish = slapos.recipe.publish:Recipe',
           'publish.serialised = slapos.recipe.publish:Serialised',
           'publish-early = slapos.recipe.publish_early:Recipe',
           'publishsection = slapos.recipe.publish:PublishSection',
           'publishurl = slapos.recipe.publishurl:Recipe',
+          'random.time = slapos.recipe.random:Time',
+          'random.integer = slapos.recipe.random:Integer',
           'readline = slapos.recipe.readline:Recipe',
           'redis.server = slapos.recipe.redis:Recipe',
           'request = slapos.recipe.request:Recipe',
-          'request.serialised = slapos.recipe.request:Serialised',
+          'request.serialised = slapos.recipe.request:RequestJSONEncoded',
           'request.edge = slapos.recipe.request:RequestEdge',
           'requestoptional = slapos.recipe.request:RequestOptional',
+          'requestoptional.serialised = '
+          'slapos.recipe.request:RequestOptionalJSONEncoded',
           're6stnet.registry = slapos.recipe.re6stnet:Recipe',
           'reverseproxy.nginx = slapos.recipe.reverse_proxy_nginx:Recipe',
-          'seleniumrunner = slapos.recipe.seleniumrunner:Recipe',
           'sheepdogtestbed = slapos.recipe.sheepdogtestbed:SheepDogTestBed',
           'shell = slapos.recipe.shell:Recipe',
-          'shellinabox = slapos.recipe.shellinabox:Recipe',
           'signalwrapper= slapos.recipe.signal_wrapper:Recipe',
           'simplelogger = slapos.recipe.simplelogger:Recipe',
           'simplehttpserver = slapos.recipe.simplehttpserver:Recipe',
           'siptester = slapos.recipe.siptester:SipTesterRecipe',
           'slapconfiguration = slapos.recipe.slapconfiguration:Recipe',
           'slapconfiguration.serialised = slapos.recipe.slapconfiguration:Serialised',
           'slapconfiguration.jsondump = slapos.recipe.slapconfiguration:JsonDump',
           'slapcontainer = slapos.recipe.container:Recipe',
-          'slapmonitor = slapos.recipe.slapmonitor:MonitorRecipe',
-          'slapmonitor-xml = slapos.recipe.slapmonitor:MonitorXMLRecipe',
-          'slapreport = slapos.recipe.slapreport:Recipe',
           'softwaretype = slapos.recipe.softwaretype:Recipe', # BBB
           'sphinx= slapos.recipe.sphinx:Recipe',
           'squid = slapos.recipe.squid:Recipe',
           'sshkeys_authority = slapos.recipe.sshkeys_authority:Recipe',
           'sshkeys_authority.request = slapos.recipe.sshkeys_authority:Request',
           'stunnel = slapos.recipe.stunnel:Recipe',
           'switch-softwaretype = slapos.recipe.switch_softwaretype:Recipe',
           'symbolic.link = slapos.recipe.symbolic_link:Recipe',
           'tidstorage = slapos.recipe.tidstorage:Recipe',
           'trac = slapos.recipe.trac:Recipe',
           'urlparse = slapos.recipe._urlparse:Recipe',
           'uuid = slapos.recipe._uuid:Recipe',
           'userinfo = slapos.recipe.userinfo:Recipe',
-          'vifib = slapos.recipe.vifib:Recipe',
-          'waitfor = slapos.recipe.waitfor:Recipe',
           'webchecker = slapos.recipe.web_checker:Recipe',
           'wrapper = slapos.recipe.wrapper:Recipe',
-          'xvfb = slapos.recipe.xvfb:Recipe',
           'xwiki = slapos.recipe.xwiki:Recipe',
           'zabbixagent = slapos.recipe.zabbixagent:Recipe',
           'zimbra.kvm = slapos.recipe.zimbra_kvm:Recipe',
           'zeo = slapos.recipe.zeo:Recipe',
           'zero-knowledge.read = slapos.recipe.zero_knowledge:ReadRecipe',
           'zero-knowledge.write = slapos.recipe.zero_knowledge:WriteRecipe'
         ],
         'slapos.recipe.nosqltestbed.plugin': [
           'kumo = slapos.recipe.nosqltestbed.kumo:KumoTestBed',
         ],
       },
       test_suite='slapos.test',
-      tests_require=[ 'jsonschema' ],
-    )
+      tests_require=[
+        'jsonschema',
+        'mock',
+        'testfixtures',
+      ],
+    )
```

### Comparing `slapos.cookbook-1.0.9/slapos/test/test_json_schema.py` & `slapos.cookbook-1.0.92/slapos/recipe/mkdirectory.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,57 +20,26 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-
-import unittest
 import os
-import glob
-import json
-import slapos.test
-import jsonschema
-
-
-def getSchemaValidator(filename):
-  schema_json_file = "/".join(slapos.test.__file__.split("/")[:-1])
-  schema_json_file += "/%s" % filename
-  with open(schema_json_file, "r") as json_file:
-    json_dict = json.loads(json_file.read())
-    json_file.close()
-  return json_dict
-
-def createTest(path, json_dict):
-  def run(self, *args, **kwargs):
-    with open(path, "r") as json_file:
-      self.assertEquals(jsonschema.validate(json.loads(json_file.read()), json_dict), None)
-      json_file.close()
-
-  return run
-
-def generateSoftwareCfgTest():
-  json_dict = getSchemaValidator("schema.json")
-  base_path = "/".join(slapos.test.__file__.split("/")[:-3])
-  for path in glob.glob("%s/software/*/software.cfg.json" % base_path):
-    test_name = "test_%s_software_cfg_json" % path.split("/")[-2]
-    setattr(TestJSONSchemaValidation, test_name , createTest(path, json_dict)) 
-
-
-def generateJSONSchemaTest():
-  json_dict = getSchemaValidator("metaschema.json")
-  base_path = "/".join(slapos.test.__file__.split("/")[:-3])
-  for path in glob.glob("%s/software/*/*schema.json" % base_path):
-    software_type = path.split("/")[-2]
-    filename = path.split("/")[-1].replace("-", "_").replace(".", "_")
-    test_name = "test_schema_%s_%s" % (software_type, filename)
-    setattr(TestJSONSchemaValidation, test_name , createTest(path, json_dict)) 
 
-class TestJSONSchemaValidation(unittest.TestCase):
-  pass
+from slapos.recipe.librecipe import GenericBaseRecipe
 
-generateSoftwareCfgTest()
-generateJSONSchemaTest()
+class Recipe(GenericBaseRecipe):
 
-if __name__ == '__main__':
-  unittest.main()
+  def _options(self, options):
+    self.directory = options.copy()
+    del self.directory['recipe']
+    self.mode = int(self.directory.pop('mode', '0777'), 8)
+
+  def install(self):
+    for path in sorted(self.directory.itervalues()):
+      if path and not os.path.isdir(path):
+        os.makedirs(path, self.mode)
+    # WARNING: This recipe is currently used to create directories that will
+    #          contain user data  (e.g. NEO db). Such directories must never
+    #          be purged by the uninstallation of a recipe.
+    return []
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/proactive/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/proactive/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/configurationfile/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/nbdserver/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -21,20 +21,32 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
+import binascii
+import os
+import sys
 
 class Recipe(GenericBaseRecipe):
+  """
+  nbd instance configuration.
+  """
+
   def install(self):
-    configuration_file = self.createFile(
-        self.options['configuration-file-path'],
-        self.substituteTemplate(
-            self.options['configuration-template-path'],
-            self.options
-        )
+    config = dict(
+      ip=self.options['ip'],
+      port=self.options['port'],
+      image_path=self.options['image-path'],
+      qemu_path=self.options['qemu-path'],
+      shell_path=self.options['shell-path'],
     )
 
-    return configuration_file
+    # Runners
+    runner_path = self.createExecutable(
+      self.options['path'],
+      self.substituteTemplate(self.getTemplateFilename('nbdserver_run.in'),
+                              config))
 
+    return [runner_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apacheperl/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/apacheperl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,18 +53,17 @@
     )
     httpd_conf = self.createFile(self.options['httpd-conf'],
       self.substituteTemplate(self.getTemplateFilename('apache.in'),
                               apache_config)
     )
     path_list.append(httpd_conf)
 
-    wrapper = self.createPythonScript(self.options['wrapper'],
-        'slapos.recipe.librecipe.execute.execute',
-        [self.options['httpd-binary'], '-f', self.options['httpd-conf'],
-         '-DFOREGROUND']
+    wrapper = self.createWrapper(self.options['wrapper'],
+        (self.options['httpd-binary'], '-f', self.options['httpd-conf'],
+          '-DFOREGROUND'),
     )
     path_list.append(wrapper)
 
     if os.path.exists(self.options['pid-file']):
       # Reload apache configuration
       with open(self.options['pid-file']) as pid_file:
         pid = int(pid_file.read().strip(), 10)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apacheperl/template/apache.in` & `slapos.cookbook-1.0.92/slapos/recipe/apacheperl/template/apache.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/neoppod.py` & `slapos.cookbook-1.0.92/slapos/recipe/neoppod.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
+import os
 from slapos.recipe.librecipe import GenericBaseRecipe
 from zc.buildout import UserError
 
 class NeoBaseRecipe(GenericBaseRecipe):
 
   _binding_port_mandatory = True
 
@@ -37,29 +38,33 @@
       # All parameters are always provided.
       # This parameter needs special care, because it is initially generated
       # empty, until all requested master nodes get their partitions
       # allocated.
       # Only then can this recipe start succeeding and actually doing anything
       # useful, as per NEO deploying constraints.
       raise UserError('"masters" parameter is mandatory')
-    option_list = [
+    args = [
       options['binary'],
+      # Keep the -l option first, as expected by logrotate snippets.
       '-l', options['logfile'],
       '-m', options['masters'],
       '-b', self._getBindingAddress(),
       # TODO: reuse partition reference for better log readability.
       #'-n', options['name'],
       '-c', options['cluster'],
     ]
-    option_list.extend(self._getOptionList())
-    return [self.createPythonScript(
-      options['wrapper'],
-      'slapos.recipe.librecipe.execute.execute',
-      option_list
-    )]
+    if options['ssl']:
+      etc = os.path.join(self.buildout['buildout']['directory'], 'etc', '')
+      args += (
+        '--ca', etc + 'ca.crt',
+        '--cert', etc + 'neo.crt',
+        '--key', etc + 'neo.key',
+        )
+    args += self._getOptionList()
+    return self.createWrapper(options['wrapper'], args)
 
   def _getBindingAddress(self):
     options = self.options
     bind = options['ip']
     if 'port' in options:
       # Some node types support port auto-allocation when no binding port is
       # requested.
@@ -80,14 +85,18 @@
       '-d', self.options['database-parameters'],
       '-a', self.options['database-adapter'],
       '-w', self.options['wait-database'],
     ]
     engine = self.options.get('engine')
     if engine: # old versions of NEO don't support -e
       r  += '-e', engine
+    if self.options.get('dedup'):
+      r.append('--dedup')
+    if self.options.get('disable-drop-partitions'):
+      r.append('--disable-drop-partitions')
     return r
 
 class Admin(NeoBaseRecipe):
   def _getOptionList(self):
     return []
 
 class Master(NeoBaseRecipe):
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/nbdserver/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/check_page_content/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,32 +21,31 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
-import binascii
-import os
 import sys
 
 class Recipe(GenericBaseRecipe):
   """
-  nbd instance configuration.
+  Create script that will check if content at "url" is available
+  (e.g page has a link to itself).
   """
 
   def install(self):
-    config = dict(
-      ip=self.options['ip'],
-      port=self.options['port'],
-      image_path=self.options['image-path'],
-      qemu_path=self.options['qemu-path'],
-      shell_path=self.options['shell-path'],
-    )
+    url = self.options['url'].strip()
+    config = {
+      'url': url,
+      'shell_path': self.options['dash_path'],
+      'curl_path': self.options['curl_path'],
+      'match': self.options.get('match', url)
+    }
 
-    # Runners
-    runner_path = self.createExecutable(
+    # XXX-Cedric in this script, curl won't check certificate
+    promise = self.createExecutable(
       self.options['path'],
-      self.substituteTemplate(self.getTemplateFilename('nbdserver_run.in'),
-                              config))
+      self.substituteTemplate(self.getTemplateFilename('check_page_content.in'), config)
+    )
 
-    return [runner_path]
+    return [promise]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/davstorage/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/davstorage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,34 +94,27 @@
 
     config_file = self.createFile(self.options['conf-file'],
        self.substituteTemplate(self.getTemplateFilename('httpd.conf.in'),
                                apache_config)
     )
     path_list.append(config_file)
 
-    wrapper = self.createPythonScript(self.options['wrapper'],
-      'slapos.recipe.librecipe.execute.execute',
-      [self.options['apache-binary'], '-f', config_file, '-DFOREGROUND'])
+    wrapper = self.createWrapper(self.options['wrapper'],
+      (self.options['apache-binary'], '-f', config_file, '-DFOREGROUND'))
     path_list.append(wrapper)
 
     promise = self.createPythonScript(self.options['promise'],
       __name__ + '.promise',
-      dict(host=self.options['ip'], port=int(self.options['port_webdav']),
-           user=self.options['user'], password=self.options['password'])
-                                     )
+      (self.options['ip'], int(self.options['port_webdav']),
+       self.options['user'], self.options['password']))
     path_list.append(promise)
 
     return path_list
 
-def promise(args):
-  host = args['host']
-  port = args['port']
-  user = args['user']
-  password = args['password']
-
+def promise(host, port, user, password):
   connection = httplib.HTTPSConnection(host, port)
   auth = base64.b64encode('%s:%s' % (user, password))
   connection.request('OPTIONS', '/',
                      headers=dict(
                        Authorization='Basic %s' % auth,
                      )
                     )
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/davstorage/template/httpd.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/davstorage/template/httpd.conf.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/container.py` & `slapos.cookbook-1.0.92/slapos/recipe/container.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/xvfb/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/generic_memcached/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2012 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -19,38 +19,39 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
-#############################################################################
-
+##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
-  def install(self):
+  """
+  memcached instance configuration.
 
-    config = {
-      'xvfb_binary': self.options['xvfb-path'],
-      'shell_path': self.options['shell-path'],
-      'fbdir_path': self.options['fbdir-path'],
-      'tmp_path': self.options['tmp-path'],
-      }
-
-    xvfb_path = self.createExecutable(
-      self.options['runner-path'],
-      self.substituteTemplate(self.getTemplateFilename('xvfb_run.in'),
-                              config))
-    result = [xvfb_path]
+  wrapper-path -- location of the init script to generate
 
-    # Allow to take screenshot if needed
-    if ('xwd-path' in self.options) and ('xwd-hook-path' in self.options):
+  binary-path -- location of the memcached command
 
-      config['xwd_binary'] = self.options['xwd-path']
-      result.append(self.createExecutable(
-        self.options['xwd-hook-path'],
-        self.substituteTemplate(self.getTemplateFilename('xwd_run.in'),
-                                config)))
+  ip -- ip of the memcached server
 
-    return result
+  port -- port of the memcached server
+  """
+
+  def install(self):
+    template_filename = self.getTemplateFilename('memcached.in')
+
+    config = dict(
+        memcached_binary=self.options['binary_path'],
+        memcached_ip=self.options['ip'],
+        memcached_port=self.options['port'],
+        shell_path=self.options['shell-path'],
+    )
+
+    executable_path = self.createExecutable(
+      self.options['wrapper_path'],
+      self.substituteTemplate(self.getTemplateFilename('memcached.in'),
+                              config))
 
+    return [executable_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/notifier.py` & `slapos.cookbook-1.0.92/slapos/recipe/notifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,27 +28,23 @@
 from hashlib import sha512
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
 
   def install(self):
     options = self.options
-    script = self.createWrapper(name=options['wrapper'],
-                                command=options['server-binary'],
-                                parameters=[
+    # Script that execute the callback(s) upon receiving a notification.
+    return self.createWrapper(options['wrapper'],
+                                (options['server-binary'],
                                    '--callbacks', options['callbacks'],
                                    '--feeds', options['feeds'],
                                    '--equeue-socket', options['equeue-socket'],
                                    options['host'], options['port']
-                                   ],
-                                comments=[
-                                    '',
-                                    'Upon receiving a notification, execute the callback(s).',
-                                    ''])
-    return [script]
+                                   ),
+                                )
 
 
 class Callback(GenericBaseRecipe):
 
   def createCallback(self, notification_id, callback):
     # XXX: hashing the name here and in
     # slapos.toolbox/slapos/pubsub/__init__.py is completely messed up and
@@ -62,51 +58,65 @@
   def install(self):
     # XXX this path is returned multiple times, one for each callback that has been added.
     return [self.createCallback(self.options['on-notification-id'],
                                 self.options['callback'])]
 
 class Notify(GenericBaseRecipe):
 
+  def __init__(self, buildout, name, options):
+    super(Notify, self).__init__(buildout, name, options)
+    log = os.path.join(options['feeds'], options['name'])
+    options['log-file'] = log
+    self.options = options
+
   def createNotifier(self, notifier_binary, wrapper, executable,
-                     log, title, notification_url, feed_url, pidfile=None):
+                     log, title, notification_url, feed_url, max_run='1', pidfile=None,
+                     instance_root_name=None, log_url=None, status_item_directory=None):
 
     if not os.path.exists(log):
       # Just a touch
       open(log, 'w').close()
 
-    parameters = [
+    cmd = [notifier_binary,
             '-l', log,
             '--title', title,
             '--feed', feed_url,
+            '--max-run', str(max_run),
             '--notification-url',
             ]
-    parameters.extend(notification_url.split(' '))
-    parameters.extend(['--executable', executable])
+    cmd += notification_url.split(' ')
+    cmd += '--executable', executable
+    # For a more verbose mode, writing feed items for any action
+    instance_root_name = instance_root_name or self.options.get('instance-root-name', None)
+    log_url = log_url or self.options.get('log-url', None)
+    status_item_directory = status_item_directory or self.options.get('status-item-directory', None)
+    if instance_root_name and log_url and status_item_directory:
+      cmd += (
+        '--instance-root-name', instance_root_name,
+        '--log-url', log_url,
+        '--status-item-directory', status_item_directory,
+      )
+
+    kw = {}
+    if pidfile:
+      kw['pidfile'] = pidfile
 
-    return self.createWrapper(name=wrapper,
-                              command=notifier_binary,
-                              parameters=parameters,
-                              pidfile=pidfile,
-                              parameters_extra=True,
-                              comments=[
-                                  '',
-                                  'Call an executable and send notification(s).',
-                                  ''])
+    # Script that call an executable and send notification(s).
+    return self.createWrapper(wrapper, cmd, **kw)
 
 
   def install(self):
     feed_url = self.unparseUrl(scheme='http', host=self.options['host'],
                                port=self.options['port'],
                                path='/get/%s' % self.options['name'])
 
-    log = os.path.join(self.options['feeds'], self.options['name'])
-
     options = self.options
     script = self.createNotifier(notifier_binary=options['notifier-binary'],
                                  wrapper=options['wrapper'],
                                  executable=options['executable'],
-                                 log=log,
+                                 log=options['log-file'],
                                  title=options['title'],
                                  pidfile=options['pidfile'],
                                  notification_url=options['notify'],
-                                 feed_url=feed_url)
+                                 feed_url=feed_url,
+                                 max_run=options.get('max-run', "1"))
     return [script]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/dcron.py` & `slapos.cookbook-1.0.92/slapos/recipe/dcron.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,22 @@
 
 class Recipe(GenericBaseRecipe):
 
   def install(self):
     self.logger.info("Installing dcron...")
 
     options = self.options
-    script = self.createWrapper(name=options['binary'],
-                                command=options['dcrond-binary'].strip(),
-                                parameters=[
+    script = self.createWrapper(options['binary'],
+                                (options['dcrond-binary'].strip(),
                                     '-s', options['cron-entries'],
                                     '-c', options['crontabs'],
                                     '-t', options['cronstamps'],
                                     '-f', '-l', '5',
                                     '-M', options['catcher']
-                                    ])
+                                    ))
 
     self.logger.debug('Main cron executable created at : %r', script)
 
     self.logger.info("dcron successfully installed.")
 
     return [script]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/fontconfig/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/fontconfig/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,16 +34,14 @@
   fontconfig instance configuration.
 
   conf-path -- location of the configuration file
 
   font-system-folder -- fonts installed by software release
 
   font-folder -- location where to download fonts
-
-  url-list -- From where to download fonts
   """
 
   def install(self):
     created_file_list = []
     font_folder = self.options['font-folder']
     service_folder = self.options['service-folder']
     snippet_filename = self.getTemplateFilename(
@@ -58,28 +56,8 @@
         )
     template_filename = self.getTemplateFilename('fontconfig.cfg.in')
     configuration_path = self.createFile(
         self.options['conf-path'],
         self.substituteTemplate(template_filename, config))
 
     created_file_list.append(configuration_path)
-    # Instanciate onetimedownloads, one for each url
-    wrapper_template_location = pkg_resources.resource_filename(
-                                        __name__, os.path.join(
-                                        'template', 'onetimedownload_run.in'))
-
-    onetimedownload_config = {}
-    onetimedownload_config.update(self.options)
-    for index, url in enumerate(self.options['url-list'].split()):
-      if not url.strip():
-        continue
-      bin_path = os.path.join(service_folder, 'onetimedownload%s' % index)
-      file_path = os.path.join(font_folder, '%s' % index)
-      onetimedownload_config['url'] = url
-      onetimedownload_config['file_path'] = file_path
-      onetimedownload_runner_path = self.createExecutable(bin_path,
-          self.substituteTemplate(wrapper_template_location,
-                                  onetimedownload_config))
-
-      created_file_list.append(onetimedownload_runner_path)
-
     return created_file_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5_test/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/mysql/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,130 +20,172 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
+import os
+import sys
+import subprocess
+
 from slapos.recipe.librecipe import GenericBaseRecipe
-import urlparse
+from slapos.recipe.librecipe import filehash
 
-# The follow recipes should be unified somehow in order to improve
-# code mantainence.
 
 class Recipe(GenericBaseRecipe):
+
   def install(self):
-    testinstance = self.options['test-instance-path']
-    mysql_connection_string_list = []
     path_list = []
-    # XXX: assume existence of 100 test databases, because slaves are not
-    # functional yet in slapos: testdb_0...testdb_100, with testuser_N
-    mysql_template = "%s@%s:%s %s %s"
-    mysql_url_list = self.options.get('mysql-url-list')
-    if mysql_url_list is None:
-      mysql_parsed = urlparse.urlparse(self.options['mysql-url'])
-      for i in range(0, 100):
-        mysql_connection_string_list.append(mysql_template % ('testdb_%s'% i,
-          mysql_parsed.hostname, mysql_parsed.port, 'testuser_%s'% i, mysql_parsed.password))
-      mysql_connection_string = mysql_template % ('erp5_test', mysql_parsed.hostname,
-        mysql_parsed.port, 'erp5_test', mysql_parsed.password)
-    else:
-      for mysql_url in mysql_url_list:
-        mysql_parsed = urlparse.urlparse(mysql_url)
-        mysql_connection_string_list.append(mysql_template % (
-          mysql_parsed.path.lstrip('/'),
-          mysql_parsed.hostname,
-          mysql_parsed.port,
-          mysql_parsed.username,
-          mysql_parsed.password,
-        ))
-      mysql_connection_string = mysql_connection_string_list.pop()
-    cloudooo_parsed = urlparse.urlparse(self.options['cloudooo-url'])
-    memcached_parsed = urlparse.urlparse(self.options['memcached-url'])
-    kumofs_parsed = urlparse.urlparse(self.options['kumofs-url'])
-    common_dict = dict(
-        instance_home=testinstance,
-        prepend_path=self.options['prepend-path'],
-        openssl_binary=self.options['openssl-binary'],
-        test_ca_path=self.options['certificate-authority-path'],
-    )
-    common_list = [
-      '--conversion_server_hostname=%s' % cloudooo_parsed.hostname,
-      '--conversion_server_port=%s' % cloudooo_parsed.port,
-      '--volatile_memcached_server_hostname=%s' % memcached_parsed.hostname,
-      '--volatile_memcached_server_port=%s' % memcached_parsed.port,
-      '--persistent_memcached_server_hostname=%s' % kumofs_parsed.hostname,
-      '--persistent_memcached_server_port=%s' % kumofs_parsed.port,
-    ]
-    path_list.append(self.createPythonScript(self.options['run-unit-test'],
-        __name__ + '.test.runUnitTest', [dict(
-        call_list=[self.options['run-unit-test-binary'],
-          '--erp5_sql_connection_string', mysql_connection_string,
-          '--extra_sql_connection_string_list', ','.join(
-            mysql_connection_string_list),
-          ] + common_list, **common_dict)]))
-    path_list.append(self.createPythonScript(self.options['run-test-suite'],
-        __name__ + '.test.runUnitTest', [dict(
-        call_list=[self.options['run-test-suite-binary'],
-          '--db_list', ','.join(mysql_connection_string_list),
-          ] + common_list, **common_dict)]))
 
-    return path_list
+    template_filename = self.getTemplateFilename('my.cnf.in')
 
-class CloudoooRecipe(GenericBaseRecipe):
-  def install(self):
-    path_list = []
-    common_dict = dict(
-        prepend_path=self.options['prepend-path'],
+    mysql_conf = dict(
+        ip=self.options['ip'],
+        data_directory=self.options['data-directory'],
+        tcp_port=self.options['port'],
+        pid_file=self.options['pid-file'],
+        socket=self.options['socket'],
+        error_log=self.options['error-log'],
+        mysql_database=self.options['database'],
+        mysql_user=self.options['user'],
+        mysql_password=self.options['password'],
     )
-    common_list = [
-           "--paster_path", self.options['ooo-paster'],
-           self.options['configuration-file']
-          ]
-    run_unit_test_path = self.createPythonScript(self.options['run-unit-test'],
-        __name__ + '.test.runUnitTest', [dict(
-        call_list=[self.options['run-unit-test-binary'],
-          ] + common_list, **common_dict)])
-
-    path_list.append(run_unit_test_path)
-    path_list.append(self.createPythonScript(self.options['run-test-suite'],
-        __name__ + '.test.runTestSuite', [dict(
-        call_list=[self.options['run-test-suite-binary'],
-          ], **common_dict)]))
-
-    return path_list
 
-class EggTestRecipe(GenericBaseRecipe):
-  """
-  Recipe used to create wrapper used to run test suite (python setup.py test)
-  off a list of Python eggs.
-  """
-  def install(self):
-    path_list = []
-    test_list = self.options['test-list'].strip().replace('\n', ',')
-    common_dict = {}
+    mysql_binary = self.options['mysql-binary']
+    socket = self.options['socket'],
+    post_rotate = self.createWrapper(
+      self.options['logrotate-post'],
+      (mysql_binary, '--no-defaults', '-B', '-u', 'root',
+        '--socket=%s' % socket, '-e', 'FLUSH LOGS'),
+    )
+    path_list.append(post_rotate)
 
-    environment_dict = {}
-    if self.options.get('environment'):
-      environment_part = self.buildout.get(self.options['environment'])
-      if environment_part:
-        for key, value in environment_part.iteritems():
-          environment_dict[key] = value
+    mysql_conf_file = self.createFile(
+      self.options['conf-file'],
+      self.substituteTemplate(template_filename, mysql_conf)
+    )
+    path_list.append(mysql_conf_file)
 
-    common_list = [ "--source_code_path_list", test_list]
+    mysql_script_list = []
 
-    argument_dict = dict(
-        call_list=[self.options['run-test-suite-binary'],] + common_list,
-        environment=environment_dict,
-        **common_dict
+    init_script = self.substituteTemplate(
+      self.getTemplateFilename('initmysql.sql.in'),
+      {
+        'mysql_database': mysql_conf['mysql_database'],
+        'mysql_user': mysql_conf['mysql_user'],
+        'mysql_password': mysql_conf['mysql_password']
+      }
     )
-    if 'prepend-path' in self.options:
-      argument_dict['prepend_path'] = self.options['prepend-path']
+    mysql_script_list.append(init_script)
+    mysql_script_list.append('EXIT')
+    mysql_script = '\n'.join(mysql_script_list)
+
+    mysql_upgrade_binary = self.options['mysql-upgrade-binary']
+    mysql_update = self.createPythonScript(
+      self.options['update-wrapper'],
+      '%s.mysql.updateMysql' % __name__,
+      (dict(
+        mysql_script=mysql_script,
+        mysql_binary=mysql_binary,
+        mysql_upgrade_binary=mysql_upgrade_binary,
+        socket=socket,
+       ),)
+    )
+    path_list.append(mysql_update)
 
-    run_test_suite_script = self.createPythonScript(
-        self.options['run-test-suite'], __name__ + '.test.runTestSuite',
-        [argument_dict]
+    mysqld_binary = self.options['mysqld-binary']
+    mysqld = self.createPythonScript(
+      self.options['wrapper'],
+      '%s.mysql.runMysql' % __name__,
+      (dict(
+        mysql_install_binary=self.options['mysql-install-binary'],
+        mysqld_binary=mysqld_binary,
+        data_directory=mysql_conf['data_directory'],
+        mysql_binary=mysql_binary,
+        socket=socket,
+        configuration_file=mysql_conf_file,
+        cwd=self.options['mysql-base-directory'],
+       ),)
     )
+    path_list.append(mysqld)
+
+    # backup configuration
+    if self.optionIsTrue('backup', default=False):
+      backup_script = self.createPythonScript(
+        self.options['backup-script'],
+        '%s.do_backup' % __name__,
+        (dict(
+          mydumper_binary=self.options['mydumper-binary'],
+          database=mysql_conf['mysql_database'],
+          socket=mysql_conf['socket'],
+          backup_directory=self.options['backup-directory']
+         ),)
+      )
+      path_list.append(backup_script)
+
+    # Recovering backup
+    if self.optionIsTrue('recovering', default=False):
+      recovering_script = self.createPythonScript(
+        self.options['recovering-wrapper'],
+        '%s.import_dump' % __name__,
+        ({
+          'lock_file': os.path.join(self.work_directory,
+                                    'import_done'),
+          'database': mysql_conf['mysql_database'],
+          'mysql_binary': self.options['mysql-binary'],
+          'mysql_socket': mysql_conf['socket'],
+          'duplicity_binary': self.options['duplicity-binary'],
+          'remote_backup': self.parameter_dict['remote-backup'],
+          'local_directory': self.mysql_backup_directory,
+          'dump_name': dump_filename,
+          'zcat_binary': self.options['zcat-binary'],
+        },)
+      )
+      path_list.append(recovering_script)
 
-    path_list.append(run_test_suite_script)
 
     return path_list
+
+# Replace zcat dump.sql.gz | mysql
+def import_dump(args):
+  # Get data from kwargs
+  cache_file = args['cache_file']
+  database = args['database']
+  mysql_binary = args['mysql_binary']
+  mysql_socket = args['mysql_socket']
+  dump_file = args['dump_file']
+  zcat_binary = args['zcat_binary']
+
+  sha512sum = filehash(dump_file)
+  with open(cache_file, 'r') as cache_fileobj:
+    last_sha512sum = cache_fileobj.read().strip()
+
+  if sha512sum != last_sha512sum:
+    zcat = subprocess.Popen([zcat_binary, dump_file], stdout=subprocess.PIPE)
+    mysql = subprocess.Popen([mysql_binary, '--socket=%s' % mysql_socket, '-D',
+                              database, '-u', 'root'], stdin=zcat.stdout)
+    zcat.stdout.close()
+
+    returncode = mysql.wait()
+
+    if returncode == 0:
+      with open(cache_file, 'w') as cache_fileobj:
+        cache_fileobj.write(sha512sum)
+
+    sys.exit(returncode)
+
+def promise(args):
+  # This is not a dependency of slapos.cookbook, because it shall be runned
+  # in a python environment having mysqlclient
+  import MySQLdb
+
+  user = args['user']
+  password = args['password']
+  db = args['db']
+  host = args['host']
+  port = args['port']
+
+  db = MySQLdb.connect(host=host, port=port, user=user, passwd=password,
+                       db=db)
+  cursor = db.cursor()
+  cursor.close()
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/reverse_proxy_nginx/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/reverse_proxy_nginx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,22 +66,20 @@
         self.options['configuration-file'],
         self.substituteTemplate(self.getTemplateFilename('nginx.conf.in'),
         nginx_configuration_dict)
     )
     path_list.append(nginx_configuration_file)
     
     # Generate Nginx wrapper
-    wrapper = self.createWrapper(
-        name=self.options['wrapper'],
-        command=self.options['nginx-executable'],
-        parameters=[
+    path_list.append(self.createWrapper(
+        self.options['wrapper'],
+        (self.options['nginx-executable'],
             '-c', self.options['configuration-file'],
             '-p', self.options['home-directory']
-        ]
-    )
+        )))
 
     # TODO: reload configuration or have feature like apache_map
 
     # Send connection informations about each slave
     for slave_instance in slave_instance_list:
       reference = slave_instance.get("slave_reference")
       self.logger.debug('Sending connection parameters of slave '
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/reverse_proxy_nginx/template/nginx.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/reverse_proxy_nginx/template/nginx.conf.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/condor.py` & `slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/condor.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,35 +58,34 @@
     #Generate BOINC/Condor launcher script
     grid_wrapper = self.options['boinc_condor_wrapper'].strip()
     parameters = dict(startCondor=startCondor, startBoinc=startBoinc,
                       bg_base=self.options['work_dir'].strip(),
                       condor_wrapper_list=condor_wrapper_list,
                       boinc_wrapper_list=boinc_wrapper_list)
     bonjourGrid_wrapper = self.createPythonScript(grid_wrapper,
-        '%s.configure.launchScript' % __name__,
-        parameters
+        __name__ + '.configure.launchScript',
+        (parameters,)
     )
     path_list.append(bonjourGrid_wrapper)
 
     #Generate wrapper for BonjourGrid Master
     bonjourgrid_master = self.options['master_script'].strip()
     python = self.options['python-bin'].strip()
     bg_wrapper = self.options['wrapper'].strip()
     log = self.options['log_file'].strip()
     pid_file = self.options['pid_file'].strip()
-    wrapper = self.createPythonScript(bg_wrapper,
-        'slapos.recipe.librecipe.execute.execute',
-        ([python, bonjourgrid_master, '--log_file', log,
+    wrapper = self.createWrapper(bg_wrapper,
+        (python, bonjourgrid_master, '--log_file', log,
           '--pid_file', pid_file,
           '--master_wrapper', grid_wrapper,
           '--directory', self.options['work_dir'].strip(),
           '--server', self.options['redis-url'].strip(),
           '--port', self.options['redis-port'].strip(),
           '--num_workers', self.options['nworkers'].strip(),
-        ])
+         ),
     )
     path_list.append(wrapper)
 
 
     #generate Computer information file
     config_info_file = os.path.join(self.options['work_dir'].strip(),
                                 'machineinfo.sh')
@@ -109,25 +108,24 @@
 
     #Generate wrapper for BonjourGrid Worker
     bonjourgrid_client = self.options['client_script'].strip()
     python = self.options['python-bin'].strip()
     bg_wrapper = self.options['wrapper'].strip()
     log = self.options['log_file'].strip()
     pid_file = self.options['pid_file'].strip()
-    wrapper = self.createPythonScript(bg_wrapper,
-        'slapos.recipe.librecipe.execute.execute',
-        ([python, bonjourgrid_client, '--log_file', log,
+    wrapper = self.createWrapper(bg_wrapper,
+        (python, bonjourgrid_client, '--log_file', log,
           '--pid_file', pid_file,
           '--boinc_wrapper', boinc_script,
           '--condor_wrapper', condor_script,
           '--directory', self.options['work_dir'].strip(),
           '--install_directory', self.options['install_dir'].strip(),
           '--server', self.options['redis-url'].strip(),
           '--port', self.options['redis-port'].strip(),
-        ])
+         ),
     )
     path_list.append(wrapper)
 
     #generate BOINC and Condor configure script for bonjourgrid
     boinc_wrapper = self.createPythonScript(boinc_script,
         '%s.boinc.runBoinc' % __name__,
         dict(ipv6=self.options['ipv6'].strip(),
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/configure.py` & `slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/configure.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/boinc.py` & `slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/boinc.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/bonjourgrid/template/machineinfo.sh.in` & `slapos.cookbook-1.0.92/slapos/recipe/bonjourgrid/template/machineinfo.sh.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/logrotate.py` & `slapos.cookbook-1.0.92/slapos/recipe/logrotate.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     ]
 
     logrotate_conf_file = self.createFile(logrotate_conf_file,
         '\n'.join(logrotate_conf))
 
     state_file = self.options['state-file']
 
-    logrotate = self.createPythonScript(
+    logrotate = self.createWrapper(
       self.options['wrapper'],
-      'slapos.recipe.librecipe.execute.execute',
-      [self.options['logrotate-binary'], '-s', state_file, logrotate_conf_file, ]
+      (self.options['logrotate-binary'],
+        '-s', state_file, logrotate_conf_file),
     )
 
     return [logrotate, logrotate_conf_file]
 
 class Part(GenericBaseRecipe):
 
   def install(self):
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/simplelogger.py` & `slapos.cookbook-1.0.92/slapos/recipe/simplelogger.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,21 @@
 #
 ##############################################################################
 import sys
 import time
 
 from slapos.recipe.librecipe import GenericBaseRecipe
 
-def log(args):
+def log(filename):
   prefix = time.strftime('%Y-%m-%d.%H:%M.%s:')
-  with open(args['filename'], 'aw') as logfile:
+  with open(filename, 'a') as logfile:
     for line in sys.stdin:
       print >> logfile, prefix, line,
     print >> logfile, prefix, '------------------------'
 
 class Recipe(GenericBaseRecipe):
 
   def install(self):
-    wrapper = self.options['wrapper']
-    log = self.options['log']
-
-    script = self.createPythonScript(wrapper,
-                                     __name__ + '.log',
-                                     arguments=dict(filename=log))
-    return [script]
+    return self.createPythonScript(
+      self.options['wrapper'],
+      __name__ + '.log',
+      (self.options['log'],))
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/librecipe/genericslap.py` & `slapos.cookbook-1.0.92/slapos/recipe/librecipe/genericslap.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 #
 ##############################################################################
 from slapos import slap
 import time
 
 from generic import GenericBaseRecipe
 
+CONNECTION_CACHE = {}
+
 class GenericSlapRecipe(GenericBaseRecipe):
   """Base class for all slap.recipe.* needing SLAP informations like instance
      parameters.
      recipes that don't explicitely need to retrieve from server informations
      should use GenericBaseRecipe."""
 
   def __init__(self, buildout, name, options):
@@ -46,19 +48,26 @@
     self.computer_partition_id = slap_connection['partition-id']
     self.server_url = slap_connection['server-url']
     self.software_release_url = slap_connection['software-release-url']
     self.key_file = slap_connection.get('key-file')
     self.cert_file = slap_connection.get('cert-file')
 
   def install(self):
+
+    cache_key = "%s_%s" % (self.computer_id, self.computer_partition_id)
+    self.computer_partition = CONNECTION_CACHE.get(cache_key, None)
+
     self.slap.initializeConnection(self.server_url, self.key_file,
         self.cert_file)
-    self.computer_partition = self.slap.registerComputerPartition(
-      self.computer_id,
-      self.computer_partition_id)
+    if self.computer_partition is None:
+      self.computer_partition = self.slap.registerComputerPartition(
+        self.computer_id,
+        self.computer_partition_id)
+      CONNECTION_CACHE[cache_key] = self.computer_partition
+
     self.request = self.computer_partition.request
     self.setConnectionDict = self.computer_partition.setConnectionDict
     self.parameter_dict = self.computer_partition.getInstanceParameterDict()
 
     # call children part of install
     path_list = self._install()
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/librecipe/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/librecipe/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/librecipe/inotify.py` & `slapos.cookbook-1.0.92/slapos/recipe/librecipe/inotify.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,31 +21,24 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 import os
-
-import inotifyx
+from inotify_simple import INotify, flags
 
 def subfiles(directory):
   """Return the list of subfiles of a directory, and wait for the newly created
   ones.
 
   CAUTION : *DONT TRY TO CONVERT THE RESULT OF THIS FUNCTION INTO A LIST !
   ALWAYS ITERATE OVER IT !!!*"""
-  watchfd = inotifyx.init()
-  inotifyx.add_watch(watchfd, directory, inotifyx.IN_CREATE)
-  try:
 
-    subfiles = set(os.listdir(directory))
-    subfiles |= set([file_.name for file_ in inotifyx.get_events(watchfd, 0)])
+  with INotify() as inotify:
+    inotify.add_watch(directory, flags.CLOSE_WRITE | flags.MOVED_TO)
 
+    names = os.listdir(directory)
     while True:
-      for file_ in subfiles:
-        yield os.path.join(directory, file_)
-
-      subfiles = [file_.name for file_ in inotifyx.get_events(watchfd)]
-
-  finally:
-    os.close(watchfd)
+      for name in names:
+        yield os.path.join(directory, name)
+      names = (event.name for event in inotify.read())
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/librecipe/generic.py` & `slapos.cookbook-1.0.92/slapos/recipe/librecipe/generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 import io
 import logging
 import os
 import sys
 import inspect
 import re
 import shutil
-from textwrap import dedent
 import urllib
 import urlparse
 
 import pkg_resources
 import zc.buildout
 
 from slapos.recipe.librecipe import shlex
@@ -57,15 +56,21 @@
     self.buildout = buildout
     self.logger = logging.getLogger(name)
 
     self.options = options.copy() # If _options use self.optionIsTrue
     self._options(options) # Options Hook
     self.options = options.copy() # Updated options dict
 
-    self._ws = self.getWorkingSet()
+  @property
+  def _ws(self):
+    # getWorkingSet() is slow and it is not always needed.
+    # So _ws should be a lazy attribute.
+    if getattr(self, '_ws_internal', None) is None:
+      self._ws_internal = self.getWorkingSet()
+    return self._ws_internal
 
   def update(self):
     """By default update method does the same thing than install"""
     return self.install()
 
   def install(self):
     """Install method of the recipe. This must be overriden in child
@@ -106,84 +111,68 @@
       lines = []
 
     if not line in lines:
       lines.append(line)
       with io.open(filepath, 'w+', encoding=encoding) as f:
         f.write(u'\n'.join(lines))
 
-  def createPythonScript(self, name, absolute_function, arguments=''):
+  def createPythonScript(self, name, absolute_function, args=(), kw={}):
     """Create a python script using zc.buildout.easy_install.scripts
 
      * function should look like 'module.function', or only 'function'
        if it is a builtin function."""
-    absolute_function = tuple(absolute_function.rsplit('.', 1))
-    if len(absolute_function) == 1:
-      absolute_function = ('__builtin__',) + absolute_function
-    if len(absolute_function) != 2:
-      raise ValueError("A non valid function was given")
-
-    module, function = absolute_function
+    function = absolute_function.rsplit('.', 1)
+    if len(function) == 1:
+      module = '__builtin__'
+      function, = function
+    else:
+      module, function = function
     path, filename = os.path.split(os.path.abspath(name))
 
-    script = zc.buildout.easy_install.scripts(
-      [(filename, module, function)], self._ws, sys.executable,
-      path, arguments=arguments)[0]
-    return script
-
-  def createWrapper(self, name, command, parameters, comments=[],
-      parameters_extra=False, environment=None,
-      pidfile=None
-  ):
-    """
-    Creates a very simple (one command) shell script for process replacement.
-    Takes care of quoting.
-    if pidfile parameter is specified, then it will make the wrapper a singleton,
-    accepting to run only if no other instance is running.
-    """
-
-    lines = [ '#!/bin/sh' ]
-
-    for comment in comments:
-      lines.append('# %s' % comment)
-
-    if environment:
-      for key in environment:
-        lines.append('export %s=%s' % (key, environment[key]))
-
-    if pidfile:
-      lines.append(dedent("""\
-          # Check for other instances
-          pidfile=%s
-          if [ -e $pidfile ]; then
-            pid=$(cat $pidfile)
-            if [ ! -z "$(ps -p $pid | grep $(basename %s))" ]; then
-              echo "Already running with pid $pid."
-              exit 1
-            else
-              rm $pidfile
-            fi
-          fi
-          echo $$ > $pidfile""" % (pidfile, command)))
+    assert not isinstance(args, (basestring, dict)), args
+    args = map(repr, args)
+    args += map('%s=%r'.__mod__, kw.iteritems())
 
-    lines.append('exec %s' % shlex.quote(command))
+    return zc.buildout.easy_install.scripts(
+      [(filename, module, function)], self._ws, sys.executable,
+      path, arguments=', '.join(args))[0]
 
-    for param in parameters:
+  def createWrapper(self, path, args, env=None, **kw):
+    """Create a wrapper script for process replacement"""
+    assert args
+    if kw:
+      return self.createPythonScript(path,
+        'slapos.recipe.librecipe.execute.generic_exec',
+        (args, env) if env else (args,), kw)
+
+    # Simple case: creates a basic shell script for process replacement.
+    # This must be kept minimal to avoid code duplication with generic_exec.
+    # In particular, do not implement workaround for shebang size limitation
+    # here (note that this can't be done correctly with a POSIX shell, because
+    # the process can't be given a name).
+
+    lines = ['#!/bin/sh']
+
+    if env:
+      for k, v in sorted(env.iteritems()):
+        lines.append('export %s=%s' % (k, shlex.quote(v)))
+
+    lines.append('exec')
+
+    args = map(shlex.quote, args)
+    args.append('"$@"')
+    for arg in args:
       if len(lines[-1]) < 40:
-        lines[-1] += ' ' + shlex.quote(param)
+        lines[-1] += ' ' + arg
       else:
         lines[-1] += ' \\'
-        lines.append('\t' + shlex.quote(param))
-
-    if parameters_extra:
-        # pass-through further parameters
-        lines[-1] += ' \\'
-        lines.append('\t"$@"')
+        lines.append('\t' + arg)
 
-    content = '\n'.join(lines) + '\n'
-    return self.createFile(name, content, 0700)
+    lines.append('')
+    return self.createFile(path, '\n'.join(lines), 0700)
 
   def createDirectory(self, parent, name, mode=0700):
     path = os.path.join(parent, name)
     if not os.path.exists(path):
       os.mkdir(path, mode)
     elif not os.path.isdir(path):
       raise OSError("%r exists but is not a directory." % name)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/librecipe/filehash.py` & `slapos.cookbook-1.0.92/slapos/recipe/librecipe/filehash.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/firefox/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/6tunnel/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,33 +19,40 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
-#############################################################################
-
+##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
-import sys
 
 class Recipe(GenericBaseRecipe):
-  def install(self):
-
-    prefjs = self.createFile(
-      self.options['prefsjs-path'],
-      self.substituteTemplate(self.getTemplateFilename('prefs.js'), {}))
+  """
+  ipv4toipv6 tunnel configuration.
+  """
+  # Override in subclasses
+  template_name = None
 
-    config = {
-      'firefox_binary': self.options['firefox-path'],
-      'python_path': sys.executable,
-      'tmp_path': self.options['tmp-path'],
-      'pref_path': prefjs,
-      }
-
-    runner = self.createExecutable(
-      self.options['runner-path'],
-      self.substituteTemplate(self.getTemplateFilename('firefox_run.in'),
-                              config))
+  def install(self):
+    return [
+      self.createExecutable(
+        self.options['runner-path'],
+        self.substituteTemplate(
+          self.getTemplateFilename(self.template_name),
+          {
+            'ipv6': self.options['ipv6'],
+            'ipv6_port': self.options['ipv6-port'],
+            'ipv4': self.options['ipv4'],
+            'ipv4_port': self.options['ipv4-port'],
+            'shell_path': self.options['shell-path'],
+            '6tunnel_path': self.options['6tunnel-path'],
+          },
+        ),
+      )
+    ]
 
-    return [runner, prefjs]
+class SixToFour(Recipe):
+    template_name = '6to4.in'
 
+class FourToSix(Recipe):
+    template_name = '4to6.in'
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_zope/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/apachephp/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,126 +20,140 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-from slapos.recipe.librecipe import GenericBaseRecipe
-import binascii
-import hashlib
+import shutil
 import os
-import re
-import zc.buildout
+import signal
+from binascii import b2a_uu as uuencode
 
-_isurl = re.compile('([a-zA-Z0-9+.-]+)://').match
+from slapos.recipe.librecipe import GenericBaseRecipe
 
-# based on Zope2.utilities.mkzopeinstance.write_inituser
-def Zope2InitUser(path, username, password):
-  # Set password only once
-  # Currently, rely on existence of a simple file:
-  # Create it the first time, then next time, detect this file and do no-op.
-  inituser_done_path = '%s_done' % path
-  if os.path.exists(inituser_done_path):
-    return
-
-  if os.path.exists(path):
-    return
-  open(path, 'w').write('')
-  os.chmod(path, 0600)
-  open(path, 'w').write('%s:{SHA}%s\n' % (
-    username,binascii.b2a_base64(hashlib.sha1(password).digest())[:-1]))
+class Recipe(GenericBaseRecipe):
 
-  open(inituser_done_path, 'w').write('"inituser" file already created once.')
+  def __init__(self, buildout, name, options):
+    self.environ = {}
 
-class Recipe(GenericBaseRecipe):
-  def _options(self, options):
-    options['password'] = self.generatePassword()
-    options['deadlock-password'] = self.generatePassword()
+    environment_section = options.get('environment-section', '').strip()
+    if environment_section and environment_section in buildout:
+      # Use environment variables from the designated config section.
+      self.environ.update(buildout[environment_section])
+    for variable in options.get('environment', '').splitlines():
+      if variable.strip():
+        try:
+          key, value = variable.split('=', 1)
+          self.environ[key.strip()] = value
+        except ValueError:
+          raise zc.buildout.UserError('Invalid environment variable definition: %s', variable)
+    # Extrapolate the environment variables using values from the current
+    # environment.
+    for key in self.environ:
+      self.environ[key] = self.environ[key] % os.environ
+
+    return GenericBaseRecipe.__init__(self, buildout, name, options)
 
   def install(self):
-    """
-    All zope have to share file created by portal_classes
-    (until everything is integrated into the ZODB).
-    So, do not request zope instance and create multiple in the same partition.
-    """
     path_list = []
-    Zope2InitUser(self.options['inituser'], self.options['user'],
-      self.options['password'])
 
-    # Symlink to BT5 repositories defined in instance config.
-    # Those paths will eventually end up in the ZODB, and having symlinks
-    # inside the XXX makes it possible to reuse such ZODB with another software
-    # release[ version].
-    # Note: this path cannot be used for development, it's really just a
-    # read-only repository.
-    repository_path = self.options['bt5-repository']
-
-    self.bt5_repository_list = []
-    append = self.bt5_repository_list.append
-    for repository in self.options.get('bt5-repository-list', '').split():
-      repository = repository.strip()
-      if not repository:
-        continue
-
-      if _isurl(repository) and not repository.startswith("file://"):
-        # XXX: assume it's a valid URL
-        append(repository)
-        continue
-
-      if repository.startswith('file://'):
-        repository = repository.replace('file://', '', '')
-
-      if os.path.isabs(repository):
-        repo_id = hashlib.sha1(repository).hexdigest()
-        link = os.path.join(repository_path, repo_id)
-        if os.path.lexists(link):
-          if not os.path.islink(link):
-            raise zc.buildout.UserError(
-              'Target link already %r exists but it is not link' % link)
-          os.unlink(link)
-        os.symlink(repository, link)
-        self.logger.debug('Created link %r -> %r' % (link, repository_path))
-        # Always provide a URL-Type
-        append("file://" + link)
-
-    # Create zope configuration file
-    zope_config = dict(
-        thread_amount=self.options['thread-amount'],
-        zodb_root_path=self.options['zodb-path'],
-        zodb_cache_size=int(self.options['zodb-cache-size']),
-    )
-    zope_environment = dict(
-      TMP=self.options['tmp-path'],
-      TMPDIR=self.options['tmp-path'],
-      HOME=self.options['tmp-path'],
-      PATH=self.options['bin-path']
+    # Copy application if not already existing
+    htdocs_location = self.options['htdocs']
+    if not (os.path.exists(htdocs_location) and os.listdir(htdocs_location)):
+      try:
+        os.rmdir(htdocs_location)
+      except:
+        pass
+      shutil.copytree(self.options['source'], htdocs_location)
+
+    # Install php.ini
+    php_ini = self.createFile(os.path.join(self.options['php-ini-dir'],
+                                           'php.ini'),
+      self.substituteTemplate(self.getTemplateFilename('php.ini.in'),
+        dict(tmp_directory=self.options['tmp-dir']))
     )
-    # configure default Zope2 zcml
-    open(self.options['site-zcml'], 'w').write(open(self.getTemplateFilename(
-        'site.zcml')).read())
-    zope_config['instance'] = self.options['instance-path']
-    zope_config['event_log'] = self.options['event-log']
-    zope_config['z2_log'] = self.options['z2-log']
-    zope_config['pid-filename'] = self.options['pid-file']
-    zope_config['lock-filename'] = self.options['lock-file']
-    zope_config['products'] = 'products %s' % self.options['instance-products']
-    zope_config['address'] = '%s:%s' % (self.options['ip'], self.options['port'])
-    zope_config.update(dump_url=self.options['deadlock-path'],
-      secret=self.options['deadlock-password'])
-
-    zope_wrapper_template_location = self.getTemplateFilename('zope.conf.in')
-    zope_conf_content = self.substituteTemplate(zope_wrapper_template_location,
-      zope_config)
-
-    if ('promise-path' in self.options) and ('site-id' in self.options):
-      zope_conf_content += self.substituteTemplate(self.getTemplateFilename(
-          'zope.conf.promise.in'), {
-            'site-id': self.options['site-id'],
-            'promise-path': self.options['promise-path'],
-            })
-
-    zope_conf_path = self.createFile(self.options['configuration-file'], zope_conf_content)
-    path_list.append(zope_conf_path)
-    # Create init script
-    path_list.append(self.createPythonScript(self.options['wrapper'], 'slapos.recipe.librecipe.execute.executee', [[self.options['runzope-binary'].strip(), '-C', zope_conf_path], zope_environment]))
+    path_list.append(php_ini)
+
+    # Install apache
+    if self.optionIsTrue('default-conf', True):
+      apache_config = dict(
+        pid_file=self.options['pid-file'],
+        lock_file=self.options['lock-file'],
+        ip=self.options['ip'],
+        port=self.options['port'],
+        error_log=self.options['error-log'],
+        access_log=self.options['access-log'],
+        document_root=self.options['htdocs'],
+        php_ini_dir=self.options['php-ini-dir'],
+      )
+      httpd_conf = self.createFile(self.options['httpd-conf'],
+        self.substituteTemplate(self.getTemplateFilename('apache.in'),
+                                apache_config)
+      )
+      path_list.append(httpd_conf)
+
+    wrapper = self.createWrapper(self.options['wrapper'],
+                                 (self.options['httpd-binary'],
+                                     '-f',
+                                     self.options['httpd-conf'],
+                                     '-DFOREGROUND'
+                                     ),
+                                 self.environ)
+    path_list.append(wrapper)
+
+    secret_key_filename = os.path.join(self.buildout['buildout']['directory'],
+                                       '.php_secret_key')
+    if not os.path.exists(secret_key_filename):
+      secret_key = uuencode(os.urandom(45)).strip()
+      # Remove unsafe characters
+      secret_key = secret_key.translate(None, '"\'\\')
+      with open(secret_key_filename, 'w') as secret_key_file:
+        secret_key_file.write(secret_key)
+    else:
+      with open(secret_key_filename, 'r') as secret_key_file:
+        secret_key = secret_key_file.read()
+
+    # Generate application configuration file
+    if self.options.get('template'):
+      application_conf = dict(mysql_database=self.options['mysql-database'],
+                              mysql_user=self.options['mysql-username'],
+                              mysql_password=self.options['mysql-password'],
+                              mysql_host='%s:%s' % (self.options['mysql-host'],
+                                                    self.options['mysql-port']),
+                              mysql_ip=self.options['mysql-host'],
+                              mysql_port=self.options['mysql-port'],
+                              secret_key=secret_key,
+                              ip='[%s]' % self.options['ip'],
+                              port=self.options['port'],
+                              # XXX-Cedric: add frontend url.
+                             )
+      # Allow to give custom parameters to template
+      application_parameter_prefix = 'application-'
+      for key in self.options.keys():
+        if key.startswith(application_parameter_prefix):
+          application_conf[key.lstrip(application_parameter_prefix)] = self.options[key]
+
+      directory, file_ = os.path.split(self.options['configuration'])
+
+      path = self.options['htdocs']
+      if directory:
+        path = os.path.join(path, directory)
+        if not os.path.exists(path):
+          os.makedirs(path)
+        if not os.path.isdir(path):
+          raise OSError("Cannot create %r." % path)
+
+      destination = os.path.join(path, file_)
+      config = self.createFile(destination,
+        self.substituteTemplate(self.options['template'], application_conf))
+      path_list.append(config)
+
+    #if os.path.exists(self.options['pid-file']):
+    #  # Reload apache configuration
+    #  with open(self.options['pid-file']) as pid_file:
+    #    pid = int(pid_file.read().strip(), 10)
+    #  try:
+    #    os.kill(pid, signal.SIGUSR1) # Graceful restart
+    #  except OSError:
+    #    pass
     return path_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/README.zero_knowledge.txt` & `slapos.cookbook-1.0.92/slapos/recipe/README.zero_knowledge.rst`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/kvm/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/lampgeneric/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2013 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,61 +20,64 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-from slapos.recipe.librecipe import GenericBaseRecipe
+
+import shutil
 import os
-import sys
+import zc.buildout
 
-class Recipe(GenericBaseRecipe):
-  """
-  kvm instance configuration.
-  """
-  def install(self):
-    # Sanitize drive type parameter
-    self.options.setdefault('disk-type', 'virtio')
-    if not self.options.get('disk-type') in ['ide', 'scsi', 'sd',
-        'mtd', 'floppy', 'pflash', 'virtio']:
-      print 'Warning: "disk-type" parameter is not in allowed values. Using ' \
-          '"virtio" value.'
-      self.options['disk-type'] = 'virtio'
+from slapos.recipe.librecipe import GenericBaseRecipe
 
-    self.options['python-path'] = sys.executable
+class Recipe(GenericBaseRecipe):
+  # XXX-Cedric: write docstring
 
+  def install(self):
     path_list = []
 
-    if self.isTrueValue(self.options.get('use-nat')):
-      # XXX This could be done using Jinja.
-      for port in self.options['nat-rules'].split():
-        tunnel_port = int(port) + 10000
-        tunnel_path = self.createExecutable(
-            '%s-%s' % (self.options['6tunnel-wrapper-path'], tunnel_port),
-            self.substituteTemplate(
-                self.getTemplateFilename('6to4.in'),
-                {
-                    'ipv6': self.options['ipv6'],
-                    'ipv6_port': tunnel_port,
-                    'ipv4': self.options['ipv4'],
-                    'ipv4_port': tunnel_port,
-                    'shell_path': self.options['shell-path'],
-                    '6tunnel_path': self.options['6tunnel-path'],
-                },
-            ),
-        )
-        path_list.append(tunnel_path)
-
-    runner_path = self.createExecutable(
-        self.options['runner-path'],
-        self.substituteTemplate(self.getTemplateFilename('kvm_run.in'),
-                                self.options))
-    path_list.append(runner_path)
-
-    controller_path = self.createExecutable(
-      self.options['controller-path'],
-      self.substituteTemplate(self.getTemplateFilename('kvm_controller_run.in'),
-                              self.options))
+    # Download and unpack application if not already existing
+    htdocs_location = self.options['htdocs']
+    if not (os.path.exists(htdocs_location) and os.listdir(htdocs_location)):
+      try:
+        os.rmdir(htdocs_location)
+      except:
+        pass
+      self.download(htdocs_location)
+
+    # Install php.ini
+    php_ini = self.createFile(os.path.join(self.options['php-ini-dir'],
+                                           'php.ini'),
+      self.substituteTemplate(self.getTemplateFilename('php.ini.in'),
+        dict(tmp_directory=self.options['tmp-dir']))
+    )
+    path_list.append(php_ini)
+
+    # Install apache
+    apache_config = dict(
+      pid_file=self.options['pid-file'],
+      lock_file=self.options['lock-file'],
+      ip=self.options['ip'],
+      port=self.options['port'],
+      error_log=self.options['error-log'],
+      access_log=self.options['access-log'],
+      document_root=self.options['htdocs'],
+      php_ini_dir=self.options['php-ini-dir'],
+    )
+    httpd_conf = self.createFile(self.options['httpd-conf'],
+      self.substituteTemplate(self.getTemplateFilename('apache.in'),
+                              apache_config)
+    )
+    path_list.append(httpd_conf)
+
+    wrapper = self.createWrapper(self.options['wrapper'],
+                                 (self.options['httpd-binary'],
+                                     '-f',
+                                     self.options['httpd-conf'],
+                                     '-DFOREGROUND'
+                                     ))
+    path_list.append(wrapper)
 
 
     return path_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/kvm/template/kvm_controller_run.in` & `slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/template/kvm_controller_run.in`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-#!%(python-path)s
+#!%(python_path)s
 # BEWARE: This file is operated by slapgrid
 # BEWARE: It will be overwritten automatically
 
 # Echo client program
 import socket
 import time
 
-# XXX: to be factored with slapos.toolbox qemu qmp wrapper.
-
-socket_path = '%(socket-path)s'
-vnc_password = '%(vnc-passwd)s'
-
 # Connect to KVM qmp socket
 so = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
 connected = False
 while not connected:
   try:
-    so.connect(socket_path)
+    so.connect('%(socket_path)s')
   except socket.error:
     time.sleep(1)
   else:
     connected = True
 data = so.recv(1024)
 
 # Enable qmp
 so.send('{ "execute": "qmp_capabilities" }')
 data = so.recv(1024)
 
 # Set VNC password
 so.send('{ "execute": "change", ' \
         '"arguments": { "device": "vnc", "target": "password", ' \
-        '               "arg": "' + vnc_password + '" } }')
+        '               "arg": "%(vnc_passwd)s" } }')
 data = so.recv(1024)
 
 # Finish
 so.close()
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/sphinx/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/sphinx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     sphinx_conf_path = self.createFile(
         self.options['configuration-file'],
         self.substituteTemplate(self.getTemplateFilename('sphinx.conf.in'),
           config)
     )
 
     # Create init script
-    wrapper = self.createPythonScript(
+    wrapper = self.createWrapper(
         self.options['wrapper'],
-        'slapos.recipe.librecipe.execute.execute',
-        [self.options['sphinx-searchd-binary'].strip(), '-c',
-         sphinx_conf_path, '--nodetach'],
+        (self.options['sphinx-searchd-binary'].strip(), '-c',
+          sphinx_conf_path, '--nodetach'),
         )
 
     return [wrapper, sphinx_conf_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/sphinx/template/sphinx.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/sphinx/template/sphinx.conf.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/postgres/backup.py` & `slapos.cookbook-1.0.92/slapos/recipe/postgres/backup.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/postgres/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 #
 ##############################################################################
 
 import md5
 import os
 import subprocess
 import textwrap
+import shutil
 from zc.buildout import UserError
 
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 
 
 class Recipe(GenericBaseRecipe):
@@ -75,19 +76,27 @@
 
     def install(self):
         pgdata = self.options['pgdata-directory']
 
         # if the pgdata already exists, skip all steps, we don't need to do anything.
 
         if not os.path.exists(pgdata):
-            self.createCluster()
-            self.createConfig()
-            self.createDatabase()
-            self.updateSuperuser()
-            self.createRunScript()
+            try:
+                self.createCluster()
+                self.createConfig()
+                self.createDatabase()
+                self.updateSuperuser()
+                self.createRunScript()
+            except:
+                # do not leave half-installed postgresql - else next time we
+                # run we won't update it.
+                shutil.rmtree(pgdata)
+                raise
+
+
 
         # install() methods usually return the pathnames of managed files.
         # If they are missing, they will be rebuilt.
         # In this case, we already check for the existence of pgdata,
         # so we don't need to return anything here.
 
         return []
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/publishurl.py` & `slapos.cookbook-1.0.92/slapos/recipe/publishurl.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/varnishlogd.in` & `slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/varnishlogd.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/default.vcl.in` & `slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/default.vcl.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_varnish/template/varnishd.in` & `slapos.cookbook-1.0.92/slapos/recipe/generic_varnish/template/varnishd.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/redis/MyRedis2410.py` & `slapos.cookbook-1.0.92/slapos/recipe/redis/MyRedis2410.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/redis/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/redis/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 import os
-
+import sys
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
 
   def install(self):
     path_list = []
 
@@ -41,31 +41,45 @@
     configuration = dict(pid_file=self.options['pid_file'],
                         port=self.options['port'],
                         ipv6=self.options['ipv6'],
                         server_dir=self.options['server_dir'],
                         log_file=self.options['log_file'],
                         master_passwd=master_passwd
     )
+    if self.options.get('unixsocket'):
+        unixsocket = "unixsocket %s\nunixsocketperm 700" % self.options['unixsocket']
+    else:
+        unixsocket = ""
+    configuration['unixsocket'] = unixsocket
 
     config = self.createFile(config_file,
       self.substituteTemplate(self.getTemplateFilename('redis.conf.in'),
       configuration))
     path_list.append(config)
 
-    redis = self.createPythonScript(
+    redis = self.createWrapper(
       self.options['wrapper'],
-      'slapos.recipe.librecipe.execute.execute',
-      [self.options['server_bin'], config_file]
+      (self.options['server_bin'], config_file),
     )
     path_list.append(redis)
 
     promise_script = self.options.get('promise_wrapper', '').strip()
     if promise_script:
       promise = self.createPythonScript(
         promise_script,
-        '%s.promise.main' % __name__,
-        dict(host=self.options['ipv6'], port=self.options['port'])
+        __name__ + '.promise',
+        (self.options['ipv6'], int(self.options['port']),
+         self.options.get('unixsocket'))
       )
       path_list.append(promise)
 
     return path_list
 
+
+def promise(host, port, unixsocket):
+  from .MyRedis2410 import Redis
+  try:
+    r = Redis(host=host, port=port, unix_socket_path=unixsocket, db=0)
+    r.publish("Promise-Service","SlapOS Promise")
+    r.connection_pool.disconnect()
+  except Exception, e:
+    sys.exit(e)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/redis/template/redis.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/redis/template/redis.conf.in`

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,178 @@
-# Redis configuration file example
+# Redis configuration file example.
+#
+# Note that in order to read the configuration file, Redis must be
+# started with the file path as first argument:
+#
+# ./redis-server /path/to/redis.conf
 
 # Note on units: when memory size is needed, it is possible to specify
 # it in the usual form of 1k 5GB 4M and so forth:
 #
 # 1k => 1000 bytes
 # 1kb => 1024 bytes
 # 1m => 1000000 bytes
 # 1mb => 1024*1024 bytes
 # 1g => 1000000000 bytes
 # 1gb => 1024*1024*1024 bytes
 #
 # units are case insensitive so 1GB 1Gb 1gB are all the same.
 
+################################## INCLUDES ###################################
+
+# Include one or more other config files here.  This is useful if you
+# have a standard template that goes to all Redis servers but also need
+# to customize a few per-server settings.  Include files can include
+# other files, so use this wisely.
+#
+# Notice option "include" won't be rewritten by command "CONFIG REWRITE"
+# from admin or Redis Sentinel. Since Redis always uses the last processed
+# line as value of a configuration directive, you'd better put includes
+# at the beginning of this file to avoid overwriting config change at runtime.
+#
+# If instead you are interested in using includes to override configuration
+# options, it is better to use include as the last line.
+#
+# include /path/to/local.conf
+# include /path/to/other.conf
+
+################################ GENERAL  #####################################
+
 # By default Redis does not run as a daemon. Use 'yes' if you need it.
 # Note that Redis will write a pid file in /var/run/redis.pid when daemonized.
 daemonize no
 
 # When running daemonized, Redis writes a pid file in /var/run/redis.pid by
 # default. You can specify a custom pid file location here.
 pidfile %(pid_file)s
 
 # Accept connections on the specified port, default is 6379.
 # If port 0 is specified Redis will not listen on a TCP socket.
-port6 %(port)s
-port 0
+port %(port)s
 
-# If you want you can bind a single interface, if the bind option is not
-# specified all the interfaces will listen for incoming connections.
-# Bind can also be an IPv6 address
+# TCP listen() backlog.
+#
+# In high requests-per-second environments you need an high backlog in order
+# to avoid slow clients connections issues. Note that the Linux kernel
+# will silently truncate it to the value of /proc/sys/net/core/somaxconn so
+# make sure to raise both the value of somaxconn and tcp_max_syn_backlog
+# in order to get the desired effect.
+tcp-backlog 511
+
+# By default Redis listens for connections from all the network interfaces
+# available on the server. It is possible to listen to just one or multiple
+# interfaces using the "bind" configuration directive, followed by one or
+# more IP addresses.
+#
+# Examples:
+#
+# bind 192.168.1.100 10.0.0.1
 # bind 127.0.0.1
-# bind ::1
-bind6 %(ipv6)s
+bind %(ipv6)s
 
-# Specify the path for the unix socket that will be used to listen for
+# Specify the path for the Unix socket that will be used to listen for
 # incoming connections. There is no default, so Redis will not listen
 # on a unix socket when not specified.
-#
-# unixsocket /tmp/redis.sock
-# unixsocketperm 755
+%(unixsocket)s
 
 # Close the connection after a client is idle for N seconds (0 to disable)
 timeout 0
 
-# Set server verbosity to 'debug'
-# it can be one of:
+# TCP keepalive.
+#
+# If non-zero, use SO_KEEPALIVE to send TCP ACKs to clients in absence
+# of communication. This is useful for two reasons:
+#
+# 1) Detect dead peers.
+# 2) Take the connection alive from the point of view of network
+#    equipment in the middle.
+#
+# On Linux, the specified value (in seconds) is the period used to send ACKs.
+# Note that to close the connection the double of the time is needed.
+# On other kernels the period depends on the kernel configuration.
+#
+# A reasonable value for this option is 60 seconds.
+tcp-keepalive 0
+
+# Specify the server verbosity level.
+# This can be one of:
 # debug (a lot of information, useful for development/testing)
 # verbose (many rarely useful info, but not a mess like the debug level)
 # notice (moderately verbose, what you want in production probably)
 # warning (only very important / critical messages are logged)
 loglevel notice
 
-# Specify the log file name. Also 'stdout' can be used to force
+# Specify the log file name. Also the empty string can be used to force
 # Redis to log on the standard output. Note that if you use standard
 # output for logging but daemonize, logs will be sent to /dev/null
 logfile %(log_file)s
 
 # To enable logging to the system logger, just set 'syslog-enabled' to yes,
 # and optionally update the other syslog parameters to suit your needs.
 # syslog-enabled no
 
 # Specify the syslog identity.
 # syslog-ident redis
 
-# Specify the syslog facility.  Must be USER or between LOCAL0-LOCAL7.
+# Specify the syslog facility. Must be USER or between LOCAL0-LOCAL7.
 # syslog-facility local0
 
 # Set the number of databases. The default database is DB 0, you can select
 # a different one on a per-connection basis using SELECT <dbid> where
 # dbid is a number between 0 and 'databases'-1
 databases 16
 
-################################ SNAPSHOTTING  #################################
+################################ SNAPSHOTTING  ################################
 #
 # Save the DB on disk:
 #
 #   save <seconds> <changes>
 #
 #   Will save the DB if both the given number of seconds and the given
 #   number of write operations against the DB occurred.
 #
 #   In the example below the behaviour will be to save:
 #   after 900 sec (15 min) if at least 1 key changed
 #   after 300 sec (5 min) if at least 10 keys changed
 #   after 60 sec if at least 10000 keys changed
 #
-#   Note: you can disable saving at all commenting all the "save" lines.
+#   Note: you can disable saving completely by commenting out all "save" lines.
 #
 #   It is also possible to remove all the previously configured save
 #   points by adding a save directive with a single empty string argument
 #   like in the following example:
 #
 #   save ""
 
 save 900 1
 save 300 10
 save 60 10000
 
 # By default Redis will stop accepting writes if RDB snapshots are enabled
 # (at least one save point) and the latest background save failed.
-# This will make the user aware (in an hard way) that data is not persisting
+# This will make the user aware (in a hard way) that data is not persisting
 # on disk properly, otherwise chances are that no one will notice and some
-# distater will happen.
+# disaster will happen.
 #
 # If the background saving process will start working again Redis will
 # automatically allow writes again.
 #
 # However if you have setup your proper monitoring of the Redis server
 # and persistence, you may want to disable this feature so that Redis will
-# continue to work as usually even if there are problems with disk,
+# continue to work as usual even if there are problems with disk,
 # permissions, and so forth.
 stop-writes-on-bgsave-error yes
 
 # Compress string objects using LZF when dump .rdb databases?
 # For default that's set to 'yes' as it's almost always a win.
 # If you want to save some CPU in the saving child set it to 'no' but
 # the dataset will likely be bigger if you have compressible values or keys.
 rdbcompression yes
 
-# Since verison 5 of RDB a CRC64 checksum is placed at the end of the file.
+# Since version 5 of RDB a CRC64 checksum is placed at the end of the file.
 # This makes the format more resistant to corruption but there is a performance
 # hit to pay (around 10%%) when saving and loading RDB files, so you can disable it
 # for maximum performances.
 #
 # RDB files created with checksum disabled have a checksum of zero that will
 # tell the loading code to skip the check.
 rdbchecksum yes
@@ -130,43 +181,52 @@
 dbfilename dump.rdb
 
 # The working directory.
 #
 # The DB will be written inside this directory, with the filename specified
 # above using the 'dbfilename' configuration directive.
 #
-# Also the Append Only File will be created inside this directory.
+# The Append Only File will also be created inside this directory.
 #
 # Note that you must specify a directory here, not a file name.
 dir %(server_dir)s
 
 ################################# REPLICATION #################################
 
 # Master-Slave replication. Use slaveof to make a Redis instance a copy of
-# another Redis server. Note that the configuration is local to the slave
-# so for example it is possible to configure the slave to save the DB with a
-# different interval, or to listen to another port, and so on.
+# another Redis server. A few things to understand ASAP about Redis replication.
+#
+# 1) Redis replication is asynchronous, but you can configure a master to
+#    stop accepting writes if it appears to be not connected with at least
+#    a given number of slaves.
+# 2) Redis slaves are able to perform a partial resynchronization with the
+#    master if the replication link is lost for a relatively small amount of
+#    time. You may want to configure the replication backlog size (see the next
+#    sections of this file) with a sensible value depending on your needs.
+# 3) Replication is automatic and does not need user intervention. After a
+#    network partition slaves automatically try to reconnect to masters
+#    and resynchronize with them.
 #
 # slaveof <masterip> <masterport>
 
 # If the master is password protected (using the "requirepass" configuration
 # directive below) it is possible to tell the slave to authenticate before
 # starting the replication synchronization process, otherwise the master will
 # refuse the slave request.
 #
 %(master_passwd)s
 
-# When a slave lost the connection with the master, or when the replication
+# When a slave loses its connection with the master, or when the replication
 # is still in progress, the slave can act in two different ways:
 #
 # 1) if slave-serve-stale-data is set to 'yes' (the default) the slave will
 #    still reply to client requests, possibly with out of date data, or the
 #    data set may just be empty if this is the first synchronization.
 #
-# 2) if slave-serve-stale data is set to 'no' the slave will reply with
+# 2) if slave-serve-stale-data is set to 'no' the slave will reply with
 #    an error "SYNC with master in progress" to all the kind of commands
 #    but to INFO and SLAVEOF.
 #
 slave-serve-stale-data yes
 
 # You can configure a slave instance to accept writes or not. Writing against
 # a slave instance may be useful to store some ephemeral data (because data
@@ -175,34 +235,154 @@
 # misconfiguration.
 #
 # Since Redis 2.6 by default slaves are read-only.
 #
 # Note: read only slaves are not designed to be exposed to untrusted clients
 # on the internet. It's just a protection layer against misuse of the instance.
 # Still a read only slave exports by default all the administrative commands
-# such as CONFIG, DEBUG, and so forth. To a limited extend you can improve
+# such as CONFIG, DEBUG, and so forth. To a limited extent you can improve
 # security of read only slaves using 'rename-command' to shadow all the
 # administrative / dangerous commands.
 slave-read-only yes
 
+# Replication SYNC strategy: disk or socket.
+#
+# -------------------------------------------------------
+# WARNING: DISKLESS REPLICATION IS EXPERIMENTAL CURRENTLY
+# -------------------------------------------------------
+#
+# New slaves and reconnecting slaves that are not able to continue the replication
+# process just receiving differences, need to do what is called a "full
+# synchronization". An RDB file is transmitted from the master to the slaves.
+# The transmission can happen in two different ways:
+#
+# 1) Disk-backed: The Redis master creates a new process that writes the RDB
+#                 file on disk. Later the file is transferred by the parent
+#                 process to the slaves incrementally.
+# 2) Diskless: The Redis master creates a new process that directly writes the
+#              RDB file to slave sockets, without touching the disk at all.
+#
+# With disk-backed replication, while the RDB file is generated, more slaves
+# can be queued and served with the RDB file as soon as the current child producing
+# the RDB file finishes its work. With diskless replication instead once
+# the transfer starts, new slaves arriving will be queued and a new transfer
+# will start when the current one terminates.
+#
+# When diskless replication is used, the master waits a configurable amount of
+# time (in seconds) before starting the transfer in the hope that multiple slaves
+# will arrive and the transfer can be parallelized.
+#
+# With slow disks and fast (large bandwidth) networks, diskless replication
+# works better.
+repl-diskless-sync no
+
+# When diskless replication is enabled, it is possible to configure the delay
+# the server waits in order to spawn the child that trnasfers the RDB via socket
+# to the slaves.
+#
+# This is important since once the transfer starts, it is not possible to serve
+# new slaves arriving, that will be queued for the next RDB transfer, so the server
+# waits a delay in order to let more slaves arrive.
+#
+# The delay is specified in seconds, and by default is 5 seconds. To disable
+# it entirely just set it to 0 seconds and the transfer will start ASAP.
+repl-diskless-sync-delay 5
+
 # Slaves send PINGs to server in a predefined interval. It's possible to change
 # this interval with the repl_ping_slave_period option. The default value is 10
 # seconds.
 #
 # repl-ping-slave-period 10
 
-# The following option sets a timeout for both Bulk transfer I/O timeout and
-# master data or ping response timeout. The default value is 60 seconds.
+# The following option sets the replication timeout for:
+#
+# 1) Bulk transfer I/O during SYNC, from the point of view of slave.
+# 2) Master timeout from the point of view of slaves (data, pings).
+# 3) Slave timeout from the point of view of masters (REPLCONF ACK pings).
 #
 # It is important to make sure that this value is greater than the value
 # specified for repl-ping-slave-period otherwise a timeout will be detected
 # every time there is low traffic between the master and the slave.
 #
 # repl-timeout 60
 
+# Disable TCP_NODELAY on the slave socket after SYNC?
+#
+# If you select "yes" Redis will use a smaller number of TCP packets and
+# less bandwidth to send data to slaves. But this can add a delay for
+# the data to appear on the slave side, up to 40 milliseconds with
+# Linux kernels using a default configuration.
+#
+# If you select "no" the delay for data to appear on the slave side will
+# be reduced but more bandwidth will be used for replication.
+#
+# By default we optimize for low latency, but in very high traffic conditions
+# or when the master and slaves are many hops away, turning this to "yes" may
+# be a good idea.
+repl-disable-tcp-nodelay no
+
+# Set the replication backlog size. The backlog is a buffer that accumulates
+# slave data when slaves are disconnected for some time, so that when a slave
+# wants to reconnect again, often a full resync is not needed, but a partial
+# resync is enough, just passing the portion of data the slave missed while
+# disconnected.
+#
+# The bigger the replication backlog, the longer the time the slave can be
+# disconnected and later be able to perform a partial resynchronization.
+#
+# The backlog is only allocated once there is at least a slave connected.
+#
+# repl-backlog-size 1mb
+
+# After a master has no longer connected slaves for some time, the backlog
+# will be freed. The following option configures the amount of seconds that
+# need to elapse, starting from the time the last slave disconnected, for
+# the backlog buffer to be freed.
+#
+# A value of 0 means to never release the backlog.
+#
+# repl-backlog-ttl 3600
+
+# The slave priority is an integer number published by Redis in the INFO output.
+# It is used by Redis Sentinel in order to select a slave to promote into a
+# master if the master is no longer working correctly.
+#
+# A slave with a low priority number is considered better for promotion, so
+# for instance if there are three slaves with priority 10, 100, 25 Sentinel will
+# pick the one with priority 10, that is the lowest.
+#
+# However a special priority of 0 marks the slave as not able to perform the
+# role of master, so a slave with priority of 0 will never be selected by
+# Redis Sentinel for promotion.
+#
+# By default the priority is 100.
+slave-priority 100
+
+# It is possible for a master to stop accepting writes if there are less than
+# N slaves connected, having a lag less or equal than M seconds.
+#
+# The N slaves need to be in "online" state.
+#
+# The lag in seconds, that must be <= the specified value, is calculated from
+# the last ping received from the slave, that is usually sent every second.
+#
+# This option does not GUARANTEE that N replicas will accept the write, but
+# will limit the window of exposure for lost writes in case not enough slaves
+# are available, to the specified number of seconds.
+#
+# For example to require at least 3 slaves with a lag <= 10 seconds use:
+#
+# min-slaves-to-write 3
+# min-slaves-max-lag 10
+#
+# Setting one or the other to 0 disables the feature.
+#
+# By default min-slaves-to-write is set to 0 (feature disabled) and
+# min-slaves-max-lag is set to 10.
+
 ################################## SECURITY ###################################
 
 # Require clients to issue AUTH <PASSWORD> before processing any other
 # commands.  This might be useful in environments in which you do not trust
 # others with access to the host running redis-server.
 #
 # This should stay commented out for backward compatibility and because most
@@ -214,50 +394,53 @@
 #
 # requirepass foobared
 
 # Command renaming.
 #
 # It is possible to change the name of dangerous commands in a shared
 # environment. For instance the CONFIG command may be renamed into something
-# of hard to guess so that it will be still available for internal-use
-# tools but not available for general clients.
+# hard to guess so that it will still be available for internal-use tools
+# but not available for general clients.
 #
 # Example:
 #
 # rename-command CONFIG b840fc02d524045429941cc15f59e41cb7be6c52
 #
-# It is also possible to completely kill a command renaming it into
+# It is also possible to completely kill a command by renaming it into
 # an empty string:
 #
 # rename-command CONFIG ""
+#
+# Please note that changing the name of commands that are logged into the
+# AOF file or transmitted to slaves may cause problems.
 
 ################################### LIMITS ####################################
 
 # Set the max number of connected clients at the same time. By default
 # this limit is set to 10000 clients, however if the Redis server is not
-# able ot configure the process file limit to allow for the specified limit
+# able to configure the process file limit to allow for the specified limit
 # the max number of allowed clients is set to the current file limit
 # minus 32 (as Redis reserves a few file descriptors for internal uses).
 #
 # Once the limit is reached Redis will close all the new connections sending
 # an error 'max number of clients reached'.
 #
 # maxclients 10000
 
 # Don't use more memory than the specified amount of bytes.
 # When the memory limit is reached Redis will try to remove keys
-# accordingly to the eviction policy selected (see maxmemmory-policy).
+# according to the eviction policy selected (see maxmemory-policy).
 #
 # If Redis can't remove keys according to the policy, or if the policy is
 # set to 'noeviction', Redis will start to reply with errors to commands
 # that would use more memory, like SET, LPUSH, and so on, and will continue
 # to reply to read-only commands like GET.
 #
 # This option is usually useful when using Redis as an LRU cache, or to set
-# an hard memory limit for an instance (using the 'noeviction' policy).
+# a hard memory limit for an instance (using the 'noeviction' policy).
 #
 # WARNING: If you have slaves attached to an instance with maxmemory on,
 # the size of the output buffers needed to feed the slaves are subtracted
 # from the used memory count, so that network problems / resyncs will
 # not trigger a loop where keys are evicted, and in turn the output
 # buffer of slaves is full with DELs of keys evicted triggering the deletion
 # of more keys, and so forth until the database is completely emptied.
@@ -265,27 +448,27 @@
 # In short... if you have slaves attached it is suggested that you set a lower
 # limit for maxmemory so that there is some free RAM on the system for slave
 # output buffers (but this is not needed if the policy is 'noeviction').
 #
 # maxmemory <bytes>
 
 # MAXMEMORY POLICY: how Redis will select what to remove when maxmemory
-# is reached? You can select among five behavior:
+# is reached. You can select among five behaviors:
 #
 # volatile-lru -> remove the key with an expire set using an LRU algorithm
-# allkeys-lru -> remove any key accordingly to the LRU algorithm
+# allkeys-lru -> remove any key according to the LRU algorithm
 # volatile-random -> remove a random key with an expire set
 # allkeys-random -> remove a random key, any key
 # volatile-ttl -> remove the key with the nearest expire time (minor TTL)
 # noeviction -> don't expire at all, just return an error on write operations
 #
-# Note: with all the kind of policies, Redis will return an error on write
-#       operations, when there are not suitable keys for eviction.
+# Note: with any of the above policies, Redis will return an error on write
+#       operations, when there are no suitable keys for eviction.
 #
-#       At the date of writing this commands are: set setnx setex append
+#       At the date of writing these commands are: set setnx setex append
 #       incr decr rpush lpush rpushx lpushx linsert lset rpoplpush sadd
 #       sinter sinterstore sunion sunionstore sdiff sdiffstore zadd zincrby
 #       zunionstore zinterstore hset hsetnx hmset hincrby incrby decrby
 #       getset mset msetnx exec sort
 #
 # The default is:
 #
@@ -318,27 +501,28 @@
 # with the better durability guarantees.
 #
 # Please check http://redis.io/topics/persistence for more information.
 
 appendonly no
 
 # The name of the append only file (default: "appendonly.aof")
-# appendfilename appendonly.aof
+
+appendfilename "appendonly.aof"
 
 # The fsync() call tells the Operating System to actually write data on disk
-# instead to wait for more data in the output buffer. Some OS will really flush
+# instead of waiting for more data in the output buffer. Some OS will really flush
 # data on disk, some other OS will just try to do it ASAP.
 #
 # Redis supports three different modes:
 #
 # no: don't fsync, just let the OS flush the data when it wants. Faster.
-# always: fsync after every write to the append only log . Slow, Safest.
+# always: fsync after every write to the append only log. Slow, Safest.
 # everysec: fsync only one time every second. Compromise.
 #
-# The default is "everysec" that's usually the right compromise between
+# The default is "everysec", as that's usually the right compromise between
 # speed and data safety. It's up to you to understand if you can relax this to
 # "no" that will let the operating system flush the output buffer when
 # it wants, for better performances (but if you can live with the idea of
 # some data loss consider the default persistence mode that's snapshotting),
 # or on the contrary, use "always" that's very slow but a bit safer than
 # everysec.
 #
@@ -358,80 +542,86 @@
 # this currently, as even performing fsync in a different thread will block
 # our synchronous write(2) call.
 #
 # In order to mitigate this problem it's possible to use the following option
 # that will prevent fsync() from being called in the main process while a
 # BGSAVE or BGREWRITEAOF is in progress.
 #
-# This means that while another child is saving the durability of Redis is
-# the same as "appendfsync none", that in practical terms means that it is
-# possible to lost up to 30 seconds of log in the worst scenario (with the
+# This means that while another child is saving, the durability of Redis is
+# the same as "appendfsync none". In practical terms, this means that it is
+# possible to lose up to 30 seconds of log in the worst scenario (with the
 # default Linux settings).
 #
 # If you have latency problems turn this to "yes". Otherwise leave it as
 # "no" that is the safest pick from the point of view of durability.
+
 no-appendfsync-on-rewrite no
 
 # Automatic rewrite of the append only file.
 # Redis is able to automatically rewrite the log file implicitly calling
-# BGREWRITEAOF when the AOF log size will growth by the specified percentage.
+# BGREWRITEAOF when the AOF log size grows by the specified percentage.
 #
 # This is how it works: Redis remembers the size of the AOF file after the
-# latest rewrite (or if no rewrite happened since the restart, the size of
+# latest rewrite (if no rewrite has happened since the restart, the size of
 # the AOF at startup is used).
 #
 # This base size is compared to the current size. If the current size is
 # bigger than the specified percentage, the rewrite is triggered. Also
 # you need to specify a minimal size for the AOF file to be rewritten, this
 # is useful to avoid rewriting the AOF file even if the percentage increase
 # is reached but it is still pretty small.
 #
 # Specify a percentage of zero in order to disable the automatic AOF
 # rewrite feature.
 
 auto-aof-rewrite-percentage 100
 auto-aof-rewrite-min-size 64mb
 
+# An AOF file may be found to be truncated at the end during the Redis
+# startup process, when the AOF data gets loaded back into memory.
+# This may happen when the system where Redis is running
+# crashes, especially when an ext4 filesystem is mounted without the
+# data=ordered option (however this can't happen when Redis itself
+# crashes or aborts but the operating system still works correctly).
+#
+# Redis can either exit with an error when this happens, or load as much
+# data as possible (the default now) and start if the AOF file is found
+# to be truncated at the end. The following option controls this behavior.
+#
+# If aof-load-truncated is set to yes, a truncated AOF file is loaded and
+# the Redis server starts emitting a log to inform the user of the event.
+# Otherwise if the option is set to no, the server aborts with an error
+# and refuses to start. When the option is set to no, the user requires
+# to fix the AOF file using the "redis-check-aof" utility before to restart
+# the server.
+#
+# Note that if the AOF file will be found to be corrupted in the middle
+# the server will still exit with an error. This option only applies when
+# Redis will try to read more data from the AOF file but not enough bytes
+# will be found.
+aof-load-truncated yes
+
 ################################ LUA SCRIPTING  ###############################
 
 # Max execution time of a Lua script in milliseconds.
 #
 # If the maximum execution time is reached Redis will log that a script is
 # still in execution after the maximum allowed time and will start to
 # reply to queries with an error.
 #
-# When a long running script exceed the maximum execution time only the
+# When a long running script exceeds the maximum execution time only the
 # SCRIPT KILL and SHUTDOWN NOSAVE commands are available. The first can be
 # used to stop a script that did not yet called write commands. The second
-# is the only way to shut down the server in the case a write commands was
-# already issue by the script but the user don't want to wait for the natural
+# is the only way to shut down the server in the case a write command was
+# already issued by the script but the user doesn't want to wait for the natural
 # termination of the script.
 #
 # Set it to 0 or a negative value for unlimited execution without warnings.
 lua-time-limit 5000
 
-################################ REDIS CLUSTER  ###############################
-#
-# Normal Redis instances can't be part of a Redis Cluster, only nodes that are
-# started as cluster nodes can. In order to start a Redis instance as a
-# cluster node enable the cluster support uncommenting the following:
-#
-# cluster-enabled yes
-
-# Every cluster node has a cluster configuration file. This file is not
-# intended to be edited by hand. It is created and updated by Redis nodes.
-# Every Redis Cluster node requires a different cluster configuration file.
-# Make sure that instances running in the same system does not have
-# overlapping cluster configuration file names.
-#
-# cluster-config-file nodes-6379.conf
-
-# In order to setup your cluster make sure to read the documentation
-# available at http://redis.io web site.
-
 ################################## SLOW LOG ###################################
 
 # The Redis Slow Log is a system to log queries that exceeded a specified
 # execution time. The execution time does not include the I/O operations
 # like talking with the client, sending the reply and so forth,
 # but just the time needed to actually execute the command (this is the only
 # stage of command execution where the thread is blocked and can not serve
@@ -448,14 +638,81 @@
 # a value of zero forces the logging of every command.
 slowlog-log-slower-than 10000
 
 # There is no limit to this length. Just be aware that it will consume memory.
 # You can reclaim memory used by the slow log with SLOWLOG RESET.
 slowlog-max-len 128
 
+################################ LATENCY MONITOR ##############################
+
+# The Redis latency monitoring subsystem samples different operations
+# at runtime in order to collect data related to possible sources of
+# latency of a Redis instance.
+#
+# Via the LATENCY command this information is available to the user that can
+# print graphs and obtain reports.
+#
+# The system only logs operations that were performed in a time equal or
+# greater than the amount of milliseconds specified via the
+# latency-monitor-threshold configuration directive. When its value is set
+# to zero, the latency monitor is turned off.
+#
+# By default latency monitoring is disabled since it is mostly not needed
+# if you don't have latency issues, and collecting data has a performance
+# impact, that while very small, can be measured under big load. Latency
+# monitoring can easily be enalbed at runtime using the command
+# "CONFIG SET latency-monitor-threshold <milliseconds>" if needed.
+latency-monitor-threshold 0
+
+############################# Event notification ##############################
+
+# Redis can notify Pub/Sub clients about events happening in the key space.
+# This feature is documented at http://redis.io/topics/notifications
+#
+# For instance if keyspace events notification is enabled, and a client
+# performs a DEL operation on key "foo" stored in the Database 0, two
+# messages will be published via Pub/Sub:
+#
+# PUBLISH __keyspace@0__:foo del
+# PUBLISH __keyevent@0__:del foo
+#
+# It is possible to select the events that Redis will notify among a set
+# of classes. Every class is identified by a single character:
+#
+#  K     Keyspace events, published with __keyspace@<db>__ prefix.
+#  E     Keyevent events, published with __keyevent@<db>__ prefix.
+#  g     Generic commands (non-type specific) like DEL, EXPIRE, RENAME, ...
+#  $     String commands
+#  l     List commands
+#  s     Set commands
+#  h     Hash commands
+#  z     Sorted set commands
+#  x     Expired events (events generated every time a key expires)
+#  e     Evicted events (events generated when a key is evicted for maxmemory)
+#  A     Alias for g$lshzxe, so that the "AKE" string means all the events.
+#
+#  The "notify-keyspace-events" takes as argument a string that is composed
+#  of zero or multiple characters. The empty string means that notifications
+#  are disabled.
+#
+#  Example: to enable list and generic events, from the point of view of the
+#           event name, use:
+#
+#  notify-keyspace-events Elg
+#
+#  Example 2: to get the stream of the expired keys subscribing to channel
+#             name __keyevent@0__:expired use:
+#
+#  notify-keyspace-events Ex
+#
+#  By default all notifications are disabled because most users don't need
+#  this feature and the feature has some overhead. Note that if you don't
+#  specify at least one of K or E, no events will be delivered.
+notify-keyspace-events ""
+
 ############################### ADVANCED CONFIG ###############################
 
 # Hashes are encoded using a memory efficient data structure when they have a
 # small number of entries, and the biggest entry does not exceed a given
 # threshold. These thresholds can be configured using the following directives.
 hash-max-ziplist-entries 512
 hash-max-ziplist-value 64
@@ -463,56 +720,70 @@
 # Similarly to hashes, small lists are also encoded in a special way in order
 # to save a lot of space. The special representation is only used when
 # you are under the following limits:
 list-max-ziplist-entries 512
 list-max-ziplist-value 64
 
 # Sets have a special encoding in just one case: when a set is composed
-# of just strings that happens to be integers in radix 10 in the range
+# of just strings that happen to be integers in radix 10 in the range
 # of 64 bit signed integers.
 # The following configuration setting sets the limit in the size of the
 # set in order to use this special memory saving encoding.
 set-max-intset-entries 512
 
 # Similarly to hashes and lists, sorted sets are also specially encoded in
 # order to save a lot of space. This encoding is only used when the length and
 # elements of a sorted set are below the following limits:
 zset-max-ziplist-entries 128
 zset-max-ziplist-value 64
 
+# HyperLogLog sparse representation bytes limit. The limit includes the
+# 16 bytes header. When an HyperLogLog using the sparse representation crosses
+# this limit, it is converted into the dense representation.
+#
+# A value greater than 16000 is totally useless, since at that point the
+# dense representation is more memory efficient.
+#
+# The suggested value is ~ 3000 in order to have the benefits of
+# the space efficient encoding without slowing down too much PFADD,
+# which is O(N) with the sparse encoding. The value can be raised to
+# ~ 10000 when CPU is not a concern, but space is, and the data set is
+# composed of many HyperLogLogs with cardinality in the 0 - 15000 range.
+hll-sparse-max-bytes 3000
+
 # Active rehashing uses 1 millisecond every 100 milliseconds of CPU time in
 # order to help rehashing the main Redis hash table (the one mapping top-level
 # keys to values). The hash table implementation Redis uses (see dict.c)
-# performs a lazy rehashing: the more operation you run into an hash table
+# performs a lazy rehashing: the more operation you run into a hash table
 # that is rehashing, the more rehashing "steps" are performed, so if the
 # server is idle the rehashing is never complete and some more memory is used
 # by the hash table.
 #
 # The default is to use this millisecond 10 times every second in order to
-# active rehashing the main dictionaries, freeing memory when possible.
+# actively rehash the main dictionaries, freeing memory when possible.
 #
 # If unsure:
 # use "activerehashing no" if you have hard latency requirements and it is
-# not a good thing in your environment that Redis can reply form time to time
+# not a good thing in your environment that Redis can reply from time to time
 # to queries with 2 milliseconds delay.
 #
 # use "activerehashing yes" if you don't have such hard requirements but
 # want to free memory asap when possible.
 activerehashing yes
 
 # The client output buffer limits can be used to force disconnection of clients
 # that are not reading data from the server fast enough for some reason (a
 # common reason is that a Pub/Sub client can't consume messages as fast as the
 # publisher can produce them).
 #
 # The limit can be set differently for the three different classes of clients:
 #
-# normal -> normal clients
-# slave  -> slave clients and MONITOR clients
-# pubsub -> clients subcribed to at least one pubsub channel or pattern
+# normal -> normal clients including MONITOR clients
+# slave  -> slave clients
+# pubsub -> clients subscribed to at least one pubsub channel or pattern
 #
 # The syntax of every client-output-buffer-limit directive is the following:
 #
 # client-output-buffer-limit <class> <hard limit> <soft limit> <soft seconds>
 #
 # A client is immediately disconnected once the hard limit is reached, or if
 # the soft limit is reached and remains reached for the specified number of
@@ -527,21 +798,34 @@
 # without asking (in a push way), but just after a request, so only
 # asynchronous clients may create a scenario where data is requested faster
 # than it can read.
 #
 # Instead there is a default limit for pubsub and slave clients, since
 # subscribers and slaves receive data in a push fashion.
 #
-# Both the hard or the soft limit can be disabled just setting it to zero.
+# Both the hard or the soft limit can be disabled by setting them to zero.
 client-output-buffer-limit normal 0 0 0
 client-output-buffer-limit slave 256mb 64mb 60
 client-output-buffer-limit pubsub 32mb 8mb 60
 
-################################## INCLUDES ###################################
-
-# Include one or more other config files here.  This is useful if you
-# have a standard template that goes to all Redis server but also need
-# to customize a few per-server settings.  Include files can include
-# other files, so use this wisely.
-#
-# include /path/to/local.conf
-# include /path/to/other.conf
+# Redis calls an internal function to perform many background tasks, like
+# closing connections of clients in timeout, purging expired keys that are
+# never requested, and so forth.
+#
+# Not all tasks are performed with the same frequency, but Redis checks for
+# tasks to perform according to the specified "hz" value.
+#
+# By default "hz" is set to 10. Raising the value will use more CPU when
+# Redis is idle, but at the same time will make Redis more responsive when
+# there are many keys expiring at the same time, and timeouts may be
+# handled with more precision.
+#
+# The range is between 1 and 500, however a value over 100 is usually not
+# a good idea. Most users should use the default of 10 and raise this up to
+# 100 only in environments where very low latency is required.
+hz 10
+
+# When a child rewrites the AOF file, if the following option is enabled
+# the file will be fsync-ed every 32 MB of data generated. This is useful
+# in order to commit the file to the disk more incrementally and avoid
+# big latency spikes.
+aof-rewrite-incremental-fsync yes
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/memcached/template/openssl.cnf.ca.in` & `slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/template/openssl.cnf.ca.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/memcached/certificate_authority.py` & `slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/certificate_authority.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import subprocess
 import time
 import ConfigParser
+import uuid
 
 
 def popenCommunicate(command_list, input=None):
   subprocess_kw = dict(stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
   if input is not None:
     subprocess_kw.update(stdin=subprocess.PIPE)
   popen = subprocess.Popen(command_list, **subprocess_kw)
@@ -40,15 +41,15 @@
       if os.path.exists(f):
         os.unlink(f)
     try:
       # no CA, let us create new one
       popenCommunicate([self.openssl_binary, 'req', '-nodes', '-config',
           self.openssl_configuration, '-new', '-x509', '-extensions',
           'v3_ca', '-keyout', self.key, '-out', self.certificate,
-          '-days', '10950'], 'Automatic Certificate Authority\n')
+          '-days', '10950'], 'Certificate Authority %s\n' % uuid.uuid1())
     except:
       try:
         for f in file_list:
           if os.path.exists(f):
             os.unlink(f)
       except:
         # do not raise during cleanup
@@ -97,16 +98,19 @@
       parser = ConfigParser.RawConfigParser()
       parser.readfp(open(os.path.join(self.request_dir, request_file), 'r'))
       if self._checkCertificate(parser.get('certificate', 'name'),
           parser.get('certificate', 'key_file'), parser.get('certificate',
             'certificate_file')):
         print 'Created certificate %r' % parser.get('certificate', 'name')
 
-def runCertificateAuthority(args):
-  ca_conf = args[0]
-  ca = CertificateAuthority(ca_conf['key'], ca_conf['certificate'],
-      ca_conf['openssl_binary'], ca_conf['openssl_configuration'],
-      ca_conf['request_dir'])
+def runCertificateAuthority(*args):
+  ca = CertificateAuthority(*args)
   while True:
     ca.checkAuthority()
     ca.checkRequestDir()
+    # XXX
+    # Antoine: I really don't like that at all. It wastes useful CPU time.
+    #          I think it would be a greater idea to use pyinotify
+    #          <http://pyinotify.sourceforge.net/>
+    #          Or we could use select() with socket as well.
     time.sleep(60)
+    # end XXX
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/sheepdogtestbed/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/sheepdogtestbed/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/softwaretype.py` & `slapos.cookbook-1.0.92/slapos/recipe/softwaretype.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,17 +31,66 @@
 from ConfigParser import ConfigParser
 import json
 import subprocess
 import slapos.slap
 import netaddr
 import logging
 import errno
+import re
 
 import zc.buildout
 
+class SlapConfigParser(ConfigParser, object):
+  """ 
+      This class overrite ConfigParser.write method to fix parse problem when
+      configuration like: 
+      foo += bar is included in buildout file. softwaretype recipe will generate
+      buildout file with foo + = bar because ConfigParser doesn't reconize += 
+      delimiter and read key as "foo +", value as "bar".
+      Then ConfigParser.write method generate
+      
+      [section]
+      foo + = bar
+      ...
+      
+      This is invalid with buildout version 2.
+  """
+
+  def write(self, fp):
+    """Write an .ini-format representation of the configuration state."""
+    if sys.version_info[0] > 2:
+      return super(SlapConfigParser, self).write(fp)
+
+    regex = re.compile(r'^(.*)\s+([+-]{1})$')
+    if self._defaults:
+      fp.write("[%s]\n" % DEFAULTSECT)
+      for (key, value) in self._defaults.items():
+        op = ""
+        result = regex.match(key)
+        if result is not None:
+          key, op = result.groups()
+
+        line = "%s %s= %s\n" % (key, op, str(value).replace('\n', '\n\t'))
+        fp.write(line)
+      fp.write("\n")
+    for section in self._sections:
+      fp.write("[%s]\n" % section)
+      for (key, value) in self._sections[section].items():
+        if key == "__name__":
+          continue
+        if (value is not None) or (self._optcre == self.OPTCRE):
+          op = ""
+          result = regex.match(key)
+          if result is not None:
+            key, op = result.groups()
+          key = "%s %s= %s" % (key, op, str(value).replace('\n', '\n\t'))
+
+        fp.write("%s\n" % key)
+      fp.write("\n")
+
 class Recipe:
 
   def __init__(self, buildout, name, options):
     self.buildout = buildout
     self.options = options
     self.name = name
     self.logger = logging.getLogger(self.name)
@@ -140,15 +189,15 @@
 
     instance_file_path = self.options[software_type]
 
     if not os.path.exists(instance_file_path):
       raise zc.buildout.UserError("The specified buildout config file %r does "
                                   "not exist." % instance_file_path)
 
-    buildout = ConfigParser()
+    buildout = SlapConfigParser()
     with open(instance_file_path) as instance_path:
       buildout.readfp(instance_path)
 
     buildout.set('buildout', 'installed', '.installed-%s.cfg' % self.name)
 
     if not buildout.has_section('slap-parameter'):
       buildout.add_section('slap-parameter')
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/symbolic_link.py` & `slapos.cookbook-1.0.92/slapos/recipe/symbolic_link.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/duplicity.py` & `slapos.cookbook-1.0.92/slapos/recipe/duplicity.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,11 +42,8 @@
       cmd.extend(options)
       cmd.extend([remote_url, backup_directory])
     else:
       # duplicity [options] local remote
       cmd.extend(options)
       cmd.extend([backup_directory, remote_url])
 
-    wrapper = self.createPythonScript(self.options['wrapper'],
-      'slapos.recipe.librecipe.execute.execute', cmd)
-
-    return [wrapper]
+    return self.createWrapper(self.options['wrapper'], cmd)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5_update/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/generic_kumofs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,55 +20,56 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-import urlparse
-from slapos.recipe.librecipe import GenericSlapRecipe
+import os
+from slapos.recipe.librecipe import GenericBaseRecipe
 
-class Recipe(GenericSlapRecipe):
-  def _install(self):
-    self.logger.warn('DEPRECATED: Please update your configuration to use erp5.promise and erp5.bootstrap instead.')
-    conversion_server = None
-    if 'cloudooo-url' in self.options and self.options['cloudooo-url']:
-      parsed = urlparse.urlparse(self.options['cloudooo-url'])
-      conversion_server = "%s:%s" % (parsed.hostname, parsed.port)
-    memcached = None
-    if 'memcached-url' in self.options and self.options['memcached-url']:
-      parsed = urlparse.urlparse(self.options['memcached-url'])
-      memcached = "%s:%s" % (parsed.hostname, parsed.port)
-    kumofs = None
-    if 'kumofs-url' in self.options and self.options['kumofs-url']:
-      parsed = urlparse.urlparse(self.options['kumofs-url'])
-      kumofs = "%s:%s" % (parsed.hostname, parsed.port)
-
-    parsed = urlparse.urlparse(self.options['mysql-url'])
-    mysql_connection_string = "%(database)s@%(hostname)s:%(port)s "\
-        "%(username)s %(password)s" % dict(
-      database=parsed.path.split('/')[1],
-      hostname=parsed.hostname,
-      port=parsed.port,
-      username=parsed.username,
-      password=parsed.password
+class Recipe(GenericBaseRecipe):
+  def install(self):
+    ip = self.options['ip']
+    kumo_manager_port = int(self.options['manager-port'])
+    kumo_server_port = int(self.options['server-port'])
+    kumo_server_listen_port = int(self.options['server-listen-port'])
+    kumo_gateway_port = int(self.options['gateway-port'])
+    path_list = []
+    if 'data-path' in self.options:
+      kumo_server_storage = self.options.get('data-path')
+    else:
+      kumo_server_storage = os.path.join(self.options['data-directory'], "kumodb.tch")
+    # XXX: kumo is not storing pid in file, unless it is not running as daemon
+    #      but running daemons is incompatible with SlapOS, so there is currently
+    #      no way to have Kumo's pid files to rotate logs and send signals to them
+    config = dict(
+      kumo_gateway_binary=self.options['kumo-gateway-binary'],
+      kumo_gateway_ip=ip,
+      kumo_gateway_log=self.options['kumo-gateway-log'],
+      kumo_manager_binary=self.options['kumo-manager-binary'],
+      kumo_manager_ip=ip,
+      kumo_manager_log=self.options['kumo-manager-log'],
+      kumo_server_binary=self.options['kumo-server-binary'],
+      kumo_server_ip=ip,
+      kumo_server_log=self.options['kumo-server-log'],
+      kumo_server_storage=kumo_server_storage,
+      kumo_manager_port=kumo_manager_port,
+      kumo_server_port=kumo_server_port,
+      kumo_server_listen_port=kumo_server_listen_port,
+      kumo_gateway_port=kumo_gateway_port,
+      shell_path=self.options['shell-path'],
     )
 
-    parsed = urlparse.urlparse(self.options['url'])
-    zope_user = parsed.username
-    zope_password = parsed.password
-    zope_host = '%s:%s' % (parsed.hostname, parsed.port)
-    bt5_list = []
-    if len(self.parameter_dict.get("bt5_list", "").strip()):
-      bt5_list = self.parameter_dict["bt5_list"].split()
-    elif self.parameter_dict.get("flavour", "default") == 'configurator':
-      bt5_list = self.options['configurator-bt5-list'].split()
-    bt5_repository_list = self.parameter_dict.get("bt5_repository_list",
-      "").split() or self.options['bt5-repository-list'].split()
+    path_list.append(self.createExecutable(self.options['gateway-wrapper'],
+      self.substituteTemplate(self.getTemplateFilename('kumo_gateway.in'),
+        config)))
+
+    path_list.append(self.createExecutable(self.options['manager-wrapper'],
+      self.substituteTemplate(self.getTemplateFilename('kumo_manager.in'),
+        config)))
+
+    path_list.append(self.createExecutable(self.options['server-wrapper'],
+      self.substituteTemplate(self.getTemplateFilename('kumo_server.in'),
+        config)))
 
-    script = self.createPythonScript(self.options['update-wrapper'],
-      __name__+'.erp5.updateERP5', [
-        self.options['site-id'], mysql_connection_string,
-        [zope_user, zope_password, zope_host],
-        memcached, conversion_server, kumofs, bt5_list, bt5_repository_list,
-        self.options['cadir-path'], self.options['openssl-binary']])
-    return [script]
+    return path_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/jsondump.py` & `slapos.cookbook-1.0.92/slapos/recipe/jsondump.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/haproxy/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/haproxy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,16 +116,15 @@
       self.options['conf-path'],
       self.substituteTemplate(
         self.getTemplateFilename('haproxy.cfg.in'),
         {'socket_path': self.options['socket-path'],
          'server_text': server_snippet},
       )
     )
-    wrapper_path = self.createPythonScript(
+    wrapper_path = self.createWrapper(
       self.options['wrapper-path'],
-      'slapos.recipe.librecipe.execute.execute',
-      arguments=[self.options['binary-path'].strip(), '-f', configuration_path],)
+      (self.options['binary-path'].strip(), '-f', configuration_path))
     ctl_path = self.createPythonScript(
       self.options['ctl-path'],
-      '%s.haproxy.haproxyctl' % __name__,
-      {'socket_path':self.options['socket-path']})
+      __name__ + '.haproxy.haproxyctl',
+      (self.options['socket-path'],))
     return [configuration_path, wrapper_path, ctl_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/haproxy/template/haproxy.cfg.in` & `slapos.cookbook-1.0.92/slapos/recipe/haproxy/template/haproxy.cfg.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -76,15 +76,15 @@
       })
     )
     path_list.append(mysql_conf_file)
 
     mysql_script_list = []
 
     # user defined functions
-    udf_registration = ""
+    udf_registration = "DROP FUNCTION IF EXISTS last_insert_grn_id;\nDROP FUNCTION IF EXISTS mroonga_snippet;\nDROP FUNCTION IF EXISTS mroonga_command;\n"
     mroonga = self.options.get('mroonga', 'ha_mroonga.so')
     if mroonga:
       udf_registration += "CREATE FUNCTION last_insert_grn_id RETURNS " \
         "INTEGER SONAME '" + mroonga + "';\n"
       udf_registration += "CREATE FUNCTION mroonga_snippet RETURNS " \
         "STRING SONAME '" + mroonga + "';\n"
       udf_registration += "CREATE FUNCTION mroonga_command RETURNS " \
@@ -150,28 +150,32 @@
         data_directory=self.options['data-directory'],
         mysql_binary=mysql_binary,
         socket=socket,
         configuration_file=mysql_conf_file,
        )]
     )
     path_list.append(mysqld)
-    environment = dict(PATH='%s' % self.options['bin-directory'])
+    environment = {'PATH': self.options['bin-directory']}
     # TODO: move to a separate recipe (ack'ed by Cedric)
     if 'backup-script' in self.options:
       # backup configuration
       full_backup = self.options['full-backup-directory']
       incremental_backup = self.options['incremental-backup-directory']
       innobackupex_argument_list = [self.options['perl-binary'],
           self.options['innobackupex-binary'],
           '--defaults-file=%s' % mysql_conf_file,
           '--socket=%s' % socket.strip(), '--user=root',
           '--ibbackup=%s'% self.options['xtrabackup-binary']]
-      innobackupex_incremental = self.createPythonScript(self.options['innobackupex-incremental'], 'slapos.recipe.librecipe.execute.executee', [innobackupex_argument_list + ['--incremental'], environment])
+      innobackupex_incremental = self.createWrapper(
+        self.options['innobackupex-incremental'],
+        innobackupex_argument_list + ['--incremental'], environment)
       path_list.append(innobackupex_incremental)
-      innobackupex_full = self.createPythonScript(self.options['innobackupex-full'], 'slapos.recipe.librecipe.execute.executee', [innobackupex_argument_list, environment])
+      innobackupex_full = self.createWrapper(
+        self.options['innobackupex-full'],
+        innobackupex_argument_list, environment)
       path_list.append(innobackupex_full)
       backup_controller = self.createPythonScript(self.options['backup-script'], __name__ + '.innobackupex.controller', [innobackupex_incremental, innobackupex_full, full_backup, incremental_backup])
       path_list.append(backup_controller)
     # TODO: move to a separate recipe (ack'ed by Cedric)
     # percona toolkit (formerly known as maatkit) installation
     for pt_script_name in (
         'pt-align',
@@ -211,15 +215,17 @@
       if option_name not in self.options:
         continue
       pt_argument_list = [self.options['perl-binary'],
           self.options[option_name],
           '--defaults-file=%s' % mysql_conf_file,
           '--socket=%s' % socket.strip(), '--user=root',
           ]
-      pt_exe = self.createPythonScript(os.path.join(self.options['bin-directory'], pt_script_name), 'slapos.recipe.librecipe.execute.executee', [pt_argument_list, environment])
+      pt_exe = self.createWrapper(
+        os.path.join(self.options['bin-directory'], pt_script_name),
+        pt_argument_list, environment)
       path_list.append(pt_exe)
 
     return path_list
 
 class WrapUpdateMySQL(GenericBaseRecipe):
   def install(self):
     return [
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/innobackupex.py` & `slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/innobackupex.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import glob
-def controller(args):
+def controller(innobackupex_incremental, innobackupex_full,
+               full_backup, incremental_backup):
   """Creates full or incremental backup
 
   If no full backup is done, it is created
 
   If full backup exists incremental backup is done starting with base
 
   base is the newest (according to date) full or incremental backup
   """
-  innobackupex_incremental, innobackupex_full, full_backup, incremental_backup \
-      = args
   if len(os.listdir(full_backup)) == 0:
     print 'Doing full backup in %r' % full_backup
     os.execv(innobackupex_full, [innobackupex_full, full_backup])
   else:
     backup_list = filter(os.path.isdir, glob.glob(full_backup + "/*") +
       glob.glob(incremental_backup + "/*"))
     backup_list.sort(key=lambda x: os.path.getmtime(x), reverse=True)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_mysql/mysql.py` & `slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import subprocess
 import time
 import sys
 import pytz
 
 
-def runMysql(args):
+def runMysql(conf):
   sleep = 60
-  conf = args[0]
   mysqld_wrapper_list = [conf['mysqld_binary'], '--defaults-file=%s' %
       conf['configuration_file']]
   # we trust mysql_install that if mysql directory is available mysql was
   # correctly initalised
   if not os.path.isdir(os.path.join(conf['data_directory'], 'mysql')):
     while True:
       # XXX: Protect with proper root password
@@ -50,71 +49,74 @@
     pass
   except ValueError:
     # 'ValueError: not allowed to raise maximum limit'
     pass
   os.execl(mysqld_wrapper_list[0], *mysqld_wrapper_list)
 
 
-def updateMysql(args):
-  conf = args[0]
+def updateMysql(conf):
   sleep = 30
   is_succeed = False
   try:
     script_filename = conf.pop('mysql_script_file')
   except KeyError:
     pass
   else:
     assert 'mysql_script' not in conf
     with open(script_filename) as script_file:
       conf['mysql_script'] = script_file.read()
+  is_succeeded = False
   while True:
-    mysql_upgrade_list = [conf['mysql_upgrade_binary'], '--user=root']
-    if 'socket' in conf:
-      mysql_upgrade_list.append('--socket=' + conf['socket'])
-    mysql_upgrade = subprocess.Popen(mysql_upgrade_list, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-    result = mysql_upgrade.communicate()[0]
-    if mysql_upgrade.returncode is None:
-      mysql_upgrade.kill()
-    if mysql_upgrade.returncode != 0 and not 'is already upgraded' in result:
-      print "Command %r failed with result:\n%s" % (mysql_upgrade_list, result)
-    else:
+    while True:
+      mysql_upgrade_list = [conf['mysql_upgrade_binary'], '--user=root']
+      if 'socket' in conf:
+        mysql_upgrade_list.append('--socket=' + conf['socket'])
+      mysql_upgrade = subprocess.Popen(mysql_upgrade_list, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+      result = mysql_upgrade.communicate()[0]
+      if mysql_upgrade.returncode is None:
+        mysql_upgrade.kill()
       if mysql_upgrade.returncode == 0:
         print "MySQL database upgraded with result:\n%s" % result
-      else:
+      elif 'is already upgraded' in result:
         print "No need to upgrade MySQL database"
+      else:
+        print "Command %r failed with result:\n%s" % (mysql_upgrade_list, result)
+        break
       mysql_list = [conf['mysql_binary'].strip(), '-B', '--user=root']
       if 'socket' in conf:
         mysql_list.append('--socket=' + conf['socket'])
       mysql = subprocess.Popen(mysql_list, stdin=subprocess.PIPE,
           stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
       result = mysql.communicate(conf['mysql_script'])[0]
       if mysql.returncode is None:
         mysql.kill()
       if mysql.returncode != 0:
         print 'Command %r failed with:\n%s' % (mysql_list, result)
-      else:
-        # import timezone database
-        mysql_tzinfo_to_sql_binary = os.path.join(
-          os.path.dirname(conf['mysql_binary'].strip()), 'mysql_tzinfo_to_sql')
-        zoneinfo_directory = '%s/zoneinfo' % os.path.dirname(pytz.__file__)
-        mysql_tzinfo_to_sql_list = [mysql_tzinfo_to_sql_binary, zoneinfo_directory]
-        mysql_tzinfo_to_sql = subprocess.Popen(mysql_tzinfo_to_sql_list, stdin=subprocess.PIPE,
-                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        timezone_sql = mysql_tzinfo_to_sql.communicate()[0]
-        if mysql.returncode != 0:
-          print 'Command %r failed with:\n%s' % (mysql_tzinfo_to_sql_list, result)
-        else:
-          mysql = subprocess.Popen(mysql_list + ['mysql',], stdin=subprocess.PIPE,
-                                   stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-          result = mysql.communicate(timezone_sql)[0]
-          if mysql.returncode is None:
-            mysql.kill()
-          if mysql.returncode != 0:
-            print 'Command %r failed with:\n%s' % (mysql_list, result)
-          is_succeed = True
-    if is_succeed:
+        break
+      # import timezone database
+      mysql_tzinfo_to_sql_binary = os.path.join(
+        os.path.dirname(conf['mysql_binary'].strip()), 'mysql_tzinfo_to_sql')
+      zoneinfo_directory = '%s/zoneinfo' % os.path.dirname(pytz.__file__)
+      mysql_tzinfo_to_sql_list = [mysql_tzinfo_to_sql_binary, zoneinfo_directory]
+      mysql_tzinfo_to_sql = subprocess.Popen(mysql_tzinfo_to_sql_list, stdin=subprocess.PIPE,
+                               stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+      timezone_sql = mysql_tzinfo_to_sql.communicate()[0]
+      if mysql_tzinfo_to_sql.returncode != 0:
+        print 'Command %r failed with:\n%s' % (mysql_tzinfo_to_sql_list, result)
+        break
+      mysql = subprocess.Popen(mysql_list + ['mysql',], stdin=subprocess.PIPE,
+                               stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+      result = mysql.communicate(timezone_sql)[0]
+      if mysql.returncode is None:
+        mysql.kill()
+      if mysql.returncode != 0:
+        print 'Command %r failed with:\n%s' % (mysql_list, result)
+        break
+      is_succeeded = True
+      break
+    if is_succeeded:
       print 'SlapOS initialisation script succesfully applied on database.'
       break
     print 'Sleeping for %ss and retrying' % sleep
     sys.stdout.flush()
     sys.stderr.flush()
     time.sleep(sleep)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/mkdirectory.py` & `slapos.cookbook-1.0.92/slapos/recipe/equeue.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,23 +20,30 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-import os
-
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
 
-  def _options(self, options):
-    self.directory = options.copy()
-    del self.directory['recipe']
-    self.mode = int(self.directory.pop('mode', '700'), 8)
-
   def install(self):
-    for path in sorted(self.directory.itervalues()):
-      if path and not os.path.isdir(path):
-        os.makedirs(path, self.mode)
-    return []
+
+    args = [
+      self.options['equeue-binary'],
+      '--database', self.options['database'],
+      '--logfile', self.options['log'],
+      '--lockfile', self.options['lockfile']
+    ]
+
+    if 'takeover-triggered-file-path' in self.options:
+      args += ('--takeover-triggered-file-path',
+               self.options['takeover-triggered-file-path'])
+
+    if 'loglevel' in self.options:
+      args += '--loglevel', self.options['loglevel']
+
+    args.append(self.options['socket'])
+
+    return self.createWrapper(self.options['wrapper'], args)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/pbs.py` & `slapos.cookbook-1.0.92/slapos/recipe/pbs.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,59 +35,53 @@
 from slapos.recipe.librecipe import GenericSlapRecipe
 from slapos.recipe.dropbear import KnownHostsFile
 from slapos.recipe.notifier import Notify
 from slapos.recipe.notifier import Callback
 from slapos.recipe.librecipe import shlex
 
 
-def promise(args):
-  ssh = subprocess.Popen(
-      [args['ssh_client'], '%(user)s@%(host)s/%(port)s' % args],
-      stdin=subprocess.PIPE, stdout=None, stderr=None
-  )
-
-  # Rdiff Backup protocol quit command
-  quitcommand = 'q' + chr(255) + chr(0) * 7
-
-  ssh.stdin.write(quitcommand)
-  ssh.stdin.flush()
-  ssh.stdin.close()
-  ssh.wait()
-
-  if ssh.poll() is None:
-    return 1
-  if ssh.returncode != 0:
+def promise(ssh_client, user, host, port):
+  # Redirect output to /dev/null
+  with open(os.devnull) as _dev_null:
+    ssh = subprocess.Popen(
+        (ssh_client, '%s@%s' % (user, host), '-p', str(port)),
+        stdin=subprocess.PIPE, stdout=_dev_null)
+  ssh.communicate('q' + chr(255) + chr(0) * 7)
+  if ssh.returncode:
     sys.stderr.write("SSH Connection failed\n")
   return ssh.returncode
 
 
-
 class Recipe(GenericSlapRecipe, Notify, Callback):
+  def _options(self, options):
+    options['rdiff-backup-data-folder'] = ""
+    if 'slave-instance-list' in options:
+      for slave in json.loads(options['slave-instance-list']):
+        if slave['type'] == 'pull':
+          options['rdiff-backup-data-folder'] = str(os.path.join(options['directory'], slave['name'], 'rdiff-backup-data'))
 
   def wrapper_push(self, remote_schema, local_dir, remote_dir, rdiff_wrapper_path):
     # Create a simple rdiff-backup wrapper that will push
 
     template = textwrap.dedent("""\
         #!/bin/sh
         #
         # Push data to a PBS *-import instance.
         #
 
         LC_ALL=C
         export LC_ALL
         RDIFF_BACKUP=%(rdiffbackup_binary)s
-        until $RDIFF_BACKUP \\
+        $RDIFF_BACKUP \\
                 --remote-schema %(remote_schema)s \\
                 --restore-as-of now \\
+                --ignore-numerical-ids \\
                 --force \\
                 %(local_dir)s \\
-                %(remote_dir)s; do
-          echo "repeating rdiff-backup..."
-          sleep 10
-        done
+                %(remote_dir)s
         """)
 
     template_dict = {
       'rdiffbackup_binary': shlex.quote(self.options['rdiffbackup-binary']),
       'remote_schema': shlex.quote(remote_schema),
       'remote_dir': shlex.quote(remote_dir),
       'local_dir': shlex.quote(local_dir)
@@ -111,103 +105,89 @@
         #
 
         sigint()
         {
           exit 1
         }
 
-        trap sigint SIGINT  # we can CTRL-C for ease of debugging
+        trap sigint INT  # we can CTRL-C for ease of debugging
 
         LC_ALL=C
         export LC_ALL
         is_first_backup=$(test -d %(rdiff_backup_data)s || echo yes)
         RDIFF_BACKUP=%(rdiffbackup_binary)s
 
         TMPDIR=%(tmpdir)s
         BACKUP_DIR=%(local_dir)s
         CORRUPTED_MSG="^Warning:\ Computed\ SHA1\ digest\ of\ "
         CANTFIND_MSG="^Warning:\ Cannot\ find\ SHA1\ digest\ for\ file\ "
         CORRUPTED_FILE=$TMPDIR/$$.rdiff_corrupted
         CANTFIND_FILE=$TMPDIR/$$.rdiff_cantfind
 
         SUCCEEDED=false
-        while ! $SUCCEEDED; do
 
-            # not using --fix-corrupted can lead to an infinite loop
-            # in case of manual changes to the backup repository.
+        # not using --fix-corrupted can lead to an infinite loop
+        # in case of manual changes to the backup repository.
 
-            CORRUPTED_ARGS=""
-            if [ "$1" = "--fix-corrupted" ]; then
-                VERIFY=$($RDIFF_BACKUP --verify $BACKUP_DIR 2>&1 >/dev/null)
-                echo "$VERIFY" | egrep "$CORRUPTED_MSG" | sed "s/$CORRUPTED_MSG//g" > $CORRUPTED_FILE
+        CORRUPTED_ARGS=""
+        if [ "$1" = "--fix-corrupted" ]; then
+            VERIFY=$($RDIFF_BACKUP --verify $BACKUP_DIR 2>&1 >/dev/null)
+            echo "$VERIFY" | egrep "$CORRUPTED_MSG" | sed "s/$CORRUPTED_MSG//g" > $CORRUPTED_FILE
 
-                # Sometimes --verify reports this spurious warning:
-                echo "$VERIFY" | egrep "$CANTFIND_MSG" | sed "s/$CANTFIND_MSG\(.*\),/--always-snapshot\ '\\1'/g" > $CANTFIND_FILE
+            # Sometimes --verify reports this spurious warning:
+            echo "$VERIFY" | egrep "$CANTFIND_MSG" | sed "s/$CANTFIND_MSG\(.*\),/--always-snapshot\ '\\1'/g" > $CANTFIND_FILE
 
-                # There can be too many files, better not to provide them through separate command line parameters
-                CORRUPTED_ARGS="--always-snapshot-fromfile $CORRUPTED_FILE --always-snapshot-fromfile $CANTFIND_FILE"
+            # There can be too many files, better not to provide them through separate command line parameters
+            CORRUPTED_ARGS="--always-snapshot-fromfile $CORRUPTED_FILE --always-snapshot-fromfile $CANTFIND_FILE"
 
-                if [ -s "$CORRUPTED_FILE" -o -s "$CANTFIND_FILE" ]; then
-                    echo Retransmitting $(cat "$CORRUPTED_FILE" "$CANTFIND_FILE" | wc -l) corrupted/missing files
-                else
-                    echo "No corrupted or missing files to retransmit"
-                fi
+            if [ -s "$CORRUPTED_FILE" -o -s "$CANTFIND_FILE" ]; then
+                echo Retransmitting $(cat "$CORRUPTED_FILE" "$CANTFIND_FILE" | wc -l) corrupted/missing files
+            else
+                echo "No corrupted or missing files to retransmit"
             fi
+        fi
+
+        $RDIFF_BACKUP \\
+                $CORRUPTED_ARGS \\
+                --remote-schema %(remote_schema)s \\
+                %(remote_dir)s \\
+                $BACKUP_DIR
 
-            $RDIFF_BACKUP \\
-                    $CORRUPTED_ARGS \\
-                    --remote-schema %(remote_schema)s \\
-                    %(remote_dir)s \\
-                    $BACKUP_DIR
+        RDIFF_BACKUP_STATUS=$?
 
-            [ "$CORRUPTED_ARGS" ] && rm -f "$CORRUPTED_FILE" "$CANTFIND_FILE"
+        [ "$CORRUPTED_ARGS" ] && rm -f "$CORRUPTED_FILE" "$CANTFIND_FILE"
 
+        if [ ! $RDIFF_BACKUP_STATUS -eq 0 ]; then
+            # Check the backup, go to the last consistent backup, so that next
+            # run will be okay.
+            echo "Checking backup directory..."
+            $RDIFF_BACKUP --check-destination-dir $BACKUP_DIR
             if [ ! $? -eq 0 ]; then
-                # Check the backup, go to the last consistent backup, so that next
-                # run will be okay.
-                echo "Checking backup directory..."
-                $RDIFF_BACKUP --check-destination-dir $BACKUP_DIR
-                if [ ! $? -eq 0 ]; then
-                    # Here, two possiblities:
-                    if [ is_first_backup ]; then
-                        continue
-                        # The first backup failed, and check-destination as well.
-                        # we may want to remove the backup.
-                    else
-                        continue
-                        # The backup command has failed, while transferring an increment, and check-destination as well.
-                        # XXX We may need to publish the failure and ask the the equeue, re-run this script again,
-                        # instead do a push to the clone.
-                    fi
+                # Here, two possiblities:
+                if [ is_first_backup ]; then
+                    continue
+                    # The first backup failed, and check-destination as well.
+                    # we may want to remove the backup.
+                else
+                    continue
+                    # The backup command has failed, while transferring an increment, and check-destination as well.
+                    # XXX We may need to publish the failure and ask the the equeue, re-run this script again,
+                    # instead do a push to the clone.
                 fi
-            else
-                # Everything's okay, cleaning up...
-                $RDIFF_BACKUP --remove-older-than %(remove_backup_older_than)s --force $BACKUP_DIR
-            fi
-
-            SUCCEEDED=true
-
-            if [ -e %(backup_signature)s ]; then
-              cd $BACKUP_DIR
-              find -type f ! -name backup.signature ! -wholename "./rdiff-backup-data/*" -print0 | xargs -P4 -0 sha256sum  | LC_ALL=C sort -k 66 > ../proof.signature
-              cmp backup.signature ../proof.signature || SUCCEEDED=false
-              diff -ruw backup.signature ../proof.signature > ../backup.diff
-              # XXX If there is a difference on the backup, we should publish the
-              # failure and ask the equeue, re-run this script again,
-              # instead do a push it to the clone.
             fi
+        else
+            # Everything's okay, cleaning up...
+            $RDIFF_BACKUP --remove-older-than %(remove_backup_older_than)s --force $BACKUP_DIR
+        fi
 
-            $SUCCEEDED || find $BACKUP_DIR -name rdiff-backup.tmp.* -exec rm -rf {} \;
-        done
         """)
 
     template_dict = {
       'rdiffbackup_binary': shlex.quote(self.options['rdiffbackup-binary']),
       'rdiff_backup_data': shlex.quote(os.path.join(local_dir, 'rdiff-backup-data')),
-      'backup_signature': shlex.quote(os.path.join(local_dir, 'backup.signature')),
       'remote_schema': shlex.quote(remote_schema),
       'remote_dir': shlex.quote(remote_dir),
       'local_dir': shlex.quote(local_dir),
       'tmpdir': '/tmp',
       'remove_backup_older_than': shlex.quote(remove_backup_older_than)
     }
 
@@ -219,49 +199,52 @@
 
 
   def add_slave(self, entry, known_hosts_file):
     path_list = []
 
     url = entry.get('url')
     if not url:
-      raise ValueError('Missing URL parameter for PBS recipe')
+      return path_list
+      # It used to raise an error if url was not defined.
+      # This behavior has been removed to accelerate deployment of the
+      # Software Release. The buildout, instead of failing, can process
+      # other sections, which will return parameters to the main instance faster
     parsed_url = urlparse.urlparse(url)
 
     slave_type = entry['type']
     if not slave_type in ['pull', 'push']:
       raise ValueError('type parameter must be either pull or push.')
 
     slave_id = entry['notification-id']
 
     print 'Processing PBS slave %s with type %s' % (slave_id, slave_type)
 
-    promise_path = os.path.join(self.options['promises-directory'], slave_id)
-    promise_dict = dict(ssh_client=self.options['sshclient-binary'],
-                        user=parsed_url.username,
-                        host=parsed_url.hostname,
-                        port=parsed_url.port)
-    promise = self.createPythonScript(promise_path,
-                                      __name__ + '.promise',
-                                      promise_dict)
-    path_list.append(promise)
+    path_list.append(self.createPythonScript(
+      os.path.join(self.options['promises-directory'], "ssh-to-%s" % slave_id),
+      __name__ + '.promise',
+      (self.options['sshclient-binary'],
+       parsed_url.username, parsed_url.hostname, parsed_url.port)))
 
     # Create known_hosts file by default.
     # In some case, we don't want to create it (case where we share IP mong partitions)
     if not self.isTrueValue(self.options.get('ignore-known-hosts-file')):
-      known_hosts_file[parsed_url.hostname] = entry['server-key']
+      # Migration code: if known_hosts file contains entry with just IP, then it
+      # is updated to use [IP]:port. It allows to share same IP among partitions
+      if parsed_url.hostname in known_hosts_file:
+        del known_hosts_file[parsed_url.hostname]
+      known_hostname = "[%s]:%s" % (parsed_url.hostname, parsed_url.port)
+      known_hosts_file[known_hostname] = entry['server-key'].strip()
 
     notifier_wrapper_path = os.path.join(self.options['wrappers-directory'], slave_id)
     rdiff_wrapper_path = notifier_wrapper_path + '_raw'
 
     # Create the rdiff-backup wrapper
     # It is useful to separate it from the notifier so that we can run it manually.
 
-    # XXX use -y because the host might not yet be in the
-    #     trusted hosts file until the next time slapgrid is run.
-    remote_schema = '{ssh} -y -K 300 -p %s {username}@{hostname}'.format(
+    remote_schema = '{ssh} -o "ConnectTimeout 300" -p %s {username}@{hostname}'.format(
               ssh=self.options['sshclient-binary'],
               username=parsed_url.username,
               hostname=parsed_url.hostname
             )
     remote_dir = '{port}::{path}'.format(port=parsed_url.port, path=parsed_url.path)
     local_dir = self.createDirectory(self.options['directory'], entry['name'])
 
@@ -283,17 +266,21 @@
     # Create notifier wrapper
     notifier_wrapper = self.createNotifier(
         notifier_binary=self.options['notifier-binary'],
         wrapper=notifier_wrapper_path,
         executable=rdiff_wrapper,
         log=os.path.join(self.options['feeds'], entry['notification-id']),
         title=entry.get('title', slave_id),
-        notification_url=entry['notify'],
+        notification_url=entry['notify'] or '',
         feed_url='%s/get/%s' % (self.options['notifier-url'], entry['notification-id']),
-        pidfile=os.path.join(self.options['run-directory'], '%s.pid' % slave_id)
+        max_run=self.options.get('pull-push-maximum-run', 1),
+        pidfile=os.path.join(self.options['run-directory'], '%s.pid' % slave_id),
+        instance_root_name=self.options.get('instance-root-name', None),
+        log_url=self.options.get('log-url', None),
+        status_item_directory=self.options.get('status-item-directory', None)
     )
     path_list.append(notifier_wrapper)
 
     if 'on-notification' in entry:
       path_list.append(self.createCallback(str(entry['on-notification']),
                                            notifier_wrapper))
     else:
@@ -315,16 +302,15 @@
       known_hosts = KnownHostsFile(self.options['known-hosts'])
       with known_hosts:
         for slave in slaves:
           path_list.extend(self.add_slave(slave, known_hosts))
     else:
       self.logger.info("Server mode")
 
-      wrapper = self.createWrapper(name=self.options['wrapper'],
-                                   command=self.options['rdiffbackup-binary'],
-                                   parameters=[
+      wrapper = self.createWrapper(self.options['wrapper'],
+                                   (self.options['rdiffbackup-binary'],
                                        '--restrict', self.options['path'],
                                        '--server'
-                                       ])
+                                       ))
       path_list.append(wrapper)
 
     return path_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/nosqltestbed/kumo/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/nosqltestbed/kumo/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/6tunnel/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/check_parameter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# vim: set et sts=2:
 ##############################################################################
 #
-# Copyright (c) 2012 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2015 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -21,38 +22,37 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
+import sys
 
 class Recipe(GenericBaseRecipe):
   """
-  ipv4toipv6 tunnel configuration.
+  Check listening port promise
   """
-  # Override in subclasses
-  template_name = None
 
   def install(self):
-    return [
-      self.createExecutable(
-        self.options['runner-path'],
-        self.substituteTemplate(
-          self.getTemplateFilename(self.template_name),
-          {
-            'ipv6': self.options['ipv6'],
-            'ipv6_port': self.options['ipv6-port'],
-            'ipv4': self.options['ipv4'],
-            'ipv4_port': self.options['ipv4-port'],
-            'shell_path': self.options['shell-path'],
-            '6tunnel_path': self.options['6tunnel-path'],
-          },
-        ),
-      )
-    ]
+    config = dict(
+      value=self.options['value'],
+      python_path=sys.executable,
+    )
 
-class SixToFour(Recipe):
-    template_name = '6to4.in'
+    if self.options.get('expected-type') == "ipv6":
+      template = self.getTemplateFilename('check_ipv6.py.in')
 
-class FourToSix(Recipe):
-    template_name = '4to6.in'
+    elif self.options.get('expected-type') == "ipv4":
+      template = self.getTemplateFilename('check_ipv4.py.in')
+    else:
+      config["expected-value"] = self.options.get('expected-value')
+ 
+      config["expected-not-value"] = self.options.get('expected-not-value')
+
+      template = self.getTemplateFilename('check_parameter.py.in')
+
+    promise = self.createExecutable(
+      self.options['path'],
+      self.substituteTemplate(template, config))
+
+    return [promise]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/condor/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/condor/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,20 +174,19 @@
               self.environ['HOSTNAME'], current_exe)
       wrapper.write(content)
       wrapper.close()
       path_list.append(wrapper_location)
       os.chmod(wrapper_location, 0744)
 
     #generate script for start condor
-    start_condor = os.path.join(self.wrapperdir, 'start_condor')
-    start_bin = os.path.join(self.wrapper_sbin, 'condor_master')
-    condor_reconfig = os.path.join(self.wrapper_sbin, 'condor_reconfig')
-    wrapper = self.createPythonScript(start_condor,
-        '%s.configure.condorStart' % __name__,
-        dict(start_bin=start_bin, condor_reconfig=condor_reconfig)
+    wrapper = self.createPythonScript(
+        os.path.join(self.wrapperdir, 'start_condor'),
+        __name__ + '.configure.condorStart',
+        (os.path.join(self.wrapper_sbin, 'condor_reconfig'),
+         os.path.join(self.wrapper_sbin, 'condor_master'))
     )
     path_list.append(wrapper)
     return path_list
 
 class AppSubmit(GenericBaseRecipe):
   """Submit a condor job into an existing Condor master instance"""
 
@@ -272,17 +271,15 @@
           f.write('to_install')
       for file in app_list[appname]['files']:
         destination = os.path.join(appdir, file)
         if os.path.exists(destination):
           os.unlink(destination)
         os.symlink(app_list[appname]['files'][file], destination)
       #generate wrapper for submitting job
-      condor_submit = os.path.join(self.options['bin'].strip(), 'condor_submit')
-      parameter = dict(submit=condor_submit, sig_install=sig_install,
-                      submit_file='submit',
-                      appname=appname, appdir=appdir)
       submit_job = self.createPythonScript(
         os.path.join(self.options['wrapper-dir'].strip(), appname),
-        '%s.configure.submitJob' % __name__, parameter
+        __name__ + '.configure.submitJob',
+        (os.path.join(self.options['bin'].strip(), 'condor_submit'),
+         'submit', appdir, appname, sig_install)
       )
       path_list.append(submit_job)
     return path_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/condor/configure.py` & `slapos.cookbook-1.0.92/slapos/recipe/condor/configure.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,31 +25,29 @@
 #
 ##############################################################################
 
 import os
 import subprocess
 import time
 
-def submitJob(args):
+def submitJob(submit, submit_file, appdir, appname, sig_install):
   """Run condor_submit (if needed) for job deployment"""
   time.sleep(10)
-  print "Check if needed to submit %s job's" % args['appname']
-  if not os.path.exists(args['sig_install']):
+  print "Check if needed to submit %s job's" % appname
+  if not os.path.exists(sig_install):
     print "Nothing for install or update...Exited"
     return
   # '-a', "log = out.log", '-a', "error = error.log",
-  launch_args = [args['submit'], '-verbose', args['submit_file']]
+  launch_args = submit, '-verbose', submit_file
   process = subprocess.Popen(launch_args, stdout=subprocess.PIPE,
-              stderr=subprocess.STDOUT, cwd=args['appdir'])
+              stderr=subprocess.STDOUT, cwd=appdir)
   result = process.communicate()[0]
   if process.returncode is None or process.returncode != 0:
     print "Failed to execute condor_submit.\nThe error was: %s" % result
   else:
-    os.unlink(args['sig_install'])
+    os.unlink(sig_install)
 
-def condorStart(args):
+def condorStart(condor_reconfig, start_bin):
   """Start Condor if deamons is currently stopped"""
-  result = os.system(args['condor_reconfig'])
-  if result != 0:
+  if subprocess.call(condor_reconfig):
     #process failled to reconfig condor that mean that condor deamons is not curently started
-    os.system(args['start_bin'])
-  
+    subprocess.call(start_bin)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/squid/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/squid/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,25 +74,19 @@
 
     template_filename = self.getTemplateFilename('squid.conf.in')
     configuration_path = self.createFile(
       self.options['conf-path'],
       self.substituteTemplate(template_filename, config))
 
     # Prepare directories
-    prepare_path = self.createPythonScript(
+    prepare_path = self.createWrapper(
       self.options['prepare-path'],
-      'slapos.recipe.librecipe.execute.execute',
-      arguments=[self.options['binary-path'].strip(), 
-                 '-z',
-                 '-f', configuration_path,
-                 ],)
+      (self.options['binary-path'].strip(),
+        '-z', '-f', configuration_path))
 
     # Create running wrapper
-    wrapper_path = self.createPythonScript(
+    wrapper_path = self.createWrapper(
       self.options['wrapper-path'],
-      'slapos.recipe.librecipe.execute.execute',
-      arguments=[self.options['binary-path'].strip(), 
-                 '-N',
-                 '-f', configuration_path,
-                 ],)
+      (self.options['binary-path'].strip(),
+        '-N', '-f', configuration_path))
 
     return [configuration_path, wrapper_path, prepare_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/squid/template/squid.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/squid/template/squid.conf.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/agent/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/apacheproxy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2012 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -19,48 +19,52 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
-#############################################################################
+##############################################################################
+import subprocess
 
-import zc.buildout
 from slapos.recipe.librecipe import GenericBaseRecipe
-import sys
 
 class Recipe(GenericBaseRecipe):
+
   def install(self):
     path_list = []
 
-    configuration_path = self.options["config"]
-    header = """[DEFAULT]
-master_url = %s
-key = %s
-
-cert = %s
-
-max_install_duration = %s
-max_uninstall_duration = %s
-max_request_duration = %s
-max_destroy_duration = %s
-""" % (self.options["master-url"],
-      "\n  ".join(self.options["key"].split("\n")),
-       "\n  ".join(self.options["cert"].split("\n")),
-       self.options["default_max_install_duration"],
-       self.options["default_max_uninstall_duration"],
-       self.options["default_max_request_duration"],
-       self.options["default_max_destroy_duration"])
-
-    with open(configuration_path, "w") as configuration:
-      configuration.write(header + self.options["configuration"])
-
-    path_list.append(self.createPythonScript(
-                       self.options['wrapper'],
-                       'slapos.recipe.librecipe.execute.execute',
-                         [self.options["agent_binary"], '--pidfile=%s' % self.options["pidfile"],
-                          "--log=%s" % self.options["log"], configuration_path]))
-
-    path_list.append(configuration_path)
+    # Install apache
+    apache_config = dict(
+      pid_file=self.options['pid-file'],
+      lock_file=self.options['lock-file'],
+      ip=self.options['ip'],
+      port=self.options['port'],
+      error_log=self.options['error-log'],
+      access_log=self.options['access-log'],
+      backend_url=self.options['url'],
+    )
+    httpd_conf = self.createFile(self.options['httpd-conf'],
+      self.substituteTemplate(self.getTemplateFilename('apache.in'),
+                              apache_config)
+    )
+    path_list.append(httpd_conf)
+
+    wrapper = self.createWrapper(self.options['wrapper'],
+                                 (self.options['httpd-binary'],
+                                     '-f',
+                                     self.options['httpd-conf'],
+                                     '-DFOREGROUND',
+                                     ))
+
+    path_list.append(wrapper)
+
+    subprocess.call([
+                        self.options['httpd-binary'],
+                        '-f',
+                        self.options['httpd-conf'],
+                        '-k',
+                        'graceful',
+                    ])
 
     return path_list
+
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_kumofs/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,56 +20,46 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-import os
 from slapos.recipe.librecipe import GenericBaseRecipe
+import sys
 
 class Recipe(GenericBaseRecipe):
+  """
+  kvm instance configuration.
+  """
   def install(self):
-    ip = self.options['ip']
-    kumo_manager_port = int(self.options['manager-port'])
-    kumo_server_port = int(self.options['server-port'])
-    kumo_server_listen_port = int(self.options['server-listen-port'])
-    kumo_gateway_port = int(self.options['gateway-port'])
-    path_list = []
-    if 'data-path' in self.options:
-      kumo_server_storage = self.options.get('data-path')
-    else:
-      kumo_server_storage = os.path.join(self.options['data-directory'], "kumodb.tch")
-    # XXX: kumo is not storing pid in file, unless it is not running as daemon
-    #      but running daemons is incompatible with SlapOS, so there is currently
-    #      no way to have Kumo's pid files to rotate logs and send signals to them
     config = dict(
-      kumo_gateway_binary=self.options['kumo-gateway-binary'],
-      kumo_gateway_ip=ip,
-      kumo_gateway_log=self.options['kumo-gateway-log'],
-      kumo_manager_binary=self.options['kumo-manager-binary'],
-      kumo_manager_ip=ip,
-      kumo_manager_log=self.options['kumo-manager-log'],
-      kumo_server_binary=self.options['kumo-server-binary'],
-      kumo_server_ip=ip,
-      kumo_server_log=self.options['kumo-server-log'],
-      kumo_server_storage=kumo_server_storage,
-      kumo_manager_port=kumo_manager_port,
-      kumo_server_port=kumo_server_port,
-      kumo_server_listen_port=kumo_server_listen_port,
-      kumo_gateway_port=kumo_gateway_port,
+      vnc_ip=self.options['vnc-ip'],
+      vnc_port=self.options['vnc-port'],
+      boot_disk_path=self.options['boot-disk-path'],
+      disk_path=self.options['data-disk-path'],
+      disk_size=self.options['data-disk-size'],
+      disk_type=self.options['data-disk-type'],
+      mac_address=self.options['mac-address'],
+      smp_count=self.options['smp-count'],
+      ram_size=self.options['ram-size'],
+      socket_path=self.options['socket-path'],
+      pid_file_path=self.options['pid-path'],
+      python_path=sys.executable,
       shell_path=self.options['shell-path'],
+      qemu_path=self.options['qemu-path'],
+      qemu_img_path=self.options['qemu-img-path'],
+      vnc_passwd=self.options['passwd']
     )
 
-    path_list.append(self.createExecutable(self.options['gateway-wrapper'],
-      self.substituteTemplate(self.getTemplateFilename('kumo_gateway.in'),
-        config)))
+    # Runners
+    runner_path = self.createExecutable(
+      self.options['runner-path'],
+      self.substituteTemplate(self.getTemplateFilename('kvm_run.in'), config))
 
-    path_list.append(self.createExecutable(self.options['manager-wrapper'],
-      self.substituteTemplate(self.getTemplateFilename('kumo_manager.in'),
-        config)))
+    controller_path = self.createExecutable(
+      self.options['controller-path'],
+      self.substituteTemplate(self.getTemplateFilename('kvm_controller_run.in'),
+                              config))
 
-    path_list.append(self.createExecutable(self.options['server-wrapper'],
-      self.substituteTemplate(self.getTemplateFilename('kumo_server.in'),
-        config)))
 
-    return path_list
+    return [runner_path, controller_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/README.librecipe.txt` & `slapos.cookbook-1.0.92/slapos/recipe/README.librecipe.rst`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generatepassword.py` & `slapos.cookbook-1.0.92/slapos/recipe/accords/accords.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# vim: set et sts=2:
+#!%(python_location)s
+
 ##############################################################################
 #
-# Copyright (c) 2012 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -21,78 +22,71 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-
-import errno
 import os
-import random
-import string
-
-def generatePassword(length):
-  return ''.join(random.SystemRandom().sample(string.ascii_lowercase, length))
-
-
-class Recipe(object):
-  """Generate a password that is only composed of lowercase letters
-
-    This recipe only makes sure that ${:passwd} does not end up in `.installed`
-    file, which is world-readable by default. So be careful not to spread it
-    throughout the buildout configuration by referencing it directly: see
-    recipes like slapos.recipe.template:jinja2 to safely process the password.
-
-    Options:
-    - bytes: password length (default: 8 characters)
-    - storage-path: plain-text persistent storage for password,
-                    that can only be accessed by the user
-      (default: ${buildout:parts-directory}/${:_buildout_section_name_})
-
-    If storage-path is empty, the recipe does not save the password, which is
-    fine it is saved by other means, e.g. using the publish-early recipe.
-  """
-
-  def __init__(self, buildout, name, options):
-    options_get = options.get
-    try:
-      self.storage_path = options['storage-path']
-    except KeyError:
-      self.storage_path = options['storage-path'] = os.path.join(
-        buildout['buildout']['parts-directory'], name)
-    passwd = None
-    if self.storage_path:
-      try:
-        with open(self.storage_path) as f:
-          passwd = f.read()
-      except IOError as e:
-        if e.errno != errno.ENOENT:
-          raise
-        self.update = self.install
-    if not passwd:
-      passwd = self.generatePassword(int(options_get('bytes', '8')))
-    self.passwd = passwd
-    # Password must not go into .installed file, for 2 reasons:
-    # security of course but also to prevent buildout to always reinstall.
-    options.get = lambda option, *args, **kw: passwd \
-      if option == 'passwd' else options_get(option, *args, **kw)
-
-  generatePassword = staticmethod(generatePassword)
-
-  def install(self):
-    if self.storage_path:
-      try:
-        os.unlink(self.storage_path)
-      except OSError as e:
-        if e.errno != errno.ENOENT:
-          raise
-      fd = os.open(self.storage_path,
-        os.O_CREAT | os.O_EXCL | os.O_WRONLY | os.O_TRUNC, 0600)
-      try:
-        os.write(fd, self.passwd)
-      finally:
-        os.close(fd)
-      return self.storage_path
-
-  def update(self):
-    return ()
+from slapos import slap
+import signal
+import subprocess
+from subprocess import Popen
+import sys
+import time
+
+def runAccords(accords_conf):
+  """Launch ACCORDS, parse manifest, broker manifest, send connection
+     informations to SlapOS Master. Destroy instance and stops ACCORDS at
+     SIGTERM."""
+  computer_id = accords_conf['computer_id']
+  computer_partition_id = accords_conf['computer_partition_id']
+  server_url = accords_conf['server_url']
+  software_release_url = accords_conf['software_release_url']
+  key_file = accords_conf['key_file']
+  cert_file = accords_conf['cert_file']
+  accords_lib_directory = accords_conf['accords_lib_directory']
+  accords_location = accords_conf['accords_location']
+  manifest_name = accords_conf['manifest_name']
+
+  environment = dict(
+     LD_LIBRARY_PATH=accords_lib_directory,
+     PATH=accords_conf['path'],
+     HOME=accords_location,
+  )
+
+  # Set handler to stop ACCORDS when end of world comes
+  # XXX use subprocess.check_call and add exception handlers
+  def sigtermHandler(signum, frame):
+    Popen(['./co-command', 'stop', '/service/*'],
+        cwd=accords_location, env=environment).communicate()
+    Popen(['./co-stop'],
+        cwd=accords_location, env=environment).communicate()
+    sys.exit(0)
+
+  signal.signal(signal.SIGTERM, sigtermHandler)
+
+  # Launch ACCORDS, parse & broke manifest to deploy instance
+  print 'Starting ACCORDS and friends...'
+  subprocess.check_call(['./co-start'],cwd=accords_location, env=environment)
+  print 'Parsing manifest...'
+  subprocess.check_call(['./co-parser', manifest_name],
+      cwd=accords_location, env=environment)
+  print 'Brokering manifest...'
+  subprocess.check_call(['./co-broker', manifest_name],
+      cwd=accords_location, env=environment)
+  print 'Done.'
+
+  # Parse answer
+  # XXX
+  connection_dict = dict(connection='hardcoded')
+
+  # Send information about published service to SlapOS Master
+  slap_connection = slap.slap()
+  slap_connection.initializeConnection(server_url, key_file, cert_file)
+  computer_partition = slap_connection.registerComputerPartition(computer_id,
+      computer_partition_id)
+  computer_partition.setConnectionDict(connection_dict)
+
+  # Go to sleep, wait kill
+  while(True):
+    time.sleep(60)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/check_page_content/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/erp5_test/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -21,31 +21,32 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
-import sys
 
-class Recipe(GenericBaseRecipe):
-  """
-  Create script that will check if content at "url" is available
-  (e.g page has a link to itself).
-  """
+# The follow recipes should be unified somehow in order to improve
+# code mantainence.
 
+class CloudoooRecipe(GenericBaseRecipe):
   def install(self):
-    url = self.options['url'].strip()
-    config = {
-      'url': url,
-      'shell_path': self.options['dash_path'],
-      'curl_path': self.options['curl_path'],
-      'match': self.options.get('match', url)
-    }
-
-    # XXX-Cedric in this script, curl won't check certificate
-    promise = self.createExecutable(
-      self.options['path'],
-      self.substituteTemplate(self.getTemplateFilename('check_page_content.in'), config)
+    path_list = []
+    common_dict = dict(
+        prepend_path=self.options['prepend-path'],
     )
+    common_list = (
+           "--paster_path", self.options['ooo-paster'],
+           self.options['configuration-file']
+          )
+    path_list.append(self.createPythonScript(self.options['run-unit-test'],
+        __name__ + '.test.runUnitTest',
+        ((self.options['run-unit-test-binary'],
+          ) + common_list, common_dict)))
+    path_list.append(self.createPythonScript(self.options['run-test-suite'],
+        __name__ + '.test.runTestSuite',
+        ((self.options['run-test-suite-binary'],
+          ), common_dict)))
+
+    return path_list
 
-    return [promise]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,40 +47,34 @@
       for k ,v in instance_dict.iteritems():
         config_instance_dict.set('instance_dict', k, v)
       value = StringIO.StringIO()
       config_instance_dict.write(value)
       CONFIG['instance_dict'] = value.getvalue()
 
     software_path_list = json.loads(self.options['software-path-list'])
+    CONFIG["software_path_list"] = ""
     if software_path_list:
       CONFIG["software_path_list"] = "[software_list]"
       CONFIG["software_path_list"] += \
           "\npath_list = %s" % ",".join(software_path_list) 
     CONFIG['computer_id'] = self.buildout['slap-connection']['computer-id']
     CONFIG['server_url'] = self.buildout['slap-connection']['server-url']
+    CONFIG['frontend_url'] = self.buildout['testnode-frontend']['connection-secure_access']
     configuration_file = self.createFile(
       self.options['configuration-file'],
       self.substituteTemplate(
         self.getTemplateFilename('erp5testnode.cfg.in'),
         CONFIG
       ),
     )
     self.path_list.append(configuration_file)
     self.path_list.append(
-      self.createPythonScript(
-        self.options['wrapper'],
-        'slapos.recipe.librecipe.execute.executee',
-        [ # Executable
-          [ self.options['testnode'], '-l', self.options['log-file'],
-            configuration_file],
-          # Environment
-          {
-            'GIT_SSL_NO_VERIFY': '1',
-          }
-        ],
+      self.createWrapper(self.options['wrapper'],
+          ( self.options['testnode'], '-l', self.options['log-file'],
+            configuration_file)
       )
     )
     self.installApache()
     return self.path_list
 
   def installApache(self):
     apache_config = dict(
@@ -100,15 +94,14 @@
         testnode_software_directory=self.options['software-directory'],
     )
     config_file = self.createFile(self.options['httpd-conf-file'],
        self.substituteTemplate(self.getTemplateFilename('httpd.conf.in'),
                                apache_config)
     )
     self.path_list.append(config_file)
-    wrapper = self.createPythonScript(self.options['httpd-wrapper'],
-      'slapos.recipe.librecipe.execute.execute',
-      [self.options['apache-binary'], '-f', config_file, '-DFOREGROUND'])
+    wrapper = self.createWrapper(self.options['httpd-wrapper'],
+      (self.options['apache-binary'], '-f', config_file, '-DFOREGROUND'))
     self.path_list.append(wrapper)
     # create empty html page to not allow listing of /
     page = open(os.path.join(self.options['log-directory'], "index.html"), "w")
     page.write("<html/>")
     page.close()
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/template/erp5testnode.cfg.in` & `slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/template/erp5testnode.cfg.in`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ipv6_address = %(ipv6_address)s
 test_suite_master_url = %(test_suite_master_url)s
 httpd_ip = %(httpd_ip)s
 httpd_port = %(httpd_port)s
 httpd_software_access_port = %(httpd_software_access_port)s
 computer_id = %(computer_id)s
 server_url = %(server_url)s
+frontend_url = %(frontend_url)s
 
 # Binaries
 git_binary = %(git_binary)s
 slapos_binary = %(slapos_binary)s
 zip_binary = %(zip_binary)s
 
 [environment]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5testnode/template/httpd.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/erp5testnode/template/httpd.conf.in`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 CustomLog "%(access_log)s" common
 
 # Allow cross site scripting
 Header set Access-Control-Allow-Origin "*"
 
 # List of modules
 LoadModule unixd_module modules/mod_unixd.so
-LoadModule access_compat_module modules/mod_access_compat.so
 LoadModule authz_core_module modules/mod_authz_core.so
 LoadModule authz_host_module modules/mod_authz_host.so
 LoadModule log_config_module modules/mod_log_config.so
 LoadModule setenvif_module modules/mod_setenvif.so
 LoadModule version_module modules/mod_version.so
 LoadModule proxy_module modules/mod_proxy.so
 LoadModule proxy_http_module modules/mod_proxy_http.so
@@ -34,24 +33,29 @@
 LoadModule negotiation_module modules/mod_negotiation.so
 LoadModule rewrite_module modules/mod_rewrite.so
 LoadModule headers_module modules/mod_headers.so
 LoadModule dir_module modules/mod_dir.so
 LoadModule alias_module modules/mod_alias.so
 LoadModule ssl_module modules/mod_ssl.so
 LoadModule autoindex_module modules/mod_autoindex.so
+# for password access
+LoadModule authn_file_module modules/mod_authn_file.so
+LoadModule authn_core_module modules/mod_authn_core.so
+LoadModule authz_user_module modules/mod_authz_user.so
+LoadModule auth_basic_module modules/mod_auth_basic.so
 
 # SSL Configuration
 SSLEngine on
 SSLCertificateFile %(certificate)s
 SSLCertificateKeyFile %(key)s
 SSLRandomSeed startup builtin
 SSLRandomSeed connect builtin
-SSLProtocol -ALL +SSLv3 +TLSv1
-SSLHonorCipherOrder On
-SSLCipherSuite RC4-SHA:HIGH:!ADH
+SSLProtocol all -SSLv2 -SSLv3
+SSLCipherSuite ECDH+AESGCM:DH+AESGCM:ECDH+AES256:DH+AES256:ECDH+AES128:DH+AES:ECDH+3DES:DH+3DES:RSA+AESGCM:RSA+AES:RSA+3DES:HIGH:!aNULL:!MD5
+SSLHonorCipherOrder on
 SSLProxyEngine On
 
 
 #DocumentRoot "%(testnode_log_directory)s"
 # Directory protection
 #<Directory />
 #    Options Indexes FollowSymLinks
@@ -64,24 +68,25 @@
 <VirtualHost *:%(port)s>
     SSLEngine on
     RewriteRule (.*) http://[%(ip)s]:%(port)s/VirtualHostBase/https/[%(ip)s]:%(port)s/VirtualHostRoot/$1 [L,P]
     DocumentRoot "%(testnode_log_directory)s"
     <Directory />
         Options Indexes FollowSymLinks
         IndexOptions FancyIndexing
-        order allow,deny
-        Allow from All
+        Require all granted
     </Directory>
 </VirtualHost>
 
+# IMPORTANT NOTE: It is very important to deny access by default, otherwise this
+# open access to private repositories. If someone would like to open access to
+# some code, it would be needed to explicitely add a .htaccess file.
 Listen [%(ip)s]:%(software_access_port)s
 <VirtualHost *:%(software_access_port)s>
     SSLEngine on
-    RewriteRule (.*) http://[%(ip)s]:%(software_access_port)s/VirtualHostBase/https/[%(ip)s]:%(software_access_port)s/VirtualHostRoot/$1 [L,P]
-    DocumentRoot "%(testnode_software_directory)s"
+    DocumentRoot "%(testnode_srv_directory)s"
     <Directory />
+        AllowOverride AuthConfig
         Options FollowSymLinks
         IndexOptions FancyIndexing
-        order allow,deny
-        Allow from All
+        Require all denied
    </Directory>
 </VirtualHost>
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/generic_memcached/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/onetimeupload/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,37 +21,34 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
+import binascii
+import os
+import sys
 
 class Recipe(GenericBaseRecipe):
   """
-  memcached instance configuration.
-
-  wrapper-path -- location of the init script to generate
-
-  binary-path -- location of the memcached command
-
-  ip -- ip of the memcached server
-
-  port -- port of the memcached server
+  kvm instance configuration.
   """
-
   def install(self):
-    template_filename = self.getTemplateFilename('memcached.in')
-
     config = dict(
-        memcached_binary=self.options['binary_path'],
-        memcached_ip=self.options['ip'],
-        memcached_port=self.options['port'],
-        shell_path=self.options['shell-path'],
+      ip=self.options['ip'],
+      port=self.options['port'],
+      onetimeupload_path=self.options['onetimeupload-path'],
+      shell_path=self.options['shell-path'],
+      log_path=self.options['log-path'],
+      image=self.options['image-path'],
+      key=self.options['key'],
     )
 
-    executable_path = self.createExecutable(
-      self.options['wrapper_path'],
-      self.substituteTemplate(self.getTemplateFilename('memcached.in'),
+    # Runners
+    runner_path = self.createExecutable(
+      self.options['path'],
+      self.substituteTemplate(self.getTemplateFilename('onetimeupload_run.in'),
                               config))
 
-    return [executable_path]
+    return [runner_path]
+
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/certificate_authority/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/certificate_authority/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,32 +23,31 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 import os
 import hashlib
 import ConfigParser
+import tempfile
 
 from slapos.recipe.librecipe import GenericBaseRecipe
+from certificate_authority import popenCommunicate
 
 class Recipe(GenericBaseRecipe):
 
   def setPath(self):
     self.ca_dir = self.options['ca-dir']
     self.request_directory = self.options['requests-directory']
     self.ca_private = self.options['ca-private']
     self.ca_certs = self.options['ca-certs']
     self.ca_newcerts = self.options['ca-newcerts']
-    self.ca_crl = self.options['ca-crl']
     self.ca_key_ext = '.key'
     self.ca_crt_ext = '.crt'
 
   def install(self):
-    path_list = []
-
     ca_country_code = self.options.get('country-code', 'XX')
     ca_email = self.options.get('email', 'xx@example.com')
     # XXX-BBB: State by mistake has been configured as string "('State',)"
     #          string, so keep this for backward compatibility of existing
     #          automatically setup CAs
     ca_state = self.options.get('state', "('State',)")
     ca_city = self.options.get('city', 'City')
@@ -71,32 +70,33 @@
         city=ca_city,
         company=ca_company,
         email_address=ca_email,
     )
     self.createFile(openssl_configuration, self.substituteTemplate(
       self.getTemplateFilename('openssl.cnf.ca.in'), config))
 
-    ca_wrapper = self.createPythonScript(
+    return self.createPythonScript(
       self.options['wrapper'],
-      '%s.certificate_authority.runCertificateAuthority' % __name__,
-      dict(
-        openssl_configuration=openssl_configuration,
-        openssl_binary=self.options['openssl-binary'],
-        certificate=os.path.join(self.ca_dir, 'cacert.pem'),
-        key=os.path.join(self.ca_private, 'cakey.pem'),
-        crl=self.ca_crl,
-        request_dir=self.request_directory
-      )
+      __name__ + '.certificate_authority.runCertificateAuthority',
+      (os.path.join(self.ca_private, 'cakey.pem'),
+       os.path.join(self.ca_dir, 'cacert.pem'),
+       self.options['openssl-binary'],
+       openssl_configuration,
+       self.request_directory)
     )
-    path_list.append(ca_wrapper)
-
-    return path_list
 
 class Request(Recipe):
 
+  def setPath(self):
+    self.request_directory = self.options['requests-directory']
+    self.ca_private = self.options['ca-private']
+    self.ca_certs = self.options['ca-certs']
+    self.ca_key_ext = '.key'
+    self.ca_crt_ext = '.crt'
+
   def _options(self, options):
     if 'name' not in options:
       options['name'] = self.name
 
   def install(self):
     self.setPath()
 
@@ -110,14 +110,15 @@
     name = self.options['name']
     hash_ = hashlib.sha512(name).hexdigest()
     key = os.path.join(self.ca_private, hash_ + self.ca_key_ext)
     certificate = os.path.join(self.ca_certs, hash_ + self.ca_crt_ext)
 
     # XXX Ugly hack to quickly provide custom certificate/key to everyone using the recipe
     if key_content and cert_content:
+      self._checkCertificateKeyConsistency(key_content, cert_content)
       open(key, 'w').write(key_content)
       open(certificate, 'w').write(cert_content)
       request_needed = False
     else:
       parser = ConfigParser.RawConfigParser()
       parser.add_section('certificate')
       parser.set('certificate', 'name', name)
@@ -132,16 +133,28 @@
         raise OSError("%r file should be a symbolic link." % link)
 
     os.symlink(key, key_file)
     os.symlink(certificate, cert_file)
 
     path_list = [key_file, cert_file]
     if request_needed:
-      wrapper = self.createPythonScript(
+      wrapper = self.createWrapper(
         self.options['wrapper'],
-        'slapos.recipe.librecipe.execute.execute_wait',
-        [ [self.options['executable']],
-          [certificate, key] ],
+        (self.options['executable'],),
+        wait_list=(certificate, key),
       )
       path_list.append(wrapper)
 
     return path_list
+
+  def _checkCertificateKeyConsistency(self, key, certificate):
+    openssl_binary = self.options.get('openssl-binary', 'openssl')
+
+    # Simple test if the user/certificates are readable and don't raise
+    popenCommunicate((openssl_binary, 'x509', '-noout', '-text'), certificate)
+    popenCommunicate((openssl_binary, 'rsa', '-noout', '-text'), key)
+
+    # Check if the key and certificate match
+    modulus_cert = popenCommunicate((openssl_binary, 'x509', '-noout', '-modulus'), certificate)
+    modulus_key = popenCommunicate((openssl_binary, 'rsa', '-noout', '-modulus'), key)
+    if modulus_cert != modulus_key:
+      raise ValueError("The key and certificate provided don't patch each other. Please check your parameters")
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/re6stnet/re6stnet.py` & `slapos.cookbook-1.0.92/slapos/recipe/re6stnet/re6stnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,255 +1,205 @@
 # -*- coding: utf-8 -*-
+import httplib
 import logging
 import json
 import os
 import time
-import sqlite3
 import slapos
 import traceback
-
-from re6st import registry, utils, x509
-from OpenSSL import crypto
-
+import logging
+from re6st import  registry
 
 log = logging.getLogger('SLAPOS-RE6STNET')
-logging.basicConfig(level=logging.DEBUG)
+logging.basicConfig(level=logging.INFO)
+
+logging.trace = logging.debug
 
 def loadJsonFile(path):
   if os.path.exists(path):
     with open(path, 'r') as f:
-      content = f.read()
-      return json.loads(content)
-  else:
-    return {}
+      return json.load(f)
+  return {}
 
 def writeFile(path, data):
   with open(path, 'w') as f:
     f.write(data)
 
 def readFile(path):
   if os.path.exists(path):
     with open(path, 'r') as f:
       content = f.read()
     return content
   return ''
 
-def getDb(db_path):
-  db = sqlite3.connect(db_path, isolation_level=None,
-                                                  check_same_thread=False)
-  db.text_factory = str
-
-  return db.cursor()
-
-def bang(args):
-  computer_guid = args['computer_id']
-  partition_id = args['partition_id']
-  slap = slapos.slap.slap()
+def updateFile(file_path, value):
+  if readFile(file_path) != value:
+    writeFile(file_path, value)
+    return True
+  return False
 
+def getComputerPartition(master_url, key_file, cert_file,
+                         computer_guid, partition_id):
+  slap = slapos.slap.slap()
   # Redeploy instance to update published information
-  slap.initializeConnection(args['server_url'], args['key_file'],
-                                                          args['cert_file'])
-  partition = slap.registerComputerPartition(computer_guid=computer_guid,
-                                                   partition_id=partition_id)
-  partition.bang(message='Published parameters changed!')
-  log.info("Bang with message 'parameters changed'...")
-
-
-def requestAddToken(args, can_bang=True):
+  slap.initializeConnection(master_url, key_file, cert_file)
+  return slap.registerComputerPartition(computer_guid, partition_id)
 
+def requestAddToken(client, token_base_path):
   time.sleep(3)
-  registry_url = args['registry_url']
-  base_token_path = args['token_base_path']
-  path_list = [x for x in os.listdir(base_token_path) if x.endswith('.add')]
+  path_list = [x for x in os.listdir(token_base_path) if x.endswith('.add')]
+
+  log.info("Searching tokens to add at %s and found %s." % (token_base_path, path_list))
 
   if not path_list:
     log.info("No new token to add. Exiting...")
     return
 
-  client = registry.RegistryClient(registry_url)
-  call_bang = False
-
   for reference_key in path_list:
-    request_file = os.path.join(base_token_path, reference_key)
+    request_file = os.path.join(token_base_path, reference_key)
     token = readFile(request_file)
+    log.info("Including token %s for %s" % (token, reference_key))
     if token :
       reference = reference_key.split('.')[0]
       # email is unique as reference is also unique
       email = '%s@slapos' % reference.lower()
       try:
-        result = client.requestAddToken(token, email)
+        result = client.addToken(email, token)
       except Exception:
-        log.debug('Request add token fail for %s... \n %s' % (request_file,
+        log.info('Request add token fail for %s... \n %s' % (request_file,
                     traceback.format_exc()))
         continue
-      if result and result == token:
+
+      if result in (token, None):
         # update information
         log.info("New token added for slave instance %s. Updating file status..." %
                             reference)
-        writeFile(os.path.join(base_token_path, '%s.status' % reference),
-                    'TOKEN_ADDED')
+        status_file = os.path.join(token_base_path, '%s.status' % reference)
+        updateFile(status_file, 'TOKEN_ADDED')
         os.unlink(request_file)
-        call_bang = True
     else:
       log.debug('Bad token. Request add token fail for %s...' % request_file)
 
-  if can_bang and call_bang:
-    bang(args)
-
-def requestRemoveToken(args):
-  base_token_path = args['token_base_path']
-  path_list = [x for x in os.listdir(base_token_path) if x.endswith('.remove')]
+def requestRemoveToken(client, token_base_path):
+  path_list = [x for x in os.listdir(token_base_path) if x.endswith('.remove')]
 
   if not path_list:
     log.info("No token to delete. Exiting...")
     return
 
-  client = registry.RegistryClient(args['registry_url'])
   for reference_key in path_list:
-    request_file = os.path.join(base_token_path, reference_key)
+    request_file = os.path.join(token_base_path, reference_key)
     token = readFile(request_file)
     if token :
       reference = reference_key.split('.')[0]
       try:
-        result = client.requestDeleteToken(token)
+        result = client.deleteToken(token)
+      except httplib.NOTFOUND:
+        # Token is alread removed.
+        result = True
       except Exception:
         log.debug('Request delete token fail for %s... \n %s' % (request_file,
                     traceback.format_exc()))
         continue
       else:
         # certificate is invalidated, it will be revoked
-        writeFile(os.path.join(base_token_path, '%s.revoke' % reference), '')
-      if result == 'True':
+        writeFile(os.path.join(token_base_path, '%s.revoke' % reference), '')
+
+      if result in (True, 'True'):
         # update information
         log.info("Token deleted for slave instance %s. Clean up file status..." %
                             reference)
+
       if result in ['True', 'False']:
         os.unlink(request_file)
-        status_file = os.path.join(base_token_path, '%s.status' % reference)
+        status_file = os.path.join(token_base_path, '%s.status' % reference)
         if os.path.exists(status_file):
           os.unlink(status_file)
-        ipv6_file = os.path.join(base_token_path, '%s.ipv6' % reference)
+        ipv6_file = os.path.join(token_base_path, '%s.ipv6' % reference)
         if os.path.exists(ipv6_file):
           os.unlink(ipv6_file)
 
     else:
       log.debug('Bad token. Request add token fail for %s...' % request_file)
 
-def requestRevoqueCertificate(args):
-
-  base_token_path = args['token_base_path']
-  db = getDb(args['db'])
-  path_list = [x for x in os.listdir(base_token_path) if x.endswith('.revoke')]
-  client = registry.RegistryClient(args['registry_url'])
-
-  for reference_key in path_list:
-    reference = reference_key.split('.')[0]
-    # XXX - email is always unique
-    email = '%s@slapos' % reference.lower()
-    cert_string = ''
-    try:
-      cert_string, = db.execute("SELECT cert FROM cert WHERE email = ?",
-          (email,)).next()
-    except StopIteration:
-      # Certificate was not generated yet !!!
-      pass
-
-    try:
-      if cert_string:
-        cert = crypto.load_certificate(crypto.FILETYPE_PEM, cert_string)
-        cn = x509.subnetFromCert(cert)
-        result = client.revoke(str(cn))
-        time.sleep(2)
-    except Exception:
-      log.debug('Request revoke certificate fail for %s... \n %s' % (reference,
-                  traceback.format_exc()))
-      continue
-    else:
-      os.unlink(os.path.join(base_token_path, reference_key))
-      log.info("Certificate revoked for slave instance %s." % reference)
-
-
-def dumpIPv6Network(slave_reference, db, network, ipv6_file):
-  email = '%s@slapos' % slave_reference.lower()
-
-  try:
-    cert_string, = db.execute("SELECT cert FROM cert WHERE email = ?",
-        (email,)).next()
-  except StopIteration:
-    # Certificate was not generated yet !!!
-    pass
-
-  try:
-    if cert_string:
-      cert = crypto.load_certificate(crypto.FILETYPE_PEM, cert_string)
-      cn = x509.subnetFromCert(cert)
-      subnet = network + utils.binFromSubnet(cn)
-      ipv6 = utils.ipFromBin(subnet)
-      writeFile(ipv6_file, ipv6)
-  except Exception:
-    log.debug('XXX for %s... \n %s' % (slave_reference,
-              traceback.format_exc()))
-
-def checkService(args, can_bang=True):
-  base_token_path = args['token_base_path']
-  token_dict = loadJsonFile(args['token_json'])
-
+def checkService(client, token_base_path, token_json, computer_partition):
+  token_dict = loadJsonFile(token_json)
+  updated = False
   if not token_dict:
     return
 
-  db = getDb(args['db'])
-  call_bang = False
-
-  computer_guid = args['computer_id']
-  partition_id = args['partition_id']
-  slap = slapos.slap.slap()
-  client = registry.RegistryClient(args['registry_url'])
-  ca = client.getCa()
-  network = x509.networkFromCa(crypto.load_certificate(crypto.FILETYPE_PEM, ca))
-
   # Check token status
   for slave_reference, token in token_dict.iteritems():
-    status_file = os.path.join(base_token_path, '%s.status' % slave_reference)
-    ipv6_file = os.path.join(base_token_path, '%s.ipv6' % slave_reference)
+    log.info("%s %s" % (slave_reference, token))
+    status_file = os.path.join(token_base_path, '%s.status' % slave_reference)
     if not os.path.exists(status_file):
       # This token is not added yet!
+      log.info("Token %s dont exist yet." % status_file)
       continue
 
-    msg = readFile(status_file)
-    if msg == 'TOKEN_USED':
-      dumpIPv6Network(slave_reference, db, network, ipv6_file)
-      continue
-
-    # Check if token is not in the database
-    status = False
-    try:
-        token_found, = db.execute("SELECT token FROM token WHERE token = ?",
-            (token,)).next()
-        if token_found == token:
-          status = True
-    except StopIteration:
-        pass
-    if not status:
+    if not client.isToken(str(token)):
       # Token is used to register client
-      call_bang = True
+      updateFile(status_file, 'TOKEN_USED')
+      log.info("Token status of %s updated to 'used'." % slave_reference)
+
+    status = readFile(status_file)
+    log.info("Token %s has %s State." % (status_file, status))
+
+    ipv6 = "::"
+    ipv4 = "0.0.0.0"
+    msg = status
+    if status == 'TOKEN_ADDED':
+      msg = 'Token is ready for use'
+    elif status == 'TOKEN_USED':
+      msg = 'Token not available, it has been used to generate re6stnet certificate.'
+
+    email = '%s@slapos' % slave_reference.lower()
+    if status == 'TOKEN_USED':
       try:
-        writeFile(status_file, 'TOKEN_USED')
-        dumpIPv6Network(slave_reference, db, network, ipv6_file)
-        log.info("Token status of %s updated to 'used'." % slave_reference)
-      except IOError:
-        # XXX- this file should always exists
-        log.debug('Error when writing in file %s. Clould not update status of %s...' %
-                              (status_file, slave_reference))
+        ipv6 = client.getIPv6Address(str(email))
+      except Exception:
+        log.info('Error for dump ipv6 for %s... \n %s' % (slave_reference,
+                                        traceback.format_exc()))
 
-  if call_bang and can_bang:
-    bang(args)
+      log.info("%s, IPV6 = %s" % (slave_reference, ipv6))
+      try:
+        ipv4 = client.getIPv4Information(str(email)) or "0.0.0.0"
+      except Exception:
+        log.info('Error for dump ipv4 for %s... \n %s' % (slave_reference,
+                                        traceback.format_exc()))
+
+      log.info("%s, IPV4 = %s" % (slave_reference, ipv4))
+
+    try:
+      log.info("Update parameters for %s" % slave_reference)
+
+      # Normalise the values as simple strings to be on the same format that
+      # the values which come from master.
+      computer_partition.setConnectionDict({'token': str(token),
+                                            '1_info': str(msg),
+                                            'ipv6': str(ipv6),
+                                            'ipv4': str(ipv4)},
+          slave_reference)
+    except Exception:
+      log.fatal("Error while sending slave %s informations: %s",
+         slave_reference, traceback.format_exc())
+
+
+def manage(registry_url, token_base_path, token_json,
+           computer_dict, can_bang=True):
 
-def manage(args):
+  client = registry.RegistryClient(registry_url)
+
+  log.info("ADD TOKEN")
   # Request Add new tokens
-  requestAddToken(args)
+  requestAddToken(client, token_base_path)
 
+  log.info("Remove TOKEN")
   # Request delete removed token
-  requestRemoveToken(args)
+  requestRemoveToken(client, token_base_path)
+
+  computer_partition = getComputerPartition(**computer_dict)
 
+  log.info("Update Services")
   # check status of all token
-  checkService(args)
+  checkService(client, token_base_path, token_json, computer_partition)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/re6stnet/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/trac.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 ##############################################################################
 #
 # Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
@@ -20,250 +21,163 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
+import os
+import sys
 import subprocess
+import shutil
+import json
 
 from slapos.recipe.librecipe import GenericBaseRecipe
-import socket
-import struct
-import os, stat
-import string, random
-import json
-import traceback
-from slapos import slap
 
 class Recipe(GenericBaseRecipe):
-  
+
   def __init__(self, buildout, name, options):
-    """Default initialisation"""
-    self.slap = slap.slap()
 
-    # SLAP related information
-    slap_connection = buildout['slap-connection']
-    self.computer_id = slap_connection['computer-id']
-    self.computer_partition_id = slap_connection['partition-id']
-    self.server_url = slap_connection['server-url']
-    self.software_release_url = slap_connection['software-release-url']
-    self.key_file = slap_connection.get('key-file')
-    self.cert_file = slap_connection.get('cert-file')
-    self.slave_list = json.loads(options['slave-instance-list'])
+    pythonPath = ""
 
-    options['slave-amount'] = '%s' % len(self.slave_list)
+    for eggs in options['eggs-dirs'].splitlines():
+      if eggs:
+        for item in os.listdir(eggs):
+          path = os.path.join(eggs, item)
+          pythonPath = path + ":" + pythonPath
+
+    options['python_path'] = pythonPath
+    options['wsgi-dir'] = os.path.join(options['site-dir'].strip(), 'apache')
+    options['git-dir'] = os.path.join(options['site-dir'].strip(), 'git')
+    options['svn-dir'] = os.path.join(options['site-dir'].strip(), 'svn')
     return GenericBaseRecipe.__init__(self, buildout, name, options)
 
-  def getSerialFromIpv6(self, ipv6):
-    prefix = ipv6.split('/')[0].lower()
-    hi, lo = struct.unpack('!QQ', socket.inet_pton(socket.AF_INET6, prefix))
-    ipv6_int = (hi << 64) | lo
-    serial = '0x1%x' % ipv6_int
-
-    # delete non significant part
-    for part in prefix.split(':')[::-1]:
-      if part:
-        for i in ['0']*(4 - len(part)):
-          part = i + part
-        serial = serial.split(part)[0] + part
-        break
-
-    return serial
-
-  def generateCertificate(self):
-    key_file = self.options['key-file'].strip()
-    cert_file = self.options['cert-file'].strip()
-    dh_file = self.options['dh-file'].strip()
-    if not os.path.exists(dh_file):
-      dh_command = [self.options['openssl-bin'], 'dhparam', '-out',
-                            '%s' % dh_file, self.options['key-size']]
-      try:
-        subprocess.check_call(dh_command)
-      except Exception:
-        if os.path.exists(dh_file):
-          os.unlink(dh_file)
-        raise
-
-    if not os.path.exists(cert_file):
-      serial = self.getSerialFromIpv6(self.options['ipv6-prefix'].strip())
-      key_command = [self.options['openssl-bin'], 'genrsa', '-out',
-                            '%s' % key_file, self.options['key-size']]
-
-      #'-config', openssl_configuration
-      cert_command = [self.options['openssl-bin'], 'req', '-nodes', '-new',
-                  '-x509', '-batch', '-key', '%s' % key_file, '-set_serial',
-                  '%s' % serial, '-days', '3650', '-out', '%s' % cert_file]
-
-      try:
-        subprocess.check_call(key_command)
-      except Exception:
-        if os.path.exists(key_file):
-          os.unlink(key_file)
-        raise
-
-      try:
-        subprocess.check_call(cert_command)
-      except Exception:
-        if os.path.exists(cert_file):
-          os.unlink(cert_file)
-        raise
-
-  def generateSlaveTokenList(self, slave_instance_list, token_file):
-    to_remove_dict = {}
-    to_add_dict = {}
-    token_dict = self.loadJsonFile(token_file)
-
-    reference_list = [slave_instance.get('slave_reference') for slave_instance
-                        in slave_instance_list]
-    for reference in reference_list:
-      if not reference in token_dict:
-        # we generate new token
-        number = reference.split('-')[1]
-        new_token = number + ''.join(random.sample(string.ascii_lowercase, 20))
-        token_dict[reference] = new_token
-        to_add_dict[reference] = new_token
-
-    for reference in token_dict.keys():
-      if not reference in reference_list:
-        # This slave instance is destroyed ?
-        to_remove_dict[reference] = token_dict.pop(reference)
-
-    return token_dict, to_add_dict, to_remove_dict
-
-  def loadJsonFile(self, path):
-    if os.path.exists(path):
-      with open(path, 'r') as f:
-        content = f.read()
-      return json.loads(content)
-    else:
-      return {}
-
-  def writeFile(self, path, data):
-    with open(path, 'w') as f:
-      f.write(data)
-    return path
-
-  def readFile(self, path):
-    if os.path.exists(path):
-      with open(path, 'r') as f:
-        content = f.read()
-      return content
-    return ''
-
-  def genHash(self, length):
-    hash_path = os.path.join(self.options['conf-dir'], '%s-hash' % length)
-    if not os.path.exists(hash_path):
-      pool = string.letters + string.digits
-      hash_string = ''.join(random.choice(pool) for i in xrange(length))
-      self.writeFile(hash_path, hash_string)
-    else:
-      hash_string = self.readFile(hash_path)
-
-    return hash_string
-
   def install(self):
-    path_list = []
-    token_save_path = os.path.join(self.options['conf-dir'], 'token.json')
-    token_list_path = self.options['token-dir']
-
-    self.generateCertificate()
-
-    wrapper = self.createFile(self.options['wrapper'], self.substituteTemplate(
-      self.getTemplateFilename('registry-run.in'), dict(
-          parameter='@%s' % self.options['config-file'],
-          pid_file=self.options['pid-file'],
-          command=self.options['command']
-        )
-      )
-    )
-    os.chmod(self.options['wrapper'], stat.S_IRWXU)
-
-    path_list.append(wrapper)
+    install_path = []
 
-    registry_url = 'http://%s:%s/' % (self.options['ipv4'], self.options['port'])
-    token_dict, add_token_dict, rm_token_dict = self.generateSlaveTokenList(
-                                              self.slave_list, token_save_path)
-
-    # write request add token
-    for reference in add_token_dict:
-      path = os.path.join(token_list_path, '%s.add' % reference)
-      if not os.path.exists(path):
-        self.createFile(path, add_token_dict[reference])
-
-    # write request remove token
-    for reference in rm_token_dict:
-      path = os.path.join(token_list_path, '%s.remove' % reference)
-      if not os.path.exists(path):
-        self.createFile(path, rm_token_dict[reference])
-        # remove request add token if exists
-        add_path = os.path.join(token_list_path, '%s.add' % reference)
-        if os.path.exists(add_path):
-          os.unlink(add_path)
-
-    self.createFile(token_save_path, json.dumps(token_dict))
-
-    service_dict = dict(token_base_path=token_list_path,
-                        token_json=token_save_path,
-                        db=self.options['db-path'],
-                        partition_id=self.computer_partition_id,
-                        computer_id=self.computer_id,
-                        registry_url=registry_url)
-    service_dict['server_url'] = self.server_url
-    service_dict['cert_file'] = self.cert_file
-    service_dict['key_file'] = self.key_file
-
-    request_add = self.createPythonScript(
-        self.options['manager-wrapper'].strip(),
-        '%s.re6stnet.manage' % __name__, service_dict
+    env = os.environ
+    env['LD_LIBRARY_PATH'] = self.options['python-lib']
+    project_dir = self.options['site-dir'].strip()
+    trac_admin = self.options['trac-admin'].strip()
+    admin = self.options['admin-user'].strip()
+    passwd = self.options['admin-password'].strip()
+    config = os.path.join(project_dir, 'conf/trac.ini')
+    filestat = self.options['file-status'].strip()
+    self.logger.info("Checking if trac project is not installed...")
+    if os.path.exists(filestat):
+      os.unlink(filestat)
+    if not os.path.exists(project_dir):
+      self.logger.info("Starting trac project installation at %s" % project_dir)
+      trac_args = [trac_admin, project_dir, 'initenv']
+      db_string = "mysql://%s:%s@%s:%s/%s" % (
+                  self.options['mysql-username'].strip(),
+                  self.options['mysql-password'].strip(),
+                  self.options['mysql-host'].strip(),
+                  self.options['mysql-port'].strip(),
+                  self.options['mysql-database'].strip()
       )
-    path_list.append(request_add)
-
-    request_drop = self.createPythonScript(
-        self.options['drop-service-wrapper'].strip(),
-        '%s.re6stnet.requestRemoveToken' % __name__, service_dict
-      )
-    path_list.append(request_drop)
-
-    request_check = self.createPythonScript(
-        self.options['check-service-wrapper'].strip(),
-        '%s.re6stnet.checkService' % __name__, service_dict
-      )
-    path_list.append(request_check)
-
-    revoke_check = self.createPythonScript(
-        self.options['revoke-service-wrapper'].strip(),
-        '%s.re6stnet.requestRevoqueCertificate' % __name__, service_dict
-      )
-    path_list.append(revoke_check)
-
-    # Send connection parameters of slave instances
-    if token_dict:
-      self.slap.initializeConnection(self.server_url, self.key_file,
-        self.cert_file)
-      computer_partition = self.slap.registerComputerPartition(
-        self.computer_id,
-        self.computer_partition_id)
-
-      for slave_reference, token in token_dict.iteritems():
-        try:
-          status_file = os.path.join(token_list_path, '%s.status' % slave_reference)
-          status = self.readFile(status_file) or 'New token requested'
-          msg = status
-          if status == 'TOKEN_ADDED':
-            msg = 'Token is ready for use'
-          elif status == 'TOKEN_USED':
-            msg = 'Token not available, it has been used to generate re6stnet certificate.'
-
-          ipv6_file = os.path.join(token_list_path, '%s.ipv6' % slave_reference)
-          ipv6 = self.readFile(ipv6_file) or '::'
-
-          computer_partition.setConnectionDict(
-              {'token':token, '1_info':msg, 'ipv6': ipv6},
-              slave_reference)
-        except Exception:
-          self.logger.fatal("Error while sending slave %s informations: %s",
-             slave_reference, traceback.format_exc())
-
-    return path_list
+      process_install = subprocess.Popen(trac_args, stdout=subprocess.PIPE,
+              stdin=subprocess.PIPE, stderr=subprocess.STDOUT, env=env)
+      process_install.stdin.write('%s\n%s\n' % (self.options['project'].strip(),
+                                            db_string))
+      result = process_install.communicate()[0]
+      process_install.stdin.close()
+      if process_install.returncode is None or process_install.returncode != 0:
+        if os.path.exists(project_dir):
+          shutil.rmtree(project_dir)
+        self.logger.error("Failed to initialize Trac.\nThe error was: %s" % result)
+        return []
+      os.mkdir(self.options['git-dir'])
+      os.mkdir(self.options['svn-dir'])
+      os.mkdir(self.options['wsgi-dir'])
+      os.unlink(config)
+      shutil.copy(self.options['trac-ini'].strip(), config)
+      shutil.copy(self.options['trac-wsgi'].strip(),
+                      os.path.join(self.options['wsgi-dir'], 'trac.wsgi'))
+    else:
+      self.logger.info("The directory %s already exist, skip project installation"
+                      % project_dir)
+      trac_args = [trac_admin, project_dir, 'repository', 'list']
+      process_upgrade = subprocess.Popen(trac_args, stdout=subprocess.PIPE,
+              stderr=subprocess.STDOUT)
+      result = process_upgrade.communicate()[0]
+      if process_upgrade.returncode is None or process_upgrade.returncode != 0:
+        self.logger.error("Failed to run Trac.\nThe error was: %s" % result)
+        return []
+
+    #Add All grant to admin user
+    self.logger.info("Granting admin rights to the admin user.")
+    trac_grant = [trac_admin, project_dir, "permission add %s TRAC_ADMIN" % admin]
+    process = subprocess.Popen(trac_grant, stdout=subprocess.PIPE,
+              stderr=subprocess.STDOUT, env=env)
+    result = process.communicate()[0]
+    if process.returncode is None or process.returncode != 0:
+      raise Exception("Failed to execute Trac-admin.\nThe error was: %s" % result)
+
+    self.logger.info("Copying additional plugins into plugins directory")
+    plugins_dir = os.path.join(project_dir, "plugins")
+    for item in os.listdir(self.options['plugins-egg-dir'].strip()):
+      source = os.path.join(self.options['plugins-egg-dir'].strip(), item)
+      destination = os.path.join(plugins_dir, item)
+      if not os.path.exists(destination):
+        shutil.copytree(source, destination)
+
+    svn_list = json.loads(self.options.get('svn-project-list', '{}'))
+    for svn_repo in svn_list:
+      svn_repo_path = os.path.join(self.options['svn-dir'], svn_repo)
+      if not os.path.exists(svn_repo_path):
+        self.logger.info("Initializing %s SVN repository..." % svn_repo)
+        svn_args = [self.options['svn-repo-script'], project_dir,
+                    svn_repo, svn_list[svn_repo]]
+        process = subprocess.Popen(svn_args, stdout=subprocess.PIPE,
+                stderr=subprocess.STDOUT)
+        result = process.communicate()[0]
+        if process.returncode is None or process.returncode != 0:
+          shutil.rmtree(svn_repo_path)
+          raise Exception("Failed to create repository.\nThe error was: %s" % result)
+        shutil.copy(self.options['trac-svn-hook'].strip(),
+                      os.path.join(svn_repo_path, 'hooks/post-commit'))
+        shutil.copy(self.options['post-revprop-change'].strip(),
+                      os.path.join(svn_repo_path, 'hooks/post-revprop-change'))
+        self.logger.info("Finished initializing %s reposiroty" % svn_repo)
+
+    repolist = json.loads(self.options.get('git-project-list', '{}'))
+    for repo, desc in repolist.iteritems():
+      absolute_path = os.path.join(self.options['git-dir'], '%s.git' % repo)
+      if not os.path.exists(absolute_path):
+        self.logger.info("Initializing %s GIT repository..." % repo)
+        subprocess.check_call([self.options['git-binary'], 'init',
+                    '--bare', absolute_path])
+        subprocess.check_call([trac_admin, project_dir, 'repository',
+                    'add', repo, absolute_path, 'git'], env=env)
+        subprocess.check_call([trac_admin, project_dir, 'repository',
+                    'resync', repo], env=env)
+        # XXX: Hardcoded path
+        shutil.copy(self.options['trac-git-hook'].strip(),
+                      os.path.join(absolute_path, 'hooks/post-commit'))
+        description_filename = os.path.join(absolute_path, 'description')
+        with open(description_filename, 'w') as description_file:
+          description_file.write(desc)
+
+    user_list = json.loads(self.options.get('user-list', '{}'))
+    fd = open(os.path.join(project_dir, 'svnpasswd'), 'w')
+    fd.write("[users]\n%s = %s" % (admin, passwd))
+    os.system("%s -cb %s %s %s" % (self.options['htpasswd'],
+                                  self.options['passwd-file'],
+                                  admin, passwd)
+    )
+    for user in user_list:
+      self.logger.info("Creating or updating user %s ..." % user)
+      user_args = [self.options['htpasswd'], '-b', self.options['passwd-file'],
+                  user, user_list[user]]
+      process = subprocess.Popen(user_args, stdout=subprocess.PIPE,
+                stderr=subprocess.STDOUT)
+      result = process.communicate()[0]
+      if process.returncode is None or process.returncode != 0:
+          raise Exception("Failed to create user %s.\nThe error was: %s" %
+                          (user, result))
+      fd.write("\n%s = %s" % (user, user_list[user]))
+    fd.close()
+    open(filestat, "w").write("done.")
 
+    return install_path
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/check_parameter/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/check_url_available/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# vim: set et sts=2:
 ##############################################################################
 #
-# Copyright (c) 2015 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -23,36 +22,35 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 from slapos.recipe.librecipe import GenericBaseRecipe
 import sys
+import os
 
 class Recipe(GenericBaseRecipe):
   """
-  Check listening port promise
+  Create script that will check if "url" is available (e.g page answers 200 OK).
   """
 
   def install(self):
-    config = dict(
-      value=self.options['value'],
-      python_path=sys.executable,
-    )
-
-    if self.options.get('expected-type') == "ipv6":
-      template = self.getTemplateFilename('check_ipv6.py.in')
-
-    elif self.options.get('expected-type') == "ipv4":
-      template = self.getTemplateFilename('check_ipv4.py.in')
-    else:
-      config["expected-value"] = self.options.get('expected-value')
- 
-      config["expected-not-value"] = self.options.get('expected-not-value')
-
-      template = self.getTemplateFilename('check_parameter.py.in')
+    timeout_file = os.path.join(os.getcwd(), 'etc/promise_timeout')
+    config = {
+      'url': self.options['url'],
+      'shell_path': self.options['dash_path'],
+      'curl_path': self.options['curl_path'],
+      'check_secure': self.options.get('check-secure', 0),
+      'http_code': self.options.get('http_code', '200'),
+      'time_out': self.options.get('timeout-file-path', timeout_file),
+      'ca-cert-file': self.options.get('ca-cert-file', ''),
+      'cert-file': self.options.get('cert-file', ''),
+      'key-file': self.options.get('key-file', ''),
+    }
 
+    # XXX-Cedric in this script, curl won't check certificate
     promise = self.createExecutable(
       self.options['path'],
-      self.substituteTemplate(template, config))
+      self.substituteTemplate(self.getTemplateFilename('check_url.in'), config)
+    )
 
     return [promise]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/novnc/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/novnc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,22 @@
 
 class Recipe(GenericBaseRecipe):
   """
   novnc instance configuration.
   """
 
   def install(self):
-    runner_path = self.createPythonScript(
+    return self.createWrapper(
       self.options['path'],
-      'slapos.recipe.librecipe.execute.execute_wait',
-      [[
+      (
         self.options['websockify-path'],
         '--web',
         self.options['novnc-location'],
         '--key=%s' % self.options['ssl-key-path'],
         '--cert=%s' % self.options['ssl-cert-path'],
         '--ssl-only',
         '%s:%s' % (self.options['ip'], self.options['port']),
         '%s:%s' % (self.options['vnc-ip'], self.options['vnc-port']),
-      ],
-      [self.options['ssl-key-path'], self.options['ssl-cert-path']]],
+       ),
+      wait_list=(self.options['ssl-key-path'],
+                 self.options['ssl-cert-path']),
     )
-
-    return [runner_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apachephp/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/random.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2016 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,141 +20,163 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-import shutil
+
+"""
+Collects various random generators to be used in
+buildout Software Releases and Instances developments.
+"""
+
+from __future__ import absolute_import
+
+import errno
 import os
-import signal
-from binascii import b2a_uu as uuencode
+import random
+import string
 
 from slapos.recipe.librecipe import GenericBaseRecipe
 
-class Recipe(GenericBaseRecipe):
+class Integer(object):
+  """
+  Generate a random integer (see standard random.randint documentation).
+
+  Input options:
+  minimum (required)
+    integer(-ish) minmum bound, included.
+  maximum (required)
+    integer(-ish) maximum bound, included.
+
+  Output options:
+  value
+    Resulting integer.
+  """
+  def __init__(self, buildout, name, options):
+    options['value'] = random.randint(int(options['minimum']), int(options['maximum']))
+
+  def install(self):
+    pass
+
+  update = install
+
+class Time(object):
+  """Generate a random time from a 24h time clock"""
 
   def __init__(self, buildout, name, options):
-    self.environ = {}
+    self.name = name
+    self.buildout = buildout
+    self.options = options
+    self.options['time'] = "%d:%d" % (random.randint(0, 23), random.randint(0, 59))
+
+  def install(self):
+    pass
 
-    environment_section = options.get('environment-section', '').strip()
-    if environment_section and environment_section in buildout:
-      # Use environment variables from the designated config section.
-      self.environ.update(buildout[environment_section])
-    for variable in options.get('environment', '').splitlines():
-      if variable.strip():
-        try:
-          key, value = variable.split('=', 1)
-          self.environ[key.strip()] = value
-        except ValueError:
-          raise zc.buildout.UserError('Invalid environment variable definition: %s', variable)
-    # Extrapolate the environment variables using values from the current
-    # environment.
-    for key in self.environ:
-      self.environ[key] = self.environ[key] % os.environ
+  update = install
 
+
+class Mac(GenericBaseRecipe):
+
+  def __init__(self, buildout, name, options):
+    if os.path.exists(options['storage-path']):
+      open_file = open(options['storage-path'], 'r')
+      options['mac-address'] = open_file.read()
+      open_file.close()
+
+    if options.get('mac-address', '') == '':
+      # First octet has to represent a locally administered address
+      octet_list = [254] + [random.randint(0x00, 0xff) for x in range(5)]
+      options['mac-address'] = ':'.join(['%02x' % x for x in octet_list])
     return GenericBaseRecipe.__init__(self, buildout, name, options)
 
   def install(self):
-    path_list = []
+    open_file = open(self.options['storage-path'], 'w')
+    open_file.write(self.options['mac-address'])
+    open_file.close()
+    return [self.options['storage-path']]
+
+
+def generatePassword(length):
+  return ''.join(random.SystemRandom().sample(string.ascii_lowercase, length))
+
+
+class Password(object):
+  """Generate a password that is only composed of lowercase letters
+
+    This recipe only makes sure that ${:passwd} does not end up in `.installed`
+    file, which is world-readable by default. So be careful not to spread it
+    throughout the buildout configuration by referencing it directly: see
+    recipes like slapos.recipe.template:jinja2 to safely process the password.
+
+    Options:
+    - bytes: password length (default: 8 characters)
+    - storage-path: plain-text persistent storage for password,
+                    that can only be accessed by the user
+      (default: ${buildout:parts-directory}/${:_buildout_section_name_})
+    - create-once: boolean value which set if storage-path won't be modified
+                   as soon the file is created with the password (not empty).
+      (default: True)
+
+    If storage-path is empty, the recipe does not save the password, which is
+    fine it is saved by other means, e.g. using the publish-early recipe.
+  """
 
-    # Copy application if not already existing
-    htdocs_location = self.options['htdocs']
-    if not (os.path.exists(htdocs_location) and os.listdir(htdocs_location)):
+  def __init__(self, buildout, name, options):
+    self.create_once = options.get('create-once', 'True').lower() \
+          in GenericBaseRecipe.TRUE_VALUES
+    try:
+      self.storage_path = options['storage-path']
+    except KeyError:
+      self.storage_path = options['storage-path'] = os.path.join(
+        buildout['buildout']['parts-directory'], name)
+    passwd = None
+    if self.storage_path:
       try:
-        os.rmdir(htdocs_location)
-      except:
-        pass
-      shutil.copytree(self.options['source'], htdocs_location)
-
-    # Install php.ini
-    php_ini = self.createFile(os.path.join(self.options['php-ini-dir'],
-                                           'php.ini'),
-      self.substituteTemplate(self.getTemplateFilename('php.ini.in'),
-        dict(tmp_directory=self.options['tmp-dir']))
-    )
-    path_list.append(php_ini)
-
-    # Install apache
-    if self.optionIsTrue('default-conf', True):
-      apache_config = dict(
-        pid_file=self.options['pid-file'],
-        lock_file=self.options['lock-file'],
-        ip=self.options['ip'],
-        port=self.options['port'],
-        error_log=self.options['error-log'],
-        access_log=self.options['access-log'],
-        document_root=self.options['htdocs'],
-        php_ini_dir=self.options['php-ini-dir'],
-      )
-      httpd_conf = self.createFile(self.options['httpd-conf'],
-        self.substituteTemplate(self.getTemplateFilename('apache.in'),
-                                apache_config)
-      )
-      path_list.append(httpd_conf)
-
-    wrapper = self.createWrapper(name=self.options['wrapper'],
-                                 command=self.options['httpd-binary'],
-                                 parameters=[
-                                     '-f',
-                                     self.options['httpd-conf'],
-                                     '-DFOREGROUND'
-                                     ],
-                                 environment=self.environ)
-    path_list.append(wrapper)
-
-    secret_key_filename = os.path.join(self.buildout['buildout']['directory'],
-                                       '.php_secret_key')
-    if not os.path.exists(secret_key_filename):
-      secret_key = uuencode(os.urandom(45)).strip()
-      # Remove unsafe characters
-      secret_key = secret_key.translate(None, '"\'\\')
-      with open(secret_key_filename, 'w') as secret_key_file:
-        secret_key_file.write(secret_key)
+        with open(self.storage_path) as f:
+          passwd = f.read().strip('\n')
+      except IOError as e:
+        if e.errno != errno.ENOENT:
+          raise
+    if not passwd:
+      passwd = self.generatePassword(int(options.get('bytes', '8')))
+      self.update = self.install
+    self.passwd = passwd
+    # Password must not go into .installed file, for 2 reasons:
+    # security of course but also to prevent buildout to always reinstall.
+    def get(option, *args, **kw):
+      return passwd if option == 'passwd' else options_get(option, *args, **kw)
+
+    try:
+      options_get = options._get
+    except AttributeError:
+      options_get = options.get
+      options.get = get
     else:
-      with open(secret_key_filename, 'r') as secret_key_file:
-        secret_key = secret_key_file.read()
+      options._get = get
+
+  generatePassword = staticmethod(generatePassword)
+
+  def install(self):
+    if self.storage_path:
+      try:
+        # The following 2 lines are just an optimization to avoid recreating
+        # the file with the same content.
+        if self.create_once and os.stat(self.storage_path).st_size:
+          return
+        os.unlink(self.storage_path)
+      except OSError as e:
+        if e.errno != errno.ENOENT:
+          raise
+
+      fd = os.open(self.storage_path,
+        os.O_CREAT | os.O_EXCL | os.O_WRONLY | os.O_TRUNC, 0600)
+      try:
+        os.write(fd, self.passwd)
+      finally:
+        os.close(fd)
+      if not self.create_once:
+        return self.storage_path
 
-    # Generate application configuration file
-    if self.options.get('template'):
-      application_conf = dict(mysql_database=self.options['mysql-database'],
-                              mysql_user=self.options['mysql-username'],
-                              mysql_password=self.options['mysql-password'],
-                              mysql_host='%s:%s' % (self.options['mysql-host'],
-                                                    self.options['mysql-port']),
-                              mysql_ip=self.options['mysql-host'],
-                              mysql_port=self.options['mysql-port'],
-                              secret_key=secret_key,
-                              ip='[%s]' % self.options['ip'],
-                              port=self.options['port'],
-                              # XXX-Cedric: add frontend url.
-                             )
-      # Allow to give custom parameters to template
-      application_parameter_prefix = 'application-'
-      for key in self.options.keys():
-        if key.startswith(application_parameter_prefix):
-          application_conf[key.lstrip(application_parameter_prefix)] = self.options[key]
-
-      directory, file_ = os.path.split(self.options['configuration'])
-
-      path = self.options['htdocs']
-      if directory:
-        path = os.path.join(path, directory)
-        if not os.path.exists(path):
-          os.makedirs(path)
-        if not os.path.isdir(path):
-          raise OSError("Cannot create %r." % path)
-
-      destination = os.path.join(path, file_)
-      config = self.createFile(destination,
-        self.substituteTemplate(self.options['template'], application_conf))
-      path_list.append(config)
-
-    #if os.path.exists(self.options['pid-file']):
-    #  # Reload apache configuration
-    #  with open(self.options['pid-file']) as pid_file:
-    #    pid = int(pid_file.read().strip(), 10)
-    #  try:
-    #    os.kill(pid, signal.SIGUSR1) # Graceful restart
-    #  except OSError:
-    #    pass
-    return path_list
+  def update(self):
+    return ()
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apachephp/template/apache.in` & `slapos.cookbook-1.0.92/slapos/recipe/lampgeneric/template/apache.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/README.generic_varnish.txt` & `slapos.cookbook-1.0.92/slapos/recipe/README.generic_varnish.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 generic_varnish
 ===============
 
 This recipe creates a varnish instance dedicated for ERP5 with a web checker[1]
 set up.
 
-How to Use
-==========
-
-On slap console, you can instanciate varnish like this:
+How to Use generic_varnish ?
+============================
 
-instance = request(
-  software_type='varnish',
-  partition_parameter_kw={
-     'backend-url':'https://[your_backend_address]:your_backend_port',
-     'web-checker-frontend-url':'http://www.example.com',
-     'web-checker-mail-address':'web-checker-result@example.com',
-     'web-checker-smtp-host':'mail.example.com',
-  }
-)
+On slap console, you can instanciate varnish like this::
+  
+  instance = request(
+    software_type='varnish',
+    partition_parameter_kw={
+       'backend-url':'https://[your_backend_address]:your_backend_port',
+       'web-checker-frontend-url':'http://www.example.com',
+       'web-checker-mail-address':'web-checker-result@example.com',
+       'web-checker-smtp-host':'mail.example.com',
+    }
+  )
 
 backend-url is the backend url that varnish will cache.
 
 web-checker-frontend-url is the entry-point-url that web checker will check
 the HTTP headers of all the pages in the web site.
 
 web-checker-mail-address is the email address where web checker will send
@@ -29,19 +29,14 @@
 
 web-checker-smtp-host is the smtp server to be used to send the web checker
 result.
 
 [Note]
 When web-checker-* parameters are not given, web_checker will be disabled.
 
-TODO
-====
-
-We need to merge this and apache_frontend recipe.
-
 References
 ==========
 
 [1] web_checker (it is a part of erp5.util)
 http://pypi.python.org/pypi/erp5.util
 web_checker: Web site HTTP Cache header checking tool
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apacheproxy/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/accords/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,52 +20,86 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
+import os
+import shutil
+from slapos.recipe.librecipe import GenericSlapRecipe
+import shutil
 import subprocess
+import sys
 
-from slapos.recipe.librecipe import GenericBaseRecipe
-
-class Recipe(GenericBaseRecipe):
-
-  def install(self):
+class Recipe(GenericSlapRecipe):
+  def _install(self):
     path_list = []
+    accords_location = self.buildout['accordsdirectory']['accords']
 
-    # Install apache
-    apache_config = dict(
-      pid_file=self.options['pid-file'],
-      lock_file=self.options['lock-file'],
-      ip=self.options['ip'],
-      port=self.options['port'],
-      error_log=self.options['error-log'],
-      access_log=self.options['access-log'],
-      backend_url=self.options['url'],
+    parameter_dict = dict(
+        userid=self.options['userid'],
+        tenantname=self.options['tenantname'],
+        password=self.options['password'],
+        domain=self.options['domain'],
+        openstack_url=self.options['openstack_url'],
+        python_location=sys.executable,
+        accords_location=accords_location,
+        manifest_name=self.options['manifest-name'],
+        # XXX this is workaround
+        accords_lib_directory=self.options['accords_lib_directory'],
+        computer_id = self.computer_id,
+        computer_partition_id = self.computer_partition_id,
+        server_url = self.server_url,
+        software_release_url = self.software_release_url,
+        key_file = self.key_file,
+        cert_file = self.cert_file,
+        path = '%s:%s' % (self.options['accords_bin_directory'],
+            os.environ.get('PATH', '')),
+    )
+    # Generate os-config.xml
+    os_config_file = self.createFile(self.options['os-config'],
+        self.substituteTemplate(self.getTemplateFilename('os_config.xml.in'),
+        parameter_dict))
+    path_list.append(os_config_file)
+
+    # Put modified accords configuration file
+    accords_configuration_parameter_dict = dict(
+        listen_ip = self.options['listen-ip']
     )
-    httpd_conf = self.createFile(self.options['httpd-conf'],
-      self.substituteTemplate(self.getTemplateFilename('apache.in'),
-                              apache_config)
+    accords_configuration_file_location = self.createFile(
+        self.options['accords-configuration-file'],
+        self.substituteTemplate(self.getTemplateFilename('accords.ini.in'),
+        accords_configuration_parameter_dict))
+    path_list.append(accords_configuration_file_location)
+
+    # XXX is it dangerous?
+    security_path = os.path.join(accords_location, 'security')
+    if os.path.exists(security_path):
+      shutil.rmtree(security_path)
+
+    # Initiate configuration
+    subprocess.check_call('./accords-config',
+                          cwd=accords_location
     )
-    path_list.append(httpd_conf)
 
-    wrapper = self.createWrapper(name=self.options['wrapper'],
-                                 command=self.options['httpd-binary'],
-                                 parameters=[
-                                     '-f',
-                                     self.options['httpd-conf'],
-                                     '-DFOREGROUND',
-                                     ])
-
-    path_list.append(wrapper)
-
-    subprocess.call([
-                        self.options['httpd-binary'],
-                        '-f',
-                        self.options['httpd-conf'],
-                        '-k',
-                        'graceful',
-                    ])
+    # Generate manifest
+    manifest_origin_location = self.options['manifest-source']
+    manifest_location = self.options['manifest-destination']
+
+    shutil.copy(manifest_origin_location, manifest_location)
+    path_list.append(manifest_location)
+
+    # Generate wrapper
+    wrapper_location = self.createPythonScript(self.options['accords-wrapper'],
+        __name__ + '.accords.runAccords',
+        (parameter_dict,))
+    path_list.append(wrapper_location)
+
+    # Generate helper for debug
+    self.createExecutable(
+        self.options['testos-wrapper'],
+        self.substituteTemplate(self.getTemplateFilename('testos.in'),
+            parameter_dict)
+    )
 
     return path_list
-
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apacheproxy/template/apache.in` & `slapos.cookbook-1.0.92/slapos/recipe/apacheproxy/template/apache.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/gitinit.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,29 +19,31 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
-#############################################################################
-
+##############################################################################
+import json
 import os
-import sys
-import zc.buildout
-from slapos.recipe.librecipe import BaseSlapRecipe
+
+from subprocess import check_call
+
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
-  def install(self):
 
-    runner = self.createPythonScript(
-      self.options['runner-path'],
-      __name__+'.testrunner.run',
-      arguments=[self.options['suite-url'],
-                 self.options['report-url'],
-                 self.options['report-project'],
-                 self.options['browser'],
-                 ])
+    def install(self):
 
-    return [runner]
+        repolist = json.loads(self.options['repos'])
+        for repo, desc in repolist.iteritems():
+            absolute_path = os.path.join(self.options['base-directory'], '%s.git' % repo)
+            if not os.path.exists(absolute_path):
+                check_call([self.options['git-binary'], 'init',
+                            '--bare', absolute_path])
+                # XXX: Hardcoded path
+                description_filename = os.path.join(absolute_path, 'description')
+                with open(description_filename, 'w') as description_file:
+                    description_file.write(desc)
 
+        return []
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/seleniumrunner/erp5functionaltestreporthandler.py` & `slapos.cookbook-1.0.92/slapos/recipe/xwiki/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,169 +19,150 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
-#############################################################################
-
-import re
-import urlparse
-import urllib
-import httplib
-import mimetools
-from random import randint
-import tempfile
+##############################################################################
+from slapos.recipe.librecipe import BaseSlapRecipe
 import os
-import stat
-import zipfile
-import mimetypes
-import datetime
-
-TB_SEP = "============================================================="\
-    "========="
-
-# REGEX FOR ZELENIUM TESTS
-TEST_PASS_RE = re.compile('<th[^>]*>Tests passed</th>\n\s*<td[^>]*>([^<]*)')
-TEST_FAILURE_RE = re.compile('<th[^>]*>Tests failed</th>\n\s*<td[^>]*>([^<]*)')
-IMAGE_RE = re.compile('<img[^>]*?>')
-TEST_ERROR_TITLE_RE = re.compile('(?:error.gif.*?>|title status_failed"><td[^>]*>)([^>]*?)</td></tr>', re.S)
-TEST_RESULT_RE = re.compile('<div style="padding-top: 10px;">\s*<p>\s*'
-                          '<img.*?</div>\s.*?</div>\s*', re.S)
-DURATION_RE = re.compile('<th[^>]*>Elapsed time \(sec\)</th>\n\s*<td[^>]*>([^<]*)')
-
-TEST_ERROR_RESULT_RE = re.compile('.*(?:error.gif|title status_failed).*', re.S)
-
-def get_content_type(f):
-  return mimetypes.guess_type(f.name)[0] or 'application/octet-stream'
-
-class ConnectionHelper:
-  def __init__(self, url):
-    self.conn = urlparse.urlparse(url)
-    if self.conn.scheme == 'http':
-      connection_type = httplib.HTTPConnection
-      if self.conn.port is None:
-        self.port = 80
-    else:
-      connection_type = httplib.HTTPSConnection
-      if self.conn.port is None:
-        self.port = 443
-    self.connection_type = connection_type
-
-  def _connect(self):
-    self.connection = self.connection_type(self.conn.hostname + ':' +
-        str(self.conn.port or self.port))
-
-  def POST(self, path, parameter_dict, file_list=None):
-    self._connect()
-    parameter_dict.update(__ac_name=self.conn.username,
-                          __ac_password=self.conn.password)
-    header_dict = {'Content-type': "application/x-www-form-urlencoded"}
-    if file_list is None:
-      body = urllib.urlencode(parameter_dict)
-    else:
-      boundary = mimetools.choose_boundary()
-      header_dict['Content-type'] = 'multipart/form-data; boundary=%s' % (
-          boundary,)
-      body = ''
-      for k, v in parameter_dict.iteritems():
-        body += '--%s\r\n' % boundary
-        body += 'Content-Disposition: form-data; name="%s"\r\n' % k
-        body += '\r\n'
-        body += '%s\r\n' % v
-      for name, filename in file_list:
-        f = open(filename, 'r')
-        body += '--%s\r\n' % boundary
-        body += 'Content-Disposition: form-data; name="%s"; filename="%s"\r\n'\
-                % (name, name)
-        body += 'Content-Type: %s\r\n' % get_content_type(f)
-        body += 'Content-Length: %d\r\n' % os.fstat(f.fileno())[stat.ST_SIZE]
-        body += '\r\n'
-        body += f.read()
-        f.close()
-        body += '\r\n'
-    self.connection.request("POST", self.conn.path + '/' + path,
-          body, header_dict)
-    self.response = self.connection.getresponse()
-
-
-class ERP5TestReportHandler:
-  def __init__(self, url, suite_name):
-    # random test id
-    self.test_id = "%s-%X" % (
-       ("%s" % datetime.date.today()).replace("-", ""),
-       randint(1, 10000000000000000),
-     )
-    self.connection_helper = ConnectionHelper(url)
-    self.suite_name = suite_name
-
-  def reportStart(self):
-    # report that test is running
-    print 'Starting test with id %s' % self.test_id
-    self.connection_helper.POST('TestResultModule_reportRunning', dict(
-      test_suite=self.suite_name,
-      test_report_id=self.test_id,
+import shutil
+import pkg_resources
+import subprocess
+import time
+import zc.buildout
+
+class Recipe(BaseSlapRecipe):
+
+  def _install(self):
+    self.requirements, self.ws = self.egg.working_set()
+    parameter_dict = self.computer_partition.getInstanceParameterDict()
+    ipv4 = self.getLocalIPv4Address()
+    ipv6 = self.getGlobalIPv6Address()
+
+    self.install_mysql_server_configuration(ipv4)
+
+    port = '8900'
+    tomcat_home = os.path.join(self.data_root_directory, 'tomcat')
+    tomcat_lib = os.path.join(tomcat_home, 'lib')
+    xwiki_home = os.path.join(tomcat_home, 'webapps', 'xwiki')
+    for src, dst in (
+        (self.options['tomcat_location'].strip(), tomcat_home),
+        (self.options['xwiki_location'].strip(), xwiki_home),
+        ):
+      if not os.path.isdir(dst):
+        try:
+          shutil.copytree(src, dst)
+        except:
+          shtuil.rmtree(dst)
+          raise
+
+    shutil.copy(self.options['jdbc_location'].strip(), os.path.join(tomcat_lib,
+      'jdbc.jar'))
+    # headless mode
+    self._writeFile(os.path.join(tomcat_home, 'bin', 'setenv.sh'), '''#!/bin/sh
+export JAVA_OPTS="${JAVA_OPTS} -Djava.awt.headless=true"
+''')
+    # tomcat wrapper
+    catalina = os.path.join(tomcat_home, 'bin', 'catalina.sh')
+    # solve "The BASEDIR environment variable is not defined correctly"
+    bindir = os.path.join(tomcat_home, 'bin')
+    for f in os.listdir(bindir):
+      if f.endswith('.sh'):
+        os.chmod(os.path.join(bindir, f), 0755)
+    tomcat_wrapper = self.createRunningWrapper('xwiki', """#!/bin/sh
+export JRE_HOME=%(java_home)s
+exec %(catalina)s run
+""" % dict(java_home=self.options['java_home'].strip(),
+  catalina = catalina))
+
+    tomcat_dict = dict(
+      http_address=ipv6,
+      http_port=port,
+      ajp_address=ipv4,
+      ajp_port="8009",
+        )
+    server_xml = os.path.join(tomcat_home, 'conf', 'server.xml')
+    self._writeFile(server_xml, pkg_resources.resource_string(__name__,
+      'template/tomcat-server.xml.in') % tomcat_dict)
+
+    hibernate_xml = os.path.join(tomcat_home, 'webapps', 'xwiki', 'WEB-INF', 'hibernate.cfg.xml')
+    self._writeFile(hibernate_xml, pkg_resources.resource_string(__name__,
+      'template/hibernate.cfg.xml.in') % dict(mysql_port='45678', mysql_ip = ipv4))
+
+    self.computer_partition.setConnectionDict(dict(
+      http_connection="http://[%s]:%s/xwiki/" % (ipv6, port),
       ))
+    return [server_xml, tomcat_wrapper]
+
+  def _initializeMysqlServer(self):
+    # XXX: Protect with proper root password
+    popen = subprocess.Popen([self.options['mysql_install_binary'],
+      '--skip-name-resolve', '--no-defaults',
+      '--datadir=%s' % self.data_directory],
+      stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+    result = popen.communicate()[0]
+    if popen.returncode is None or popen.returncode != 0:
+      message = """Failed to initialise server in %(data_directory)r.
+The error was: %(result)s""" % dict(data_directory=self.data_directory,
+        result=result)
+      raise zc.buildout.UserError(message)
+
+  def install_mysql_server_configuration(self, ip):
+    self.data_directory = os.path.join(self.data_root_directory,
+        'mysql_server')
+    self.configuration_file = os.path.join(self.etc_directory, 'my.cnf')
+    self._createDirectory(self.data_directory)
+    self.options['ip'] = ip
+    port = '45678'
+    self.options['tcp_port'] = port
+    self.options['data_directory'] = self.data_directory
+    self.options['pid_file'] = os.path.join(self.run_directory, 'mysqld.pid')
+    self.options['socket'] = os.path.join(self.run_directory, 'mysqld.sock')
+    self.options['error_log'] = os.path.join(self.log_directory, 'mysqld.log')
+    self.options['slow_query_log'] = os.path.join(self.log_directory,
+        'mysql-slow.log')
+    self._initializeMysqlServer()
+
+    mysql_conf_path = self.createConfigurationFile("my.cnf",
+        self.substituteTemplate(pkg_resources.resource_filename(__name__,
+          os.path.join('template', 'my.cnf.in')), self.options))
+    mysql_wrapper_path = self.createRunningWrapper('mysqld',
+        pkg_resources.resource_string(__name__, os.path.join('template',
+          'mysqld.bin')) % {'configuration_file': self.configuration_file,
+                        'real_binary': self.options['mysqld_binary']})
+
+    mysql_connection_dict = dict(
+        ip=ip,
+        port=port,
+        user='xwiki',
+        password='xwiki',
+        database='xwiki',
+        )
+    # XXX: Bad thing -- it is required to fill mysql with some data, but there
+    #      is no known any way to do it w/o running mysql (except rewriting
+    #      mysql_install_db)
+    mysqld = subprocess.Popen([mysql_wrapper_path],
+        stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+    try:
+      # XXX: Simplification of bad idea -- wait some time before connecting to
+      #      mysql
+      time.sleep(2)
+      mysql = subprocess.Popen([self.options['mysql_binary'].strip(),
+        '--no-defaults', '-B', '--user=root',
+        '--socket=%s' % self.options['socket'],
+        ], stdin=subprocess.PIPE, stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT)
+      result = mysql.communicate(pkg_resources.resource_string(__name__,
+        'template/initmysql.sql.in') % mysql_connection_dict)[0]
+      if mysql.returncode is None:
+        mysql.kill()
+      if mysql.returncode != 0:
+        raise zc.buildout.UserError('Issue during filling database, mysql '
+            'command result was: %s' % result)
+    finally:
+      mysqld.kill()
+    self.computer_partition.setConnectionDict(mysql_connection_dict)
+
+    return [mysql_conf_path, mysql_wrapper_path]
 
-  def reportFinished(self, out_file):
-    # make file parsable by erp5_test_results
-    out_file, success, failure, duration = self.processResult(out_file)
-
-    # XXX-Cedric : make correct display in test_result_module
-    tempcmd = tempfile.mkstemp()[1]
-    tempcmd2 = tempfile.mkstemp()[1]
-    tempout = tempfile.mkstemp()[1]
-    templog = tempfile.mkstemp()[1]
-    tl = open(templog, 'w')
-    tl.write(TB_SEP + '\n')
-    tl.write(out_file)
-
-    tl.write("----------------------------------------------------------------------\n")
-    tl.write('Ran 1 test in %.2fs\n' % duration)
-    if success:
-      tl.write('OK\n')
-    else:
-      tl.write('FAILED (failures=1)\n')
-    tl.write(TB_SEP + '\n')
-    tl.close()
-    open(tempcmd, 'w').write(""" %s""" % self.suite_name)
-    # create nice zip archive
-    tempzip = tempfile.mkstemp()[1]
-    # XXX-Cedric : support multiple tests
-    zip = zipfile.ZipFile(tempzip, 'w')
-    zip.write(tempout, '%s/001/stdout' % self.suite_name)
-    zip.write(templog, '%s/001/stderr' % self.suite_name)
-    zip.write(tempcmd, '%s/001/cmdline' % self.suite_name)
-    zip.close()
-    os.unlink(templog)
-    os.unlink(tempcmd)
-    os.unlink(tempout)
-    os.unlink(tempcmd2)
-
-    # post it to ERP5
-    self.connection_helper.POST('TestResultModule_reportCompleted',
-        dict(test_report_id=self.test_id), file_list=[('filepath', tempzip)])
-    os.unlink(tempzip)
-
-  def processResult(self, out_file):
-    file_content = out_file
-    sucess_amount = TEST_PASS_RE.search(file_content).group(1)
-    failure_amount = TEST_FAILURE_RE.search(file_content).group(1)
-    error_title_list = [re.compile('\s+').sub(' ', x).strip()
-                    for x in TEST_ERROR_TITLE_RE.findall(file_content)]
-    duration = DURATION_RE.search(file_content).group(1)
-    detail = ''
-    for test_result in TEST_RESULT_RE.findall(file_content):
-      if  TEST_ERROR_RESULT_RE.match(test_result):
-        detail += test_result
-
-    detail = IMAGE_RE.sub('', detail)
-    if detail:
-      detail = IMAGE_RE.sub('', detail)
-      detail = '''<html>
-<head>
- <style type="text/css">tr.status_failed { background-color:red };</style>
-</head>
-<body>%s</body>
-</html>''' % detail
-    return detail, int(sucess_amount), int(failure_amount), float(duration)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/pulse2/mysql.py` & `slapos.cookbook-1.0.92/slapos/recipe/lamp/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
   mysqld_wrapper_list = [conf['mysqld_binary'], '--defaults-file=%s' %
       conf['configuration_file']]
   # we trust mysql_install that if mysql directory is available mysql was
   # correctly initalised
   if not os.path.isdir(os.path.join(conf['data_directory'], 'mysql')):
     while True:
       # XXX: Protect with proper root password
-      # XXX: Follow http://dev.mysql.com/doc/refman/5.0/en/default-privileges.html
       popen = subprocess.Popen([conf['mysql_install_binary'],
         '--skip-name-resolve', '--no-defaults', '--datadir=%s' %
         conf['data_directory']],
         stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
       result = popen.communicate()[0]
       if popen.returncode is None or popen.returncode != 0:
         print "Failed to initialise server.\nThe error was: %s" % result
@@ -50,22 +49,24 @@
         print "Command %r failed with result:\n%s" % (mysql_upgrade_list, result)
         print 'Sleeping for %ss and retrying' % sleep
       else:
         if mysql_upgrade.returncode == 0:
           print "MySQL database upgraded with result:\n%s" % result
         else:
           print "No need to upgrade MySQL database"
-        mysql_list = [conf['mysql_binary'].strip(), '--no-defaults', '-B', '--user=root', '--socket=%s' % conf['socket']]
-        mysql = subprocess.Popen(mysql_list, stdin=subprocess.PIPE,
-            stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        result = mysql.communicate(conf['mysql_script'])[0]
-        if mysql.returncode is None:
-          mysql.kill()
-        if mysql.returncode != 0:
-          print 'Command %r failed with:\n%s' % (mysql_list, result)
-          print 'Sleeping for %ss and retrying' % sleep
-        else:
-          is_succeed = True
-          print 'SlapOS initialisation script succesfully applied on database.'
+        mysql_script = conf.get('mysql_script')
+        if mysql_script:
+          mysql_list = [conf['mysql_binary'].strip(), '--no-defaults', '-B', '--user=root', '--socket=%s' % conf['socket']]
+          mysql = subprocess.Popen(mysql_list, stdin=subprocess.PIPE,
+              stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+          result = mysql.communicate(conf['mysql_script'])[0]
+          if mysql.returncode is None:
+            mysql.kill()
+          if mysql.returncode != 0:
+            print 'Command %r failed with:\n%s' % (mysql_list, result)
+            print 'Sleeping for %ss and retrying' % sleep
+          else:
+            is_succeed = True
+            print 'SlapOS initialisation script succesfully applied on database.'
     sys.stdout.flush()
     sys.stderr.flush()
     time.sleep(sleep)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/pulse2/template/my.cnf.in` & `slapos.cookbook-1.0.92/slapos/recipe/lamp/template/my.cnf.in`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 skip-show-database
 port = %(tcp_port)s
 bind-address = %(ip)s
 socket = %(socket)s
 datadir = %(data_directory)s
 pid-file = %(pid_file)s
 log-error = %(error_log)s
-log-slow-file = %(slow_query_log)s
+slow_query_log
+slow_query_log_file = %(slow_query_log)s
 long_query_time = 5
 max_allowed_packet = 128M
 query_cache_size = 32M
 
-plugin-load = ha_innodb_plugin.so
+plugin-load = ha_mroonga.so
 
 # The following are important to configure and depend a lot on to the size of
 # your database and the available resources.
 #innodb_buffer_pool_size = 4G
 #innodb_log_file_size = 256M
 #innodb_log_buffer_size = 8M
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/pulse2/apache.py` & `slapos.cookbook-1.0.92/slapos/recipe/lamp/apache.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5scalabilitytestbed/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/erp5scalabilitytestbed/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/_uuid.py` & `slapos.cookbook-1.0.92/slapos/recipe/_uuid.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/request.py` & `slapos.cookbook-1.0.92/slapos/recipe/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,35 +156,53 @@
           filter_kw=filter_kw, shared=slave, state=requested_state)
       return_parameter_dict = self._getReturnParameterDict(self.instance,
           return_parameters)
       # Fetch the instance-guid and the instance-state
       # Note: SlapOS Master does not support it for slave instances
       if not slave:
         try:
-          options['instance-guid'] = self.instance.getInstanceGuid()
+          options['instance-guid'] = self.instance.getInstanceGuid() \
+              .encode('UTF-8')
           # XXX: deprecated, to be removed
-          options['instance_guid'] = self.instance.getInstanceGuid()
+          options['instance_guid'] = options['instance-guid']
           options['instance-state'] = self.instance.getState()
           options['instance-status'] = self.instance.getStatus()
         except (slapmodule.ResourceNotReady, AttributeError):
           # Backward compatibility. Old SlapOS master and core don't know this.
           self.logger.warning("Impossible to fetch instance GUID nor state.")
     except (slapmodule.NotFoundError, slapmodule.ServerError, slapmodule.ResourceNotReady) as exc:
+      self.logger.warning(
+        'Request for %(request_name)r with software release '
+        '%(software_release)r and software type %(software_type)r failed '
+        'with partition_parameter_kw=%(partition_parameter_kw)r, '
+        'filter_kw=%(filter_kw)r, shared=%(shared)r, state=%(state)r.', dict(
+          software_release=software_url,
+          software_type=software_type,
+          request_name=name,
+          partition_parameter_kw=partition_parameter_kw,
+          filter_kw=filter_kw,
+          shared=slave,
+          state=requested_state
+        )
+      )
       self._raise_request_exception = exc
       self._raise_request_exception_formatted = traceback.format_exc()
       return_parameter_dict = {}
 
     # Then try to get all the parameters. In case of problem, put empty string.
     for param in return_parameters:
-      options['connection-%s' % param] = ''
+      value = ''
       try:
-        options['connection-%s' % param] = return_parameter_dict[param]
+        value = return_parameter_dict[param]
       except KeyError:
         if self.failed is None:
           self.failed = param
+      if isinstance(value, unicode):
+        value = value.encode('UTF-8')
+      options['connection-%s' % param] = value
 
   def _filterForStorage(self, partition_parameter_kw):
     return partition_parameter_kw
 
   def _getReturnParameterDict(self, instance, return_parameter_list):
     result = {}
     for param in return_parameter_list:
@@ -245,25 +263,35 @@
           'Requested instance is currently %s. If this error persists, '\
           'check status of this instance.' % (self.failed, status)
       self.logger.warning(error_message)
     return []
 
   update = install
 
-class Serialised(Recipe):
+class JSONCodec(object):
   def _filterForStorage(self, partition_parameter_kw):
     return wrap(partition_parameter_kw)
 
   def _getReturnParameterDict(self, instance, return_parameter_list):
     try:
       return json.loads(instance.getConnectionParameter(JSON_SERIALISED_MAGIC_KEY))
     except slapmodule.NotFoundError:
       return {}
 
+class RequestJSONEncoded(JSONCodec, Recipe):
+  """
+  Like Recipe, but serialised with JSONCodec.
+  """
+  pass
 
+class RequestOptionalJSONEncoded(JSONCodec, RequestOptional):
+  """
+  Like RequestOptional, but serialised with JSONCodec.
+  """
+  pass
 
 
 CONNECTION_PARAMETER_STRING = 'connection-'
 
 class RequestEdge(Recipe):
   """
   For each country in country-list, do a request.
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/zero_knowledge.py` & `slapos.cookbook-1.0.92/slapos/recipe/zero_knowledge.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,62 +32,70 @@
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 
 class WriteRecipe(GenericBaseRecipe):
   """
   """
   def __init__(self, buildout, name, options):
-    if not "filename" in options:
-      raise zc.buildout.UserError("You have to provide the parameter \"filename\"")
+    if not "filename" in options and not "file-path" in options:
+      raise zc.buildout.UserError("You have to provide the parameter either \"filename\" or \"file-path\"")
 
-    self.filename = options['filename'].strip()
-    self.path = os.path.join(buildout['buildout']['directory'], self.filename)
+    self._options = options.copy()
+    if options.get('filename'):
+      self.filename = options['filename'].strip()
+      self.path = os.path.join(buildout['buildout']['directory'], self.filename)
+      del self._options['filename']
+    else:
+      self.path = options['file-path'].strip()
+      del self._options['file-path']
+    del self._options['recipe']
     self.name = name
-    self.options = options.copy()
-    del self.options['filename']
-    del self.options['recipe']
+
+  def install(self):
 
     # Set up the parser, and write config file if needed
     self.parser = ConfigParser.ConfigParser()
     try:
       self.parser.read(self.path)
       #clean_options(options)
-      for key in self.options:
+      for key in self._options:
         if key not in self.parser.options(self.name):
-          self.parser.set(self.name, key, self.options[key])
+          self.parser.set(self.name, key, self._options[key])
       with open(self.path, 'w') as file:
         self.parser.write(file)
     # If the file or section do not exist
     except (ConfigParser.NoSectionError, IOError) as e:
       self.full_install()
 
-  install = update = lambda self: []
-
   def full_install(self):
     """XXX-Nicolas : when some parameter's value is changed in
     buildout profile, this will override custom user defined values"""
     self.parser.read(self.path)
     if self.parser.has_section(self.name):
       self.parser.remove_section(self.name)
     self.parser.add_section(self.name)
-    for key in self.options:
-      self.parser.set(self.name, key, self.options[key])
+    for key in self._options:
+      self.parser.set(self.name, key, self._options[key])
     with open(self.path, 'w') as file:
       self.parser.write(file)
 
+  update = install
 
 class ReadRecipe(GenericBaseRecipe):
   """
   """
   def __init__(self, buildout, name, options):
-    if not "filename" in options:
-      raise zc.buildout.UserError("You have to provide the parameter \"filename\"")
+    if not "filename" in options and not "file-path" in options:
+      raise zc.buildout.UserError("You have to provide the parameter either \"filename\" or file-path")
 
-    self.filename = options['filename'].strip()
-    self.path = os.path.join(buildout['buildout']['directory'], self.filename)
+    if options.get('filename'):
+      self.filename = options['filename'].strip()
+      self.path = os.path.join(buildout['buildout']['directory'], self.filename)
+    else:
+      self.path = options['file-path'].strip()
 
     # Set up the parser, and write config file if needed
     self.parser = ConfigParser.ConfigParser()
     if os.path.exists(self.path):
       self.parser.read(self.path)
       for section in self.parser.sections():
         for key ,value in self.parser.items(section):
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/publish.py` & `slapos.cookbook-1.0.92/slapos/recipe/publish.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,35 +27,36 @@
 import zc.buildout
 from slapos.recipe.librecipe import wrap
 from slapos.recipe.librecipe import GenericSlapRecipe
 
 CONNECTION_PARAMETER_STRING = 'connection-'
 
 class Recipe(GenericSlapRecipe):
-  def _install(self):
-    publish_dict = {}
-    done = set()
+  def __init__(self, buildout, name, options):
+    super(Recipe, self).__init__(buildout, name, options)
+    # Tell buildout about the sections we will access during install.
+    self._extend_set = done = set()
     extends = [self.name]
     while extends:
-        name = extends.pop()
-        done.add(name)
-        for k, v in self.buildout[name].iteritems():
-          if k[:1] == '-':
-            if k == '-extends':
-              extends += set(v.split()) - done
-          elif k != 'recipe':
-            publish_dict[k] = v
+      name = extends.pop()
+      done.add(name)
+      extends += set(self.buildout[name].get('-extends', '').split()) - done
+
+  def _install(self):
+    publish_dict = {}
+    for name in self._extend_set:
+      for k, v in self.buildout[name].iteritems():
+        if k != 'recipe' and not k.startswith('-'):
+          publish_dict[k] = v
     self._setConnectionDict(publish_dict, self.options.get('-slave-reference'))
     return []
 
   def _setConnectionDict(self, publish_dict, slave_reference=None):
     return self.setConnectionDict(publish_dict, slave_reference)
 
-SERIALISED_MAGIC_KEY = '_'
-
 class Serialised(Recipe):
   def _setConnectionDict(self, publish_dict, slave_reference=None):
     return super(Serialised, self)._setConnectionDict(wrap(publish_dict), slave_reference)
 
 
 
 class PublishSection(GenericSlapRecipe):
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/lockfile.py` & `slapos.cookbook-1.0.92/slapos/recipe/switch_softwaretype.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,63 @@
 ##############################################################################
 #
-# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2014 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
-# guarantees and support are strongly adviced to contract a Free Software
+# guarantees and support are strongly advised to contract a Free Software
 # Service Company
 #
 # This program is Free Software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
-# Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.
 #
 ##############################################################################
-import os
-import sys
-import subprocess
 
-import inotifyx
+import os, subprocess, sys
 
-from slapos.recipe.librecipe import GenericBaseRecipe
+class Recipe:
 
-class LockFile(object):
+  def __init__(self, buildout, name, options):
+    self.buildout = buildout
+    self.options = options
+    self.name = name
+    self.software_type = buildout["slap-configuration"]["slap-software-type"]
+    section, key = self.options[self.software_type].split(":")
+    self.base = self.buildout[section][key]
 
-  class LockException(Exception):
-    pass
-
-  def __init__(self, filename, wait=True, exit=False):
-    self.filename = filename
-    if wait:
-      self.callback = lambda: self.waitDeletion()
-    elif not exit:
-      self.callback = lambda: self.raiseException()
-    else:
-      self.callback = lambda: sys.exit(1)
-
-  def raiseException(self):
-    raise LockFile.LockException("Not able to lock the file")
-
-  def waitDeletion(self):
-    inotify_fd = inotifyx.init()
-    try:
-      inotifyx.add_watch(inotify_fd, self.filename, inotifyx.IN_DELETE)
-      inotifyx.get_events(inotify_fd)
-    except IOError: # add_watch failed
-      pass
-    finally:
-      os.close(inotify_fd)
-
-    self.__enter__()
-
-  def __enter__(self):
+  def install(self):
+    # XXX-Antoine: We gotta find a better way to do this. I tried to check
+    # out how slapgrid-cp was running buildout. But it is worse than that.
+    args = sys.argv[:]
+    for x in self.buildout["slap-connection"].iteritems():
+      args.append("slap-connection:%s=%s" % x)
+    for x in "directory", "eggs-directory", "develop-eggs-directory":
+      args.append("buildout:%s=%s" % (x, self.buildout["buildout"][x]))
+    args.append("buildout:installed=.installed-%s.cfg" % self.name)
+    # Options.get (from zc.buildout) should deserialize.
     try:
-      # Atomic file acquisition
-      self._fd = os.open(self.filename, os.O_CREAT | os.O_EXCL)
-    except OSError:
-      self.callback()
-
-  def __exit__(self, exc_type, exc_value, traceback):
-    os.close(self._fd)
-    os.unlink(self.filename)
-
-def locked_run(args):
-  with LockFile(args['filename'], wait=args['wait'], exit=True):
-    subprocess.check_call([args['binary']])
-
-class Recipe(GenericBaseRecipe):
+      override = self.options["override"][self.software_type]
+    except (KeyError, TypeError):
+      buildout = self.base
+    else:
+      # unfortunately, buildout:extends does not work when given at command line
+      buildout = os.path.join(self.buildout["buildout"]["parts-directory"],
+                              self.name + ".cfg")
+      with open(override) as src, open(buildout, "w", 0) as dst:
+        dst.write("[buildout]\nextends = %s\n\n" % self.base + src.read())
+    subprocess.check_call(args + ["-oc", buildout])
+    return []
 
-  def install(self):
-    wrapper = self.createPythonScript(self.options['wrapper'],
-                                      __name__ + '.locked_run',
-                                      dict(
-                                        filename=self.options['lock-file'],
-                                        wait=self.optionIsTrue('wait', False),
-                                        binary=self.options['binary'],
-                                      )
-                                     )
-    return [wrapper]
+  update = install
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/equeue.py` & `slapos.cookbook-1.0.92/slapos/recipe/tidstorage/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,33 +20,33 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
+import os
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
-
   def install(self):
+    configuration_file = self.createFile(
+      self.options['configuration-path'],
+      self.substituteTemplate(
+        self.getTemplateFilename('tidstorage.py.in'), self.options))
+    r = [configuration_file]
+
+    wrapper = self.options.get('tidstorage-wrapper')
+    wrapper and r.append(self.createWrapper(wrapper,
+      (self.options['tidstoraged-binary'],
+        '--nofork', '--config', configuration_file)))
+
+    r.append(self.createWrapper(
+      self.options['repozo-wrapper'],
+      (self.options['tidstorage-repozo-binary'],
+        '--config', configuration_file,
+        '--repozo', self.options['repozo-binary'],
+        '--gzip',
+        '--quick',
+       )))
 
-    parameters = [
-      '--database', self.options['database'],
-      '--logfile', self.options['log'],
-      '--lockfile', self.options['lockfile']
-    ]
-
-    if 'takeover-triggered-file-path' in self.options:
-      parameters.extend(['--takeover-triggered-file-path', self.options['takeover-triggered-file-path']])
-
-    if 'loglevel' in self.options:
-      parameters.extend(['--loglevel', self.options['loglevel']])
-
-    parameters.append(self.options['socket'])
-
-    wrapper = self.createWrapper(name=self.options['wrapper'],
-                                 command=self.options['equeue-binary'],
-                                 parameters=parameters)
-
-    return [wrapper]
-
+    return r
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/simplehttpserver/simplehttpserver.py` & `slapos.cookbook-1.0.92/slapos/recipe/simplehttpserver/simplehttpserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
       if exception.errno != errno.EEXIST:
         logging.error('Failed to create file in %s. The error is \n%s' % (
           file_path, str(exception)))
 
     logging.info('Writing recieved content to file %s' % file_path)
     try:
       with open(file_path, method) as myfile:
-        myfile.write(content.decode('utf-8'))
+        myfile.write(content)
         logging.info('Done.')
     except IOError as e:
       logging.error('Something happened while processing \'writeFile\'. The message is %s' %
                     str(e))
 
 class HTTPServerV6(HTTPServer):
   address_family = socket.AF_INET6
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/simplehttpserver/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/simplehttpserver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,13 +64,12 @@
       'cwd': self.options['base-path'],
       'log-file': self.options['log-file'],
       'cert-file': self.options.get('cert-file', ''),
       'key-file': self.options.get('key-file', ''),
       'root-dir': self.options['root-dir']
     }
 
-    server = self.createPythonScript(
+    return self.createPythonScript(
         self.options['wrapper'].strip(),
-        '%s.simplehttpserver.run' % __name__, parameters
+        __name__ + '.simplehttpserver.run',
+        (parameters,)
       )
-
-    return [server]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/copyfilelist.py` & `slapos.cookbook-1.0.92/slapos/recipe/copyfilelist.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/sshkeys_authority.py` & `slapos.cookbook-1.0.92/slapos/recipe/sshkeys_authority.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,37 +29,44 @@
 import os
 import subprocess
 import re
 
 from slapos.recipe.librecipe import GenericBaseRecipe
 from slapos.recipe.librecipe.inotify import subfiles
 
-# This authority only works with dropbear sshkey generator
-def sshkeys_authority(args):
-  requests_directory = args['requests']
-  keygen_binary = args['sshkeygen']
+# This authority only works with dropbear or openssh sshkey generators
+def sshkeys_authority(request_directory, keygen_binary):
+  if 'openssh' in keygen_binary:
+    authority_type = 'openssh'
+  else:
+    # Keep dropbear for compatibility
+    authority_type = 'dropbear'
 
-  for request_filename in subfiles(requests_directory):
+  for request_filename in subfiles(request_directory):
 
     with open(request_filename) as request_file:
       request = json.load(request_file)
 
     key_type = request.get('type', 'rsa')
-    size = str(request.get('size', 2048))
+    size = str(request.get('size', 4096))
     try:
       private_key = request['private_key']
       public_key = request['public_key']
     except KeyError:
       break
 
     if not os.path.exists(private_key):
       if os.path.exists(public_key):
         os.unlink(public_key)
-      keygen_cmd = [keygen_binary, '-t', key_type, '-f', private_key,
-                    '-s', size]
+      if authority_type == 'openssh':
+        keygen_cmd = [keygen_binary, '-N', "", '-C', "", '-t', key_type,
+                      '-f', private_key, '-b', size]
+      else:
+        keygen_cmd = [keygen_binary, '-t', key_type, '-f', private_key,
+                      '-s', size]
       # If the keygeneration return an non-zero status, it means there's a
       # big problem. Let's exit in this case
       subprocess.check_call(keygen_cmd, env=os.environ.copy())
 
     if not os.path.exists(public_key):
       keygen_cmd = [keygen_binary, '-f', private_key, '-y']
 
@@ -84,26 +91,21 @@
           public_key_value = matchresult.group(0)
           break
 
       with open(public_key, 'w') as public_key_file:
         public_key_file.write(public_key_value)
 
 
-
 class Recipe(GenericBaseRecipe):
 
   def install(self):
-    args = dict(
-      requests=self.options['request-directory'],
-      sshkeygen=self.options['keygen-binary'],
-    )
-
-    wrapper = self.createPythonScript(self.options['wrapper'],
-      __name__ + '.sshkeys_authority', args)
-    return [wrapper]
+    return self.createPythonScript(self.options['wrapper'],
+      __name__ + '.sshkeys_authority',
+      (self.options['request-directory'],
+       self.options['keygen-binary']))
 
 class Request(GenericBaseRecipe):
 
   def _options(self, options):
     if 'name' not in options:
       options['name'] = self.name
 
@@ -146,15 +148,13 @@
       elif os.path.exists(link):
         raise OSError("%r should be a symbolic link." % link)
 
     os.symlink(self.public_key, public_key_link)
     os.symlink(self.private_key, private_key_link)
     # end-XXX
 
-    wrapper = self.createPythonScript(
+    wrapper = self.createWrapper(
       self.options['wrapper'],
-      'slapos.recipe.librecipe.execute.execute_wait',
-      [ [self.options['executable']],
-        [self.private_key, self.public_key] ])
-
+      (self.options['executable'],),
+      wait_list=(self.private_key, self.public_key))
 
     return [request_file, wrapper, public_key_link, private_key_link]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5_bootstrap/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/shell.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2012-2014 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,40 +20,23 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-
+import os
+import json
 from slapos.recipe.librecipe import GenericBaseRecipe
-import sys
-import urlparse
 
 class Recipe(GenericBaseRecipe):
-  """
-  Instanciate ERP5 in Zope
-  """
 
   def install(self):
-    mysql = urlparse.urlsplit(self.options['mysql-url'])
-    zope = urlparse.urlsplit(self.options['zope-url'])
-    # Note: raises when there is more than a single element in path, as it's
-    # not supported by manage_addERP5Site anyway.
-    _, zope_path = zope.path.split('/')
-    return [self.createExecutable(
-      self.options['runner-path'],
-      self.substituteTemplate(
-        self.getTemplateFilename('erp5_bootstrap.in'),
-        {
-          'python_path': sys.executable,
-          'base_url': urlparse.urlunsplit((zope.scheme, zope.netloc, '', '', '')),
-          'site_id': zope_path,
-          'sql_connection_string': '%(database)s@%(hostname)s:%(port)s %(username)s %(password)s' % {
-            'database': mysql.path.split('/')[1],
-            'hostname': mysql.hostname,
-            'port': mysql.port,
-            'username': mysql.username,
-            'password': mysql.password
-          },
-        },
-    ))]
+    ps1 = self.options.get('ps1')
+    shell = self.options['shell']
+    env = {
+      'HOME': self.options['home'],
+      'PATH': ':'.join(self.options['path'].split('\n')),
+      'PS1': str(json.loads(ps1)) if ps1 else os.getenv('PS1', '> '),
+      'SHELL': shell,
+    }
+    return self.createWrapper(self.options['wrapper'], (shell,), env)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apache_zope_backend/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/stunnel/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,81 +20,77 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
+import os
+import signal
+import errno
+
 from slapos.recipe.librecipe import GenericBaseRecipe
-import pkg_resources
+
+def kill(pid_file, sig=signal.SIGUSR1):
+  if os.path.exists(pid_file):
+    with open(pid_file) as f:
+      pid = int(f.read().strip())
+    try:
+      os.kill(pid, sig)
+    except OSError, e:
+      if e.errno != errno.ESRCH: # No such process
+        raise e
+      os.unlink(pid_file)
 
 class Recipe(GenericBaseRecipe):
+
   def install(self):
-    try:
-      backend_list = self.options['backend-list']
-    except KeyError:
-      backend_list = [(self.options['port'], self.options['backend'])]
-
-    scheme = self.options['scheme']
-    if scheme == 'http':
-      required_path_list = []
-      ssl_enable = ssl_snippet = ''
-    elif scheme == 'https':
-      key = self.options['key-file']
-      certificate = self.options['cert-file']
-      required_path_list = [key, certificate]
-      ssl_snippet = self.substituteTemplate(self.getTemplateFilename('snippet.ssl.in'), {
-        'key': key,
-        'certificate': certificate,
-        'ssl_session_cache': self.options['ssl-session-cache'],
-      })
-      if 'ssl-authentication' in self.options and self.optionIsTrue(
-          'ssl-authentication'):
-        ssl_snippet += self.substituteTemplate(self.getTemplateFilename('snippet.ssl.ca.in'), {
-          'ca_certificate': self.options['ssl-authentication-certificate'],
-          'ca_crl': self.options['ssl-authentication-crl'],
-        })
-      ssl_enable = 'SSLEngine on'
+    path_list = []
+
+    self.isClient = self.optionIsTrue('client', default=False)
+    if self.isClient:
+      self.logger.info("Client mode")
     else:
-      raise ValueError('Unsupported scheme %s' % scheme)
+      self.logger.info("Server mode")
+
+    conf = {}
+
+    for type_ in ['remote', 'local']:
+      for data in ['host', 'port']:
+        confkey, opt = ['%s%s%s' % (type_, i, data) for i in ['_', '-']]
+        conf[confkey] = self.options[opt]
+
+    pid_file = self.options['pid-file']
+    conf.update(pid_file=pid_file)
 
-    ip_list = self.options['ip']
-    if isinstance(ip_list, basestring):
-      ip_list = [ip_list]
-    backend_path = self.options.get('backend-path', '/')
-    vhost_template_name = self.getTemplateFilename('vhost.in')
-    apache_config_file = self.createFile(
-      self.options['configuration-file'],
-      self.substituteTemplate(
-        self.getTemplateFilename('apache.zope.conf.in'),
-        {
-          'path': '/',
-          'server_admin': 'admin@',
-          'pid_file': self.options['pid-file'],
-          'lock_file': self.options['lock-file'],
-          'error_log': self.options['error-log'],
-          'access_log': self.options['access-log'],
-          'access_control_string': self.options['access-control-string'],
-          'ssl_snippet': ssl_snippet,
-          'vhosts': ''.join(self.substituteTemplate(vhost_template_name, {
-            'ip': ip,
-            'port': port,
-            'backend': ('%s/%s' % (backend.rstrip('/'), backend_path.strip('/'))).rstrip('/'),
-            'ssl_enable': ssl_enable,
-          }) for (port, backend) in backend_list for ip in ip_list),
-        },
-      )
+    log_file = self.options['log-file']
+    conf.update(log=log_file)
+
+    if self.isClient:
+      template = self.getTemplateFilename('client.conf.in')
+
+    else:
+      template = self.getTemplateFilename('server.conf.in')
+      key = self.options['key-file']
+      cert = self.options['cert-file']
+      conf.update(key=key, cert=cert)
+
+    conf_file = self.createFile(
+      self.options['config-file'],
+      self.substituteTemplate(template, conf))
+    path_list.append(conf_file)
+
+    wrapper = self.createWrapper(
+      self.options['wrapper'],
+      (self.options['stunnel-binary'], conf_file),
     )
-    return [
-      apache_config_file,
-      self.createPythonScript(
-        self.options['wrapper'],
-        __name__ + '.apache.runApache',
-        [
-          {
-            'required_path_list': required_path_list,
-            'binary': self.options['apache-binary'],
-            'config': apache_config_file,
-          },
-        ],
-      ),
-    ]
+    path_list.append(wrapper)
+
+    # Reload configuration
+    kill(pid_file, signal.SIGHUP)
+
+    if 'post-rotate-script' in self.options:
+      path_list.append(self.createPythonScript(
+        self.options['post-rotate-script'],
+        __name__ + '.kill', (pid_file,)))
+
+    return path_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/addresiliency/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/addresiliency/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,30 +34,22 @@
         scripts on the partition.
 
         bin/takeover will perform a rename (must be run manually).
         bin/bully will monitor, run elections and perform renames when needed.
     """
 
     def _install(self):
-        path_list = []
-
         slap_connection = self.buildout['slap-connection']
 
-        takeover_wrapper = self.createPythonScript(
-            name=self.options['wrapper-takeover'],
-            absolute_function='slapos.recipe.addresiliency.takeover.run',
-            arguments={
+        return self.createPythonScript(
+            self.options['wrapper-takeover'],
+            __name__ + '.takeover.takeover',
+            kw={
                 'server_url': slap_connection['server-url'],
                 'key_file': slap_connection.get('key-file'),
                 'cert_file': slap_connection.get('cert-file'),
-                'computer_id': slap_connection['computer-id'],
+                'computer_guid': slap_connection['computer-id'],
                 'partition_id': slap_connection['partition-id'],
-                'software': slap_connection['software-release-url'],
+                'software_release': slap_connection['software-release-url'],
                 'namebase': self.parameter_dict['namebase'],
                 'takeover_triggered_file_path': self.options['takeover-triggered-file-path'],
             })
-
-        path_list.append(takeover_wrapper)
-
-        return path_list
-
-
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/addresiliency/takeover.py` & `slapos.cookbook-1.0.92/slapos/recipe/addresiliency/takeover.py`

 * *Files 17% similar despite different names*

```diff
@@ -74,18 +74,7 @@
   cp_winner.bang(message='partitions have been renamed!')
   # Note: Root instance will reconfigure itself the winning instance (software_type
   # and parameters.)
 
   # Create "lock" file preventing equeue to run import scripts
   # XXX hardcoded
   open(takeover_triggered_file_path, 'w').write('')
-
-def run(args):
-  slapos.recipe.addresiliency.takeover.takeover(server_url = args.pop('server_url'),
-                                                key_file = args.pop('key_file'),
-                                                cert_file = args.pop('cert_file'),
-                                                computer_guid = args.pop('computer_id'),
-                                                partition_id = args.pop('partition_id'),
-                                                software_release = args.pop('software'),
-                                                namebase = args.pop('namebase'),
-                                                takeover_triggered_file_path = args.pop('takeover_triggered_file_path'))
-
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/slapreport/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/_urlparse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,27 +20,33 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
+from urlparse import urlparse
 
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
 
-  def install(self):
-    options = self.options
-    script = self.createWrapper(name=options['path'],
-                                command=options['slapreport-path'],
-                                parameters=[
-                                    options['pid-file'],
-                                    options['consumption-log-path'],
-                                    options['database-path'],
-                                    options['logbox-ip'],
-                                    options['logbox-port'],
-                                    options['logbox-user'],
-                                    options['logbox-passwd'],
-                                    ])
-    return [script]
+  def _options(self, options):
+    url = urlparse(options['url'])
+
+    def to_str(data):
+      if data is None:
+        return ''
+      return str(data)
 
+    options.update(scheme=url.scheme,
+                   username=to_str(url.username),
+                   password=to_str(url.password),
+                   host=to_str(url.hostname),
+                   port=to_str(url.port),
+                   path=url.path.strip('/'),
+                   params=url.params,
+                   query=url.query,
+                   fragment=url.fragment)
+
+  def install(self):
+    return []
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/readline.py` & `slapos.cookbook-1.0.92/slapos/recipe/readline.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/lamp/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/lamp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,13 +294,13 @@
       self.getTemplateFilename('stunnel.conf.in'), {
         'log': os.path.join(self.log_directory, 'stunnel.log'),
         'pid_file': os.path.join(self.run_directory, 'stunnel.pid'),
         'remote_host': remote_host, 'remote_port': remote_port,
         'local_host': local_host, 'local_port': local_port,
       }))
     wrapper = zc.buildout.easy_install.scripts([('stunnel',
-      'slapos.recipe.librecipe.execute', 'execute')], self.ws,
-      sys.executable, self.wrapper_directory, arguments=[
-        self.options['stunnel_binary'].strip(), stunnel_conf_path]
+      'slapos.recipe.librecipe.execute', 'generic_exec')], self.ws,
+      sys.executable, self.wrapper_directory, arguments='%r, %r'
+        % (self.options['stunnel_binary'].strip(), stunnel_conf_path)
       )[0]
     self.path_list.append(wrapper)
     return (local_host, local_port,)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/lamp/runner.py` & `slapos.cookbook-1.0.92/slapos/recipe/lamp/runner.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/lamp/mysql.py` & `slapos.cookbook-1.0.92/slapos/recipe/mysql/mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 import subprocess
 import time
 import sys
 
 
-def runMysql(args):
+def runMysql(conf):
   sleep = 60
-  conf = args[0]
   mysqld_wrapper_list = [conf['mysqld_binary'], '--defaults-file=%s' %
       conf['configuration_file']]
   # we trust mysql_install that if mysql directory is available mysql was
   # correctly initalised
   if not os.path.isdir(os.path.join(conf['data_directory'], 'mysql')):
     while True:
       # XXX: Protect with proper root password
+      # XXX: Follow http://dev.mysql.com/doc/refman/5.0/en/default-privileges.html
       popen = subprocess.Popen([conf['mysql_install_binary'],
-        '--skip-name-resolve', '--no-defaults', '--datadir=%s' %
-        conf['data_directory']],
-        stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        '--skip-name-resolve', '--skip-host-cache', '--no-defaults',
+        '--datadir=%s' % conf['data_directory']],
+        stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=conf['cwd'])
       result = popen.communicate()[0]
       if popen.returncode is None or popen.returncode != 0:
         print "Failed to initialise server.\nThe error was: %s" % result
         print "Waiting for %ss and retrying" % sleep
         time.sleep(sleep)
       else:
         print "Mysql properly initialised"
@@ -30,16 +30,15 @@
     print "MySQL already initialised"
   print "Starting %r" % mysqld_wrapper_list[0]
   sys.stdout.flush()
   sys.stderr.flush()
   os.execl(mysqld_wrapper_list[0], *mysqld_wrapper_list)
 
 
-def updateMysql(args):
-  conf = args[0]
+def updateMysql(conf):
   sleep = 30
   is_succeed = False
   while True:
     if not is_succeed:
       mysql_upgrade_list = [conf['mysql_upgrade_binary'], '--no-defaults', '--user=root', '--socket=%s' % conf['socket']]
       mysql_upgrade = subprocess.Popen(mysql_upgrade_list, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
       result = mysql_upgrade.communicate()[0]
@@ -49,24 +48,22 @@
         print "Command %r failed with result:\n%s" % (mysql_upgrade_list, result)
         print 'Sleeping for %ss and retrying' % sleep
       else:
         if mysql_upgrade.returncode == 0:
           print "MySQL database upgraded with result:\n%s" % result
         else:
           print "No need to upgrade MySQL database"
-        mysql_script = conf.get('mysql_script')
-        if mysql_script:
-          mysql_list = [conf['mysql_binary'].strip(), '--no-defaults', '-B', '--user=root', '--socket=%s' % conf['socket']]
-          mysql = subprocess.Popen(mysql_list, stdin=subprocess.PIPE,
-              stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-          result = mysql.communicate(conf['mysql_script'])[0]
-          if mysql.returncode is None:
-            mysql.kill()
-          if mysql.returncode != 0:
-            print 'Command %r failed with:\n%s' % (mysql_list, result)
-            print 'Sleeping for %ss and retrying' % sleep
-          else:
-            is_succeed = True
-            print 'SlapOS initialisation script succesfully applied on database.'
+        mysql_list = [conf['mysql_binary'].strip(), '--no-defaults', '-B', '--user=root', '--socket=%s' % conf['socket']]
+        mysql = subprocess.Popen(mysql_list, stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        result = mysql.communicate(conf['mysql_script'])[0]
+        if mysql.returncode is None:
+          mysql.kill()
+        if mysql.returncode != 0:
+          print 'Command %r failed with:\n%s' % (mysql_list, result)
+          print 'Sleeping for %ss and retrying' % sleep
+        else:
+          is_succeed = True
+          print 'SlapOS initialisation script succesfully applied on database.'
     sys.stdout.flush()
     sys.stderr.flush()
     time.sleep(sleep)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/lamp/template/apache.in` & `slapos.cookbook-1.0.92/slapos/recipe/lamp/template/apache.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/lamp/template/my.cnf.in` & `slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/my.cnf.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/shell.py` & `slapos.cookbook-1.0.92/slapos/recipe/cloud9/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,38 +20,33 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-import os
-import json
 from slapos.recipe.librecipe import GenericBaseRecipe
+import os
 
 class Recipe(GenericBaseRecipe):
+  """Deploy a fully operational cloud9 service."""
 
-  def install(self):
-    env = os.environ.copy()
+  def _options(self, options):
+    self.ip = options['ip'].strip()
+    self.port = options['port'].strip()
+    self.git = options['git-binary'].strip()
+    self.node_executable = options['node-binary'].strip()
+    self.cloud9 = options['cloud9'].strip()
+    self.workdir = options['working-directory'].strip()
+    self.wrapper = options['wrapper'].strip()
+    # Set cloud9 access URL
+    options['access-url'] = 'http://[%s]:%s' % (self.ip, self.port)
 
-    path_list = self.options['path'].split('\n')
-    env.update(PATH=':'.join(path_list))
-    env.update(SHELL=self.options['shell'])
-    env.update(HOME=self.options['home'])
-
-    ps1 = self.options.get('ps1')
-    if ps1 is not None:
-      env.update(PS1=str(json.loads(ps1)))
-    else:
-      env.update(PS1=env.get('PS1', '> '))
+  def install(self):
+    environment = {
+        'PATH': os.path.dirname(self.git) + ':' + os.environ['PATH'],
+    }
 
-    wrapper = self.createPythonScript(
-      self.options['wrapper'],
-      'slapos.recipe.librecipe.execute.executee',
-      [ # Executable
-        [self.options['shell']],
-        # Environment
-        env
-      ]
-    )
+    cloud9_args = [self.node_executable, self.cloud9, '-l', self.ip, '-p',
+        self.port, '-w', self.workdir]
 
-    return [wrapper]
+    return self.createWrapper(self.wrapper, cloud9_args, environment)
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/_urlparse.py` & `slapos.cookbook-1.0.92/slapos/recipe/erp5_promise/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##############################################################################
 #
-# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2012 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,33 +20,37 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-from urlparse import urlparse
 
 from slapos.recipe.librecipe import GenericBaseRecipe
+import ConfigParser
 
 class Recipe(GenericBaseRecipe):
-
-  def _options(self, options):
-    url = urlparse(options['url'])
-
-    def to_str(data):
-      if data is None:
-        return ''
-      return str(data)
-
-    options.update(scheme=url.scheme,
-                   username=to_str(url.username),
-                   password=to_str(url.password),
-                   host=to_str(url.hostname),
-                   port=to_str(url.port),
-                   path=url.path.strip('/'),
-                   params=url.params,
-                   query=url.query,
-                   fragment=url.fragment)
+  """
+  Generate ERP5 promise configuration file
+  """
 
   def install(self):
-    return []
+    promise_parser = ConfigParser.RawConfigParser()
+    for section_name, option_id_list in (
+          ('portal_templates', (
+            ('repository', 'bt5-repository-url'),
+            ('expected_bt5', 'bt5'),
+          )),
+          ('external_service', (
+            ('cloudooo_url', 'cloudooo-url'),
+            ('memcached_url', 'memcached-url'),
+            ('kumofs_url', 'kumofs-url'),
+            ('smtp_url', 'smtp-url'),
+          )),
+        ):
+      promise_parser.add_section(section_name)
+      for internal_id, option_id in option_id_list:
+        option = self.options.get(option_id)
+        if option:
+          promise_parser.set(section_name, internal_id, option)
+    promise_parser.write(open(self.options['promise-path'], 'w'))
+    return [self.options['promise-path']]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/README.kvm.txt` & `slapos.cookbook-1.0.92/slapos/recipe/README.kvm.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 kvm
 ===
 
-Introduction
-------------
+kvm: Introduction
+-----------------
 
 The erp5.recipe.kvm aims to integrate KVM setups and buildout. This recipe is 
 able to download one remote image and setup a KVM environment to use it. 
 
 This recipe is also capable to reuse images or partitions already present on
 disk to create the setup.
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/slapconfiguration.py` & `slapos.cookbook-1.0.92/slapos/recipe/slapconfiguration.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,30 +22,37 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
 
 import json
+import logging
 import os
 
 import slapos.slap
 from slapos.recipe.librecipe import unwrap
 from ConfigParser import RawConfigParser
 from netaddr import valid_ipv4, valid_ipv6
 from slapos.util import mkdir_p
+from slapos import format as slapformat
+
+
+logger = logging.getLogger("slapos")
+
 
 class Recipe(object):
   """
-  Retrieves slap partition parameters, and makes them available to other
-  buildout section in various ways, and in various encodings.
-  Populates the buildout section it is used in with all slap partition
-  parameters.
-  Also provides access to partition properties: all IPv4, IPv6 and tap
-  interfaces it is allowed to use.
+  Retrieve slap partition parameters and make them available in buildout section.
+
+  There are two sources of parameters. First is configuration file slapos.cfg and
+  derived information.
+  Second is partition's resource_file which is made available in form of keys joined
+  with "-" and with all "_" replaced by "-".
+  For example {"tun": {"ipv4": <addr>}} would be available in buildout as ${instance:tun-ipv4}.
 
   Input:
     url
       Slap server url.
       Example:
         ${slap-connection:server-url}
     key & cert (optional)
@@ -63,48 +70,44 @@
       Example:
         ${slap-connection:partition-id}
     storage-home
       Path of folder configured for data storage
       Example:
         ${storage-configuration:storage-home}
 
-  Output:
+  Output (keys derived from SlapOS configuration):
+    root-instance-title
+      Hosting subscription or root instance title
+    instance-title
+      Title of instance running into this partition
     slap-software-type
       Current partition's software type.
     ipv4
       Set of IPv4 addresses.
     ipv6
       Set of IPv6 addresses.
     ipv4-random
       One of the IPv4 addresses.
     ipv6-random
       One of the IPv6 addresses.
-    tap
-      Set of TAP interfaces.
-    tap-network-information-dict
-      Dict of set of all TAP network information
-    tap-ipv4
-      ipv4 allowed for this TAP
-    tap-gateway
-      ipv4 of gateway interface of this TAP
-    tap-netmask
-      ipv4 netmask address of this TAP
-    tap-network
-      ipv4 network address of this TAP
+    global_ipv4_network
+      The global IPv4 network
     configuration
       Dict of all parameters.
     storage-dict
       Dict of partition data path when it is configured
     configuration.<key>
       One key per partition parameter.
       Partition parameter whose name cannot be represented unambiguously in
       buildout syntax are ignored. They cannot be accessed from buildout syntax
       anyway, and are available through "configuration" output key.
     instance-state
       The instance state.
+
+    Also note that all information from resource file will be appended
   """
 
   # XXX: used to detect if a configuration key is a valid section key. This
   # assumes buildout uses ConfigParser - which is currently the case.
   OPTCRE_match = RawConfigParser.OPTCRE.match
 
   def __init__(self, buildout, name, options):
@@ -114,14 +117,20 @@
       match = self.OPTCRE_match
       for key, value in parameter_dict.iteritems():
           if match(key) is not None:
               continue
           options['configuration.' + key] = value
 
   def fetch_parameter_dict(self, options, instance_root):
+      """Gather parameters about current computer and partition.
+
+      Use two sources of truth
+      1. SlapOS Master - for external computer/partition information
+      2. format.Partition.resource_file - for partition specific details
+      """
       slap = slapos.slap.slap()
       slap.initializeConnection(
           options['url'],
           options.get('key'),
           options.get('cert'),
       )
       computer_partition = slap.registerComputerPartition(
@@ -142,14 +151,22 @@
               ):
           try:
               value = parameter_dict.pop(his_key)
           except KeyError:
               pass
           else:
               options[his_key.replace('_', '-')] = value
+      # Get Instance and root instance title or return UNKNOWN if not set
+      options['instance-title'] = parameter_dict.pop('instance_title',
+                                            'UNKNOWN Instance').encode('UTF-8')
+      options['root-instance-title'] = parameter_dict.pop('root_instance_title',
+                                            'UNKNOWN').encode('UTF-8')
+      options['instance-guid'] = computer_partition.getInstanceGuid() \
+          .encode('UTF-8')
+
       ipv4_set = set()
       v4_add = ipv4_set.add
       ipv6_set = set()
       v6_add = ipv6_set.add
       tap_set = set()
       tap_add = tap_set.add
       route_gw_set = set()
@@ -186,28 +203,14 @@
       options['ipv6'] = ipv6_set
 
       # also export single ip values for those recipes that don't support sets.
       if ipv4_set:
           options['ipv4-random'] = list(ipv4_set)[0].encode('UTF-8')
       if ipv6_set:
           options['ipv6-random'] = list(ipv6_set)[0].encode('UTF-8')
-      if route_ipv4_set:
-        options['tap-ipv4'] = list(route_ipv4_set)[0].encode('UTF-8')
-        options['tap-network-information-dict'] = dict(ipv4=route_ipv4_set,
-                                    netmask=route_mask_set,
-                                    gateway=route_gw_set,
-                                    network=route_network_set)
-      else:
-        options['tap-network-information-dict'] = {}
-      if route_gw_set:
-        options['tap-gateway'] = list(route_gw_set)[0].encode('UTF-8')
-      if route_mask_set:
-        options['tap-netmask'] = list(route_mask_set)[0].encode('UTF-8')
-      if route_network_set:
-        options['tap-network'] = list(route_network_set)[0].encode('UTF-8')
 
       storage_home = options.get('storage-home')
       storage_dict = {}
       if storage_home and os.path.exists(storage_home) and \
                                   os.path.isdir(storage_home):
         for filename in os.listdir(storage_home):
           storage_path = os.path.join(storage_home, filename, 
@@ -216,15 +219,36 @@
             storage_link = os.path.join(instance_root, 'DATA', filename)
             mkdir_p(os.path.join(instance_root, 'DATA'))
             if not os.path.lexists(storage_link):
               os.symlink(storage_path, storage_link)
             storage_dict[filename] = storage_link
       options['storage-dict'] = storage_dict
 
-      options['tap'] = tap_set
+      # The external information transfered from Slap Master has been processed
+      # so we extend with information gathered from partition resource file
+      if hasattr(slapformat.Partition, "resource_file"):
+        resource_home = instance_root
+        while not os.path.exists(os.path.join(resource_home, slapformat.Partition.resource_file)):
+          resource_home = os.path.normpath(os.path.join(resource_home, '..'))
+          if resource_home == "/":
+            break
+        else:
+          # no break happened - let's add partition resources into options
+          logger.debug("Using partition resource file {}".format(
+            os.path.join(resource_home, slapformat.Partition.resource_file)))
+          with open(os.path.join(resource_home, slapformat.Partition.resource_file)) as fi:
+            partition_params = json.load(fi)
+          # be very careful with overriding master's information
+          for key, value in flatten_dict(partition_params).items():
+            if key not in options:
+              if isinstance(value, unicode):
+                value = value.encode('UTF-8')
+              options[key] = value
+      # print out augmented options to see what we are passing
+      logger.debug(str(options))
       return self._expandParameterDict(options, parameter_dict)
 
   def _expandParameterDict(self, options, parameter_dict):
       options['configuration'] = parameter_dict
       return parameter_dict
 
   install = update = lambda self: []
@@ -245,7 +269,18 @@
       fout.write(json.dumps(parameter_dict, indent=2, sort_keys=True))
 
     def install(self):
         return [self._json_output]
 
     update = install
 
+
+def flatten_dict(data, key_prefix=''):
+  """Transform folded dict into one-level key-subkey-subsubkey dictionary."""
+  output = {}
+  for key, value in data.items():
+    prefixed_key = key_prefix + key.replace("_", "-")  # to be consistent with `fetch_parameter_dict`
+    if isinstance(value, dict):
+      output.update(flatten_dict(value, key_prefix=prefixed_key + "-"))
+      continue
+    output[prefixed_key] = value
+  return output
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/signal_wrapper.py` & `slapos.cookbook-1.0.92/slapos/recipe/signal_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,10 +28,10 @@
 
 class Recipe(GenericBaseRecipe):
   def install(self):
     return [
       self.createPythonScript(
         self.options['wrapper-path'],
         'slapos.recipe.librecipe.execute.execute_with_signal_translation',
-        [self.options['wrapped-path']]
+        ((self.options['wrapped-path'],),)
       )
     ]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/boinc/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/boinc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,32 +120,31 @@
     environment = dict(
         PATH=os.pathsep.join([self.svn, bin_dir, self.perl, os.environ['PATH']]),
         PYTHONPATH=os.pathsep.join([python_path, os.environ['PYTHONPATH']]),
     )
 
     #Generate wrapper for php
     wrapperphp = os.path.join(self.home, 'bin/php')
-    php_wrapper = self.createPythonScript(wrapperphp,
-        'slapos.recipe.librecipe.execute.executee',
-        ([self.phpbin, '-c', self.phpini], os.environ)
+    php_wrapper = self.createWrapper(wrapperphp,
+        (self.phpbin, '-c', self.phpini),
     )
     path_list.append(php_wrapper)
 
+    mysql_dict = dict(db=self.database,
+        host=self.mysqlhost, port=self.mysqlport,
+        user=self.username, passwd=self.password)
+
     #Generate python script for MySQL database test (starting)
     file_status = os.path.join(self.home, '.boinc_config')
     if os.path.exists(file_status):
       os.unlink(file_status)
     mysql_wrapper = self.createPythonScript(
       os.path.join(self.wrapperdir, 'start_config'),
       '%s.configure.checkMysql' % __name__,
-      dict(mysql_port=self.mysqlport, mysql_host=self.mysqlhost,
-          mysql_user=self.username, mysql_password=self.password,
-          database=self.database,
-          file_status=file_status, environment=environment
-      )
+      (environment, mysql_dict, file_status)
     )
 
     # Generate make project wrapper file
     readme_file = os.path.join(self.installroot, self.project+'.readme')
     launch_args = [make_project, '--url_base', self.url_base, "--db_name",
               self.database, "--db_user", self.username, "--db_passwd",
               self.password, "--project_root", self.installroot, "--db_host",
@@ -160,16 +159,15 @@
       if os.path.exists(readme_file):
         os.unlink(readme_file)
     launch_args += [self.project, niceprojectname]
 
     install_wrapper = self.createPythonScript(
       os.path.join(self.wrapperdir, 'make_project'),
       '%s.configure.makeProject' % __name__,
-      dict(launch_args=launch_args, request_file=request_make_boinc,
-      make_sig=file_status, env=environment)
+      (file_status, launch_args, request_make_boinc, environment)
     )
     path_list.append(install_wrapper)
 
     #generate sh script for project configuration
     bash = os.path.join(self.home, 'bin', 'project_config.sh')
     sh_script = self.createFile(bash,
         self.substituteTemplate(self.getTemplateFilename('project_config.in'),
@@ -193,33 +191,31 @@
         environment=environment,
         service_status=service_status,
         drop_install=drop_install,
         sedconfig=bash
     )
     start_service = self.createPythonScript(
       os.path.join(self.wrapperdir, 'config_project'),
-      '%s.configure.services' % __name__, parameter
+      '%s.configure.services' % __name__, (parameter,)
     )
     path_list.append(start_service)
 
     #Generate Boinc start project wrapper
     start_args = [os.path.join(self.installroot, 'bin/start')]
     start_boinc = os.path.join(self.home, '.start_boinc')
     if os.path.exists(start_boinc):
       os.unlink(start_boinc)
     boinc_parameter = dict(service_status=service_status,
         installroot=self.installroot, drop_install=drop_install,
-        mysql_port=self.mysqlport, mysql_host=self.mysqlhost,
-        mysql_user=self.username, mysql_password=self.password,
-        database=self.database, environment=environment,
+        mysql_dict=mysql_dict, environment=environment,
         start_boinc=start_boinc)
     start_wrapper = self.createPythonScript(os.path.join(self.wrapperdir,
         'start_boinc'),
         '%s.configure.restart_boinc' % __name__,
-        boinc_parameter
+        (boinc_parameter,)
     )
     path_list.append(start_wrapper)
 
     return path_list
 
   update = install
 
@@ -358,15 +354,15 @@
                 binary=app_list[appname][version]['binary'],
                 extension=app_list[appname][version]['extension'],
                 bash=bash, home_dir=home,
                 lockfile=lockfile,
         )
         deploy_app = self.createPythonScript(
           os.path.join(wrapperdir, 'boinc_%s' % appname),
-          '%s.configure.deployApp' % __name__, parameter
+          '%s.configure.deployApp' % __name__, (parameter,)
         )
         path_list.append(deploy_app)
 
     return path_list
 
   update = install
 
@@ -400,22 +396,20 @@
       config_dest = os.path.join(installdir, 'cc_config.xml')
       file = open(config_dest, 'w')
       file.write(open(self.options['cconfig'].strip(), 'r').read())
       file.close()
       cc_cmd = '--read_cc_config'
     cmd = self.createPythonScript(cmd_wrapper,
         '%s.configure.runCmd' % __name__,
-        dict(base_cmd=base_cmd, cc_cmd=cc_cmd, installdir=installdir,
-        project_url=url, key=key)
+        (base_cmd, cc_cmd, installdir, url, key)
     )
     path_list.append(cmd)
 
     #Generate BOINC client wrapper
-    boinc = self.createPythonScript(boinc_wrapper,
-            'slapos.recipe.librecipe.execute.execute',
-            [boincbin, '--allow_multiple_clients', '--gui_rpc_port',
+    boinc = self.createWrapper(boinc_wrapper,
+            (boincbin, '--allow_multiple_clients', '--gui_rpc_port',
               str(self.options['rpc-port']), '--allow_remote_gui_rpc',
-              '--dir', installdir, '--redirectio', '--check_all_logins']
+              '--dir', installdir, '--redirectio', '--check_all_logins'),
     )
     path_list.append(boinc)
 
     return path_list
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/boinc/configure.py` & `slapos.cookbook-1.0.92/slapos/recipe/boinc/configure.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,61 +31,53 @@
 import time
 import shutil
 import re
 import filecmp
 
 from lock_file import LockFile
 
-def checkMysql(args):
-  sys.path += args['environment']['PYTHONPATH'].split(':')
+def checkMysql(environment, connect_kw, file_status=None):
+  sys.path += environment['PYTHONPATH'].split(':')
   import MySQLdb
   #Sleep until mysql server becomes available
   while True:
     try:
-      conn = MySQLdb.connect(host = args['mysql_host'],
-                          user = args['mysql_user'],
-                          port = int(args['mysql_port']),
-                          passwd = args['mysql_password'],
-                          db = args['database'])
-      conn.close()
-      print "Successfully connect to MySQL database... "
-      if args.has_key('file_status'):
-        writeFile(args['file_status'], "starting")
+      MySQLdb.connect(**connect_kw).close()
       break
     except Exception, ex:
       print "The result is: \n" + ex.message
       print "Could not connect to MySQL database... sleep for 2 secondes"
       time.sleep(2)
-
+  print "Successfully connect to MySQL database... "
+  if file_status:
+    writeFile(file_status, "starting")
 
 def checkFile(file, stime):
   """Loop until 'file' is created (exist)"""
   while True:
     print "Search for file %s..." % file
     if not os.path.exists(file):
       print "File not found... sleep for %s secondes" % stime
       time.sleep(stime)
     else:
       break
 
 
 def restart_boinc(args):
   """Stop (if currently is running state) and start all Boinc service"""
+  environment = args['environment']
   if args['drop_install']:
     checkFile(args['service_status'], 3)
   else:
-    checkMysql(args)
+    checkMysql(environment, args['mysql_dict'], args.get('file_status'))
   print "Restart Boinc..."
-  env = os.environ
-  env['PATH'] = args['environment']['PATH']
-  env['PYTHONPATH'] = args['environment']['PYTHONPATH']
-  binstart = os.path.join(args['installroot'], 'bin/start')
-  binstop = os.path.join(args['installroot'], 'bin/stop')
-  os.system(binstop)
-  os.system(binstart)
+  env = os.environ.copy()
+  env.update(environment)
+  subprocess.call((os.path.join(args['installroot'], 'bin', 'stop'),), env=env)
+  subprocess.call((os.path.join(args['installroot'], 'bin', 'start'),), env=env)
   writeFile(args['start_boinc'], "started")
   print "Done."
 
 
 def check_installRequest(args):
   print "Cheking if needed to install %s..." % args['appname']
   install_request_file = os.path.join(args['home_dir'],
@@ -118,25 +110,24 @@
               cwd=cwd)
   result = process.communicate()[0]
   if process.returncode is None or process.returncode != 0:
     print "Failed to execute executable.\nThe error was: %s" % result
     return False
   return True
 
-def makeProject(args):
+def makeProject(make_sig, launch_args, request_file, extra_environ):
   """Run BOINC make_project script but once only"""
   #Wait for DateBase initialization...
-  checkFile(args['make_sig'], 3)
+  checkFile(make_sig, 3)
   print "Cheking if needed to run BOINC make_project..."
-  if os.path.exists(args['request_file']):
-    env = os.environ
-    env['PATH'] = args['env']['PATH']
-    env['PYTHONPATH'] = args['env']['PYTHONPATH']
-    if startProcess(args['launch_args'], env=env):
-      os.unlink(args['request_file'])
+  if os.path.exists(request_file):
+    env = os.environ.copy()
+    env.update(extra_environ)
+    if startProcess(launch_args, env=env):
+      os.unlink(request_file)
     print "Finished running BOINC make_projet...Ending"
   else:
     print "No new request for make_project. Exiting..."
 
 
 def services(args):
   """This function configure a new installed boinc project instance"""
@@ -151,17 +142,16 @@
   print "Generating .htpasswd file... File=%s" % topath
   passwd = open(args['passwd'], 'r').read()
   htpwd_args = [args['htpasswd'], '-b', '-c', topath, args['username'], passwd]
   if not startProcess(htpwd_args):
     return
 
   print "execute script xadd..."
-  env = os.environ
-  env['PATH'] = args['environment']['PATH']
-  env['PYTHONPATH'] = args['environment']['PYTHONPATH']
+  env = os.environ.copy()
+  env.update(args['environment'])
   if not startProcess([os.path.join(args['installroot'], 'bin/xadd')], env):
     return
   print "Update files and directories permissions..."
   upload = os.path.join(args['installroot'], 'upload')
   inc = os.path.join(args['installroot'], 'html/inc')
   languages = os.path.join(args['installroot'], 'html/languages')
   compiled = os.path.join(args['installroot'], 'html/languages/compiled')
@@ -208,17 +198,16 @@
       print args['appname'] + " Work units will be updated from %s to %s" % (
                 args['previous_wu'], args['wu_number'])
   else:
     args['previous_wu'] = 0
     newInstall = True
   #Sleep until file .start_boinc exist (File indicate that BOINC has been started)
   checkFile(args['start_boinc'], 3)
-  env = os.environ
-  env['PATH'] = args['environment']['PATH']
-  env['PYTHONPATH'] = args['environment']['PYTHONPATH']
+  env = os.environ.copy()
+  env.update(args['environment'])
 
   print "setup directories..."
   numversion = args['version'].replace('.', '')
   args['inputfile'] = os.path.join(args['installroot'], 'download',
                         args['appname'] + numversion + '_input')
   base_app = os.path.join(args['installroot'], 'apps', args['appname'])
   base_app_version = os.path.join(base_app, args['version'])
@@ -259,15 +248,15 @@
 
   if signBin:
     print "Sign the application binary..."
     sign = os.path.join(args['installroot'], 'bin/sign_executable')
     privateKeyFile = os.path.join(args['installroot'], 'keys/code_sign_private')
     output = open(binary + '.sig', 'w')
     p_sign = subprocess.Popen([sign, binary, privateKeyFile], stdout=output,
-            stderr=subprocess.STDOUT)
+            stderr=subprocess.STDOUT, env=env)
     result = p_sign.communicate()[0]
     if p_sign.returncode is None or p_sign.returncode != 0:
       print "Failed to execute bin/sign_executable.\nThe error was: %s" % result
       return
     output.close()
 
   print "execute script xadd..."
@@ -286,18 +275,16 @@
     print "Failed to execute bin/update_versions.\nThe error was: %s" % result
     return
 
   print "Fill the database... calling bin/create_work..."
   create_wu(args, env)
 
   print "Restart Boinc..."
-  binstart = os.path.join(args['installroot'], 'bin/start')
-  binstop = os.path.join(args['installroot'], 'bin/stop')
-  os.system(binstop)
-  os.system(binstart)
+  subprocess.call((os.path.join(args['installroot'], 'bin', 'stop'),), env=env)
+  subprocess.call((os.path.join(args['installroot'], 'bin', 'start'),), env=env)
 
   print "Boinc Application deployment is done... writing end signal file..."
   writeFile(token, str(args['wu_number']))
 
 
 def create_wu(args, env):
   """Create or update number of work unit for an existing boinc application"""
@@ -311,29 +298,28 @@
         args['appname'] + numversion + '_input']
   for i in range(args['previous_wu'], args['wu_number']):
     print "Creating project wroker %s..." % str(i+1)
     launch_args[4] = args['appname'] + str(i+1) + numversion + '_nodelete'
     startProcess(launch_args, env, args['installroot'])
 
 
-def runCmd(args):
+def runCmd(base_cmd, cc_cmd, installdir, url, key):
   """Wait for Boinc Client started and run boinc cmd"""
-  client_config = os.path.join(args['installdir'], 'client_state.xml')
+  client_config = os.path.join(installdir, 'client_state.xml')
   checkFile(client_config, 5)
   time.sleep(10)
   #Scan client state xml to find client ipv4 adress
   host = re.search("<ip_addr>([\w\d\.:]+)</ip_addr>",
                 open(client_config, 'r').read()).group(1)
-  args['base_cmd'][2] = host + ':' + args['base_cmd'][2]
-  print "Run boinccmd with host at %s " % args['base_cmd'][2]
-  project_args = args['base_cmd'] + ['--project_attach', args['project_url'],
-                      args['key']]
-  startProcess(project_args, cwd=args['installdir'])
-  if args['cc_cmd'] != '':
+  base_cmd[2] = host + ':' + base_cmd[2]
+  print "Run boinccmd with host at %s " % base_cmd[2]
+  project_args = base_cmd + ['--project_attach', url, key]
+  startProcess(project_args, cwd=installdir)
+  if cc_cmd:
     #Load or reload cc_config file
-    startProcess(args['base_cmd'] + [args['cc_cmd']], cwd=args['installdir'])
+    startProcess(base_cmd + [cc_cmd], cwd=installdir)
 
 
 def writeFile(file, content):
   f = open(file, 'w')
   f.write(content)
   f.close()
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/hibernate.cfg.xml.in` & `slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/hibernate.cfg.xml.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/my.cnf.in` & `slapos.cookbook-1.0.92/slapos/recipe/mysql/template/my.cnf.in`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 skip-show-database
 port = %(tcp_port)s
 bind-address = %(ip)s
 socket = %(socket)s
 datadir = %(data_directory)s
 pid-file = %(pid_file)s
 log-error = %(error_log)s
-slow_query_log
-slow_query_log_file = %(slow_query_log)s
 long_query_time = 5
 max_allowed_packet = 128M
 query_cache_size = 32M
 
 plugin-load = ha_mroonga.so
 
 # The following are important to configure and depend a lot on to the size of
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/xwiki/template/tomcat-server.xml.in` & `slapos.cookbook-1.0.92/slapos/recipe/xwiki/template/tomcat-server.xml.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/README.kvm_frontend.txt` & `slapos.cookbook-1.0.92/slapos/recipe/README.kvm_frontend.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 kvm_frontend
-===
+=============
 
-Introduction
-------------
+kvm_frontend: Introduction
+---------------------------
 
 The ``slapos.recipe.kvm_frontend`` aims to provide proxy server to KVM instances.
 
 It allows HTTPS IPv4/IPv6 proxying (with or without domain name), and supports
 the WebSocket technology needed for VNC-in-webapplication noVNC.
 
 It works following the master/slave instances system. A master instance is
 created, containing all what is needed to run the proxy. Slave instances
 are later created, adding one line in the master instance's proxy configuration
 that specify the IP/port to proxy to the KVM.
-
 The slave instance (kvm) is then accessible from
 http://[masterinstanceIPorhostname]/[randomgeneratednumber]
 
 
 Instance parameters
-------------
+-------------------
 
 Incoming master instance parameters
-+++++++
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-``port``                - Port of server, optional, defaults to 4443.
-``domain``              - domain name to use, optional, default to
-                          "host.vifib.net".
-``redirect_plain_http`` - if value is one of ['y', 'yes', '1', 'true'], instance
-                          will try to create a simple http server on port 80
-                          redirecting to the proxy. Optional.
+ * ``port``                - Port of server, optional, defaults to 4443.
+ * ``domain``              - domain name to use, optional, default to ``host.vifib.net``.
+ * ``redirect_plain_http`` - if value is one of ``['y', 'yes', '1', 'true']``,
+   will try to create a simple http server on port 80 redirecting to the proxy. Optional.
 
 Incoming slave instance parameters
-+++++++
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-``host``    - KVM instance IP or hostname. Mandatory.
-``port``    - KVM instance port, Mandatory.
-``https``   - if value is one of ['n', 'no', '0', 'false'], will try to connect
-              to target in plain http. Optional.
+ * ``host``    - KVM instance IP or hostname. Mandatory.
+ * ``port``    - KVM instance port, Mandatory.
+ * ``https``   - if value is one of ``['n', 'no', '0', 'false']``, will try to connect to target in plain http. Optional.
 
 Connection parameters
--------------
+---------------------
 
 Outgoing master connection parameters
-+++++++
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-``domain_ipv6_address``  - Proxy IP
-``site_url``             - Proxy URL
+ * ``domain_ipv6_address``  - Proxy IP
+ * ``site_url``             - Proxy URL
 
-Outgoing slave connection parameters are :
-+++++++
+Outgoing slave connection parameters
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-``site_url``             - URL of instance
-``domain_name``          - Domain name of proxy
-``port``                 - Port of proxy
+ * ``site_url``             - URL of instance
+ * ``domain_name``          - Domain name of proxy
+ * ``port``                 - Port of proxy
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/erp5/template/apache.zope.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/apachephp/template/apache.in`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,56 @@
-# Apache configuration file for Zope
+# Apache static configuration
 # Automatically generated
 
-# List of modules
-LoadModule unixd_module modules/mod_unixd.so
-LoadModule access_compat_module modules/mod_access_compat.so
-LoadModule authz_core_module modules/mod_authz_core.so
-LoadModule authz_host_module modules/mod_authz_host.so
-LoadModule log_config_module modules/mod_log_config.so
-LoadModule setenvif_module modules/mod_setenvif.so
-LoadModule version_module modules/mod_version.so
-LoadModule proxy_module modules/mod_proxy.so
-LoadModule proxy_http_module modules/mod_proxy_http.so
-LoadModule socache_shmcb_module modules/mod_socache_shmcb.so
-LoadModule ssl_module modules/mod_ssl.so
-LoadModule mime_module modules/mod_mime.so
-LoadModule dav_module modules/mod_dav.so
-LoadModule dav_fs_module modules/mod_dav_fs.so
-LoadModule negotiation_module modules/mod_negotiation.so
-LoadModule rewrite_module modules/mod_rewrite.so
-LoadModule headers_module modules/mod_headers.so
-LoadModule antiloris_module modules/mod_antiloris.so
-
 # Basic server configuration
 PidFile "%(pid_file)s"
 Listen %(ip)s:%(port)s
-ServerAdmin %(server_admin)s
+PHPINIDir %(php_ini_dir)s
+ServerAdmin someone@email
+DefaultType text/plain
 TypesConfig conf/mime.types
 AddType application/x-compress .Z
 AddType application/x-gzip .gz .tgz
-
-ServerTokens Prod
-ServerSignature Off
-TraceEnable Off
-
-# As backend is trusting REMOTE_USER header unset it always
-RequestHeader unset REMOTE_USER
-
-# SSL Configuration
-%(ssl_snippet)s
+AddType application/x-httpd-php .php .phtml .php5 .php4
+AddType application/x-httpd-php-source .phps
 
 # Log configuration
 ErrorLog "%(error_log)s"
-# Default apache log format with request time in microsecond at the end
-LogFormat "%%h %%l %%u %%t \"%%r\" %%>s %%b \"%%{Referer}i\" \"%%{User-Agent}i\" %%D" combined
-CustomLog "%(access_log)s" combined
+LogLevel warn
+LogFormat "%%h %%{REMOTE_USER}i %%l %%u %%t \"%%r\" %%>s %%b \"%%{Referer}i\" \"%%{User-Agent}i\"" combined
+LogFormat "%%h %%{REMOTE_USER}i %%l %%u %%t \"%%r\" %%>s %%b" common
+CustomLog "%(access_log)s" common
 
 # Directory protection
 <Directory />
     Options FollowSymLinks
     AllowOverride None
-    Order deny,allow
-    Deny from all
+    Require all denied
 </Directory>
 
-%(path_enable)s
+<Directory %(document_root)s>
+  Options FollowSymLinks
+  AllowOverride All
+  Require all granted
+</Directory>
+DocumentRoot %(document_root)s
+DirectoryIndex index.html index.php
 
-# Magic of Zope related rewrite
-RewriteEngine On
-%(rewrite_rule)s
+# List of modules
+LoadModule unixd_module modules/mod_unixd.so
+LoadModule access_compat_module modules/mod_access_compat.so
+LoadModule authz_core_module modules/mod_authz_core.so
+LoadModule authz_host_module modules/mod_authz_host.so
+LoadModule log_config_module modules/mod_log_config.so
+LoadModule setenvif_module modules/mod_setenvif.so
+LoadModule version_module modules/mod_version.so
+LoadModule proxy_module modules/mod_proxy.so
+LoadModule proxy_http_module modules/mod_proxy_http.so
+LoadModule mime_module modules/mod_mime.so
+LoadModule dav_module modules/mod_dav.so
+LoadModule dav_fs_module modules/mod_dav_fs.so
+LoadModule negotiation_module modules/mod_negotiation.so
+LoadModule rewrite_module modules/mod_rewrite.so
+LoadModule headers_module modules/mod_headers.so
+LoadModule dir_module modules/mod_dir.so
+LoadModule php5_module modules/libphp5.so
+LoadModule alias_module modules/mod_alias.so
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/mioga/instantiate.py` & `slapos.cookbook-1.0.92/slapos/recipe/mioga/instantiate.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,44 +199,41 @@
     #   self.substituteTemplate(self.getTemplateFilename('apache.in'),
     #                           apache_config)
     # )
     path_list.append(os.path.abspath(self.options['httpd_conf']))
 
     services_dir = self.options['services_dir']
 
-    httpd_wrapper = self.createPythonScript(
+    httpd_wrapper = self.createWrapper(
       os.path.join(services_dir, 'httpd_wrapper'),
-      'slapos.recipe.librecipe.execute.execute',
-      [self.options['httpd_binary'], '-f', self.options['httpd_conf'],
-       '-DFOREGROUND']
+      (self.options['httpd_binary'],
+        '-f', self.options['httpd_conf'], '-DFOREGROUND'),
     )
     path_list.append(httpd_wrapper)
 
     for fifo in [notifier_fifo, searchengine_fifo]:
       if os.path.exists(fifo):
         if not stat.S_ISFIFO(os.stat(fifo).st_mode):
           raise Exception("The file "+fifo+" exists but is not a FIFO.")
       else:
         os.mkfifo(fifo, 0600)
 
     site_perl_bin = os.path.join(self.options['site_perl'], 'bin')
     mioga_conf_path = os.path.join(mioga_base, 'conf', 'Mioga.conf')
-    notifier_wrapper = self.createPythonScript(
+    notifier_wrapper = self.createWrapper(
       os.path.join(services_dir, 'notifier'),
-      'slapos.recipe.librecipe.execute.execute',
-      [ os.path.join(site_perl_bin, 'notifier.pl'),
-        mioga_conf_path ]
+      (os.path.join(site_perl_bin, 'notifier.pl'),
+        mioga_conf_path),
     )
     path_list.append(notifier_wrapper)
 
-    searchengine_wrapper = self.createPythonScript(
+    searchengine_wrapper = self.createWrapper(
       os.path.join(services_dir, 'searchengine'),
-      'slapos.recipe.librecipe.execute.execute',
-      [ os.path.join(site_perl_bin, 'searchengine.pl'),
-        mioga_conf_path ]
+      (os.path.join(site_perl_bin, 'searchengine.pl'),
+        mioga_conf_path),
     )
     path_list.append(searchengine_wrapper)
 
     crawl_fm = FileModifier( os.path.join('bin', 'search', 'crawl_sample.sh') )
     # TODO: The crawl script will still call the shell command "date"
     crawl_fm.modify(r'/var/tmp/crawl', self.options['log_dir'] + '/crawl')
     crawl_fm.modify(r'/var/lib/Mioga2/conf', mioga_base + '/conf')
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/README.lamp.txt` & `slapos.cookbook-1.0.92/slapos/recipe/README.lamp.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,87 +2,96 @@
 =====
 
 The lamp recipe helps you to deploy simply a php based application on slapos. This recipe is 
 able to setup mariadb, apache and apache-php for your php application, and is also capable of
 configuring your software during installation to ensure a full compatibility.
 
 
-How to use?
------------
+How to use lamp ?
+-----------------
 
 just add this part in your software.cfg to use the lamp.simple module
 
-[instance-recipe]
-egg = slapos.cookbook
-module = lamp.simple
+.. code-block:: ini
+
+  [instance-recipe]
+  egg = slapos.cookbook
+  module = lamp.simple
 
 you also need to extend lamp.cfg
 
-extends =
-  http://git.erp5.org/gitweb/slapos.git/blob_plain/refs/tags/slapos-0.50:/stack/lamp.cfg
+.. code-block:: ini
+
+  extends =
+    https://lab.nexedi.com/nexedi/slapos/raw/slapos-0.50/stack/lamp.cfg
 
 
 lamp.runner
-=====
+===========
 
 When you install some software (such as prestashop) you need to remove or rename folder, with slapos you can not 
 access to the www-data directory. to do this, you need to tell to lamp recipe to remove or/and it when software 
 will be instantiated. Some software requires more than rename or delete a folder (manualy create database etc...)
 in this case you need to write a python script and lamp recipe must run it when installing your software.
 
 
 
-How to use?
------------
+How to use lamp.runner ?
+------------------------
 
 this part of lamp recipe work with slapos.toolbox, Therefore you must add it to your recipe.
 in software.cfg, replace instance-recipe-egg part by
 
-[instance-recipe-egg]
-recipe = zc.recipe.egg
-eggs =
-    ${mysql-python:egg}
-    ${instance-recipe:egg}
-    slapos.toolbox[lampconfigure]
+.. code-block:: ini
+
+  [instance-recipe-egg]
+  recipe = zc.recipe.egg
+  eggs =
+      ${python-mysqlclient:egg}
+      ${instance-recipe:egg}
+      slapos.toolbox[lampconfigure]
 
 and add into your instance.cfg
 
-lampconfigure_directory = ${buildout:bin-directory}/lampconfigure
+.. code-block:: ini
+
+  lampconfigure_directory = ${buildout:bin-directory}/lampconfigure
 
 
 CONDITION
---------
+----------
 
 the action (delete, rename, script, chmod) only starts when the condition is filled.
-in instance.cfg, add 
+in instance.cfg, add:: 
 
-file_token = path_of_file
+  file_token = path_of_file
 
 and the action will begin when path_of_www-data/path_of_file will be created
-you can also use database to check condition. add 
+you can also use database to check condition. add ::
 
-table_name = name_of_table
-constraint = sql_where_condition
+  table_name = name_of_table
+  constraint = sql_where_condition
 
-name_of_table is the full or partial name(in some cases we can not know the prefix used to create tables) of table
-into mariadb databse for example table_name = admin. if you use
-name_of_table = **, the action will begin when database is ready. 
-constraint is the sql_condition to use when search entry into name_of_table for example constraint = `admin_id`=1
+``name_of_table`` is the full or partial name(in some cases we can not know the prefix used to create tables) of table
+into mariadb databse for example ``table_name = admin``. if you use
+``name_of_table = **``, the action will begin when database is ready.
+constraint is the sql_condition to use when search entry into name_of_table for example constraint = ``admin_id=1``
 
 you can't use file_token and table_name at the same time, otherwise file_token will be used in priority. Beware of conditions that will never be satisfied.
 
 
 
 ACTION
 -------
+
 The action starts when condition is true
-1- delete file or folder
-into instance.cfg, use 
 
-delete = file_or_folder1, file_or_folder2, file_or_folder3 ...
+1- delete file or folder into instance.cfg, use:: 
+
+  delete = file_or_folder1, file_or_folder2, file_or_folder3 ...
 
 for example delete = admin 
 
 2- rename file or folder
 into instance.cfg, use 
 
 rename_chmod = mode (optional)
@@ -102,29 +111,34 @@
 mode = mode_to_apply (ex= 0644)
 
 4- Launch python script
 
 use script = ${configure-script:location}/${configure-script:filename} into instance.cfg, add part configure-script
 into software.cfg
 
-parts = configure-script
+.. code-block:: ini
+
+  parts = configure-script
+
+  [configure-script]
+  recipe = hexagonit.recipe.download
+  location = ${buildout:parts-directory}/${:_buildout_section_name_}
+  url = url_of_script_name.py
+  filename = script_name.py
+  download-only = True
+
+The script_name.py should contain a main function, sys.argv is given to the main. you can write script_name.py like this::
+
+    ...
+    def setup(args):
+      mysql_port, mysql_host, mysql_user, mysql_password, mysql_database, base_url, htdocs = args
+      .......
+
+    if __name__ == '__main__':
+        setup(sys.argv[1:])
+
+
+- base_url: is the url of php software
+- htdocs: is the path of www-data directory
+- mysql_user, mysql_password, mysql_database, mysql_host: is the mariadb parameters
 
-[configure-script]
-recipe = hexagonit.recipe.download
-location = ${buildout:parts-directory}/${:_buildout_section_name_}
-url = url_of_script_name.py
-filename = script_name.py
-download-only = True
-
-The script_name.py should contain a main function, sys.argv is given to the main. you can write script_name.py like this
-....
-def setup(args):
-    mysql_port, mysql_host, mysql_user, mysql_password, mysql_database, base_url, htdocs = args
-    .......
-
-if __name__ == '__main__':
-    setup(sys.argv[1:])
-
-base_url: is the url of php software
-htdocs: is the path of www-data directory
-mysql_user, mysql_password, mysql_database, mysql_host: is the mariadb parameters
 you can also use "import MySQLdb" if you want to access to database via your python script
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/waitfor.py` & `slapos.cookbook-1.0.92/slapos/recipe/check_port_listening.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# vim: set et sts=2:
 ##############################################################################
 #
-# Copyright (c) 2010 Vifib SARL and Contributors. All Rights Reserved.
+# Copyright (c) 2011 Vifib SARL and Contributors. All Rights Reserved.
 #
 # WARNING: This program as such is intended to be used by professional
 # programmers who take the whole responsibility of assessing all potential
 # consequences resulting from its eventual inadequacies and bugs
 # End users who are looking for a ready-to-use solution with commercial
 # guarantees and support are strongly adviced to contract a Free Software
 # Service Company
@@ -20,23 +21,40 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-import shlex
-
 from slapos.recipe.librecipe import GenericBaseRecipe
+from zc.buildout.easy_install import _safe_arg, script_header
+import sys
+
+template = script_header + r"""
+# BEWARE: This file is operated by slapgrid
+# BEWARE: It will be overwritten automatically
+import socket
+import sys
+
+addr = "%(hostname)s", %(port)s
+
+try:
+  socket.create_connection(addr).close()
+except (socket.error, socket.timeout):
+  sys.stderr.write("%%s on %%s isn't listening\n" %% addr)
+  sys.exit(127)
+"""
 
 class Recipe(GenericBaseRecipe):
+  """
+  Check listening port promise
+  """
 
   def install(self):
-    files = [f for f in self.options['files'].split('\n') if f]
-    command_line = shlex.split(self.options['command-line'])
-    wrapper = self.createPythonScript(
-      self.options['wrapper'],
-      'slapos.recipe.librecipe.execute.execute_wait',
-      [ command_line,
-        files ],
-    )
-    return [wrapper]
+    promise = self.createExecutable(self.options['path'], template % {
+      'python': _safe_arg(sys.executable),
+      'dash_S': '', # BBB buildout 1.x
+      'hostname': self.options['hostname'],
+      'port': self.options['port'],
+      })
+
+    return [promise]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/apachephpconfigure/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/apachephpconfigure/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
       print "Creating lampconfigure with 'run' arguments"
       command = argument + data
 
 
     configureinstall_wrapper_path = self.createPythonScript(
         self.options['configureinstall-location'],
         __name__ + '.runner.executeRunner',
-        [argument, delete, rename, chmod, data]
+        (argument, delete, rename, chmod, data)
     )
     
     #TODO finish to port this and remove upper one
     #configureinstall_wrapper_path = self.createPythonScript(
     #    self.options['configureinstall-location'],
     #    'slapos.lamp.run',
     #    [command]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/web_checker/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/web_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/web_checker/template/web_checker.cfg.in` & `slapos.cookbook-1.0.92/slapos/recipe/web_checker/template/web_checker.cfg.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/publish_early.py` & `slapos.cookbook-1.0.92/slapos/recipe/publish_early.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/libcloud/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/libcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/zeo/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/zeo/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -85,14 +85,13 @@
     # Create configuration file
     template_filename = self.getTemplateFilename('zeo.conf.in')
     configuration_path = self.createFile(
         self.options['conf-path'],
         self.substituteTemplate(template_filename, config))
 
     # Create running wrapper
-    wrapper_path = self.createPythonScript(
+    wrapper_path = self.createWrapper(
       self.options['wrapper-path'],
-      'slapos.recipe.librecipe.execute.execute',
-      arguments=[self.options['binary-path'].strip(), '-C',
-        self.options['conf-path']],)
+      (self.options['binary-path'].strip(),
+        '-C', self.options['conf-path']))
 
     return [configuration_path, wrapper_path]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/accords/template/accords.ini.in` & `slapos.cookbook-1.0.92/slapos/recipe/accords/template/accords.ini.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/zimbra_kvm/template/kvm_run.in` & `slapos.cookbook-1.0.92/slapos/recipe/zimbra_kvm/template/kvm_run.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/kvm_frontend/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/kvm_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/kvm_frontend/template/kvm-proxy.js` & `slapos.cookbook-1.0.92/slapos/recipe/kvm_frontend/template/kvm-proxy.js`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/mysql/template/my.cnf.in` & `slapos.cookbook-1.0.92/slapos/recipe/generic_mysql/template/my.cnf.in`

 * *Files 17% similar despite different names*

```diff
@@ -5,42 +5,51 @@
 # different engine, like MyISAM. Such behaviour generates problems only, when
 # tables requested as InnoDB are silently created with MyISAM engine.
 #
 # Loud fail is really required in such case.
 sql-mode="NO_ENGINE_SUBSTITUTION"
 
 skip-show-database
-port = %(tcp_port)s
-bind-address = %(ip)s
+%(networking)s
 socket = %(socket)s
 datadir = %(data_directory)s
 pid-file = %(pid_file)s
 log-error = %(error_log)s
-long_query_time = 5
+slow_query_log
+slow_query_log_file = %(slow_query_log)s
+long_query_time = 1
 max_allowed_packet = 128M
-query_cache_size = 32M
-
-plugin-load = ha_mroonga.so
+query_cache_size = 0
+query_cache_type = 0
+innodb_file_per_table = 0
+
+plugin-load = ha_mroonga.so;handlersocket.so
+
+# By default only 100 connections are allowed, when using zeo
+# we may have much more connections
+max_connections = 1000
 
 # The following are important to configure and depend a lot on to the size of
 # your database and the available resources.
 #innodb_buffer_pool_size = 4G
 #innodb_log_file_size = 256M
 #innodb_log_buffer_size = 8M
 
+# very important to allow parallel indexing
+innodb_locks_unsafe_for_binlog = 1
+
 # Some dangerous settings you may want to uncomment if you only want
 # performance or less disk access. Useful for unit tests.
 #innodb_flush_log_at_trx_commit = 0
 #innodb_flush_method = nosync
 #innodb_doublewrite = 0
 #sync_frm = 0
 
-# Uncomment the following if you need binary logging, which is recommended
-# on production instances (either for replication or incremental backups).
-#log-bin=mysql-bin
+%(log_bin)s
+%(expire_logs_days)s
 
 # Force utf8 usage
 collation_server = utf8_unicode_ci
 character_set_server = utf8
 skip-character-set-client-handshake
 
 [mysql]
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/libcloudrequest.py` & `slapos.cookbook-1.0.92/slapos/recipe/libcloudrequest.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/mydumper.py` & `slapos.cookbook-1.0.92/slapos/recipe/mydumper.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 #
 ##############################################################################
-import subprocess
+import os
 
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 
 def _mydumper_base_cmd(mydumper, database, user, password,
                        socket=None, host=None, port=None, **kw):
   cmd = [mydumper]
@@ -54,22 +54,22 @@
     cmd.append('--compress')
 
   if args['rows'] is not None:
     cmd.extend(['-r', args['rows']])
 
   cmd.extend(['-o', args['directory']])
 
-  subprocess.check_call(cmd)
+  os.execv(cmd[0], cmd)
 
 
 def do_import(args):
   cmd = _mydumper_base_cmd(**args)
   cmd.append('--overwrite-tables')
   cmd.extend(['-d', args['directory']])
-  subprocess.check_call(cmd)
+  os.execv(cmd[0], cmd)
 
 
 class Recipe(GenericBaseRecipe):
 
   def install(self):
     config = {
       'database': self.options['database'],
@@ -91,13 +91,9 @@
       config['mydumper'] = self.options['myloader-binary']
     else:
       function = do_export
       config['mydumper'] = self.options['mydumper-binary']
       config['compression'] = self.optionIsTrue('compression', default=False)
       config['rows'] = self.options.get('rows')
 
-    wrapper = self.createPythonScript(name=self.options['wrapper'],
-                                      absolute_function = '%s.%s' % (__name__, function.func_name),
-                                      arguments=config)
-
-    return [wrapper]
-
+    return self.createPythonScript(self.options['wrapper'],
+      '%s.%s' % (function.__module__, function.__name__), (config,))
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/svcdaemon.py` & `slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/svcdaemon.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,18 @@
       self.bin_directory, arguments=[cron_output])[0]
     self.path_list.append(catcher)
     cron_d = os.path.join(self.etc_directory, 'cron.d')
     crontabs = os.path.join(self.etc_directory, 'crontabs')
     self._createDirectory(cron_d)
     self._createDirectory(crontabs)
     wrapper = zc.buildout.easy_install.scripts([('crond',
-      'slapos.recipe.librecipe.execute', 'execute')], self.ws, sys.executable,
-      self.wrapper_directory, arguments=[
+      'slapos.recipe.librecipe.execute', 'generic_exec')], self.ws,
+      sys.executable, self.wrapper_directory, arguments=repr((
         self.options['dcrond_binary'].strip(), '-s', cron_d, '-c', crontabs,
-        '-t', timestamps, '-f', '-l', '5', '-M', catcher]
+        '-t', timestamps, '-f', '-l', '5', '-M', catcher))[1:-1]
       )[0]
     self.path_list.append(wrapper)
     return cron_d
 
   def installZabbixAgentd(self, ip, port, hostname, server_ip,
                           user_parameter_string=''):
     log_file = os.path.join(self.log_directory, 'zabbix_agentd.log')
@@ -97,18 +97,18 @@
       "zabbix_agentd.conf",
       pkg_resources.resource_string(
         __name__, 'template/zabbix_agentd.conf.in') % zabbix_agentd_conf)
 
     self.path_list.append(zabbix_agentd_path)
 
     wrapper = zc.buildout.easy_install.scripts([('zabbixagentd',
-      'slapos.recipe.librecipe.execute', 'execute')], self.ws, sys.executable,
-      self.bin_directory, arguments=[
+      'slapos.recipe.librecipe.execute', 'generic_exec')], self.ws,
+      sys.executable, self.bin_directory, arguments=repr((
         self.options['zabbix_agentd_binary'].strip(), '-c',
-        zabbix_agentd_path])[0]
+        zabbix_agentd_path))[1:-1])[0]
 
     self.path_list.extend(zc.buildout.easy_install.scripts([
       ('zabbixagentd', __name__ + '.svcdaemon', 'svcdaemon')],
       self.ws, sys.executable, self.wrapper_directory, arguments=[dict(
         real_binary=wrapper, pid_file=zabbix_agentd_conf['pid_file'])]))
 
     return zabbix_agentd_conf
```

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/zabbixagent/template/zabbix_agentd.conf.in` & `slapos.cookbook-1.0.92/slapos/recipe/zabbixagent/template/zabbix_agentd.conf.in`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/siptester/__init__.py` & `slapos.cookbook-1.0.92/slapos/recipe/siptester/__init__.py`

 * *Files identical despite different names*

### Comparing `slapos.cookbook-1.0.9/slapos/recipe/wrapper.py` & `slapos.cookbook-1.0.92/slapos/recipe/wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,36 +26,59 @@
 ##############################################################################
 
 import shlex
 
 from slapos.recipe.librecipe import GenericBaseRecipe
 
 class Recipe(GenericBaseRecipe):
+    """Recipe to create a script from given command and options.
+
+    :param str command-line: shell command which launches the intended process
+    :param str wrapper-path: absolute path to file's destination
+
+    :param lines wait-for-files: list of files to wait for
+    :param lines hash-files: list of files to be checked by hash
+    :param str pidfile: path to pidfile ensure exclusivity for the process
+    :param str private-dev-shm: size of private /dev/shm, using user namespaces
+    :param bool reserve-cpu: command will ask for an exclusive CPU core
+    """
     def install(self):
-        command_line = shlex.split(self.options['command-line'])
+        args = shlex.split(self.options['command-line'])
         wrapper_path = self.options['wrapper-path']
         wait_files = self.options.get('wait-for-files')
-        environment = self.options.get('environment')
-        parameters_extra = self.options.get('parameters-extra')
-
-        if not wait_files and not environment:
-          # Create a simple wrapper as shell script
-          return [self.createWrapper(
-             name=wrapper_path,
-             command=command_line[0],
-             parameters=command_line[1:],
-             parameters_extra=parameters_extra,
-          )]
-
-        # More complex needs: create a Python script as wrapper
-
-        if wait_files is not None:
-            wait_files = [filename.strip() for filename in wait_files.split()
-                          if filename.strip()]
-        if environment is not None:
-            environment = dict((k.strip(), v.strip()) for k, v in [
-              line.split('=') for line in environment.splitlines() if line.strip() ])
-        return [self.createPythonScript(
-            wrapper_path,
-            'slapos.recipe.librecipe.execute.generic_exec',
-            (command_line, wait_files, environment,),
-        )]
+        hash_files = self.options.get('hash-files')
+        pidfile = self.options.get('pidfile')
+        private_dev_shm = self.options.get('private-dev-shm')
+
+        environment = {}
+        for line in (self.options.get('environment') or '').splitlines():
+          line = line.strip()
+          if line:
+            k, v = line.split('=')
+            environment[k.rstrip()] = v.lstrip()
+
+        kw = {}
+        if wait_files:
+          kw['wait_list'] = wait_files.split()
+        if pidfile:
+          kw['pidfile'] = pidfile
+        if private_dev_shm:
+          kw['private_dev_shm'] = private_dev_shm
+        if self.isTrueValue(self.options.get('reserve-cpu')):
+          kw['reserve_cpu'] = True
+        if hash_files:
+          hash_file_list = hash_files.split()
+          hash = self.generateHashFromFiles(hash_file_list)
+          wrapper_path = "%s-%s" % (wrapper_path, hash)
+
+        return self.createWrapper(wrapper_path, args, environment, **kw)
+
+    def generateHashFromFiles(self, file_list):
+      import hashlib
+      hasher = hashlib.md5()
+      for path in file_list:
+        with open(path, 'r') as afile:
+          buf = afile.read()
+        hasher.update("%s\n" % len(buf))
+        hasher.update(buf)
+      hash = hasher.hexdigest()
+      return hash
```


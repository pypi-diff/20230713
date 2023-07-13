# Comparing `tmp/service-buddy-too-0.1.58.tar.gz` & `tmp/service-buddy-too-0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service-buddy-too-0.1.58.tar", last modified: Fri May 12 17:54:24 2023, max compression
+gzip compressed data, was "service-buddy-too-0.1.59.tar", last modified: Thu Jul 13 08:31:33 2023, max compression
```

## Comparing `service-buddy-too-0.1.58.tar` & `service-buddy-too-0.1.59.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (123)       68 2023-05-12 17:54:22.000000 service-buddy-too-0.1.58/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.200540 service-buddy-too-0.1.58/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 17:54:22.000000 service-buddy-too-0.1.58/scripts/service-buddy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.200540 service-buddy-too-0.1.58/service_buddy_too/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/ci/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/ci/bamboo_build_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/ci/bitbucket_pipeline_build_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/ci/build_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4311 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/ci/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/ci/travis_build_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/codegenerator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/codegenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/codegenerator/builtin-code-templates.json
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/codegenerator/code_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/codegenerator/cookie_cutter_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2412 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commandline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/commands/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/bootstrap/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/commands/clone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/clone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/clone/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/git/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/commands/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/initialize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/initialize/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/commands/list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/commands/list/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/context/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/context/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/service/application.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2821 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/service/initializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2495 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/service/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/service/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/service/service_template_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/util/command_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/util/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/util/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/service_buddy_too/vcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/vcs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4697 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/vcs/bitbucket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/vcs/github_vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-12 17:53:40.000000 service-buddy-too-0.1.58/service_buddy_too/vcs/vcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:24.200540 service-buddy-too-0.1.58/service_buddy_too.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 17:54:24.000000 service-buddy-too-0.1.58/service_buddy_too.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-12 17:54:24.000000 service-buddy-too-0.1.58/service_buddy_too.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:24.000000 service-buddy-too-0.1.58/service_buddy_too.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:24.000000 service-buddy-too-0.1.58/service_buddy_too.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 17:54:24.000000 service-buddy-too-0.1.58/service_buddy_too.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 17:54:24.000000 service-buddy-too-0.1.58/service_buddy_too.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:22.000000 service-buddy-too-0.1.58/service_buddy_too.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:54:24.204540 service-buddy-too-0.1.58/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2243 2023-05-12 17:54:22.000000 service-buddy-too-0.1.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.188405 service-buddy-too-0.1.59/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (123)       68 2023-07-13 08:31:29.000000 service-buddy-too-0.1.59/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 08:31:33.188405 service-buddy-too-0.1.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.180405 service-buddy-too-0.1.59/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-13 08:31:29.000000 service-buddy-too-0.1.59/scripts/service-buddy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/ci/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/ci/bamboo_build_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/ci/bitbucket_pipeline_build_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/ci/build_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4311 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/ci/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/ci/travis_build_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/codegenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/codegenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/codegenerator/builtin-code-templates.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/codegenerator/code_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/codegenerator/cookie_cutter_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2412 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commandline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/commands/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/bootstrap/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/commands/clone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/clone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/clone/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/git/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/commands/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/initialize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/initialize/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/commands/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/commands/list/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/context/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/context/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/service/application.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2821 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/service/initializer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2495 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/service/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/service/service_template_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/util/command_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/util/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/util/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.188405 service-buddy-too-0.1.59/service_buddy_too/vcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/vcs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4697 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/vcs/bitbucket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/vcs/github_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-13 08:30:33.000000 service-buddy-too-0.1.59/service_buddy_too/vcs/vcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:31:33.184405 service-buddy-too-0.1.59/service_buddy_too.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 08:31:33.000000 service-buddy-too-0.1.59/service_buddy_too.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-13 08:31:33.000000 service-buddy-too-0.1.59/service_buddy_too.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:31:33.000000 service-buddy-too-0.1.59/service_buddy_too.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:31:33.000000 service-buddy-too-0.1.59/service_buddy_too.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 08:31:33.000000 service-buddy-too-0.1.59/service_buddy_too.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 08:31:33.000000 service-buddy-too-0.1.59/service_buddy_too.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:31:29.000000 service-buddy-too-0.1.59/service_buddy_too.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:31:33.188405 service-buddy-too-0.1.59/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-07-13 08:31:29.000000 service-buddy-too-0.1.59/setup.py
```

### Comparing `service-buddy-too-0.1.58/LICENSE` & `service-buddy-too-0.1.59/LICENSE`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/README.md` & `service-buddy-too-0.1.59/README.md`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/ci/bamboo_build_creator.py` & `service-buddy-too-0.1.59/service_buddy_too/ci/bamboo_build_creator.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/ci/bitbucket_pipeline_build_creator.py` & `service-buddy-too-0.1.59/service_buddy_too/ci/bitbucket_pipeline_build_creator.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/ci/build_creator.py` & `service-buddy-too-0.1.59/service_buddy_too/ci/build_creator.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/ci/ci.py` & `service-buddy-too-0.1.59/service_buddy_too/ci/ci.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/ci/travis_build_creator.py` & `service-buddy-too-0.1.59/service_buddy_too/ci/travis_build_creator.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/codegenerator/builtin-code-templates.json` & `service-buddy-too-0.1.59/service_buddy_too/codegenerator/builtin-code-templates.json`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/codegenerator/code_creator.py` & `service-buddy-too-0.1.59/service_buddy_too/codegenerator/code_creator.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/codegenerator/cookie_cutter_creator.py` & `service-buddy-too-0.1.59/service_buddy_too/codegenerator/cookie_cutter_creator.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/commandline.py` & `service-buddy-too-0.1.59/service_buddy_too/commandline.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/commands/bootstrap/command.py` & `service-buddy-too-0.1.59/service_buddy_too/commands/bootstrap/command.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/commands/git/command.py` & `service-buddy-too-0.1.59/service_buddy_too/commands/git/command.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/commands/initialize/command.py` & `service-buddy-too-0.1.59/service_buddy_too/commands/initialize/command.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/commands/list/command.py` & `service-buddy-too-0.1.59/service_buddy_too/commands/list/command.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/context/service_context.py` & `service-buddy-too-0.1.59/service_buddy_too/context/service_context.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/service/initializer.py` & `service-buddy-too-0.1.59/service_buddy_too/service/initializer.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/service/loader.py` & `service-buddy-too-0.1.59/service_buddy_too/service/loader.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/service/service.py` & `service-buddy-too-0.1.59/service_buddy_too/service/service.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/service/service_template_generator.py` & `service-buddy-too-0.1.59/service_buddy_too/service/service_template_generator.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/util/command_util.py` & `service-buddy-too-0.1.59/service_buddy_too/util/command_util.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/util/log_handler.py` & `service-buddy-too-0.1.59/service_buddy_too/util/log_handler.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/util/pretty_printer.py` & `service-buddy-too-0.1.59/service_buddy_too/util/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/vcs/bitbucket.py` & `service-buddy-too-0.1.59/service_buddy_too/vcs/bitbucket.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/vcs/github_vcs.py` & `service-buddy-too-0.1.59/service_buddy_too/vcs/github_vcs.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too/vcs/vcs.py` & `service-buddy-too-0.1.59/service_buddy_too/vcs/vcs.py`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/service_buddy_too.egg-info/SOURCES.txt` & `service-buddy-too-0.1.59/service_buddy_too.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `service-buddy-too-0.1.58/setup.py` & `service-buddy-too-0.1.59/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'service-buddy-too',
-        version = '0.1.58',
+        version = '0.1.59',
         description = 'CLI for managing micro-services',
         long_description = 'CLI for managing micro-services',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
@@ -62,15 +62,15 @@
         entry_points = {},
         data_files = [],
         package_data = {
             'service_buddy_too': ['codegenerator/builtin-code-templates.json']
         },
         install_requires = [
             'PyGithub',
-            'cookiecutter',
+            'cookiecutter==2.1.1',
             'click',
             'infra-buddy-too',
             'requests',
             'atlassian-python-api'
         ],
         dependency_links = [],
         zip_safe = True,
```


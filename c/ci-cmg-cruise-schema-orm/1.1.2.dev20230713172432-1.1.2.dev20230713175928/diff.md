# Comparing `tmp/ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432.tar.gz` & `tmp/ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432.tar", last modified: Thu Jul 13 17:24:36 2023, max compression
+gzip compressed data, was "ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928.tar", last modified: Thu Jul 13 17:59:32 2023, max compression
```

## Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432.tar` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:24:36.327818 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/
--rw-r--r--   0 max        (501) staff       (20)     1065 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/LICENSE
--rw-r--r--   0 max        (501) staff       (20)       24 2023-03-03 14:59:28.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/MANIFEST.in
--rw-r--r--   0 max        (501) staff       (20)     1931 2023-07-13 17:24:36.327649 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     1282 2023-01-19 20:19:31.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/README.md
--rw-r--r--   0 max        (501) staff       (20)       67 2023-01-23 16:31:30.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/requirements.txt
--rw-r--r--   0 max        (501) staff       (20)       38 2023-07-13 17:24:36.327863 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      888 2023-07-13 17:24:35.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:24:36.309594 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:24:36.312729 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     1931 2023-07-13 17:24:36.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     2078 2023-07-13 17:24:36.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-07-13 17:24:36.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       38 2023-07-13 17:24:36.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       19 2023-07-13 17:24:36.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/top_level.txt
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:24:36.313007 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/
--rw-r--r--   0 max        (501) staff       (20)        0 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/__init__.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:24:36.325612 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/
--rw-r--r--   0 max        (501) staff       (20)        0 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/__init__.py
--rw-r--r--   0 max        (501) staff       (20)      833 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/access_path.py
--rw-r--r--   0 max        (501) staff       (20)     4084 2023-01-20 19:30:23.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/contact.py
--rw-r--r--   0 max        (501) staff       (20)     3382 2023-07-12 22:06:06.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset.py
--rw-r--r--   0 max        (501) staff       (20)      766 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_instrument_mapping.py
--rw-r--r--   0 max        (501) staff       (20)     2458 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_parameter.py
--rw-r--r--   0 max        (501) staff       (20)      742 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_platform_mapping.py
--rw-r--r--   0 max        (501) staff       (20)      728 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_project_mapping.py
--rw-r--r--   0 max        (501) staff       (20)      728 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_scientist_mapping.py
--rw-r--r--   0 max        (501) staff       (20)      704 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_shape_mapping.py
--rw-r--r--   0 max        (501) staff       (20)      950 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_source_mapping.py
--rw-r--r--   0 max        (501) staff       (20)      718 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_survey_mapping.py
--rw-r--r--   0 max        (501) staff       (20)      865 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_type.py
--rw-r--r--   0 max        (501) staff       (20)     3975 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file.py
--rw-r--r--   0 max        (501) staff       (20)      734 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_access_path_mapping.py
--rw-r--r--   0 max        (501) staff       (20)     1116 2023-01-30 18:11:50.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_format.py
--rw-r--r--   0 max        (501) staff       (20)     2417 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_parameter.py
--rw-r--r--   0 max        (501) staff       (20)      667 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_shape_mapping.py
--rw-r--r--   0 max        (501) staff       (20)      888 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_type.py
--rw-r--r--   0 max        (501) staff       (20)     1230 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/instrument.py
--rw-r--r--   0 max        (501) staff       (20)     1971 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/parameter_detail.py
--rw-r--r--   0 max        (501) staff       (20)     1950 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/platform.py
--rw-r--r--   0 max        (501) staff       (20)      599 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/project.py
--rw-r--r--   0 max        (501) staff       (20)     2459 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/project_parameter.py
--rw-r--r--   0 max        (501) staff       (20)     1227 2023-01-19 18:31:22.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/shape.py
--rw-r--r--   0 max        (501) staff       (20)     3018 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/survey.py
--rw-r--r--   0 max        (501) staff       (20)     2445 2023-07-12 22:06:31.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/survey_parameter.py
--rw-r--r--   0 max        (501) staff       (20)      692 2023-01-19 03:25:06.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/survey_shape_mapping.py
--rw-r--r--   0 max        (501) staff       (20)     1260 2023-01-20 19:48:48.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/version_description.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:24:36.327407 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/
--rw-r--r--   0 max        (501) staff       (20)        0 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/__init__.py
--rw-r--r--   0 max        (501) staff       (20)      525 2023-07-13 14:41:37.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/column_consts.py
--rw-r--r--   0 max        (501) staff       (20)     1058 2023-03-13 18:04:20.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/cx_oracle.py
--rw-r--r--   0 max        (501) staff       (20)     9953 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/entity.py
--rw-r--r--   0 max        (501) staff       (20)     1266 2023-01-07 22:09:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/jdbc.py
--rw-r--r--   0 max        (501) staff       (20)     4097 2023-02-09 15:10:00.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/persistence.py
--rw-r--r--   0 max        (501) staff       (20)     5672 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/query.py
--rw-r--r--   0 max        (501) staff       (20)      227 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/query_pair.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:59:32.668943 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/
+-rw-r--r--   0 max        (501) staff       (20)     1065 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)       24 2023-03-03 14:59:28.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/MANIFEST.in
+-rw-r--r--   0 max        (501) staff       (20)     1931 2023-07-13 17:59:32.668800 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     1282 2023-01-19 20:19:31.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/README.md
+-rw-r--r--   0 max        (501) staff       (20)       67 2023-01-23 16:31:30.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-07-13 17:59:32.668986 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      888 2023-07-13 17:59:31.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:59:32.658404 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:59:32.659785 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     1931 2023-07-13 17:59:32.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     2078 2023-07-13 17:59:32.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-07-13 17:59:32.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-07-13 17:59:32.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       19 2023-07-13 17:59:32.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:59:32.659901 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/
+-rw-r--r--   0 max        (501) staff       (20)        0 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/__init__.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:59:32.667079 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/
+-rw-r--r--   0 max        (501) staff       (20)        0 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)      833 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/access_path.py
+-rw-r--r--   0 max        (501) staff       (20)     4084 2023-01-20 19:30:23.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/contact.py
+-rw-r--r--   0 max        (501) staff       (20)     3382 2023-07-12 22:06:06.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset.py
+-rw-r--r--   0 max        (501) staff       (20)      766 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_instrument_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)     2458 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_parameter.py
+-rw-r--r--   0 max        (501) staff       (20)      742 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_platform_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)      728 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_project_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)      728 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_scientist_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)      704 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_shape_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)      950 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_source_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)      718 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_survey_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)      865 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_type.py
+-rw-r--r--   0 max        (501) staff       (20)     3975 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file.py
+-rw-r--r--   0 max        (501) staff       (20)      734 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_access_path_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)     1116 2023-01-30 18:11:50.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_format.py
+-rw-r--r--   0 max        (501) staff       (20)     2417 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_parameter.py
+-rw-r--r--   0 max        (501) staff       (20)      667 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_shape_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)      888 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_type.py
+-rw-r--r--   0 max        (501) staff       (20)     1230 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/instrument.py
+-rw-r--r--   0 max        (501) staff       (20)     1971 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/parameter_detail.py
+-rw-r--r--   0 max        (501) staff       (20)     1950 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/platform.py
+-rw-r--r--   0 max        (501) staff       (20)      599 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/project.py
+-rw-r--r--   0 max        (501) staff       (20)     2459 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/project_parameter.py
+-rw-r--r--   0 max        (501) staff       (20)     1227 2023-01-19 18:31:22.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/shape.py
+-rw-r--r--   0 max        (501) staff       (20)     3018 2023-07-12 22:06:43.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/survey.py
+-rw-r--r--   0 max        (501) staff       (20)     2445 2023-07-12 22:06:31.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/survey_parameter.py
+-rw-r--r--   0 max        (501) staff       (20)      692 2023-01-19 03:25:06.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/survey_shape_mapping.py
+-rw-r--r--   0 max        (501) staff       (20)     1260 2023-01-20 19:48:48.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/version_description.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-13 17:59:32.668614 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/
+-rw-r--r--   0 max        (501) staff       (20)        0 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)      525 2023-07-13 14:41:37.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/column_consts.py
+-rw-r--r--   0 max        (501) staff       (20)     1058 2023-03-13 18:04:20.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/cx_oracle.py
+-rw-r--r--   0 max        (501) staff       (20)     9953 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/entity.py
+-rw-r--r--   0 max        (501) staff       (20)     1266 2023-01-07 22:09:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/jdbc.py
+-rw-r--r--   0 max        (501) staff       (20)     4097 2023-02-09 15:10:00.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/persistence.py
+-rw-r--r--   0 max        (501) staff       (20)     5672 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/query.py
+-rw-r--r--   0 max        (501) staff       (20)      227 2022-11-10 16:04:34.000000 ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/query_pair.py
```

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/LICENSE` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/LICENSE`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/PKG-INFO` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ci-cmg-cruise-schema-orm
-Version: 1.1.2.dev20230713172432
+Version: 1.1.2.dev20230713175928
 Summary: ORM classes for the cruise schema
 Home-page: https://github.com/ci-cmg/cruise-schema-orm-py
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/README.md` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/README.md`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/setup.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ci-cmg-cruise-schema-orm",
-  version="1.1.2.dev20230713172432",
+  version="1.1.2.dev20230713175928",
   description="ORM classes for the cruise schema",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/cruise-schema-orm-py",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/PKG-INFO` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ci-cmg-cruise-schema-orm
-Version: 1.1.2.dev20230713172432
+Version: 1.1.2.dev20230713175928
 Summary: ORM classes for the cruise schema
 Home-page: https://github.com/ci-cmg/cruise-schema-orm-py
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ci_cmg_cruise_schema_orm.egg-info/SOURCES.txt` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ci_cmg_cruise_schema_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/access_path.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/access_path.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/contact.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_instrument_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_instrument_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_parameter.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_parameter.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_platform_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_platform_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_project_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_project_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_scientist_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_scientist_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_shape_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_shape_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_source_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_source_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_survey_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_survey_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/dataset_type.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/dataset_type.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_access_path_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_access_path_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_format.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_format.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_parameter.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_parameter.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_shape_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_shape_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/file_type.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/file_type.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/instrument.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/instrument.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/parameter_detail.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/parameter_detail.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/platform.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/platform.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/project.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/project.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/project_parameter.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/project_parameter.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/shape.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/shape.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/survey.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/survey.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/survey_parameter.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/survey_parameter.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/survey_shape_mapping.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/survey_shape_mapping.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/entity/version_description.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/entity/version_description.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/column_consts.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/column_consts.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/cx_oracle.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/cx_oracle.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/entity.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/entity.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/jdbc.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/jdbc.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/persistence.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/persistence.py`

 * *Files identical despite different names*

### Comparing `ci-cmg-cruise-schema-orm-1.1.2.dev20230713172432/src/ncei_cruise_schema/orm/query.py` & `ci-cmg-cruise-schema-orm-1.1.2.dev20230713175928/src/ncei_cruise_schema/orm/query.py`

 * *Files identical despite different names*


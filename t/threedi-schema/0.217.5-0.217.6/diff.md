# Comparing `tmp/threedi-schema-0.217.5.tar.gz` & `tmp/threedi-schema-0.217.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.217.5.tar", last modified: Thu Jun 15 13:50:15 2023, max compression
+gzip compressed data, was "threedi-schema-0.217.6.tar", last modified: Thu Jul 13 07:49:58 2023, max compression
```

## Comparing `threedi-schema-0.217.5.tar` & `threedi-schema-0.217.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.746772 threedi-schema-0.217.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-15 13:50:15.746772 threedi-schema-0.217.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-15 13:50:15.746772 threedi-schema-0.217.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.738772 threedi-schema-0.217.5/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.738772 threedi-schema-0.217.5/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.742772 threedi-schema-0.217.5/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.742772 threedi-schema-0.217.5/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.742772 threedi-schema-0.217.5/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.742772 threedi-schema-0.217.5/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.746772 threedi-schema-0.217.5/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.746772 threedi-schema-0.217.5/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-15 13:50:06.000000 threedi-schema-0.217.5/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:50:15.738772 threedi-schema-0.217.5/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-15 13:50:15.000000 threedi-schema-0.217.5/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-15 13:50:15.000000 threedi-schema-0.217.5/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:50:15.000000 threedi-schema-0.217.5/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 13:50:15.000000 threedi-schema-0.217.5/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:50:15.000000 threedi-schema-0.217.5/threedi_schema.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 13:50:15.000000 threedi-schema-0.217.5/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 13:50:15.000000 threedi-schema-0.217.5/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.382753 threedi-schema-0.217.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-13 07:49:58.382753 threedi-schema-0.217.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 07:49:58.382753 threedi-schema-0.217.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.374753 threedi-schema-0.217.6/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.378753 threedi-schema-0.217.6/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.378753 threedi-schema-0.217.6/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.378753 threedi-schema-0.217.6/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.378753 threedi-schema-0.217.6/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.382753 threedi-schema-0.217.6/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.382753 threedi-schema-0.217.6/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.382753 threedi-schema-0.217.6/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:45.000000 threedi-schema-0.217.6/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-13 07:49:46.000000 threedi-schema-0.217.6/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-13 07:49:46.000000 threedi-schema-0.217.6/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-13 07:49:46.000000 threedi-schema-0.217.6/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-13 07:49:46.000000 threedi-schema-0.217.6/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:49:58.374753 threedi-schema-0.217.6/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-13 07:49:58.000000 threedi-schema-0.217.6/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-13 07:49:58.000000 threedi-schema-0.217.6/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:49:58.000000 threedi-schema-0.217.6/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 07:49:58.000000 threedi-schema-0.217.6/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:49:58.000000 threedi-schema-0.217.6/threedi_schema.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 07:49:58.000000 threedi-schema-0.217.6/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 07:49:58.000000 threedi-schema-0.217.6/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.217.5/CHANGES.rst` & `threedi-schema-0.217.6/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog of threedi-schema
 ===================================================
 
+0.217.6 (2023-07-13)
+--------------------
+
+- Extend FrictionType enum with Chézy friction with conveyance and
+  Manning friction with conveyance.
+
+
 0.217.5 (2023-06-15)
 --------------------
 
 - Fixed set_views (spatialite metadata tables wwere not updated).
 
 
 0.217.4 (2023-06-15)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `threedi-schema-0.217.5/LICENSE` & `threedi-schema-0.217.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/PKG-INFO` & `threedi-schema-0.217.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.217.5
+Version: 0.217.6
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,21 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.6 (2023-07-13)
+--------------------
+
+- Extend FrictionType enum with Chézy friction with conveyance and
+  Manning friction with conveyance.
+
+
 0.217.5 (2023-06-15)
 --------------------
 
 - Fixed set_views (spatialite metadata tables wwere not updated).
 
 
 0.217.4 (2023-06-15)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `threedi-schema-0.217.5/README.rst` & `threedi-schema-0.217.6/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/setup.py` & `threedi-schema-0.217.6/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/application/schema.py` & `threedi-schema-0.217.6/threedi_schema/application/schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/application/threedi_database.py` & `threedi-schema-0.217.6/threedi_schema/application/threedi_database.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/beta_features.py` & `threedi-schema-0.217.6/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/domain/constants.py` & `threedi-schema-0.217.6/threedi_schema/domain/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
     TABULATED_YZ = 7
     INVERTED_EGG = 8
 
 
 class FrictionType(Enum):
     CHEZY = 1
     MANNING = 2
+    CHEZY_CONVEYANCE = 3
+    MANNING_CONVEYANCE = 4
 
 
 class InitializationType(Enum):
     MAX = 0
     MIN = 1
     AVERAGE = 2
```

### Comparing `threedi-schema-0.217.5/threedi_schema/domain/custom_types.py` & `threedi-schema-0.217.6/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/domain/indexes.py` & `threedi-schema-0.217.6/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/domain/models.py` & `threedi-schema-0.217.6/threedi_schema/domain/models.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/domain/views.py` & `threedi-schema-0.217.6/threedi_schema/domain/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/infrastructure/spatial_index.py` & `threedi-schema-0.217.6/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/infrastructure/spatialite_versions.py` & `threedi-schema-0.217.6/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/infrastructure/views.py` & `threedi-schema-0.217.6/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/env.py` & `threedi-schema-0.217.6/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0200_initial.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi-schema-0.217.6/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/scripts.py` & `threedi-schema-0.217.6/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/tests/conftest.py` & `threedi-schema-0.217.6/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/tests/test_migration_213.py` & `threedi-schema-0.217.6/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/tests/test_schema.py` & `threedi-schema-0.217.6/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema/tests/test_spatalite_versions.py` & `threedi-schema-0.217.6/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.5/threedi_schema.egg-info/PKG-INFO` & `threedi-schema-0.217.6/threedi_schema.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.217.5
+Version: 0.217.6
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,21 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.6 (2023-07-13)
+--------------------
+
+- Extend FrictionType enum with Chézy friction with conveyance and
+  Manning friction with conveyance.
+
+
 0.217.5 (2023-06-15)
 --------------------
 
 - Fixed set_views (spatialite metadata tables wwere not updated).
 
 
 0.217.4 (2023-06-15)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `threedi-schema-0.217.5/threedi_schema.egg-info/SOURCES.txt` & `threedi-schema-0.217.6/threedi_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

